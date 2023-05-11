# Comparing `tmp/geofileops-0.8.0a4.tar.gz` & `tmp/geofileops-0.8.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofileops-0.8.0a4.tar", last modified: Wed May 10 09:08:33 2023, max compression
+gzip compressed data, was "geofileops-0.8.0a5.tar", last modified: Thu May 11 10:19:31 2023, max compression
```

## Comparing `geofileops-0.8.0a4.tar` & `geofileops-0.8.0a5.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmark_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmark_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/benchmark/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarks/benchmarks_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/benchmarks/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/benchmark/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/geofileops/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    84479 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)    91013 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/geoops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.949225 geofileops-0.8.0a4/geofileops/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/helpers/_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/helpers/layerstyles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.949225 geofileops-0.8.0a4/geofileops/util/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    71319 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_geoops_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)   101634 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geodataframe_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geofiletypes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30024 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/util/test.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/geofileops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.945224 geofileops-0.8.0a4/geofileops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 09:08:33.000000 geofileops-0.8.0a4/geofileops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.953225 geofileops-0.8.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:33.961224 geofileops-0.8.0a4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/BEFL-kbl.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/geofileops_testdata.qgz
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/linestring-row-trees.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/linestring-watercourse.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/linestrings_hedges.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/point.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-invalid.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-no-rows.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-all.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-one.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-two+three.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-parcel.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-simplify-onborder-testcase.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-twolayers.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygon-zone.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygonstyle.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/data/polygonstyle.sld
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38647 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_singlelayer_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofileops_twolayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_spatialite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-10 09:08:18.000000 geofileops-0.8.0a4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.817957 geofileops-0.8.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-11 10:19:31.817957 geofileops-0.8.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.805957 geofileops-0.8.0a5/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/benchmark_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/benchmark_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/benchmarker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.805957 geofileops-0.8.0a5/benchmark/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/benchmarks/benchmarks_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/benchmarks/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/benchmark/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.805957 geofileops-0.8.0a5/geofileops/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84479 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96065 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/geoops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.809957 geofileops-0.8.0a5/geofileops/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/helpers/_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/helpers/layerstyles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.809957 geofileops-0.8.0a5/geofileops/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72763 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_geoops_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107339 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22065 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/geodataframe_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/geofiletypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30024 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/util/test.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/geofileops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.809957 geofileops-0.8.0a5/geofileops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-11 10:19:31.000000 geofileops-0.8.0a5/geofileops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-11 10:19:31.000000 geofileops-0.8.0a5/geofileops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:19:31.000000 geofileops-0.8.0a5/geofileops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 10:19:31.000000 geofileops-0.8.0a5/geofileops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 10:19:31.000000 geofileops-0.8.0a5/geofileops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 10:19:31.817957 geofileops-0.8.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.813957 geofileops-0.8.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:19:31.817957 geofileops-0.8.0a5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/BEFL-kbl.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/geofileops_testdata.qgz
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/linestring-row-trees.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/linestring-watercourse.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/linestrings_hedges.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/point.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-invalid.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-no-rows.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-overlappingcircles-all.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-overlappingcircles-one.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-overlappingcircles-two+three.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-parcel.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-simplify-onborder-testcase.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-twolayers.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygon-zone.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygonstyle.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/data/polygonstyle.sld
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18119 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geofileops_singlelayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38315 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geofileops_singlelayer_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geofileops_singlelayer_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geofileops_singlelayer_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40218 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geofileops_twolayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_spatialite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-11 10:19:19.000000 geofileops-0.8.0a5/tests/test_version.py
```

### Comparing `geofileops-0.8.0a4/LICENSE.txt` & `geofileops-0.8.0a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/PKG-INFO` & `geofileops-0.8.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a4
+Version: 0.8.0a5
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a4/README.md` & `geofileops-0.8.0a5/README.md`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/benchmark/benchmarker.py` & `geofileops-0.8.0a5/benchmark/benchmarker.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/benchmark/benchmarks/benchmarks_geofileops.py` & `geofileops-0.8.0a5/benchmark/benchmarks/benchmarks_geofileops.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from geofileops.util import _geoops_gpd
 
 ################################################################################
 # Some init
 ################################################################################
 
 logger = logging.getLogger(__name__)
+nb_parallel = min(multiprocessing.cpu_count(), 12)
 
 ################################################################################
 # The real work
 ################################################################################
 
 
 def _get_package() -> str:
@@ -40,43 +41,76 @@
 def buffer(tmp_dir: Path) -> RunResult:
     # Init
     input_path = testdata.TestFile.AGRIPRC_2018.get_file(tmp_dir)
 
     # Go!
     start_time = datetime.now()
     output_path = tmp_dir / f"{input_path.stem}_buf.gpkg"
-    gfo.buffer(input_path, output_path, distance=1, force=True)
+    gfo.buffer(input_path, output_path, distance=1, nb_parallel=nb_parallel, force=True)
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="buffer",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr="buffer on agri parcel layer BEFL (~500.000 polygons)",
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     output_path.unlink()
     return result
 
 
 def buffer_spatialite(tmp_dir: Path) -> RunResult:
     # Init
     input_path = testdata.TestFile.AGRIPRC_2018.get_file(tmp_dir)
 
     # Go!
     start_time = datetime.now()
     output_path = tmp_dir / f"{input_path.stem}_buf_spatialite.gpkg"
-    _geoops_sql.buffer(input_path, output_path, distance=1, force=True)
+    _geoops_sql.buffer(
+        input_path, output_path, distance=1, nb_parallel=nb_parallel, force=True
+    )
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="buffer_spatialite",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr="buffer on agri parcel layer BEFL (~500.000 polygons)",
+        run_details={"nb_cpu": nb_parallel},
+    )
+
+    # Cleanup and return
+    output_path.unlink()
+    return result
+
+
+def buffer_gridsize_spatialite(tmp_dir: Path) -> RunResult:
+    # Init
+    input_path = testdata.TestFile.AGRIPRC_2018.get_file(tmp_dir)
+
+    # Go!
+    start_time = datetime.now()
+    output_path = tmp_dir / f"{input_path.stem}_buf_grid01_spatialite.gpkg"
+    _geoops_sql.buffer(
+        input_path,
+        output_path,
+        distance=1,
+        gridsize=0.1,
+        nb_parallel=nb_parallel,
+        force=True,
+    )
+    result = RunResult(
+        package=_get_package(),
+        package_version=_get_version(),
+        operation="buffer_gridsize_spatialite",
+        secs_taken=(datetime.now() - start_time).total_seconds(),
+        operation_descr=(
+            "buffer with gridsize 0.1 on agri parcel layer BEFL (~500.000 polygons)"
+        ),
         run_details={"nb_cpu": multiprocessing.cpu_count()},
     )
 
     # Cleanup and return
     output_path.unlink()
     return result
 
@@ -84,22 +118,24 @@
 def buffer_gpd(tmp_dir: Path) -> RunResult:
     # Init
     input_path = testdata.TestFile.AGRIPRC_2018.get_file(tmp_dir)
 
     # Go!
     start_time = datetime.now()
     output_path = tmp_dir / f"{input_path.stem}_buf_gpd.gpkg"
-    _geoops_gpd.buffer(input_path, output_path, distance=1, force=True)
+    _geoops_gpd.buffer(
+        input_path, output_path, distance=1, nb_parallel=nb_parallel, force=True
+    )
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="buffer_gpd",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr="buffer on agri parcel layer BEFL (~500.000 polygons)",
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     output_path.unlink()
     return result
 
 
@@ -110,23 +146,24 @@
     # Go!
     start_time = datetime.now()
     output_path = tmp_dir / f"{input_path.stem}_diss_nogroupby.gpkg"
     gfo.dissolve(
         input_path=input_path,
         output_path=output_path,
         explodecollections=True,
+        nb_parallel=nb_parallel,
         force=True,
     )
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="dissolve",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr="dissolve on agri parcels BEFL (~500.000 polygons)",
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     output_path.unlink()
     return result
 
 
@@ -138,25 +175,26 @@
     start_time = datetime.now()
     output_path = tmp_dir / f"{input_path.stem}_diss_groupby.gpkg"
     gfo.dissolve(
         input_path,
         output_path,
         groupby_columns=["GEWASGROEP"],
         explodecollections=True,
+        nb_parallel=nb_parallel,
         force=True,
     )
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="dissolve_groupby",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr=(
             "dissolve on agri parcels BEFL (~500.000 polygons), groupby=[GEWASGROEP]"
         ),
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     output_path.unlink()
     return result
 
 
@@ -168,23 +206,24 @@
     # Go!
     start_time = datetime.now()
     output_path = tmp_dir / f"{input1_path.stem}_clip_{input2_path.stem}.gpkg"
     gfo.clip(
         input_path=input1_path,
         clip_path=input2_path,
         output_path=output_path,
+        nb_parallel=nb_parallel,
         force=True,
     )
     result = RunResult(
         package="geofileops",
         package_version=gfo.__version__,
         operation="clip",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr="clip between 2 agri parcel layers BEFL (2*~500.000 polygons)",
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     # output_path.unlink()
     return result
 
 
@@ -196,25 +235,59 @@
     # Go!
     start_time = datetime.now()
     output_path = tmp_dir / f"{input1_path.stem}_inters_{input2_path.stem}.gpkg"
     gfo.intersection(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
+        nb_parallel=nb_parallel,
         force=True,
     )
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="intersection",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr=(
             "intersection between 2 agri parcel layers BEFL (2*~500.000 polygons)"
         ),
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
+    )
+
+    # Cleanup and return
+    output_path.unlink()
+    return result
+
+
+def _intersection_gridsize(tmp_dir: Path) -> RunResult:
+    # Init
+    input1_path = testdata.TestFile.AGRIPRC_2018.get_file(tmp_dir)
+    input2_path = testdata.TestFile.AGRIPRC_2019.get_file(tmp_dir)
+
+    # Go!
+    start_time = datetime.now()
+    output_path = tmp_dir / f"{input1_path.stem}_inters_grid01_{input2_path.stem}.gpkg"
+    gfo.intersection(
+        input1_path=input1_path,
+        input2_path=input2_path,
+        output_path=output_path,
+        gridsize=0.1,
+        nb_parallel=nb_parallel,
+        force=True,
+    )
+    result = RunResult(
+        package=_get_package(),
+        package_version=_get_version(),
+        operation="intersection_gridsize",
+        secs_taken=(datetime.now() - start_time).total_seconds(),
+        operation_descr=(
+            "intersection with gridsize 0.1 between 2 agri parcel layers BEFL "
+            "(2*~500.000 polygons)"
+        ),
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     output_path.unlink()
     return result
 
 
@@ -243,26 +316,27 @@
         / f"{input1_path.stem}_join_inters_{input2_path.stem}_{_get_package()}.gpkg"
     )
     gfo.join_by_location(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
         spatial_relations_query="intersects is True",
+        nb_parallel=nb_parallel,
         force=True,
     )
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="join_by_location_intersects",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr=(
             "join_by_location_intersects between 2 agri parcel layers BEFL "
             "(2*~500.000 polygons)"
         ),
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     logger.info(f"nb features in result: {gfo.get_layerinfo(output_path).featurecount}")
     output_path.unlink()
     return result
 
@@ -275,21 +349,22 @@
     # Go!
     start_time = datetime.now()
     output_path = tmp_dir / f"{input1_path.stem}_inters_{input2_path.stem}.gpkg"
     gfo.union(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
+        nb_parallel=nb_parallel,
         force=True,
     )
     result = RunResult(
         package=_get_package(),
         package_version=_get_version(),
         operation="union",
         secs_taken=(datetime.now() - start_time).total_seconds(),
         operation_descr="union between 2 agri parcel layers BEFL (2*~500.000 polygons)",
-        run_details={"nb_cpu": multiprocessing.cpu_count()},
+        run_details={"nb_cpu": nb_parallel},
     )
 
     # Cleanup and return
     output_path.unlink()
     return result
```

### Comparing `geofileops-0.8.0a4/benchmark/benchmarks/testdata.py` & `geofileops-0.8.0a5/benchmark/benchmarks/testdata.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/benchmark/reporter.py` & `geofileops-0.8.0a5/benchmark/reporter.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/__init__.py` & `geofileops-0.8.0a5/geofileops/__init__.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/fileops.py` & `geofileops-0.8.0a5/geofileops/fileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/geoops.py` & `geofileops-0.8.0a5/geofileops/geoops.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     func: Callable[[Any], Any],
     only_geom_input: bool = True,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
     force_output_geometrytype: Union[GeometryType, str, None] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Apply a python lambda function on the geometry column of the input file.
 
@@ -75,14 +76,17 @@
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to output only simple geometries.
             Defaults to False.
         force_output_geometrytype (GeometryType, optional): The output geometry type to
             force. If None, a best-effort guess is made and will always result in a
             multi-type. Defaults to None.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -95,14 +99,15 @@
         func=func,
         only_geom_input=only_geom_input,
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def buffer(
@@ -114,14 +119,15 @@
     join_style: BufferJoinStyle = BufferJoinStyle.ROUND,
     mitre_limit: float = 5.0,
     single_sided: bool = False,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Applies a buffer operation on geometry column of the input file.
 
@@ -162,14 +168,17 @@
             file only contains one layer.
         columns (List[str], optional): list of columns to retain. If None, all standard
             columns are retained. In addition to standard columns, it is also possible
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to output only simple geometries.
             Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -269,14 +278,15 @@
             output_path=Path(output_path),
             distance=distance,
             quadrantsegments=quadrantsegments,
             input_layer=input_layer,
             output_layer=output_layer,
             columns=columns,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
         )
     else:
         # If special buffer options, use geopandas version
         return _geoops_gpd.buffer(
@@ -288,14 +298,15 @@
             join_style=join_style,
             mitre_limit=mitre_limit,
             single_sided=single_sided,
             input_layer=input_layer,
             output_layer=output_layer,
             columns=columns,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
         )
 
 
 def clip_by_geometry(
@@ -322,15 +333,15 @@
             file only contains one layer.
         columns (List[str], optional): list of columns to retain. If None, all standard
             columns are retained. In addition to standard columns, it is also possible
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to output only simple geometries.
             Defaults to False.
-       force (bool, optional): overwrite existing output file(s).
+        force (bool, optional): overwrite existing output file(s).
             Defaults to False.
     """
     return _geoops_ogr.clip_by_geometry(
         input_path=Path(input_path),
         output_path=Path(output_path),
         clip_geometry=clip_geometry,
         input_layer=input_layer,
@@ -344,14 +355,15 @@
 def convexhull(
     input_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Applies a convexhull operation on the input file.
 
@@ -366,14 +378,17 @@
             file only contains one layer.
         columns (List[str], optional): list of columns to retain. If None, all standard
             columns are retained. In addition to standard columns, it is also possible
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to output only simple geometries.
             Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -383,27 +398,29 @@
     return _geoops_sql.convexhull(
         input_path=Path(input_path),
         output_path=Path(output_path),
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def delete_duplicate_geometries(
     input_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     force: bool = False,
 ):
     """
     Copy all rows to the output file, except for duplicate geometries.
 
     Args:
         input_path (PathLike): the input file
@@ -414,39 +431,44 @@
             file only contains one layer.
         columns (List[str], optional): list of columns to retain. If None, all standard
             columns are retained. In addition to standard columns, it is also possible
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to output only simple geometries.
             Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         force (bool, optional): overwrite existing output file(s).
             Defaults to False.
     """
     logger.info(f"Start delete_duplicate_geometries on {input_path}")
     return _geoops_sql.delete_duplicate_geometries(
         input_path=Path(input_path),
         output_path=Path(output_path),
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         force=force,
     )
 
 
 def dissolve(
     input_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     explodecollections: bool,
     groupby_columns: Union[List[str], str, None] = None,
     agg_columns: Optional[dict] = None,
     tiles_path: Union[str, "os.PathLike[Any]", None] = None,
     nb_squarish_tiles: int = 1,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Applies a dissolve operation on the input file.
 
@@ -563,14 +585,17 @@
             Can be used to evade huge geometries being created if the input
             geometries are very interconnected.
             Defaults to 1 (= the output is not tiled).
         input_layer (str, optional): input layer name. Optional if the
             file only contains one layer.
         output_layer (str, optional): input layer name. Optional if the
             file only contains one layer.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -596,14 +621,15 @@
         explodecollections=explodecollections,
         groupby_columns=groupby_columns,
         agg_columns=agg_columns,
         tiles_path=tiles_path,
         nb_squarish_tiles=nb_squarish_tiles,
         input_layer=input_layer,
         output_layer=output_layer,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def export_by_bounds(
@@ -726,15 +752,15 @@
     input_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
     force_output_geometrytype: Optional[GeometryType] = None,
-    gridsize: Optional[float] = None,
+    gridsize: float = 0.0,
     precision: Optional[float] = None,
     validate_attribute_data: bool = False,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
@@ -757,32 +783,34 @@
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to output only simple geometries.
             Defaults to False.
         force_output_geometrytype (GeometryType, optional): The output geometry type to
             force the output to. If None, the geometry type of the input is used.
             Defaults to None.
-        gridsize (float, optional): the size of the grid the coordinates will be rounded
-            to. Eg. 0.001 to keep 3 decimals. None doesn't change the precision.
-            Defaults to None.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         validate_attribute_data (bool, optional): True to validate if all attribute data
             can be read. Raises an exception if an error is found, as this type of error
             cannot be fixed using makevalid. Defaults to False.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
             Defaults to False.
     """
 
     logger.info(f"Start makevalid on {input_path}")
-    if precision is not None and gridsize is not None:
+    if gridsize is None:
+        gridsize = 0.0
+    if precision is not None and gridsize != 0.0:
         raise ValueError(
             "the precision parameter is deprecated and cannot be combined with gridsize"
         )
     if precision is not None:
         gridsize = precision
         warnings.warn(
             "the precision parameter is deprecated and will be removed in a future "
@@ -871,14 +899,15 @@
     sql_stmt: str,
     sql_dialect: Optional[Literal["SQLITE", "OGRSQL"]] = "SQLITE",
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
     force_output_geometrytype: Union[GeometryType, str, None] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = 1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Execute an SQL query on the file.
 
@@ -949,14 +978,17 @@
             columns are retained. In addition to standard columns, it is also possible
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
         force_output_geometrytype (GeometryType, optional): The output geometry type to
             force. Defaults to None, and then the geometry type of the input is used
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to 1. If nb_parallel != 1, make sure your query still returns
             correct results if it is executed per batch of rows instead of in one go
             on the entire layer. To use all available cores, pass -1.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage. If batchsize != -1,
@@ -977,14 +1009,15 @@
         sql_stmt=sql_stmt,
         sql_dialect=sql_dialect,
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def simplify(
@@ -993,14 +1026,15 @@
     tolerance: float,
     algorithm: SimplifyAlgorithm = SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
     lookahead: int = 8,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Applies a simplify operation on geometry column of the input file.
 
@@ -1026,14 +1060,17 @@
             file only contains one layer.
         columns (List[str], optional): list of columns to retain. If None, all standard
             columns are retained. In addition to standard columns, it is also possible
             to specify "fid", a unique index available in all input files. Note that the
             "fid" will be aliased eg. to "fid_1". Defaults to None.
         explodecollections (bool, optional): True to output only simple geometries.
             Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1045,14 +1082,15 @@
             input_path=Path(input_path),
             output_path=Path(output_path),
             tolerance=tolerance,
             input_layer=input_layer,
             output_layer=output_layer,
             columns=columns,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
         )
     else:
         return _geoops_gpd.simplify(
             input_path=Path(input_path),
@@ -1060,14 +1098,15 @@
             tolerance=tolerance,
             algorithm=algorithm,
             lookahead=lookahead,
             input_layer=input_layer,
             output_layer=output_layer,
             columns=columns,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
         )
 
 
 ################################################################################
@@ -1080,14 +1119,15 @@
     clip_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     input_layer: Optional[str] = None,
     input_columns: Optional[List[str]] = None,
     clip_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Clip the input layer with the clip layer.
 
@@ -1124,14 +1164,17 @@
             that the "fid" will be aliased eg. to "fid_1". Defaults to None.
         clip_layer (str, optional): clip layer name. Optional if the
             file only contains one layer.
         output_layer (str, optional): output layer name. Optional if the
             file only contains one layer.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1149,14 +1192,15 @@
         clip_path=Path(clip_path),
         output_path=Path(output_path),
         input_layer=input_layer,
         input_columns=input_columns,
         clip_layer=clip_layer,
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def erase(
@@ -1164,14 +1208,15 @@
     erase_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     input_layer: Optional[str] = None,
     input_columns: Optional[List[str]] = None,
     erase_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Erase all geometries in the erase layer from the input layer.
 
@@ -1195,14 +1240,17 @@
             that the "fid" will be aliased eg. to "fid_1". Defaults to None.
         erase_layer (str, optional): erase layer name. Optional if the
             file only contains one layer.
         output_layer (str, optional): output layer name. Optional if the
             file only contains one layer.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1215,14 +1263,15 @@
         erase_path=Path(erase_path),
         output_path=Path(output_path),
         input_layer=input_layer,
         input_columns=input_columns,
         erase_layer=erase_layer,
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def export_by_location(
@@ -1231,14 +1280,15 @@
     output_path: Union[str, "os.PathLike[Any]"],
     min_area_intersect: Optional[float] = None,
     area_inters_column_name: Optional[str] = "area_inters",
     input1_layer: Optional[str] = None,
     input1_columns: Optional[List[str]] = None,
     input2_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Exports all features in input_to_select_from_path that intersect with any
     features in input_to_compare_with_path.
@@ -1261,14 +1311,17 @@
             possible to specify "fid", a unique index available in all input files. Note
             that the "fid" will be aliased eg. to "fid_1". Defaults to None.
         input2_layer (str, optional): input layer name. Optional if the
             file only contains one layer.
         input2_columns (List[str], optional): NA.
         output_layer (str, optional): output layer name. Optional if the
             file only contains one layer.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1284,14 +1337,15 @@
         output_path=Path(output_path),
         min_area_intersect=min_area_intersect,
         area_inters_column_name=area_inters_column_name,
         input_layer=input1_layer,
         input_columns=input1_columns,
         input_to_compare_with_layer=input2_layer,
         output_layer=output_layer,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def export_by_distance(
@@ -1299,14 +1353,15 @@
     input_to_compare_with_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     max_distance: float,
     input1_layer: Optional[str] = None,
     input1_columns: Optional[List[str]] = None,
     input2_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Exports all features in input_to_select_from_path that are within the
     distance specified of any features in input_to_compare_with_path.
@@ -1322,14 +1377,17 @@
             standard columns are retained. In addition to standard columns, it is also
             possible to specify "fid", a unique index available in all input files. Note
             that the "fid" will be aliased eg. to "fid_1". Defaults to None.
         input2_layer (str, optional): input layer name. Optional if the
             file only contains one layer.
         output_layer (str, optional): output layer name. Optional if the
             file only contains one layer.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1345,14 +1403,15 @@
         input_to_compare_with_path=Path(input_to_compare_with_path),
         output_path=Path(output_path),
         max_distance=max_distance,
         input1_layer=input1_layer,
         input1_columns=input1_columns,
         input2_layer=input2_layer,
         output_layer=output_layer,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def intersect(
@@ -1363,14 +1422,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     warnings.warn(
         "intersect() is deprecated because it was renamed intersection(). "
         "Will be removed in a future version",
@@ -1384,14 +1444,15 @@
         input1_columns=input1_columns,
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def intersection(
@@ -1402,14 +1463,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Calculate the pairwise intersection of alle features in input1 with all
     features in input2.
@@ -1437,14 +1499,17 @@
             possible to specify "fid". Defaults to None.
         input2_columns_prefix (str, optional): prefix to use in the column aliases.
             Defaults to "l2_".
         output_layer (str, optional): output layer name. If None, the output_path stem
             is used. Defaults to None.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1461,14 +1526,15 @@
         input1_columns=input1_columns,
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def join_by_location(
@@ -1482,14 +1548,15 @@
     input1_layer: Optional[str] = None,
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Joins all features in input1 with all features in input2.
 
@@ -1543,14 +1610,17 @@
         input2_columns (List[str], optional): columns to select. If None is specified,
             all columns are selected. As explained for input1_columns, it is also
             possible to specify "fid". Defaults to None.
         input2_columns_prefix (str, optional): prefix to use in the column aliases.
             Defaults to "l2_".
         output_layer (str, optional): output layer name. If None, the output_path stem
             is used. Defaults to None.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1572,14 +1642,15 @@
         input1_columns=input1_columns,
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=False,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def join_nearest(
@@ -1590,14 +1661,15 @@
     input1_layer: Optional[str] = None,
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Joins features in input1 with the nb_nearest features that are closest to
     them in input2.
@@ -1622,14 +1694,17 @@
         input2_columns (List[str], optional): columns to select. If None is specified,
             all columns are selected. As explained for input1_columns, it is also
             possible to specify "fid". Defaults to None.
         input2_columns_prefix (str, optional): prefix to use in the column aliases.
             Defaults to "l2_".
         output_layer (str, optional): output layer name. If None, the output_path stem
             is used. Defaults to None.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1648,14 +1723,15 @@
         input1_columns=input1_columns,
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=False,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def select_two_layers(
@@ -1668,14 +1744,15 @@
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
     force_output_geometrytype: Optional[GeometryType] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = 1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Executes the sqlite query specified on the 2 input layers specified.
 
@@ -1775,14 +1852,17 @@
         output_layer (str, optional): output layer name. If None, the output_path stem
             is used. Defaults to None.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
         force_output_geometrytype (GeometryType, optional): The output geometry
             type to force. Defaults to None, and then the geometry type of the
             input1 layer is used.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1838,14 +1918,15 @@
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def symmetric_difference(
@@ -1856,14 +1937,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Calculates the "symmetric difference" of the two input layers.
 
@@ -1891,14 +1973,17 @@
             possible to specify "fid". Defaults to None.
         input2_columns_prefix (str, optional): prefix to use in the column aliases.
             Defaults to "l2_".
         output_layer (str, optional): output layer name. If None, the output_path stem
             is used. Defaults to None.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduc
             e the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
@@ -1917,14 +2002,15 @@
         input1_columns=input1_columns,
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def split(
@@ -1935,14 +2021,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Split the features in input1 with all features in input2.
 
@@ -1973,14 +2060,17 @@
             possible to specify "fid". Defaults to None.
         input2_columns_prefix (str, optional): prefix to use in the column aliases.
             Defaults to "l2_".
         output_layer (str, optional): output layer name. If None, the output_path stem
             is used. Defaults to None.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -1995,14 +2085,15 @@
         input1_columns=input1_columns,
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def union(
@@ -2013,14 +2104,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     """
     Calculates the pairwise "union" of the two input layers.
 
@@ -2047,14 +2139,17 @@
             possible to specify "fid". Defaults to None.
         input2_columns_prefix (str, optional): prefix to use in the column aliases.
             Defaults to "l2_".
         output_layer (str, optional): output layer name. If None, the output_path stem
             is used. Defaults to None.
         explodecollections (bool, optional): True to convert all multi-geometries to
             singular ones after the dissolve. Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): the number of parallel processes to use.
             Defaults to -1: use all available processors.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): overwrite existing output file(s).
@@ -2071,11 +2166,12 @@
         input1_columns=input1_columns,
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
```

### Comparing `geofileops-0.8.0a4/geofileops/helpers/_parameter_helper.py` & `geofileops-0.8.0a5/geofileops/helpers/_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/helpers/layerstyles.py` & `geofileops-0.8.0a5/geofileops/helpers/layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/_general_util.py` & `geofileops-0.8.0a5/geofileops/util/_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/_geoops_gpd.py` & `geofileops-0.8.0a5/geofileops/util/_geoops_gpd.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,4432 +27,4522 @@
 000001a0: 6564 5475 706c 652c 0a20 2020 204f 7074  edTuple,.    Opt
 000001b0: 696f 6e61 6c2c 0a20 2020 2054 7570 6c65  ional,.    Tuple
 000001c0: 2c0a 2020 2020 556e 696f 6e2c 0a29 0a69  ,.    Union,.).i
 000001d0: 6d70 6f72 7420 7761 726e 696e 6773 0a0a  mport warnings..
 000001e0: 696d 706f 7274 2063 6c6f 7564 7069 636b  import cloudpick
 000001f0: 6c65 0a69 6d70 6f72 7420 6765 6f70 616e  le.import geopan
 00000200: 6461 7320 6173 2067 7064 0a69 6d70 6f72  das as gpd.impor
-00000210: 7420 6e75 6d70 7920 6173 206e 700a 696d  t numpy as np.im
-00000220: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-00000230: 640a 696d 706f 7274 2070 7375 7469 6c0a  d.import psutil.
-00000240: 696d 706f 7274 2073 6861 7065 6c79 2e67  import shapely.g
-00000250: 656f 6d65 7472 7920 6173 2073 685f 6765  eometry as sh_ge
-00000260: 6f6d 0a0a 696d 706f 7274 2067 656f 6669  om..import geofi
-00000270: 6c65 6f70 7320 6173 2067 666f 0a66 726f  leops as gfo.fro
-00000280: 6d20 6765 6f66 696c 656f 7073 2069 6d70  m geofileops imp
-00000290: 6f72 7420 6669 6c65 6f70 730a 6672 6f6d  ort fileops.from
-000002a0: 2067 656f 6669 6c65 6f70 732e 7574 696c   geofileops.util
-000002b0: 2069 6d70 6f72 7420 5f67 656e 6572 616c   import _general
-000002c0: 5f75 7469 6c0a 6672 6f6d 2067 656f 6669  _util.from geofi
-000002d0: 6c65 6f70 732e 7574 696c 2069 6d70 6f72  leops.util impor
-000002e0: 7420 5f67 656f 6f70 735f 7371 6c0a 6672  t _geoops_sql.fr
-000002f0: 6f6d 2067 656f 6669 6c65 6f70 732e 7574  om geofileops.ut
-00000300: 696c 2069 6d70 6f72 7420 5f69 6f5f 7574  il import _io_ut
-00000310: 696c 0a66 726f 6d20 6765 6f66 696c 656f  il.from geofileo
-00000320: 7073 2e68 656c 7065 7273 2069 6d70 6f72  ps.helpers impor
-00000330: 7420 5f70 6172 616d 6574 6572 5f68 656c  t _parameter_hel
-00000340: 7065 720a 6672 6f6d 2067 656f 6669 6c65  per.from geofile
-00000350: 6f70 732e 7574 696c 2069 6d70 6f72 7420  ops.util import 
-00000360: 5f70 726f 6365 7373 696e 675f 7574 696c  _processing_util
-00000370: 0a66 726f 6d20 6765 6f66 696c 656f 7073  .from geofileops
-00000380: 2e75 7469 6c2e 6765 6f6d 6574 7279 5f75  .util.geometry_u
-00000390: 7469 6c20 696d 706f 7274 2047 656f 6d65  til import Geome
-000003a0: 7472 7954 7970 652c 2050 7269 6d69 7469  tryType, Primiti
-000003b0: 7665 5479 7065 2c20 5369 6d70 6c69 6679  veType, Simplify
-000003c0: 416c 676f 7269 7468 6d0a 6672 6f6d 2067  Algorithm.from g
-000003d0: 656f 6669 6c65 6f70 732e 7574 696c 2e67  eofileops.util.g
-000003e0: 656f 6d65 7472 795f 7574 696c 2069 6d70  eometry_util imp
-000003f0: 6f72 7420 4275 6666 6572 456e 6443 6170  ort BufferEndCap
-00000400: 5374 796c 652c 2042 7566 6665 724a 6f69  Style, BufferJoi
-00000410: 6e53 7479 6c65 0a66 726f 6d20 6765 6f66  nStyle.from geof
-00000420: 696c 656f 7073 2e75 7469 6c20 696d 706f  ileops.util impo
-00000430: 7274 2067 656f 7365 7269 6573 5f75 7469  rt geoseries_uti
-00000440: 6c0a 6672 6f6d 2067 656f 6669 6c65 6f70  l.from geofileop
-00000450: 732e 7574 696c 2069 6d70 6f72 7420 6772  s.util import gr
-00000460: 6964 5f75 7469 6c0a 0a23 2323 2323 2323  id_util..#######
-00000470: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000004a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000004b0: 2323 2323 2323 2323 230a 2320 536f 6d65  #########.# Some
-000004c0: 2069 6e69 740a 2323 2323 2323 2323 2323   init.##########
-000004d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000004e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000004f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000510: 2323 2323 2323 0a0a 2320 446f 6e27 7420  ######..# Don't 
-00000520: 7368 6f77 2074 6869 7320 6765 6f70 616e  show this geopan
-00000530: 6461 7320 7761 726e 696e 672e 2e2e 0a77  das warning....w
-00000540: 6172 6e69 6e67 732e 6669 6c74 6572 7761  arnings.filterwa
-00000550: 726e 696e 6773 2822 6967 6e6f 7265 222c  rnings("ignore",
-00000560: 2022 4765 6f53 6572 6965 732e 6973 6e61   "GeoSeries.isna
-00000570: 222c 2055 7365 7257 6172 6e69 6e67 290a  ", UserWarning).
-00000580: 0a6c 6f67 6765 7220 3d20 6c6f 6767 696e  .logger = loggin
-00000590: 672e 6765 744c 6f67 6765 7228 5f5f 6e61  g.getLogger(__na
-000005a0: 6d65 5f5f 290a 0a23 2323 2323 2323 2323  me__)..#########
-000005b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000005c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000005d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000005e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000005f0: 2323 2323 2323 230a 2320 536f 6d65 2068  #######.# Some h
-00000600: 656c 7065 7220 6675 6e63 7469 6f6e 730a  elper functions.
-00000610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000210: 7420 6765 6f70 616e 6461 732e 5f63 6f6d  t geopandas._com
+00000220: 7061 7420 6173 2067 7064 5f63 6f6d 7061  pat as gpd_compa
+00000230: 740a 696d 706f 7274 206e 756d 7079 2061  t.import numpy a
+00000240: 7320 6e70 0a69 6d70 6f72 7420 7061 6e64  s np.import pand
+00000250: 6173 2061 7320 7064 0a69 6d70 6f72 7420  as as pd.import 
+00000260: 7073 7574 696c 0a0a 6966 2067 7064 5f63  psutil..if gpd_c
+00000270: 6f6d 7061 742e 5553 455f 5059 4745 4f53  ompat.USE_PYGEOS
+00000280: 3a0a 2020 2020 696d 706f 7274 2070 7967  :.    import pyg
+00000290: 656f 7320 6173 2073 6861 7065 6c79 325f  eos as shapely2_
+000002a0: 6f72 5f70 7967 656f 730a 656c 7365 3a0a  or_pygeos.else:.
+000002b0: 2020 2020 696d 706f 7274 2073 6861 7065      import shape
+000002c0: 6c79 2061 7320 7368 6170 656c 7932 5f6f  ly as shapely2_o
+000002d0: 725f 7079 6765 6f73 0a69 6d70 6f72 7420  r_pygeos.import 
+000002e0: 7368 6170 656c 792e 6765 6f6d 6574 7279  shapely.geometry
+000002f0: 2061 7320 7368 5f67 656f 6d0a 0a69 6d70   as sh_geom..imp
+00000300: 6f72 7420 6765 6f66 696c 656f 7073 2061  ort geofileops a
+00000310: 7320 6766 6f0a 6672 6f6d 2067 656f 6669  s gfo.from geofi
+00000320: 6c65 6f70 7320 696d 706f 7274 2066 696c  leops import fil
+00000330: 656f 7073 0a66 726f 6d20 6765 6f66 696c  eops.from geofil
+00000340: 656f 7073 2e75 7469 6c20 696d 706f 7274  eops.util import
+00000350: 205f 6765 6e65 7261 6c5f 7574 696c 0a66   _general_util.f
+00000360: 726f 6d20 6765 6f66 696c 656f 7073 2e75  rom geofileops.u
+00000370: 7469 6c20 696d 706f 7274 205f 6765 6f6f  til import _geoo
+00000380: 7073 5f73 716c 0a66 726f 6d20 6765 6f66  ps_sql.from geof
+00000390: 696c 656f 7073 2e75 7469 6c20 696d 706f  ileops.util impo
+000003a0: 7274 205f 696f 5f75 7469 6c0a 6672 6f6d  rt _io_util.from
+000003b0: 2067 656f 6669 6c65 6f70 732e 6865 6c70   geofileops.help
+000003c0: 6572 7320 696d 706f 7274 205f 7061 7261  ers import _para
+000003d0: 6d65 7465 725f 6865 6c70 6572 0a66 726f  meter_helper.fro
+000003e0: 6d20 6765 6f66 696c 656f 7073 2e75 7469  m geofileops.uti
+000003f0: 6c20 696d 706f 7274 205f 7072 6f63 6573  l import _proces
+00000400: 7369 6e67 5f75 7469 6c0a 6672 6f6d 2067  sing_util.from g
+00000410: 656f 6669 6c65 6f70 732e 7574 696c 2e67  eofileops.util.g
+00000420: 656f 6d65 7472 795f 7574 696c 2069 6d70  eometry_util imp
+00000430: 6f72 7420 4765 6f6d 6574 7279 5479 7065  ort GeometryType
+00000440: 2c20 5072 696d 6974 6976 6554 7970 652c  , PrimitiveType,
+00000450: 2053 696d 706c 6966 7941 6c67 6f72 6974   SimplifyAlgorit
+00000460: 686d 0a66 726f 6d20 6765 6f66 696c 656f  hm.from geofileo
+00000470: 7073 2e75 7469 6c2e 6765 6f6d 6574 7279  ps.util.geometry
+00000480: 5f75 7469 6c20 696d 706f 7274 2042 7566  _util import Buf
+00000490: 6665 7245 6e64 4361 7053 7479 6c65 2c20  ferEndCapStyle, 
+000004a0: 4275 6666 6572 4a6f 696e 5374 796c 650a  BufferJoinStyle.
+000004b0: 6672 6f6d 2067 656f 6669 6c65 6f70 732e  from geofileops.
+000004c0: 7574 696c 2069 6d70 6f72 7420 6765 6f73  util import geos
+000004d0: 6572 6965 735f 7574 696c 0a66 726f 6d20  eries_util.from 
+000004e0: 6765 6f66 696c 656f 7073 2e75 7469 6c20  geofileops.util 
+000004f0: 696d 706f 7274 2067 7269 645f 7574 696c  import grid_util
+00000500: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00000510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000550: 2323 0a23 2053 6f6d 6520 696e 6974 0a23  ##.# Some init.#
+00000560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000570: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000580: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000590: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000005a0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+000005b0: 0a23 2044 6f6e 2774 2073 686f 7720 7468  .# Don't show th
+000005c0: 6973 2067 656f 7061 6e64 6173 2077 6172  is geopandas war
+000005d0: 6e69 6e67 2e2e 2e0a 7761 726e 696e 6773  ning....warnings
+000005e0: 2e66 696c 7465 7277 6172 6e69 6e67 7328  .filterwarnings(
+000005f0: 2269 676e 6f72 6522 2c20 2247 656f 5365  "ignore", "GeoSe
+00000600: 7269 6573 2e69 736e 6122 2c20 5573 6572  ries.isna", User
+00000610: 5761 726e 696e 6729 0a0a 6c6f 6767 6572  Warning)..logger
+00000620: 203d 206c 6f67 6769 6e67 2e67 6574 4c6f   = logging.getLo
+00000630: 6767 6572 285f 5f6e 616d 655f 5f29 0a0a  gger(__name__)..
 00000640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000660: 0a0a 0a63 6c61 7373 2050 6172 616c 6c65  ...class Paralle
-00000670: 6c69 7a61 7469 6f6e 436f 6e66 6967 3a0a  lizationConfig:.
-00000680: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000690: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000006a0: 2020 2020 2020 2020 6279 7465 735f 6261          bytes_ba
-000006b0: 7365 666f 6f74 7072 696e 743a 2069 6e74  sefootprint: int
-000006c0: 203d 2035 3020 2a20 3130 3234 202a 2031   = 50 * 1024 * 1
-000006d0: 3032 342c 0a20 2020 2020 2020 2062 7974  024,.        byt
-000006e0: 6573 5f70 6572 5f72 6f77 3a20 696e 7420  es_per_row: int 
-000006f0: 3d20 3130 302c 0a20 2020 2020 2020 206d  = 100,.        m
-00000700: 696e 5f61 7667 5f72 6f77 735f 7065 725f  in_avg_rows_per_
-00000710: 6261 7463 683a 2069 6e74 203d 2031 3030  batch: int = 100
-00000720: 302c 0a20 2020 2020 2020 206d 6178 5f61  0,.        max_a
-00000730: 7667 5f72 6f77 735f 7065 725f 6261 7463  vg_rows_per_batc
-00000740: 683a 2069 6e74 203d 2031 3030 3030 2c0a  h: int = 10000,.
-00000750: 2020 2020 2020 2020 6279 7465 735f 6d69          bytes_mi
-00000760: 6e5f 7065 725f 7072 6f63 6573 733d 4e6f  n_per_process=No
-00000770: 6e65 2c0a 2020 2020 2020 2020 6279 7465  ne,.        byte
-00000780: 735f 7573 6162 6c65 3d4e 6f6e 652c 0a20  s_usable=None,. 
-00000790: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-000007a0: 6c66 2e62 7974 6573 5f62 6173 6566 6f6f  lf.bytes_basefoo
-000007b0: 7470 7269 6e74 203d 2062 7974 6573 5f62  tprint = bytes_b
-000007c0: 6173 6566 6f6f 7470 7269 6e74 0a20 2020  asefootprint.   
-000007d0: 2020 2020 2073 656c 662e 6279 7465 735f       self.bytes_
-000007e0: 7065 725f 726f 7720 3d20 6279 7465 735f  per_row = bytes_
-000007f0: 7065 725f 726f 770a 2020 2020 2020 2020  per_row.        
-00000800: 7365 6c66 2e6d 696e 5f61 7667 5f72 6f77  self.min_avg_row
-00000810: 735f 7065 725f 6261 7463 6820 3d20 6d69  s_per_batch = mi
-00000820: 6e5f 6176 675f 726f 7773 5f70 6572 5f62  n_avg_rows_per_b
-00000830: 6174 6368 0a20 2020 2020 2020 2073 656c  atch.        sel
-00000840: 662e 6d61 785f 6176 675f 726f 7773 5f70  f.max_avg_rows_p
-00000850: 6572 5f62 6174 6368 203d 206d 6178 5f61  er_batch = max_a
-00000860: 7667 5f72 6f77 735f 7065 725f 6261 7463  vg_rows_per_batc
-00000870: 680a 2020 2020 2020 2020 6966 2062 7974  h.        if byt
-00000880: 6573 5f6d 696e 5f70 6572 5f70 726f 6365  es_min_per_proce
-00000890: 7373 2069 7320 4e6f 6e65 3a0a 2020 2020  ss is None:.    
-000008a0: 2020 2020 2020 2020 7365 6c66 2e62 7974          self.byt
-000008b0: 6573 5f6d 696e 5f70 6572 5f70 726f 6365  es_min_per_proce
-000008c0: 7373 203d 2028 0a20 2020 2020 2020 2020  ss = (.         
-000008d0: 2020 2020 2020 2062 7974 6573 5f62 6173         bytes_bas
-000008e0: 6566 6f6f 7470 7269 6e74 202b 2062 7974  efootprint + byt
-000008f0: 6573 5f70 6572 5f72 6f77 202a 206d 696e  es_per_row * min
-00000900: 5f61 7667 5f72 6f77 735f 7065 725f 6261  _avg_rows_per_ba
-00000910: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
-00000920: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00000930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000940: 2e62 7974 6573 5f6d 696e 5f70 6572 5f70  .bytes_min_per_p
-00000950: 726f 6365 7373 203d 2062 7974 6573 5f6d  rocess = bytes_m
-00000960: 696e 5f70 6572 5f70 726f 6365 7373 0a20  in_per_process. 
-00000970: 2020 2020 2020 2069 6620 6279 7465 735f         if bytes_
-00000980: 7573 6162 6c65 2069 7320 4e6f 6e65 3a0a  usable is None:.
-00000990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000009a0: 2e62 7974 6573 5f75 7361 626c 6520 3d20  .bytes_usable = 
-000009b0: 7073 7574 696c 2e76 6972 7475 616c 5f6d  psutil.virtual_m
-000009c0: 656d 6f72 7928 292e 6176 6169 6c61 626c  emory().availabl
-000009d0: 6520 2a20 302e 390a 2020 2020 2020 2020  e * 0.9.        
-000009e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000009f0: 2020 7365 6c66 2e62 7974 6573 5f75 7361    self.bytes_usa
-00000a00: 626c 6520 3d20 6279 7465 735f 7573 6162  ble = bytes_usab
-00000a10: 6c65 0a0a 0a70 6172 616c 6c65 6c69 7a61  le...paralleliza
-00000a20: 7469 6f6e 5061 7261 6d73 203d 204e 616d  tionParams = Nam
-00000a30: 6564 5475 706c 6528 0a20 2020 2022 7265  edTuple(.    "re
-00000a40: 7375 6c74 222c 0a20 2020 205b 2822 6e62  sult",.    [("nb
-00000a50: 5f70 6172 616c 6c65 6c22 2c20 696e 7429  _parallel", int)
-00000a60: 2c20 2822 6e62 5f62 6174 6368 6573 5f72  , ("nb_batches_r
-00000a70: 6563 6f6d 6d65 6e64 6564 222c 2069 6e74  ecommended", int
-00000a80: 292c 2028 226e 625f 726f 7773 5f70 6572  ), ("nb_rows_per
-00000a90: 5f62 6174 6368 222c 2069 6e74 295d 2c0a  _batch", int)],.
-00000aa0: 290a 0a0a 6465 6620 6765 745f 7061 7261  )...def get_para
-00000ab0: 6c6c 656c 697a 6174 696f 6e5f 7061 7261  llelization_para
-00000ac0: 6d73 280a 2020 2020 6e62 5f72 6f77 735f  ms(.    nb_rows_
-00000ad0: 746f 7461 6c3a 2069 6e74 2c0a 2020 2020  total: int,.    
-00000ae0: 6e62 5f70 6172 616c 6c65 6c3a 2069 6e74  nb_parallel: int
-00000af0: 203d 202d 312c 0a20 2020 206e 625f 6261   = -1,.    nb_ba
-00000b00: 7463 6865 735f 7072 6576 696f 7573 5f70  tches_previous_p
-00000b10: 6173 733a 204f 7074 696f 6e61 6c5b 696e  ass: Optional[in
-00000b20: 745d 203d 204e 6f6e 652c 0a20 2020 2070  t] = None,.    p
-00000b30: 6172 616c 6c65 6c69 7a61 7469 6f6e 5f63  arallelization_c
-00000b40: 6f6e 6669 673a 204f 7074 696f 6e61 6c5b  onfig: Optional[
-00000b50: 5061 7261 6c6c 656c 697a 6174 696f 6e43  ParallelizationC
-00000b60: 6f6e 6669 675d 203d 204e 6f6e 652c 0a29  onfig] = None,.)
-00000b70: 202d 3e20 7061 7261 6c6c 656c 697a 6174   -> parallelizat
-00000b80: 696f 6e50 6172 616d 733a 0a20 2020 2022  ionParams:.    "
-00000b90: 2222 0a20 2020 2044 6574 6572 6d69 6e65  "".    Determine
-00000ba0: 7320 7265 636f 6d6d 656e 6465 6420 7061  s recommended pa
-00000bb0: 7261 6c6c 656c 697a 6174 696f 6e20 7061  rallelization pa
-00000bc0: 7261 6d73 2e0a 0a20 2020 2041 7267 733a  rams...    Args:
-00000bd0: 0a20 2020 2020 2020 206e 625f 726f 7773  .        nb_rows
-00000be0: 5f74 6f74 616c 2028 696e 7429 3a20 5468  _total (int): Th
-00000bf0: 6520 746f 7461 6c20 6e75 6d62 6572 206f  e total number o
-00000c00: 6620 726f 7773 2074 6861 7420 7769 6c6c  f rows that will
-00000c10: 2062 6520 7072 6f63 6573 7365 640a 2020   be processed.  
-00000c20: 2020 2020 2020 6e62 5f70 6172 616c 6c65        nb_paralle
-00000c30: 6c20 2869 6e74 2c20 6f70 7469 6f6e 616c  l (int, optional
-00000c40: 293a 2054 6865 206c 6576 656c 206f 6620  ): The level of 
-00000c50: 7061 7261 6c6c 656c 697a 6174 696f 6e20  parallelization 
-00000c60: 7265 7175 6573 7465 642e 0a20 2020 2020  requested..     
-00000c70: 2020 2020 2020 2049 6620 2d31 2c20 7472         If -1, tr
-00000c80: 6965 7320 746f 2075 7365 2061 6c6c 2072  ies to use all r
-00000c90: 6573 6f75 7263 6573 2061 7661 696c 6162  esources availab
-00000ca0: 6c65 2e20 4465 6661 756c 7473 2074 6f20  le. Defaults to 
-00000cb0: 2d31 2e0a 2020 2020 2020 2020 6e62 5f62  -1..        nb_b
-00000cc0: 6174 6368 6573 5f70 7265 7669 6f75 735f  atches_previous_
-00000cd0: 7061 7373 2028 696e 742c 206f 7074 696f  pass (int, optio
-00000ce0: 6e61 6c29 3a20 4966 2061 7070 6c69 6361  nal): If applica
-00000cf0: 626c 652c 2074 6865 206e 756d 6265 7220  ble, the number 
-00000d00: 6f66 2062 6174 6368 6573 0a20 2020 2020  of batches.     
-00000d10: 2020 2020 2020 2075 7365 6420 696e 2061         used in a
-00000d20: 2070 7265 7669 6f75 7320 7061 7373 206f   previous pass o
-00000d30: 6620 7468 6520 6361 6c63 756c 6174 696f  f the calculatio
-00000d40: 6e2e 2044 6566 6175 6c74 7320 746f 204e  n. Defaults to N
-00000d50: 6f6e 652e 0a0a 2020 2020 5265 7475 726e  one...    Return
-00000d60: 733a 0a20 2020 2020 2020 2070 6172 616c  s:.        paral
-00000d70: 6c65 6c69 7a61 7469 6f6e 5061 7261 6d73  lelizationParams
-00000d80: 3a20 5468 6520 7265 636f 6d6d 656e 6465  : The recommende
-00000d90: 6420 7061 7261 6d65 7465 7273 2e0a 2020  d parameters..  
-00000da0: 2020 2222 220a 2020 2020 2320 496e 6974    """.    # Init
-00000db0: 2070 6172 616c 6c65 6c69 7a61 7469 6f6e   parallelization
-00000dc0: 2063 6f6e 6669 670a 0a20 2020 2023 2049   config..    # I
-00000dd0: 6620 636f 6e66 6967 2069 7320 4e6f 6e65  f config is None
-00000de0: 2c20 7365 7420 746f 2065 6d70 7479 2064  , set to empty d
-00000df0: 6963 740a 2020 2020 6966 2070 6172 616c  ict.    if paral
-00000e00: 6c65 6c69 7a61 7469 6f6e 5f63 6f6e 6669  lelization_confi
-00000e10: 6720 6973 206e 6f74 204e 6f6e 653a 0a20  g is not None:. 
-00000e20: 2020 2020 2020 2070 6172 616c 6c65 6c69         paralleli
-00000e30: 7a61 7469 6f6e 5f63 6f6e 6669 675f 6c6f  zation_config_lo
-00000e40: 6361 6c20 3d20 7061 7261 6c6c 656c 697a  cal = paralleliz
-00000e50: 6174 696f 6e5f 636f 6e66 6967 0a20 2020  ation_config.   
-00000e60: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
-00000e70: 6172 616c 6c65 6c69 7a61 7469 6f6e 5f63  arallelization_c
-00000e80: 6f6e 6669 675f 6c6f 6361 6c20 3d20 5061  onfig_local = Pa
-00000e90: 7261 6c6c 656c 697a 6174 696f 6e43 6f6e  rallelizationCon
-00000ea0: 6669 6728 290a 0a20 2020 2023 2049 6620  fig()..    # If 
-00000eb0: 7468 6520 6e75 6d62 6572 206f 6620 726f  the number of ro
-00000ec0: 7773 2069 7320 7265 616c 6c79 206c 6f77  ws is really low
-00000ed0: 2c20 6a75 7374 2075 7365 206f 6e65 2062  , just use one b
-00000ee0: 6174 6368 0a20 2020 2023 2054 4f44 4f3a  atch.    # TODO:
-00000ef0: 2066 6f72 2076 6572 7920 636f 6d70 6c65   for very comple
-00000f00: 7820 6665 6174 7572 6573 2c20 706f 7373  x features, poss
-00000f10: 6962 6c79 2074 6869 7320 6c69 6d69 7420  ibly this limit 
-00000f20: 6973 206e 6f74 2061 2067 6f6f 6420 6964  is not a good id
-00000f30: 6561 0a20 2020 2069 6620 6e62 5f72 6f77  ea.    if nb_row
-00000f40: 735f 746f 7461 6c20 3c20 7061 7261 6c6c  s_total < parall
-00000f50: 656c 697a 6174 696f 6e5f 636f 6e66 6967  elization_config
-00000f60: 5f6c 6f63 616c 2e6d 696e 5f61 7667 5f72  _local.min_avg_r
-00000f70: 6f77 735f 7065 725f 6261 7463 683a 0a20  ows_per_batch:. 
-00000f80: 2020 2020 2020 2072 6574 7572 6e20 7061         return pa
-00000f90: 7261 6c6c 656c 697a 6174 696f 6e50 6172  rallelizationPar
-00000fa0: 616d 7328 312c 2031 2c20 6e62 5f72 6f77  ams(1, 1, nb_row
-00000fb0: 735f 746f 7461 6c29 0a0a 2020 2020 6966  s_total)..    if
-00000fc0: 206e 625f 7061 7261 6c6c 656c 203d 3d20   nb_parallel == 
-00000fd0: 2d31 3a0a 2020 2020 2020 2020 6e62 5f70  -1:.        nb_p
-00000fe0: 6172 616c 6c65 6c20 3d20 6d75 6c74 6970  arallel = multip
-00000ff0: 726f 6365 7373 696e 672e 6370 755f 636f  rocessing.cpu_co
-00001000: 756e 7428 290a 0a20 2020 206d 656d 5f75  unt()..    mem_u
-00001010: 7361 626c 6520 3d20 5f67 656e 6572 616c  sable = _general
-00001020: 5f75 7469 6c2e 666f 726d 6174 6279 7465  _util.formatbyte
-00001030: 7328 7061 7261 6c6c 656c 697a 6174 696f  s(parallelizatio
-00001040: 6e5f 636f 6e66 6967 5f6c 6f63 616c 2e62  n_config_local.b
-00001050: 7974 6573 5f75 7361 626c 6529 0a20 2020  ytes_usable).   
-00001060: 206c 6f67 6765 722e 6465 6275 6728 6622   logger.debug(f"
-00001070: 6d65 6d6f 7279 5f75 7361 626c 653a 207b  memory_usable: {
-00001080: 6d65 6d5f 7573 6162 6c65 7d2c 2077 6974  mem_usable}, wit
-00001090: 683a 2229 0a20 2020 206d 656d 5f61 7661  h:").    mem_ava
-000010a0: 696c 6162 6c65 203d 205f 6765 6e65 7261  ilable = _genera
-000010b0: 6c5f 7574 696c 2e66 6f72 6d61 7462 7974  l_util.formatbyt
-000010c0: 6573 2870 7375 7469 6c2e 7669 7274 7561  es(psutil.virtua
-000010d0: 6c5f 6d65 6d6f 7279 2829 2e61 7661 696c  l_memory().avail
-000010e0: 6162 6c65 290a 2020 2020 6c6f 6767 6572  able).    logger
-000010f0: 2e64 6562 7567 2866 2220 202d 3e20 6d65  .debug(f"  -> me
-00001100: 6d2e 6176 6169 6c61 626c 653a 207b 6d65  m.available: {me
-00001110: 6d5f 6176 6169 6c61 626c 657d 2229 0a20  m_available}"). 
-00001120: 2020 2073 7761 705f 6672 6565 203d 205f     swap_free = _
-00001130: 6765 6e65 7261 6c5f 7574 696c 2e66 6f72  general_util.for
-00001140: 6d61 7462 7974 6573 2870 7375 7469 6c2e  matbytes(psutil.
-00001150: 7377 6170 5f6d 656d 6f72 7928 292e 6672  swap_memory().fr
-00001160: 6565 290a 2020 2020 6c6f 6767 6572 2e64  ee).    logger.d
-00001170: 6562 7567 2866 2220 202d 3e20 7377 6170  ebug(f"  -> swap
-00001180: 2e66 7265 653a 207b 7377 6170 5f66 7265  .free: {swap_fre
-00001190: 657d 2229 0a0a 2020 2020 2320 4966 206e  e}")..    # If n
-000011a0: 6f74 2065 6e6f 7567 6820 6d65 6d6f 7279  ot enough memory
-000011b0: 2066 6f72 2074 6865 2061 6d6f 756e 7420   for the amount 
-000011c0: 6f66 2070 6172 616c 6c65 6c6c 6973 6d20  of parallellism 
-000011d0: 6173 6b65 642c 2072 6564 7563 650a 2020  asked, reduce.  
-000011e0: 2020 6966 2028 0a20 2020 2020 2020 206e    if (.        n
-000011f0: 625f 7061 7261 6c6c 656c 202a 2070 6172  b_parallel * par
-00001200: 616c 6c65 6c69 7a61 7469 6f6e 5f63 6f6e  allelization_con
-00001210: 6669 675f 6c6f 6361 6c2e 6279 7465 735f  fig_local.bytes_
-00001220: 6d69 6e5f 7065 725f 7072 6f63 6573 730a  min_per_process.
-00001230: 2020 2020 2920 3e20 7061 7261 6c6c 656c      ) > parallel
-00001240: 697a 6174 696f 6e5f 636f 6e66 6967 5f6c  ization_config_l
-00001250: 6f63 616c 2e62 7974 6573 5f75 7361 626c  ocal.bytes_usabl
-00001260: 653a 0a20 2020 2020 2020 206e 625f 7061  e:.        nb_pa
-00001270: 7261 6c6c 656c 203d 2069 6e74 280a 2020  rallel = int(.  
-00001280: 2020 2020 2020 2020 2020 7061 7261 6c6c            parall
-00001290: 656c 697a 6174 696f 6e5f 636f 6e66 6967  elization_config
-000012a0: 5f6c 6f63 616c 2e62 7974 6573 5f75 7361  _local.bytes_usa
-000012b0: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
-000012c0: 2f20 7061 7261 6c6c 656c 697a 6174 696f  / parallelizatio
-000012d0: 6e5f 636f 6e66 6967 5f6c 6f63 616c 2e62  n_config_local.b
-000012e0: 7974 6573 5f6d 696e 5f70 6572 5f70 726f  ytes_min_per_pro
-000012f0: 6365 7373 0a20 2020 2020 2020 2029 0a20  cess.        ). 
-00001300: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00001310: 6275 6728 6622 4e62 5f70 6172 616c 6c65  bug(f"Nb_paralle
-00001320: 6c20 7265 6475 6365 6420 746f 207b 6e62  l reduced to {nb
-00001330: 5f70 6172 616c 6c65 6c7d 2074 6f20 7265  _parallel} to re
-00001340: 6475 6365 206d 656d 6f72 7920 7573 6167  duce memory usag
-00001350: 6522 290a 0a20 2020 2023 204f 7074 696d  e")..    # Optim
-00001360: 616c 206e 756d 6265 7220 6f66 2062 6174  al number of bat
-00001370: 6368 6573 2061 6e64 2072 6f77 7320 7065  ches and rows pe
-00001380: 7220 6261 7463 6820 6261 7365 6420 6f6e  r batch based on
-00001390: 206d 656d 6f72 7920 7573 6167 650a 2020   memory usage.  
-000013a0: 2020 6e62 5f62 6174 6368 6573 203d 206d    nb_batches = m
-000013b0: 6174 682e 6365 696c 280a 2020 2020 2020  ath.ceil(.      
-000013c0: 2020 286e 625f 726f 7773 5f74 6f74 616c    (nb_rows_total
-000013d0: 202a 2070 6172 616c 6c65 6c69 7a61 7469   * parallelizati
-000013e0: 6f6e 5f63 6f6e 6669 675f 6c6f 6361 6c2e  on_config_local.
-000013f0: 6279 7465 735f 7065 725f 726f 7720 2a20  bytes_per_row * 
-00001400: 6e62 5f70 6172 616c 6c65 6c29 0a20 2020  nb_parallel).   
-00001410: 2020 2020 202f 2028 0a20 2020 2020 2020       / (.       
-00001420: 2020 2020 2070 6172 616c 6c65 6c69 7a61       paralleliza
-00001430: 7469 6f6e 5f63 6f6e 6669 675f 6c6f 6361  tion_config_loca
-00001440: 6c2e 6279 7465 735f 7573 6162 6c65 0a20  l.bytes_usable. 
-00001450: 2020 2020 2020 2020 2020 202d 2070 6172             - par
-00001460: 616c 6c65 6c69 7a61 7469 6f6e 5f63 6f6e  allelization_con
-00001470: 6669 675f 6c6f 6361 6c2e 6279 7465 735f  fig_local.bytes_
-00001480: 6261 7365 666f 6f74 7072 696e 7420 2a20  basefootprint * 
-00001490: 6e62 5f70 6172 616c 6c65 6c0a 2020 2020  nb_parallel.    
-000014a0: 2020 2020 290a 2020 2020 290a 0a20 2020      ).    )..   
-000014b0: 2023 204d 616b 6520 7375 7265 2074 6865   # Make sure the
-000014c0: 2061 7665 7261 6765 2062 6174 6368 2064   average batch d
-000014d0: 6f65 736e 2774 2063 6f6e 7461 696e 203e  oesn't contain >
-000014e0: 206d 6178 5f61 7667 5f72 6f77 735f 7065   max_avg_rows_pe
-000014f0: 725f 6261 7463 680a 2020 2020 6261 7463  r_batch.    batc
-00001500: 685f 7369 7a65 203d 206d 6174 682e 6365  h_size = math.ce
-00001510: 696c 286e 625f 726f 7773 5f74 6f74 616c  il(nb_rows_total
-00001520: 202f 206e 625f 6261 7463 6865 7329 0a20   / nb_batches). 
-00001530: 2020 2069 6620 6261 7463 685f 7369 7a65     if batch_size
-00001540: 203e 2070 6172 616c 6c65 6c69 7a61 7469   > parallelizati
-00001550: 6f6e 5f63 6f6e 6669 675f 6c6f 6361 6c2e  on_config_local.
-00001560: 6d61 785f 6176 675f 726f 7773 5f70 6572  max_avg_rows_per
-00001570: 5f62 6174 6368 3a0a 2020 2020 2020 2020  _batch:.        
-00001580: 6261 7463 685f 7369 7a65 203d 2070 6172  batch_size = par
-00001590: 616c 6c65 6c69 7a61 7469 6f6e 5f63 6f6e  allelization_con
-000015a0: 6669 675f 6c6f 6361 6c2e 6d61 785f 6176  fig_local.max_av
-000015b0: 675f 726f 7773 5f70 6572 5f62 6174 6368  g_rows_per_batch
-000015c0: 0a20 2020 2020 2020 206e 625f 6261 7463  .        nb_batc
-000015d0: 6865 7320 3d20 6d61 7468 2e63 6569 6c28  hes = math.ceil(
-000015e0: 6e62 5f72 6f77 735f 746f 7461 6c20 2f20  nb_rows_total / 
-000015f0: 6261 7463 685f 7369 7a65 290a 0a20 2020  batch_size)..   
-00001600: 206d 656d 5f70 7265 6469 6374 6564 203d   mem_predicted =
-00001610: 2028 0a20 2020 2020 2020 2070 6172 616c   (.        paral
-00001620: 6c65 6c69 7a61 7469 6f6e 5f63 6f6e 6669  lelization_confi
-00001630: 675f 6c6f 6361 6c2e 6279 7465 735f 6261  g_local.bytes_ba
-00001640: 7365 666f 6f74 7072 696e 740a 2020 2020  sefootprint.    
-00001650: 2020 2020 2b20 6261 7463 685f 7369 7a65      + batch_size
-00001660: 202a 2070 6172 616c 6c65 6c69 7a61 7469   * parallelizati
-00001670: 6f6e 5f63 6f6e 6669 675f 6c6f 6361 6c2e  on_config_local.
-00001680: 6279 7465 735f 7065 725f 726f 770a 2020  bytes_per_row.  
-00001690: 2020 2920 2a20 6e62 5f62 6174 6368 6573    ) * nb_batches
-000016a0: 0a0a 2020 2020 2320 4d61 6b65 2073 7572  ..    # Make sur
-000016b0: 6520 7468 6572 6520 6172 6520 656e 6f75  e there are enou
-000016c0: 6768 2062 6174 6368 6573 2074 6f20 7573  gh batches to us
-000016d0: 6520 6173 206d 7563 6820 7061 7261 6c6c  e as much parall
-000016e0: 656c 6973 6d20 6173 2070 6f73 7369 626c  elism as possibl
-000016f0: 650a 2020 2020 6966 206e 625f 6261 7463  e.    if nb_batc
-00001700: 6865 7320 3e20 3120 616e 6420 6e62 5f62  hes > 1 and nb_b
-00001710: 6174 6368 6573 203c 206e 625f 7061 7261  atches < nb_para
-00001720: 6c6c 656c 3a0a 2020 2020 2020 2020 6d61  llel:.        ma
-00001730: 785f 7061 7261 6c6c 656c 5f62 6174 6368  x_parallel_batch
-00001740: 7369 7a65 203d 2069 6e74 280a 2020 2020  size = int(.    
-00001750: 2020 2020 2020 2020 7061 7261 6c6c 656c          parallel
-00001760: 697a 6174 696f 6e5f 636f 6e66 6967 5f6c  ization_config_l
-00001770: 6f63 616c 2e6d 6178 5f61 7667 5f72 6f77  ocal.max_avg_row
-00001780: 735f 7065 725f 6261 7463 680a 2020 2020  s_per_batch.    
-00001790: 2020 2020 2020 2020 2a20 6e62 5f62 6174          * nb_bat
-000017a0: 6368 6573 0a20 2020 2020 2020 2020 2020  ches.           
-000017b0: 202f 2062 6174 6368 5f73 697a 650a 2020   / batch_size.  
-000017c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000017d0: 6e62 5f70 6172 616c 6c65 6c20 3d20 6d69  nb_parallel = mi
-000017e0: 6e28 6d61 785f 7061 7261 6c6c 656c 5f62  n(max_parallel_b
-000017f0: 6174 6368 7369 7a65 2c20 6e62 5f70 6172  atchsize, nb_par
-00001800: 616c 6c65 6c29 0a20 2020 2020 2020 2069  allel).        i
-00001810: 6620 6e62 5f62 6174 6368 6573 5f70 7265  f nb_batches_pre
-00001820: 7669 6f75 735f 7061 7373 2069 7320 4e6f  vious_pass is No
-00001830: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00001840: 6e62 5f62 6174 6368 6573 203d 2072 6f75  nb_batches = rou
-00001850: 6e64 286e 625f 7061 7261 6c6c 656c 202a  nd(nb_parallel *
-00001860: 2031 2e32 3529 0a20 2020 2020 2020 2065   1.25).        e
-00001870: 6c69 6620 6e62 5f62 6174 6368 6573 203c  lif nb_batches <
-00001880: 206e 625f 6261 7463 6865 735f 7072 6576   nb_batches_prev
-00001890: 696f 7573 5f70 6173 7320 2f20 343a 0a20  ious_pass / 4:. 
-000018a0: 2020 2020 2020 2020 2020 206e 625f 6261             nb_ba
-000018b0: 7463 6865 7320 3d20 726f 756e 6428 6e62  tches = round(nb
-000018c0: 5f70 6172 616c 6c65 6c20 2a20 312e 3235  _parallel * 1.25
-000018d0: 290a 0a20 2020 2062 6174 6368 5f73 697a  )..    batch_siz
-000018e0: 6520 3d20 6d61 7468 2e63 6569 6c28 6e62  e = math.ceil(nb
-000018f0: 5f72 6f77 735f 746f 7461 6c20 2f20 6e62  _rows_total / nb
-00001900: 5f62 6174 6368 6573 290a 0a20 2020 2023  _batches)..    #
-00001910: 204c 6f67 2072 6573 756c 740a 2020 2020   Log result.    
-00001920: 6c6f 6767 6572 2e64 6562 7567 2866 226e  logger.debug(f"n
-00001930: 625f 6261 7463 6865 735f 7265 636f 6d6d  b_batches_recomm
-00001940: 656e 6465 643a 207b 6e62 5f62 6174 6368  ended: {nb_batch
-00001950: 6573 7d2c 2072 6f77 735f 7065 725f 6261  es}, rows_per_ba
-00001960: 7463 683a 207b 6261 7463 685f 7369 7a65  tch: {batch_size
-00001970: 7d22 290a 2020 2020 6c6f 6767 6572 2e64  }").    logger.d
-00001980: 6562 7567 2866 2220 2d3e 206e 625f 726f  ebug(f" -> nb_ro
-00001990: 7773 5f69 6e70 7574 5f6c 6179 6572 3a20  ws_input_layer: 
-000019a0: 7b6e 625f 726f 7773 5f74 6f74 616c 7d22  {nb_rows_total}"
-000019b0: 290a 2020 2020 6c6f 6767 6572 2e64 6562  ).    logger.deb
-000019c0: 7567 2866 2220 2d3e 206d 656d 5f70 7265  ug(f" -> mem_pre
-000019d0: 6469 6374 6564 3a20 7b5f 6765 6e65 7261  dicted: {_genera
-000019e0: 6c5f 7574 696c 2e66 6f72 6d61 7462 7974  l_util.formatbyt
-000019f0: 6573 286d 656d 5f70 7265 6469 6374 6564  es(mem_predicted
-00001a00: 297d 2229 0a0a 2020 2020 7265 7475 726e  )}")..    return
-00001a10: 2070 6172 616c 6c65 6c69 7a61 7469 6f6e   parallelization
-00001a20: 5061 7261 6d73 286e 625f 7061 7261 6c6c  Params(nb_parall
-00001a30: 656c 2c20 6e62 5f62 6174 6368 6573 2c20  el, nb_batches, 
-00001a40: 6261 7463 685f 7369 7a65 290a 0a0a 636c  batch_size)...cl
-00001a50: 6173 7320 4765 6f4f 7065 7261 7469 6f6e  ass GeoOperation
-00001a60: 2865 6e75 6d2e 456e 756d 293a 0a20 2020  (enum.Enum):.   
-00001a70: 2053 494d 504c 4946 5920 3d20 2273 696d   SIMPLIFY = "sim
-00001a80: 706c 6966 7922 0a20 2020 2042 5546 4645  plify".    BUFFE
-00001a90: 5220 3d20 2262 7566 6665 7222 0a20 2020  R = "buffer".   
-00001aa0: 2043 4f4e 5645 5848 554c 4c20 3d20 2263   CONVEXHULL = "c
-00001ab0: 6f6e 7665 7868 756c 6c22 0a20 2020 2041  onvexhull".    A
-00001ac0: 5050 4c59 203d 2022 6170 706c 7922 0a0a  PPLY = "apply"..
-00001ad0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00001ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b20: 230a 2320 5468 6520 7265 616c 2073 7475  #.# The real stu
-00001b30: 6666 0a23 2323 2323 2323 2323 2323 2323  ff.#############
-00001b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000690: 0a23 2053 6f6d 6520 6865 6c70 6572 2066  .# Some helper f
+000006a0: 756e 6374 696f 6e73 0a23 2323 2323 2323  unctions.#######
+000006b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000006c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000006d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000006e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000006f0: 2323 2323 2323 2323 230a 0a0a 636c 6173  #########...clas
+00000700: 7320 5061 7261 6c6c 656c 697a 6174 696f  s Parallelizatio
+00000710: 6e43 6f6e 6669 673a 0a20 2020 2064 6566  nConfig:.    def
+00000720: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00000730: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00000740: 2062 7974 6573 5f62 6173 6566 6f6f 7470   bytes_basefootp
+00000750: 7269 6e74 3a20 696e 7420 3d20 3530 202a  rint: int = 50 *
+00000760: 2031 3032 3420 2a20 3130 3234 2c0a 2020   1024 * 1024,.  
+00000770: 2020 2020 2020 6279 7465 735f 7065 725f        bytes_per_
+00000780: 726f 773a 2069 6e74 203d 2031 3030 2c0a  row: int = 100,.
+00000790: 2020 2020 2020 2020 6d69 6e5f 6176 675f          min_avg_
+000007a0: 726f 7773 5f70 6572 5f62 6174 6368 3a20  rows_per_batch: 
+000007b0: 696e 7420 3d20 3130 3030 2c0a 2020 2020  int = 1000,.    
+000007c0: 2020 2020 6d61 785f 6176 675f 726f 7773      max_avg_rows
+000007d0: 5f70 6572 5f62 6174 6368 3a20 696e 7420  _per_batch: int 
+000007e0: 3d20 3130 3030 302c 0a20 2020 2020 2020  = 10000,.       
+000007f0: 2062 7974 6573 5f6d 696e 5f70 6572 5f70   bytes_min_per_p
+00000800: 726f 6365 7373 3d4e 6f6e 652c 0a20 2020  rocess=None,.   
+00000810: 2020 2020 2062 7974 6573 5f75 7361 626c       bytes_usabl
+00000820: 653d 4e6f 6e65 2c0a 2020 2020 293a 0a20  e=None,.    ):. 
+00000830: 2020 2020 2020 2073 656c 662e 6279 7465         self.byte
+00000840: 735f 6261 7365 666f 6f74 7072 696e 7420  s_basefootprint 
+00000850: 3d20 6279 7465 735f 6261 7365 666f 6f74  = bytes_basefoot
+00000860: 7072 696e 740a 2020 2020 2020 2020 7365  print.        se
+00000870: 6c66 2e62 7974 6573 5f70 6572 5f72 6f77  lf.bytes_per_row
+00000880: 203d 2062 7974 6573 5f70 6572 5f72 6f77   = bytes_per_row
+00000890: 0a20 2020 2020 2020 2073 656c 662e 6d69  .        self.mi
+000008a0: 6e5f 6176 675f 726f 7773 5f70 6572 5f62  n_avg_rows_per_b
+000008b0: 6174 6368 203d 206d 696e 5f61 7667 5f72  atch = min_avg_r
+000008c0: 6f77 735f 7065 725f 6261 7463 680a 2020  ows_per_batch.  
+000008d0: 2020 2020 2020 7365 6c66 2e6d 6178 5f61        self.max_a
+000008e0: 7667 5f72 6f77 735f 7065 725f 6261 7463  vg_rows_per_batc
+000008f0: 6820 3d20 6d61 785f 6176 675f 726f 7773  h = max_avg_rows
+00000900: 5f70 6572 5f62 6174 6368 0a20 2020 2020  _per_batch.     
+00000910: 2020 2069 6620 6279 7465 735f 6d69 6e5f     if bytes_min_
+00000920: 7065 725f 7072 6f63 6573 7320 6973 204e  per_process is N
+00000930: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00000940: 2073 656c 662e 6279 7465 735f 6d69 6e5f   self.bytes_min_
+00000950: 7065 725f 7072 6f63 6573 7320 3d20 280a  per_process = (.
+00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000970: 6279 7465 735f 6261 7365 666f 6f74 7072  bytes_basefootpr
+00000980: 696e 7420 2b20 6279 7465 735f 7065 725f  int + bytes_per_
+00000990: 726f 7720 2a20 6d69 6e5f 6176 675f 726f  row * min_avg_ro
+000009a0: 7773 5f70 6572 5f62 6174 6368 0a20 2020  ws_per_batch.   
+000009b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000009c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000009d0: 2020 2020 2073 656c 662e 6279 7465 735f       self.bytes_
+000009e0: 6d69 6e5f 7065 725f 7072 6f63 6573 7320  min_per_process 
+000009f0: 3d20 6279 7465 735f 6d69 6e5f 7065 725f  = bytes_min_per_
+00000a00: 7072 6f63 6573 730a 2020 2020 2020 2020  process.        
+00000a10: 6966 2062 7974 6573 5f75 7361 626c 6520  if bytes_usable 
+00000a20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00000a30: 2020 2020 2073 656c 662e 6279 7465 735f       self.bytes_
+00000a40: 7573 6162 6c65 203d 2070 7375 7469 6c2e  usable = psutil.
+00000a50: 7669 7274 7561 6c5f 6d65 6d6f 7279 2829  virtual_memory()
+00000a60: 2e61 7661 696c 6162 6c65 202a 2030 2e39  .available * 0.9
+00000a70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00000a80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000a90: 6279 7465 735f 7573 6162 6c65 203d 2062  bytes_usable = b
+00000aa0: 7974 6573 5f75 7361 626c 650a 0a0a 7061  ytes_usable...pa
+00000ab0: 7261 6c6c 656c 697a 6174 696f 6e50 6172  rallelizationPar
+00000ac0: 616d 7320 3d20 4e61 6d65 6454 7570 6c65  ams = NamedTuple
+00000ad0: 280a 2020 2020 2272 6573 756c 7422 2c0a  (.    "result",.
+00000ae0: 2020 2020 5b28 226e 625f 7061 7261 6c6c      [("nb_parall
+00000af0: 656c 222c 2069 6e74 292c 2028 226e 625f  el", int), ("nb_
+00000b00: 6261 7463 6865 735f 7265 636f 6d6d 656e  batches_recommen
+00000b10: 6465 6422 2c20 696e 7429 2c20 2822 6e62  ded", int), ("nb
+00000b20: 5f72 6f77 735f 7065 725f 6261 7463 6822  _rows_per_batch"
+00000b30: 2c20 696e 7429 5d2c 0a29 0a0a 0a64 6566  , int)],.)...def
+00000b40: 2067 6574 5f70 6172 616c 6c65 6c69 7a61   get_paralleliza
+00000b50: 7469 6f6e 5f70 6172 616d 7328 0a20 2020  tion_params(.   
+00000b60: 206e 625f 726f 7773 5f74 6f74 616c 3a20   nb_rows_total: 
+00000b70: 696e 742c 0a20 2020 206e 625f 7061 7261  int,.    nb_para
+00000b80: 6c6c 656c 3a20 696e 7420 3d20 2d31 2c0a  llel: int = -1,.
+00000b90: 2020 2020 6e62 5f62 6174 6368 6573 5f70      nb_batches_p
+00000ba0: 7265 7669 6f75 735f 7061 7373 3a20 4f70  revious_pass: Op
+00000bb0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00000bc0: 6e65 2c0a 2020 2020 7061 7261 6c6c 656c  ne,.    parallel
+00000bd0: 697a 6174 696f 6e5f 636f 6e66 6967 3a20  ization_config: 
+00000be0: 4f70 7469 6f6e 616c 5b50 6172 616c 6c65  Optional[Paralle
+00000bf0: 6c69 7a61 7469 6f6e 436f 6e66 6967 5d20  lizationConfig] 
+00000c00: 3d20 4e6f 6e65 2c0a 2920 2d3e 2070 6172  = None,.) -> par
+00000c10: 616c 6c65 6c69 7a61 7469 6f6e 5061 7261  allelizationPara
+00000c20: 6d73 3a0a 2020 2020 2222 220a 2020 2020  ms:.    """.    
+00000c30: 4465 7465 726d 696e 6573 2072 6563 6f6d  Determines recom
+00000c40: 6d65 6e64 6564 2070 6172 616c 6c65 6c69  mended paralleli
+00000c50: 7a61 7469 6f6e 2070 6172 616d 732e 0a0a  zation params...
+00000c60: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000c70: 2020 6e62 5f72 6f77 735f 746f 7461 6c20    nb_rows_total 
+00000c80: 2869 6e74 293a 2054 6865 2074 6f74 616c  (int): The total
+00000c90: 206e 756d 6265 7220 6f66 2072 6f77 7320   number of rows 
+00000ca0: 7468 6174 2077 696c 6c20 6265 2070 726f  that will be pro
+00000cb0: 6365 7373 6564 0a20 2020 2020 2020 206e  cessed.        n
+00000cc0: 625f 7061 7261 6c6c 656c 2028 696e 742c  b_parallel (int,
+00000cd0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00000ce0: 6c65 7665 6c20 6f66 2070 6172 616c 6c65  level of paralle
+00000cf0: 6c69 7a61 7469 6f6e 2072 6571 7565 7374  lization request
+00000d00: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00000d10: 4966 202d 312c 2074 7269 6573 2074 6f20  If -1, tries to 
+00000d20: 7573 6520 616c 6c20 7265 736f 7572 6365  use all resource
+00000d30: 7320 6176 6169 6c61 626c 652e 2044 6566  s available. Def
+00000d40: 6175 6c74 7320 746f 202d 312e 0a20 2020  aults to -1..   
+00000d50: 2020 2020 206e 625f 6261 7463 6865 735f       nb_batches_
+00000d60: 7072 6576 696f 7573 5f70 6173 7320 2869  previous_pass (i
+00000d70: 6e74 2c20 6f70 7469 6f6e 616c 293a 2049  nt, optional): I
+00000d80: 6620 6170 706c 6963 6162 6c65 2c20 7468  f applicable, th
+00000d90: 6520 6e75 6d62 6572 206f 6620 6261 7463  e number of batc
+00000da0: 6865 730a 2020 2020 2020 2020 2020 2020  hes.            
+00000db0: 7573 6564 2069 6e20 6120 7072 6576 696f  used in a previo
+00000dc0: 7573 2070 6173 7320 6f66 2074 6865 2063  us pass of the c
+00000dd0: 616c 6375 6c61 7469 6f6e 2e20 4465 6661  alculation. Defa
+00000de0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
+00000df0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00000e00: 2020 2020 7061 7261 6c6c 656c 697a 6174      parallelizat
+00000e10: 696f 6e50 6172 616d 733a 2054 6865 2072  ionParams: The r
+00000e20: 6563 6f6d 6d65 6e64 6564 2070 6172 616d  ecommended param
+00000e30: 6574 6572 732e 0a20 2020 2022 2222 0a20  eters..    """. 
+00000e40: 2020 2023 2049 6e69 7420 7061 7261 6c6c     # Init parall
+00000e50: 656c 697a 6174 696f 6e20 636f 6e66 6967  elization config
+00000e60: 0a0a 2020 2020 2320 4966 2063 6f6e 6669  ..    # If confi
+00000e70: 6720 6973 204e 6f6e 652c 2073 6574 2074  g is None, set t
+00000e80: 6f20 656d 7074 7920 6469 6374 0a20 2020  o empty dict.   
+00000e90: 2069 6620 7061 7261 6c6c 656c 697a 6174   if parallelizat
+00000ea0: 696f 6e5f 636f 6e66 6967 2069 7320 6e6f  ion_config is no
+00000eb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00000ec0: 7061 7261 6c6c 656c 697a 6174 696f 6e5f  parallelization_
+00000ed0: 636f 6e66 6967 5f6c 6f63 616c 203d 2070  config_local = p
+00000ee0: 6172 616c 6c65 6c69 7a61 7469 6f6e 5f63  arallelization_c
+00000ef0: 6f6e 6669 670a 2020 2020 656c 7365 3a0a  onfig.    else:.
+00000f00: 2020 2020 2020 2020 7061 7261 6c6c 656c          parallel
+00000f10: 697a 6174 696f 6e5f 636f 6e66 6967 5f6c  ization_config_l
+00000f20: 6f63 616c 203d 2050 6172 616c 6c65 6c69  ocal = Paralleli
+00000f30: 7a61 7469 6f6e 436f 6e66 6967 2829 0a0a  zationConfig()..
+00000f40: 2020 2020 2320 4966 2074 6865 206e 756d      # If the num
+00000f50: 6265 7220 6f66 2072 6f77 7320 6973 2072  ber of rows is r
+00000f60: 6561 6c6c 7920 6c6f 772c 206a 7573 7420  eally low, just 
+00000f70: 7573 6520 6f6e 6520 6261 7463 680a 2020  use one batch.  
+00000f80: 2020 2320 544f 444f 3a20 666f 7220 7665    # TODO: for ve
+00000f90: 7279 2063 6f6d 706c 6578 2066 6561 7475  ry complex featu
+00000fa0: 7265 732c 2070 6f73 7369 626c 7920 7468  res, possibly th
+00000fb0: 6973 206c 696d 6974 2069 7320 6e6f 7420  is limit is not 
+00000fc0: 6120 676f 6f64 2069 6465 610a 2020 2020  a good idea.    
+00000fd0: 6966 206e 625f 726f 7773 5f74 6f74 616c  if nb_rows_total
+00000fe0: 203c 2070 6172 616c 6c65 6c69 7a61 7469   < parallelizati
+00000ff0: 6f6e 5f63 6f6e 6669 675f 6c6f 6361 6c2e  on_config_local.
+00001000: 6d69 6e5f 6176 675f 726f 7773 5f70 6572  min_avg_rows_per
+00001010: 5f62 6174 6368 3a0a 2020 2020 2020 2020  _batch:.        
+00001020: 7265 7475 726e 2070 6172 616c 6c65 6c69  return paralleli
+00001030: 7a61 7469 6f6e 5061 7261 6d73 2831 2c20  zationParams(1, 
+00001040: 312c 206e 625f 726f 7773 5f74 6f74 616c  1, nb_rows_total
+00001050: 290a 0a20 2020 2069 6620 6e62 5f70 6172  )..    if nb_par
+00001060: 616c 6c65 6c20 3d3d 202d 313a 0a20 2020  allel == -1:.   
+00001070: 2020 2020 206e 625f 7061 7261 6c6c 656c       nb_parallel
+00001080: 203d 206d 756c 7469 7072 6f63 6573 7369   = multiprocessi
+00001090: 6e67 2e63 7075 5f63 6f75 6e74 2829 0a0a  ng.cpu_count()..
+000010a0: 2020 2020 6d65 6d5f 7573 6162 6c65 203d      mem_usable =
+000010b0: 205f 6765 6e65 7261 6c5f 7574 696c 2e66   _general_util.f
+000010c0: 6f72 6d61 7462 7974 6573 2870 6172 616c  ormatbytes(paral
+000010d0: 6c65 6c69 7a61 7469 6f6e 5f63 6f6e 6669  lelization_confi
+000010e0: 675f 6c6f 6361 6c2e 6279 7465 735f 7573  g_local.bytes_us
+000010f0: 6162 6c65 290a 2020 2020 6c6f 6767 6572  able).    logger
+00001100: 2e64 6562 7567 2866 226d 656d 6f72 795f  .debug(f"memory_
+00001110: 7573 6162 6c65 3a20 7b6d 656d 5f75 7361  usable: {mem_usa
+00001120: 626c 657d 2c20 7769 7468 3a22 290a 2020  ble}, with:").  
+00001130: 2020 6d65 6d5f 6176 6169 6c61 626c 6520    mem_available 
+00001140: 3d20 5f67 656e 6572 616c 5f75 7469 6c2e  = _general_util.
+00001150: 666f 726d 6174 6279 7465 7328 7073 7574  formatbytes(psut
+00001160: 696c 2e76 6972 7475 616c 5f6d 656d 6f72  il.virtual_memor
+00001170: 7928 292e 6176 6169 6c61 626c 6529 0a20  y().available). 
+00001180: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00001190: 6622 2020 2d3e 206d 656d 2e61 7661 696c  f"  -> mem.avail
+000011a0: 6162 6c65 3a20 7b6d 656d 5f61 7661 696c  able: {mem_avail
+000011b0: 6162 6c65 7d22 290a 2020 2020 7377 6170  able}").    swap
+000011c0: 5f66 7265 6520 3d20 5f67 656e 6572 616c  _free = _general
+000011d0: 5f75 7469 6c2e 666f 726d 6174 6279 7465  _util.formatbyte
+000011e0: 7328 7073 7574 696c 2e73 7761 705f 6d65  s(psutil.swap_me
+000011f0: 6d6f 7279 2829 2e66 7265 6529 0a20 2020  mory().free).   
+00001200: 206c 6f67 6765 722e 6465 6275 6728 6622   logger.debug(f"
+00001210: 2020 2d3e 2073 7761 702e 6672 6565 3a20    -> swap.free: 
+00001220: 7b73 7761 705f 6672 6565 7d22 290a 0a20  {swap_free}").. 
+00001230: 2020 2023 2049 6620 6e6f 7420 656e 6f75     # If not enou
+00001240: 6768 206d 656d 6f72 7920 666f 7220 7468  gh memory for th
+00001250: 6520 616d 6f75 6e74 206f 6620 7061 7261  e amount of para
+00001260: 6c6c 656c 6c69 736d 2061 736b 6564 2c20  llellism asked, 
+00001270: 7265 6475 6365 0a20 2020 2069 6620 280a  reduce.    if (.
+00001280: 2020 2020 2020 2020 6e62 5f70 6172 616c          nb_paral
+00001290: 6c65 6c20 2a20 7061 7261 6c6c 656c 697a  lel * paralleliz
+000012a0: 6174 696f 6e5f 636f 6e66 6967 5f6c 6f63  ation_config_loc
+000012b0: 616c 2e62 7974 6573 5f6d 696e 5f70 6572  al.bytes_min_per
+000012c0: 5f70 726f 6365 7373 0a20 2020 2029 203e  _process.    ) >
+000012d0: 2070 6172 616c 6c65 6c69 7a61 7469 6f6e   parallelization
+000012e0: 5f63 6f6e 6669 675f 6c6f 6361 6c2e 6279  _config_local.by
+000012f0: 7465 735f 7573 6162 6c65 3a0a 2020 2020  tes_usable:.    
+00001300: 2020 2020 6e62 5f70 6172 616c 6c65 6c20      nb_parallel 
+00001310: 3d20 696e 7428 0a20 2020 2020 2020 2020  = int(.         
+00001320: 2020 2070 6172 616c 6c65 6c69 7a61 7469     parallelizati
+00001330: 6f6e 5f63 6f6e 6669 675f 6c6f 6361 6c2e  on_config_local.
+00001340: 6279 7465 735f 7573 6162 6c65 0a20 2020  bytes_usable.   
+00001350: 2020 2020 2020 2020 202f 2070 6172 616c           / paral
+00001360: 6c65 6c69 7a61 7469 6f6e 5f63 6f6e 6669  lelization_confi
+00001370: 675f 6c6f 6361 6c2e 6279 7465 735f 6d69  g_local.bytes_mi
+00001380: 6e5f 7065 725f 7072 6f63 6573 730a 2020  n_per_process.  
+00001390: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000013a0: 6c6f 6767 6572 2e64 6562 7567 2866 224e  logger.debug(f"N
+000013b0: 625f 7061 7261 6c6c 656c 2072 6564 7563  b_parallel reduc
+000013c0: 6564 2074 6f20 7b6e 625f 7061 7261 6c6c  ed to {nb_parall
+000013d0: 656c 7d20 746f 2072 6564 7563 6520 6d65  el} to reduce me
+000013e0: 6d6f 7279 2075 7361 6765 2229 0a0a 2020  mory usage")..  
+000013f0: 2020 2320 4f70 7469 6d61 6c20 6e75 6d62    # Optimal numb
+00001400: 6572 206f 6620 6261 7463 6865 7320 616e  er of batches an
+00001410: 6420 726f 7773 2070 6572 2062 6174 6368  d rows per batch
+00001420: 2062 6173 6564 206f 6e20 6d65 6d6f 7279   based on memory
+00001430: 2075 7361 6765 0a20 2020 206e 625f 6261   usage.    nb_ba
+00001440: 7463 6865 7320 3d20 6d61 7468 2e63 6569  tches = math.cei
+00001450: 6c28 0a20 2020 2020 2020 2028 6e62 5f72  l(.        (nb_r
+00001460: 6f77 735f 746f 7461 6c20 2a20 7061 7261  ows_total * para
+00001470: 6c6c 656c 697a 6174 696f 6e5f 636f 6e66  llelization_conf
+00001480: 6967 5f6c 6f63 616c 2e62 7974 6573 5f70  ig_local.bytes_p
+00001490: 6572 5f72 6f77 202a 206e 625f 7061 7261  er_row * nb_para
+000014a0: 6c6c 656c 290a 2020 2020 2020 2020 2f20  llel).        / 
+000014b0: 280a 2020 2020 2020 2020 2020 2020 7061  (.            pa
+000014c0: 7261 6c6c 656c 697a 6174 696f 6e5f 636f  rallelization_co
+000014d0: 6e66 6967 5f6c 6f63 616c 2e62 7974 6573  nfig_local.bytes
+000014e0: 5f75 7361 626c 650a 2020 2020 2020 2020  _usable.        
+000014f0: 2020 2020 2d20 7061 7261 6c6c 656c 697a      - paralleliz
+00001500: 6174 696f 6e5f 636f 6e66 6967 5f6c 6f63  ation_config_loc
+00001510: 616c 2e62 7974 6573 5f62 6173 6566 6f6f  al.bytes_basefoo
+00001520: 7470 7269 6e74 202a 206e 625f 7061 7261  tprint * nb_para
+00001530: 6c6c 656c 0a20 2020 2020 2020 2029 0a20  llel.        ). 
+00001540: 2020 2029 0a0a 2020 2020 2320 4d61 6b65     )..    # Make
+00001550: 2073 7572 6520 7468 6520 6176 6572 6167   sure the averag
+00001560: 6520 6261 7463 6820 646f 6573 6e27 7420  e batch doesn't 
+00001570: 636f 6e74 6169 6e20 3e20 6d61 785f 6176  contain > max_av
+00001580: 675f 726f 7773 5f70 6572 5f62 6174 6368  g_rows_per_batch
+00001590: 0a20 2020 2062 6174 6368 5f73 697a 6520  .    batch_size 
+000015a0: 3d20 6d61 7468 2e63 6569 6c28 6e62 5f72  = math.ceil(nb_r
+000015b0: 6f77 735f 746f 7461 6c20 2f20 6e62 5f62  ows_total / nb_b
+000015c0: 6174 6368 6573 290a 2020 2020 6966 2062  atches).    if b
+000015d0: 6174 6368 5f73 697a 6520 3e20 7061 7261  atch_size > para
+000015e0: 6c6c 656c 697a 6174 696f 6e5f 636f 6e66  llelization_conf
+000015f0: 6967 5f6c 6f63 616c 2e6d 6178 5f61 7667  ig_local.max_avg
+00001600: 5f72 6f77 735f 7065 725f 6261 7463 683a  _rows_per_batch:
+00001610: 0a20 2020 2020 2020 2062 6174 6368 5f73  .        batch_s
+00001620: 697a 6520 3d20 7061 7261 6c6c 656c 697a  ize = paralleliz
+00001630: 6174 696f 6e5f 636f 6e66 6967 5f6c 6f63  ation_config_loc
+00001640: 616c 2e6d 6178 5f61 7667 5f72 6f77 735f  al.max_avg_rows_
+00001650: 7065 725f 6261 7463 680a 2020 2020 2020  per_batch.      
+00001660: 2020 6e62 5f62 6174 6368 6573 203d 206d    nb_batches = m
+00001670: 6174 682e 6365 696c 286e 625f 726f 7773  ath.ceil(nb_rows
+00001680: 5f74 6f74 616c 202f 2062 6174 6368 5f73  _total / batch_s
+00001690: 697a 6529 0a0a 2020 2020 6d65 6d5f 7072  ize)..    mem_pr
+000016a0: 6564 6963 7465 6420 3d20 280a 2020 2020  edicted = (.    
+000016b0: 2020 2020 7061 7261 6c6c 656c 697a 6174      parallelizat
+000016c0: 696f 6e5f 636f 6e66 6967 5f6c 6f63 616c  ion_config_local
+000016d0: 2e62 7974 6573 5f62 6173 6566 6f6f 7470  .bytes_basefootp
+000016e0: 7269 6e74 0a20 2020 2020 2020 202b 2062  rint.        + b
+000016f0: 6174 6368 5f73 697a 6520 2a20 7061 7261  atch_size * para
+00001700: 6c6c 656c 697a 6174 696f 6e5f 636f 6e66  llelization_conf
+00001710: 6967 5f6c 6f63 616c 2e62 7974 6573 5f70  ig_local.bytes_p
+00001720: 6572 5f72 6f77 0a20 2020 2029 202a 206e  er_row.    ) * n
+00001730: 625f 6261 7463 6865 730a 0a20 2020 2023  b_batches..    #
+00001740: 204d 616b 6520 7375 7265 2074 6865 7265   Make sure there
+00001750: 2061 7265 2065 6e6f 7567 6820 6261 7463   are enough batc
+00001760: 6865 7320 746f 2075 7365 2061 7320 6d75  hes to use as mu
+00001770: 6368 2070 6172 616c 6c65 6c69 736d 2061  ch parallelism a
+00001780: 7320 706f 7373 6962 6c65 0a20 2020 2069  s possible.    i
+00001790: 6620 6e62 5f62 6174 6368 6573 203e 2031  f nb_batches > 1
+000017a0: 2061 6e64 206e 625f 6261 7463 6865 7320   and nb_batches 
+000017b0: 3c20 6e62 5f70 6172 616c 6c65 6c3a 0a20  < nb_parallel:. 
+000017c0: 2020 2020 2020 206d 6178 5f70 6172 616c         max_paral
+000017d0: 6c65 6c5f 6261 7463 6873 697a 6520 3d20  lel_batchsize = 
+000017e0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+000017f0: 2070 6172 616c 6c65 6c69 7a61 7469 6f6e   parallelization
+00001800: 5f63 6f6e 6669 675f 6c6f 6361 6c2e 6d61  _config_local.ma
+00001810: 785f 6176 675f 726f 7773 5f70 6572 5f62  x_avg_rows_per_b
+00001820: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
+00001830: 202a 206e 625f 6261 7463 6865 730a 2020   * nb_batches.  
+00001840: 2020 2020 2020 2020 2020 2f20 6261 7463            / batc
+00001850: 685f 7369 7a65 0a20 2020 2020 2020 2029  h_size.        )
+00001860: 0a20 2020 2020 2020 206e 625f 7061 7261  .        nb_para
+00001870: 6c6c 656c 203d 206d 696e 286d 6178 5f70  llel = min(max_p
+00001880: 6172 616c 6c65 6c5f 6261 7463 6873 697a  arallel_batchsiz
+00001890: 652c 206e 625f 7061 7261 6c6c 656c 290a  e, nb_parallel).
+000018a0: 2020 2020 2020 2020 6966 206e 625f 6261          if nb_ba
+000018b0: 7463 6865 735f 7072 6576 696f 7573 5f70  tches_previous_p
+000018c0: 6173 7320 6973 204e 6f6e 653a 0a20 2020  ass is None:.   
+000018d0: 2020 2020 2020 2020 206e 625f 6261 7463           nb_batc
+000018e0: 6865 7320 3d20 726f 756e 6428 6e62 5f70  hes = round(nb_p
+000018f0: 6172 616c 6c65 6c20 2a20 312e 3235 290a  arallel * 1.25).
+00001900: 2020 2020 2020 2020 656c 6966 206e 625f          elif nb_
+00001910: 6261 7463 6865 7320 3c20 6e62 5f62 6174  batches < nb_bat
+00001920: 6368 6573 5f70 7265 7669 6f75 735f 7061  ches_previous_pa
+00001930: 7373 202f 2034 3a0a 2020 2020 2020 2020  ss / 4:.        
+00001940: 2020 2020 6e62 5f62 6174 6368 6573 203d      nb_batches =
+00001950: 2072 6f75 6e64 286e 625f 7061 7261 6c6c   round(nb_parall
+00001960: 656c 202a 2031 2e32 3529 0a0a 2020 2020  el * 1.25)..    
+00001970: 6261 7463 685f 7369 7a65 203d 206d 6174  batch_size = mat
+00001980: 682e 6365 696c 286e 625f 726f 7773 5f74  h.ceil(nb_rows_t
+00001990: 6f74 616c 202f 206e 625f 6261 7463 6865  otal / nb_batche
+000019a0: 7329 0a0a 2020 2020 2320 4c6f 6720 7265  s)..    # Log re
+000019b0: 7375 6c74 0a20 2020 206c 6f67 6765 722e  sult.    logger.
+000019c0: 6465 6275 6728 6622 6e62 5f62 6174 6368  debug(f"nb_batch
+000019d0: 6573 5f72 6563 6f6d 6d65 6e64 6564 3a20  es_recommended: 
+000019e0: 7b6e 625f 6261 7463 6865 737d 2c20 726f  {nb_batches}, ro
+000019f0: 7773 5f70 6572 5f62 6174 6368 3a20 7b62  ws_per_batch: {b
+00001a00: 6174 6368 5f73 697a 657d 2229 0a20 2020  atch_size}").   
+00001a10: 206c 6f67 6765 722e 6465 6275 6728 6622   logger.debug(f"
+00001a20: 202d 3e20 6e62 5f72 6f77 735f 696e 7075   -> nb_rows_inpu
+00001a30: 745f 6c61 7965 723a 207b 6e62 5f72 6f77  t_layer: {nb_row
+00001a40: 735f 746f 7461 6c7d 2229 0a20 2020 206c  s_total}").    l
+00001a50: 6f67 6765 722e 6465 6275 6728 6622 202d  ogger.debug(f" -
+00001a60: 3e20 6d65 6d5f 7072 6564 6963 7465 643a  > mem_predicted:
+00001a70: 207b 5f67 656e 6572 616c 5f75 7469 6c2e   {_general_util.
+00001a80: 666f 726d 6174 6279 7465 7328 6d65 6d5f  formatbytes(mem_
+00001a90: 7072 6564 6963 7465 6429 7d22 290a 0a20  predicted)}").. 
+00001aa0: 2020 2072 6574 7572 6e20 7061 7261 6c6c     return parall
+00001ab0: 656c 697a 6174 696f 6e50 6172 616d 7328  elizationParams(
+00001ac0: 6e62 5f70 6172 616c 6c65 6c2c 206e 625f  nb_parallel, nb_
+00001ad0: 6261 7463 6865 732c 2062 6174 6368 5f73  batches, batch_s
+00001ae0: 697a 6529 0a0a 0a63 6c61 7373 2047 656f  ize)...class Geo
+00001af0: 4f70 6572 6174 696f 6e28 656e 756d 2e45  Operation(enum.E
+00001b00: 6e75 6d29 3a0a 2020 2020 5349 4d50 4c49  num):.    SIMPLI
+00001b10: 4659 203d 2022 7369 6d70 6c69 6679 220a  FY = "simplify".
+00001b20: 2020 2020 4255 4646 4552 203d 2022 6275      BUFFER = "bu
+00001b30: 6666 6572 220a 2020 2020 434f 4e56 4558  ffer".    CONVEX
+00001b40: 4855 4c4c 203d 2022 636f 6e76 6578 6875  HULL = "convexhu
+00001b50: 6c6c 220a 2020 2020 4150 504c 5920 3d20  ll".    APPLY = 
+00001b60: 2261 7070 6c79 220a 0a0a 2323 2323 2323  "apply"...######
 00001b70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001b80: 2323 230a 0a0a 6465 6620 6170 706c 7928  ###...def apply(
-00001b90: 0a20 2020 2069 6e70 7574 5f70 6174 683a  .    input_path:
-00001ba0: 2050 6174 682c 0a20 2020 206f 7574 7075   Path,.    outpu
-00001bb0: 745f 7061 7468 3a20 5061 7468 2c0a 2020  t_path: Path,.  
-00001bc0: 2020 6675 6e63 3a20 4361 6c6c 6162 6c65    func: Callable
-00001bd0: 5b5b 416e 795d 2c20 416e 795d 2c0a 2020  [[Any], Any],.  
-00001be0: 2020 6f6e 6c79 5f67 656f 6d5f 696e 7075    only_geom_inpu
-00001bf0: 743a 2062 6f6f 6c20 3d20 5472 7565 2c0a  t: bool = True,.
-00001c00: 2020 2020 696e 7075 745f 6c61 7965 723a      input_layer:
-00001c10: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00001c20: 204e 6f6e 652c 0a20 2020 206f 7574 7075   None,.    outpu
-00001c30: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
-00001c40: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00001c50: 2020 2063 6f6c 756d 6e73 3a20 4f70 7469     columns: Opti
-00001c60: 6f6e 616c 5b4c 6973 745b 7374 725d 5d20  onal[List[str]] 
-00001c70: 3d20 4e6f 6e65 2c0a 2020 2020 6578 706c  = None,.    expl
-00001c80: 6f64 6563 6f6c 6c65 6374 696f 6e73 3a20  odecollections: 
-00001c90: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00001ca0: 2020 666f 7263 655f 6f75 7470 7574 5f67    force_output_g
-00001cb0: 656f 6d65 7472 7974 7970 653a 2055 6e69  eometrytype: Uni
-00001cc0: 6f6e 5b47 656f 6d65 7472 7954 7970 652c  on[GeometryType,
-00001cd0: 2073 7472 2c20 4e6f 6e65 5d20 3d20 4e6f   str, None] = No
-00001ce0: 6e65 2c0a 2020 2020 6e62 5f70 6172 616c  ne,.    nb_paral
-00001cf0: 6c65 6c3a 2069 6e74 203d 202d 312c 0a20  lel: int = -1,. 
-00001d00: 2020 2062 6174 6368 7369 7a65 3a20 696e     batchsize: in
-00001d10: 7420 3d20 2d31 2c0a 2020 2020 666f 7263  t = -1,.    forc
-00001d20: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
-00001d30: 0a29 3a0a 2020 2020 2320 496e 6974 0a20  .):.    # Init. 
-00001d40: 2020 206f 7065 7261 7469 6f6e 5f70 6172     operation_par
-00001d50: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
-00001d60: 226f 6e6c 795f 6765 6f6d 5f69 6e70 7574  "only_geom_input
-00001d70: 223a 206f 6e6c 795f 6765 6f6d 5f69 6e70  ": only_geom_inp
-00001d80: 7574 2c0a 2020 2020 2020 2020 2270 6963  ut,.        "pic
-00001d90: 6b6c 6564 5f66 756e 6322 3a20 636c 6f75  kled_func": clou
-00001da0: 6470 6963 6b6c 652e 6475 6d70 7328 6675  dpickle.dumps(fu
-00001db0: 6e63 292c 0a20 2020 207d 0a0a 2020 2020  nc),.    }..    
-00001dc0: 2320 476f 210a 2020 2020 7265 7475 726e  # Go!.    return
-00001dd0: 205f 6170 706c 795f 6765 6f6f 7065 7261   _apply_geoopera
-00001de0: 7469 6f6e 5f74 6f5f 6c61 7965 7228 0a20  tion_to_layer(. 
-00001df0: 2020 2020 2020 2069 6e70 7574 5f70 6174         input_pat
-00001e00: 683d 696e 7075 745f 7061 7468 2c0a 2020  h=input_path,.  
-00001e10: 2020 2020 2020 6f75 7470 7574 5f70 6174        output_pat
-00001e20: 683d 6f75 7470 7574 5f70 6174 682c 0a20  h=output_path,. 
-00001e30: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
-00001e40: 3d47 656f 4f70 6572 6174 696f 6e2e 4150  =GeoOperation.AP
-00001e50: 504c 592c 0a20 2020 2020 2020 206f 7065  PLY,.        ope
-00001e60: 7261 7469 6f6e 5f70 6172 616d 733d 6f70  ration_params=op
-00001e70: 6572 6174 696f 6e5f 7061 7261 6d73 2c0a  eration_params,.
-00001e80: 2020 2020 2020 2020 696e 7075 745f 6c61          input_la
-00001e90: 7965 723d 696e 7075 745f 6c61 7965 722c  yer=input_layer,
-00001ea0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-00001eb0: 6c61 7965 723d 6f75 7470 7574 5f6c 6179  layer=output_lay
-00001ec0: 6572 2c0a 2020 2020 2020 2020 636f 6c75  er,.        colu
-00001ed0: 6d6e 733d 636f 6c75 6d6e 732c 0a20 2020  mns=columns,.   
-00001ee0: 2020 2020 2065 7870 6c6f 6465 636f 6c6c       explodecoll
-00001ef0: 6563 7469 6f6e 733d 6578 706c 6f64 6563  ections=explodec
-00001f00: 6f6c 6c65 6374 696f 6e73 2c0a 2020 2020  ollections,.    
-00001f10: 2020 2020 666f 7263 655f 6f75 7470 7574      force_output
-00001f20: 5f67 656f 6d65 7472 7974 7970 653d 666f  _geometrytype=fo
-00001f30: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
-00001f40: 7472 7974 7970 652c 0a20 2020 2020 2020  trytype,.       
-00001f50: 206e 625f 7061 7261 6c6c 656c 3d6e 625f   nb_parallel=nb_
-00001f60: 7061 7261 6c6c 656c 2c0a 2020 2020 2020  parallel,.      
-00001f70: 2020 6261 7463 6873 697a 653d 6261 7463    batchsize=batc
-00001f80: 6873 697a 652c 0a20 2020 2020 2020 2066  hsize,.        f
-00001f90: 6f72 6365 3d66 6f72 6365 2c0a 2020 2020  orce=force,.    
-00001fa0: 290a 0a0a 6465 6620 6275 6666 6572 280a  )...def buffer(.
-00001fb0: 2020 2020 696e 7075 745f 7061 7468 3a20      input_path: 
-00001fc0: 5061 7468 2c0a 2020 2020 6f75 7470 7574  Path,.    output
-00001fd0: 5f70 6174 683a 2050 6174 682c 0a20 2020  _path: Path,.   
-00001fe0: 2064 6973 7461 6e63 653a 2066 6c6f 6174   distance: float
-00001ff0: 2c0a 2020 2020 7175 6164 7261 6e74 7365  ,.    quadrantse
-00002000: 676d 656e 7473 3a20 696e 7420 3d20 352c  gments: int = 5,
-00002010: 0a20 2020 2065 6e64 6361 705f 7374 796c  .    endcap_styl
-00002020: 653a 2042 7566 6665 7245 6e64 4361 7053  e: BufferEndCapS
-00002030: 7479 6c65 203d 2042 7566 6665 7245 6e64  tyle = BufferEnd
-00002040: 4361 7053 7479 6c65 2e52 4f55 4e44 2c0a  CapStyle.ROUND,.
-00002050: 2020 2020 6a6f 696e 5f73 7479 6c65 3a20      join_style: 
-00002060: 4275 6666 6572 4a6f 696e 5374 796c 6520  BufferJoinStyle 
-00002070: 3d20 4275 6666 6572 4a6f 696e 5374 796c  = BufferJoinStyl
-00002080: 652e 524f 554e 442c 0a20 2020 206d 6974  e.ROUND,.    mit
-00002090: 7265 5f6c 696d 6974 3a20 666c 6f61 7420  re_limit: float 
-000020a0: 3d20 352e 302c 0a20 2020 2073 696e 676c  = 5.0,.    singl
-000020b0: 655f 7369 6465 643a 2062 6f6f 6c20 3d20  e_sided: bool = 
-000020c0: 4661 6c73 652c 0a20 2020 2069 6e70 7574  False,.    input
-000020d0: 5f6c 6179 6572 3a20 4f70 7469 6f6e 616c  _layer: Optional
-000020e0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-000020f0: 2020 6f75 7470 7574 5f6c 6179 6572 3a20    output_layer: 
-00002100: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00002110: 4e6f 6e65 2c0a 2020 2020 636f 6c75 6d6e  None,.    column
-00002120: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-00002130: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
-00002140: 2020 2065 7870 6c6f 6465 636f 6c6c 6563     explodecollec
-00002150: 7469 6f6e 733a 2062 6f6f 6c20 3d20 4661  tions: bool = Fa
-00002160: 6c73 652c 0a20 2020 206e 625f 7061 7261  lse,.    nb_para
-00002170: 6c6c 656c 3a20 696e 7420 3d20 2d31 2c0a  llel: int = -1,.
-00002180: 2020 2020 6261 7463 6873 697a 653a 2069      batchsize: i
-00002190: 6e74 203d 202d 312c 0a20 2020 2066 6f72  nt = -1,.    for
-000021a0: 6365 3a20 626f 6f6c 203d 2046 616c 7365  ce: bool = False
-000021b0: 2c0a 293a 0a20 2020 2023 2049 6e69 740a  ,.):.    # Init.
-000021c0: 2020 2020 6f70 6572 6174 696f 6e5f 7061      operation_pa
-000021d0: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
-000021e0: 2022 6469 7374 616e 6365 223a 2064 6973   "distance": dis
-000021f0: 7461 6e63 652c 0a20 2020 2020 2020 2022  tance,.        "
-00002200: 7175 6164 7261 6e74 7365 676d 656e 7473  quadrantsegments
-00002210: 223a 2071 7561 6472 616e 7473 6567 6d65  ": quadrantsegme
-00002220: 6e74 732c 0a20 2020 2020 2020 2022 656e  nts,.        "en
-00002230: 6463 6170 5f73 7479 6c65 223a 2065 6e64  dcap_style": end
-00002240: 6361 705f 7374 796c 652c 0a20 2020 2020  cap_style,.     
-00002250: 2020 2022 6a6f 696e 5f73 7479 6c65 223a     "join_style":
-00002260: 206a 6f69 6e5f 7374 796c 652c 0a20 2020   join_style,.   
-00002270: 2020 2020 2022 6d69 7472 655f 6c69 6d69       "mitre_limi
-00002280: 7422 3a20 6d69 7472 655f 6c69 6d69 742c  t": mitre_limit,
-00002290: 0a20 2020 2020 2020 2022 7369 6e67 6c65  .        "single
-000022a0: 5f73 6964 6564 223a 2073 696e 676c 655f  _sided": single_
-000022b0: 7369 6465 642c 0a20 2020 207d 0a0a 2020  sided,.    }..  
-000022c0: 2020 2320 4275 6666 6572 206f 7065 7261    # Buffer opera
-000022d0: 7469 6f6e 2061 6c77 6179 7320 7265 7375  tion always resu
-000022e0: 6c74 7320 696e 2070 6f6c 7967 6f6e 732e  lts in polygons.
-000022f0: 2e2e 0a20 2020 2069 6620 6578 706c 6f64  ...    if explod
-00002300: 6563 6f6c 6c65 6374 696f 6e73 3a0a 2020  ecollections:.  
-00002310: 2020 2020 2020 666f 7263 655f 6f75 7470        force_outp
-00002320: 7574 5f67 656f 6d65 7472 7974 7970 6520  ut_geometrytype 
-00002330: 3d20 4765 6f6d 6574 7279 5479 7065 2e50  = GeometryType.P
-00002340: 4f4c 5947 4f4e 2e6e 616d 650a 2020 2020  OLYGON.name.    
-00002350: 656c 7365 3a0a 2020 2020 2020 2020 666f  else:.        fo
-00002360: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
-00002370: 7472 7974 7970 6520 3d20 4765 6f6d 6574  trytype = Geomet
-00002380: 7279 5479 7065 2e4d 554c 5449 504f 4c59  ryType.MULTIPOLY
-00002390: 474f 4e2e 6e61 6d65 0a0a 2020 2020 2320  GON.name..    # 
-000023a0: 476f 210a 2020 2020 7265 7475 726e 205f  Go!.    return _
-000023b0: 6170 706c 795f 6765 6f6f 7065 7261 7469  apply_geooperati
-000023c0: 6f6e 5f74 6f5f 6c61 7965 7228 0a20 2020  on_to_layer(.   
-000023d0: 2020 2020 2069 6e70 7574 5f70 6174 683d       input_path=
-000023e0: 696e 7075 745f 7061 7468 2c0a 2020 2020  input_path,.    
-000023f0: 2020 2020 6f75 7470 7574 5f70 6174 683d      output_path=
-00002400: 6f75 7470 7574 5f70 6174 682c 0a20 2020  output_path,.   
-00002410: 2020 2020 206f 7065 7261 7469 6f6e 3d47       operation=G
-00002420: 656f 4f70 6572 6174 696f 6e2e 4255 4646  eoOperation.BUFF
-00002430: 4552 2c0a 2020 2020 2020 2020 6f70 6572  ER,.        oper
-00002440: 6174 696f 6e5f 7061 7261 6d73 3d6f 7065  ation_params=ope
-00002450: 7261 7469 6f6e 5f70 6172 616d 732c 0a20  ration_params,. 
-00002460: 2020 2020 2020 2069 6e70 7574 5f6c 6179         input_lay
-00002470: 6572 3d69 6e70 7574 5f6c 6179 6572 2c0a  er=input_layer,.
-00002480: 2020 2020 2020 2020 6f75 7470 7574 5f6c          output_l
-00002490: 6179 6572 3d6f 7574 7075 745f 6c61 7965  ayer=output_laye
-000024a0: 722c 0a20 2020 2020 2020 2063 6f6c 756d  r,.        colum
-000024b0: 6e73 3d63 6f6c 756d 6e73 2c0a 2020 2020  ns=columns,.    
-000024c0: 2020 2020 6578 706c 6f64 6563 6f6c 6c65      explodecolle
-000024d0: 6374 696f 6e73 3d65 7870 6c6f 6465 636f  ctions=explodeco
-000024e0: 6c6c 6563 7469 6f6e 732c 0a20 2020 2020  llections,.     
-000024f0: 2020 2066 6f72 6365 5f6f 7574 7075 745f     force_output_
-00002500: 6765 6f6d 6574 7279 7479 7065 3d66 6f72  geometrytype=for
-00002510: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
-00002520: 7279 7479 7065 2c0a 2020 2020 2020 2020  rytype,.        
-00002530: 6e62 5f70 6172 616c 6c65 6c3d 6e62 5f70  nb_parallel=nb_p
-00002540: 6172 616c 6c65 6c2c 0a20 2020 2020 2020  arallel,.       
-00002550: 2062 6174 6368 7369 7a65 3d62 6174 6368   batchsize=batch
-00002560: 7369 7a65 2c0a 2020 2020 2020 2020 666f  size,.        fo
-00002570: 7263 653d 666f 7263 652c 0a20 2020 2029  rce=force,.    )
-00002580: 0a0a 0a64 6566 2063 6f6e 7665 7868 756c  ...def convexhul
-00002590: 6c28 0a20 2020 2069 6e70 7574 5f70 6174  l(.    input_pat
-000025a0: 683a 2050 6174 682c 0a20 2020 206f 7574  h: Path,.    out
-000025b0: 7075 745f 7061 7468 3a20 5061 7468 2c0a  put_path: Path,.
-000025c0: 2020 2020 696e 7075 745f 6c61 7965 723a      input_layer:
-000025d0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-000025e0: 204e 6f6e 652c 0a20 2020 206f 7574 7075   None,.    outpu
-000025f0: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
-00002600: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00002610: 2020 2063 6f6c 756d 6e73 3a20 4f70 7469     columns: Opti
-00002620: 6f6e 616c 5b4c 6973 745b 7374 725d 5d20  onal[List[str]] 
-00002630: 3d20 4e6f 6e65 2c0a 2020 2020 6578 706c  = None,.    expl
-00002640: 6f64 6563 6f6c 6c65 6374 696f 6e73 3a20  odecollections: 
-00002650: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00002660: 2020 6e62 5f70 6172 616c 6c65 6c3a 2069    nb_parallel: i
-00002670: 6e74 203d 202d 312c 0a20 2020 2062 6174  nt = -1,.    bat
-00002680: 6368 7369 7a65 3a20 696e 7420 3d20 2d31  chsize: int = -1
-00002690: 2c0a 2020 2020 666f 7263 653a 2062 6f6f  ,.    force: boo
-000026a0: 6c20 3d20 4661 6c73 652c 0a29 3a0a 2020  l = False,.):.  
-000026b0: 2020 2320 496e 6974 0a20 2020 206f 7065    # Init.    ope
-000026c0: 7261 7469 6f6e 5f70 6172 616d 7320 3d20  ration_params = 
-000026d0: 7b7d 0a0a 2020 2020 2320 476f 210a 2020  {}..    # Go!.  
-000026e0: 2020 7265 7475 726e 205f 6170 706c 795f    return _apply_
-000026f0: 6765 6f6f 7065 7261 7469 6f6e 5f74 6f5f  geooperation_to_
-00002700: 6c61 7965 7228 0a20 2020 2020 2020 2069  layer(.        i
-00002710: 6e70 7574 5f70 6174 683d 696e 7075 745f  nput_path=input_
-00002720: 7061 7468 2c0a 2020 2020 2020 2020 6f75  path,.        ou
-00002730: 7470 7574 5f70 6174 683d 6f75 7470 7574  tput_path=output
-00002740: 5f70 6174 682c 0a20 2020 2020 2020 206f  _path,.        o
-00002750: 7065 7261 7469 6f6e 3d47 656f 4f70 6572  peration=GeoOper
-00002760: 6174 696f 6e2e 434f 4e56 4558 4855 4c4c  ation.CONVEXHULL
-00002770: 2c0a 2020 2020 2020 2020 6f70 6572 6174  ,.        operat
-00002780: 696f 6e5f 7061 7261 6d73 3d6f 7065 7261  ion_params=opera
-00002790: 7469 6f6e 5f70 6172 616d 732c 0a20 2020  tion_params,.   
-000027a0: 2020 2020 2069 6e70 7574 5f6c 6179 6572       input_layer
-000027b0: 3d69 6e70 7574 5f6c 6179 6572 2c0a 2020  =input_layer,.  
-000027c0: 2020 2020 2020 6f75 7470 7574 5f6c 6179        output_lay
-000027d0: 6572 3d6f 7574 7075 745f 6c61 7965 722c  er=output_layer,
-000027e0: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
-000027f0: 3d63 6f6c 756d 6e73 2c0a 2020 2020 2020  =columns,.      
-00002800: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
-00002810: 696f 6e73 3d65 7870 6c6f 6465 636f 6c6c  ions=explodecoll
-00002820: 6563 7469 6f6e 732c 0a20 2020 2020 2020  ections,.       
-00002830: 206e 625f 7061 7261 6c6c 656c 3d6e 625f   nb_parallel=nb_
-00002840: 7061 7261 6c6c 656c 2c0a 2020 2020 2020  parallel,.      
-00002850: 2020 6261 7463 6873 697a 653d 6261 7463    batchsize=batc
-00002860: 6873 697a 652c 0a20 2020 2020 2020 2066  hsize,.        f
-00002870: 6f72 6365 3d66 6f72 6365 2c0a 2020 2020  orce=force,.    
-00002880: 290a 0a0a 6465 6620 7369 6d70 6c69 6679  )...def simplify
-00002890: 280a 2020 2020 696e 7075 745f 7061 7468  (.    input_path
-000028a0: 3a20 5061 7468 2c0a 2020 2020 6f75 7470  : Path,.    outp
-000028b0: 7574 5f70 6174 683a 2050 6174 682c 0a20  ut_path: Path,. 
-000028c0: 2020 2074 6f6c 6572 616e 6365 3a20 666c     tolerance: fl
-000028d0: 6f61 742c 0a20 2020 2061 6c67 6f72 6974  oat,.    algorit
-000028e0: 686d 3a20 5369 6d70 6c69 6679 416c 676f  hm: SimplifyAlgo
-000028f0: 7269 7468 6d20 3d20 5369 6d70 6c69 6679  rithm = Simplify
-00002900: 416c 676f 7269 7468 6d2e 5241 4d45 525f  Algorithm.RAMER_
-00002910: 444f 5547 4c41 535f 5045 5543 4b45 522c  DOUGLAS_PEUCKER,
-00002920: 0a20 2020 206c 6f6f 6b61 6865 6164 3a20  .    lookahead: 
-00002930: 696e 7420 3d20 382c 0a20 2020 2069 6e70  int = 8,.    inp
-00002940: 7574 5f6c 6179 6572 3a20 4f70 7469 6f6e  ut_layer: Option
-00002950: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00002960: 2020 2020 6f75 7470 7574 5f6c 6179 6572      output_layer
-00002970: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00002980: 3d20 4e6f 6e65 2c0a 2020 2020 636f 6c75  = None,.    colu
-00002990: 6d6e 733a 204f 7074 696f 6e61 6c5b 4c69  mns: Optional[Li
-000029a0: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
-000029b0: 0a20 2020 2065 7870 6c6f 6465 636f 6c6c  .    explodecoll
-000029c0: 6563 7469 6f6e 733a 2062 6f6f 6c20 3d20  ections: bool = 
-000029d0: 4661 6c73 652c 0a20 2020 206e 625f 7061  False,.    nb_pa
-000029e0: 7261 6c6c 656c 3a20 696e 7420 3d20 2d31  rallel: int = -1
-000029f0: 2c0a 2020 2020 6261 7463 6873 697a 653a  ,.    batchsize:
-00002a00: 2069 6e74 203d 202d 312c 0a20 2020 2066   int = -1,.    f
-00002a10: 6f72 6365 3a20 626f 6f6c 203d 2046 616c  orce: bool = Fal
-00002a20: 7365 2c0a 293a 0a20 2020 2023 2049 6e69  se,.):.    # Ini
-00002a30: 740a 2020 2020 6f70 6572 6174 696f 6e5f  t.    operation_
-00002a40: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
-00002a50: 2020 2022 746f 6c65 7261 6e63 6522 3a20     "tolerance": 
-00002a60: 746f 6c65 7261 6e63 652c 0a20 2020 2020  tolerance,.     
-00002a70: 2020 2022 616c 676f 7269 7468 6d22 3a20     "algorithm": 
-00002a80: 616c 676f 7269 7468 6d2c 0a20 2020 2020  algorithm,.     
-00002a90: 2020 2022 7374 6570 223a 206c 6f6f 6b61     "step": looka
-00002aa0: 6865 6164 2c0a 2020 2020 7d0a 0a20 2020  head,.    }..   
-00002ab0: 2023 2047 6f21 0a20 2020 2072 6574 7572   # Go!.    retur
-00002ac0: 6e20 5f61 7070 6c79 5f67 656f 6f70 6572  n _apply_geooper
-00002ad0: 6174 696f 6e5f 746f 5f6c 6179 6572 280a  ation_to_layer(.
-00002ae0: 2020 2020 2020 2020 696e 7075 745f 7061          input_pa
-00002af0: 7468 3d69 6e70 7574 5f70 6174 682c 0a20  th=input_path,. 
-00002b00: 2020 2020 2020 206f 7574 7075 745f 7061         output_pa
-00002b10: 7468 3d6f 7574 7075 745f 7061 7468 2c0a  th=output_path,.
-00002b20: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-00002b30: 6e3d 4765 6f4f 7065 7261 7469 6f6e 2e53  n=GeoOperation.S
-00002b40: 494d 504c 4946 592c 0a20 2020 2020 2020  IMPLIFY,.       
-00002b50: 206f 7065 7261 7469 6f6e 5f70 6172 616d   operation_param
-00002b60: 733d 6f70 6572 6174 696f 6e5f 7061 7261  s=operation_para
-00002b70: 6d73 2c0a 2020 2020 2020 2020 696e 7075  ms,.        inpu
-00002b80: 745f 6c61 7965 723d 696e 7075 745f 6c61  t_layer=input_la
-00002b90: 7965 722c 0a20 2020 2020 2020 206f 7574  yer,.        out
-00002ba0: 7075 745f 6c61 7965 723d 6f75 7470 7574  put_layer=output
-00002bb0: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
-00002bc0: 636f 6c75 6d6e 733d 636f 6c75 6d6e 732c  columns=columns,
-00002bd0: 0a20 2020 2020 2020 2065 7870 6c6f 6465  .        explode
-00002be0: 636f 6c6c 6563 7469 6f6e 733d 6578 706c  collections=expl
-00002bf0: 6f64 6563 6f6c 6c65 6374 696f 6e73 2c0a  odecollections,.
-00002c00: 2020 2020 2020 2020 6e62 5f70 6172 616c          nb_paral
-00002c10: 6c65 6c3d 6e62 5f70 6172 616c 6c65 6c2c  lel=nb_parallel,
-00002c20: 0a20 2020 2020 2020 2062 6174 6368 7369  .        batchsi
-00002c30: 7a65 3d62 6174 6368 7369 7a65 2c0a 2020  ze=batchsize,.  
-00002c40: 2020 2020 2020 666f 7263 653d 666f 7263        force=forc
-00002c50: 652c 0a20 2020 2029 0a0a 0a64 6566 205f  e,.    )...def _
-00002c60: 6170 706c 795f 6765 6f6f 7065 7261 7469  apply_geooperati
-00002c70: 6f6e 5f74 6f5f 6c61 7965 7228 0a20 2020  on_to_layer(.   
-00002c80: 2069 6e70 7574 5f70 6174 683a 2050 6174   input_path: Pat
-00002c90: 682c 0a20 2020 206f 7574 7075 745f 7061  h,.    output_pa
-00002ca0: 7468 3a20 5061 7468 2c0a 2020 2020 6f70  th: Path,.    op
-00002cb0: 6572 6174 696f 6e3a 2047 656f 4f70 6572  eration: GeoOper
-00002cc0: 6174 696f 6e2c 0a20 2020 206f 7065 7261  ation,.    opera
-00002cd0: 7469 6f6e 5f70 6172 616d 733a 2064 6963  tion_params: dic
-00002ce0: 742c 0a20 2020 2069 6e70 7574 5f6c 6179  t,.    input_lay
-00002cf0: 6572 3a20 4f70 7469 6f6e 616c 5b73 7472  er: Optional[str
-00002d00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 636f  ] = None,.    co
-00002d10: 6c75 6d6e 733a 204f 7074 696f 6e61 6c5b  lumns: Optional[
-00002d20: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
-00002d30: 652c 0a20 2020 206f 7574 7075 745f 6c61  e,.    output_la
-00002d40: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
-00002d50: 725d 203d 204e 6f6e 652c 0a20 2020 2065  r] = None,.    e
-00002d60: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
-00002d70: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-00002d80: 0a20 2020 2066 6f72 6365 5f6f 7574 7075  .    force_outpu
-00002d90: 745f 6765 6f6d 6574 7279 7479 7065 3a20  t_geometrytype: 
-00002da0: 556e 696f 6e5b 4765 6f6d 6574 7279 5479  Union[GeometryTy
-00002db0: 7065 2c20 7374 722c 204e 6f6e 655d 203d  pe, str, None] =
-00002dc0: 204e 6f6e 652c 0a20 2020 206e 625f 7061   None,.    nb_pa
-00002dd0: 7261 6c6c 656c 3a20 696e 7420 3d20 2d31  rallel: int = -1
-00002de0: 2c0a 2020 2020 6261 7463 6873 697a 653a  ,.    batchsize:
-00002df0: 2069 6e74 203d 202d 312c 0a20 2020 2066   int = -1,.    f
-00002e00: 6f72 6365 3a20 626f 6f6c 203d 2046 616c  orce: bool = Fal
-00002e10: 7365 2c0a 293a 0a20 2020 2022 2222 0a20  se,.):.    """. 
-00002e20: 2020 2041 7070 6c69 6573 2061 2067 656f     Applies a geo
-00002e30: 206f 7065 7261 7469 6f6e 206f 6e20 6120   operation on a 
-00002e40: 6c61 7965 722e 0a0a 2020 2020 5468 6520  layer...    The 
-00002e50: 6f70 6572 6174 696f 6e20 746f 2061 7070  operation to app
-00002e60: 6c79 2063 616e 2062 6520 6f6e 6520 6f66  ly can be one of
-00002e70: 2074 6865 2074 6865 2066 6f6c 6c6f 7769   the the followi
-00002e80: 6e67 3a0a 2020 2020 2020 2d20 4255 4646  ng:.      - BUFF
-00002e90: 4552 3a20 6170 706c 7920 6120 6275 6666  ER: apply a buff
-00002ea0: 6572 2e20 4f70 6572 6174 696f 6e20 7061  er. Operation pa
-00002eb0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00002ec0: 2020 2020 2d20 6469 7374 616e 6365 3a20      - distance: 
-00002ed0: 6469 7374 616e 6365 2074 6f20 6275 6666  distance to buff
-00002ee0: 6572 0a20 2020 2020 2020 2020 202d 2071  er.          - q
-00002ef0: 7561 6472 616e 7473 6567 6d65 6e74 733a  uadrantsegments:
-00002f00: 206e 756d 6265 7220 6f66 2070 6f69 6e74   number of point
-00002f10: 7320 7573 6564 2074 6f20 7265 7072 6573  s used to repres
-00002f20: 656e 7420 312f 3420 6f66 2061 2063 6972  ent 1/4 of a cir
-00002f30: 636c 650a 2020 2020 2020 2020 2020 2d20  cle.          - 
-00002f40: 656e 6463 6170 5f73 7479 6c65 3a20 6275  endcap_style: bu
-00002f50: 6666 6572 2073 7479 6c65 2074 6f20 7573  ffer style to us
-00002f60: 6520 666f 7220 6120 706f 696e 7420 6f72  e for a point or
-00002f70: 2074 6865 2065 6e64 2070 6f69 6e74 7320   the end points 
-00002f80: 6f66 0a20 2020 2020 2020 2020 2020 2061  of.            a
-00002f90: 206c 696e 653a 0a20 2020 2020 2020 2020   line:.         
-00002fa0: 2020 202d 2052 4f55 4e44 3a20 666f 7220     - ROUND: for 
-00002fb0: 706f 696e 7473 2061 6e64 206c 696e 6573  points and lines
-00002fc0: 2074 6865 2065 6e64 7320 6172 6520 6275   the ends are bu
-00002fd0: 6666 6572 6564 2072 6f75 6e64 6564 2e0a  ffered rounded..
-00002fe0: 2020 2020 2020 2020 2020 2020 2d20 464c              - FL
-00002ff0: 4154 3a20 6120 706f 696e 7420 7374 6179  AT: a point stay
-00003000: 7320 6120 706f 696e 742c 2061 2062 7566  s a point, a buf
-00003010: 6665 7265 6420 6c69 6e65 2077 696c 6c20  fered line will 
-00003020: 656e 6420 666c 6174 0a20 2020 2020 2020  end flat.       
-00003030: 2020 2020 2020 2061 7420 7468 6520 656e         at the en
-00003040: 6420 706f 696e 7473 0a20 2020 2020 2020  d points.       
-00003050: 2020 2020 202d 2053 5155 4152 453a 2061       - SQUARE: a
-00003060: 2070 6f69 6e74 2062 6563 6f6d 6573 2061   point becomes a
-00003070: 2073 7175 6172 652c 2061 2062 7566 6665   square, a buffe
-00003080: 7265 6420 6c69 6e65 2077 696c 6c20 656e  red line will en
-00003090: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-000030a0: 666c 6174 2061 7420 7468 6520 656e 6420  flat at the end 
-000030b0: 706f 696e 7473 2c20 6275 7420 656c 6f6e  points, but elon
-000030c0: 6761 7465 6420 6279 2022 6469 7374 616e  gated by "distan
-000030d0: 6365 220a 2020 2020 2020 2020 2d20 6a6f  ce".        - jo
-000030e0: 696e 5f73 7479 6c65 3a20 6275 6666 6572  in_style: buffer
-000030f0: 2073 7479 6c65 2074 6f20 7573 6520 666f   style to use fo
-00003100: 7220 636f 726e 6572 7320 696e 2061 206c  r corners in a l
-00003110: 696e 6520 6f72 2061 2070 6f6c 7967 6f6e  ine or a polygon
-00003120: 0a20 2020 2020 2020 2020 2062 6f75 6e64  .          bound
-00003130: 6172 793a 0a20 2020 2020 2020 2020 2020  ary:.           
-00003140: 202d 2052 4f55 4e44 3a20 636f 726e 6572   - ROUND: corner
-00003150: 7320 696e 2074 6865 2072 6573 756c 7420  s in the result 
-00003160: 6172 6520 726f 756e 6465 640a 2020 2020  are rounded.    
-00003170: 2020 2020 2020 2020 2d20 4d49 5452 453a          - MITRE:
-00003180: 2063 6f72 6e65 7273 2069 6e20 7468 6520   corners in the 
-00003190: 7265 7375 6c74 2061 7265 2073 6861 7270  result are sharp
-000031a0: 0a20 2020 2020 2020 2020 2020 202d 2042  .            - B
-000031b0: 4556 454c 3a20 6172 6520 666c 6174 7465  EVEL: are flatte
-000031c0: 6e65 640a 2020 2020 2020 2020 2d20 6d69  ned.        - mi
-000031d0: 7472 655f 6c69 6d69 743a 2069 6e20 6361  tre_limit: in ca
-000031e0: 7365 206f 6620 6a6f 696e 5f73 7479 6c65  se of join_style
-000031f0: 204d 4954 5245 2c20 6966 2074 6865 0a20   MITRE, if the. 
-00003200: 2020 2020 2020 2020 2020 2073 7069 6b79             spiky
-00003210: 2072 6573 756c 7420 666f 7220 6120 7368   result for a sh
-00003220: 6172 7020 616e 676c 6520 6265 636f 6d65  arp angle become
-00003230: 7320 6c6f 6e67 6572 2074 6861 6e20 7468  s longer than th
-00003240: 6973 206c 696d 6974 2c20 6974 0a20 2020  is limit, it.   
-00003250: 2020 2020 2020 2020 2069 7320 2262 6576           is "bev
-00003260: 656c 6564 2220 6174 2074 6869 7320 6469  eled" at this di
-00003270: 7374 616e 6365 2e20 4465 6661 756c 7473  stance. Defaults
-00003280: 2074 6f20 352e 302e 0a20 2020 2020 2020   to 5.0..       
-00003290: 202d 2073 696e 676c 655f 7369 6465 643a   - single_sided:
-000032a0: 206f 6e6c 7920 6f6e 6520 7369 6465 206f   only one side o
-000032b0: 6620 7468 6520 6c69 6e65 2069 7320 6275  f the line is bu
-000032c0: 6666 6572 6564 2c0a 2020 2020 2020 2020  ffered,.        
-000032d0: 2020 2020 6966 2064 6973 7461 6e63 6520      if distance 
-000032e0: 6973 206e 6567 6174 6976 652c 2074 6865  is negative, the
-000032f0: 206c 6566 7420 7369 6465 2c20 6966 2064   left side, if d
-00003300: 6973 7461 6e63 6520 6973 2070 6f73 6974  istance is posit
-00003310: 6976 652c 0a20 2020 2020 2020 2020 2020  ive,.           
-00003320: 2074 6865 2072 6967 6874 2068 616e 6420   the right hand 
-00003330: 7369 6465 2e20 4f6e 6c79 2072 656c 6576  side. Only relev
-00003340: 616e 7420 666f 7220 6c69 6e65 2067 656f  ant for line geo
-00003350: 6d65 7472 6965 732e 0a20 2020 2020 202d  metries..      -
-00003360: 2043 4f4e 5645 5848 554c 4c3a 2061 7070   CONVEXHULL: app
-00003370: 7920 6120 636f 6e76 6578 2068 756c 6c2e  y a convex hull.
-00003380: 0a20 2020 2020 202d 2053 494d 504c 4946  .      - SIMPLIF
-00003390: 593a 2073 696d 706c 6966 7920 7468 6520  Y: simplify the 
-000033a0: 6765 6f6d 6574 7279 2e20 4f70 6572 6174  geometry. Operat
-000033b0: 696f 6e20 7061 7261 6d65 7465 7273 3a0a  ion parameters:.
-000033c0: 2020 2020 2020 2020 2020 2d20 616c 676f            - algo
-000033d0: 7269 7468 6d3a 2076 6563 746f 725f 7574  rithm: vector_ut
-000033e0: 696c 2e53 696d 706c 6966 7941 6c67 6f72  il.SimplifyAlgor
-000033f0: 6974 686d 0a20 2020 2020 2020 2020 202d  ithm.          -
-00003400: 2074 6f6c 6572 616e 6365 3a20 6d61 7869   tolerance: maxi
-00003410: 6d75 6d20 6469 7374 616e 6365 2074 6f20  mum distance to 
-00003420: 7369 6d70 6c69 6679 2e0a 2020 2020 2020  simplify..      
-00003430: 2020 2020 2d20 6c6f 6f6b 6168 6561 643a      - lookahead:
-00003440: 2066 6f72 204c 414e 472c 2074 6865 206e   for LANG, the n
-00003450: 756d 6265 7220 6f66 2070 6f69 6e74 7320  umber of points 
-00003460: 746f 2066 6f72 7761 7264 2d6c 6f6f 6b0a  to forward-look.
-00003470: 2020 2020 2020 2d20 4150 504c 593a 2061        - APPLY: a
-00003480: 7070 6c79 2061 206c 616d 6264 6120 6675  pply a lambda fu
-00003490: 6e63 7469 6f6e 2e20 4f70 6572 6174 696f  nction. Operatio
-000034a0: 6e20 7061 7261 6d65 7465 723a 0a20 2020  n parameter:.   
-000034b0: 2020 2020 2020 202d 2070 6963 6b6c 6564         - pickled
-000034c0: 5f66 756e 633a 206c 616d 6264 6120 6675  _func: lambda fu
-000034d0: 6e63 7469 6f6e 2074 6f20 6170 706c 792c  nction to apply,
-000034e0: 2070 6963 6b6c 6564 2074 6f20 6279 7465   pickled to byte
-000034f0: 732e 0a20 2020 2020 2020 2020 202d 206f  s..          - o
-00003500: 6e6c 795f 6765 6f6d 5f69 6e70 7574 3a20  nly_geom_input: 
-00003510: 6966 2054 7275 652c 206f 6e6c 7920 7468  if True, only th
-00003520: 6520 6765 6f6d 6574 7279 2069 7320 6176  e geometry is av
-00003530: 6169 6c61 626c 6520 6173 0a20 2020 2020  ailable as.     
-00003540: 2020 2020 2020 2069 6e70 7574 2066 6f72         input for
-00003550: 2074 6865 206c 616d 6264 6120 6675 6e63   the lambda func
-00003560: 7469 6f6e 2e20 4966 2066 616c 7365 2c20  tion. If false, 
-00003570: 7468 6520 726f 7720 6973 2074 6865 2069  the row is the i
-00003580: 6e70 7574 2e0a 0a20 2020 2041 7267 733a  nput...    Args:
-00003590: 0a20 2020 2020 2020 2069 6e70 7574 5f70  .        input_p
-000035a0: 6174 6820 2850 6174 6829 3a20 5b64 6573  ath (Path): [des
-000035b0: 6372 6970 7469 6f6e 5d0a 2020 2020 2020  cription].      
-000035c0: 2020 6f75 7470 7574 5f70 6174 6820 2850    output_path (P
-000035d0: 6174 6829 3a20 5b64 6573 6372 6970 7469  ath): [descripti
-000035e0: 6f6e 5d0a 2020 2020 2020 2020 6f70 6572  on].        oper
-000035f0: 6174 696f 6e20 2847 656f 4f70 6572 6174  ation (GeoOperat
-00003600: 696f 6e29 3a20 7468 6520 6765 6f20 6f70  ion): the geo op
-00003610: 6572 6174 696f 6e20 746f 2061 7070 6c79  eration to apply
-00003620: 2e0a 2020 2020 2020 2020 6f70 6572 6174  ..        operat
-00003630: 696f 6e5f 7061 7261 6d73 2028 6469 6374  ion_params (dict
-00003640: 2c20 6f70 7469 6f6e 616c 293a 2074 6865  , optional): the
-00003650: 2070 6172 616d 6574 6572 7320 666f 7220   parameters for 
-00003660: 7468 6520 6765 6f20 6f70 6572 6174 696f  the geo operatio
-00003670: 6e2e 0a20 2020 2020 2020 2020 2020 2044  n..            D
-00003680: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-00003690: 0a20 2020 2020 2020 2069 6e70 7574 5f6c  .        input_l
-000036a0: 6179 6572 2028 7374 722c 206f 7074 696f  ayer (str, optio
-000036b0: 6e61 6c29 3a20 5b64 6573 6372 6970 7469  nal): [descripti
-000036c0: 6f6e 5d2e 2044 6566 6175 6c74 7320 746f  on]. Defaults to
-000036d0: 204e 6f6e 652e 0a20 2020 2020 2020 206f   None..        o
-000036e0: 7574 7075 745f 6c61 7965 7220 2873 7472  utput_layer (str
-000036f0: 2c20 6f70 7469 6f6e 616c 293a 205b 6465  , optional): [de
-00003700: 7363 7269 7074 696f 6e5d 2e20 4465 6661  scription]. Defa
-00003710: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-00003720: 2020 2020 2020 636f 6c75 6d6e 7320 284c        columns (L
-00003730: 6973 745b 7374 725d 2c20 6f70 7469 6f6e  ist[str], option
-00003740: 616c 293a 2049 6620 6e6f 7420 4e6f 6e65  al): If not None
-00003750: 2c20 6f6e 6c79 206f 7574 7075 7420 7468  , only output th
-00003760: 6520 636f 6c75 6d6e 730a 2020 2020 2020  e columns.      
-00003770: 2020 2020 2020 7370 6563 6966 6965 642e        specified.
-00003780: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-00003790: 652e 0a20 2020 2020 2020 2065 7870 6c6f  e..        explo
-000037a0: 6465 636f 6c6c 6563 7469 6f6e 7320 2862  decollections (b
-000037b0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-000037c0: 5472 7565 2074 6f20 636f 6e76 6572 7420  True to convert 
-000037d0: 616c 6c20 6d75 6c74 692d 6765 6f6d 6574  all multi-geomet
-000037e0: 7269 6573 2074 6f0a 2020 2020 2020 2020  ries to.        
-000037f0: 2020 2020 7369 6e67 756c 6172 206f 6e65      singular one
-00003800: 7320 6475 7269 6e67 2074 6865 2067 656f  s during the geo
-00003810: 6f70 6572 6174 696f 6e2e 2044 6566 6175  operation. Defau
-00003820: 6c74 7320 746f 2046 616c 7365 2e0a 2020  lts to False..  
-00003830: 2020 2020 2020 666f 7263 655f 6f75 7470        force_outp
-00003840: 7574 5f67 656f 6d65 7472 7974 7970 6520  ut_geometrytype 
-00003850: 2847 656f 6d65 7472 7954 7970 652c 206f  (GeometryType, o
-00003860: 7074 696f 6e61 6c29 3a20 5468 6520 6f75  ptional): The ou
-00003870: 7470 7574 2067 656f 6d65 7472 7920 7479  tput geometry ty
-00003880: 7065 2074 6f0a 2020 2020 2020 2020 2020  pe to.          
-00003890: 2020 666f 7263 652e 2049 6620 4e6f 6e65    force. If None
-000038a0: 2c20 6120 6265 7374 2d65 6666 6f72 7420  , a best-effort 
-000038b0: 6775 6573 7320 6973 206d 6164 652e 2044  guess is made. D
-000038c0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-000038d0: 0a20 2020 2020 2020 206e 625f 7061 7261  .        nb_para
-000038e0: 6c6c 656c 2028 696e 742c 206f 7074 696f  llel (int, optio
-000038f0: 6e61 6c29 3a20 5b64 6573 6372 6970 7469  nal): [descripti
-00003900: 6f6e 5d2e 2044 6566 6175 6c74 7320 746f  on]. Defaults to
-00003910: 202d 312e 0a20 2020 2020 2020 2062 6174   -1..        bat
-00003920: 6368 7369 7a65 2028 696e 742c 206f 7074  chsize (int, opt
-00003930: 696f 6e61 6c29 3a20 696e 6469 6361 7469  ional): indicati
-00003940: 7665 206e 756d 6265 7220 6f66 2072 6f77  ve number of row
-00003950: 7320 746f 2070 726f 6365 7373 2070 6572  s to process per
-00003960: 0a20 2020 2020 2020 2020 2020 2062 6174  .            bat
-00003970: 6368 2e20 4120 736d 616c 6c65 7220 6261  ch. A smaller ba
-00003980: 7463 6820 7369 7a65 2c20 706f 7373 6962  tch size, possib
-00003990: 6c79 2069 6e20 636f 6d62 696e 6174 696f  ly in combinatio
-000039a0: 6e20 7769 7468 2061 0a20 2020 2020 2020  n with a.       
-000039b0: 2020 2020 2073 6d61 6c6c 6572 206e 625f       smaller nb_
-000039c0: 7061 7261 6c6c 656c 2c20 7769 6c6c 2072  parallel, will r
-000039d0: 6564 7563 6520 7468 6520 6d65 6d6f 7279  educe the memory
-000039e0: 2075 7361 6765 2e0a 2020 2020 2020 2020   usage..        
-000039f0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00003a00: 2d31 3a20 2874 7279 2074 6f29 2064 6574  -1: (try to) det
-00003a10: 6572 6d69 6e65 206f 7074 696d 616c 2073  ermine optimal s
-00003a20: 697a 6520 6175 746f 6d61 7469 6361 6c6c  ize automaticall
-00003a30: 792e 0a20 2020 2020 2020 2066 6f72 6365  y..        force
-00003a40: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-00003a50: 293a 205b 6465 7363 7269 7074 696f 6e5d  ): [description]
-00003a60: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
-00003a70: 6c73 652e 0a20 2020 2022 2222 0a20 2020  lse..    """.   
-00003a80: 2023 2049 6e69 740a 2020 2020 7374 6172   # Init.    star
-00003a90: 745f 7469 6d65 5f67 6c6f 6261 6c20 3d20  t_time_global = 
-00003aa0: 6461 7465 7469 6d65 2e6e 6f77 2829 0a0a  datetime.now()..
-00003ab0: 2020 2020 2320 4368 6563 6b20 696e 7075      # Check inpu
-00003ac0: 7420 7061 7261 6d65 7465 7273 2e2e 2e0a  t parameters....
-00003ad0: 2020 2020 6f70 6572 6174 696f 6e5f 6e61      operation_na
-00003ae0: 6d65 203d 206f 7065 7261 7469 6f6e 2e6e  me = operation.n
-00003af0: 616d 652e 6c6f 7765 7228 290a 2020 2020  ame.lower().    
-00003b00: 6966 206e 6f74 2069 6e70 7574 5f70 6174  if not input_pat
-00003b10: 682e 6578 6973 7473 2829 3a0a 2020 2020  h.exists():.    
-00003b20: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00003b30: 7272 6f72 2866 227b 6f70 6572 6174 696f  rror(f"{operatio
-00003b40: 6e5f 6e61 6d65 7d3a 2069 6e70 7574 5f70  n_name}: input_p
-00003b50: 6174 6820 646f 6573 6e27 7420 6578 6973  ath doesn't exis
-00003b60: 743a 207b 696e 7075 745f 7061 7468 7d22  t: {input_path}"
-00003b70: 290a 2020 2020 6966 2069 6e70 7574 5f70  ).    if input_p
-00003b80: 6174 6820 3d3d 206f 7574 7075 745f 7061  ath == output_pa
-00003b90: 7468 3a0a 2020 2020 2020 2020 7261 6973  th:.        rais
-00003ba0: 6520 5661 6c75 6545 7272 6f72 2866 227b  e ValueError(f"{
-00003bb0: 6f70 6572 6174 696f 6e5f 6e61 6d65 7d3a  operation_name}:
-00003bc0: 206f 7574 7075 745f 7061 7468 206d 7573   output_path mus
-00003bd0: 7420 6e6f 7420 6571 7561 6c20 696e 7075  t not equal inpu
-00003be0: 745f 7061 7468 2229 0a20 2020 2069 6620  t_path").    if 
-00003bf0: 696e 7075 745f 6c61 7965 7220 6973 204e  input_layer is N
-00003c00: 6f6e 653a 0a20 2020 2020 2020 2069 6e70  one:.        inp
-00003c10: 7574 5f6c 6179 6572 203d 2067 666f 2e67  ut_layer = gfo.g
-00003c20: 6574 5f6f 6e6c 795f 6c61 7965 7228 696e  et_only_layer(in
-00003c30: 7075 745f 7061 7468 290a 2020 2020 6966  put_path).    if
-00003c40: 206f 7574 7075 745f 7061 7468 2e65 7869   output_path.exi
-00003c50: 7374 7328 293a 0a20 2020 2020 2020 2069  sts():.        i
-00003c60: 6620 666f 7263 6520 6973 2046 616c 7365  f force is False
-00003c70: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00003c80: 6767 6572 2e69 6e66 6f28 6622 5374 6f70  gger.info(f"Stop
-00003c90: 207b 6f70 6572 6174 696f 6e5f 6e61 6d65   {operation_name
-00003ca0: 7d3a 206f 7574 7075 7420 6578 6973 7473  }: output exists
-00003cb0: 2061 6c72 6561 6479 207b 6f75 7470 7574   already {output
-00003cc0: 5f70 6174 687d 2229 0a20 2020 2020 2020  _path}").       
-00003cd0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00003ce0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00003cf0: 2020 2020 2020 6766 6f2e 7265 6d6f 7665        gfo.remove
-00003d00: 286f 7574 7075 745f 7061 7468 290a 2020  (output_path).  
-00003d10: 2020 6966 2069 6e70 7574 5f6c 6179 6572    if input_layer
-00003d20: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00003d30: 2020 696e 7075 745f 6c61 7965 7220 3d20    input_layer = 
-00003d40: 6766 6f2e 6765 745f 6f6e 6c79 5f6c 6179  gfo.get_only_lay
-00003d50: 6572 2869 6e70 7574 5f70 6174 6829 0a20  er(input_path). 
-00003d60: 2020 2069 6620 6f75 7470 7574 5f6c 6179     if output_lay
-00003d70: 6572 2069 7320 4e6f 6e65 3a0a 2020 2020  er is None:.    
-00003d80: 2020 2020 6f75 7470 7574 5f6c 6179 6572      output_layer
-00003d90: 203d 2067 666f 2e67 6574 5f64 6566 6175   = gfo.get_defau
-00003da0: 6c74 5f6c 6179 6572 286f 7574 7075 745f  lt_layer(output_
-00003db0: 7061 7468 290a 2020 2020 6966 2069 7369  path).    if isi
-00003dc0: 6e73 7461 6e63 6528 666f 7263 655f 6f75  nstance(force_ou
-00003dd0: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-00003de0: 652c 2047 656f 6d65 7472 7954 7970 6529  e, GeometryType)
-00003df0: 3a0a 2020 2020 2020 2020 666f 7263 655f  :.        force_
-00003e00: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
-00003e10: 7970 6520 3d20 666f 7263 655f 6f75 7470  ype = force_outp
-00003e20: 7574 5f67 656f 6d65 7472 7974 7970 652e  ut_geometrytype.
-00003e30: 6e61 6d65 0a0a 2020 2020 2320 5072 6570  name..    # Prep
-00003e40: 6172 6520 746d 7020 6669 6c65 730a 2020  are tmp files.  
-00003e50: 2020 7465 6d70 6469 7220 3d20 5f69 6f5f    tempdir = _io_
-00003e60: 7574 696c 2e63 7265 6174 655f 7465 6d70  util.create_temp
-00003e70: 6469 7228 6622 6765 6f66 696c 656f 7073  dir(f"geofileops
-00003e80: 2f7b 6f70 6572 6174 696f 6e2e 7661 6c75  /{operation.valu
-00003e90: 657d 2229 0a20 2020 206c 6f67 6765 722e  e}").    logger.
-00003ea0: 696e 666f 2866 2253 7461 7274 2063 616c  info(f"Start cal
-00003eb0: 6375 6c61 7469 6f6e 2074 6f20 7465 6d70  culation to temp
-00003ec0: 2066 696c 6573 2069 6e20 7b74 656d 7064   files in {tempd
-00003ed0: 6972 7d22 290a 0a20 2020 2023 2043 616c  ir}")..    # Cal
-00003ee0: 6375 6c61 7465 0a20 2020 2074 7279 3a0a  culate.    try:.
-00003ef0: 2020 2020 2020 2020 2320 5265 6d61 726b          # Remark
-00003f00: 3a20 6361 6c63 756c 6174 696e 6720 6361  : calculating ca
-00003f10: 6e20 6265 2064 6f6e 6520 696e 2070 6172  n be done in par
-00003f20: 616c 6c65 6c2c 2062 7574 206f 6e6c 7920  allel, but only 
-00003f30: 6f6e 6520 7072 6f63 6573 730a 2020 2020  one process.    
-00003f40: 2020 2020 2320 6361 6e20 7772 6974 6520      # can write 
-00003f50: 746f 2074 6865 2073 616d 6520 6f75 7470  to the same outp
-00003f60: 7574 2066 696c 6520 6174 2074 6865 2074  ut file at the t
-00003f70: 696d 652e 2e2e 0a0a 2020 2020 2020 2020  ime.....        
-00003f80: 2320 4361 6c63 756c 6174 6520 7468 6520  # Calculate the 
-00003f90: 6265 7374 206e 756d 6265 7220 6f66 2070  best number of p
-00003fa0: 6172 616c 6c65 6c20 7072 6f63 6573 7365  arallel processe
-00003fb0: 7320 616e 6420 6261 7463 6865 7320 666f  s and batches fo
-00003fc0: 720a 2020 2020 2020 2020 2320 7468 6520  r.        # the 
-00003fd0: 6176 6169 6c61 626c 6520 7265 736f 7572  available resour
-00003fe0: 6365 730a 2020 2020 2020 2020 696e 7075  ces.        inpu
-00003ff0: 745f 6c61 7965 7269 6e66 6f20 3d20 6766  t_layerinfo = gf
-00004000: 6f2e 6765 745f 6c61 7965 7269 6e66 6f28  o.get_layerinfo(
-00004010: 696e 7075 745f 7061 7468 2c20 696e 7075  input_path, inpu
-00004020: 745f 6c61 7965 7229 0a20 2020 2020 2020  t_layer).       
-00004030: 206e 625f 726f 7773 5f74 6f74 616c 203d   nb_rows_total =
-00004040: 2069 6e70 7574 5f6c 6179 6572 696e 666f   input_layerinfo
-00004050: 2e66 6561 7475 7265 636f 756e 740a 2020  .featurecount.  
-00004060: 2020 2020 2020 6966 2062 6174 6368 7369        if batchsi
-00004070: 7a65 203e 2030 3a0a 2020 2020 2020 2020  ze > 0:.        
-00004080: 2020 2020 7061 7261 6c6c 656c 6c69 7a61      parallelliza
-00004090: 7469 6f6e 5f63 6f6e 6669 6720 3d20 5061  tion_config = Pa
-000040a0: 7261 6c6c 656c 697a 6174 696f 6e43 6f6e  rallelizationCon
-000040b0: 6669 6728 0a20 2020 2020 2020 2020 2020  fig(.           
-000040c0: 2020 2020 206d 696e 5f61 7667 5f72 6f77       min_avg_row
-000040d0: 735f 7065 725f 6261 7463 683d 6d61 7468  s_per_batch=math
-000040e0: 2e63 6569 6c28 6261 7463 6873 697a 6520  .ceil(batchsize 
-000040f0: 2f20 3229 2c0a 2020 2020 2020 2020 2020  / 2),.          
-00004100: 2020 2020 2020 6d61 785f 6176 675f 726f        max_avg_ro
-00004110: 7773 5f70 6572 5f62 6174 6368 3d62 6174  ws_per_batch=bat
-00004120: 6368 7369 7a65 2c0a 2020 2020 2020 2020  chsize,.        
-00004130: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00004140: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00004150: 7061 7261 6c6c 656c 6c69 7a61 7469 6f6e  parallellization
-00004160: 5f63 6f6e 6669 6720 3d20 5061 7261 6c6c  _config = Parall
-00004170: 656c 697a 6174 696f 6e43 6f6e 6669 6728  elizationConfig(
-00004180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004190: 206d 6178 5f61 7667 5f72 6f77 735f 7065   max_avg_rows_pe
-000041a0: 725f 6261 7463 683d 3530 3030 300a 2020  r_batch=50000.  
-000041b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000041c0: 2020 2020 6e62 5f70 6172 616c 6c65 6c2c      nb_parallel,
-000041d0: 206e 625f 6261 7463 6865 732c 2072 6561   nb_batches, rea
-000041e0: 6c5f 6261 7463 6873 697a 6520 3d20 6765  l_batchsize = ge
-000041f0: 745f 7061 7261 6c6c 656c 697a 6174 696f  t_parallelizatio
-00004200: 6e5f 7061 7261 6d73 280a 2020 2020 2020  n_params(.      
-00004210: 2020 2020 2020 6e62 5f72 6f77 735f 746f        nb_rows_to
-00004220: 7461 6c3d 6e62 5f72 6f77 735f 746f 7461  tal=nb_rows_tota
-00004230: 6c2c 0a20 2020 2020 2020 2020 2020 206e  l,.            n
-00004240: 625f 7061 7261 6c6c 656c 3d6e 625f 7061  b_parallel=nb_pa
-00004250: 7261 6c6c 656c 2c0a 2020 2020 2020 2020  rallel,.        
-00004260: 2020 2020 7061 7261 6c6c 656c 697a 6174      parallelizat
-00004270: 696f 6e5f 636f 6e66 6967 3d70 6172 616c  ion_config=paral
-00004280: 6c65 6c6c 697a 6174 696f 6e5f 636f 6e66  lellization_conf
-00004290: 6967 2c0a 2020 2020 2020 2020 290a 0a20  ig,.        ).. 
-000042a0: 2020 2020 2020 2023 2054 4f44 4f3a 2064         # TODO: d
-000042b0: 6574 6572 6d69 6e65 2074 6865 206f 7074  etermine the opt
-000042c0: 696d 616c 2062 6174 6368 2073 697a 6573  imal batch sizes
-000042d0: 2077 6974 6820 6d69 6e20 616e 6420 6d61   with min and ma
-000042e0: 7820 6f66 2072 6f77 6964 2077 696c 6c0a  x of rowid will.
-000042f0: 2020 2020 2020 2020 2320 696e 2073 6f6d          # in som
-00004300: 6520 6361 7365 2069 6d70 726f 7665 2070  e case improve p
-00004310: 6572 666f 726d 616e 6365 0a20 2020 2020  erformance.     
-00004320: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00004330: 716c 5f73 746d 7420 3d20 6627 2727 5345  ql_stmt = f'''SE
-00004340: 4c45 4354 204d 494e 2872 6f77 6964 2920  LECT MIN(rowid) 
-00004350: 6173 206d 696e 5f72 6f77 6964 2c20 4d41  as min_rowid, MA
-00004360: 5828 726f 7769 6429 2061 7320 6d61 785f  X(rowid) as max_
-00004370: 726f 7769 640a 2020 2020 2020 2020 2020  rowid.          
-00004380: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-00004390: 524f 4d20 227b 696e 7075 745f 6c61 7965  ROM "{input_laye
-000043a0: 727d 2227 2727 0a20 2020 2020 2020 2072  r}"'''.        r
-000043b0: 6573 756c 7420 3d20 6766 6f2e 7265 6164  esult = gfo.read
-000043c0: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
-000043d0: 2020 2070 6174 683d 7465 6d70 5f70 6174     path=temp_pat
-000043e0: 682c 206c 6179 6572 3d69 6e70 7574 5f6c  h, layer=input_l
-000043f0: 6179 6572 2c20 7371 6c5f 7374 6d74 3d73  ayer, sql_stmt=s
-00004400: 716c 5f73 746d 742c 2073 716c 5f64 6961  ql_stmt, sql_dia
-00004410: 6c65 6374 3d22 5351 4c49 5445 220a 2020  lect="SQLITE".  
-00004420: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004430: 6966 206c 656e 2872 6573 756c 7429 203d  if len(result) =
-00004440: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00004450: 206d 696e 5f72 6f77 6964 203d 2072 6573   min_rowid = res
-00004460: 756c 745b 276d 696e 5f72 6f77 6964 275d  ult['min_rowid']
-00004470: 2e76 616c 7565 735b 305d 0a20 2020 2020  .values[0].     
-00004480: 2020 2020 2020 206d 6178 5f72 6f77 6964         max_rowid
-00004490: 203d 2072 6573 756c 745b 276d 6178 5f72   = result['max_r
-000044a0: 6f77 6964 275d 2e76 616c 7565 735b 305d  owid'].values[0]
-000044b0: 0a20 2020 2020 2020 2020 2020 206e 625f  .            nb_
-000044c0: 726f 7769 6473 5f70 6572 5f62 6174 6368  rowids_per_batch
-000044d0: 203d 2028 6d61 785f 726f 7769 6420 2d20   = (max_rowid - 
-000044e0: 6d69 6e5f 726f 7769 6429 2f6e 625f 6261  min_rowid)/nb_ba
-000044f0: 7463 6865 730a 2020 2020 2020 2020 656c  tches.        el
-00004500: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00004510: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-00004520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004530: 2066 2245 7272 6f72 2067 6574 7469 6e67   f"Error getting
-00004540: 206d 696e 2061 6e64 206d 6178 2072 6f77   min and max row
-00004550: 6964 2066 6f72 207b 7465 6d70 5f70 6174  id for {temp_pat
-00004560: 687d 2c20 6c61 7965 7220 7b69 6e70 7574  h}, layer {input
-00004570: 5f6c 6179 6572 7d22 0a20 2020 2020 2020  _layer}".       
-00004580: 2020 2020 2029 0a20 2020 2020 2020 2022       ).        "
-00004590: 2222 0a0a 2020 2020 2020 2020 2320 5072  ""..        # Pr
-000045a0: 6f63 6573 7369 6e67 2069 6e20 7468 7265  ocessing in thre
-000045b0: 6164 7320 6973 2032 7820 6661 7374 6572  ads is 2x faster
-000045c0: 2066 6f72 2073 6d61 6c6c 2064 6174 6173   for small datas
-000045d0: 6574 7320 286f 6e20 5769 6e64 6f77 7329  ets (on Windows)
-000045e0: 0a20 2020 2020 2020 2063 616c 6375 6c61  .        calcula
-000045f0: 7465 5f69 6e5f 7468 7265 6164 7320 3d20  te_in_threads = 
-00004600: 5472 7565 2069 6620 696e 7075 745f 6c61  True if input_la
-00004610: 7965 7269 6e66 6f2e 6665 6174 7572 6563  yerinfo.featurec
-00004620: 6f75 6e74 203c 3d20 3130 3020 656c 7365  ount <= 100 else
-00004630: 2046 616c 7365 0a20 2020 2020 2020 2077   False.        w
-00004640: 6974 6820 5f70 726f 6365 7373 696e 675f  ith _processing_
-00004650: 7574 696c 2e50 6f6f 6c65 6445 7865 6375  util.PooledExecu
-00004660: 746f 7246 6163 746f 7279 280a 2020 2020  torFactory(.    
-00004670: 2020 2020 2020 2020 7468 7265 6164 706f          threadpo
-00004680: 6f6c 3d63 616c 6375 6c61 7465 5f69 6e5f  ol=calculate_in_
-00004690: 7468 7265 6164 732c 0a20 2020 2020 2020  threads,.       
-000046a0: 2020 2020 206d 6178 5f77 6f72 6b65 7273       max_workers
-000046b0: 3d6e 625f 7061 7261 6c6c 656c 2c0a 2020  =nb_parallel,.  
-000046c0: 2020 2020 2020 2020 2020 696e 6974 6961            initia
-000046d0: 6c69 7a65 723d 5f70 726f 6365 7373 696e  lizer=_processin
-000046e0: 675f 7574 696c 2e69 6e69 7469 616c 697a  g_util.initializ
-000046f0: 655f 776f 726b 6572 2829 2c0a 2020 2020  e_worker(),.    
-00004700: 2020 2020 2920 6173 2063 616c 6375 6c61      ) as calcula
-00004710: 7465 5f70 6f6f 6c3a 0a20 2020 2020 2020  te_pool:.       
-00004720: 2020 2020 2023 2050 7265 7061 7265 206f       # Prepare o
-00004730: 7574 7075 7420 6669 6c65 6e61 6d65 0a20  utput filename. 
-00004740: 2020 2020 2020 2020 2020 2074 6d70 5f6f             tmp_o
-00004750: 7574 7075 745f 7061 7468 203d 2074 656d  utput_path = tem
-00004760: 7064 6972 202f 206f 7574 7075 745f 7061  pdir / output_pa
-00004770: 7468 2e6e 616d 650a 0a20 2020 2020 2020  th.name..       
-00004780: 2020 2020 2072 6f77 5f6f 6666 7365 7420       row_offset 
-00004790: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-000047a0: 6261 7463 6865 7320 3d20 7b7d 0a20 2020  batches = {}.   
-000047b0: 2020 2020 2020 2020 2066 7574 7572 655f           future_
-000047c0: 746f 5f62 6174 6368 5f69 6420 3d20 7b7d  to_batch_id = {}
-000047d0: 0a20 2020 2020 2020 2020 2020 206e 625f  .            nb_
-000047e0: 646f 6e65 203d 2030 0a0a 2020 2020 2020  done = 0..      
-000047f0: 2020 2020 2020 666f 7220 6261 7463 685f        for batch_
-00004800: 6964 2069 6e20 7261 6e67 6528 6e62 5f62  id in range(nb_b
-00004810: 6174 6368 6573 293a 0a20 2020 2020 2020  atches):.       
-00004820: 2020 2020 2020 2020 2062 6174 6368 6573           batches
-00004830: 5b62 6174 6368 5f69 645d 203d 207b 7d0a  [batch_id] = {}.
-00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 6261 7463 6865 735b 6261 7463 685f 6964  batches[batch_id
-00004860: 5d5b 226c 6179 6572 225d 203d 206f 7574  ]["layer"] = out
-00004870: 7075 745f 6c61 7965 720a 0a20 2020 2020  put_layer..     
-00004880: 2020 2020 2020 2020 2020 2023 204f 7574             # Out
-00004890: 7075 7420 6561 6368 2062 6174 6368 2074  put each batch t
-000048a0: 6f20 6120 7365 7065 7261 7465 2074 656d  o a seperate tem
-000048b0: 706f 7261 7279 2066 696c 652c 206f 7468  porary file, oth
-000048c0: 6572 7769 7365 2074 6865 7265 0a20 2020  erwise there.   
-000048d0: 2020 2020 2020 2020 2020 2020 2023 2061               # a
-000048e0: 7265 2074 696d 656f 7574 2069 7373 7565  re timeout issue
-000048f0: 7320 7768 656e 2070 726f 6365 7373 696e  s when processin
-00004900: 6720 6c61 7267 6520 6669 6c65 730a 2020  g large files.  
-00004910: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00004920: 7470 7574 5f74 6d70 5f70 6172 7469 616c  tput_tmp_partial
-00004930: 5f70 6174 6820 3d20 280a 2020 2020 2020  _path = (.      
-00004940: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00004950: 6d70 6469 7220 2f20 6622 7b6f 7574 7075  mpdir / f"{outpu
-00004960: 745f 7061 7468 2e73 7465 6d7d 5f7b 6261  t_path.stem}_{ba
-00004970: 7463 685f 6964 7d7b 6f75 7470 7574 5f70  tch_id}{output_p
-00004980: 6174 682e 7375 6666 6978 7d22 0a20 2020  ath.suffix}".   
-00004990: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000049b0: 6174 6368 6573 5b62 6174 6368 5f69 645d  atches[batch_id]
-000049c0: 5b22 746d 705f 7061 7274 6961 6c5f 6f75  ["tmp_partial_ou
-000049d0: 7470 7574 5f70 6174 6822 5d20 3d20 6f75  tput_path"] = ou
-000049e0: 7470 7574 5f74 6d70 5f70 6172 7469 616c  tput_tmp_partial
-000049f0: 5f70 6174 680a 0a20 2020 2020 2020 2020  _path..         
-00004a00: 2020 2020 2020 2023 2046 6f72 2074 6865         # For the
-00004a10: 206c 6173 7420 7472 616e 736c 6174 655f   last translate_
-00004a20: 6964 2c20 7461 6b65 2061 6c6c 2072 6f77  id, take all row
-00004a30: 6964 2773 206c 6566 742e 2e2e 0a20 2020  id's left....   
-00004a40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004a50: 6261 7463 685f 6964 203c 206e 625f 6261  batch_id < nb_ba
-00004a60: 7463 6865 7320 2d20 313a 0a20 2020 2020  tches - 1:.     
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004a80: 6f77 7320 3d20 736c 6963 6528 726f 775f  ows = slice(row_
-00004a90: 6f66 6673 6574 2c20 726f 775f 6f66 6673  offset, row_offs
-00004aa0: 6574 202b 2072 6561 6c5f 6261 7463 6873  et + real_batchs
-00004ab0: 697a 6529 0a20 2020 2020 2020 2020 2020  ize).           
-00004ac0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004ae0: 6f77 7320 3d20 736c 6963 6528 726f 775f  ows = slice(row_
-00004af0: 6f66 6673 6574 2c20 6e62 5f72 6f77 735f  offset, nb_rows_
-00004b00: 746f 7461 6c29 0a0a 2020 2020 2020 2020  total)..        
-00004b10: 2020 2020 2020 2020 2320 5265 6d61 726b          # Remark
-00004b20: 3a20 7468 6973 2074 656d 7020 6669 6c65  : this temp file
-00004b30: 2064 6f65 736e 2774 206e 6565 6420 7370   doesn't need sp
-00004b40: 6174 6961 6c20 696e 6465 780a 2020 2020  atial index.    
-00004b50: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00004b60: 6d61 726b 3a20 6265 6361 7573 6520 666f  mark: because fo
-00004b70: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
-00004b80: 7472 7974 7970 6520 666f 7220 4765 6f44  trytype for GeoD
-00004b90: 6174 6146 7261 6d65 0a20 2020 2020 2020  ataFrame.       
-00004ba0: 2020 2020 2020 2020 2023 206f 7065 7261           # opera
-00004bb0: 7469 6f6e 7320 6973 2028 6120 6c6f 7429  tions is (a lot)
-00004bc0: 206d 6f72 6520 6c69 6d69 7465 6420 7468   more limited th
-00004bd0: 616e 2067 6461 6c2d 6261 7365 642c 2074  an gdal-based, t
-00004be0: 6865 2067 6461 6c20 7665 7273 696f 6e0a  he gdal version.
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2320 6973 2075 7365 6420 6c61 7465 7220  # is used later 
-00004c10: 6f6e 2077 6865 6e20 7468 6520 7265 7375  on when the resu
-00004c20: 6c74 7320 6172 6520 6d65 7267 6564 2074  lts are merged t
-00004c30: 6f20 7468 6520 7265 7375 6c74 2066 696c  o the result fil
-00004c40: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-00004c50: 2020 2066 7574 7572 6520 3d20 6361 6c63     future = calc
-00004c60: 756c 6174 655f 706f 6f6c 2e73 7562 6d69  ulate_pool.submi
-00004c70: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00004c80: 2020 2020 2020 205f 6170 706c 795f 6765         _apply_ge
-00004c90: 6f6f 7065 7261 7469 6f6e 2c0a 2020 2020  ooperation,.    
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 696e 7075 745f 7061 7468 3d69 6e70 7574  input_path=input
-00004cc0: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-00004cd0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00004ce0: 745f 7061 7468 3d6f 7574 7075 745f 746d  t_path=output_tm
-00004cf0: 705f 7061 7274 6961 6c5f 7061 7468 2c0a  p_partial_path,.
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d10: 2020 2020 6f70 6572 6174 696f 6e3d 6f70      operation=op
-00004d20: 6572 6174 696f 6e2c 0a20 2020 2020 2020  eration,.       
-00004d30: 2020 2020 2020 2020 2020 2020 206f 7065               ope
-00004d40: 7261 7469 6f6e 5f70 6172 616d 733d 6f70  ration_params=op
-00004d50: 6572 6174 696f 6e5f 7061 7261 6d73 2c0a  eration_params,.
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d70: 2020 2020 696e 7075 745f 6c61 7965 723d      input_layer=
-00004d80: 696e 7075 745f 6c61 7965 722c 0a20 2020  input_layer,.   
-00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004da0: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
-00004db0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004dc0: 2020 2020 2020 6f75 7470 7574 5f6c 6179        output_lay
-00004dd0: 6572 3d6f 7574 7075 745f 6c61 7965 722c  er=output_layer,
-00004de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004df0: 2020 2020 2072 6f77 733d 726f 7773 2c0a       rows=rows,.
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 6578 706c 6f64 6563 6f6c 6c65      explodecolle
-00004e20: 6374 696f 6e73 3d65 7870 6c6f 6465 636f  ctions=explodeco
-00004e30: 6c6c 6563 7469 6f6e 732c 0a20 2020 2020  llections,.     
-00004e40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004e50: 6f72 6365 3d66 6f72 6365 2c0a 2020 2020  orce=force,.    
-00004e60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00004e70: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-00004e80: 7475 7265 5f74 6f5f 6261 7463 685f 6964  ture_to_batch_id
-00004e90: 5b66 7574 7572 655d 203d 2062 6174 6368  [future] = batch
-00004ea0: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
-00004eb0: 2020 2020 726f 775f 6f66 6673 6574 202b      row_offset +
-00004ec0: 3d20 7265 616c 5f62 6174 6368 7369 7a65  = real_batchsize
-00004ed0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00004ee0: 4c6f 6f70 2074 696c 6c20 616c 6c20 7061  Loop till all pa
-00004ef0: 7261 6c6c 656c 2070 726f 6365 7373 6573  rallel processes
-00004f00: 2061 7265 2072 6561 6479 2c20 6275 7420   are ready, but 
-00004f10: 7072 6f63 6573 7320 6561 6368 206f 6e65  process each one
-00004f20: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
-00004f30: 6861 7420 6973 2072 6561 6479 2061 6c72  hat is ready alr
-00004f40: 6561 6479 0a20 2020 2020 2020 2020 2020  eady.           
-00004f50: 2073 7461 7274 5f74 696d 6520 3d20 6461   start_time = da
-00004f60: 7465 7469 6d65 2e6e 6f77 2829 0a20 2020  tetime.now().   
-00004f70: 2020 2020 2020 2020 205f 6765 6e65 7261           _genera
-00004f80: 6c5f 7574 696c 2e72 6570 6f72 745f 7072  l_util.report_pr
-00004f90: 6f67 7265 7373 280a 2020 2020 2020 2020  ogress(.        
-00004fa0: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
-00004fb0: 6d65 2c20 6e62 5f64 6f6e 652c 206e 625f  me, nb_done, nb_
-00004fc0: 6261 7463 6865 732c 206f 7065 7261 7469  batches, operati
-00004fd0: 6f6e 2e76 616c 7565 2c20 6e62 5f70 6172  on.value, nb_par
-00004fe0: 616c 6c65 6c0a 2020 2020 2020 2020 2020  allel.          
-00004ff0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00005000: 666f 7220 6675 7475 7265 2069 6e20 6675  for future in fu
-00005010: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
-00005020: 6564 2866 7574 7572 655f 746f 5f62 6174  ed(future_to_bat
-00005030: 6368 5f69 6429 3a0a 2020 2020 2020 2020  ch_id):.        
-00005040: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 206d 6573 7361 6765 203d 2066 7574 7572   message = futur
-00005070: 652e 7265 7375 6c74 2829 0a20 2020 2020  e.result().     
-00005080: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00005090: 6f67 6765 722e 6465 6275 6728 6d65 7373  ogger.debug(mess
-000050a0: 6167 6529 0a0a 2020 2020 2020 2020 2020  age)..          
-000050b0: 2020 2020 2020 2020 2020 2320 4966 2074            # If t
-000050c0: 6865 2063 616c 6375 6c61 7465 2067 6176  he calculate gav
-000050d0: 6520 7265 7375 6c74 732c 2063 6f70 7920  e results, copy 
-000050e0: 746f 206f 7574 7075 740a 2020 2020 2020  to output.      
-000050f0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00005100: 7463 685f 6964 203d 2066 7574 7572 655f  tch_id = future_
-00005110: 746f 5f62 6174 6368 5f69 645b 6675 7475  to_batch_id[futu
-00005120: 7265 5d0a 2020 2020 2020 2020 2020 2020  re].            
-00005130: 2020 2020 2020 2020 746d 705f 7061 7274          tmp_part
-00005140: 6961 6c5f 6f75 7470 7574 5f70 6174 6820  ial_output_path 
-00005150: 3d20 6261 7463 6865 735b 6261 7463 685f  = batches[batch_
-00005160: 6964 5d5b 0a20 2020 2020 2020 2020 2020  id][.           
-00005170: 2020 2020 2020 2020 2020 2020 2022 746d               "tm
-00005180: 705f 7061 7274 6961 6c5f 6f75 7470 7574  p_partial_output
-00005190: 5f70 6174 6822 0a20 2020 2020 2020 2020  _path".         
-000051a0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051c0: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-000051d0: 2020 2020 2020 2020 2020 2020 2020 746d                tm
-000051e0: 705f 7061 7274 6961 6c5f 6f75 7470 7574  p_partial_output
-000051f0: 5f70 6174 682e 6578 6973 7473 2829 0a20  _path.exists(). 
-00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005210: 2020 2020 2020 2061 6e64 2074 6d70 5f70         and tmp_p
-00005220: 6172 7469 616c 5f6f 7574 7075 745f 7061  artial_output_pa
-00005230: 7468 2e73 7461 7428 292e 7374 5f73 697a  th.stat().st_siz
-00005240: 6520 3e20 300a 2020 2020 2020 2020 2020  e > 0.          
-00005250: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005270: 2020 2020 2023 2052 656d 6172 6b3a 2062       # Remark: b
-00005280: 6563 6175 7365 2066 6f72 6365 5f6f 7574  ecause force_out
-00005290: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
-000052a0: 2066 6f72 2047 656f 4461 7461 4672 616d   for GeoDataFram
-000052b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000052c0: 2020 2020 2020 2020 2020 2320 6f70 6572            # oper
-000052d0: 6174 696f 6e73 2069 7320 2861 206c 6f74  ations is (a lot
-000052e0: 2920 6d6f 7265 206c 696d 6974 6564 2074  ) more limited t
-000052f0: 6861 6e20 6764 616c 2d62 6173 6564 2c20  han gdal-based, 
-00005300: 7573 6520 7468 650a 2020 2020 2020 2020  use the.        
-00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005320: 2320 6764 616c 2076 6572 7369 6f6e 2076  # gdal version v
-00005330: 6961 205f 6170 7065 6e64 5f74 6f5f 6e6f  ia _append_to_no
-00005340: 6c6f 636b 2e0a 2020 2020 2020 2020 2020  lock..          
-00005350: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005360: 206e 625f 6261 7463 6865 7320 3d3d 2031   nb_batches == 1
-00005370: 2061 6e64 2066 6f72 6365 5f6f 7574 7075   and force_outpu
-00005380: 745f 6765 6f6d 6574 7279 7479 7065 2069  t_geometrytype i
-00005390: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000053a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053b0: 2020 2020 6766 6f2e 6d6f 7665 2874 6d70      gfo.move(tmp
-000053c0: 5f70 6172 7469 616c 5f6f 7574 7075 745f  _partial_output_
-000053d0: 7061 7468 2c20 746d 705f 6f75 7470 7574  path, tmp_output
-000053e0: 5f70 6174 6829 0a20 2020 2020 2020 2020  _path).         
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005400: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005420: 2066 696c 656f 7073 2e5f 6170 7065 6e64   fileops._append
-00005430: 5f74 6f5f 6e6f 6c6f 636b 280a 2020 2020  _to_nolock(.    
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 2020 2020 2020 2020 7372 633d              src=
-00005460: 746d 705f 7061 7274 6961 6c5f 6f75 7470  tmp_partial_outp
-00005470: 7574 5f70 6174 682c 0a20 2020 2020 2020  ut_path,.       
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2020 2020 2020 2020 2064 7374 3d74 6d70           dst=tmp
-000054a0: 5f6f 7574 7075 745f 7061 7468 2c0a 2020  _output_path,.  
-000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054c0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000054d0: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
-000054e0: 3d65 7870 6c6f 6465 636f 6c6c 6563 7469  =explodecollecti
-000054f0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005510: 2020 2020 2063 7265 6174 655f 7370 6174       create_spat
-00005520: 6961 6c5f 696e 6465 783d 4661 6c73 652c  ial_index=False,
-00005530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001bb0: 2323 2323 2323 2323 2323 0a23 2054 6865  ##########.# The
+00001bc0: 2072 6561 6c20 7374 7566 660a 2323 2323   real stuff.####
+00001bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001c00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001c10: 2323 2323 2323 2323 2323 2323 0a0a 0a64  ############...d
+00001c20: 6566 2061 7070 6c79 280a 2020 2020 696e  ef apply(.    in
+00001c30: 7075 745f 7061 7468 3a20 5061 7468 2c0a  put_path: Path,.
+00001c40: 2020 2020 6f75 7470 7574 5f70 6174 683a      output_path:
+00001c50: 2050 6174 682c 0a20 2020 2066 756e 633a   Path,.    func:
+00001c60: 2043 616c 6c61 626c 655b 5b41 6e79 5d2c   Callable[[Any],
+00001c70: 2041 6e79 5d2c 0a20 2020 206f 6e6c 795f   Any],.    only_
+00001c80: 6765 6f6d 5f69 6e70 7574 3a20 626f 6f6c  geom_input: bool
+00001c90: 203d 2054 7275 652c 0a20 2020 2069 6e70   = True,.    inp
+00001ca0: 7574 5f6c 6179 6572 3a20 4f70 7469 6f6e  ut_layer: Option
+00001cb0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00001cc0: 2020 2020 6f75 7470 7574 5f6c 6179 6572      output_layer
+00001cd0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00001ce0: 3d20 4e6f 6e65 2c0a 2020 2020 636f 6c75  = None,.    colu
+00001cf0: 6d6e 733a 204f 7074 696f 6e61 6c5b 4c69  mns: Optional[Li
+00001d00: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
+00001d10: 0a20 2020 2065 7870 6c6f 6465 636f 6c6c  .    explodecoll
+00001d20: 6563 7469 6f6e 733a 2062 6f6f 6c20 3d20  ections: bool = 
+00001d30: 4661 6c73 652c 0a20 2020 2066 6f72 6365  False,.    force
+00001d40: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+00001d50: 7479 7065 3a20 556e 696f 6e5b 4765 6f6d  type: Union[Geom
+00001d60: 6574 7279 5479 7065 2c20 7374 722c 204e  etryType, str, N
+00001d70: 6f6e 655d 203d 204e 6f6e 652c 0a20 2020  one] = None,.   
+00001d80: 2067 7269 6473 697a 653a 2066 6c6f 6174   gridsize: float
+00001d90: 203d 2030 2e30 2c0a 2020 2020 6e62 5f70   = 0.0,.    nb_p
+00001da0: 6172 616c 6c65 6c3a 2069 6e74 203d 202d  arallel: int = -
+00001db0: 312c 0a20 2020 2062 6174 6368 7369 7a65  1,.    batchsize
+00001dc0: 3a20 696e 7420 3d20 2d31 2c0a 2020 2020  : int = -1,.    
+00001dd0: 666f 7263 653a 2062 6f6f 6c20 3d20 4661  force: bool = Fa
+00001de0: 6c73 652c 0a29 3a0a 2020 2020 2320 496e  lse,.):.    # In
+00001df0: 6974 0a20 2020 206f 7065 7261 7469 6f6e  it.    operation
+00001e00: 5f70 6172 616d 7320 3d20 7b0a 2020 2020  _params = {.    
+00001e10: 2020 2020 226f 6e6c 795f 6765 6f6d 5f69      "only_geom_i
+00001e20: 6e70 7574 223a 206f 6e6c 795f 6765 6f6d  nput": only_geom
+00001e30: 5f69 6e70 7574 2c0a 2020 2020 2020 2020  _input,.        
+00001e40: 2270 6963 6b6c 6564 5f66 756e 6322 3a20  "pickled_func": 
+00001e50: 636c 6f75 6470 6963 6b6c 652e 6475 6d70  cloudpickle.dump
+00001e60: 7328 6675 6e63 292c 0a20 2020 207d 0a0a  s(func),.    }..
+00001e70: 2020 2020 2320 476f 210a 2020 2020 7265      # Go!.    re
+00001e80: 7475 726e 205f 6170 706c 795f 6765 6f6f  turn _apply_geoo
+00001e90: 7065 7261 7469 6f6e 5f74 6f5f 6c61 7965  peration_to_laye
+00001ea0: 7228 0a20 2020 2020 2020 2069 6e70 7574  r(.        input
+00001eb0: 5f70 6174 683d 696e 7075 745f 7061 7468  _path=input_path
+00001ec0: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
+00001ed0: 5f70 6174 683d 6f75 7470 7574 5f70 6174  _path=output_pat
+00001ee0: 682c 0a20 2020 2020 2020 206f 7065 7261  h,.        opera
+00001ef0: 7469 6f6e 3d47 656f 4f70 6572 6174 696f  tion=GeoOperatio
+00001f00: 6e2e 4150 504c 592c 0a20 2020 2020 2020  n.APPLY,.       
+00001f10: 206f 7065 7261 7469 6f6e 5f70 6172 616d   operation_param
+00001f20: 733d 6f70 6572 6174 696f 6e5f 7061 7261  s=operation_para
+00001f30: 6d73 2c0a 2020 2020 2020 2020 696e 7075  ms,.        inpu
+00001f40: 745f 6c61 7965 723d 696e 7075 745f 6c61  t_layer=input_la
+00001f50: 7965 722c 0a20 2020 2020 2020 206f 7574  yer,.        out
+00001f60: 7075 745f 6c61 7965 723d 6f75 7470 7574  put_layer=output
+00001f70: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+00001f80: 636f 6c75 6d6e 733d 636f 6c75 6d6e 732c  columns=columns,
+00001f90: 0a20 2020 2020 2020 2065 7870 6c6f 6465  .        explode
+00001fa0: 636f 6c6c 6563 7469 6f6e 733d 6578 706c  collections=expl
+00001fb0: 6f64 6563 6f6c 6c65 6374 696f 6e73 2c0a  odecollections,.
+00001fc0: 2020 2020 2020 2020 666f 7263 655f 6f75          force_ou
+00001fd0: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
+00001fe0: 653d 666f 7263 655f 6f75 7470 7574 5f67  e=force_output_g
+00001ff0: 656f 6d65 7472 7974 7970 652c 0a20 2020  eometrytype,.   
+00002000: 2020 2020 2067 7269 6473 697a 653d 6772       gridsize=gr
+00002010: 6964 7369 7a65 2c0a 2020 2020 2020 2020  idsize,.        
+00002020: 6e62 5f70 6172 616c 6c65 6c3d 6e62 5f70  nb_parallel=nb_p
+00002030: 6172 616c 6c65 6c2c 0a20 2020 2020 2020  arallel,.       
+00002040: 2062 6174 6368 7369 7a65 3d62 6174 6368   batchsize=batch
+00002050: 7369 7a65 2c0a 2020 2020 2020 2020 666f  size,.        fo
+00002060: 7263 653d 666f 7263 652c 0a20 2020 2029  rce=force,.    )
+00002070: 0a0a 0a64 6566 2062 7566 6665 7228 0a20  ...def buffer(. 
+00002080: 2020 2069 6e70 7574 5f70 6174 683a 2050     input_path: P
+00002090: 6174 682c 0a20 2020 206f 7574 7075 745f  ath,.    output_
+000020a0: 7061 7468 3a20 5061 7468 2c0a 2020 2020  path: Path,.    
+000020b0: 6469 7374 616e 6365 3a20 666c 6f61 742c  distance: float,
+000020c0: 0a20 2020 2071 7561 6472 616e 7473 6567  .    quadrantseg
+000020d0: 6d65 6e74 733a 2069 6e74 203d 2035 2c0a  ments: int = 5,.
+000020e0: 2020 2020 656e 6463 6170 5f73 7479 6c65      endcap_style
+000020f0: 3a20 4275 6666 6572 456e 6443 6170 5374  : BufferEndCapSt
+00002100: 796c 6520 3d20 4275 6666 6572 456e 6443  yle = BufferEndC
+00002110: 6170 5374 796c 652e 524f 554e 442c 0a20  apStyle.ROUND,. 
+00002120: 2020 206a 6f69 6e5f 7374 796c 653a 2042     join_style: B
+00002130: 7566 6665 724a 6f69 6e53 7479 6c65 203d  ufferJoinStyle =
+00002140: 2042 7566 6665 724a 6f69 6e53 7479 6c65   BufferJoinStyle
+00002150: 2e52 4f55 4e44 2c0a 2020 2020 6d69 7472  .ROUND,.    mitr
+00002160: 655f 6c69 6d69 743a 2066 6c6f 6174 203d  e_limit: float =
+00002170: 2035 2e30 2c0a 2020 2020 7369 6e67 6c65   5.0,.    single
+00002180: 5f73 6964 6564 3a20 626f 6f6c 203d 2046  _sided: bool = F
+00002190: 616c 7365 2c0a 2020 2020 696e 7075 745f  alse,.    input_
+000021a0: 6c61 7965 723a 204f 7074 696f 6e61 6c5b  layer: Optional[
+000021b0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000021c0: 206f 7574 7075 745f 6c61 7965 723a 204f   output_layer: O
+000021d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000021e0: 6f6e 652c 0a20 2020 2063 6f6c 756d 6e73  one,.    columns
+000021f0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+00002200: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+00002210: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
+00002220: 696f 6e73 3a20 626f 6f6c 203d 2046 616c  ions: bool = Fal
+00002230: 7365 2c0a 2020 2020 6772 6964 7369 7a65  se,.    gridsize
+00002240: 3a20 666c 6f61 7420 3d20 302e 302c 0a20  : float = 0.0,. 
+00002250: 2020 206e 625f 7061 7261 6c6c 656c 3a20     nb_parallel: 
+00002260: 696e 7420 3d20 2d31 2c0a 2020 2020 6261  int = -1,.    ba
+00002270: 7463 6873 697a 653a 2069 6e74 203d 202d  tchsize: int = -
+00002280: 312c 0a20 2020 2066 6f72 6365 3a20 626f  1,.    force: bo
+00002290: 6f6c 203d 2046 616c 7365 2c0a 293a 0a20  ol = False,.):. 
+000022a0: 2020 2023 2049 6e69 740a 2020 2020 6f70     # Init.    op
+000022b0: 6572 6174 696f 6e5f 7061 7261 6d73 203d  eration_params =
+000022c0: 207b 0a20 2020 2020 2020 2022 6469 7374   {.        "dist
+000022d0: 616e 6365 223a 2064 6973 7461 6e63 652c  ance": distance,
+000022e0: 0a20 2020 2020 2020 2022 7175 6164 7261  .        "quadra
+000022f0: 6e74 7365 676d 656e 7473 223a 2071 7561  ntsegments": qua
+00002300: 6472 616e 7473 6567 6d65 6e74 732c 0a20  drantsegments,. 
+00002310: 2020 2020 2020 2022 656e 6463 6170 5f73         "endcap_s
+00002320: 7479 6c65 223a 2065 6e64 6361 705f 7374  tyle": endcap_st
+00002330: 796c 652c 0a20 2020 2020 2020 2022 6a6f  yle,.        "jo
+00002340: 696e 5f73 7479 6c65 223a 206a 6f69 6e5f  in_style": join_
+00002350: 7374 796c 652c 0a20 2020 2020 2020 2022  style,.        "
+00002360: 6d69 7472 655f 6c69 6d69 7422 3a20 6d69  mitre_limit": mi
+00002370: 7472 655f 6c69 6d69 742c 0a20 2020 2020  tre_limit,.     
+00002380: 2020 2022 7369 6e67 6c65 5f73 6964 6564     "single_sided
+00002390: 223a 2073 696e 676c 655f 7369 6465 642c  ": single_sided,
+000023a0: 0a20 2020 207d 0a0a 2020 2020 2320 4275  .    }..    # Bu
+000023b0: 6666 6572 206f 7065 7261 7469 6f6e 2061  ffer operation a
+000023c0: 6c77 6179 7320 7265 7375 6c74 7320 696e  lways results in
+000023d0: 2070 6f6c 7967 6f6e 732e 2e2e 0a20 2020   polygons....   
+000023e0: 2069 6620 6578 706c 6f64 6563 6f6c 6c65   if explodecolle
+000023f0: 6374 696f 6e73 3a0a 2020 2020 2020 2020  ctions:.        
+00002400: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
+00002410: 6d65 7472 7974 7970 6520 3d20 4765 6f6d  metrytype = Geom
+00002420: 6574 7279 5479 7065 2e50 4f4c 5947 4f4e  etryType.POLYGON
+00002430: 2e6e 616d 650a 2020 2020 656c 7365 3a0a  .name.    else:.
+00002440: 2020 2020 2020 2020 666f 7263 655f 6f75          force_ou
+00002450: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
+00002460: 6520 3d20 4765 6f6d 6574 7279 5479 7065  e = GeometryType
+00002470: 2e4d 554c 5449 504f 4c59 474f 4e2e 6e61  .MULTIPOLYGON.na
+00002480: 6d65 0a0a 2020 2020 2320 476f 210a 2020  me..    # Go!.  
+00002490: 2020 7265 7475 726e 205f 6170 706c 795f    return _apply_
+000024a0: 6765 6f6f 7065 7261 7469 6f6e 5f74 6f5f  geooperation_to_
+000024b0: 6c61 7965 7228 0a20 2020 2020 2020 2069  layer(.        i
+000024c0: 6e70 7574 5f70 6174 683d 696e 7075 745f  nput_path=input_
+000024d0: 7061 7468 2c0a 2020 2020 2020 2020 6f75  path,.        ou
+000024e0: 7470 7574 5f70 6174 683d 6f75 7470 7574  tput_path=output
+000024f0: 5f70 6174 682c 0a20 2020 2020 2020 206f  _path,.        o
+00002500: 7065 7261 7469 6f6e 3d47 656f 4f70 6572  peration=GeoOper
+00002510: 6174 696f 6e2e 4255 4646 4552 2c0a 2020  ation.BUFFER,.  
+00002520: 2020 2020 2020 6f70 6572 6174 696f 6e5f        operation_
+00002530: 7061 7261 6d73 3d6f 7065 7261 7469 6f6e  params=operation
+00002540: 5f70 6172 616d 732c 0a20 2020 2020 2020  _params,.       
+00002550: 2069 6e70 7574 5f6c 6179 6572 3d69 6e70   input_layer=inp
+00002560: 7574 5f6c 6179 6572 2c0a 2020 2020 2020  ut_layer,.      
+00002570: 2020 6f75 7470 7574 5f6c 6179 6572 3d6f    output_layer=o
+00002580: 7574 7075 745f 6c61 7965 722c 0a20 2020  utput_layer,.   
+00002590: 2020 2020 2063 6f6c 756d 6e73 3d63 6f6c       columns=col
+000025a0: 756d 6e73 2c0a 2020 2020 2020 2020 6578  umns,.        ex
+000025b0: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
+000025c0: 3d65 7870 6c6f 6465 636f 6c6c 6563 7469  =explodecollecti
+000025d0: 6f6e 732c 0a20 2020 2020 2020 2066 6f72  ons,.        for
+000025e0: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
+000025f0: 7279 7479 7065 3d66 6f72 6365 5f6f 7574  rytype=force_out
+00002600: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
+00002610: 2c0a 2020 2020 2020 2020 6772 6964 7369  ,.        gridsi
+00002620: 7a65 3d67 7269 6473 697a 652c 0a20 2020  ze=gridsize,.   
+00002630: 2020 2020 206e 625f 7061 7261 6c6c 656c       nb_parallel
+00002640: 3d6e 625f 7061 7261 6c6c 656c 2c0a 2020  =nb_parallel,.  
+00002650: 2020 2020 2020 6261 7463 6873 697a 653d        batchsize=
+00002660: 6261 7463 6873 697a 652c 0a20 2020 2020  batchsize,.     
+00002670: 2020 2066 6f72 6365 3d66 6f72 6365 2c0a     force=force,.
+00002680: 2020 2020 290a 0a0a 6465 6620 636f 6e76      )...def conv
+00002690: 6578 6875 6c6c 280a 2020 2020 696e 7075  exhull(.    inpu
+000026a0: 745f 7061 7468 3a20 5061 7468 2c0a 2020  t_path: Path,.  
+000026b0: 2020 6f75 7470 7574 5f70 6174 683a 2050    output_path: P
+000026c0: 6174 682c 0a20 2020 2069 6e70 7574 5f6c  ath,.    input_l
+000026d0: 6179 6572 3a20 4f70 7469 6f6e 616c 5b73  ayer: Optional[s
+000026e0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+000026f0: 6f75 7470 7574 5f6c 6179 6572 3a20 4f70  output_layer: Op
+00002700: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00002710: 6e65 2c0a 2020 2020 636f 6c75 6d6e 733a  ne,.    columns:
+00002720: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00002730: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+00002740: 2065 7870 6c6f 6465 636f 6c6c 6563 7469   explodecollecti
+00002750: 6f6e 733a 2062 6f6f 6c20 3d20 4661 6c73  ons: bool = Fals
+00002760: 652c 0a20 2020 2067 7269 6473 697a 653a  e,.    gridsize:
+00002770: 2066 6c6f 6174 203d 2030 2e30 2c0a 2020   float = 0.0,.  
+00002780: 2020 6e62 5f70 6172 616c 6c65 6c3a 2069    nb_parallel: i
+00002790: 6e74 203d 202d 312c 0a20 2020 2062 6174  nt = -1,.    bat
+000027a0: 6368 7369 7a65 3a20 696e 7420 3d20 2d31  chsize: int = -1
+000027b0: 2c0a 2020 2020 666f 7263 653a 2062 6f6f  ,.    force: boo
+000027c0: 6c20 3d20 4661 6c73 652c 0a29 3a0a 2020  l = False,.):.  
+000027d0: 2020 2320 496e 6974 0a20 2020 206f 7065    # Init.    ope
+000027e0: 7261 7469 6f6e 5f70 6172 616d 7320 3d20  ration_params = 
+000027f0: 7b7d 0a0a 2020 2020 2320 476f 210a 2020  {}..    # Go!.  
+00002800: 2020 7265 7475 726e 205f 6170 706c 795f    return _apply_
+00002810: 6765 6f6f 7065 7261 7469 6f6e 5f74 6f5f  geooperation_to_
+00002820: 6c61 7965 7228 0a20 2020 2020 2020 2069  layer(.        i
+00002830: 6e70 7574 5f70 6174 683d 696e 7075 745f  nput_path=input_
+00002840: 7061 7468 2c0a 2020 2020 2020 2020 6f75  path,.        ou
+00002850: 7470 7574 5f70 6174 683d 6f75 7470 7574  tput_path=output
+00002860: 5f70 6174 682c 0a20 2020 2020 2020 206f  _path,.        o
+00002870: 7065 7261 7469 6f6e 3d47 656f 4f70 6572  peration=GeoOper
+00002880: 6174 696f 6e2e 434f 4e56 4558 4855 4c4c  ation.CONVEXHULL
+00002890: 2c0a 2020 2020 2020 2020 6f70 6572 6174  ,.        operat
+000028a0: 696f 6e5f 7061 7261 6d73 3d6f 7065 7261  ion_params=opera
+000028b0: 7469 6f6e 5f70 6172 616d 732c 0a20 2020  tion_params,.   
+000028c0: 2020 2020 2069 6e70 7574 5f6c 6179 6572       input_layer
+000028d0: 3d69 6e70 7574 5f6c 6179 6572 2c0a 2020  =input_layer,.  
+000028e0: 2020 2020 2020 6f75 7470 7574 5f6c 6179        output_lay
+000028f0: 6572 3d6f 7574 7075 745f 6c61 7965 722c  er=output_layer,
+00002900: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
+00002910: 3d63 6f6c 756d 6e73 2c0a 2020 2020 2020  =columns,.      
+00002920: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
+00002930: 696f 6e73 3d65 7870 6c6f 6465 636f 6c6c  ions=explodecoll
+00002940: 6563 7469 6f6e 732c 0a20 2020 2020 2020  ections,.       
+00002950: 2067 7269 6473 697a 653d 6772 6964 7369   gridsize=gridsi
+00002960: 7a65 2c0a 2020 2020 2020 2020 6e62 5f70  ze,.        nb_p
+00002970: 6172 616c 6c65 6c3d 6e62 5f70 6172 616c  arallel=nb_paral
+00002980: 6c65 6c2c 0a20 2020 2020 2020 2062 6174  lel,.        bat
+00002990: 6368 7369 7a65 3d62 6174 6368 7369 7a65  chsize=batchsize
+000029a0: 2c0a 2020 2020 2020 2020 666f 7263 653d  ,.        force=
+000029b0: 666f 7263 652c 0a20 2020 2029 0a0a 0a64  force,.    )...d
+000029c0: 6566 2073 696d 706c 6966 7928 0a20 2020  ef simplify(.   
+000029d0: 2069 6e70 7574 5f70 6174 683a 2050 6174   input_path: Pat
+000029e0: 682c 0a20 2020 206f 7574 7075 745f 7061  h,.    output_pa
+000029f0: 7468 3a20 5061 7468 2c0a 2020 2020 746f  th: Path,.    to
+00002a00: 6c65 7261 6e63 653a 2066 6c6f 6174 2c0a  lerance: float,.
+00002a10: 2020 2020 616c 676f 7269 7468 6d3a 2053      algorithm: S
+00002a20: 696d 706c 6966 7941 6c67 6f72 6974 686d  implifyAlgorithm
+00002a30: 203d 2053 696d 706c 6966 7941 6c67 6f72   = SimplifyAlgor
+00002a40: 6974 686d 2e52 414d 4552 5f44 4f55 474c  ithm.RAMER_DOUGL
+00002a50: 4153 5f50 4555 434b 4552 2c0a 2020 2020  AS_PEUCKER,.    
+00002a60: 6c6f 6f6b 6168 6561 643a 2069 6e74 203d  lookahead: int =
+00002a70: 2038 2c0a 2020 2020 696e 7075 745f 6c61   8,.    input_la
+00002a80: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
+00002a90: 725d 203d 204e 6f6e 652c 0a20 2020 206f  r] = None,.    o
+00002aa0: 7574 7075 745f 6c61 7965 723a 204f 7074  utput_layer: Opt
+00002ab0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00002ac0: 652c 0a20 2020 2063 6f6c 756d 6e73 3a20  e,.    columns: 
+00002ad0: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+00002ae0: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
+00002af0: 6578 706c 6f64 6563 6f6c 6c65 6374 696f  explodecollectio
+00002b00: 6e73 3a20 626f 6f6c 203d 2046 616c 7365  ns: bool = False
+00002b10: 2c0a 2020 2020 6772 6964 7369 7a65 3a20  ,.    gridsize: 
+00002b20: 666c 6f61 7420 3d20 302e 302c 0a20 2020  float = 0.0,.   
+00002b30: 206e 625f 7061 7261 6c6c 656c 3a20 696e   nb_parallel: in
+00002b40: 7420 3d20 2d31 2c0a 2020 2020 6261 7463  t = -1,.    batc
+00002b50: 6873 697a 653a 2069 6e74 203d 202d 312c  hsize: int = -1,
+00002b60: 0a20 2020 2066 6f72 6365 3a20 626f 6f6c  .    force: bool
+00002b70: 203d 2046 616c 7365 2c0a 293a 0a20 2020   = False,.):.   
+00002b80: 2023 2049 6e69 740a 2020 2020 6f70 6572   # Init.    oper
+00002b90: 6174 696f 6e5f 7061 7261 6d73 203d 207b  ation_params = {
+00002ba0: 0a20 2020 2020 2020 2022 746f 6c65 7261  .        "tolera
+00002bb0: 6e63 6522 3a20 746f 6c65 7261 6e63 652c  nce": tolerance,
+00002bc0: 0a20 2020 2020 2020 2022 616c 676f 7269  .        "algori
+00002bd0: 7468 6d22 3a20 616c 676f 7269 7468 6d2c  thm": algorithm,
+00002be0: 0a20 2020 2020 2020 2022 7374 6570 223a  .        "step":
+00002bf0: 206c 6f6f 6b61 6865 6164 2c0a 2020 2020   lookahead,.    
+00002c00: 7d0a 0a20 2020 2023 2047 6f21 0a20 2020  }..    # Go!.   
+00002c10: 2072 6574 7572 6e20 5f61 7070 6c79 5f67   return _apply_g
+00002c20: 656f 6f70 6572 6174 696f 6e5f 746f 5f6c  eooperation_to_l
+00002c30: 6179 6572 280a 2020 2020 2020 2020 696e  ayer(.        in
+00002c40: 7075 745f 7061 7468 3d69 6e70 7574 5f70  put_path=input_p
+00002c50: 6174 682c 0a20 2020 2020 2020 206f 7574  ath,.        out
+00002c60: 7075 745f 7061 7468 3d6f 7574 7075 745f  put_path=output_
+00002c70: 7061 7468 2c0a 2020 2020 2020 2020 6f70  path,.        op
+00002c80: 6572 6174 696f 6e3d 4765 6f4f 7065 7261  eration=GeoOpera
+00002c90: 7469 6f6e 2e53 494d 504c 4946 592c 0a20  tion.SIMPLIFY,. 
+00002ca0: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+00002cb0: 5f70 6172 616d 733d 6f70 6572 6174 696f  _params=operatio
+00002cc0: 6e5f 7061 7261 6d73 2c0a 2020 2020 2020  n_params,.      
+00002cd0: 2020 696e 7075 745f 6c61 7965 723d 696e    input_layer=in
+00002ce0: 7075 745f 6c61 7965 722c 0a20 2020 2020  put_layer,.     
+00002cf0: 2020 206f 7574 7075 745f 6c61 7965 723d     output_layer=
+00002d00: 6f75 7470 7574 5f6c 6179 6572 2c0a 2020  output_layer,.  
+00002d10: 2020 2020 2020 636f 6c75 6d6e 733d 636f        columns=co
+00002d20: 6c75 6d6e 732c 0a20 2020 2020 2020 2065  lumns,.        e
+00002d30: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
+00002d40: 733d 6578 706c 6f64 6563 6f6c 6c65 6374  s=explodecollect
+00002d50: 696f 6e73 2c0a 2020 2020 2020 2020 6772  ions,.        gr
+00002d60: 6964 7369 7a65 3d67 7269 6473 697a 652c  idsize=gridsize,
+00002d70: 0a20 2020 2020 2020 206e 625f 7061 7261  .        nb_para
+00002d80: 6c6c 656c 3d6e 625f 7061 7261 6c6c 656c  llel=nb_parallel
+00002d90: 2c0a 2020 2020 2020 2020 6261 7463 6873  ,.        batchs
+00002da0: 697a 653d 6261 7463 6873 697a 652c 0a20  ize=batchsize,. 
+00002db0: 2020 2020 2020 2066 6f72 6365 3d66 6f72         force=for
+00002dc0: 6365 2c0a 2020 2020 290a 0a0a 6465 6620  ce,.    )...def 
+00002dd0: 5f61 7070 6c79 5f67 656f 6f70 6572 6174  _apply_geooperat
+00002de0: 696f 6e5f 746f 5f6c 6179 6572 280a 2020  ion_to_layer(.  
+00002df0: 2020 696e 7075 745f 7061 7468 3a20 5061    input_path: Pa
+00002e00: 7468 2c0a 2020 2020 6f75 7470 7574 5f70  th,.    output_p
+00002e10: 6174 683a 2050 6174 682c 0a20 2020 206f  ath: Path,.    o
+00002e20: 7065 7261 7469 6f6e 3a20 4765 6f4f 7065  peration: GeoOpe
+00002e30: 7261 7469 6f6e 2c0a 2020 2020 6f70 6572  ration,.    oper
+00002e40: 6174 696f 6e5f 7061 7261 6d73 3a20 6469  ation_params: di
+00002e50: 6374 2c0a 2020 2020 696e 7075 745f 6c61  ct,.    input_la
+00002e60: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
+00002e70: 725d 203d 204e 6f6e 652c 0a20 2020 2063  r] = None,.    c
+00002e80: 6f6c 756d 6e73 3a20 4f70 7469 6f6e 616c  olumns: Optional
+00002e90: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
+00002ea0: 6e65 2c0a 2020 2020 6f75 7470 7574 5f6c  ne,.    output_l
+00002eb0: 6179 6572 3a20 4f70 7469 6f6e 616c 5b73  ayer: Optional[s
+00002ec0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00002ed0: 6578 706c 6f64 6563 6f6c 6c65 6374 696f  explodecollectio
+00002ee0: 6e73 3a20 626f 6f6c 203d 2046 616c 7365  ns: bool = False
+00002ef0: 2c0a 2020 2020 666f 7263 655f 6f75 7470  ,.    force_outp
+00002f00: 7574 5f67 656f 6d65 7472 7974 7970 653a  ut_geometrytype:
+00002f10: 2055 6e69 6f6e 5b47 656f 6d65 7472 7954   Union[GeometryT
+00002f20: 7970 652c 2073 7472 2c20 4e6f 6e65 5d20  ype, str, None] 
+00002f30: 3d20 4e6f 6e65 2c0a 2020 2020 6772 6964  = None,.    grid
+00002f40: 7369 7a65 3a20 666c 6f61 7420 3d20 302e  size: float = 0.
+00002f50: 302c 0a20 2020 206e 625f 7061 7261 6c6c  0,.    nb_parall
+00002f60: 656c 3a20 696e 7420 3d20 2d31 2c0a 2020  el: int = -1,.  
+00002f70: 2020 6261 7463 6873 697a 653a 2069 6e74    batchsize: int
+00002f80: 203d 202d 312c 0a20 2020 2066 6f72 6365   = -1,.    force
+00002f90: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00002fa0: 293a 0a20 2020 2022 2222 0a20 2020 2041  ):.    """.    A
+00002fb0: 7070 6c69 6573 2061 2067 656f 206f 7065  pplies a geo ope
+00002fc0: 7261 7469 6f6e 206f 6e20 6120 6c61 7965  ration on a laye
+00002fd0: 722e 0a0a 2020 2020 5468 6520 6f70 6572  r...    The oper
+00002fe0: 6174 696f 6e20 746f 2061 7070 6c79 2063  ation to apply c
+00002ff0: 616e 2062 6520 6f6e 6520 6f66 2074 6865  an be one of the
+00003000: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+00003010: 2020 2020 2020 2d20 4255 4646 4552 3a20        - BUFFER: 
+00003020: 6170 706c 7920 6120 6275 6666 6572 2e20  apply a buffer. 
+00003030: 4f70 6572 6174 696f 6e20 7061 7261 6d65  Operation parame
+00003040: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
+00003050: 2d20 6469 7374 616e 6365 3a20 6469 7374  - distance: dist
+00003060: 616e 6365 2074 6f20 6275 6666 6572 0a20  ance to buffer. 
+00003070: 2020 2020 2020 2020 202d 2071 7561 6472           - quadr
+00003080: 616e 7473 6567 6d65 6e74 733a 206e 756d  antsegments: num
+00003090: 6265 7220 6f66 2070 6f69 6e74 7320 7573  ber of points us
+000030a0: 6564 2074 6f20 7265 7072 6573 656e 7420  ed to represent 
+000030b0: 312f 3420 6f66 2061 2063 6972 636c 650a  1/4 of a circle.
+000030c0: 2020 2020 2020 2020 2020 2d20 656e 6463            - endc
+000030d0: 6170 5f73 7479 6c65 3a20 6275 6666 6572  ap_style: buffer
+000030e0: 2073 7479 6c65 2074 6f20 7573 6520 666f   style to use fo
+000030f0: 7220 6120 706f 696e 7420 6f72 2074 6865  r a point or the
+00003100: 2065 6e64 2070 6f69 6e74 7320 6f66 0a20   end points of. 
+00003110: 2020 2020 2020 2020 2020 2061 206c 696e             a lin
+00003120: 653a 0a20 2020 2020 2020 2020 2020 202d  e:.            -
+00003130: 2052 4f55 4e44 3a20 666f 7220 706f 696e   ROUND: for poin
+00003140: 7473 2061 6e64 206c 696e 6573 2074 6865  ts and lines the
+00003150: 2065 6e64 7320 6172 6520 6275 6666 6572   ends are buffer
+00003160: 6564 2072 6f75 6e64 6564 2e0a 2020 2020  ed rounded..    
+00003170: 2020 2020 2020 2020 2d20 464c 4154 3a20          - FLAT: 
+00003180: 6120 706f 696e 7420 7374 6179 7320 6120  a point stays a 
+00003190: 706f 696e 742c 2061 2062 7566 6665 7265  point, a buffere
+000031a0: 6420 6c69 6e65 2077 696c 6c20 656e 6420  d line will end 
+000031b0: 666c 6174 0a20 2020 2020 2020 2020 2020  flat.           
+000031c0: 2020 2061 7420 7468 6520 656e 6420 706f     at the end po
+000031d0: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
+000031e0: 202d 2053 5155 4152 453a 2061 2070 6f69   - SQUARE: a poi
+000031f0: 6e74 2062 6563 6f6d 6573 2061 2073 7175  nt becomes a squ
+00003200: 6172 652c 2061 2062 7566 6665 7265 6420  are, a buffered 
+00003210: 6c69 6e65 2077 696c 6c20 656e 640a 2020  line will end.  
+00003220: 2020 2020 2020 2020 2020 2020 666c 6174              flat
+00003230: 2061 7420 7468 6520 656e 6420 706f 696e   at the end poin
+00003240: 7473 2c20 6275 7420 656c 6f6e 6761 7465  ts, but elongate
+00003250: 6420 6279 2022 6469 7374 616e 6365 220a  d by "distance".
+00003260: 2020 2020 2020 2020 2d20 6a6f 696e 5f73          - join_s
+00003270: 7479 6c65 3a20 6275 6666 6572 2073 7479  tyle: buffer sty
+00003280: 6c65 2074 6f20 7573 6520 666f 7220 636f  le to use for co
+00003290: 726e 6572 7320 696e 2061 206c 696e 6520  rners in a line 
+000032a0: 6f72 2061 2070 6f6c 7967 6f6e 0a20 2020  or a polygon.   
+000032b0: 2020 2020 2020 2062 6f75 6e64 6172 793a         boundary:
+000032c0: 0a20 2020 2020 2020 2020 2020 202d 2052  .            - R
+000032d0: 4f55 4e44 3a20 636f 726e 6572 7320 696e  OUND: corners in
+000032e0: 2074 6865 2072 6573 756c 7420 6172 6520   the result are 
+000032f0: 726f 756e 6465 640a 2020 2020 2020 2020  rounded.        
+00003300: 2020 2020 2d20 4d49 5452 453a 2063 6f72      - MITRE: cor
+00003310: 6e65 7273 2069 6e20 7468 6520 7265 7375  ners in the resu
+00003320: 6c74 2061 7265 2073 6861 7270 0a20 2020  lt are sharp.   
+00003330: 2020 2020 2020 2020 202d 2042 4556 454c           - BEVEL
+00003340: 3a20 6172 6520 666c 6174 7465 6e65 640a  : are flattened.
+00003350: 2020 2020 2020 2020 2d20 6d69 7472 655f          - mitre_
+00003360: 6c69 6d69 743a 2069 6e20 6361 7365 206f  limit: in case o
+00003370: 6620 6a6f 696e 5f73 7479 6c65 204d 4954  f join_style MIT
+00003380: 5245 2c20 6966 2074 6865 0a20 2020 2020  RE, if the.     
+00003390: 2020 2020 2020 2073 7069 6b79 2072 6573         spiky res
+000033a0: 756c 7420 666f 7220 6120 7368 6172 7020  ult for a sharp 
+000033b0: 616e 676c 6520 6265 636f 6d65 7320 6c6f  angle becomes lo
+000033c0: 6e67 6572 2074 6861 6e20 7468 6973 206c  nger than this l
+000033d0: 696d 6974 2c20 6974 0a20 2020 2020 2020  imit, it.       
+000033e0: 2020 2020 2069 7320 2262 6576 656c 6564       is "beveled
+000033f0: 2220 6174 2074 6869 7320 6469 7374 616e  " at this distan
+00003400: 6365 2e20 4465 6661 756c 7473 2074 6f20  ce. Defaults to 
+00003410: 352e 302e 0a20 2020 2020 2020 202d 2073  5.0..        - s
+00003420: 696e 676c 655f 7369 6465 643a 206f 6e6c  ingle_sided: onl
+00003430: 7920 6f6e 6520 7369 6465 206f 6620 7468  y one side of th
+00003440: 6520 6c69 6e65 2069 7320 6275 6666 6572  e line is buffer
+00003450: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+00003460: 6966 2064 6973 7461 6e63 6520 6973 206e  if distance is n
+00003470: 6567 6174 6976 652c 2074 6865 206c 6566  egative, the lef
+00003480: 7420 7369 6465 2c20 6966 2064 6973 7461  t side, if dista
+00003490: 6e63 6520 6973 2070 6f73 6974 6976 652c  nce is positive,
+000034a0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+000034b0: 2072 6967 6874 2068 616e 6420 7369 6465   right hand side
+000034c0: 2e20 4f6e 6c79 2072 656c 6576 616e 7420  . Only relevant 
+000034d0: 666f 7220 6c69 6e65 2067 656f 6d65 7472  for line geometr
+000034e0: 6965 732e 0a20 2020 2020 202d 2043 4f4e  ies..      - CON
+000034f0: 5645 5848 554c 4c3a 2061 7070 7920 6120  VEXHULL: appy a 
+00003500: 636f 6e76 6578 2068 756c 6c2e 0a20 2020  convex hull..   
+00003510: 2020 202d 2053 494d 504c 4946 593a 2073     - SIMPLIFY: s
+00003520: 696d 706c 6966 7920 7468 6520 6765 6f6d  implify the geom
+00003530: 6574 7279 2e20 4f70 6572 6174 696f 6e20  etry. Operation 
+00003540: 7061 7261 6d65 7465 7273 3a0a 2020 2020  parameters:.    
+00003550: 2020 2020 2020 2d20 616c 676f 7269 7468        - algorith
+00003560: 6d3a 2076 6563 746f 725f 7574 696c 2e53  m: vector_util.S
+00003570: 696d 706c 6966 7941 6c67 6f72 6974 686d  implifyAlgorithm
+00003580: 0a20 2020 2020 2020 2020 202d 2074 6f6c  .          - tol
+00003590: 6572 616e 6365 3a20 6d61 7869 6d75 6d20  erance: maximum 
+000035a0: 6469 7374 616e 6365 2074 6f20 7369 6d70  distance to simp
+000035b0: 6c69 6679 2e0a 2020 2020 2020 2020 2020  lify..          
+000035c0: 2d20 6c6f 6f6b 6168 6561 643a 2066 6f72  - lookahead: for
+000035d0: 204c 414e 472c 2074 6865 206e 756d 6265   LANG, the numbe
+000035e0: 7220 6f66 2070 6f69 6e74 7320 746f 2066  r of points to f
+000035f0: 6f72 7761 7264 2d6c 6f6f 6b0a 2020 2020  orward-look.    
+00003600: 2020 2d20 4150 504c 593a 2061 7070 6c79    - APPLY: apply
+00003610: 2061 206c 616d 6264 6120 6675 6e63 7469   a lambda functi
+00003620: 6f6e 2e20 4f70 6572 6174 696f 6e20 7061  on. Operation pa
+00003630: 7261 6d65 7465 723a 0a20 2020 2020 2020  rameter:.       
+00003640: 2020 202d 2070 6963 6b6c 6564 5f66 756e     - pickled_fun
+00003650: 633a 206c 616d 6264 6120 6675 6e63 7469  c: lambda functi
+00003660: 6f6e 2074 6f20 6170 706c 792c 2070 6963  on to apply, pic
+00003670: 6b6c 6564 2074 6f20 6279 7465 732e 0a20  kled to bytes.. 
+00003680: 2020 2020 2020 2020 202d 206f 6e6c 795f           - only_
+00003690: 6765 6f6d 5f69 6e70 7574 3a20 6966 2054  geom_input: if T
+000036a0: 7275 652c 206f 6e6c 7920 7468 6520 6765  rue, only the ge
+000036b0: 6f6d 6574 7279 2069 7320 6176 6169 6c61  ometry is availa
+000036c0: 626c 6520 6173 0a20 2020 2020 2020 2020  ble as.         
+000036d0: 2020 2069 6e70 7574 2066 6f72 2074 6865     input for the
+000036e0: 206c 616d 6264 6120 6675 6e63 7469 6f6e   lambda function
+000036f0: 2e20 4966 2066 616c 7365 2c20 7468 6520  . If false, the 
+00003700: 726f 7720 6973 2074 6865 2069 6e70 7574  row is the input
+00003710: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00003720: 2020 2020 2069 6e70 7574 5f70 6174 6820       input_path 
+00003730: 2850 6174 6829 3a20 5b64 6573 6372 6970  (Path): [descrip
+00003740: 7469 6f6e 5d0a 2020 2020 2020 2020 6f75  tion].        ou
+00003750: 7470 7574 5f70 6174 6820 2850 6174 6829  tput_path (Path)
+00003760: 3a20 5b64 6573 6372 6970 7469 6f6e 5d0a  : [description].
+00003770: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
+00003780: 6e20 2847 656f 4f70 6572 6174 696f 6e29  n (GeoOperation)
+00003790: 3a20 7468 6520 6765 6f20 6f70 6572 6174  : the geo operat
+000037a0: 696f 6e20 746f 2061 7070 6c79 2e0a 2020  ion to apply..  
+000037b0: 2020 2020 2020 6f70 6572 6174 696f 6e5f        operation_
+000037c0: 7061 7261 6d73 2028 6469 6374 2c20 6f70  params (dict, op
+000037d0: 7469 6f6e 616c 293a 2074 6865 2070 6172  tional): the par
+000037e0: 616d 6574 6572 7320 666f 7220 7468 6520  ameters for the 
+000037f0: 6765 6f20 6f70 6572 6174 696f 6e2e 0a20  geo operation.. 
+00003800: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00003810: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
+00003820: 2020 2020 2069 6e70 7574 5f6c 6179 6572       input_layer
+00003830: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+00003840: 3a20 5b64 6573 6372 6970 7469 6f6e 5d2e  : [description].
+00003850: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00003860: 652e 0a20 2020 2020 2020 206f 7574 7075  e..        outpu
+00003870: 745f 6c61 7965 7220 2873 7472 2c20 6f70  t_layer (str, op
+00003880: 7469 6f6e 616c 293a 205b 6465 7363 7269  tional): [descri
+00003890: 7074 696f 6e5d 2e20 4465 6661 756c 7473  ption]. Defaults
+000038a0: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
+000038b0: 2020 636f 6c75 6d6e 7320 284c 6973 745b    columns (List[
+000038c0: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
+000038d0: 2049 6620 6e6f 7420 4e6f 6e65 2c20 6f6e   If not None, on
+000038e0: 6c79 206f 7574 7075 7420 7468 6520 636f  ly output the co
+000038f0: 6c75 6d6e 730a 2020 2020 2020 2020 2020  lumns.          
+00003900: 2020 7370 6563 6966 6965 642e 2044 6566    specified. Def
+00003910: 6175 6c74 7320 746f 204e 6f6e 652e 0a20  aults to None.. 
+00003920: 2020 2020 2020 2065 7870 6c6f 6465 636f         explodeco
+00003930: 6c6c 6563 7469 6f6e 7320 2862 6f6f 6c2c  llections (bool,
+00003940: 206f 7074 696f 6e61 6c29 3a20 5472 7565   optional): True
+00003950: 2074 6f20 636f 6e76 6572 7420 616c 6c20   to convert all 
+00003960: 6d75 6c74 692d 6765 6f6d 6574 7269 6573  multi-geometries
+00003970: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+00003980: 7369 6e67 756c 6172 206f 6e65 7320 6475  singular ones du
+00003990: 7269 6e67 2074 6865 2067 656f 6f70 6572  ring the geooper
+000039a0: 6174 696f 6e2e 2044 6566 6175 6c74 7320  ation. Defaults 
+000039b0: 746f 2046 616c 7365 2e0a 2020 2020 2020  to False..      
+000039c0: 2020 666f 7263 655f 6f75 7470 7574 5f67    force_output_g
+000039d0: 656f 6d65 7472 7974 7970 6520 2847 656f  eometrytype (Geo
+000039e0: 6d65 7472 7954 7970 652c 206f 7074 696f  metryType, optio
+000039f0: 6e61 6c29 3a20 5468 6520 6f75 7470 7574  nal): The output
+00003a00: 2067 656f 6d65 7472 7920 7479 7065 2074   geometry type t
+00003a10: 6f0a 2020 2020 2020 2020 2020 2020 666f  o.            fo
+00003a20: 7263 652e 2049 6620 4e6f 6e65 2c20 6120  rce. If None, a 
+00003a30: 6265 7374 2d65 6666 6f72 7420 6775 6573  best-effort gues
+00003a40: 7320 6973 206d 6164 652e 2044 6566 6175  s is made. Defau
+00003a50: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
+00003a60: 2020 2020 2067 7269 6473 697a 6520 2866       gridsize (f
+00003a70: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
+00003a80: 2074 6865 2073 697a 6520 6f66 2074 6865   the size of the
+00003a90: 2067 7269 6420 7468 6520 636f 6f72 6469   grid the coordi
+00003aa0: 6e61 7465 7320 6f66 2074 6865 206f 7570  nates of the oup
+00003ab0: 7574 0a20 2020 2020 2020 2020 2020 2077  ut.            w
+00003ac0: 696c 6c20 6265 2072 6f75 6e64 6564 2074  ill be rounded t
+00003ad0: 6f2e 2045 672e 2030 2e30 3031 2074 6f20  o. Eg. 0.001 to 
+00003ae0: 6b65 6570 2033 2064 6563 696d 616c 732e  keep 3 decimals.
+00003af0: 2056 616c 7565 2030 2e30 2064 6f65 736e   Value 0.0 doesn
+00003b00: 2774 2063 6861 6e67 650a 2020 2020 2020  't change.      
+00003b10: 2020 2020 2020 7468 6520 7072 6563 6973        the precis
+00003b20: 696f 6e2e 2044 6566 6175 6c74 7320 746f  ion. Defaults to
+00003b30: 2030 2e30 2e0a 2020 2020 2020 2020 6e62   0.0..        nb
+00003b40: 5f70 6172 616c 6c65 6c20 2869 6e74 2c20  _parallel (int, 
+00003b50: 6f70 7469 6f6e 616c 293a 205b 6465 7363  optional): [desc
+00003b60: 7269 7074 696f 6e5d 2e20 4465 6661 756c  ription]. Defaul
+00003b70: 7473 2074 6f20 2d31 2e0a 2020 2020 2020  ts to -1..      
+00003b80: 2020 6261 7463 6873 697a 6520 2869 6e74    batchsize (int
+00003b90: 2c20 6f70 7469 6f6e 616c 293a 2069 6e64  , optional): ind
+00003ba0: 6963 6174 6976 6520 6e75 6d62 6572 206f  icative number o
+00003bb0: 6620 726f 7773 2074 6f20 7072 6f63 6573  f rows to proces
+00003bc0: 7320 7065 720a 2020 2020 2020 2020 2020  s per.          
+00003bd0: 2020 6261 7463 682e 2041 2073 6d61 6c6c    batch. A small
+00003be0: 6572 2062 6174 6368 2073 697a 652c 2070  er batch size, p
+00003bf0: 6f73 7369 626c 7920 696e 2063 6f6d 6269  ossibly in combi
+00003c00: 6e61 7469 6f6e 2077 6974 6820 610a 2020  nation with a.  
+00003c10: 2020 2020 2020 2020 2020 736d 616c 6c65            smalle
+00003c20: 7220 6e62 5f70 6172 616c 6c65 6c2c 2077  r nb_parallel, w
+00003c30: 696c 6c20 7265 6475 6365 2074 6865 206d  ill reduce the m
+00003c40: 656d 6f72 7920 7573 6167 652e 0a20 2020  emory usage..   
+00003c50: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00003c60: 7320 746f 202d 313a 2028 7472 7920 746f  s to -1: (try to
+00003c70: 2920 6465 7465 726d 696e 6520 6f70 7469  ) determine opti
+00003c80: 6d61 6c20 7369 7a65 2061 7574 6f6d 6174  mal size automat
+00003c90: 6963 616c 6c79 2e0a 2020 2020 2020 2020  ically..        
+00003ca0: 666f 7263 6520 2862 6f6f 6c2c 206f 7074  force (bool, opt
+00003cb0: 696f 6e61 6c29 3a20 5b64 6573 6372 6970  ional): [descrip
+00003cc0: 7469 6f6e 5d2e 2044 6566 6175 6c74 7320  tion]. Defaults 
+00003cd0: 746f 2046 616c 7365 2e0a 2020 2020 2222  to False..    ""
+00003ce0: 220a 2020 2020 2320 496e 6974 0a20 2020  ".    # Init.   
+00003cf0: 2073 7461 7274 5f74 696d 655f 676c 6f62   start_time_glob
+00003d00: 616c 203d 2064 6174 6574 696d 652e 6e6f  al = datetime.no
+00003d10: 7728 290a 0a20 2020 2023 2043 6865 636b  w()..    # Check
+00003d20: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+00003d30: 732e 2e2e 0a20 2020 206f 7065 7261 7469  s....    operati
+00003d40: 6f6e 5f6e 616d 6520 3d20 6f70 6572 6174  on_name = operat
+00003d50: 696f 6e2e 6e61 6d65 2e6c 6f77 6572 2829  ion.name.lower()
+00003d60: 0a20 2020 2069 6620 6e6f 7420 696e 7075  .    if not inpu
+00003d70: 745f 7061 7468 2e65 7869 7374 7328 293a  t_path.exists():
+00003d80: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00003d90: 616c 7565 4572 726f 7228 6622 7b6f 7065  alueError(f"{ope
+00003da0: 7261 7469 6f6e 5f6e 616d 657d 3a20 696e  ration_name}: in
+00003db0: 7075 745f 7061 7468 2064 6f65 736e 2774  put_path doesn't
+00003dc0: 2065 7869 7374 3a20 7b69 6e70 7574 5f70   exist: {input_p
+00003dd0: 6174 687d 2229 0a20 2020 2069 6620 696e  ath}").    if in
+00003de0: 7075 745f 7061 7468 203d 3d20 6f75 7470  put_path == outp
+00003df0: 7574 5f70 6174 683a 0a20 2020 2020 2020  ut_path:.       
+00003e00: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00003e10: 7228 6622 7b6f 7065 7261 7469 6f6e 5f6e  r(f"{operation_n
+00003e20: 616d 657d 3a20 6f75 7470 7574 5f70 6174  ame}: output_pat
+00003e30: 6820 6d75 7374 206e 6f74 2065 7175 616c  h must not equal
+00003e40: 2069 6e70 7574 5f70 6174 6822 290a 2020   input_path").  
+00003e50: 2020 6966 2069 6e70 7574 5f6c 6179 6572    if input_layer
+00003e60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00003e70: 2020 696e 7075 745f 6c61 7965 7220 3d20    input_layer = 
+00003e80: 6766 6f2e 6765 745f 6f6e 6c79 5f6c 6179  gfo.get_only_lay
+00003e90: 6572 2869 6e70 7574 5f70 6174 6829 0a20  er(input_path). 
+00003ea0: 2020 2069 6620 6f75 7470 7574 5f70 6174     if output_pat
+00003eb0: 682e 6578 6973 7473 2829 3a0a 2020 2020  h.exists():.    
+00003ec0: 2020 2020 6966 2066 6f72 6365 2069 7320      if force is 
+00003ed0: 4661 6c73 653a 0a20 2020 2020 2020 2020  False:.         
+00003ee0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+00003ef0: 2253 746f 7020 7b6f 7065 7261 7469 6f6e  "Stop {operation
+00003f00: 5f6e 616d 657d 3a20 6f75 7470 7574 2065  _name}: output e
+00003f10: 7869 7374 7320 616c 7265 6164 7920 7b6f  xists already {o
+00003f20: 7574 7075 745f 7061 7468 7d22 290a 2020  utput_path}").  
+00003f30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00003f40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00003f50: 2020 2020 2020 2020 2020 2067 666f 2e72             gfo.r
+00003f60: 656d 6f76 6528 6f75 7470 7574 5f70 6174  emove(output_pat
+00003f70: 6829 0a20 2020 2069 6620 696e 7075 745f  h).    if input_
+00003f80: 6c61 7965 7220 6973 204e 6f6e 653a 0a20  layer is None:. 
+00003f90: 2020 2020 2020 2069 6e70 7574 5f6c 6179         input_lay
+00003fa0: 6572 203d 2067 666f 2e67 6574 5f6f 6e6c  er = gfo.get_onl
+00003fb0: 795f 6c61 7965 7228 696e 7075 745f 7061  y_layer(input_pa
+00003fc0: 7468 290a 2020 2020 6966 206f 7574 7075  th).    if outpu
+00003fd0: 745f 6c61 7965 7220 6973 204e 6f6e 653a  t_layer is None:
+00003fe0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+00003ff0: 6c61 7965 7220 3d20 6766 6f2e 6765 745f  layer = gfo.get_
+00004000: 6465 6661 756c 745f 6c61 7965 7228 6f75  default_layer(ou
+00004010: 7470 7574 5f70 6174 6829 0a20 2020 2069  tput_path).    i
+00004020: 6620 6973 696e 7374 616e 6365 2866 6f72  f isinstance(for
+00004030: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
+00004040: 7279 7479 7065 2c20 4765 6f6d 6574 7279  rytype, Geometry
+00004050: 5479 7065 293a 0a20 2020 2020 2020 2066  Type):.        f
+00004060: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
+00004070: 6574 7279 7479 7065 203d 2066 6f72 6365  etrytype = force
+00004080: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+00004090: 7479 7065 2e6e 616d 650a 0a20 2020 2023  type.name..    #
+000040a0: 2050 7265 7061 7265 2074 6d70 2066 696c   Prepare tmp fil
+000040b0: 6573 0a20 2020 2074 656d 7064 6972 203d  es.    tempdir =
+000040c0: 205f 696f 5f75 7469 6c2e 6372 6561 7465   _io_util.create
+000040d0: 5f74 656d 7064 6972 2866 2267 656f 6669  _tempdir(f"geofi
+000040e0: 6c65 6f70 732f 7b6f 7065 7261 7469 6f6e  leops/{operation
+000040f0: 2e76 616c 7565 7d22 290a 2020 2020 6c6f  .value}").    lo
+00004100: 6767 6572 2e69 6e66 6f28 6622 5374 6172  gger.info(f"Star
+00004110: 7420 6361 6c63 756c 6174 696f 6e20 746f  t calculation to
+00004120: 2074 656d 7020 6669 6c65 7320 696e 207b   temp files in {
+00004130: 7465 6d70 6469 727d 2229 0a0a 2020 2020  tempdir}")..    
+00004140: 2320 4361 6c63 756c 6174 650a 2020 2020  # Calculate.    
+00004150: 7472 793a 0a20 2020 2020 2020 2023 2052  try:.        # R
+00004160: 656d 6172 6b3a 2063 616c 6375 6c61 7469  emark: calculati
+00004170: 6e67 2063 616e 2062 6520 646f 6e65 2069  ng can be done i
+00004180: 6e20 7061 7261 6c6c 656c 2c20 6275 7420  n parallel, but 
+00004190: 6f6e 6c79 206f 6e65 2070 726f 6365 7373  only one process
+000041a0: 0a20 2020 2020 2020 2023 2063 616e 2077  .        # can w
+000041b0: 7269 7465 2074 6f20 7468 6520 7361 6d65  rite to the same
+000041c0: 206f 7574 7075 7420 6669 6c65 2061 7420   output file at 
+000041d0: 7468 6520 7469 6d65 2e2e 2e0a 0a20 2020  the time.....   
+000041e0: 2020 2020 2023 2043 616c 6375 6c61 7465       # Calculate
+000041f0: 2074 6865 2062 6573 7420 6e75 6d62 6572   the best number
+00004200: 206f 6620 7061 7261 6c6c 656c 2070 726f   of parallel pro
+00004210: 6365 7373 6573 2061 6e64 2062 6174 6368  cesses and batch
+00004220: 6573 2066 6f72 0a20 2020 2020 2020 2023  es for.        #
+00004230: 2074 6865 2061 7661 696c 6162 6c65 2072   the available r
+00004240: 6573 6f75 7263 6573 0a20 2020 2020 2020  esources.       
+00004250: 2069 6e70 7574 5f6c 6179 6572 696e 666f   input_layerinfo
+00004260: 203d 2067 666f 2e67 6574 5f6c 6179 6572   = gfo.get_layer
+00004270: 696e 666f 2869 6e70 7574 5f70 6174 682c  info(input_path,
+00004280: 2069 6e70 7574 5f6c 6179 6572 290a 2020   input_layer).  
+00004290: 2020 2020 2020 6e62 5f72 6f77 735f 746f        nb_rows_to
+000042a0: 7461 6c20 3d20 696e 7075 745f 6c61 7965  tal = input_laye
+000042b0: 7269 6e66 6f2e 6665 6174 7572 6563 6f75  rinfo.featurecou
+000042c0: 6e74 0a20 2020 2020 2020 2069 6620 6261  nt.        if ba
+000042d0: 7463 6873 697a 6520 3e20 303a 0a20 2020  tchsize > 0:.   
+000042e0: 2020 2020 2020 2020 2070 6172 616c 6c65           paralle
+000042f0: 6c6c 697a 6174 696f 6e5f 636f 6e66 6967  llization_config
+00004300: 203d 2050 6172 616c 6c65 6c69 7a61 7469   = Parallelizati
+00004310: 6f6e 436f 6e66 6967 280a 2020 2020 2020  onConfig(.      
+00004320: 2020 2020 2020 2020 2020 6d69 6e5f 6176            min_av
+00004330: 675f 726f 7773 5f70 6572 5f62 6174 6368  g_rows_per_batch
+00004340: 3d6d 6174 682e 6365 696c 2862 6174 6368  =math.ceil(batch
+00004350: 7369 7a65 202f 2032 292c 0a20 2020 2020  size / 2),.     
+00004360: 2020 2020 2020 2020 2020 206d 6178 5f61             max_a
+00004370: 7667 5f72 6f77 735f 7065 725f 6261 7463  vg_rows_per_batc
+00004380: 683d 6261 7463 6873 697a 652c 0a20 2020  h=batchsize,.   
+00004390: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000043a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000043b0: 2020 2020 2070 6172 616c 6c65 6c6c 697a       parallelliz
+000043c0: 6174 696f 6e5f 636f 6e66 6967 203d 2050  ation_config = P
+000043d0: 6172 616c 6c65 6c69 7a61 7469 6f6e 436f  arallelizationCo
+000043e0: 6e66 6967 280a 2020 2020 2020 2020 2020  nfig(.          
+000043f0: 2020 2020 2020 6d61 785f 6176 675f 726f        max_avg_ro
+00004400: 7773 5f70 6572 5f62 6174 6368 3d35 3030  ws_per_batch=500
+00004410: 3030 0a20 2020 2020 2020 2020 2020 2029  00.            )
+00004420: 0a20 2020 2020 2020 206e 625f 7061 7261  .        nb_para
+00004430: 6c6c 656c 2c20 6e62 5f62 6174 6368 6573  llel, nb_batches
+00004440: 2c20 7265 616c 5f62 6174 6368 7369 7a65  , real_batchsize
+00004450: 203d 2067 6574 5f70 6172 616c 6c65 6c69   = get_paralleli
+00004460: 7a61 7469 6f6e 5f70 6172 616d 7328 0a20  zation_params(. 
+00004470: 2020 2020 2020 2020 2020 206e 625f 726f             nb_ro
+00004480: 7773 5f74 6f74 616c 3d6e 625f 726f 7773  ws_total=nb_rows
+00004490: 5f74 6f74 616c 2c0a 2020 2020 2020 2020  _total,.        
+000044a0: 2020 2020 6e62 5f70 6172 616c 6c65 6c3d      nb_parallel=
+000044b0: 6e62 5f70 6172 616c 6c65 6c2c 0a20 2020  nb_parallel,.   
+000044c0: 2020 2020 2020 2020 2070 6172 616c 6c65           paralle
+000044d0: 6c69 7a61 7469 6f6e 5f63 6f6e 6669 673d  lization_config=
+000044e0: 7061 7261 6c6c 656c 6c69 7a61 7469 6f6e  parallellization
+000044f0: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
+00004500: 2029 0a0a 2020 2020 2020 2020 2320 544f   )..        # TO
+00004510: 444f 3a20 6465 7465 726d 696e 6520 7468  DO: determine th
+00004520: 6520 6f70 7469 6d61 6c20 6261 7463 6820  e optimal batch 
+00004530: 7369 7a65 7320 7769 7468 206d 696e 2061  sizes with min a
+00004540: 6e64 206d 6178 206f 6620 726f 7769 6420  nd max of rowid 
+00004550: 7769 6c6c 0a20 2020 2020 2020 2023 2069  will.        # i
+00004560: 6e20 736f 6d65 2063 6173 6520 696d 7072  n some case impr
+00004570: 6f76 6520 7065 7266 6f72 6d61 6e63 650a  ove performance.
+00004580: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00004590: 2020 2020 7371 6c5f 7374 6d74 203d 2066      sql_stmt = f
+000045a0: 2727 2753 454c 4543 5420 4d49 4e28 726f  '''SELECT MIN(ro
+000045b0: 7769 6429 2061 7320 6d69 6e5f 726f 7769  wid) as min_rowi
+000045c0: 642c 204d 4158 2872 6f77 6964 2920 6173  d, MAX(rowid) as
+000045d0: 206d 6178 5f72 6f77 6964 0a20 2020 2020   max_rowid.     
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045f0: 2020 2020 4652 4f4d 2022 7b69 6e70 7574      FROM "{input
+00004600: 5f6c 6179 6572 7d22 2727 270a 2020 2020  _layer}"'''.    
+00004610: 2020 2020 7265 7375 6c74 203d 2067 666f      result = gfo
+00004620: 2e72 6561 645f 6669 6c65 280a 2020 2020  .read_file(.    
+00004630: 2020 2020 2020 2020 7061 7468 3d74 656d          path=tem
+00004640: 705f 7061 7468 2c20 6c61 7965 723d 696e  p_path, layer=in
+00004650: 7075 745f 6c61 7965 722c 2073 716c 5f73  put_layer, sql_s
+00004660: 746d 743d 7371 6c5f 7374 6d74 2c20 7371  tmt=sql_stmt, sq
+00004670: 6c5f 6469 616c 6563 743d 2253 514c 4954  l_dialect="SQLIT
+00004680: 4522 0a20 2020 2020 2020 2029 0a20 2020  E".        ).   
+00004690: 2020 2020 2069 6620 6c65 6e28 7265 7375       if len(resu
+000046a0: 6c74 2920 3d3d 2031 3a0a 2020 2020 2020  lt) == 1:.      
+000046b0: 2020 2020 2020 6d69 6e5f 726f 7769 6420        min_rowid 
+000046c0: 3d20 7265 7375 6c74 5b27 6d69 6e5f 726f  = result['min_ro
+000046d0: 7769 6427 5d2e 7661 6c75 6573 5b30 5d0a  wid'].values[0].
+000046e0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+000046f0: 726f 7769 6420 3d20 7265 7375 6c74 5b27  rowid = result['
+00004700: 6d61 785f 726f 7769 6427 5d2e 7661 6c75  max_rowid'].valu
+00004710: 6573 5b30 5d0a 2020 2020 2020 2020 2020  es[0].          
+00004720: 2020 6e62 5f72 6f77 6964 735f 7065 725f    nb_rowids_per_
+00004730: 6261 7463 6820 3d20 286d 6178 5f72 6f77  batch = (max_row
+00004740: 6964 202d 206d 696e 5f72 6f77 6964 292f  id - min_rowid)/
+00004750: 6e62 5f62 6174 6368 6573 0a20 2020 2020  nb_batches.     
+00004760: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00004770: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00004780: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00004790: 2020 2020 2020 6622 4572 726f 7220 6765        f"Error ge
+000047a0: 7474 696e 6720 6d69 6e20 616e 6420 6d61  tting min and ma
+000047b0: 7820 726f 7769 6420 666f 7220 7b74 656d  x rowid for {tem
+000047c0: 705f 7061 7468 7d2c 206c 6179 6572 207b  p_path}, layer {
+000047d0: 696e 7075 745f 6c61 7965 727d 220a 2020  input_layer}".  
+000047e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000047f0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00004800: 2023 2050 726f 6365 7373 696e 6720 696e   # Processing in
+00004810: 2074 6872 6561 6473 2069 7320 3278 2066   threads is 2x f
+00004820: 6173 7465 7220 666f 7220 736d 616c 6c20  aster for small 
+00004830: 6461 7461 7365 7473 2028 6f6e 2057 696e  datasets (on Win
+00004840: 646f 7773 290a 2020 2020 2020 2020 6361  dows).        ca
+00004850: 6c63 756c 6174 655f 696e 5f74 6872 6561  lculate_in_threa
+00004860: 6473 203d 2054 7275 6520 6966 2069 6e70  ds = True if inp
+00004870: 7574 5f6c 6179 6572 696e 666f 2e66 6561  ut_layerinfo.fea
+00004880: 7475 7265 636f 756e 7420 3c3d 2031 3030  turecount <= 100
+00004890: 2065 6c73 6520 4661 6c73 650a 2020 2020   else False.    
+000048a0: 2020 2020 7769 7468 205f 7072 6f63 6573      with _proces
+000048b0: 7369 6e67 5f75 7469 6c2e 506f 6f6c 6564  sing_util.Pooled
+000048c0: 4578 6563 7574 6f72 4661 6374 6f72 7928  ExecutorFactory(
+000048d0: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
+000048e0: 6561 6470 6f6f 6c3d 6361 6c63 756c 6174  eadpool=calculat
+000048f0: 655f 696e 5f74 6872 6561 6473 2c0a 2020  e_in_threads,.  
+00004900: 2020 2020 2020 2020 2020 6d61 785f 776f            max_wo
+00004910: 726b 6572 733d 6e62 5f70 6172 616c 6c65  rkers=nb_paralle
+00004920: 6c2c 0a20 2020 2020 2020 2020 2020 2069  l,.            i
+00004930: 6e69 7469 616c 697a 6572 3d5f 7072 6f63  nitializer=_proc
+00004940: 6573 7369 6e67 5f75 7469 6c2e 696e 6974  essing_util.init
+00004950: 6961 6c69 7a65 5f77 6f72 6b65 7228 292c  ialize_worker(),
+00004960: 0a20 2020 2020 2020 2029 2061 7320 6361  .        ) as ca
+00004970: 6c63 756c 6174 655f 706f 6f6c 3a0a 2020  lculate_pool:.  
+00004980: 2020 2020 2020 2020 2020 2320 5072 6570            # Prep
+00004990: 6172 6520 6f75 7470 7574 2066 696c 656e  are output filen
+000049a0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+000049b0: 746d 705f 6f75 7470 7574 5f70 6174 6820  tmp_output_path 
+000049c0: 3d20 7465 6d70 6469 7220 2f20 6f75 7470  = tempdir / outp
+000049d0: 7574 5f70 6174 682e 6e61 6d65 0a0a 2020  ut_path.name..  
+000049e0: 2020 2020 2020 2020 2020 726f 775f 6f66            row_of
+000049f0: 6673 6574 203d 2030 0a20 2020 2020 2020  fset = 0.       
+00004a00: 2020 2020 2062 6174 6368 6573 203d 207b       batches = {
+00004a10: 7d0a 2020 2020 2020 2020 2020 2020 6675  }.            fu
+00004a20: 7475 7265 5f74 6f5f 6261 7463 685f 6964  ture_to_batch_id
+00004a30: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00004a40: 2020 6e62 5f64 6f6e 6520 3d20 300a 0a20    nb_done = 0.. 
+00004a50: 2020 2020 2020 2020 2020 2066 6f72 2062             for b
+00004a60: 6174 6368 5f69 6420 696e 2072 616e 6765  atch_id in range
+00004a70: 286e 625f 6261 7463 6865 7329 3a0a 2020  (nb_batches):.  
+00004a80: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+00004a90: 7463 6865 735b 6261 7463 685f 6964 5d20  tches[batch_id] 
+00004aa0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+00004ab0: 2020 2020 2062 6174 6368 6573 5b62 6174       batches[bat
+00004ac0: 6368 5f69 645d 5b22 6c61 7965 7222 5d20  ch_id]["layer"] 
+00004ad0: 3d20 6f75 7470 7574 5f6c 6179 6572 0a0a  = output_layer..
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004af0: 2320 4f75 7470 7574 2065 6163 6820 6261  # Output each ba
+00004b00: 7463 6820 746f 2061 2073 6570 6572 6174  tch to a seperat
+00004b10: 6520 7465 6d70 6f72 6172 7920 6669 6c65  e temporary file
+00004b20: 2c20 6f74 6865 7277 6973 6520 7468 6572  , otherwise ther
+00004b30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00004b40: 2020 2320 6172 6520 7469 6d65 6f75 7420    # are timeout 
+00004b50: 6973 7375 6573 2077 6865 6e20 7072 6f63  issues when proc
+00004b60: 6573 7369 6e67 206c 6172 6765 2066 696c  essing large fil
+00004b70: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00004b80: 2020 206f 7574 7075 745f 746d 705f 7061     output_tmp_pa
+00004b90: 7274 6961 6c5f 7061 7468 203d 2028 0a20  rtial_path = (. 
+00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bb0: 2020 2074 656d 7064 6972 202f 2066 227b     tempdir / f"{
+00004bc0: 6f75 7470 7574 5f70 6174 682e 7374 656d  output_path.stem
+00004bd0: 7d5f 7b62 6174 6368 5f69 647d 7b6f 7574  }_{batch_id}{out
+00004be0: 7075 745f 7061 7468 2e73 7566 6669 787d  put_path.suffix}
+00004bf0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004c00: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00004c10: 2020 2020 6261 7463 6865 735b 6261 7463      batches[batc
+00004c20: 685f 6964 5d5b 2274 6d70 5f70 6172 7469  h_id]["tmp_parti
+00004c30: 616c 5f6f 7574 7075 745f 7061 7468 225d  al_output_path"]
+00004c40: 203d 206f 7574 7075 745f 746d 705f 7061   = output_tmp_pa
+00004c50: 7274 6961 6c5f 7061 7468 0a0a 2020 2020  rtial_path..    
+00004c60: 2020 2020 2020 2020 2020 2020 2320 466f              # Fo
+00004c70: 7220 7468 6520 6c61 7374 2074 7261 6e73  r the last trans
+00004c80: 6c61 7465 5f69 642c 2074 616b 6520 616c  late_id, take al
+00004c90: 6c20 726f 7769 6427 7320 6c65 6674 2e2e  l rowid's left..
+00004ca0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004cb0: 2020 6966 2062 6174 6368 5f69 6420 3c20    if batch_id < 
+00004cc0: 6e62 5f62 6174 6368 6573 202d 2031 3a0a  nb_batches - 1:.
+00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ce0: 2020 2020 726f 7773 203d 2073 6c69 6365      rows = slice
+00004cf0: 2872 6f77 5f6f 6666 7365 742c 2072 6f77  (row_offset, row
+00004d00: 5f6f 6666 7365 7420 2b20 7265 616c 5f62  _offset + real_b
+00004d10: 6174 6368 7369 7a65 290a 2020 2020 2020  atchsize).      
+00004d20: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d40: 2020 2020 726f 7773 203d 2073 6c69 6365      rows = slice
+00004d50: 2872 6f77 5f6f 6666 7365 742c 206e 625f  (row_offset, nb_
+00004d60: 726f 7773 5f74 6f74 616c 290a 0a20 2020  rows_total)..   
+00004d70: 2020 2020 2020 2020 2020 2020 2023 2052               # R
+00004d80: 656d 6172 6b3a 2074 6869 7320 7465 6d70  emark: this temp
+00004d90: 2066 696c 6520 646f 6573 6e27 7420 6e65   file doesn't ne
+00004da0: 6564 2073 7061 7469 616c 2069 6e64 6578  ed spatial index
+00004db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004dc0: 2023 2052 656d 6172 6b3a 2062 6563 6175   # Remark: becau
+00004dd0: 7365 2066 6f72 6365 5f6f 7574 7075 745f  se force_output_
+00004de0: 6765 6f6d 6574 7279 7479 7065 2066 6f72  geometrytype for
+00004df0: 2047 656f 4461 7461 4672 616d 650a 2020   GeoDataFrame.  
+00004e00: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00004e10: 6f70 6572 6174 696f 6e73 2069 7320 2861  operations is (a
+00004e20: 206c 6f74 2920 6d6f 7265 206c 696d 6974   lot) more limit
+00004e30: 6564 2074 6861 6e20 6764 616c 2d62 6173  ed than gdal-bas
+00004e40: 6564 2c20 7468 6520 6764 616c 2076 6572  ed, the gdal ver
+00004e50: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
+00004e60: 2020 2020 2023 2069 7320 7573 6564 206c       # is used l
+00004e70: 6174 6572 206f 6e20 7768 656e 2074 6865  ater on when the
+00004e80: 2072 6573 756c 7473 2061 7265 206d 6572   results are mer
+00004e90: 6765 6420 746f 2074 6865 2072 6573 756c  ged to the resul
+00004ea0: 7420 6669 6c65 2e0a 2020 2020 2020 2020  t file..        
+00004eb0: 2020 2020 2020 2020 6675 7475 7265 203d          future =
+00004ec0: 2063 616c 6375 6c61 7465 5f70 6f6f 6c2e   calculate_pool.
+00004ed0: 7375 626d 6974 280a 2020 2020 2020 2020  submit(.        
+00004ee0: 2020 2020 2020 2020 2020 2020 5f61 7070              _app
+00004ef0: 6c79 5f67 656f 6f70 6572 6174 696f 6e2c  ly_geooperation,
+00004f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f10: 2020 2020 2069 6e70 7574 5f70 6174 683d       input_path=
+00004f20: 696e 7075 745f 7061 7468 2c0a 2020 2020  input_path,.    
+00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f40: 6f75 7470 7574 5f70 6174 683d 6f75 7470  output_path=outp
+00004f50: 7574 5f74 6d70 5f70 6172 7469 616c 5f70  ut_tmp_partial_p
+00004f60: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+00004f70: 2020 2020 2020 2020 206f 7065 7261 7469           operati
+00004f80: 6f6e 3d6f 7065 7261 7469 6f6e 2c0a 2020  on=operation,.  
+00004f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fa0: 2020 6f70 6572 6174 696f 6e5f 7061 7261    operation_para
+00004fb0: 6d73 3d6f 7065 7261 7469 6f6e 5f70 6172  ms=operation_par
+00004fc0: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
+00004fd0: 2020 2020 2020 2020 2069 6e70 7574 5f6c           input_l
+00004fe0: 6179 6572 3d69 6e70 7574 5f6c 6179 6572  ayer=input_layer
+00004ff0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005000: 2020 2020 2020 636f 6c75 6d6e 733d 636f        columns=co
+00005010: 6c75 6d6e 732c 0a20 2020 2020 2020 2020  lumns,.         
+00005020: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00005030: 745f 6c61 7965 723d 6f75 7470 7574 5f6c  t_layer=output_l
+00005040: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+00005050: 2020 2020 2020 2020 2020 726f 7773 3d72            rows=r
+00005060: 6f77 732c 0a20 2020 2020 2020 2020 2020  ows,.           
+00005070: 2020 2020 2020 2020 2065 7870 6c6f 6465           explode
+00005080: 636f 6c6c 6563 7469 6f6e 733d 6578 706c  collections=expl
+00005090: 6f64 6563 6f6c 6c65 6374 696f 6e73 2c0a  odecollections,.
+000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050b0: 2020 2020 6772 6964 7369 7a65 3d67 7269      gridsize=gri
+000050c0: 6473 697a 652c 0a20 2020 2020 2020 2020  dsize,.         
+000050d0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+000050e0: 3d66 6f72 6365 2c0a 2020 2020 2020 2020  =force,.        
+000050f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00005100: 2020 2020 2020 2020 2020 6675 7475 7265            future
+00005110: 5f74 6f5f 6261 7463 685f 6964 5b66 7574  _to_batch_id[fut
+00005120: 7572 655d 203d 2062 6174 6368 5f69 640a  ure] = batch_id.
+00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005140: 726f 775f 6f66 6673 6574 202b 3d20 7265  row_offset += re
+00005150: 616c 5f62 6174 6368 7369 7a65 0a0a 2020  al_batchsize..  
+00005160: 2020 2020 2020 2020 2020 2320 4c6f 6f70            # Loop
+00005170: 2074 696c 6c20 616c 6c20 7061 7261 6c6c   till all parall
+00005180: 656c 2070 726f 6365 7373 6573 2061 7265  el processes are
+00005190: 2072 6561 6479 2c20 6275 7420 7072 6f63   ready, but proc
+000051a0: 6573 7320 6561 6368 206f 6e65 0a20 2020  ess each one.   
+000051b0: 2020 2020 2020 2020 2023 2074 6861 7420           # that 
+000051c0: 6973 2072 6561 6479 2061 6c72 6561 6479  is ready already
+000051d0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+000051e0: 7274 5f74 696d 6520 3d20 6461 7465 7469  rt_time = dateti
+000051f0: 6d65 2e6e 6f77 2829 0a20 2020 2020 2020  me.now().       
+00005200: 2020 2020 205f 6765 6e65 7261 6c5f 7574       _general_ut
+00005210: 696c 2e72 6570 6f72 745f 7072 6f67 7265  il.report_progre
+00005220: 7373 280a 2020 2020 2020 2020 2020 2020  ss(.            
+00005230: 2020 2020 7374 6172 745f 7469 6d65 2c20      start_time, 
+00005240: 6e62 5f64 6f6e 652c 206e 625f 6261 7463  nb_done, nb_batc
+00005250: 6865 732c 206f 7065 7261 7469 6f6e 2e76  hes, operation.v
+00005260: 616c 7565 2c20 6e62 5f70 6172 616c 6c65  alue, nb_paralle
+00005270: 6c0a 2020 2020 2020 2020 2020 2020 290a  l.            ).
+00005280: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00005290: 6675 7475 7265 2069 6e20 6675 7475 7265  future in future
+000052a0: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
+000052b0: 7574 7572 655f 746f 5f62 6174 6368 5f69  uture_to_batch_i
+000052c0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+000052d0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000052e0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+000052f0: 7361 6765 203d 2066 7574 7572 652e 7265  sage = future.re
+00005300: 7375 6c74 2829 0a20 2020 2020 2020 2020  sult().         
+00005310: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00005320: 722e 6465 6275 6728 6d65 7373 6167 6529  r.debug(message)
+00005330: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005340: 2020 2020 2020 2320 4966 2074 6865 2063        # If the c
+00005350: 616c 6375 6c61 7465 2067 6176 6520 7265  alculate gave re
+00005360: 7375 6c74 732c 2063 6f70 7920 746f 206f  sults, copy to o
+00005370: 7574 7075 740a 2020 2020 2020 2020 2020  utput.          
+00005380: 2020 2020 2020 2020 2020 6261 7463 685f            batch_
+00005390: 6964 203d 2066 7574 7572 655f 746f 5f62  id = future_to_b
+000053a0: 6174 6368 5f69 645b 6675 7475 7265 5d0a  atch_id[future].
+000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053c0: 2020 2020 746d 705f 7061 7274 6961 6c5f      tmp_partial_
+000053d0: 6f75 7470 7574 5f70 6174 6820 3d20 6261  output_path = ba
+000053e0: 7463 6865 735b 6261 7463 685f 6964 5d5b  tches[batch_id][
+000053f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005400: 2020 2020 2020 2020 2022 746d 705f 7061           "tmp_pa
+00005410: 7274 6961 6c5f 6f75 7470 7574 5f70 6174  rtial_output_pat
+00005420: 6822 0a20 2020 2020 2020 2020 2020 2020  h".             
+00005430: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00005440: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005450: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005460: 2020 2020 2020 2020 2020 746d 705f 7061            tmp_pa
+00005470: 7274 6961 6c5f 6f75 7470 7574 5f70 6174  rtial_output_pat
+00005480: 682e 6578 6973 7473 2829 0a20 2020 2020  h.exists().     
+00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054a0: 2020 2061 6e64 2074 6d70 5f70 6172 7469     and tmp_parti
+000054b0: 616c 5f6f 7574 7075 745f 7061 7468 2e73  al_output_path.s
+000054c0: 7461 7428 292e 7374 5f73 697a 6520 3e20  tat().st_size > 
+000054d0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+000054e0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005500: 2023 2052 656d 6172 6b3a 2062 6563 6175   # Remark: becau
+00005510: 7365 2066 6f72 6365 5f6f 7574 7075 745f  se force_output_
+00005520: 6765 6f6d 6574 7279 7479 7065 2066 6f72  geometrytype for
+00005530: 2047 656f 4461 7461 4672 616d 650a 2020   GeoDataFrame.  
 00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
-00005560: 6f6d 6574 7279 7479 7065 3d66 6f72 6365  ometrytype=force
-00005570: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
-00005580: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
-00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055a0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 6766 6f2e 7265 6d6f 7665 2874 6d70 5f70  gfo.remove(tmp_p
-000055d0: 6172 7469 616c 5f6f 7574 7075 745f 7061  artial_output_pa
-000055e0: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
-000055f0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00005600: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
-00005610: 2020 2020 2020 2020 2020 2062 6174 6368             batch
-00005620: 5f69 6420 3d20 6675 7475 7265 5f74 6f5f  _id = future_to_
-00005630: 6261 7463 685f 6964 5b66 7574 7572 655d  batch_id[future]
-00005640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005650: 2020 2020 2023 2063 616c 6375 6c61 7465       # calculate
-00005660: 5f70 6f6f 6c2e 7368 7574 646f 776e 2829  _pool.shutdown()
-00005670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005680: 2020 2020 206c 6f67 6765 722e 6578 6365       logger.exce
-00005690: 7074 696f 6e28 6622 4572 726f 7220 6578  ption(f"Error ex
-000056a0: 6563 7574 696e 6720 7b62 6174 6368 6573  ecuting {batches
-000056b0: 5b62 6174 6368 5f69 645d 7d22 290a 0a20  [batch_id]}").. 
-000056c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000056d0: 204c 6f67 2074 6865 2070 726f 6772 6573   Log the progres
-000056e0: 7320 616e 6420 7072 6564 6963 7469 6f6e  s and prediction
-000056f0: 2073 7065 6564 0a20 2020 2020 2020 2020   speed.         
-00005700: 2020 2020 2020 206e 625f 646f 6e65 202b         nb_done +
-00005710: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00005720: 2020 2020 5f67 656e 6572 616c 5f75 7469      _general_uti
-00005730: 6c2e 7265 706f 7274 5f70 726f 6772 6573  l.report_progres
-00005740: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00005750: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
-00005760: 652c 206e 625f 646f 6e65 2c20 6e62 5f62  e, nb_done, nb_b
-00005770: 6174 6368 6573 2c20 6f70 6572 6174 696f  atches, operatio
-00005780: 6e2e 7661 6c75 652c 206e 625f 7061 7261  n.value, nb_para
-00005790: 6c6c 656c 0a20 2020 2020 2020 2020 2020  llel.           
-000057a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000057b0: 2320 526f 756e 6420 7570 2061 6e64 2063  # Round up and c
-000057c0: 6c65 616e 2075 700a 2020 2020 2020 2020  lean up.        
-000057d0: 2320 4e6f 7720 6372 6561 7465 2073 7061  # Now create spa
-000057e0: 7469 616c 2069 6e64 6578 2061 6e64 206d  tial index and m
-000057f0: 6f76 6520 746f 206f 7574 7075 7420 6c6f  ove to output lo
-00005800: 6361 7469 6f6e 0a20 2020 2020 2020 2069  cation.        i
-00005810: 6620 746d 705f 6f75 7470 7574 5f70 6174  f tmp_output_pat
-00005820: 682e 6578 6973 7473 2829 3a0a 2020 2020  h.exists():.    
-00005830: 2020 2020 2020 2020 6766 6f2e 6372 6561          gfo.crea
-00005840: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
-00005850: 2870 6174 683d 746d 705f 6f75 7470 7574  (path=tmp_output
-00005860: 5f70 6174 682c 206c 6179 6572 3d6f 7574  _path, layer=out
-00005870: 7075 745f 6c61 7965 7229 0a20 2020 2020  put_layer).     
-00005880: 2020 2020 2020 2067 666f 2e6d 6f76 6528         gfo.move(
-00005890: 746d 705f 6f75 7470 7574 5f70 6174 682c  tmp_output_path,
-000058a0: 206f 7574 7075 745f 7061 7468 290a 2020   output_path).  
-000058b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000058c0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-000058d0: 6562 7567 2866 2252 6573 756c 7420 6f66  ebug(f"Result of
-000058e0: 207b 6f70 6572 6174 696f 6e7d 2077 6173   {operation} was
-000058f0: 2065 6d70 7479 2122 290a 0a20 2020 2066   empty!")..    f
-00005900: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-00005910: 2320 436c 6561 6e20 746d 7020 6469 720a  # Clean tmp dir.
-00005920: 2020 2020 2020 2020 7368 7574 696c 2e72          shutil.r
-00005930: 6d74 7265 6528 7465 6d70 6469 7229 0a20  mtree(tempdir). 
-00005940: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00005950: 666f 2866 227b 6f70 6572 6174 696f 6e7d  fo(f"{operation}
-00005960: 2072 6561 6479 2c20 746f 6f6b 207b 6461   ready, took {da
-00005970: 7465 7469 6d65 2e6e 6f77 2829 2d73 7461  tetime.now()-sta
-00005980: 7274 5f74 696d 655f 676c 6f62 616c 7d21  rt_time_global}!
-00005990: 2229 0a0a 0a64 6566 205f 6170 706c 795f  ")...def _apply_
-000059a0: 6765 6f6f 7065 7261 7469 6f6e 280a 2020  geooperation(.  
-000059b0: 2020 696e 7075 745f 7061 7468 3a20 5061    input_path: Pa
-000059c0: 7468 2c0a 2020 2020 6f75 7470 7574 5f70  th,.    output_p
-000059d0: 6174 683a 2050 6174 682c 0a20 2020 206f  ath: Path,.    o
-000059e0: 7065 7261 7469 6f6e 3a20 4765 6f4f 7065  peration: GeoOpe
-000059f0: 7261 7469 6f6e 2c0a 2020 2020 6f70 6572  ration,.    oper
-00005a00: 6174 696f 6e5f 7061 7261 6d73 3a20 6469  ation_params: di
-00005a10: 6374 2c0a 2020 2020 696e 7075 745f 6c61  ct,.    input_la
-00005a20: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
-00005a30: 725d 203d 204e 6f6e 652c 0a20 2020 206f  r] = None,.    o
-00005a40: 7574 7075 745f 6c61 7965 723a 204f 7074  utput_layer: Opt
-00005a50: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00005a60: 652c 0a20 2020 2063 6f6c 756d 6e73 3a20  e,.    columns: 
-00005a70: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-00005a80: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-00005a90: 726f 7773 3d4e 6f6e 652c 0a20 2020 2065  rows=None,.    e
-00005aa0: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
-00005ab0: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
-00005ac0: 0a20 2020 2066 6f72 6365 3a20 626f 6f6c  .    force: bool
-00005ad0: 203d 2046 616c 7365 2c0a 2920 2d3e 2073   = False,.) -> s
-00005ae0: 7472 3a0a 2020 2020 2320 496e 6974 0a20  tr:.    # Init. 
-00005af0: 2020 2069 6620 6f75 7470 7574 5f70 6174     if output_pat
-00005b00: 682e 6578 6973 7473 2829 3a0a 2020 2020  h.exists():.    
-00005b10: 2020 2020 6966 2066 6f72 6365 2069 7320      if force is 
-00005b20: 4661 6c73 653a 0a20 2020 2020 2020 2020  False:.         
-00005b30: 2020 206d 6573 7361 6765 203d 2066 2253     message = f"S
-00005b40: 746f 7020 7b6f 7065 7261 7469 6f6e 7d3a  top {operation}:
-00005b50: 206f 7574 7075 7420 6578 6973 7473 2061   output exists a
-00005b60: 6c72 6561 6479 207b 6f75 7470 7574 5f70  lready {output_p
-00005b70: 6174 687d 220a 2020 2020 2020 2020 2020  ath}".          
-00005b80: 2020 7265 7475 726e 206d 6573 7361 6765    return message
-00005b90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00005ba0: 2020 2020 2020 2020 2020 2067 666f 2e72             gfo.r
-00005bb0: 656d 6f76 6528 6f75 7470 7574 5f70 6174  emove(output_pat
-00005bc0: 6829 0a0a 2020 2020 2320 4e6f 7720 676f  h)..    # Now go
-00005bd0: 210a 2020 2020 7374 6172 745f 7469 6d65  !.    start_time
-00005be0: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
-00005bf0: 290a 2020 2020 6461 7461 5f67 6466 203d  ).    data_gdf =
-00005c00: 2067 666f 2e72 6561 645f 6669 6c65 280a   gfo.read_file(.
-00005c10: 2020 2020 2020 2020 7061 7468 3d69 6e70          path=inp
-00005c20: 7574 5f70 6174 682c 206c 6179 6572 3d69  ut_path, layer=i
-00005c30: 6e70 7574 5f6c 6179 6572 2c20 636f 6c75  nput_layer, colu
-00005c40: 6d6e 733d 636f 6c75 6d6e 732c 2072 6f77  mns=columns, row
-00005c50: 733d 726f 7773 0a20 2020 2029 0a0a 2020  s=rows.    )..  
-00005c60: 2020 2320 5275 6e20 6f70 6572 6174 696f    # Run operatio
-00005c70: 6e73 0a20 2020 2069 6620 6f70 6572 6174  ns.    if operat
-00005c80: 696f 6e20 6973 2047 656f 4f70 6572 6174  ion is GeoOperat
-00005c90: 696f 6e2e 4255 4646 4552 3a0a 2020 2020  ion.BUFFER:.    
-00005ca0: 2020 2020 6461 7461 5f67 6466 2e67 656f      data_gdf.geo
-00005cb0: 6d65 7472 7920 3d20 6461 7461 5f67 6466  metry = data_gdf
-00005cc0: 2e67 656f 6d65 7472 792e 6275 6666 6572  .geometry.buffer
-00005cd0: 280a 2020 2020 2020 2020 2020 2020 6469  (.            di
-00005ce0: 7374 616e 6365 3d6f 7065 7261 7469 6f6e  stance=operation
-00005cf0: 5f70 6172 616d 735b 2264 6973 7461 6e63  _params["distanc
-00005d00: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
-00005d10: 2072 6573 6f6c 7574 696f 6e3d 6f70 6572   resolution=oper
-00005d20: 6174 696f 6e5f 7061 7261 6d73 5b22 7175  ation_params["qu
-00005d30: 6164 7261 6e74 7365 676d 656e 7473 225d  adrantsegments"]
-00005d40: 2c0a 2020 2020 2020 2020 2020 2020 6361  ,.            ca
-00005d50: 705f 7374 796c 653d 6f70 6572 6174 696f  p_style=operatio
-00005d60: 6e5f 7061 7261 6d73 5b22 656e 6463 6170  n_params["endcap
-00005d70: 5f73 7479 6c65 225d 2e76 616c 7565 2c0a  _style"].value,.
-00005d80: 2020 2020 2020 2020 2020 2020 6a6f 696e              join
-00005d90: 5f73 7479 6c65 3d6f 7065 7261 7469 6f6e  _style=operation
-00005da0: 5f70 6172 616d 735b 226a 6f69 6e5f 7374  _params["join_st
-00005db0: 796c 6522 5d2e 7661 6c75 652c 0a20 2020  yle"].value,.   
-00005dc0: 2020 2020 2020 2020 206d 6974 7265 5f6c           mitre_l
-00005dd0: 696d 6974 3d6f 7065 7261 7469 6f6e 5f70  imit=operation_p
-00005de0: 6172 616d 735b 226d 6974 7265 5f6c 696d  arams["mitre_lim
-00005df0: 6974 225d 2c0a 2020 2020 2020 2020 2020  it"],.          
-00005e00: 2020 7369 6e67 6c65 5f73 6964 6564 3d6f    single_sided=o
-00005e10: 7065 7261 7469 6f6e 5f70 6172 616d 735b  peration_params[
-00005e20: 2273 696e 676c 655f 7369 6465 6422 5d2c  "single_sided"],
-00005e30: 0a20 2020 2020 2020 2029 0a20 2020 2065  .        ).    e
-00005e40: 6c69 6620 6f70 6572 6174 696f 6e20 6973  lif operation is
-00005e50: 2047 656f 4f70 6572 6174 696f 6e2e 434f   GeoOperation.CO
-00005e60: 4e56 4558 4855 4c4c 3a0a 2020 2020 2020  NVEXHULL:.      
-00005e70: 2020 6461 7461 5f67 6466 2e67 656f 6d65    data_gdf.geome
-00005e80: 7472 7920 3d20 6461 7461 5f67 6466 2e67  try = data_gdf.g
-00005e90: 656f 6d65 7472 792e 636f 6e76 6578 5f68  eometry.convex_h
-00005ea0: 756c 6c0a 2020 2020 656c 6966 206f 7065  ull.    elif ope
-00005eb0: 7261 7469 6f6e 2069 7320 4765 6f4f 7065  ration is GeoOpe
-00005ec0: 7261 7469 6f6e 2e53 494d 504c 4946 593a  ration.SIMPLIFY:
-00005ed0: 0a20 2020 2020 2020 2064 6174 615f 6764  .        data_gd
-00005ee0: 662e 6765 6f6d 6574 7279 203d 2067 656f  f.geometry = geo
-00005ef0: 7365 7269 6573 5f75 7469 6c2e 7369 6d70  series_util.simp
-00005f00: 6c69 6679 5f65 7874 280a 2020 2020 2020  lify_ext(.      
-00005f10: 2020 2020 2020 6461 7461 5f67 6466 2e67        data_gdf.g
-00005f20: 656f 6d65 7472 792c 0a20 2020 2020 2020  eometry,.       
-00005f30: 2020 2020 2061 6c67 6f72 6974 686d 3d6f       algorithm=o
-00005f40: 7065 7261 7469 6f6e 5f70 6172 616d 735b  peration_params[
-00005f50: 2261 6c67 6f72 6974 686d 225d 2c0a 2020  "algorithm"],.  
-00005f60: 2020 2020 2020 2020 2020 746f 6c65 7261            tolera
-00005f70: 6e63 653d 6f70 6572 6174 696f 6e5f 7061  nce=operation_pa
-00005f80: 7261 6d73 5b22 746f 6c65 7261 6e63 6522  rams["tolerance"
-00005f90: 5d2c 0a20 2020 2020 2020 2020 2020 206c  ],.            l
-00005fa0: 6f6f 6b61 6865 6164 3d6f 7065 7261 7469  ookahead=operati
-00005fb0: 6f6e 5f70 6172 616d 735b 2273 7465 7022  on_params["step"
-00005fc0: 5d2c 0a20 2020 2020 2020 2029 0a20 2020  ],.        ).   
-00005fd0: 2065 6c69 6620 6f70 6572 6174 696f 6e20   elif operation 
-00005fe0: 6973 2047 656f 4f70 6572 6174 696f 6e2e  is GeoOperation.
-00005ff0: 4150 504c 593a 0a20 2020 2020 2020 2066  APPLY:.        f
-00006000: 756e 6320 3d20 7069 636b 6c65 2e6c 6f61  unc = pickle.loa
-00006010: 6473 286f 7065 7261 7469 6f6e 5f70 6172  ds(operation_par
-00006020: 616d 735b 2270 6963 6b6c 6564 5f66 756e  ams["pickled_fun
-00006030: 6322 5d29 0a20 2020 2020 2020 2069 6620  c"]).        if 
-00006040: 6f70 6572 6174 696f 6e5f 7061 7261 6d73  operation_params
-00006050: 5b22 6f6e 6c79 5f67 656f 6d5f 696e 7075  ["only_geom_inpu
-00006060: 7422 5d20 6973 2054 7275 653a 0a20 2020  t"] is True:.   
-00006070: 2020 2020 2020 2020 2064 6174 615f 6764           data_gd
-00006080: 662e 6765 6f6d 6574 7279 203d 2064 6174  f.geometry = dat
-00006090: 615f 6764 662e 6765 6f6d 6574 7279 2e61  a_gdf.geometry.a
-000060a0: 7070 6c79 2866 756e 6329 0a20 2020 2020  pply(func).     
-000060b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000060c0: 2020 2020 2064 6174 615f 6764 662e 6765       data_gdf.ge
-000060d0: 6f6d 6574 7279 203d 2064 6174 615f 6764  ometry = data_gd
-000060e0: 662e 6170 706c 7928 6675 6e63 2c20 6178  f.apply(func, ax
-000060f0: 6973 3d31 290a 2020 2020 656c 7365 3a0a  is=1).    else:.
-00006100: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00006110: 6c75 6545 7272 6f72 2866 226f 7065 7261  lueError(f"opera
-00006120: 7469 6f6e 206e 6f74 2073 7570 706f 7274  tion not support
-00006130: 6564 3a20 7b6f 7065 7261 7469 6f6e 7d22  ed: {operation}"
-00006140: 290a 0a20 2020 2023 2052 656d 6f76 6520  )..    # Remove 
-00006150: 726f 7773 2077 6865 7265 2067 656f 6d20  rows where geom 
-00006160: 6973 2065 6d70 7479 0a20 2020 2064 6174  is empty.    dat
-00006170: 615f 6764 6620 3d20 6461 7461 5f67 6466  a_gdf = data_gdf
-00006180: 5b7e 6461 7461 5f67 6466 2e67 656f 6d65  [~data_gdf.geome
-00006190: 7472 792e 6973 5f65 6d70 7479 5d0a 2020  try.is_empty].  
-000061a0: 2020 6461 7461 5f67 6466 203d 2064 6174    data_gdf = dat
-000061b0: 615f 6764 665b 7e64 6174 615f 6764 662e  a_gdf[~data_gdf.
-000061c0: 6765 6f6d 6574 7279 2e69 736e 6128 295d  geometry.isna()]
-000061d0: 0a0a 2020 2020 2320 4966 2074 6865 7265  ..    # If there
-000061e0: 2069 7320 616e 2066 6964 2063 6f6c 756d   is an fid colum
-000061f0: 6e20 696e 2074 6865 2064 6174 6173 6574  n in the dataset
-00006200: 2c20 7265 6e61 6d65 2069 742c 2062 6563  , rename it, bec
-00006210: 6175 7365 2074 6865 2066 6964 2063 6f6c  ause the fid col
-00006220: 756d 6e20 6973 2061 0a20 2020 2023 2022  umn is a.    # "
-00006230: 7370 6563 6961 6c20 6361 7365 2220 696e  special case" in
-00006240: 2067 6461 6c20 7468 6174 2073 686f 756c   gdal that shoul
-00006250: 6420 6e6f 7420 6265 2077 7269 7474 656e  d not be written
-00006260: 2e0a 2020 2020 636f 6c75 6d6e 735f 6c6f  ..    columns_lo
-00006270: 7765 725f 6c6f 6f6b 7570 203d 207b 636f  wer_lookup = {co
-00006280: 6c75 6d6e 2e6c 6f77 6572 2829 3a20 636f  lumn.lower(): co
-00006290: 6c75 6d6e 2066 6f72 2063 6f6c 756d 6e20  lumn for column 
-000062a0: 696e 2064 6174 615f 6764 662e 636f 6c75  in data_gdf.colu
-000062b0: 6d6e 737d 0a20 2020 2069 6620 2266 6964  mns}.    if "fid
-000062c0: 2220 696e 2063 6f6c 756d 6e73 5f6c 6f77  " in columns_low
-000062d0: 6572 5f6c 6f6f 6b75 703a 0a20 2020 2020  er_lookup:.     
-000062e0: 2020 2066 6964 5f63 6f6c 756d 6e20 3d20     fid_column = 
-000062f0: 636f 6c75 6d6e 735f 6c6f 7765 725f 6c6f  columns_lower_lo
-00006300: 6f6b 7570 5b22 6669 6422 5d0a 2020 2020  okup["fid"].    
-00006310: 2020 2020 666f 7220 6669 645f 6e75 6d62      for fid_numb
-00006320: 6572 2069 6e20 7261 6e67 6528 312c 2031  er in range(1, 1
-00006330: 3030 293a 0a20 2020 2020 2020 2020 2020  00):.           
-00006340: 206e 6577 5f6e 616d 6520 3d20 6622 7b66   new_name = f"{f
-00006350: 6964 5f63 6f6c 756d 6e7d 5f7b 6669 645f  id_column}_{fid_
-00006360: 6e75 6d62 6572 7d22 0a20 2020 2020 2020  number}".       
-00006370: 2020 2020 2069 6620 6e65 775f 6e61 6d65       if new_name
-00006380: 206e 6f74 2069 6e20 636f 6c75 6d6e 735f   not in columns_
-00006390: 6c6f 7765 725f 6c6f 6f6b 7570 3a0a 2020  lower_lookup:.  
-000063a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-000063b0: 7461 5f67 6466 203d 2064 6174 615f 6764  ta_gdf = data_gd
-000063c0: 662e 7265 6e61 6d65 280a 2020 2020 2020  f.rename(.      
-000063d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000063e0: 6c75 6d6e 733d 7b66 6964 5f63 6f6c 756d  lumns={fid_colum
-000063f0: 6e3a 206e 6577 5f6e 616d 657d 2c20 636f  n: new_name}, co
-00006400: 7079 3d46 616c 7365 2020 2320 7479 7065  py=False  # type
-00006410: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-00006420: 2020 2020 2020 2020 2029 0a20 2020 2069           ).    i
-00006430: 6620 6578 706c 6f64 6563 6f6c 6c65 6374  f explodecollect
-00006440: 696f 6e73 3a0a 2020 2020 2020 2020 6461  ions:.        da
-00006450: 7461 5f67 6466 203d 2064 6174 615f 6764  ta_gdf = data_gd
-00006460: 662e 6578 706c 6f64 6528 6967 6e6f 7265  f.explode(ignore
-00006470: 5f69 6e64 6578 3d54 7275 6529 2020 2320  _index=True)  # 
-00006480: 7479 7065 3a20 6967 6e6f 7265 0a0a 2020  type: ignore..  
-00006490: 2020 2320 4966 2074 6865 2072 6573 756c    # If the resul
-000064a0: 7420 6973 2065 6d70 7479 2c20 616e 6420  t is empty, and 
-000064b0: 6e6f 206f 7574 7075 7420 6765 6f6d 6574  no output geomet
-000064c0: 7279 7479 7065 2073 7065 6369 6669 6564  rytype specified
-000064d0: 2c20 7573 6520 696e 7075 740a 2020 2020  , use input.    
-000064e0: 2320 6765 6f6d 6574 7279 7479 7065 0a20  # geometrytype. 
-000064f0: 2020 2066 6f72 6365 5f6f 7574 7075 745f     force_output_
-00006500: 6765 6f6d 6574 7279 7479 7065 203d 204e  geometrytype = N
-00006510: 6f6e 650a 2020 2020 6966 206c 656e 2864  one.    if len(d
-00006520: 6174 615f 6764 6629 203d 3d20 303a 0a20  ata_gdf) == 0:. 
-00006530: 2020 2020 2020 2069 6e70 7574 5f6c 6179         input_lay
-00006540: 6572 696e 666f 203d 2067 666f 2e67 6574  erinfo = gfo.get
-00006550: 5f6c 6179 6572 696e 666f 2869 6e70 7574  _layerinfo(input
-00006560: 5f70 6174 682c 2069 6e70 7574 5f6c 6179  _path, input_lay
-00006570: 6572 290a 2020 2020 2020 2020 666f 7263  er).        forc
-00006580: 655f 6f75 7470 7574 5f67 656f 6d65 7472  e_output_geometr
-00006590: 7974 7970 6520 3d20 696e 7075 745f 6c61  ytype = input_la
-000065a0: 7965 7269 6e66 6f2e 6765 6f6d 6574 7279  yerinfo.geometry
-000065b0: 7479 7065 2e74 6f5f 6d75 6c74 6974 7970  type.to_multityp
-000065c0: 652e 6e61 6d65 0a0a 2020 2020 2320 6173  e.name..    # as
-000065d0: 7365 7274 2074 6f20 6576 6164 6520 7079  sert to evade py
-000065e0: 4c61 6e63 6520 7761 726e 696e 670a 2020  Lance warning.  
-000065f0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00006600: 6e63 6528 6461 7461 5f67 6466 2c20 6770  nce(data_gdf, gp
-00006610: 642e 4765 6f44 6174 6146 7261 6d65 290a  d.GeoDataFrame).
-00006620: 2020 2020 2320 5573 6520 666f 7263 655f      # Use force_
-00006630: 6d75 6c74 6974 7970 652c 2074 6f20 6576  multitype, to ev
-00006640: 6164 6520 7761 726e 696e 6773 2077 6865  ade warnings whe
-00006650: 6e20 736f 6d65 2062 6174 6368 6573 2063  n some batches c
-00006660: 6f6e 7461 696e 0a20 2020 2023 2073 696e  ontain.    # sin
-00006670: 676c 6574 7970 6520 616e 6420 736f 6d65  gletype and some
-00006680: 2063 6f6e 7461 696e 206d 756c 7469 7479   contain multity
-00006690: 7065 2067 656f 6d65 7472 6965 730a 2020  pe geometries.  
-000066a0: 2020 6766 6f2e 746f 5f66 696c 6528 0a20    gfo.to_file(. 
-000066b0: 2020 2020 2020 2067 6466 3d64 6174 615f         gdf=data_
-000066c0: 6764 662c 0a20 2020 2020 2020 2070 6174  gdf,.        pat
-000066d0: 683d 6f75 7470 7574 5f70 6174 682c 0a20  h=output_path,. 
-000066e0: 2020 2020 2020 206c 6179 6572 3d6f 7574         layer=out
-000066f0: 7075 745f 6c61 7965 722c 0a20 2020 2020  put_layer,.     
-00006700: 2020 2069 6e64 6578 3d46 616c 7365 2c0a     index=False,.
-00006710: 2020 2020 2020 2020 666f 7263 655f 6f75          force_ou
-00006720: 7470 7574 5f67 656f 6d65 7472 7974 7970  tput_geometrytyp
-00006730: 653d 666f 7263 655f 6f75 7470 7574 5f67  e=force_output_g
-00006740: 656f 6d65 7472 7974 7970 652c 0a20 2020  eometrytype,.   
-00006750: 2020 2020 2066 6f72 6365 5f6d 756c 7469       force_multi
-00006760: 7479 7065 3d54 7275 652c 0a20 2020 2020  type=True,.     
-00006770: 2020 2063 7265 6174 655f 7370 6174 6961     create_spatia
-00006780: 6c5f 696e 6465 783d 4661 6c73 652c 0a20  l_index=False,. 
-00006790: 2020 2029 0a0a 2020 2020 6d65 7373 6167     )..    messag
-000067a0: 6520 3d20 6622 546f 6f6b 207b 6461 7465  e = f"Took {date
-000067b0: 7469 6d65 2e6e 6f77 2829 2d73 7461 7274  time.now()-start
-000067c0: 5f74 696d 657d 2066 6f72 207b 6c65 6e28  _time} for {len(
-000067d0: 6461 7461 5f67 6466 297d 2072 6f77 7320  data_gdf)} rows 
-000067e0: 287b 726f 7773 7d29 2122 0a20 2020 2072  ({rows})!".    r
-000067f0: 6574 7572 6e20 6d65 7373 6167 650a 0a0a  eturn message...
-00006800: 6465 6620 6469 7373 6f6c 7665 280a 2020  def dissolve(.  
-00006810: 2020 696e 7075 745f 7061 7468 3a20 5061    input_path: Pa
-00006820: 7468 2c0a 2020 2020 6f75 7470 7574 5f70  th,.    output_p
-00006830: 6174 683a 2050 6174 682c 0a20 2020 2067  ath: Path,.    g
-00006840: 726f 7570 6279 5f63 6f6c 756d 6e73 3a20  roupby_columns: 
-00006850: 4f70 7469 6f6e 616c 5b49 7465 7261 626c  Optional[Iterabl
-00006860: 655b 7374 725d 5d20 3d20 4e6f 6e65 2c0a  e[str]] = None,.
-00006870: 2020 2020 6167 675f 636f 6c75 6d6e 733a      agg_columns:
-00006880: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
-00006890: 3d20 4e6f 6e65 2c0a 2020 2020 6578 706c  = None,.    expl
-000068a0: 6f64 6563 6f6c 6c65 6374 696f 6e73 3a20  odecollections: 
-000068b0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-000068c0: 2074 696c 6573 5f70 6174 683a 204f 7074   tiles_path: Opt
-000068d0: 696f 6e61 6c5b 5061 7468 5d20 3d20 4e6f  ional[Path] = No
-000068e0: 6e65 2c0a 2020 2020 6e62 5f73 7175 6172  ne,.    nb_squar
-000068f0: 6973 685f 7469 6c65 733a 2069 6e74 203d  ish_tiles: int =
-00006900: 2031 2c0a 2020 2020 696e 7075 745f 6c61   1,.    input_la
-00006910: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
-00006920: 725d 203d 204e 6f6e 652c 0a20 2020 206f  r] = None,.    o
-00006930: 7574 7075 745f 6c61 7965 723a 204f 7074  utput_layer: Opt
-00006940: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00006950: 652c 0a20 2020 206e 625f 7061 7261 6c6c  e,.    nb_parall
-00006960: 656c 3a20 696e 7420 3d20 2d31 2c0a 2020  el: int = -1,.  
-00006970: 2020 6261 7463 6873 697a 653a 2069 6e74    batchsize: int
-00006980: 203d 202d 312c 0a20 2020 2066 6f72 6365   = -1,.    force
-00006990: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-000069a0: 2920 2d3e 2064 6963 743a 0a20 2020 2022  ) -> dict:.    "
-000069b0: 2222 0a20 2020 2046 756e 6374 696f 6e20  "".    Function 
-000069c0: 7468 6174 2061 7070 6c69 6573 2061 2064  that applies a d
-000069d0: 6973 736f 6c76 652e 0a0a 2020 2020 4d6f  issolve...    Mo
-000069e0: 7265 2064 6574 6169 6c65 6420 646f 6375  re detailed docu
-000069f0: 6d65 6e74 6174 696f 6e20 696e 206d 6f64  mentation in mod
-00006a00: 756c 6520 6765 6f6f 7073 210a 2020 2020  ule geoops!.    
-00006a10: 2222 220a 0a20 2020 2023 2049 6e69 7420  """..    # Init 
-00006a20: 616e 6420 7661 6c69 6461 7465 2069 6e70  and validate inp
-00006a30: 7574 2070 6172 616d 6574 6572 730a 2020  ut parameters.  
-00006a40: 2020 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    # ------------
-00006a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006a60: 2d2d 2d2d 2d2d 0a20 2020 2073 7461 7274  ------.    start
-00006a70: 5f74 696d 6520 3d20 6461 7465 7469 6d65  _time = datetime
-00006a80: 2e6e 6f77 2829 0a20 2020 206f 7065 7261  .now().    opera
-00006a90: 7469 6f6e 203d 2022 6469 7373 6f6c 7665  tion = "dissolve
-00006aa0: 220a 2020 2020 7265 7375 6c74 5f69 6e66  ".    result_inf
-00006ab0: 6f20 3d20 7b7d 0a0a 2020 2020 2320 4368  o = {}..    # Ch
-00006ac0: 6563 6b20 696e 7075 7420 7061 7261 6d65  eck input parame
-00006ad0: 7465 7273 0a20 2020 2069 6620 6772 6f75  ters.    if grou
-00006ae0: 7062 795f 636f 6c75 6d6e 7320 6973 206e  pby_columns is n
-00006af0: 6f74 204e 6f6e 6520 616e 6420 6c65 6e28  ot None and len(
-00006b00: 6c69 7374 2867 726f 7570 6279 5f63 6f6c  list(groupby_col
-00006b10: 756d 6e73 2929 203d 3d20 303a 0a20 2020  umns)) == 0:.   
-00006b20: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00006b30: 4572 726f 7228 2267 726f 7570 6279 5f63  Error("groupby_c
-00006b40: 6f6c 756d 6e73 3d5b 5d20 6973 206e 6f74  olumns=[] is not
-00006b50: 2073 7570 706f 7274 6564 2e20 5573 6520   supported. Use 
-00006b60: 4e6f 6e65 2e22 290a 2020 2020 6966 206e  None.").    if n
-00006b70: 6f74 2069 6e70 7574 5f70 6174 682e 6578  ot input_path.ex
-00006b80: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
-00006b90: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00006ba0: 2866 2269 6e70 7574 5f70 6174 6820 646f  (f"input_path do
-00006bb0: 6573 6e27 7420 6578 6973 743a 207b 696e  esn't exist: {in
-00006bc0: 7075 745f 7061 7468 7d22 290a 2020 2020  put_path}").    
-00006bd0: 6966 2069 6e70 7574 5f70 6174 6820 3d3d  if input_path ==
-00006be0: 206f 7574 7075 745f 7061 7468 3a0a 2020   output_path:.  
-00006bf0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00006c00: 6545 7272 6f72 2822 6f75 7470 7574 5f70  eError("output_p
-00006c10: 6174 6820 6d75 7374 206e 6f74 2065 7175  ath must not equ
-00006c20: 616c 2069 6e70 7574 5f70 6174 6822 290a  al input_path").
-00006c30: 0a20 2020 2069 6e70 7574 5f6c 6179 6572  .    input_layer
-00006c40: 696e 666f 203d 2067 666f 2e67 6574 5f6c  info = gfo.get_l
-00006c50: 6179 6572 696e 666f 2869 6e70 7574 5f70  ayerinfo(input_p
-00006c60: 6174 682c 2069 6e70 7574 5f6c 6179 6572  ath, input_layer
-00006c70: 290a 2020 2020 6966 2069 6e70 7574 5f6c  ).    if input_l
-00006c80: 6179 6572 696e 666f 2e67 656f 6d65 7472  ayerinfo.geometr
-00006c90: 7974 7970 652e 746f 5f70 7269 6d69 7469  ytype.to_primiti
-00006ca0: 7665 7479 7065 2069 6e20 5b0a 2020 2020  vetype in [.    
-00006cb0: 2020 2020 5072 696d 6974 6976 6554 7970      PrimitiveTyp
-00006cc0: 652e 504f 494e 542c 0a20 2020 2020 2020  e.POINT,.       
-00006cd0: 2050 7269 6d69 7469 7665 5479 7065 2e4c   PrimitiveType.L
-00006ce0: 494e 4553 5452 494e 472c 0a20 2020 205d  INESTRING,.    ]
-00006cf0: 3a0a 2020 2020 2020 2020 6966 2074 696c  :.        if til
-00006d00: 6573 5f70 6174 6820 6973 206e 6f74 204e  es_path is not N
-00006d10: 6f6e 6520 6f72 206e 625f 7371 7561 7269  one or nb_squari
-00006d20: 7368 5f74 696c 6573 203e 2031 3a0a 2020  sh_tiles > 1:.  
-00006d30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00006d40: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00006d50: 2020 2020 2020 2020 2020 2020 6622 4469              f"Di
-00006d60: 7373 6f6c 7665 2074 6f20 7469 6c65 7320  ssolve to tiles 
-00006d70: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-00006d80: 2066 6f72 207b 696e 7075 745f 6c61 7965   for {input_laye
-00006d90: 7269 6e66 6f2e 6765 6f6d 6574 7279 7479  rinfo.geometryty
-00006da0: 7065 7d22 0a20 2020 2020 2020 2020 2020  pe}".           
-00006db0: 2020 2020 2022 2c20 736f 2074 696c 6573       ", so tiles
-00006dc0: 5f70 6174 6820 7368 6f75 6c64 2062 6520  _path should be 
-00006dd0: 4e6f 6e65 2061 6e64 206e 625f 7371 7561  None and nb_squa
-00006de0: 7269 7368 5f74 696c 6573 2073 686f 756c  rish_tiles shoul
-00006df0: 6420 6265 2031 2922 0a20 2020 2020 2020  d be 1)".       
-00006e00: 2020 2020 2029 0a0a 2020 2020 2320 4368       )..    # Ch
-00006e10: 6563 6b20 636f 6c75 6d6e 7320 696e 2067  eck columns in g
-00006e20: 726f 7570 6279 5f63 6f6c 756d 6e73 0a20  roupby_columns. 
-00006e30: 2020 2069 6620 6772 6f75 7062 795f 636f     if groupby_co
-00006e40: 6c75 6d6e 7320 6973 206e 6f74 204e 6f6e  lumns is not Non
-00006e50: 653a 0a20 2020 2020 2020 2063 6f6c 756d  e:.        colum
-00006e60: 6e73 5f69 6e5f 6c61 7965 725f 7570 7065  ns_in_layer_uppe
-00006e70: 7220 3d20 5b0a 2020 2020 2020 2020 2020  r = [.          
-00006e80: 2020 636f 6c75 6d6e 2e75 7070 6572 2829    column.upper()
-00006e90: 2066 6f72 2063 6f6c 756d 6e20 696e 206c   for column in l
-00006ea0: 6973 7428 696e 7075 745f 6c61 7965 7269  ist(input_layeri
-00006eb0: 6e66 6f2e 636f 6c75 6d6e 7329 202b 205b  nfo.columns) + [
-00006ec0: 2266 6964 225d 0a20 2020 2020 2020 205d  "fid"].        ]
-00006ed0: 0a20 2020 2020 2020 2066 6f72 2063 6f6c  .        for col
-00006ee0: 756d 6e20 696e 2067 726f 7570 6279 5f63  umn in groupby_c
-00006ef0: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
-00006f00: 2020 2020 6966 2063 6f6c 756d 6e2e 7570      if column.up
-00006f10: 7065 7228 2920 6e6f 7420 696e 2063 6f6c  per() not in col
-00006f20: 756d 6e73 5f69 6e5f 6c61 7965 725f 7570  umns_in_layer_up
-00006f30: 7065 723a 0a20 2020 2020 2020 2020 2020  per:.           
-00006f40: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00006f50: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00006f60: 2020 2020 2020 2020 2020 2066 2263 6f6c             f"col
-00006f70: 756d 6e20 696e 2067 726f 7570 6279 5f63  umn in groupby_c
-00006f80: 6f6c 756d 6e73 206e 6f74 2061 7661 696c  olumns not avail
-00006f90: 6162 6c65 2069 6e20 6c61 7965 723a 207b  able in layer: {
-00006fa0: 636f 6c75 6d6e 7d22 0a20 2020 2020 2020  column}".       
-00006fb0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00006fc0: 2320 4368 6563 6b20 6167 675f 636f 6c75  # Check agg_colu
-00006fd0: 6d6e 7320 7061 7261 6d0a 2020 2020 6966  mns param.    if
-00006fe0: 2061 6767 5f63 6f6c 756d 6e73 2069 7320   agg_columns is 
-00006ff0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00007000: 2020 2320 5661 6c69 6461 7465 2074 6865    # Validate the
-00007010: 2064 6963 7420 7374 7275 6374 7572 652c   dict structure,
-00007020: 2073 6f20 7765 2063 616e 2061 7373 756d   so we can assum
-00007030: 6520 6576 6572 7974 6869 6e67 2069 7320  e everything is 
-00007040: 4f4b 2066 7572 7468 6572 206f 6e0a 2020  OK further on.  
-00007050: 2020 2020 2020 5f70 6172 616d 6574 6572        _parameter
-00007060: 5f68 656c 7065 722e 7661 6c69 6461 7465  _helper.validate
-00007070: 5f61 6767 5f63 6f6c 756d 6e73 2861 6767  _agg_columns(agg
-00007080: 5f63 6f6c 756d 6e73 290a 0a20 2020 2020  _columns)..     
-00007090: 2020 2023 2046 6972 7374 2074 616b 6520     # First take 
-000070a0: 6120 6465 6570 2063 6f70 792c 2061 7320  a deep copy, as 
-000070b0: 7661 6c75 6573 2063 616e 2062 6520 6368  values can be ch
-000070c0: 616e 6765 6420 6675 7274 6865 7220 6f6e  anged further on
-000070d0: 2074 6f20 7472 6561 7420 636f 6c75 6d6e   to treat column
-000070e0: 730a 2020 2020 2020 2020 2320 6361 7365  s.        # case
-000070f0: 2069 6e73 656e 7369 7469 7665 0a20 2020   insensitive.   
-00007100: 2020 2020 2061 6767 5f63 6f6c 756d 6e73       agg_columns
-00007110: 203d 206a 736f 6e2e 6c6f 6164 7328 6a73   = json.loads(js
-00007120: 6f6e 2e64 756d 7073 2861 6767 5f63 6f6c  on.dumps(agg_col
-00007130: 756d 6e73 2929 0a20 2020 2020 2020 2061  umns)).        a
-00007140: 7373 6572 7420 6167 675f 636f 6c75 6d6e  ssert agg_column
-00007150: 7320 6973 206e 6f74 204e 6f6e 650a 2020  s is not None.  
-00007160: 2020 2020 2020 6966 2022 6a73 6f6e 2220        if "json" 
-00007170: 696e 2061 6767 5f63 6f6c 756d 6e73 3a0a  in agg_columns:.
-00007180: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00007190: 6767 5f63 6f6c 756d 6e73 5b22 6a73 6f6e  gg_columns["json
-000071a0: 225d 2069 7320 4e6f 6e65 3a0a 2020 2020  "] is None:.    
-000071b0: 2020 2020 2020 2020 2020 2020 6167 675f              agg_
-000071c0: 636f 6c75 6d6e 735b 226a 736f 6e22 5d20  columns["json"] 
-000071d0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-000071e0: 2020 2020 2020 2020 636f 6c20 666f 7220          col for 
-000071f0: 636f 6c20 696e 2069 6e70 7574 5f6c 6179  col in input_lay
-00007200: 6572 696e 666f 2e63 6f6c 756d 6e73 2069  erinfo.columns i
-00007210: 6620 636f 6c2e 7570 7065 7228 2920 213d  f col.upper() !=
-00007220: 2022 494e 4445 5822 0a20 2020 2020 2020   "INDEX".       
-00007230: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00007240: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007250: 2020 2020 2020 2020 2020 2020 2023 2041               # A
-00007260: 6c69 676e 2063 6173 696e 6720 6f66 2063  lign casing of c
-00007270: 6f6c 756d 6e20 6e61 6d65 7320 746f 2064  olumn names to d
-00007280: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-00007290: 2020 2020 6167 675f 636f 6c75 6d6e 735b      agg_columns[
-000072a0: 226a 736f 6e22 5d20 3d20 5f67 656e 6572  "json"] = _gener
-000072b0: 616c 5f75 7469 6c2e 616c 6967 6e5f 6361  al_util.align_ca
-000072c0: 7369 6e67 5f6c 6973 7428 0a20 2020 2020  sing_list(.     
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000072e0: 6767 5f63 6f6c 756d 6e73 5b22 6a73 6f6e  gg_columns["json
-000072f0: 225d 2c20 6c69 7374 2869 6e70 7574 5f6c  "], list(input_l
-00007300: 6179 6572 696e 666f 2e63 6f6c 756d 6e73  ayerinfo.columns
-00007310: 2920 2b20 5b22 6669 6422 5d0a 2020 2020  ) + ["fid"].    
-00007320: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007330: 2020 2020 2020 656c 6966 2022 636f 6c75        elif "colu
-00007340: 6d6e 7322 2069 6e20 6167 675f 636f 6c75  mns" in agg_colu
-00007350: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
-00007360: 2023 204c 6f6f 7020 7468 726f 7567 6820   # Loop through 
-00007370: 616c 6c20 726f 7773 0a20 2020 2020 2020  all rows.       
-00007380: 2020 2020 2066 6f72 2061 6767 5f63 6f6c       for agg_col
-00007390: 756d 6e20 696e 2061 6767 5f63 6f6c 756d  umn in agg_colum
-000073a0: 6e73 5b22 636f 6c75 6d6e 7322 5d3a 0a20  ns["columns"]:. 
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000073c0: 2043 6865 636b 2069 6620 636f 6c75 6d6e   Check if column
-000073d0: 2065 7869 7374 7320 2b20 7365 7420 6361   exists + set ca
-000073e0: 7369 6e67 2073 616d 6520 6173 2069 6e20  sing same as in 
-000073f0: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
-00007400: 2020 2020 2061 6767 5f63 6f6c 756d 6e5b       agg_column[
-00007410: 2263 6f6c 756d 6e22 5d20 3d20 5f67 656e  "column"] = _gen
-00007420: 6572 616c 5f75 7469 6c2e 616c 6967 6e5f  eral_util.align_
-00007430: 6361 7369 6e67 280a 2020 2020 2020 2020  casing(.        
-00007440: 2020 2020 2020 2020 2020 2020 6167 675f              agg_
-00007450: 636f 6c75 6d6e 5b22 636f 6c75 6d6e 225d  column["column"]
-00007460: 2c20 6c69 7374 2869 6e70 7574 5f6c 6179  , list(input_lay
-00007470: 6572 696e 666f 2e63 6f6c 756d 6e73 2920  erinfo.columns) 
-00007480: 2b20 5b22 6669 6422 5d0a 2020 2020 2020  + ["fid"].      
-00007490: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000074a0: 2023 204e 6f77 2069 6e70 7574 2070 6172   # Now input par
-000074b0: 616d 6574 6572 7320 6172 6520 6368 6563  ameters are chec
-000074c0: 6b65 642c 2063 6865 636b 2069 6620 7765  ked, check if we
-000074d0: 206e 6565 6420 746f 2063 616c 6361 6c61   need to calcala
-000074e0: 7465 2061 6e79 7761 790a 2020 2020 6966  te anyway.    if
-000074f0: 206f 7574 7075 745f 7061 7468 2e65 7869   output_path.exi
-00007500: 7374 7328 293a 0a20 2020 2020 2020 2069  sts():.        i
-00007510: 6620 666f 7263 6520 6973 2046 616c 7365  f force is False
-00007520: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00007530: 7375 6c74 5f69 6e66 6f5b 0a20 2020 2020  sult_info[.     
-00007540: 2020 2020 2020 2020 2020 2022 6d65 7373             "mess
-00007550: 6167 6522 0a20 2020 2020 2020 2020 2020  age".           
-00007560: 205d 203d 2066 226f 7574 7075 7420 6578   ] = f"output ex
-00007570: 6973 7473 2061 6c72 6561 6479 207b 6f75  ists already {ou
-00007580: 7470 7574 5f70 6174 687d 2061 6e64 2066  tput_path} and f
-00007590: 6f72 6365 2069 7320 6661 6c73 6522 0a20  orce is false". 
-000075a0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000075b0: 722e 696e 666f 2872 6573 756c 745f 696e  r.info(result_in
-000075c0: 666f 5b22 6d65 7373 6167 6522 5d29 0a20  fo["message"]). 
-000075d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000075e0: 6e20 7265 7375 6c74 5f69 6e66 6f0a 2020  n result_info.  
-000075f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00007600: 2020 2020 2020 2020 6766 6f2e 7265 6d6f          gfo.remo
-00007610: 7665 286f 7574 7075 745f 7061 7468 290a  ve(output_path).
-00007620: 0a20 2020 2023 204e 6f77 2073 7461 7274  .    # Now start
-00007630: 2064 6973 736f 6c76 696e 670a 2020 2020   dissolving.    
-00007640: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
-00007650: 2d2d 2d2d 2d2d 0a20 2020 2023 2045 6d70  ------.    # Emp
-00007660: 7479 206f 7220 4c69 6e65 2061 6e64 2070  ty or Line and p
-00007670: 6f69 6e74 206c 6179 6572 7320 6172 653a  oint layers are:
-00007680: 0a20 2020 2023 2020 202a 206e 6f74 2073  .    #   * not s
-00007690: 6f20 6c61 7267 6520 286d 656d 6f72 792d  o large (memory-
-000076a0: 7769 7365 290a 2020 2020 2320 2020 2a20  wise).    #   * 
-000076b0: 6172 656e 2774 2063 6f6d 7075 7461 7469  aren't computati
-000076c0: 6f6e 616c 6c79 2068 6561 7679 0a20 2020  onally heavy.   
-000076d0: 2023 2041 6464 6974 696f 6e61 6c6c 7920   # Additionally 
-000076e0: 6c69 6e65 206c 6179 6572 7320 6172 6520  line layers are 
-000076f0: 6120 7061 696e 2074 6f20 6861 6e64 6c65  a pain to handle
-00007700: 2063 6f72 7265 6374 6c79 2062 6563 6175   correctly becau
-00007710: 7365 206f 660a 2020 2020 2320 726f 756e  se of.    # roun
-00007720: 6469 6e67 2069 7373 7565 7320 6174 2074  ding issues at t
-00007730: 6865 2062 6f72 6465 7273 206f 6620 7469  he borders of ti
-00007740: 6c65 732e 2e2e 2073 6f20 6a75 7374 2064  les... so just d
-00007750: 6973 736f 6c76 6520 7468 656d 2069 6e20  issolve them in 
-00007760: 6f6e 6520 676f 2e0a 2020 2020 6966 2028  one go..    if (
-00007770: 0a20 2020 2020 2020 2069 6e70 7574 5f6c  .        input_l
-00007780: 6179 6572 696e 666f 2e66 6561 7475 7265  ayerinfo.feature
-00007790: 636f 756e 7420 3d3d 2030 0a20 2020 2020  count == 0.     
-000077a0: 2020 206f 7220 696e 7075 745f 6c61 7965     or input_laye
-000077b0: 7269 6e66 6f2e 6765 6f6d 6574 7279 7479  rinfo.geometryty
-000077c0: 7065 2e74 6f5f 7072 696d 6974 6976 6574  pe.to_primitivet
-000077d0: 7970 650a 2020 2020 2020 2020 696e 205b  ype.        in [
-000077e0: 0a20 2020 2020 2020 2020 2020 2050 7269  .            Pri
-000077f0: 6d69 7469 7665 5479 7065 2e50 4f49 4e54  mitiveType.POINT
-00007800: 2c0a 2020 2020 2020 2020 2020 2020 5072  ,.            Pr
-00007810: 696d 6974 6976 6554 7970 652e 4c49 4e45  imitiveType.LINE
-00007820: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-00007830: 5d0a 2020 2020 293a 0a20 2020 2020 2020  ].    ):.       
-00007840: 205f 6765 6f6f 7073 5f73 716c 2e64 6973   _geoops_sql.dis
-00007850: 736f 6c76 655f 7369 6e67 6c65 7468 7265  solve_singlethre
-00007860: 6164 280a 2020 2020 2020 2020 2020 2020  ad(.            
-00007870: 696e 7075 745f 7061 7468 3d69 6e70 7574  input_path=input
-00007880: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-00007890: 2020 206f 7574 7075 745f 7061 7468 3d6f     output_path=o
-000078a0: 7574 7075 745f 7061 7468 2c0a 2020 2020  utput_path,.    
-000078b0: 2020 2020 2020 2020 6578 706c 6f64 6563          explodec
-000078c0: 6f6c 6c65 6374 696f 6e73 3d65 7870 6c6f  ollections=explo
-000078d0: 6465 636f 6c6c 6563 7469 6f6e 732c 0a20  decollections,. 
-000078e0: 2020 2020 2020 2020 2020 2067 726f 7570             group
-000078f0: 6279 5f63 6f6c 756d 6e73 3d67 726f 7570  by_columns=group
-00007900: 6279 5f63 6f6c 756d 6e73 2c0a 2020 2020  by_columns,.    
-00007910: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
-00007920: 6d6e 733d 6167 675f 636f 6c75 6d6e 732c  mns=agg_columns,
-00007930: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-00007940: 7574 5f6c 6179 6572 3d69 6e70 7574 5f6c  ut_layer=input_l
-00007950: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
-00007960: 2020 6f75 7470 7574 5f6c 6179 6572 3d6f    output_layer=o
-00007970: 7574 7075 745f 6c61 7965 722c 0a20 2020  utput_layer,.   
-00007980: 2020 2020 2020 2020 2066 6f72 6365 3d66           force=f
-00007990: 6f72 6365 2c0a 2020 2020 2020 2020 290a  orce,.        ).
-000079a0: 0a20 2020 2065 6c69 6620 696e 7075 745f  .    elif input_
-000079b0: 6c61 7965 7269 6e66 6f2e 6765 6f6d 6574  layerinfo.geomet
-000079c0: 7279 7479 7065 2e74 6f5f 7072 696d 6974  rytype.to_primit
-000079d0: 6976 6574 7970 6520 6973 2050 7269 6d69  ivetype is Primi
-000079e0: 7469 7665 5479 7065 2e50 4f4c 5947 4f4e  tiveType.POLYGON
-000079f0: 3a0a 2020 2020 2020 2020 2320 4966 2061  :.        # If a
-00007a00: 2074 696c 6573 5f70 6174 6820 6973 2073   tiles_path is s
-00007a10: 7065 6369 6669 6564 2c20 7265 6164 2074  pecified, read t
-00007a20: 686f 7365 2074 696c 6573 2e2e 2e0a 2020  hose tiles....  
-00007a30: 2020 2020 2020 7265 7375 6c74 5f74 696c        result_til
-00007a40: 6573 5f67 6466 203d 204e 6f6e 650a 2020  es_gdf = None.  
-00007a50: 2020 2020 2020 6966 2074 696c 6573 5f70        if tiles_p
-00007a60: 6174 6820 6973 206e 6f74 204e 6f6e 653a  ath is not None:
-00007a70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00007a80: 756c 745f 7469 6c65 735f 6764 6620 3d20  ult_tiles_gdf = 
-00007a90: 6766 6f2e 7265 6164 5f66 696c 6528 7469  gfo.read_file(ti
-00007aa0: 6c65 735f 7061 7468 290a 2020 2020 2020  les_path).      
-00007ab0: 2020 2020 2020 6966 206e 625f 7061 7261        if nb_para
-00007ac0: 6c6c 656c 203d 3d20 2d31 3a0a 2020 2020  llel == -1:.    
-00007ad0: 2020 2020 2020 2020 2020 2020 6e62 5f63              nb_c
-00007ae0: 7075 203d 206d 756c 7469 7072 6f63 6573  pu = multiproces
-00007af0: 7369 6e67 2e63 7075 5f63 6f75 6e74 2829  sing.cpu_count()
-00007b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b10: 206e 625f 7061 7261 6c6c 656c 203d 206e   nb_parallel = n
-00007b20: 625f 6370 7520 2023 2069 6e74 2831 2e32  b_cpu  # int(1.2
-00007b30: 3520 2a20 6e62 5f63 7075 290a 2020 2020  5 * nb_cpu).    
-00007b40: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00007b50: 6572 2e64 6562 7567 2866 224e 6220 6370  er.debug(f"Nb cp
-00007b60: 7573 2066 6f75 6e64 3a20 7b6e 625f 6370  us found: {nb_cp
-00007b70: 757d 2c20 6e62 5f70 6172 616c 6c65 6c3a  u}, nb_parallel:
-00007b80: 207b 6e62 5f70 6172 616c 6c65 6c7d 2229   {nb_parallel}")
-00007b90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00007ba0: 2020 2020 2020 2020 2020 2023 2045 6c73             # Els
-00007bb0: 652c 2063 7265 6174 6520 6120 6772 6964  e, create a grid
-00007bc0: 2062 6173 6564 206f 6e20 7468 6520 6e75   based on the nu
-00007bd0: 6d62 6572 206f 6620 7469 6c65 7320 7761  mber of tiles wa
-00007be0: 6e74 6564 2061 7320 7265 7375 6c74 0a20  nted as result. 
-00007bf0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00007c00: 745f 7469 6c65 735f 6764 6620 3d20 6772  t_tiles_gdf = gr
-00007c10: 6964 5f75 7469 6c2e 6372 6561 7465 5f67  id_util.create_g
-00007c20: 7269 6432 280a 2020 2020 2020 2020 2020  rid2(.          
-00007c30: 2020 2020 2020 696e 7075 745f 6c61 7965        input_laye
-00007c40: 7269 6e66 6f2e 746f 7461 6c5f 626f 756e  rinfo.total_boun
-00007c50: 6473 2c20 6e62 5f73 7175 6172 6973 685f  ds, nb_squarish_
-00007c60: 7469 6c65 732c 2069 6e70 7574 5f6c 6179  tiles, input_lay
-00007c70: 6572 696e 666f 2e63 7273 0a20 2020 2020  erinfo.crs.     
-00007c80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00007c90: 2020 2020 2069 6620 6c65 6e28 7265 7375       if len(resu
-00007ca0: 6c74 5f74 696c 6573 5f67 6466 2920 3e20  lt_tiles_gdf) > 
-00007cb0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00007cc0: 2020 2067 666f 2e74 6f5f 6669 6c65 280a     gfo.to_file(.
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ce0: 2020 2020 7265 7375 6c74 5f74 696c 6573      result_tiles
-00007cf0: 5f67 6466 2c0a 2020 2020 2020 2020 2020  _gdf,.          
-00007d00: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00007d10: 5f70 6174 682e 7061 7265 6e74 202f 2066  _path.parent / f
-00007d20: 227b 6f75 7470 7574 5f70 6174 682e 7374  "{output_path.st
-00007d30: 656d 7d5f 7469 6c65 732e 6770 6b67 222c  em}_tiles.gpkg",
-00007d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d50: 2029 0a0a 2020 2020 2020 2020 2320 4966   )..        # If
-00007d60: 2061 2074 696c 6564 2072 6573 756c 7420   a tiled result 
-00007d70: 6973 2061 736b 6564 2c20 6164 6420 7469  is asked, add ti
-00007d80: 6c65 5f69 6420 746f 2067 726f 7570 206f  le_id to group o
-00007d90: 6e20 666f 7220 7468 6520 7265 7375 6c74  n for the result
-00007da0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00007db0: 7265 7375 6c74 5f74 696c 6573 5f67 6466  result_tiles_gdf
-00007dc0: 2920 3e20 313a 0a20 2020 2020 2020 2020  ) > 1:.         
-00007dd0: 2020 2072 6573 756c 745f 7469 6c65 735f     result_tiles_
-00007de0: 6764 665b 2274 696c 655f 6964 225d 203d  gdf["tile_id"] =
-00007df0: 2072 6573 756c 745f 7469 6c65 735f 6764   result_tiles_gd
-00007e00: 662e 7265 7365 745f 696e 6465 7828 292e  f.reset_index().
-00007e10: 696e 6465 780a 0a20 2020 2020 2020 2023  index..        #
-00007e20: 2054 6865 2064 6973 736f 6c76 6520 666f   The dissolve fo
-00007e30: 7220 706f 6c79 676f 6e73 2069 7320 646f  r polygons is do
-00007e40: 6e65 2069 6e20 7365 7665 7261 6c20 7061  ne in several pa
-00007e50: 7373 6573 2c20 616e 6420 6166 7465 7220  sses, and after 
-00007e60: 7468 6520 6669 7273 740a 2020 2020 2020  the first.      
-00007e70: 2020 2320 7061 7373 2c20 6f6e 6c79 2074    # pass, only t
-00007e80: 6865 2027 6f6e 626f 7264 6572 2720 6665  he 'onborder' fe
-00007e90: 6174 7572 6573 2061 7265 2066 7572 7468  atures are furth
-00007ea0: 6572 2064 6973 736f 6c76 6564 2c20 6173  er dissolved, as
-00007eb0: 2074 6865 0a20 2020 2020 2020 2023 2027   the.        # '
-00007ec0: 6e6f 746f 6e62 6f72 6465 7227 2066 6561  notonborder' fea
-00007ed0: 7475 7265 7320 6172 6520 616c 7265 6164  tures are alread
-00007ee0: 7920 4f4b 2e0a 2020 2020 2020 2020 7465  y OK..        te
-00007ef0: 6d70 6469 7220 3d20 5f69 6f5f 7574 696c  mpdir = _io_util
-00007f00: 2e63 7265 6174 655f 7465 6d70 6469 7228  .create_tempdir(
-00007f10: 6622 6765 6f66 696c 656f 7073 2f7b 6f70  f"geofileops/{op
-00007f20: 6572 6174 696f 6e7d 2229 0a20 2020 2020  eration}").     
-00007f30: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00007f40: 2020 2020 6966 206f 7574 7075 745f 6c61      if output_la
-00007f50: 7965 7220 6973 204e 6f6e 653a 0a20 2020  yer is None:.   
-00007f60: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00007f70: 7075 745f 6c61 7965 7220 3d20 6766 6f2e  put_layer = gfo.
-00007f80: 6765 745f 6465 6661 756c 745f 6c61 7965  get_default_laye
-00007f90: 7228 6f75 7470 7574 5f70 6174 6829 0a20  r(output_path). 
-00007fa0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00007fb0: 745f 746d 705f 7061 7468 203d 2074 656d  t_tmp_path = tem
-00007fc0: 7064 6972 202f 2066 227b 6f75 7470 7574  pdir / f"{output
-00007fd0: 5f70 6174 682e 7374 656d 7d2e 6770 6b67  _path.stem}.gpkg
-00007fe0: 220a 2020 2020 2020 2020 2020 2020 7072  ".            pr
-00007ff0: 6576 5f6e 625f 6261 7463 6865 7320 3d20  ev_nb_batches = 
-00008000: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00008010: 206c 6173 745f 7061 7373 203d 2046 616c   last_pass = Fal
-00008020: 7365 0a20 2020 2020 2020 2020 2020 2070  se.            p
-00008030: 6173 735f 6964 203d 2030 0a20 2020 2020  ass_id = 0.     
-00008040: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00008050: 666f 2866 2253 7461 7274 2064 6973 736f  fo(f"Start disso
-00008060: 6c76 6520 6f6e 2066 696c 6520 7b69 6e70  lve on file {inp
-00008070: 7574 5f70 6174 687d 2229 0a20 2020 2020  ut_path}").     
-00008080: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-00008090: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000080a0: 2020 2023 2047 6574 2069 6e66 6f20 6f66     # Get info of
-000080b0: 2074 6865 2063 7572 7265 6e74 2066 696c   the current fil
-000080c0: 6520 7468 6174 206e 6565 6473 2074 6f20  e that needs to 
-000080d0: 6265 2064 6973 736f 6c76 6564 0a20 2020  be dissolved.   
-000080e0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-000080f0: 735f 696e 7075 745f 6c61 7965 7269 6e66  s_input_layerinf
-00008100: 6f20 3d20 6766 6f2e 6765 745f 6c61 7965  o = gfo.get_laye
-00008110: 7269 6e66 6f28 696e 7075 745f 7061 7468  rinfo(input_path
-00008120: 2c20 696e 7075 745f 6c61 7965 7229 0a20  , input_layer). 
-00008130: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00008140: 625f 726f 7773 5f74 6f74 616c 203d 2070  b_rows_total = p
-00008150: 6173 735f 696e 7075 745f 6c61 7965 7269  ass_input_layeri
-00008160: 6e66 6f2e 6665 6174 7572 6563 6f75 6e74  nfo.featurecount
-00008170: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008180: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
-00008190: 6520 6265 7374 206e 756d 6265 7220 6f66  e best number of
-000081a0: 2070 6172 616c 6c65 6c20 7072 6f63 6573   parallel proces
-000081b0: 7365 7320 616e 6420 6261 7463 6865 7320  ses and batches 
-000081c0: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
-000081d0: 2020 2020 2320 7468 6520 6176 6169 6c61      # the availa
-000081e0: 626c 6520 7265 736f 7572 6365 7320 666f  ble resources fo
-000081f0: 7220 7468 6520 6375 7272 656e 7420 7061  r the current pa
-00008200: 7373 0a20 2020 2020 2020 2020 2020 2020  ss.             
-00008210: 2020 2069 6620 6261 7463 6873 697a 6520     if batchsize 
-00008220: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-00008230: 2020 2020 2020 2020 2070 6172 616c 6c65           paralle
-00008240: 6c69 7a61 7469 6f6e 5f63 6f6e 6669 6720  lization_config 
-00008250: 3d20 5061 7261 6c6c 656c 697a 6174 696f  = Parallelizatio
-00008260: 6e43 6f6e 6669 6728 0a20 2020 2020 2020  nConfig(.       
-00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008280: 206d 696e 5f61 7667 5f72 6f77 735f 7065   min_avg_rows_pe
-00008290: 725f 6261 7463 683d 696e 7428 6d61 7468  r_batch=int(math
-000082a0: 2e63 6569 6c28 6261 7463 6873 697a 6520  .ceil(batchsize 
-000082b0: 2f20 3229 292c 0a20 2020 2020 2020 2020  / 2)),.         
-000082c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000082d0: 6178 5f61 7667 5f72 6f77 735f 7065 725f  ax_avg_rows_per_
-000082e0: 6261 7463 683d 6261 7463 6873 697a 652c  batch=batchsize,
-000082f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008300: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00008310: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2070 6172 616c 6c65 6c69 7a61 7469 6f6e   parallelization
-00008340: 5f63 6f6e 6669 6720 3d20 5061 7261 6c6c  _config = Parall
-00008350: 656c 697a 6174 696f 6e43 6f6e 6669 6728  elizationConfig(
-00008360: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008370: 2020 6e62 5f70 6172 616c 6c65 6c2c 206e    nb_parallel, n
-00008380: 625f 6261 7463 6865 735f 7265 636f 6d6d  b_batches_recomm
-00008390: 656e 6465 642c 205f 203d 2067 6574 5f70  ended, _ = get_p
-000083a0: 6172 616c 6c65 6c69 7a61 7469 6f6e 5f70  arallelization_p
-000083b0: 6172 616d 7328 0a20 2020 2020 2020 2020  arams(.         
-000083c0: 2020 2020 2020 2020 2020 206e 625f 726f             nb_ro
-000083d0: 7773 5f74 6f74 616c 3d6e 625f 726f 7773  ws_total=nb_rows
-000083e0: 5f74 6f74 616c 2c0a 2020 2020 2020 2020  _total,.        
-000083f0: 2020 2020 2020 2020 2020 2020 6e62 5f70              nb_p
-00008400: 6172 616c 6c65 6c3d 6e62 5f70 6172 616c  arallel=nb_paral
-00008410: 6c65 6c2c 0a20 2020 2020 2020 2020 2020  lel,.           
-00008420: 2020 2020 2020 2020 206e 625f 6261 7463           nb_batc
-00008430: 6865 735f 7072 6576 696f 7573 5f70 6173  hes_previous_pas
-00008440: 733d 7072 6576 5f6e 625f 6261 7463 6865  s=prev_nb_batche
-00008450: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00008460: 2020 2020 2020 2070 6172 616c 6c65 6c69         paralleli
-00008470: 7a61 7469 6f6e 5f63 6f6e 6669 673d 7061  zation_config=pa
-00008480: 7261 6c6c 656c 697a 6174 696f 6e5f 636f  rallelization_co
-00008490: 6e66 6967 2c0a 2020 2020 2020 2020 2020  nfig,.          
-000084a0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000084b0: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
-000084c0: 6520 6964 6561 6c20 6e75 6d62 6572 206f  e ideal number o
-000084d0: 6620 6261 7463 6865 7320 6973 2063 6c6f  f batches is clo
-000084e0: 7365 2074 6f20 7468 6520 6e62 2e20 7265  se to the nb. re
-000084f0: 7375 6c74 2074 696c 6573 2061 736b 6564  sult tiles asked
-00008500: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008510: 2020 2320 6469 7373 6f6c 7665 2074 6f77    # dissolve tow
-00008520: 6172 6473 2074 6865 2061 736b 6564 2072  ards the asked r
-00008530: 6573 756c 7421 0a20 2020 2020 2020 2020  esult!.         
-00008540: 2020 2020 2020 2023 2049 6620 6e6f 742c         # If not,
-00008550: 2061 2074 656d 706f 7261 7279 2072 6573   a temporary res
-00008560: 756c 7420 6973 2063 7265 6174 6564 2075  ult is created u
-00008570: 7369 6e67 2073 6d61 6c6c 6572 2074 696c  sing smaller til
-00008580: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00008590: 2020 2069 6620 6e62 5f62 6174 6368 6573     if nb_batches
-000085a0: 5f72 6563 6f6d 6d65 6e64 6564 203c 3d20  _recommended <= 
-000085b0: 6c65 6e28 7265 7375 6c74 5f74 696c 6573  len(result_tiles
-000085c0: 5f67 6466 2920 2a20 312e 313a 0a20 2020  _gdf) * 1.1:.   
-000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085e0: 2074 696c 6573 5f67 6466 203d 2072 6573   tiles_gdf = res
-000085f0: 756c 745f 7469 6c65 735f 6764 660a 2020  ult_tiles_gdf.  
-00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008610: 2020 6c61 7374 5f70 6173 7320 3d20 5472    last_pass = Tr
-00008620: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00008630: 2020 2020 2020 206e 625f 7061 7261 6c6c         nb_parall
-00008640: 656c 203d 206d 696e 286c 656e 2872 6573  el = min(len(res
-00008650: 756c 745f 7469 6c65 735f 6764 6629 2c20  ult_tiles_gdf), 
-00008660: 6e62 5f70 6172 616c 6c65 6c29 0a20 2020  nb_parallel).   
-00008670: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00008680: 6620 6c65 6e28 7265 7375 6c74 5f74 696c  f len(result_til
-00008690: 6573 5f67 6466 2920 3d3d 2031 3a0a 2020  es_gdf) == 1:.  
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086b0: 2020 2320 4372 6561 7465 2061 2067 7269    # Create a gri
-000086c0: 6420 6261 7365 6420 6f6e 2074 6865 2069  d based on the i
-000086d0: 6465 616c 206e 756d 6265 7220 6f66 2062  deal number of b
-000086e0: 6174 6368 6573 2c20 6275 7420 6d61 6b65  atches, but make
-000086f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008700: 2020 2020 2023 2073 7572 6520 7468 6520       # sure the 
-00008710: 6e75 6d62 6572 2069 7320 736d 616c 6c65  number is smalle
-00008720: 7220 7468 616e 2074 6865 206d 6178 696d  r than the maxim
-00008730: 756d 2e2e 2e0a 2020 2020 2020 2020 2020  um....          
-00008740: 2020 2020 2020 2020 2020 6e62 5f73 7175            nb_squ
-00008750: 6172 6973 685f 7469 6c65 735f 6d61 7820  arish_tiles_max 
-00008760: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00008770: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
-00008780: 6576 5f6e 625f 6261 7463 6865 7320 6973  ev_nb_batches is
-00008790: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087b0: 2020 206e 625f 7371 7561 7269 7368 5f74     nb_squarish_t
-000087c0: 696c 6573 5f6d 6178 203d 206d 6178 2870  iles_max = max(p
-000087d0: 7265 765f 6e62 5f62 6174 6368 6573 202d  rev_nb_batches -
-000087e0: 2031 2c20 3129 0a20 2020 2020 2020 2020   1, 1).         
-000087f0: 2020 2020 2020 2020 2020 2074 696c 6573             tiles
-00008800: 5f67 6466 203d 2067 7269 645f 7574 696c  _gdf = grid_util
-00008810: 2e63 7265 6174 655f 6772 6964 3228 0a20  .create_grid2(. 
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2020 2020 2020 2074 6f74 616c 5f62 6f75         total_bou
-00008840: 6e64 733d 7061 7373 5f69 6e70 7574 5f6c  nds=pass_input_l
-00008850: 6179 6572 696e 666f 2e74 6f74 616c 5f62  ayerinfo.total_b
-00008860: 6f75 6e64 732c 0a20 2020 2020 2020 2020  ounds,.         
-00008870: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00008880: 625f 7371 7561 7269 7368 5f74 696c 6573  b_squarish_tiles
-00008890: 3d6e 625f 6261 7463 6865 735f 7265 636f  =nb_batches_reco
-000088a0: 6d6d 656e 6465 642c 0a20 2020 2020 2020  mmended,.       
-000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 206e 625f 7371 7561 7269 7368 5f74 696c   nb_squarish_til
-000088d0: 6573 5f6d 6178 3d6e 625f 7371 7561 7269  es_max=nb_squari
-000088e0: 7368 5f74 696c 6573 5f6d 6178 2c0a 2020  sh_tiles_max,.  
-000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008900: 2020 2020 2020 6372 733d 7061 7373 5f69        crs=pass_i
-00008910: 6e70 7574 5f6c 6179 6572 696e 666f 2e63  nput_layerinfo.c
-00008920: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
-00008930: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00008940: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008960: 2020 2020 2320 4966 2061 2067 7269 6420      # If a grid 
-00008970: 6973 2073 7065 6369 6669 6564 2061 6c72  is specified alr
-00008980: 6561 6479 2c20 6164 6420 6578 7472 6120  eady, add extra 
-00008990: 636f 6c75 6d6e 732f 726f 7773 2069 6e73  columns/rows ins
-000089a0: 7465 6164 206f 660a 2020 2020 2020 2020  tead of.        
-000089b0: 2020 2020 2020 2020 2020 2020 2320 6372              # cr
-000089c0: 6561 7469 6e67 206e 6577 206f 6e65 2e2e  eating new one..
-000089d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000089e0: 2020 2020 2020 7469 6c65 735f 6764 6620        tiles_gdf 
-000089f0: 3d20 6772 6964 5f75 7469 6c2e 7370 6c69  = grid_util.spli
-00008a00: 745f 7469 6c65 7328 0a20 2020 2020 2020  t_tiles(.       
+00005550: 2020 2020 2020 2320 6f70 6572 6174 696f        # operatio
+00005560: 6e73 2069 7320 2861 206c 6f74 2920 6d6f  ns is (a lot) mo
+00005570: 7265 206c 696d 6974 6564 2074 6861 6e20  re limited than 
+00005580: 6764 616c 2d62 6173 6564 2c20 7573 6520  gdal-based, use 
+00005590: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+000055a0: 2020 2020 2020 2020 2020 2020 2320 6764              # gd
+000055b0: 616c 2076 6572 7369 6f6e 2076 6961 205f  al version via _
+000055c0: 6170 7065 6e64 5f74 6f5f 6e6f 6c6f 636b  append_to_nolock
+000055d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000055e0: 2020 2020 2020 2020 2020 6966 206e 625f            if nb_
+000055f0: 6261 7463 6865 7320 3d3d 2031 2061 6e64  batches == 1 and
+00005600: 2066 6f72 6365 5f6f 7574 7075 745f 6765   force_output_ge
+00005610: 6f6d 6574 7279 7479 7065 2069 7320 4e6f  ometrytype is No
+00005620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 6766 6f2e 6d6f 7665 2874 6d70 5f70 6172  gfo.move(tmp_par
+00005650: 7469 616c 5f6f 7574 7075 745f 7061 7468  tial_output_path
+00005660: 2c20 746d 705f 6f75 7470 7574 5f70 6174  , tmp_output_pat
+00005670: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+00005680: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00005690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000056a0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+000056b0: 656f 7073 2e5f 6170 7065 6e64 5f74 6f5f  eops._append_to_
+000056c0: 6e6f 6c6f 636b 280a 2020 2020 2020 2020  nolock(.        
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056e0: 2020 2020 2020 2020 7372 633d 746d 705f          src=tmp_
+000056f0: 7061 7274 6961 6c5f 6f75 7470 7574 5f70  partial_output_p
+00005700: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005720: 2020 2020 2064 7374 3d74 6d70 5f6f 7574       dst=tmp_out
+00005730: 7075 745f 7061 7468 2c0a 2020 2020 2020  put_path,.      
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 2020 2020 2020 2020 2020 6578 706c 6f64            explod
+00005760: 6563 6f6c 6c65 6374 696f 6e73 3d65 7870  ecollections=exp
+00005770: 6c6f 6465 636f 6c6c 6563 7469 6f6e 732c  lodecollections,
+00005780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057a0: 2063 7265 6174 655f 7370 6174 6961 6c5f   create_spatial_
+000057b0: 696e 6465 783d 4661 6c73 652c 0a20 2020  index=False,.   
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000057e0: 6365 5f6f 7574 7075 745f 6765 6f6d 6574  ce_output_geomet
+000057f0: 7279 7479 7065 3d66 6f72 6365 5f6f 7574  rytype=force_out
+00005800: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
+00005810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005820: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005840: 2020 2020 2020 2020 2020 2020 6766 6f2e              gfo.
+00005850: 7265 6d6f 7665 2874 6d70 5f70 6172 7469  remove(tmp_parti
+00005860: 616c 5f6f 7574 7075 745f 7061 7468 290a  al_output_path).
+00005870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005880: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00005890: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+000058a0: 2020 2020 2020 2062 6174 6368 5f69 6420         batch_id 
+000058b0: 3d20 6675 7475 7265 5f74 6f5f 6261 7463  = future_to_batc
+000058c0: 685f 6964 5b66 7574 7572 655d 0a20 2020  h_id[future].   
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2023 2063 616c 6375 6c61 7465 5f70 6f6f   # calculate_poo
+000058f0: 6c2e 7368 7574 646f 776e 2829 0a20 2020  l.shutdown().   
+00005900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005910: 206c 6f67 6765 722e 6578 6365 7074 696f   logger.exceptio
+00005920: 6e28 6622 4572 726f 7220 6578 6563 7574  n(f"Error execut
+00005930: 696e 6720 7b62 6174 6368 6573 5b62 6174  ing {batches[bat
+00005940: 6368 5f69 645d 7d22 290a 0a20 2020 2020  ch_id]}")..     
+00005950: 2020 2020 2020 2020 2020 2023 204c 6f67             # Log
+00005960: 2074 6865 2070 726f 6772 6573 7320 616e   the progress an
+00005970: 6420 7072 6564 6963 7469 6f6e 2073 7065  d prediction spe
+00005980: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00005990: 2020 206e 625f 646f 6e65 202b 3d20 310a     nb_done += 1.
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059b0: 5f67 656e 6572 616c 5f75 7469 6c2e 7265  _general_util.re
+000059c0: 706f 7274 5f70 726f 6772 6573 7328 0a20  port_progress(. 
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059e0: 2020 2073 7461 7274 5f74 696d 652c 206e     start_time, n
+000059f0: 625f 646f 6e65 2c20 6e62 5f62 6174 6368  b_done, nb_batch
+00005a00: 6573 2c20 6f70 6572 6174 696f 6e2e 7661  es, operation.va
+00005a10: 6c75 652c 206e 625f 7061 7261 6c6c 656c  lue, nb_parallel
+00005a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a30: 2029 0a0a 2020 2020 2020 2020 2320 526f   )..        # Ro
+00005a40: 756e 6420 7570 2061 6e64 2063 6c65 616e  und up and clean
+00005a50: 2075 700a 2020 2020 2020 2020 2320 4e6f   up.        # No
+00005a60: 7720 6372 6561 7465 2073 7061 7469 616c  w create spatial
+00005a70: 2069 6e64 6578 2061 6e64 206d 6f76 6520   index and move 
+00005a80: 746f 206f 7574 7075 7420 6c6f 6361 7469  to output locati
+00005a90: 6f6e 0a20 2020 2020 2020 2069 6620 746d  on.        if tm
+00005aa0: 705f 6f75 7470 7574 5f70 6174 682e 6578  p_output_path.ex
+00005ab0: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
+00005ac0: 2020 2020 6766 6f2e 6372 6561 7465 5f73      gfo.create_s
+00005ad0: 7061 7469 616c 5f69 6e64 6578 2870 6174  patial_index(pat
+00005ae0: 683d 746d 705f 6f75 7470 7574 5f70 6174  h=tmp_output_pat
+00005af0: 682c 206c 6179 6572 3d6f 7574 7075 745f  h, layer=output_
+00005b00: 6c61 7965 7229 0a20 2020 2020 2020 2020  layer).         
+00005b10: 2020 2067 666f 2e6d 6f76 6528 746d 705f     gfo.move(tmp_
+00005b20: 6f75 7470 7574 5f70 6174 682c 206f 7574  output_path, out
+00005b30: 7075 745f 7061 7468 290a 2020 2020 2020  put_path).      
+00005b40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00005b50: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00005b60: 2866 2252 6573 756c 7420 6f66 207b 6f70  (f"Result of {op
+00005b70: 6572 6174 696f 6e7d 2077 6173 2065 6d70  eration} was emp
+00005b80: 7479 2122 290a 0a20 2020 2066 696e 616c  ty!")..    final
+00005b90: 6c79 3a0a 2020 2020 2020 2020 2320 436c  ly:.        # Cl
+00005ba0: 6561 6e20 746d 7020 6469 720a 2020 2020  ean tmp dir.    
+00005bb0: 2020 2020 7368 7574 696c 2e72 6d74 7265      shutil.rmtre
+00005bc0: 6528 7465 6d70 6469 7229 0a20 2020 2020  e(tempdir).     
+00005bd0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+00005be0: 227b 6f70 6572 6174 696f 6e7d 2072 6561  "{operation} rea
+00005bf0: 6479 2c20 746f 6f6b 207b 6461 7465 7469  dy, took {dateti
+00005c00: 6d65 2e6e 6f77 2829 2d73 7461 7274 5f74  me.now()-start_t
+00005c10: 696d 655f 676c 6f62 616c 7d21 2229 0a0a  ime_global}!")..
+00005c20: 0a64 6566 205f 6170 706c 795f 6765 6f6f  .def _apply_geoo
+00005c30: 7065 7261 7469 6f6e 280a 2020 2020 696e  peration(.    in
+00005c40: 7075 745f 7061 7468 3a20 5061 7468 2c0a  put_path: Path,.
+00005c50: 2020 2020 6f75 7470 7574 5f70 6174 683a      output_path:
+00005c60: 2050 6174 682c 0a20 2020 206f 7065 7261   Path,.    opera
+00005c70: 7469 6f6e 3a20 4765 6f4f 7065 7261 7469  tion: GeoOperati
+00005c80: 6f6e 2c0a 2020 2020 6f70 6572 6174 696f  on,.    operatio
+00005c90: 6e5f 7061 7261 6d73 3a20 6469 6374 2c0a  n_params: dict,.
+00005ca0: 2020 2020 696e 7075 745f 6c61 7965 723a      input_layer:
+00005cb0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00005cc0: 204e 6f6e 652c 0a20 2020 206f 7574 7075   None,.    outpu
+00005cd0: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
+00005ce0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00005cf0: 2020 2063 6f6c 756d 6e73 3a20 4f70 7469     columns: Opti
+00005d00: 6f6e 616c 5b4c 6973 745b 7374 725d 5d20  onal[List[str]] 
+00005d10: 3d20 4e6f 6e65 2c0a 2020 2020 726f 7773  = None,.    rows
+00005d20: 3d4e 6f6e 652c 0a20 2020 2065 7870 6c6f  =None,.    explo
+00005d30: 6465 636f 6c6c 6563 7469 6f6e 733a 2062  decollections: b
+00005d40: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00005d50: 2067 7269 6473 697a 653a 2066 6c6f 6174   gridsize: float
+00005d60: 203d 2030 2e30 2c0a 2020 2020 666f 7263   = 0.0,.    forc
+00005d70: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+00005d80: 0a29 202d 3e20 7374 723a 0a20 2020 2023  .) -> str:.    #
+00005d90: 2049 6e69 740a 2020 2020 6966 206f 7574   Init.    if out
+00005da0: 7075 745f 7061 7468 2e65 7869 7374 7328  put_path.exists(
+00005db0: 293a 0a20 2020 2020 2020 2069 6620 666f  ):.        if fo
+00005dc0: 7263 6520 6973 2046 616c 7365 3a0a 2020  rce is False:.  
+00005dd0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00005de0: 6520 3d20 6622 5374 6f70 207b 6f70 6572  e = f"Stop {oper
+00005df0: 6174 696f 6e7d 3a20 6f75 7470 7574 2065  ation}: output e
+00005e00: 7869 7374 7320 616c 7265 6164 7920 7b6f  xists already {o
+00005e10: 7574 7075 745f 7061 7468 7d22 0a20 2020  utput_path}".   
+00005e20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00005e30: 6d65 7373 6167 650a 2020 2020 2020 2020  message.        
+00005e40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00005e50: 2020 6766 6f2e 7265 6d6f 7665 286f 7574    gfo.remove(out
+00005e60: 7075 745f 7061 7468 290a 0a20 2020 2023  put_path)..    #
+00005e70: 204e 6f77 2067 6f21 0a20 2020 2073 7461   Now go!.    sta
+00005e80: 7274 5f74 696d 6520 3d20 6461 7465 7469  rt_time = dateti
+00005e90: 6d65 2e6e 6f77 2829 0a20 2020 2064 6174  me.now().    dat
+00005ea0: 615f 6764 6620 3d20 6766 6f2e 7265 6164  a_gdf = gfo.read
+00005eb0: 5f66 696c 6528 0a20 2020 2020 2020 2070  _file(.        p
+00005ec0: 6174 683d 696e 7075 745f 7061 7468 2c20  ath=input_path, 
+00005ed0: 6c61 7965 723d 696e 7075 745f 6c61 7965  layer=input_laye
+00005ee0: 722c 2063 6f6c 756d 6e73 3d63 6f6c 756d  r, columns=colum
+00005ef0: 6e73 2c20 726f 7773 3d72 6f77 730a 2020  ns, rows=rows.  
+00005f00: 2020 290a 0a20 2020 2023 2052 756e 206f    )..    # Run o
+00005f10: 7065 7261 7469 6f6e 730a 2020 2020 6966  perations.    if
+00005f20: 206f 7065 7261 7469 6f6e 2069 7320 4765   operation is Ge
+00005f30: 6f4f 7065 7261 7469 6f6e 2e42 5546 4645  oOperation.BUFFE
+00005f40: 523a 0a20 2020 2020 2020 2064 6174 615f  R:.        data_
+00005f50: 6764 662e 6765 6f6d 6574 7279 203d 2064  gdf.geometry = d
+00005f60: 6174 615f 6764 662e 6765 6f6d 6574 7279  ata_gdf.geometry
+00005f70: 2e62 7566 6665 7228 0a20 2020 2020 2020  .buffer(.       
+00005f80: 2020 2020 2064 6973 7461 6e63 653d 6f70       distance=op
+00005f90: 6572 6174 696f 6e5f 7061 7261 6d73 5b22  eration_params["
+00005fa0: 6469 7374 616e 6365 225d 2c0a 2020 2020  distance"],.    
+00005fb0: 2020 2020 2020 2020 7265 736f 6c75 7469          resoluti
+00005fc0: 6f6e 3d6f 7065 7261 7469 6f6e 5f70 6172  on=operation_par
+00005fd0: 616d 735b 2271 7561 6472 616e 7473 6567  ams["quadrantseg
+00005fe0: 6d65 6e74 7322 5d2c 0a20 2020 2020 2020  ments"],.       
+00005ff0: 2020 2020 2063 6170 5f73 7479 6c65 3d6f       cap_style=o
+00006000: 7065 7261 7469 6f6e 5f70 6172 616d 735b  peration_params[
+00006010: 2265 6e64 6361 705f 7374 796c 6522 5d2e  "endcap_style"].
+00006020: 7661 6c75 652c 0a20 2020 2020 2020 2020  value,.         
+00006030: 2020 206a 6f69 6e5f 7374 796c 653d 6f70     join_style=op
+00006040: 6572 6174 696f 6e5f 7061 7261 6d73 5b22  eration_params["
+00006050: 6a6f 696e 5f73 7479 6c65 225d 2e76 616c  join_style"].val
+00006060: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00006070: 6d69 7472 655f 6c69 6d69 743d 6f70 6572  mitre_limit=oper
+00006080: 6174 696f 6e5f 7061 7261 6d73 5b22 6d69  ation_params["mi
+00006090: 7472 655f 6c69 6d69 7422 5d2c 0a20 2020  tre_limit"],.   
+000060a0: 2020 2020 2020 2020 2073 696e 676c 655f           single_
+000060b0: 7369 6465 643d 6f70 6572 6174 696f 6e5f  sided=operation_
+000060c0: 7061 7261 6d73 5b22 7369 6e67 6c65 5f73  params["single_s
+000060d0: 6964 6564 225d 2c0a 2020 2020 2020 2020  ided"],.        
+000060e0: 290a 2020 2020 656c 6966 206f 7065 7261  ).    elif opera
+000060f0: 7469 6f6e 2069 7320 4765 6f4f 7065 7261  tion is GeoOpera
+00006100: 7469 6f6e 2e43 4f4e 5645 5848 554c 4c3a  tion.CONVEXHULL:
+00006110: 0a20 2020 2020 2020 2064 6174 615f 6764  .        data_gd
+00006120: 662e 6765 6f6d 6574 7279 203d 2064 6174  f.geometry = dat
+00006130: 615f 6764 662e 6765 6f6d 6574 7279 2e63  a_gdf.geometry.c
+00006140: 6f6e 7665 785f 6875 6c6c 0a20 2020 2065  onvex_hull.    e
+00006150: 6c69 6620 6f70 6572 6174 696f 6e20 6973  lif operation is
+00006160: 2047 656f 4f70 6572 6174 696f 6e2e 5349   GeoOperation.SI
+00006170: 4d50 4c49 4659 3a0a 2020 2020 2020 2020  MPLIFY:.        
+00006180: 6461 7461 5f67 6466 2e67 656f 6d65 7472  data_gdf.geometr
+00006190: 7920 3d20 6765 6f73 6572 6965 735f 7574  y = geoseries_ut
+000061a0: 696c 2e73 696d 706c 6966 795f 6578 7428  il.simplify_ext(
+000061b0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000061c0: 615f 6764 662e 6765 6f6d 6574 7279 2c0a  a_gdf.geometry,.
+000061d0: 2020 2020 2020 2020 2020 2020 616c 676f              algo
+000061e0: 7269 7468 6d3d 6f70 6572 6174 696f 6e5f  rithm=operation_
+000061f0: 7061 7261 6d73 5b22 616c 676f 7269 7468  params["algorith
+00006200: 6d22 5d2c 0a20 2020 2020 2020 2020 2020  m"],.           
+00006210: 2074 6f6c 6572 616e 6365 3d6f 7065 7261   tolerance=opera
+00006220: 7469 6f6e 5f70 6172 616d 735b 2274 6f6c  tion_params["tol
+00006230: 6572 616e 6365 225d 2c0a 2020 2020 2020  erance"],.      
+00006240: 2020 2020 2020 6c6f 6f6b 6168 6561 643d        lookahead=
+00006250: 6f70 6572 6174 696f 6e5f 7061 7261 6d73  operation_params
+00006260: 5b22 7374 6570 225d 2c0a 2020 2020 2020  ["step"],.      
+00006270: 2020 290a 2020 2020 656c 6966 206f 7065    ).    elif ope
+00006280: 7261 7469 6f6e 2069 7320 4765 6f4f 7065  ration is GeoOpe
+00006290: 7261 7469 6f6e 2e41 5050 4c59 3a0a 2020  ration.APPLY:.  
+000062a0: 2020 2020 2020 6675 6e63 203d 2070 6963        func = pic
+000062b0: 6b6c 652e 6c6f 6164 7328 6f70 6572 6174  kle.loads(operat
+000062c0: 696f 6e5f 7061 7261 6d73 5b22 7069 636b  ion_params["pick
+000062d0: 6c65 645f 6675 6e63 225d 290a 2020 2020  led_func"]).    
+000062e0: 2020 2020 6966 206f 7065 7261 7469 6f6e      if operation
+000062f0: 5f70 6172 616d 735b 226f 6e6c 795f 6765  _params["only_ge
+00006300: 6f6d 5f69 6e70 7574 225d 2069 7320 5472  om_input"] is Tr
+00006310: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00006320: 6461 7461 5f67 6466 2e67 656f 6d65 7472  data_gdf.geometr
+00006330: 7920 3d20 6461 7461 5f67 6466 2e67 656f  y = data_gdf.geo
+00006340: 6d65 7472 792e 6170 706c 7928 6675 6e63  metry.apply(func
+00006350: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00006360: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00006370: 5f67 6466 2e67 656f 6d65 7472 7920 3d20  _gdf.geometry = 
+00006380: 6461 7461 5f67 6466 2e61 7070 6c79 2866  data_gdf.apply(f
+00006390: 756e 632c 2061 7869 733d 3129 0a20 2020  unc, axis=1).   
+000063a0: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+000063b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000063c0: 6622 6f70 6572 6174 696f 6e20 6e6f 7420  f"operation not 
+000063d0: 7375 7070 6f72 7465 643a 207b 6f70 6572  supported: {oper
+000063e0: 6174 696f 6e7d 2229 0a0a 2020 2020 2320  ation}")..    # 
+000063f0: 5265 6d6f 7665 2072 6f77 7320 7768 6572  Remove rows wher
+00006400: 6520 6765 6f6d 2069 7320 656d 7074 790a  e geom is empty.
+00006410: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00006420: 7461 6e63 6528 6461 7461 5f67 6466 2c20  tance(data_gdf, 
+00006430: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
+00006440: 290a 2020 2020 6173 7365 7274 2064 6174  ).    assert dat
+00006450: 615f 6764 662e 6765 6f6d 6574 7279 2069  a_gdf.geometry i
+00006460: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2064  s not None.    d
+00006470: 6174 615f 6764 6620 3d20 6461 7461 5f67  ata_gdf = data_g
+00006480: 6466 5b7e 6461 7461 5f67 6466 2e67 656f  df[~data_gdf.geo
+00006490: 6d65 7472 792e 6973 5f65 6d70 7479 5d0a  metry.is_empty].
+000064a0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+000064b0: 7461 6e63 6528 6461 7461 5f67 6466 2c20  tance(data_gdf, 
+000064c0: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
+000064d0: 290a 2020 2020 6461 7461 5f67 6466 203d  ).    data_gdf =
+000064e0: 2064 6174 615f 6764 665b 7e64 6174 615f   data_gdf[~data_
+000064f0: 6764 662e 6765 6f6d 6574 7279 2e69 736e  gdf.geometry.isn
+00006500: 6128 295d 0a0a 2020 2020 2320 4966 2074  a()]..    # If t
+00006510: 6865 7265 2069 7320 616e 2066 6964 2063  here is an fid c
+00006520: 6f6c 756d 6e20 696e 2074 6865 2064 6174  olumn in the dat
+00006530: 6173 6574 2c20 7265 6e61 6d65 2069 742c  aset, rename it,
+00006540: 2062 6563 6175 7365 2074 6865 2066 6964   because the fid
+00006550: 2063 6f6c 756d 6e20 6973 2061 0a20 2020   column is a.   
+00006560: 2023 2022 7370 6563 6961 6c20 6361 7365   # "special case
+00006570: 2220 696e 2067 6461 6c20 7468 6174 2073  " in gdal that s
+00006580: 686f 756c 6420 6e6f 7420 6265 2077 7269  hould not be wri
+00006590: 7474 656e 2e0a 2020 2020 636f 6c75 6d6e  tten..    column
+000065a0: 735f 6c6f 7765 725f 6c6f 6f6b 7570 203d  s_lower_lookup =
+000065b0: 207b 636f 6c75 6d6e 2e6c 6f77 6572 2829   {column.lower()
+000065c0: 3a20 636f 6c75 6d6e 2066 6f72 2063 6f6c  : column for col
+000065d0: 756d 6e20 696e 2064 6174 615f 6764 662e  umn in data_gdf.
+000065e0: 636f 6c75 6d6e 737d 0a20 2020 2069 6620  columns}.    if 
+000065f0: 2266 6964 2220 696e 2063 6f6c 756d 6e73  "fid" in columns
+00006600: 5f6c 6f77 6572 5f6c 6f6f 6b75 703a 0a20  _lower_lookup:. 
+00006610: 2020 2020 2020 2066 6964 5f63 6f6c 756d         fid_colum
+00006620: 6e20 3d20 636f 6c75 6d6e 735f 6c6f 7765  n = columns_lowe
+00006630: 725f 6c6f 6f6b 7570 5b22 6669 6422 5d0a  r_lookup["fid"].
+00006640: 2020 2020 2020 2020 666f 7220 6669 645f          for fid_
+00006650: 6e75 6d62 6572 2069 6e20 7261 6e67 6528  number in range(
+00006660: 312c 2031 3030 293a 0a20 2020 2020 2020  1, 100):.       
+00006670: 2020 2020 206e 6577 5f6e 616d 6520 3d20       new_name = 
+00006680: 6622 7b66 6964 5f63 6f6c 756d 6e7d 5f7b  f"{fid_column}_{
+00006690: 6669 645f 6e75 6d62 6572 7d22 0a20 2020  fid_number}".   
+000066a0: 2020 2020 2020 2020 2069 6620 6e65 775f           if new_
+000066b0: 6e61 6d65 206e 6f74 2069 6e20 636f 6c75  name not in colu
+000066c0: 6d6e 735f 6c6f 7765 725f 6c6f 6f6b 7570  mns_lower_lookup
+000066d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000066e0: 2020 6461 7461 5f67 6466 203d 2064 6174    data_gdf = dat
+000066f0: 615f 6764 662e 7265 6e61 6d65 280a 2020  a_gdf.rename(.  
+00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006710: 2020 636f 6c75 6d6e 733d 7b66 6964 5f63    columns={fid_c
+00006720: 6f6c 756d 6e3a 206e 6577 5f6e 616d 657d  olumn: new_name}
+00006730: 2c20 636f 7079 3d46 616c 7365 2020 2320  , copy=False  # 
+00006740: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00006750: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00006760: 2020 2069 6620 6578 706c 6f64 6563 6f6c     if explodecol
+00006770: 6c65 6374 696f 6e73 3a0a 2020 2020 2020  lections:.      
+00006780: 2020 6461 7461 5f67 6466 203d 2064 6174    data_gdf = dat
+00006790: 615f 6764 662e 6578 706c 6f64 6528 6967  a_gdf.explode(ig
+000067a0: 6e6f 7265 5f69 6e64 6578 3d54 7275 6529  nore_index=True)
+000067b0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+000067c0: 0a0a 2020 2020 6966 2067 7269 6473 697a  ..    if gridsiz
+000067d0: 6520 213d 2030 2e30 3a0a 2020 2020 2020  e != 0.0:.      
+000067e0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+000067f0: 6e63 6528 6461 7461 5f67 6466 2c20 6770  nce(data_gdf, gp
+00006800: 642e 4765 6f44 6174 6146 7261 6d65 290a  d.GeoDataFrame).
+00006810: 2020 2020 2020 2020 6461 7461 5f67 6466          data_gdf
+00006820: 2e67 656f 6d65 7472 7920 3d20 7368 6170  .geometry = shap
+00006830: 656c 7932 5f6f 725f 7079 6765 6f73 2e73  ely2_or_pygeos.s
+00006840: 6574 5f70 7265 6369 7369 6f6e 280a 2020  et_precision(.  
+00006850: 2020 2020 2020 2020 2020 6461 7461 5f67            data_g
+00006860: 6466 2e67 656f 6d65 7472 792e 6172 7261  df.geometry.arra
+00006870: 792e 6461 7461 2c20 6772 6964 5f73 697a  y.data, grid_siz
+00006880: 653d 6772 6964 7369 7a65 0a20 2020 2020  e=gridsize.     
+00006890: 2020 2029 0a0a 2020 2020 2320 4966 2074     )..    # If t
+000068a0: 6865 2072 6573 756c 7420 6973 2065 6d70  he result is emp
+000068b0: 7479 2c20 616e 6420 6e6f 206f 7574 7075  ty, and no outpu
+000068c0: 7420 6765 6f6d 6574 7279 7479 7065 2073  t geometrytype s
+000068d0: 7065 6369 6669 6564 2c20 7573 6520 696e  pecified, use in
+000068e0: 7075 740a 2020 2020 2320 6765 6f6d 6574  put.    # geomet
+000068f0: 7279 7479 7065 0a20 2020 2066 6f72 6365  rytype.    force
+00006900: 5f6f 7574 7075 745f 6765 6f6d 6574 7279  _output_geometry
+00006910: 7479 7065 203d 204e 6f6e 650a 2020 2020  type = None.    
+00006920: 6966 206c 656e 2864 6174 615f 6764 6629  if len(data_gdf)
+00006930: 203d 3d20 303a 0a20 2020 2020 2020 2069   == 0:.        i
+00006940: 6e70 7574 5f6c 6179 6572 696e 666f 203d  nput_layerinfo =
+00006950: 2067 666f 2e67 6574 5f6c 6179 6572 696e   gfo.get_layerin
+00006960: 666f 2869 6e70 7574 5f70 6174 682c 2069  fo(input_path, i
+00006970: 6e70 7574 5f6c 6179 6572 290a 2020 2020  nput_layer).    
+00006980: 2020 2020 666f 7263 655f 6f75 7470 7574      force_output
+00006990: 5f67 656f 6d65 7472 7974 7970 6520 3d20  _geometrytype = 
+000069a0: 696e 7075 745f 6c61 7965 7269 6e66 6f2e  input_layerinfo.
+000069b0: 6765 6f6d 6574 7279 7479 7065 2e74 6f5f  geometrytype.to_
+000069c0: 6d75 6c74 6974 7970 652e 6e61 6d65 0a0a  multitype.name..
+000069d0: 2020 2020 2320 6173 7365 7274 2074 6f20      # assert to 
+000069e0: 6576 6164 6520 7079 4c61 6e63 6520 7761  evade pyLance wa
+000069f0: 726e 696e 670a 2020 2020 6173 7365 7274  rning.    assert
+00006a00: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+00006a10: 5f67 6466 2c20 6770 642e 4765 6f44 6174  _gdf, gpd.GeoDat
+00006a20: 6146 7261 6d65 290a 2020 2020 2320 5573  aFrame).    # Us
+00006a30: 6520 666f 7263 655f 6d75 6c74 6974 7970  e force_multityp
+00006a40: 652c 2074 6f20 6576 6164 6520 7761 726e  e, to evade warn
+00006a50: 696e 6773 2077 6865 6e20 736f 6d65 2062  ings when some b
+00006a60: 6174 6368 6573 2063 6f6e 7461 696e 0a20  atches contain. 
+00006a70: 2020 2023 2073 696e 676c 6574 7970 6520     # singletype 
+00006a80: 616e 6420 736f 6d65 2063 6f6e 7461 696e  and some contain
+00006a90: 206d 756c 7469 7479 7065 2067 656f 6d65   multitype geome
+00006aa0: 7472 6965 730a 2020 2020 6766 6f2e 746f  tries.    gfo.to
+00006ab0: 5f66 696c 6528 0a20 2020 2020 2020 2067  _file(.        g
+00006ac0: 6466 3d64 6174 615f 6764 662c 0a20 2020  df=data_gdf,.   
+00006ad0: 2020 2020 2070 6174 683d 6f75 7470 7574       path=output
+00006ae0: 5f70 6174 682c 0a20 2020 2020 2020 206c  _path,.        l
+00006af0: 6179 6572 3d6f 7574 7075 745f 6c61 7965  ayer=output_laye
+00006b00: 722c 0a20 2020 2020 2020 2069 6e64 6578  r,.        index
+00006b10: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00006b20: 666f 7263 655f 6f75 7470 7574 5f67 656f  force_output_geo
+00006b30: 6d65 7472 7974 7970 653d 666f 7263 655f  metrytype=force_
+00006b40: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
+00006b50: 7970 652c 0a20 2020 2020 2020 2066 6f72  ype,.        for
+00006b60: 6365 5f6d 756c 7469 7479 7065 3d54 7275  ce_multitype=Tru
+00006b70: 652c 0a20 2020 2020 2020 2063 7265 6174  e,.        creat
+00006b80: 655f 7370 6174 6961 6c5f 696e 6465 783d  e_spatial_index=
+00006b90: 4661 6c73 652c 0a20 2020 2029 0a0a 2020  False,.    )..  
+00006ba0: 2020 6d65 7373 6167 6520 3d20 6622 546f    message = f"To
+00006bb0: 6f6b 207b 6461 7465 7469 6d65 2e6e 6f77  ok {datetime.now
+00006bc0: 2829 2d73 7461 7274 5f74 696d 657d 2066  ()-start_time} f
+00006bd0: 6f72 207b 6c65 6e28 6461 7461 5f67 6466  or {len(data_gdf
+00006be0: 297d 2072 6f77 7320 287b 726f 7773 7d29  )} rows ({rows})
+00006bf0: 2122 0a20 2020 2072 6574 7572 6e20 6d65  !".    return me
+00006c00: 7373 6167 650a 0a0a 6465 6620 6469 7373  ssage...def diss
+00006c10: 6f6c 7665 280a 2020 2020 696e 7075 745f  olve(.    input_
+00006c20: 7061 7468 3a20 5061 7468 2c0a 2020 2020  path: Path,.    
+00006c30: 6f75 7470 7574 5f70 6174 683a 2050 6174  output_path: Pat
+00006c40: 682c 0a20 2020 2067 726f 7570 6279 5f63  h,.    groupby_c
+00006c50: 6f6c 756d 6e73 3a20 4f70 7469 6f6e 616c  olumns: Optional
+00006c60: 5b49 7465 7261 626c 655b 7374 725d 5d20  [Iterable[str]] 
+00006c70: 3d20 4e6f 6e65 2c0a 2020 2020 6167 675f  = None,.    agg_
+00006c80: 636f 6c75 6d6e 733a 204f 7074 696f 6e61  columns: Optiona
+00006c90: 6c5b 6469 6374 5d20 3d20 4e6f 6e65 2c0a  l[dict] = None,.
+00006ca0: 2020 2020 6578 706c 6f64 6563 6f6c 6c65      explodecolle
+00006cb0: 6374 696f 6e73 3a20 626f 6f6c 203d 2054  ctions: bool = T
+00006cc0: 7275 652c 0a20 2020 2074 696c 6573 5f70  rue,.    tiles_p
+00006cd0: 6174 683a 204f 7074 696f 6e61 6c5b 5061  ath: Optional[Pa
+00006ce0: 7468 5d20 3d20 4e6f 6e65 2c0a 2020 2020  th] = None,.    
+00006cf0: 6e62 5f73 7175 6172 6973 685f 7469 6c65  nb_squarish_tile
+00006d00: 733a 2069 6e74 203d 2031 2c0a 2020 2020  s: int = 1,.    
+00006d10: 696e 7075 745f 6c61 7965 723a 204f 7074  input_layer: Opt
+00006d20: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00006d30: 652c 0a20 2020 206f 7574 7075 745f 6c61  e,.    output_la
+00006d40: 7965 723a 204f 7074 696f 6e61 6c5b 7374  yer: Optional[st
+00006d50: 725d 203d 204e 6f6e 652c 0a20 2020 2067  r] = None,.    g
+00006d60: 7269 6473 697a 653a 2066 6c6f 6174 203d  ridsize: float =
+00006d70: 2030 2e30 2c0a 2020 2020 6e62 5f70 6172   0.0,.    nb_par
+00006d80: 616c 6c65 6c3a 2069 6e74 203d 202d 312c  allel: int = -1,
+00006d90: 0a20 2020 2062 6174 6368 7369 7a65 3a20  .    batchsize: 
+00006da0: 696e 7420 3d20 2d31 2c0a 2020 2020 666f  int = -1,.    fo
+00006db0: 7263 653a 2062 6f6f 6c20 3d20 4661 6c73  rce: bool = Fals
+00006dc0: 652c 0a29 202d 3e20 6469 6374 3a0a 2020  e,.) -> dict:.  
+00006dd0: 2020 2222 220a 2020 2020 4675 6e63 7469    """.    Functi
+00006de0: 6f6e 2074 6861 7420 6170 706c 6965 7320  on that applies 
+00006df0: 6120 6469 7373 6f6c 7665 2e0a 0a20 2020  a dissolve...   
+00006e00: 204d 6f72 6520 6465 7461 696c 6564 2064   More detailed d
+00006e10: 6f63 756d 656e 7461 7469 6f6e 2069 6e20  ocumentation in 
+00006e20: 6d6f 6475 6c65 2067 656f 6f70 7321 0a20  module geoops!. 
+00006e30: 2020 2022 2222 0a0a 2020 2020 2320 496e     """..    # In
+00006e40: 6974 2061 6e64 2076 616c 6964 6174 6520  it and validate 
+00006e50: 696e 7075 7420 7061 7261 6d65 7465 7273  input parameters
+00006e60: 0a20 2020 2023 202d 2d2d 2d2d 2d2d 2d2d  .    # ---------
+00006e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006e80: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
+00006e90: 6172 745f 7469 6d65 203d 2064 6174 6574  art_time = datet
+00006ea0: 696d 652e 6e6f 7728 290a 2020 2020 6f70  ime.now().    op
+00006eb0: 6572 6174 696f 6e20 3d20 2264 6973 736f  eration = "disso
+00006ec0: 6c76 6522 0a20 2020 2072 6573 756c 745f  lve".    result_
+00006ed0: 696e 666f 203d 207b 7d0a 0a20 2020 2023  info = {}..    #
+00006ee0: 2043 6865 636b 2069 6e70 7574 2070 6172   Check input par
+00006ef0: 616d 6574 6572 730a 2020 2020 6966 2067  ameters.    if g
+00006f00: 726f 7570 6279 5f63 6f6c 756d 6e73 2069  roupby_columns i
+00006f10: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+00006f20: 656e 286c 6973 7428 6772 6f75 7062 795f  en(list(groupby_
+00006f30: 636f 6c75 6d6e 7329 2920 3d3d 2030 3a0a  columns)) == 0:.
+00006f40: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00006f50: 6c75 6545 7272 6f72 2822 6772 6f75 7062  lueError("groupb
+00006f60: 795f 636f 6c75 6d6e 733d 5b5d 2069 7320  y_columns=[] is 
+00006f70: 6e6f 7420 7375 7070 6f72 7465 642e 2055  not supported. U
+00006f80: 7365 204e 6f6e 652e 2229 0a20 2020 2069  se None.").    i
+00006f90: 6620 6e6f 7420 696e 7075 745f 7061 7468  f not input_path
+00006fa0: 2e65 7869 7374 7328 293a 0a20 2020 2020  .exists():.     
+00006fb0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00006fc0: 726f 7228 6622 696e 7075 745f 7061 7468  ror(f"input_path
+00006fd0: 2064 6f65 736e 2774 2065 7869 7374 3a20   doesn't exist: 
+00006fe0: 7b69 6e70 7574 5f70 6174 687d 2229 0a20  {input_path}"). 
+00006ff0: 2020 2069 6620 696e 7075 745f 7061 7468     if input_path
+00007000: 203d 3d20 6f75 7470 7574 5f70 6174 683a   == output_path:
+00007010: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00007020: 616c 7565 4572 726f 7228 226f 7574 7075  alueError("outpu
+00007030: 745f 7061 7468 206d 7573 7420 6e6f 7420  t_path must not 
+00007040: 6571 7561 6c20 696e 7075 745f 7061 7468  equal input_path
+00007050: 2229 0a0a 2020 2020 696e 7075 745f 6c61  ")..    input_la
+00007060: 7965 7269 6e66 6f20 3d20 6766 6f2e 6765  yerinfo = gfo.ge
+00007070: 745f 6c61 7965 7269 6e66 6f28 696e 7075  t_layerinfo(inpu
+00007080: 745f 7061 7468 2c20 696e 7075 745f 6c61  t_path, input_la
+00007090: 7965 7229 0a20 2020 2069 6620 696e 7075  yer).    if inpu
+000070a0: 745f 6c61 7965 7269 6e66 6f2e 6765 6f6d  t_layerinfo.geom
+000070b0: 6574 7279 7479 7065 2e74 6f5f 7072 696d  etrytype.to_prim
+000070c0: 6974 6976 6574 7970 6520 696e 205b 0a20  itivetype in [. 
+000070d0: 2020 2020 2020 2050 7269 6d69 7469 7665         Primitive
+000070e0: 5479 7065 2e50 4f49 4e54 2c0a 2020 2020  Type.POINT,.    
+000070f0: 2020 2020 5072 696d 6974 6976 6554 7970      PrimitiveTyp
+00007100: 652e 4c49 4e45 5354 5249 4e47 2c0a 2020  e.LINESTRING,.  
+00007110: 2020 5d3a 0a20 2020 2020 2020 2069 6620    ]:.        if 
+00007120: 7469 6c65 735f 7061 7468 2069 7320 6e6f  tiles_path is no
+00007130: 7420 4e6f 6e65 206f 7220 6e62 5f73 7175  t None or nb_squ
+00007140: 6172 6973 685f 7469 6c65 7320 3e20 313a  arish_tiles > 1:
+00007150: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00007160: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00007170: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00007180: 2244 6973 736f 6c76 6520 746f 2074 696c  "Dissolve to til
+00007190: 6573 2069 7320 6e6f 7420 7375 7070 6f72  es is not suppor
+000071a0: 7465 6420 666f 7220 7b69 6e70 7574 5f6c  ted for {input_l
+000071b0: 6179 6572 696e 666f 2e67 656f 6d65 7472  ayerinfo.geometr
+000071c0: 7974 7970 657d 220a 2020 2020 2020 2020  ytype}".        
+000071d0: 2020 2020 2020 2020 222c 2073 6f20 7469          ", so ti
+000071e0: 6c65 735f 7061 7468 2073 686f 756c 6420  les_path should 
+000071f0: 6265 204e 6f6e 6520 616e 6420 6e62 5f73  be None and nb_s
+00007200: 7175 6172 6973 685f 7469 6c65 7320 7368  quarish_tiles sh
+00007210: 6f75 6c64 2062 6520 3129 220a 2020 2020  ould be 1)".    
+00007220: 2020 2020 2020 2020 290a 0a20 2020 2023          )..    #
+00007230: 2043 6865 636b 2063 6f6c 756d 6e73 2069   Check columns i
+00007240: 6e20 6772 6f75 7062 795f 636f 6c75 6d6e  n groupby_column
+00007250: 730a 2020 2020 6966 2067 726f 7570 6279  s.    if groupby
+00007260: 5f63 6f6c 756d 6e73 2069 7320 6e6f 7420  _columns is not 
+00007270: 4e6f 6e65 3a0a 2020 2020 2020 2020 636f  None:.        co
+00007280: 6c75 6d6e 735f 696e 5f6c 6179 6572 5f75  lumns_in_layer_u
+00007290: 7070 6572 203d 205b 0a20 2020 2020 2020  pper = [.       
+000072a0: 2020 2020 2063 6f6c 756d 6e2e 7570 7065       column.uppe
+000072b0: 7228 2920 666f 7220 636f 6c75 6d6e 2069  r() for column i
+000072c0: 6e20 6c69 7374 2869 6e70 7574 5f6c 6179  n list(input_lay
+000072d0: 6572 696e 666f 2e63 6f6c 756d 6e73 2920  erinfo.columns) 
+000072e0: 2b20 5b22 6669 6422 5d0a 2020 2020 2020  + ["fid"].      
+000072f0: 2020 5d0a 2020 2020 2020 2020 666f 7220    ].        for 
+00007300: 636f 6c75 6d6e 2069 6e20 6772 6f75 7062  column in groupb
+00007310: 795f 636f 6c75 6d6e 733a 0a20 2020 2020  y_columns:.     
+00007320: 2020 2020 2020 2069 6620 636f 6c75 6d6e         if column
+00007330: 2e75 7070 6572 2829 206e 6f74 2069 6e20  .upper() not in 
+00007340: 636f 6c75 6d6e 735f 696e 5f6c 6179 6572  columns_in_layer
+00007350: 5f75 7070 6572 3a0a 2020 2020 2020 2020  _upper:.        
+00007360: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00007370: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00007380: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00007390: 636f 6c75 6d6e 2069 6e20 6772 6f75 7062  column in groupb
+000073a0: 795f 636f 6c75 6d6e 7320 6e6f 7420 6176  y_columns not av
+000073b0: 6169 6c61 626c 6520 696e 206c 6179 6572  ailable in layer
+000073c0: 3a20 7b63 6f6c 756d 6e7d 220a 2020 2020  : {column}".    
+000073d0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000073e0: 2020 2023 2043 6865 636b 2061 6767 5f63     # Check agg_c
+000073f0: 6f6c 756d 6e73 2070 6172 616d 0a20 2020  olumns param.   
+00007400: 2069 6620 6167 675f 636f 6c75 6d6e 7320   if agg_columns 
+00007410: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007420: 2020 2020 2023 2056 616c 6964 6174 6520       # Validate 
+00007430: 7468 6520 6469 6374 2073 7472 7563 7475  the dict structu
+00007440: 7265 2c20 736f 2077 6520 6361 6e20 6173  re, so we can as
+00007450: 7375 6d65 2065 7665 7279 7468 696e 6720  sume everything 
+00007460: 6973 204f 4b20 6675 7274 6865 7220 6f6e  is OK further on
+00007470: 0a20 2020 2020 2020 205f 7061 7261 6d65  .        _parame
+00007480: 7465 725f 6865 6c70 6572 2e76 616c 6964  ter_helper.valid
+00007490: 6174 655f 6167 675f 636f 6c75 6d6e 7328  ate_agg_columns(
+000074a0: 6167 675f 636f 6c75 6d6e 7329 0a0a 2020  agg_columns)..  
+000074b0: 2020 2020 2020 2320 4669 7273 7420 7461        # First ta
+000074c0: 6b65 2061 2064 6565 7020 636f 7079 2c20  ke a deep copy, 
+000074d0: 6173 2076 616c 7565 7320 6361 6e20 6265  as values can be
+000074e0: 2063 6861 6e67 6564 2066 7572 7468 6572   changed further
+000074f0: 206f 6e20 746f 2074 7265 6174 2063 6f6c   on to treat col
+00007500: 756d 6e73 0a20 2020 2020 2020 2023 2063  umns.        # c
+00007510: 6173 6520 696e 7365 6e73 6974 6976 650a  ase insensitive.
+00007520: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
+00007530: 6d6e 7320 3d20 6a73 6f6e 2e6c 6f61 6473  mns = json.loads
+00007540: 286a 736f 6e2e 6475 6d70 7328 6167 675f  (json.dumps(agg_
+00007550: 636f 6c75 6d6e 7329 290a 2020 2020 2020  columns)).      
+00007560: 2020 6173 7365 7274 2061 6767 5f63 6f6c    assert agg_col
+00007570: 756d 6e73 2069 7320 6e6f 7420 4e6f 6e65  umns is not None
+00007580: 0a20 2020 2020 2020 2069 6620 226a 736f  .        if "jso
+00007590: 6e22 2069 6e20 6167 675f 636f 6c75 6d6e  n" in agg_column
+000075a0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+000075b0: 6620 6167 675f 636f 6c75 6d6e 735b 226a  f agg_columns["j
+000075c0: 736f 6e22 5d20 6973 204e 6f6e 653a 0a20  son"] is None:. 
+000075d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000075e0: 6767 5f63 6f6c 756d 6e73 5b22 6a73 6f6e  gg_columns["json
+000075f0: 225d 203d 205b 0a20 2020 2020 2020 2020  "] = [.         
+00007600: 2020 2020 2020 2020 2020 2063 6f6c 2066             col f
+00007610: 6f72 2063 6f6c 2069 6e20 696e 7075 745f  or col in input_
+00007620: 6c61 7965 7269 6e66 6f2e 636f 6c75 6d6e  layerinfo.column
+00007630: 7320 6966 2063 6f6c 2e75 7070 6572 2829  s if col.upper()
+00007640: 2021 3d20 2249 4e44 4558 220a 2020 2020   != "INDEX".    
+00007650: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00007660: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007680: 2320 416c 6967 6e20 6361 7369 6e67 206f  # Align casing o
+00007690: 6620 636f 6c75 6d6e 206e 616d 6573 2074  f column names t
+000076a0: 6f20 6461 7461 0a20 2020 2020 2020 2020  o data.         
+000076b0: 2020 2020 2020 2061 6767 5f63 6f6c 756d         agg_colum
+000076c0: 6e73 5b22 6a73 6f6e 225d 203d 205f 6765  ns["json"] = _ge
+000076d0: 6e65 7261 6c5f 7574 696c 2e61 6c69 676e  neral_util.align
+000076e0: 5f63 6173 696e 675f 6c69 7374 280a 2020  _casing_list(.  
+000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007700: 2020 6167 675f 636f 6c75 6d6e 735b 226a    agg_columns["j
+00007710: 736f 6e22 5d2c 206c 6973 7428 696e 7075  son"], list(inpu
+00007720: 745f 6c61 7965 7269 6e66 6f2e 636f 6c75  t_layerinfo.colu
+00007730: 6d6e 7329 202b 205b 2266 6964 225d 0a20  mns) + ["fid"]. 
+00007740: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007750: 0a20 2020 2020 2020 2065 6c69 6620 2263  .        elif "c
+00007760: 6f6c 756d 6e73 2220 696e 2061 6767 5f63  olumns" in agg_c
+00007770: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
+00007780: 2020 2020 2320 4c6f 6f70 2074 6872 6f75      # Loop throu
+00007790: 6768 2061 6c6c 2072 6f77 730a 2020 2020  gh all rows.    
+000077a0: 2020 2020 2020 2020 666f 7220 6167 675f          for agg_
+000077b0: 636f 6c75 6d6e 2069 6e20 6167 675f 636f  column in agg_co
+000077c0: 6c75 6d6e 735b 2263 6f6c 756d 6e73 225d  lumns["columns"]
+000077d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000077e0: 2020 2320 4368 6563 6b20 6966 2063 6f6c    # Check if col
+000077f0: 756d 6e20 6578 6973 7473 202b 2073 6574  umn exists + set
+00007800: 2063 6173 696e 6720 7361 6d65 2061 7320   casing same as 
+00007810: 696e 2064 6174 610a 2020 2020 2020 2020  in data.        
+00007820: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
+00007830: 6d6e 5b22 636f 6c75 6d6e 225d 203d 205f  mn["column"] = _
+00007840: 6765 6e65 7261 6c5f 7574 696c 2e61 6c69  general_util.ali
+00007850: 676e 5f63 6173 696e 6728 0a20 2020 2020  gn_casing(.     
+00007860: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00007870: 6767 5f63 6f6c 756d 6e5b 2263 6f6c 756d  gg_column["colum
+00007880: 6e22 5d2c 206c 6973 7428 696e 7075 745f  n"], list(input_
+00007890: 6c61 7965 7269 6e66 6f2e 636f 6c75 6d6e  layerinfo.column
+000078a0: 7329 202b 205b 2266 6964 225d 0a20 2020  s) + ["fid"].   
+000078b0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+000078c0: 2020 2020 2320 4e6f 7720 696e 7075 7420      # Now input 
+000078d0: 7061 7261 6d65 7465 7273 2061 7265 2063  parameters are c
+000078e0: 6865 636b 6564 2c20 6368 6563 6b20 6966  hecked, check if
+000078f0: 2077 6520 6e65 6564 2074 6f20 6361 6c63   we need to calc
+00007900: 616c 6174 6520 616e 7977 6179 0a20 2020  alate anyway.   
+00007910: 2069 6620 6f75 7470 7574 5f70 6174 682e   if output_path.
+00007920: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
+00007930: 2020 6966 2066 6f72 6365 2069 7320 4661    if force is Fa
+00007940: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00007950: 2072 6573 756c 745f 696e 666f 5b0a 2020   result_info[.  
+00007960: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00007970: 6573 7361 6765 220a 2020 2020 2020 2020  essage".        
+00007980: 2020 2020 5d20 3d20 6622 6f75 7470 7574      ] = f"output
+00007990: 2065 7869 7374 7320 616c 7265 6164 7920   exists already 
+000079a0: 7b6f 7574 7075 745f 7061 7468 7d20 616e  {output_path} an
+000079b0: 6420 666f 7263 6520 6973 2066 616c 7365  d force is false
+000079c0: 220a 2020 2020 2020 2020 2020 2020 6c6f  ".            lo
+000079d0: 6767 6572 2e69 6e66 6f28 7265 7375 6c74  gger.info(result
+000079e0: 5f69 6e66 6f5b 226d 6573 7361 6765 225d  _info["message"]
+000079f0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007a00: 7475 726e 2072 6573 756c 745f 696e 666f  turn result_info
+00007a10: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00007a20: 2020 2020 2020 2020 2020 2067 666f 2e72             gfo.r
+00007a30: 656d 6f76 6528 6f75 7470 7574 5f70 6174  emove(output_pat
+00007a40: 6829 0a0a 2020 2020 2320 4e6f 7720 7374  h)..    # Now st
+00007a50: 6172 7420 6469 7373 6f6c 7669 6e67 0a20  art dissolving. 
+00007a60: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
+00007a70: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2320  ---------.    # 
+00007a80: 456d 7074 7920 6f72 204c 696e 6520 616e  Empty or Line an
+00007a90: 6420 706f 696e 7420 6c61 7965 7273 2061  d point layers a
+00007aa0: 7265 3a0a 2020 2020 2320 2020 2a20 6e6f  re:.    #   * no
+00007ab0: 7420 736f 206c 6172 6765 2028 6d65 6d6f  t so large (memo
+00007ac0: 7279 2d77 6973 6529 0a20 2020 2023 2020  ry-wise).    #  
+00007ad0: 202a 2061 7265 6e27 7420 636f 6d70 7574   * aren't comput
+00007ae0: 6174 696f 6e61 6c6c 7920 6865 6176 790a  ationally heavy.
+00007af0: 2020 2020 2320 4164 6469 7469 6f6e 616c      # Additional
+00007b00: 6c79 206c 696e 6520 6c61 7965 7273 2061  ly line layers a
+00007b10: 7265 2061 2070 6169 6e20 746f 2068 616e  re a pain to han
+00007b20: 646c 6520 636f 7272 6563 746c 7920 6265  dle correctly be
+00007b30: 6361 7573 6520 6f66 0a20 2020 2023 2072  cause of.    # r
+00007b40: 6f75 6e64 696e 6720 6973 7375 6573 2061  ounding issues a
+00007b50: 7420 7468 6520 626f 7264 6572 7320 6f66  t the borders of
+00007b60: 2074 696c 6573 2e2e 2e20 736f 206a 7573   tiles... so jus
+00007b70: 7420 6469 7373 6f6c 7665 2074 6865 6d20  t dissolve them 
+00007b80: 696e 206f 6e65 2067 6f2e 0a20 2020 2069  in one go..    i
+00007b90: 6620 280a 2020 2020 2020 2020 696e 7075  f (.        inpu
+00007ba0: 745f 6c61 7965 7269 6e66 6f2e 6665 6174  t_layerinfo.feat
+00007bb0: 7572 6563 6f75 6e74 203d 3d20 300a 2020  urecount == 0.  
+00007bc0: 2020 2020 2020 6f72 2069 6e70 7574 5f6c        or input_l
+00007bd0: 6179 6572 696e 666f 2e67 656f 6d65 7472  ayerinfo.geometr
+00007be0: 7974 7970 652e 746f 5f70 7269 6d69 7469  ytype.to_primiti
+00007bf0: 7665 7479 7065 0a20 2020 2020 2020 2069  vetype.        i
+00007c00: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
+00007c10: 5072 696d 6974 6976 6554 7970 652e 504f  PrimitiveType.PO
+00007c20: 494e 542c 0a20 2020 2020 2020 2020 2020  INT,.           
+00007c30: 2050 7269 6d69 7469 7665 5479 7065 2e4c   PrimitiveType.L
+00007c40: 494e 4553 5452 494e 472c 0a20 2020 2020  INESTRING,.     
+00007c50: 2020 205d 0a20 2020 2029 3a0a 2020 2020     ].    ):.    
+00007c60: 2020 2020 5f67 656f 6f70 735f 7371 6c2e      _geoops_sql.
+00007c70: 6469 7373 6f6c 7665 5f73 696e 676c 6574  dissolve_singlet
+00007c80: 6872 6561 6428 0a20 2020 2020 2020 2020  hread(.         
+00007c90: 2020 2069 6e70 7574 5f70 6174 683d 696e     input_path=in
+00007ca0: 7075 745f 7061 7468 2c0a 2020 2020 2020  put_path,.      
+00007cb0: 2020 2020 2020 6f75 7470 7574 5f70 6174        output_pat
+00007cc0: 683d 6f75 7470 7574 5f70 6174 682c 0a20  h=output_path,. 
+00007cd0: 2020 2020 2020 2020 2020 2065 7870 6c6f             explo
+00007ce0: 6465 636f 6c6c 6563 7469 6f6e 733d 6578  decollections=ex
+00007cf0: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
+00007d00: 2c0a 2020 2020 2020 2020 2020 2020 6772  ,.            gr
+00007d10: 6f75 7062 795f 636f 6c75 6d6e 733d 6772  oupby_columns=gr
+00007d20: 6f75 7062 795f 636f 6c75 6d6e 732c 0a20  oupby_columns,. 
+00007d30: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
+00007d40: 6f6c 756d 6e73 3d61 6767 5f63 6f6c 756d  olumns=agg_colum
+00007d50: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00007d60: 696e 7075 745f 6c61 7965 723d 696e 7075  input_layer=inpu
+00007d70: 745f 6c61 7965 722c 0a20 2020 2020 2020  t_layer,.       
+00007d80: 2020 2020 206f 7574 7075 745f 6c61 7965       output_laye
+00007d90: 723d 6f75 7470 7574 5f6c 6179 6572 2c0a  r=output_layer,.
+00007da0: 2020 2020 2020 2020 2020 2020 6772 6964              grid
+00007db0: 7369 7a65 3d67 7269 6473 697a 652c 0a20  size=gridsize,. 
+00007dc0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+00007dd0: 3d66 6f72 6365 2c0a 2020 2020 2020 2020  =force,.        
+00007de0: 290a 0a20 2020 2065 6c69 6620 696e 7075  )..    elif inpu
+00007df0: 745f 6c61 7965 7269 6e66 6f2e 6765 6f6d  t_layerinfo.geom
+00007e00: 6574 7279 7479 7065 2e74 6f5f 7072 696d  etrytype.to_prim
+00007e10: 6974 6976 6574 7970 6520 6973 2050 7269  itivetype is Pri
+00007e20: 6d69 7469 7665 5479 7065 2e50 4f4c 5947  mitiveType.POLYG
+00007e30: 4f4e 3a0a 2020 2020 2020 2020 2320 4966  ON:.        # If
+00007e40: 2061 2074 696c 6573 5f70 6174 6820 6973   a tiles_path is
+00007e50: 2073 7065 6369 6669 6564 2c20 7265 6164   specified, read
+00007e60: 2074 686f 7365 2074 696c 6573 2e2e 2e0a   those tiles....
+00007e70: 2020 2020 2020 2020 7265 7375 6c74 5f74          result_t
+00007e80: 696c 6573 5f67 6466 203d 204e 6f6e 650a  iles_gdf = None.
+00007e90: 2020 2020 2020 2020 6966 2074 696c 6573          if tiles
+00007ea0: 5f70 6174 6820 6973 206e 6f74 204e 6f6e  _path is not Non
+00007eb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00007ec0: 6573 756c 745f 7469 6c65 735f 6764 6620  esult_tiles_gdf 
+00007ed0: 3d20 6766 6f2e 7265 6164 5f66 696c 6528  = gfo.read_file(
+00007ee0: 7469 6c65 735f 7061 7468 290a 2020 2020  tiles_path).    
+00007ef0: 2020 2020 2020 2020 6966 206e 625f 7061          if nb_pa
+00007f00: 7261 6c6c 656c 203d 3d20 2d31 3a0a 2020  rallel == -1:.  
+00007f10: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+00007f20: 5f63 7075 203d 206d 756c 7469 7072 6f63  _cpu = multiproc
+00007f30: 6573 7369 6e67 2e63 7075 5f63 6f75 6e74  essing.cpu_count
+00007f40: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00007f50: 2020 206e 625f 7061 7261 6c6c 656c 203d     nb_parallel =
+00007f60: 206e 625f 6370 7520 2023 2069 6e74 2831   nb_cpu  # int(1
+00007f70: 2e32 3520 2a20 6e62 5f63 7075 290a 2020  .25 * nb_cpu).  
+00007f80: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00007f90: 6767 6572 2e64 6562 7567 2866 224e 6220  gger.debug(f"Nb 
+00007fa0: 6370 7573 2066 6f75 6e64 3a20 7b6e 625f  cpus found: {nb_
+00007fb0: 6370 757d 2c20 6e62 5f70 6172 616c 6c65  cpu}, nb_paralle
+00007fc0: 6c3a 207b 6e62 5f70 6172 616c 6c65 6c7d  l: {nb_parallel}
+00007fd0: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00007fe0: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+00007ff0: 6c73 652c 2063 7265 6174 6520 6120 6772  lse, create a gr
+00008000: 6964 2062 6173 6564 206f 6e20 7468 6520  id based on the 
+00008010: 6e75 6d62 6572 206f 6620 7469 6c65 7320  number of tiles 
+00008020: 7761 6e74 6564 2061 7320 7265 7375 6c74  wanted as result
+00008030: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00008040: 756c 745f 7469 6c65 735f 6764 6620 3d20  ult_tiles_gdf = 
+00008050: 6772 6964 5f75 7469 6c2e 6372 6561 7465  grid_util.create
+00008060: 5f67 7269 6432 280a 2020 2020 2020 2020  _grid2(.        
+00008070: 2020 2020 2020 2020 696e 7075 745f 6c61          input_la
+00008080: 7965 7269 6e66 6f2e 746f 7461 6c5f 626f  yerinfo.total_bo
+00008090: 756e 6473 2c20 6e62 5f73 7175 6172 6973  unds, nb_squaris
+000080a0: 685f 7469 6c65 732c 2069 6e70 7574 5f6c  h_tiles, input_l
+000080b0: 6179 6572 696e 666f 2e63 7273 0a20 2020  ayerinfo.crs.   
+000080c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000080d0: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
+000080e0: 7375 6c74 5f74 696c 6573 5f67 6466 2920  sult_tiles_gdf) 
+000080f0: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
+00008100: 2020 2020 2067 666f 2e74 6f5f 6669 6c65       gfo.to_file
+00008110: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008120: 2020 2020 2020 7265 7375 6c74 5f74 696c        result_til
+00008130: 6573 5f67 6466 2c0a 2020 2020 2020 2020  es_gdf,.        
+00008140: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00008150: 7574 5f70 6174 682e 7061 7265 6e74 202f  ut_path.parent /
+00008160: 2066 227b 6f75 7470 7574 5f70 6174 682e   f"{output_path.
+00008170: 7374 656d 7d5f 7469 6c65 732e 6770 6b67  stem}_tiles.gpkg
+00008180: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00008190: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
+000081a0: 4966 2061 2074 696c 6564 2072 6573 756c  If a tiled resul
+000081b0: 7420 6973 2061 736b 6564 2c20 6164 6420  t is asked, add 
+000081c0: 7469 6c65 5f69 6420 746f 2067 726f 7570  tile_id to group
+000081d0: 206f 6e20 666f 7220 7468 6520 7265 7375   on for the resu
+000081e0: 6c74 0a20 2020 2020 2020 2069 6620 6c65  lt.        if le
+000081f0: 6e28 7265 7375 6c74 5f74 696c 6573 5f67  n(result_tiles_g
+00008200: 6466 2920 3e20 313a 0a20 2020 2020 2020  df) > 1:.       
+00008210: 2020 2020 2072 6573 756c 745f 7469 6c65       result_tile
+00008220: 735f 6764 665b 2274 696c 655f 6964 225d  s_gdf["tile_id"]
+00008230: 203d 2072 6573 756c 745f 7469 6c65 735f   = result_tiles_
+00008240: 6764 662e 7265 7365 745f 696e 6465 7828  gdf.reset_index(
+00008250: 292e 696e 6465 780a 0a20 2020 2020 2020  ).index..       
+00008260: 2023 2054 6865 2064 6973 736f 6c76 6520   # The dissolve 
+00008270: 666f 7220 706f 6c79 676f 6e73 2069 7320  for polygons is 
+00008280: 646f 6e65 2069 6e20 7365 7665 7261 6c20  done in several 
+00008290: 7061 7373 6573 2c20 616e 6420 6166 7465  passes, and afte
+000082a0: 7220 7468 6520 6669 7273 740a 2020 2020  r the first.    
+000082b0: 2020 2020 2320 7061 7373 2c20 6f6e 6c79      # pass, only
+000082c0: 2074 6865 2027 6f6e 626f 7264 6572 2720   the 'onborder' 
+000082d0: 6665 6174 7572 6573 2061 7265 2066 7572  features are fur
+000082e0: 7468 6572 2064 6973 736f 6c76 6564 2c20  ther dissolved, 
+000082f0: 6173 2074 6865 0a20 2020 2020 2020 2023  as the.        #
+00008300: 2027 6e6f 746f 6e62 6f72 6465 7227 2066   'notonborder' f
+00008310: 6561 7475 7265 7320 6172 6520 616c 7265  eatures are alre
+00008320: 6164 7920 4f4b 2e0a 2020 2020 2020 2020  ady OK..        
+00008330: 7465 6d70 6469 7220 3d20 5f69 6f5f 7574  tempdir = _io_ut
+00008340: 696c 2e63 7265 6174 655f 7465 6d70 6469  il.create_tempdi
+00008350: 7228 6622 6765 6f66 696c 656f 7073 2f7b  r(f"geofileops/{
+00008360: 6f70 6572 6174 696f 6e7d 2229 0a20 2020  operation}").   
+00008370: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00008380: 2020 2020 2020 6966 206f 7574 7075 745f        if output_
+00008390: 6c61 7965 7220 6973 204e 6f6e 653a 0a20  layer is None:. 
+000083a0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000083b0: 7574 7075 745f 6c61 7965 7220 3d20 6766  utput_layer = gf
+000083c0: 6f2e 6765 745f 6465 6661 756c 745f 6c61  o.get_default_la
+000083d0: 7965 7228 6f75 7470 7574 5f70 6174 6829  yer(output_path)
+000083e0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000083f0: 7075 745f 746d 705f 7061 7468 203d 2074  put_tmp_path = t
+00008400: 656d 7064 6972 202f 2066 227b 6f75 7470  empdir / f"{outp
+00008410: 7574 5f70 6174 682e 7374 656d 7d2e 6770  ut_path.stem}.gp
+00008420: 6b67 220a 2020 2020 2020 2020 2020 2020  kg".            
+00008430: 7072 6576 5f6e 625f 6261 7463 6865 7320  prev_nb_batches 
+00008440: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00008450: 2020 206c 6173 745f 7061 7373 203d 2046     last_pass = F
+00008460: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00008470: 2070 6173 735f 6964 203d 2030 0a20 2020   pass_id = 0.   
+00008480: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00008490: 696e 666f 2866 2253 7461 7274 2064 6973  info(f"Start dis
+000084a0: 736f 6c76 6520 6f6e 2066 696c 6520 7b69  solve on file {i
+000084b0: 6e70 7574 5f70 6174 687d 2229 0a20 2020  nput_path}").   
+000084c0: 2020 2020 2020 2020 2077 6869 6c65 2054           while T
+000084d0: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
+000084e0: 2020 2020 2023 2047 6574 2069 6e66 6f20       # Get info 
+000084f0: 6f66 2074 6865 2063 7572 7265 6e74 2066  of the current f
+00008500: 696c 6520 7468 6174 206e 6565 6473 2074  ile that needs t
+00008510: 6f20 6265 2064 6973 736f 6c76 6564 0a20  o be dissolved. 
+00008520: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00008530: 6173 735f 696e 7075 745f 6c61 7965 7269  ass_input_layeri
+00008540: 6e66 6f20 3d20 6766 6f2e 6765 745f 6c61  nfo = gfo.get_la
+00008550: 7965 7269 6e66 6f28 696e 7075 745f 7061  yerinfo(input_pa
+00008560: 7468 2c20 696e 7075 745f 6c61 7965 7229  th, input_layer)
+00008570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008580: 206e 625f 726f 7773 5f74 6f74 616c 203d   nb_rows_total =
+00008590: 2070 6173 735f 696e 7075 745f 6c61 7965   pass_input_laye
+000085a0: 7269 6e66 6f2e 6665 6174 7572 6563 6f75  rinfo.featurecou
+000085b0: 6e74 0a0a 2020 2020 2020 2020 2020 2020  nt..            
+000085c0: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+000085d0: 7468 6520 6265 7374 206e 756d 6265 7220  the best number 
+000085e0: 6f66 2070 6172 616c 6c65 6c20 7072 6f63  of parallel proc
+000085f0: 6573 7365 7320 616e 6420 6261 7463 6865  esses and batche
+00008600: 7320 666f 720a 2020 2020 2020 2020 2020  s for.          
+00008610: 2020 2020 2020 2320 7468 6520 6176 6169        # the avai
+00008620: 6c61 626c 6520 7265 736f 7572 6365 7320  lable resources 
+00008630: 666f 7220 7468 6520 6375 7272 656e 7420  for the current 
+00008640: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00008650: 2020 2020 2069 6620 6261 7463 6873 697a       if batchsiz
+00008660: 6520 3e20 303a 0a20 2020 2020 2020 2020  e > 0:.         
+00008670: 2020 2020 2020 2020 2020 2070 6172 616c             paral
+00008680: 6c65 6c69 7a61 7469 6f6e 5f63 6f6e 6669  lelization_confi
+00008690: 6720 3d20 5061 7261 6c6c 656c 697a 6174  g = Parallelizat
+000086a0: 696f 6e43 6f6e 6669 6728 0a20 2020 2020  ionConfig(.     
+000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086c0: 2020 206d 696e 5f61 7667 5f72 6f77 735f     min_avg_rows_
+000086d0: 7065 725f 6261 7463 683d 696e 7428 6d61  per_batch=int(ma
+000086e0: 7468 2e63 6569 6c28 6261 7463 6873 697a  th.ceil(batchsiz
+000086f0: 6520 2f20 3229 292c 0a20 2020 2020 2020  e / 2)),.       
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 206d 6178 5f61 7667 5f72 6f77 735f 7065   max_avg_rows_pe
+00008720: 725f 6261 7463 683d 6261 7463 6873 697a  r_batch=batchsiz
+00008730: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00008740: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008750: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2020 2070 6172 616c 6c65 6c69 7a61 7469     parallelizati
+00008780: 6f6e 5f63 6f6e 6669 6720 3d20 5061 7261  on_config = Para
+00008790: 6c6c 656c 697a 6174 696f 6e43 6f6e 6669  llelizationConfi
+000087a0: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+000087b0: 2020 2020 6e62 5f70 6172 616c 6c65 6c2c      nb_parallel,
+000087c0: 206e 625f 6261 7463 6865 735f 7265 636f   nb_batches_reco
+000087d0: 6d6d 656e 6465 642c 205f 203d 2067 6574  mmended, _ = get
+000087e0: 5f70 6172 616c 6c65 6c69 7a61 7469 6f6e  _parallelization
+000087f0: 5f70 6172 616d 7328 0a20 2020 2020 2020  _params(.       
+00008800: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+00008810: 726f 7773 5f74 6f74 616c 3d6e 625f 726f  rows_total=nb_ro
+00008820: 7773 5f74 6f74 616c 2c0a 2020 2020 2020  ws_total,.      
+00008830: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+00008840: 5f70 6172 616c 6c65 6c3d 6e62 5f70 6172  _parallel=nb_par
+00008850: 616c 6c65 6c2c 0a20 2020 2020 2020 2020  allel,.         
+00008860: 2020 2020 2020 2020 2020 206e 625f 6261             nb_ba
+00008870: 7463 6865 735f 7072 6576 696f 7573 5f70  tches_previous_p
+00008880: 6173 733d 7072 6576 5f6e 625f 6261 7463  ass=prev_nb_batc
+00008890: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
+000088a0: 2020 2020 2020 2020 2070 6172 616c 6c65           paralle
+000088b0: 6c69 7a61 7469 6f6e 5f63 6f6e 6669 673d  lization_config=
+000088c0: 7061 7261 6c6c 656c 697a 6174 696f 6e5f  parallelization_
+000088d0: 636f 6e66 6967 2c0a 2020 2020 2020 2020  config,.        
+000088e0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000088f0: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+00008900: 7468 6520 6964 6561 6c20 6e75 6d62 6572  the ideal number
+00008910: 206f 6620 6261 7463 6865 7320 6973 2063   of batches is c
+00008920: 6c6f 7365 2074 6f20 7468 6520 6e62 2e20  lose to the nb. 
+00008930: 7265 7375 6c74 2074 696c 6573 2061 736b  result tiles ask
+00008940: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+00008950: 2020 2020 2320 6469 7373 6f6c 7665 2074      # dissolve t
+00008960: 6f77 6172 6473 2074 6865 2061 736b 6564  owards the asked
+00008970: 2072 6573 756c 7421 0a20 2020 2020 2020   result!.       
+00008980: 2020 2020 2020 2020 2023 2049 6620 6e6f           # If no
+00008990: 742c 2061 2074 656d 706f 7261 7279 2072  t, a temporary r
+000089a0: 6573 756c 7420 6973 2063 7265 6174 6564  esult is created
+000089b0: 2075 7369 6e67 2073 6d61 6c6c 6572 2074   using smaller t
+000089c0: 696c 6573 0a20 2020 2020 2020 2020 2020  iles.           
+000089d0: 2020 2020 2069 6620 6e62 5f62 6174 6368       if nb_batch
+000089e0: 6573 5f72 6563 6f6d 6d65 6e64 6564 203c  es_recommended <
+000089f0: 3d20 6c65 6e28 7265 7375 6c74 5f74 696c  = len(result_til
+00008a00: 6573 5f67 6466 2920 2a20 312e 313a 0a20  es_gdf) * 1.1:. 
 00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2072 6573 756c 745f 7469 6c65 735f 6764   result_tiles_gd
-00008a30: 662c 206e 625f 6261 7463 6865 735f 7265  f, nb_batches_re
-00008a40: 636f 6d6d 656e 6465 640a 2020 2020 2020  commended.      
-00008a50: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 6766 6f2e 746f 5f66 696c 6528 0a20 2020  gfo.to_file(.   
-00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a90: 2074 696c 6573 5f67 6466 2c20 7465 6d70   tiles_gdf, temp
-00008aa0: 6469 7220 2f20 6622 7b6f 7574 7075 745f  dir / f"{output_
-00008ab0: 7061 7468 2e73 7465 6d7d 5f7b 7061 7373  path.stem}_{pass
-00008ac0: 5f69 647d 5f74 696c 6573 2e67 706b 6722  _id}_tiles.gpkg"
-00008ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008ae0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00008af0: 2020 2020 2320 4966 2074 6865 206e 756d      # If the num
-00008b00: 6265 7220 6f66 2074 696c 6573 2065 6e64  ber of tiles end
-00008b10: 7320 7570 2061 7320 312c 2069 7420 6973  s up as 1, it is
-00008b20: 2074 6865 206c 6173 7420 7061 7373 2061   the last pass a
-00008b30: 6e79 7761 792e 2e2e 0a20 2020 2020 2020  nyway....       
-00008b40: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00008b50: 7469 6c65 735f 6764 6629 203d 3d20 313a  tiles_gdf) == 1:
-00008b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b70: 2020 2020 206c 6173 745f 7061 7373 203d       last_pass =
-00008b80: 2054 7275 650a 0a20 2020 2020 2020 2020   True..         
-00008b90: 2020 2020 2020 2023 2049 6620 7765 2061         # If we a
-00008ba0: 7265 206e 6f74 2069 6e20 7468 6520 6c61  re not in the la
-00008bb0: 7374 2070 6173 732c 206f 6e62 6f72 6465  st pass, onborde
-00008bc0: 7220 7061 7263 656c 7320 7769 6c6c 206e  r parcels will n
-00008bd0: 6565 6420 6578 7472 610a 2020 2020 2020  eed extra.      
-00008be0: 2020 2020 2020 2020 2020 2320 7072 6f63            # proc
-00008bf0: 6573 7369 6e67 2073 7469 6c6c 2069 6e20  essing still in 
-00008c00: 6675 7274 6865 7220 7061 7373 6573 2c20  further passes, 
-00008c10: 736f 2061 7265 2073 6176 6564 2069 6e20  so are saved in 
-00008c20: 6120 7365 7065 7261 7465 0a20 2020 2020  a seperate.     
-00008c30: 2020 2020 2020 2020 2020 2023 2067 666f             # gfo
-00008c40: 2e20 5468 6520 6e6f 746f 6e62 6f72 6465  . The notonborde
-00008c50: 7220 726f 7773 2061 7265 2066 696e 616c  r rows are final
-00008c60: 2069 6d6d 6564 6961 7465 6c79 0a20 2020   immediately.   
-00008c70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00008c80: 6c61 7374 5f70 6173 7320 6973 206e 6f74  last_pass is not
-00008c90: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
-00008ca0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00008cb0: 745f 746d 705f 6f6e 626f 7264 6572 5f70  t_tmp_onborder_p
-00008cc0: 6174 6820 3d20 280a 2020 2020 2020 2020  ath = (.        
-00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ce0: 7465 6d70 6469 7220 2f20 6622 7b6f 7574  tempdir / f"{out
-00008cf0: 7075 745f 7061 7468 2e73 7465 6d7d 5f7b  put_path.stem}_{
-00008d00: 7061 7373 5f69 647d 5f6f 6e62 6f72 6465  pass_id}_onborde
-00008d10: 722e 6770 6b67 220a 2020 2020 2020 2020  r.gpkg".        
-00008d20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00008d30: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00008d40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00008d50: 2020 2020 2020 2020 6f75 7470 7574 5f74          output_t
-00008d60: 6d70 5f6f 6e62 6f72 6465 725f 7061 7468  mp_onborder_path
-00008d70: 203d 206f 7574 7075 745f 746d 705f 7061   = output_tmp_pa
-00008d80: 7468 0a0a 2020 2020 2020 2020 2020 2020  th..            
-00008d90: 2020 2020 2320 4e6f 7720 676f 210a 2020      # Now go!.  
-00008da0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00008db0: 6767 6572 2e69 6e66 6f28 6622 5374 6172  gger.info(f"Star
-00008dc0: 7420 6469 7373 6f6c 7665 2070 6173 7320  t dissolve pass 
-00008dd0: 7b70 6173 735f 6964 7d20 746f 207b 6c65  {pass_id} to {le
-00008de0: 6e28 7469 6c65 735f 6764 6629 7d20 7469  n(tiles_gdf)} ti
-00008df0: 6c65 7322 290a 2020 2020 2020 2020 2020  les").          
-00008e00: 2020 2020 2020 5f20 3d20 5f64 6973 736f        _ = _disso
-00008e10: 6c76 655f 706f 6c79 676f 6e73 5f70 6173  lve_polygons_pas
-00008e20: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00008e30: 2020 2020 2020 2069 6e70 7574 5f70 6174         input_pat
-00008e40: 683d 696e 7075 745f 7061 7468 2c0a 2020  h=input_path,.  
+00008a20: 2020 2074 696c 6573 5f67 6466 203d 2072     tiles_gdf = r
+00008a30: 6573 756c 745f 7469 6c65 735f 6764 660a  esult_tiles_gdf.
+00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a50: 2020 2020 6c61 7374 5f70 6173 7320 3d20      last_pass = 
+00008a60: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00008a70: 2020 2020 2020 2020 206e 625f 7061 7261           nb_para
+00008a80: 6c6c 656c 203d 206d 696e 286c 656e 2872  llel = min(len(r
+00008a90: 6573 756c 745f 7469 6c65 735f 6764 6629  esult_tiles_gdf)
+00008aa0: 2c20 6e62 5f70 6172 616c 6c65 6c29 0a20  , nb_parallel). 
+00008ab0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00008ac0: 6c69 6620 6c65 6e28 7265 7375 6c74 5f74  lif len(result_t
+00008ad0: 696c 6573 5f67 6466 2920 3d3d 2031 3a0a  iles_gdf) == 1:.
+00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008af0: 2020 2020 2320 4372 6561 7465 2061 2067      # Create a g
+00008b00: 7269 6420 6261 7365 6420 6f6e 2074 6865  rid based on the
+00008b10: 2069 6465 616c 206e 756d 6265 7220 6f66   ideal number of
+00008b20: 2062 6174 6368 6573 2c20 6275 7420 6d61   batches, but ma
+00008b30: 6b65 0a20 2020 2020 2020 2020 2020 2020  ke.             
+00008b40: 2020 2020 2020 2023 2073 7572 6520 7468         # sure th
+00008b50: 6520 6e75 6d62 6572 2069 7320 736d 616c  e number is smal
+00008b60: 6c65 7220 7468 616e 2074 6865 206d 6178  ler than the max
+00008b70: 696d 756d 2e2e 2e0a 2020 2020 2020 2020  imum....        
+00008b80: 2020 2020 2020 2020 2020 2020 6e62 5f73              nb_s
+00008b90: 7175 6172 6973 685f 7469 6c65 735f 6d61  quarish_tiles_ma
+00008ba0: 7820 3d20 4e6f 6e65 0a20 2020 2020 2020  x = None.       
+00008bb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00008bc0: 7072 6576 5f6e 625f 6261 7463 6865 7320  prev_nb_batches 
+00008bd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bf0: 2020 2020 206e 625f 7371 7561 7269 7368       nb_squarish
+00008c00: 5f74 696c 6573 5f6d 6178 203d 206d 6178  _tiles_max = max
+00008c10: 2870 7265 765f 6e62 5f62 6174 6368 6573  (prev_nb_batches
+00008c20: 202d 2031 2c20 3129 0a20 2020 2020 2020   - 1, 1).       
+00008c30: 2020 2020 2020 2020 2020 2020 2074 696c               til
+00008c40: 6573 5f67 6466 203d 2067 7269 645f 7574  es_gdf = grid_ut
+00008c50: 696c 2e63 7265 6174 655f 6772 6964 3228  il.create_grid2(
+00008c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c70: 2020 2020 2020 2020 2074 6f74 616c 5f62           total_b
+00008c80: 6f75 6e64 733d 7061 7373 5f69 6e70 7574  ounds=pass_input
+00008c90: 5f6c 6179 6572 696e 666f 2e74 6f74 616c  _layerinfo.total
+00008ca0: 5f62 6f75 6e64 732c 0a20 2020 2020 2020  _bounds,.       
+00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cc0: 206e 625f 7371 7561 7269 7368 5f74 696c   nb_squarish_til
+00008cd0: 6573 3d6e 625f 6261 7463 6865 735f 7265  es=nb_batches_re
+00008ce0: 636f 6d6d 656e 6465 642c 0a20 2020 2020  commended,.     
+00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d00: 2020 206e 625f 7371 7561 7269 7368 5f74     nb_squarish_t
+00008d10: 696c 6573 5f6d 6178 3d6e 625f 7371 7561  iles_max=nb_squa
+00008d20: 7269 7368 5f74 696c 6573 5f6d 6178 2c0a  rish_tiles_max,.
+00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d40: 2020 2020 2020 2020 6372 733d 7061 7373          crs=pass
+00008d50: 5f69 6e70 7574 5f6c 6179 6572 696e 666f  _input_layerinfo
+00008d60: 2e63 7273 2c0a 2020 2020 2020 2020 2020  .crs,.          
+00008d70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00008d80: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00008d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008da0: 2020 2020 2020 2320 4966 2061 2067 7269        # If a gri
+00008db0: 6420 6973 2073 7065 6369 6669 6564 2061  d is specified a
+00008dc0: 6c72 6561 6479 2c20 6164 6420 6578 7472  lready, add extr
+00008dd0: 6120 636f 6c75 6d6e 732f 726f 7773 2069  a columns/rows i
+00008de0: 6e73 7465 6164 206f 660a 2020 2020 2020  nstead of.      
+00008df0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00008e00: 6372 6561 7469 6e67 206e 6577 206f 6e65  creating new one
+00008e10: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00008e20: 2020 2020 2020 2020 7469 6c65 735f 6764          tiles_gd
+00008e30: 6620 3d20 6772 6964 5f75 7469 6c2e 7370  f = grid_util.sp
+00008e40: 6c69 745f 7469 6c65 7328 0a20 2020 2020  lit_tiles(.     
 00008e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e60: 2020 6f75 7470 7574 5f6e 6f74 6f6e 626f    output_notonbo
-00008e70: 7264 6572 5f70 6174 683d 6f75 7470 7574  rder_path=output
-00008e80: 5f74 6d70 5f70 6174 682c 0a20 2020 2020  _tmp_path,.     
-00008e90: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00008ea0: 7574 7075 745f 6f6e 626f 7264 6572 5f70  utput_onborder_p
-00008eb0: 6174 683d 6f75 7470 7574 5f74 6d70 5f6f  ath=output_tmp_o
-00008ec0: 6e62 6f72 6465 725f 7061 7468 2c0a 2020  nborder_path,.  
-00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ee0: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
-00008ef0: 696f 6e73 3d65 7870 6c6f 6465 636f 6c6c  ions=explodecoll
-00008f00: 6563 7469 6f6e 732c 0a20 2020 2020 2020  ections,.       
-00008f10: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-00008f20: 7570 6279 5f63 6f6c 756d 6e73 3d67 726f  upby_columns=gro
-00008f30: 7570 6279 5f63 6f6c 756d 6e73 2c0a 2020  upby_columns,.  
-00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f50: 2020 6167 675f 636f 6c75 6d6e 733d 6167    agg_columns=ag
-00008f60: 675f 636f 6c75 6d6e 732c 0a20 2020 2020  g_columns,.     
-00008f70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00008f80: 696c 6573 5f67 6466 3d74 696c 6573 5f67  iles_gdf=tiles_g
-00008f90: 6466 2c0a 2020 2020 2020 2020 2020 2020  df,.            
-00008fa0: 2020 2020 2020 2020 696e 7075 745f 6c61          input_la
-00008fb0: 7965 723d 696e 7075 745f 6c61 7965 722c  yer=input_layer,
-00008fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008fd0: 2020 2020 206f 7574 7075 745f 6c61 7965       output_laye
-00008fe0: 723d 6f75 7470 7574 5f6c 6179 6572 2c0a  r=output_layer,.
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009000: 2020 2020 6e62 5f70 6172 616c 6c65 6c3d      nb_parallel=
-00009010: 6e62 5f70 6172 616c 6c65 6c2c 0a20 2020  nb_parallel,.   
-00009020: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009040: 2320 5072 6570 6172 6520 7468 6520 6e65  # Prepare the ne
-00009050: 7874 2070 6173 730a 2020 2020 2020 2020  xt pass.        
-00009060: 2020 2020 2020 2020 2320 5468 6520 696e          # The in
-00009070: 7075 7420 7061 7468 2069 7320 7468 6520  put path is the 
-00009080: 6f6e 626f 7264 6572 2066 696c 650a 2020  onborder file.  
-00009090: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000090a0: 6576 5f6e 625f 6261 7463 6865 7320 3d20  ev_nb_batches = 
-000090b0: 6c65 6e28 7469 6c65 735f 6764 6629 0a20  len(tiles_gdf). 
-000090c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000090d0: 6e70 7574 5f70 6174 6820 3d20 6f75 7470  nput_path = outp
-000090e0: 7574 5f74 6d70 5f6f 6e62 6f72 6465 725f  ut_tmp_onborder_
-000090f0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-00009100: 2020 2020 2070 6173 735f 6964 202b 3d20       pass_id += 
-00009110: 310a 0a20 2020 2020 2020 2020 2020 2020  1..             
-00009120: 2020 2023 2049 6620 7765 2061 7265 2072     # If we are r
-00009130: 6561 6479 2e2e 2e0a 2020 2020 2020 2020  eady....        
-00009140: 2020 2020 2020 2020 6966 206c 6173 745f          if last_
-00009150: 7061 7373 2069 7320 5472 7565 3a0a 2020  pass is True:.  
-00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 6272 6561 6b0a 0a20 2020 2020 2020    break..       
-00009180: 2020 2020 2023 2043 616c 6375 6c61 7469       # Calculati
-00009190: 6f6e 2072 6561 6479 2120 4e6f 7720 6669  on ready! Now fi
-000091a0: 6e61 6c69 7365 206f 7574 7075 7421 0a20  nalise output!. 
-000091b0: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
-000091c0: 7468 6572 6520 6973 2061 2072 6573 756c  there is a resul
-000091d0: 7420 6f6e 2062 6f72 6465 722c 2061 7070  t on border, app
-000091e0: 656e 6420 6974 2074 6f20 7468 6520 7265  end it to the re
-000091f0: 7374 0a20 2020 2020 2020 2020 2020 2069  st.            i
-00009200: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-00009210: 2020 2020 7374 7228 6f75 7470 7574 5f74      str(output_t
-00009220: 6d70 5f6f 6e62 6f72 6465 725f 7061 7468  mp_onborder_path
-00009230: 2920 213d 2073 7472 286f 7574 7075 745f  ) != str(output_
-00009240: 746d 705f 7061 7468 290a 2020 2020 2020  tmp_path).      
-00009250: 2020 2020 2020 2020 2020 616e 6420 6f75            and ou
-00009260: 7470 7574 5f74 6d70 5f6f 6e62 6f72 6465  tput_tmp_onborde
-00009270: 725f 7061 7468 2e65 7869 7374 7328 290a  r_path.exists().
-00009280: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-00009290: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-000092a0: 666f 2e61 7070 656e 645f 746f 280a 2020  fo.append_to(.  
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 6f75 7470 7574 5f74 6d70 5f6f 6e62    output_tmp_onb
-000092d0: 6f72 6465 725f 7061 7468 2c20 6f75 7470  order_path, outp
-000092e0: 7574 5f74 6d70 5f70 6174 682c 2064 7374  ut_tmp_path, dst
-000092f0: 5f6c 6179 6572 3d6f 7574 7075 745f 6c61  _layer=output_la
-00009300: 7965 720a 2020 2020 2020 2020 2020 2020  yer.            
-00009310: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00009320: 2020 2023 2049 6620 7468 6572 6520 6973     # If there is
-00009330: 2061 2072 6573 756c 742e 2e2e 0a20 2020   a result....   
-00009340: 2020 2020 2020 2020 2069 6620 6f75 7470           if outp
-00009350: 7574 5f74 6d70 5f70 6174 682e 6578 6973  ut_tmp_path.exis
-00009360: 7473 2829 3a0a 2020 2020 2020 2020 2020  ts():.          
-00009370: 2020 2020 2020 2320 4966 2074 696c 6564        # If tiled
-00009380: 206f 7574 7075 7420 6173 6b65 642c 2061   output asked, a
-00009390: 6464 2022 7469 6c65 5f69 6422 2074 6f20  dd "tile_id" to 
-000093a0: 6772 6f75 7062 795f 636f 6c75 6d6e 730a  groupby_columns.
+00008e60: 2020 2072 6573 756c 745f 7469 6c65 735f     result_tiles_
+00008e70: 6764 662c 206e 625f 6261 7463 6865 735f  gdf, nb_batches_
+00008e80: 7265 636f 6d6d 656e 6465 640a 2020 2020  recommended.    
+00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ea0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008eb0: 2020 6766 6f2e 746f 5f66 696c 6528 0a20    gfo.to_file(. 
+00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ed0: 2020 2074 696c 6573 5f67 6466 2c20 7465     tiles_gdf, te
+00008ee0: 6d70 6469 7220 2f20 6622 7b6f 7574 7075  mpdir / f"{outpu
+00008ef0: 745f 7061 7468 2e73 7465 6d7d 5f7b 7061  t_path.stem}_{pa
+00008f00: 7373 5f69 647d 5f74 696c 6573 2e67 706b  ss_id}_tiles.gpk
+00008f10: 6722 0a20 2020 2020 2020 2020 2020 2020  g".             
+00008f20: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00008f30: 2020 2020 2020 2320 4966 2074 6865 206e        # If the n
+00008f40: 756d 6265 7220 6f66 2074 696c 6573 2065  umber of tiles e
+00008f50: 6e64 7320 7570 2061 7320 312c 2069 7420  nds up as 1, it 
+00008f60: 6973 2074 6865 206c 6173 7420 7061 7373  is the last pass
+00008f70: 2061 6e79 7761 792e 2e2e 0a20 2020 2020   anyway....     
+00008f80: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00008f90: 6e28 7469 6c65 735f 6764 6629 203d 3d20  n(tiles_gdf) == 
+00008fa0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+00008fb0: 2020 2020 2020 206c 6173 745f 7061 7373         last_pass
+00008fc0: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
+00008fd0: 2020 2020 2020 2020 2023 2049 6620 7765           # If we
+00008fe0: 2061 7265 206e 6f74 2069 6e20 7468 6520   are not in the 
+00008ff0: 6c61 7374 2070 6173 732c 206f 6e62 6f72  last pass, onbor
+00009000: 6465 7220 7061 7263 656c 7320 7769 6c6c  der parcels will
+00009010: 206e 6565 6420 6578 7472 610a 2020 2020   need extra.    
+00009020: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00009030: 6f63 6573 7369 6e67 2073 7469 6c6c 2069  ocessing still i
+00009040: 6e20 6675 7274 6865 7220 7061 7373 6573  n further passes
+00009050: 2c20 736f 2061 7265 2073 6176 6564 2069  , so are saved i
+00009060: 6e20 6120 7365 7065 7261 7465 0a20 2020  n a seperate.   
+00009070: 2020 2020 2020 2020 2020 2020 2023 2067               # g
+00009080: 666f 2e20 5468 6520 6e6f 746f 6e62 6f72  fo. The notonbor
+00009090: 6465 7220 726f 7773 2061 7265 2066 696e  der rows are fin
+000090a0: 616c 2069 6d6d 6564 6961 7465 6c79 0a20  al immediately. 
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000090c0: 6620 6c61 7374 5f70 6173 7320 6973 206e  f last_pass is n
+000090d0: 6f74 2054 7275 653a 0a20 2020 2020 2020  ot True:.       
+000090e0: 2020 2020 2020 2020 2020 2020 206f 7574               out
+000090f0: 7075 745f 746d 705f 6f6e 626f 7264 6572  put_tmp_onborder
+00009100: 5f70 6174 6820 3d20 280a 2020 2020 2020  _path = (.      
+00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009120: 2020 7465 6d70 6469 7220 2f20 6622 7b6f    tempdir / f"{o
+00009130: 7574 7075 745f 7061 7468 2e73 7465 6d7d  utput_path.stem}
+00009140: 5f7b 7061 7373 5f69 647d 5f6f 6e62 6f72  _{pass_id}_onbor
+00009150: 6465 722e 6770 6b67 220a 2020 2020 2020  der.gpkg".      
+00009160: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009180: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009190: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+000091a0: 5f74 6d70 5f6f 6e62 6f72 6465 725f 7061  _tmp_onborder_pa
+000091b0: 7468 203d 206f 7574 7075 745f 746d 705f  th = output_tmp_
+000091c0: 7061 7468 0a0a 2020 2020 2020 2020 2020  path..          
+000091d0: 2020 2020 2020 2320 4e6f 7720 676f 210a        # Now go!.
+000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091f0: 6c6f 6767 6572 2e69 6e66 6f28 6622 5374  logger.info(f"St
+00009200: 6172 7420 6469 7373 6f6c 7665 2070 6173  art dissolve pas
+00009210: 7320 7b70 6173 735f 6964 7d20 746f 207b  s {pass_id} to {
+00009220: 6c65 6e28 7469 6c65 735f 6764 6629 7d20  len(tiles_gdf)} 
+00009230: 7469 6c65 7322 290a 2020 2020 2020 2020  tiles").        
+00009240: 2020 2020 2020 2020 5f20 3d20 5f64 6973          _ = _dis
+00009250: 736f 6c76 655f 706f 6c79 676f 6e73 5f70  solve_polygons_p
+00009260: 6173 7328 0a20 2020 2020 2020 2020 2020  ass(.           
+00009270: 2020 2020 2020 2020 2069 6e70 7574 5f70           input_p
+00009280: 6174 683d 696e 7075 745f 7061 7468 2c0a  ath=input_path,.
+00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092a0: 2020 2020 6f75 7470 7574 5f6e 6f74 6f6e      output_noton
+000092b0: 626f 7264 6572 5f70 6174 683d 6f75 7470  border_path=outp
+000092c0: 7574 5f74 6d70 5f70 6174 682c 0a20 2020  ut_tmp_path,.   
+000092d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092e0: 206f 7574 7075 745f 6f6e 626f 7264 6572   output_onborder
+000092f0: 5f70 6174 683d 6f75 7470 7574 5f74 6d70  _path=output_tmp
+00009300: 5f6f 6e62 6f72 6465 725f 7061 7468 2c0a  _onborder_path,.
+00009310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009320: 2020 2020 6578 706c 6f64 6563 6f6c 6c65      explodecolle
+00009330: 6374 696f 6e73 3d65 7870 6c6f 6465 636f  ctions=explodeco
+00009340: 6c6c 6563 7469 6f6e 732c 0a20 2020 2020  llections,.     
+00009350: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00009360: 726f 7570 6279 5f63 6f6c 756d 6e73 3d67  roupby_columns=g
+00009370: 726f 7570 6279 5f63 6f6c 756d 6e73 2c0a  roupby_columns,.
+00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 2020 2020 6167 675f 636f 6c75 6d6e 733d      agg_columns=
+000093a0: 6167 675f 636f 6c75 6d6e 732c 0a20 2020  agg_columns,.   
 000093b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093c0: 6966 206c 656e 2872 6573 756c 745f 7469  if len(result_ti
-000093d0: 6c65 735f 6764 6629 203e 2031 3a0a 2020  les_gdf) > 1:.  
-000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093f0: 2020 6966 2067 726f 7570 6279 5f63 6f6c    if groupby_col
-00009400: 756d 6e73 2069 7320 4e6f 6e65 3a0a 2020  umns is None:.  
-00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009420: 2020 2020 2020 6772 6f75 7062 795f 636f        groupby_co
-00009430: 6c75 6d6e 7320 3d20 5b22 7469 6c65 5f69  lumns = ["tile_i
-00009440: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
-00009450: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009470: 2020 2020 2020 6772 6f75 7062 795f 636f        groupby_co
-00009480: 6c75 6d6e 7320 3d20 6c69 7374 2867 726f  lumns = list(gro
-00009490: 7570 6279 5f63 6f6c 756d 6e73 292e 636f  upby_columns).co
-000094a0: 7079 2829 0a20 2020 2020 2020 2020 2020  py().           
-000094b0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-000094c0: 7570 6279 5f63 6f6c 756d 6e73 2e61 7070  upby_columns.app
-000094d0: 656e 6428 2274 696c 655f 6964 2229 0a0a  end("tile_id")..
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 2320 5072 6570 6172 6520 7374 7269 6e67  # Prepare string
-00009500: 7320 746f 2075 7365 2069 6e20 7365 6c65  s to use in sele
-00009510: 6374 2062 6173 6564 206f 6e20 6772 6f75  ct based on grou
-00009520: 7062 795f 636f 6c75 6d6e 730a 2020 2020  pby_columns.    
-00009530: 2020 2020 2020 2020 2020 2020 6966 2067              if g
-00009540: 726f 7570 6279 5f63 6f6c 756d 6e73 2069  roupby_columns i
-00009550: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 6772 6f75 7062 795f 7072 6566 6978 6564  groupby_prefixed
-00009580: 5f6c 6973 7420 3d20 5b0a 2020 2020 2020  _list = [.      
-00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 6627 7b7b 7072 6566 6978 7d7d 227b    f'{{prefix}}"{
-000095b0: 636f 6c75 6d6e 7d22 2720 666f 7220 636f  column}"' for co
-000095c0: 6c75 6d6e 2069 6e20 6772 6f75 7062 795f  lumn in groupby_
-000095d0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-000095e0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009600: 2020 6772 6f75 7062 795f 7365 6c65 6374    groupby_select
-00009610: 5f70 7265 6669 7865 645f 7374 7220 3d20  _prefixed_str = 
-00009620: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00009630: 2020 2020 2020 2020 2020 6622 2c20 7b27            f", {'
-00009640: 2c20 272e 6a6f 696e 2867 726f 7570 6279  , '.join(groupby
-00009650: 5f70 7265 6669 7865 645f 6c69 7374 297d  _prefixed_list)}
-00009660: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00009670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009680: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-00009690: 7062 795f 6772 6f75 7062 795f 7072 6566  pby_groupby_pref
-000096a0: 6978 6564 5f73 7472 203d 2028 0a20 2020  ixed_str = (.   
-000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096c0: 2020 2020 2066 2247 524f 5550 2042 5920       f"GROUP BY 
-000096d0: 7b27 2c20 272e 6a6f 696e 2867 726f 7570  {', '.join(group
-000096e0: 6279 5f70 7265 6669 7865 645f 6c69 7374  by_prefixed_list
-000096f0: 297d 220a 2020 2020 2020 2020 2020 2020  )}".            
-00009700: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00009710: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00009720: 726f 7570 6279 5f66 696c 7465 725f 6c69  roupby_filter_li
-00009730: 7374 203d 205b 0a20 2020 2020 2020 2020  st = [.         
-00009740: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00009750: 2720 414e 4420 6765 6f5f 6461 7461 2e22  ' AND geo_data."
-00009760: 7b63 6f6c 756d 6e7d 2220 3d20 6a73 6f6e  {column}" = json
-00009770: 5f64 6174 612e 227b 636f 6c75 6d6e 7d22  _data."{column}"
-00009780: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00009790: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-000097a0: 6c75 6d6e 2069 6e20 6772 6f75 7062 795f  lumn in groupby_
-000097b0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-000097c0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097e0: 2020 6772 6f75 7062 795f 6669 6c74 6572    groupby_filter
-000097f0: 5f73 7472 203d 2022 2022 2e6a 6f69 6e28  _str = " ".join(
-00009800: 6772 6f75 7062 795f 6669 6c74 6572 5f6c  groupby_filter_l
-00009810: 6973 7429 0a20 2020 2020 2020 2020 2020  ist).           
-00009820: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00009830: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00009840: 726f 7570 6279 5f73 656c 6563 745f 7072  roupby_select_pr
-00009850: 6566 6978 6564 5f73 7472 203d 2022 220a  efixed_str = "".
-00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009870: 2020 2020 6772 6f75 7062 795f 6772 6f75      groupby_grou
-00009880: 7062 795f 7072 6566 6978 6564 5f73 7472  pby_prefixed_str
-00009890: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
-000098a0: 2020 2020 2020 2020 2020 6772 6f75 7062            groupb
-000098b0: 795f 6669 6c74 6572 5f73 7472 203d 2022  y_filter_str = "
-000098c0: 220a 0a20 2020 2020 2020 2020 2020 2020  "..             
-000098d0: 2020 2023 2050 7265 7061 7265 2073 7472     # Prepare str
-000098e0: 696e 6773 2074 6f20 7573 6520 696e 2073  ings to use in s
-000098f0: 656c 6563 7420 6261 7365 6420 6f6e 2061  elect based on a
-00009900: 6767 5f63 6f6c 756d 6e73 0a20 2020 2020  gg_columns.     
-00009910: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
-00009920: 6f6c 756d 6e73 5f73 7472 203d 2022 220a  olumns_str = "".
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 6966 2061 6767 5f63 6f6c 756d 6e73 2069  if agg_columns i
-00009950: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009970: 6966 2022 6a73 6f6e 2220 696e 2061 6767  if "json" in agg
-00009980: 5f63 6f6c 756d 6e73 3a0a 2020 2020 2020  _columns:.      
-00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 2020 2320 5468 6520 6167 6772 6567 6174    # The aggregat
-000099b0: 696f 6e20 6973 2074 6f20 6120 6a73 6f6e  ion is to a json
-000099c0: 2063 6f6c 756d 6e2c 2073 6f20 6164 640a   column, so add.
-000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
-000099f0: 6d6e 735f 7374 7220 2b3d 2028 0a20 2020  mns_str += (.   
-00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a10: 2020 2020 2020 2020 2022 2c6a 736f 6e5f           ",json_
-00009a20: 6772 6f75 705f 6172 7261 7928 4449 5354  group_array(DIST
-00009a30: 494e 4354 206a 736f 6e5f 6461 7461 2e6a  INCT json_data.j
-00009a40: 736f 6e5f 726f 7729 2061 7320 6a73 6f6e  son_row) as json
-00009a50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00009a60: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 656c 6966 2022 636f 6c75 6d6e 7322 2069  elif "columns" i
-00009a90: 6e20 6167 675f 636f 6c75 6d6e 733a 0a20  n agg_columns:. 
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2066 6f72 2061 6767 5f63         for agg_c
-00009ac0: 6f6c 756d 6e20 696e 2061 6767 5f63 6f6c  olumn in agg_col
-00009ad0: 756d 6e73 5b22 636f 6c75 6d6e 7322 5d3a  umns["columns"]:
+000093c0: 2074 696c 6573 5f67 6466 3d74 696c 6573   tiles_gdf=tiles
+000093d0: 5f67 6466 2c0a 2020 2020 2020 2020 2020  _gdf,.          
+000093e0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+000093f0: 6c61 7965 723d 696e 7075 745f 6c61 7965  layer=input_laye
+00009400: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00009410: 2020 2020 2020 206f 7574 7075 745f 6c61         output_la
+00009420: 7965 723d 6f75 7470 7574 5f6c 6179 6572  yer=output_layer
+00009430: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009440: 2020 2020 2020 6772 6964 7369 7a65 3d67        gridsize=g
+00009450: 7269 6473 697a 652c 0a20 2020 2020 2020  ridsize,.       
+00009460: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+00009470: 7061 7261 6c6c 656c 3d6e 625f 7061 7261  parallel=nb_para
+00009480: 6c6c 656c 2c0a 2020 2020 2020 2020 2020  llel,.          
+00009490: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000094a0: 2020 2020 2020 2020 2023 2050 7265 7061           # Prepa
+000094b0: 7265 2074 6865 206e 6578 7420 7061 7373  re the next pass
+000094c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094d0: 2023 2054 6865 2069 6e70 7574 2070 6174   # The input pat
+000094e0: 6820 6973 2074 6865 206f 6e62 6f72 6465  h is the onborde
+000094f0: 7220 6669 6c65 0a20 2020 2020 2020 2020  r file.         
+00009500: 2020 2020 2020 2070 7265 765f 6e62 5f62         prev_nb_b
+00009510: 6174 6368 6573 203d 206c 656e 2874 696c  atches = len(til
+00009520: 6573 5f67 6466 290a 2020 2020 2020 2020  es_gdf).        
+00009530: 2020 2020 2020 2020 696e 7075 745f 7061          input_pa
+00009540: 7468 203d 206f 7574 7075 745f 746d 705f  th = output_tmp_
+00009550: 6f6e 626f 7264 6572 5f70 6174 680a 2020  onborder_path.  
+00009560: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00009570: 7373 5f69 6420 2b3d 2031 0a0a 2020 2020  ss_id += 1..    
+00009580: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00009590: 2077 6520 6172 6520 7265 6164 792e 2e2e   we are ready...
+000095a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000095b0: 2069 6620 6c61 7374 5f70 6173 7320 6973   if last_pass is
+000095c0: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
+000095d0: 2020 2020 2020 2020 2020 2062 7265 616b             break
+000095e0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000095f0: 4361 6c63 756c 6174 696f 6e20 7265 6164  Calculation read
+00009600: 7921 204e 6f77 2066 696e 616c 6973 6520  y! Now finalise 
+00009610: 6f75 7470 7574 210a 2020 2020 2020 2020  output!.        
+00009620: 2020 2020 2320 4966 2074 6865 7265 2069      # If there i
+00009630: 7320 6120 7265 7375 6c74 206f 6e20 626f  s a result on bo
+00009640: 7264 6572 2c20 6170 7065 6e64 2069 7420  rder, append it 
+00009650: 746f 2074 6865 2072 6573 740a 2020 2020  to the rest.    
+00009660: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+00009670: 2020 2020 2020 2020 2020 2020 2073 7472               str
+00009680: 286f 7574 7075 745f 746d 705f 6f6e 626f  (output_tmp_onbo
+00009690: 7264 6572 5f70 6174 6829 2021 3d20 7374  rder_path) != st
+000096a0: 7228 6f75 7470 7574 5f74 6d70 5f70 6174  r(output_tmp_pat
+000096b0: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+000096c0: 2020 2061 6e64 206f 7574 7075 745f 746d     and output_tm
+000096d0: 705f 6f6e 626f 7264 6572 5f70 6174 682e  p_onborder_path.
+000096e0: 6578 6973 7473 2829 0a20 2020 2020 2020  exists().       
+000096f0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00009700: 2020 2020 2020 2020 6766 6f2e 6170 7065          gfo.appe
+00009710: 6e64 5f74 6f28 0a20 2020 2020 2020 2020  nd_to(.         
+00009720: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00009730: 745f 746d 705f 6f6e 626f 7264 6572 5f70  t_tmp_onborder_p
+00009740: 6174 682c 206f 7574 7075 745f 746d 705f  ath, output_tmp_
+00009750: 7061 7468 2c20 6473 745f 6c61 7965 723d  path, dst_layer=
+00009760: 6f75 7470 7574 5f6c 6179 6572 0a20 2020  output_layer.   
+00009770: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00009780: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00009790: 2074 6865 7265 2069 7320 6120 7265 7375   there is a resu
+000097a0: 6c74 2e2e 2e0a 2020 2020 2020 2020 2020  lt....          
+000097b0: 2020 6966 206f 7574 7075 745f 746d 705f    if output_tmp_
+000097c0: 7061 7468 2e65 7869 7374 7328 293a 0a20  path.exists():. 
+000097d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000097e0: 2049 6620 7469 6c65 6420 6f75 7470 7574   If tiled output
+000097f0: 2061 736b 6564 2c20 6164 6420 2274 696c   asked, add "til
+00009800: 655f 6964 2220 746f 2067 726f 7570 6279  e_id" to groupby
+00009810: 5f63 6f6c 756d 6e73 0a20 2020 2020 2020  _columns.       
+00009820: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00009830: 7265 7375 6c74 5f74 696c 6573 5f67 6466  result_tiles_gdf
+00009840: 2920 3e20 313a 0a20 2020 2020 2020 2020  ) > 1:.         
+00009850: 2020 2020 2020 2020 2020 2069 6620 6772             if gr
+00009860: 6f75 7062 795f 636f 6c75 6d6e 7320 6973  oupby_columns is
+00009870: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00009880: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00009890: 726f 7570 6279 5f63 6f6c 756d 6e73 203d  roupby_columns =
+000098a0: 205b 2274 696c 655f 6964 225d 0a20 2020   ["tile_id"].   
+000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000098d0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+000098e0: 726f 7570 6279 5f63 6f6c 756d 6e73 203d  roupby_columns =
+000098f0: 206c 6973 7428 6772 6f75 7062 795f 636f   list(groupby_co
+00009900: 6c75 6d6e 7329 2e63 6f70 7928 290a 2020  lumns).copy().  
+00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 2020 6772 6f75 7062 795f 636f        groupby_co
+00009930: 6c75 6d6e 732e 6170 7065 6e64 2822 7469  lumns.append("ti
+00009940: 6c65 5f69 6422 290a 0a20 2020 2020 2020  le_id")..       
+00009950: 2020 2020 2020 2020 2023 2050 7265 7061           # Prepa
+00009960: 7265 2073 7472 696e 6773 2074 6f20 7573  re strings to us
+00009970: 6520 696e 2073 656c 6563 7420 6261 7365  e in select base
+00009980: 6420 6f6e 2067 726f 7570 6279 5f63 6f6c  d on groupby_col
+00009990: 756d 6e73 0a20 2020 2020 2020 2020 2020  umns.           
+000099a0: 2020 2020 2069 6620 6772 6f75 7062 795f       if groupby_
+000099b0: 636f 6c75 6d6e 7320 6973 206e 6f74 204e  columns is not N
+000099c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000099d0: 2020 2020 2020 2020 2067 726f 7570 6279           groupby
+000099e0: 5f70 7265 6669 7865 645f 6c69 7374 203d  _prefixed_list =
+000099f0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00009a00: 2020 2020 2020 2020 2020 2066 277b 7b70             f'{{p
+00009a10: 7265 6669 787d 7d22 7b63 6f6c 756d 6e7d  refix}}"{column}
+00009a20: 2227 2066 6f72 2063 6f6c 756d 6e20 696e  "' for column in
+00009a30: 2067 726f 7570 6279 5f63 6f6c 756d 6e73   groupby_columns
+00009a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a50: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+00009a60: 2020 2020 2020 2020 2020 2067 726f 7570             group
+00009a70: 6279 5f73 656c 6563 745f 7072 6566 6978  by_select_prefix
+00009a80: 6564 5f73 7472 203d 2028 0a20 2020 2020  ed_str = (.     
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2020 2066 222c 207b 272c 2027 2e6a 6f69     f", {', '.joi
+00009ab0: 6e28 6772 6f75 7062 795f 7072 6566 6978  n(groupby_prefix
+00009ac0: 6564 5f6c 6973 7429 7d22 0a20 2020 2020  ed_list)}".     
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
 00009ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009af0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-00009b00: 6e69 740a 2020 2020 2020 2020 2020 2020  nit.            
-00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b20: 6469 7374 696e 6374 5f73 7472 203d 2022  distinct_str = "
-00009b30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00009b40: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00009b50: 7472 615f 7061 7261 6d5f 7374 7220 3d20  tra_param_str = 
-00009b60: 2222 0a0a 2020 2020 2020 2020 2020 2020  ""..            
-00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b80: 2320 5072 6570 6172 6520 6167 6772 6567  # Prepare aggreg
-00009b90: 6174 696f 6e20 6b65 7977 6f72 642e 0a20  ation keyword.. 
+00009af0: 2020 2020 2067 726f 7570 6279 5f67 726f       groupby_gro
+00009b00: 7570 6279 5f70 7265 6669 7865 645f 7374  upby_prefixed_st
+00009b10: 7220 3d20 280a 2020 2020 2020 2020 2020  r = (.          
+00009b20: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00009b30: 4752 4f55 5020 4259 207b 272c 2027 2e6a  GROUP BY {', '.j
+00009b40: 6f69 6e28 6772 6f75 7062 795f 7072 6566  oin(groupby_pref
+00009b50: 6978 6564 5f6c 6973 7429 7d22 0a20 2020  ixed_list)}".   
+00009b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b70: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00009b80: 2020 2020 2020 2020 6772 6f75 7062 795f          groupby_
+00009b90: 6669 6c74 6572 5f6c 6973 7420 3d20 5b0a  filter_list = [.
 00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 2020 2020 2020 2020 2020 2069 6620 6167             if ag
-00009bc0: 675f 636f 6c75 6d6e 5b22 6167 6722 5d2e  g_column["agg"].
-00009bd0: 6c6f 7765 7228 2920 696e 205b 0a20 2020  lower() in [.   
-00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00009c00: 756e 7422 2c0a 2020 2020 2020 2020 2020  unt",.          
-00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c20: 2020 2020 2020 2273 756d 222c 0a20 2020        "sum",.   
-00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c40: 2020 2020 2020 2020 2020 2020 2022 6d69               "mi
-00009c50: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c70: 2020 2020 226d 6178 222c 0a20 2020 2020      "max",.     
-00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c90: 2020 2020 2020 2020 2020 2022 6d65 6469             "medi
-00009ca0: 616e 222c 0a20 2020 2020 2020 2020 2020  an",.           
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 205d 3a0a 2020 2020 2020 2020 2020 2020   ]:.            
-00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ce0: 2020 2020 6167 6772 6567 6174 696f 6e5f      aggregation_
-00009cf0: 7374 7220 3d20 6167 675f 636f 6c75 6d6e  str = agg_column
-00009d00: 5b22 6167 6722 5d0a 2020 2020 2020 2020  ["agg"].        
-00009d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d20: 2020 2020 656c 6966 2061 6767 5f63 6f6c      elif agg_col
-00009d30: 756d 6e5b 2261 6767 225d 2e6c 6f77 6572  umn["agg"].lower
-00009d40: 2829 2069 6e20 5b22 6d65 616e 222c 2022  () in ["mean", "
-00009d50: 6176 6722 5d3a 0a20 2020 2020 2020 2020  avg"]:.         
-00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d70: 2020 2020 2020 2061 6767 7265 6761 7469         aggregati
-00009d80: 6f6e 5f73 7472 203d 2022 6176 6722 0a20  on_str = "avg". 
-00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009da0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00009db0: 6167 675f 636f 6c75 6d6e 5b22 6167 6722  agg_column["agg"
-00009dc0: 5d2e 6c6f 7765 7228 2920 3d3d 2022 636f  ].lower() == "co
-00009dd0: 6e63 6174 223a 0a20 2020 2020 2020 2020  ncat":.         
-00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009df0: 2020 2020 2020 2061 6767 7265 6761 7469         aggregati
-00009e00: 6f6e 5f73 7472 203d 2022 6772 6f75 705f  on_str = "group_
-00009e10: 636f 6e63 6174 220a 2020 2020 2020 2020  concat".        
-00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e30: 2020 2020 2020 2020 6966 2022 7365 7022          if "sep"
-00009e40: 2069 6e20 6167 675f 636f 6c75 6d6e 3a0a   in agg_column:.
-00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e70: 2020 2020 6578 7472 615f 7061 7261 6d5f      extra_param_
-00009e80: 7374 7220 3d20 6622 2c20 277b 6167 675f  str = f", '{agg_
-00009e90: 636f 6c75 6d6e 5b27 7365 7027 5d7d 2722  column['sep']}'"
-00009ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009eb0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00009ec0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ee0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00009ef0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f10: 2020 2020 2020 2020 2066 2261 6767 7265           f"aggre
-00009f20: 6761 7469 6f6e 207b 6167 675f 636f 6c75  gation {agg_colu
-00009f30: 6d6e 5b27 6167 6727 5d7d 2069 7320 6e6f  mn['agg']} is no
-00009f40: 7420 7375 7070 6f72 7465 6422 0a20 2020  t supported".   
+00009bb0: 2020 2020 2020 2020 6627 2041 4e44 2067          f' AND g
+00009bc0: 656f 5f64 6174 612e 227b 636f 6c75 6d6e  eo_data."{column
+00009bd0: 7d22 203d 206a 736f 6e5f 6461 7461 2e22  }" = json_data."
+00009be0: 7b63 6f6c 756d 6e7d 2227 0a20 2020 2020  {column}"'.     
+00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c00: 2020 2066 6f72 2063 6f6c 756d 6e20 696e     for column in
+00009c10: 2067 726f 7570 6279 5f63 6f6c 756d 6e73   groupby_columns
+00009c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c30: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+00009c40: 2020 2020 2020 2020 2020 2067 726f 7570             group
+00009c50: 6279 5f66 696c 7465 725f 7374 7220 3d20  by_filter_str = 
+00009c60: 2220 222e 6a6f 696e 2867 726f 7570 6279  " ".join(groupby
+00009c70: 5f66 696c 7465 725f 6c69 7374 290a 2020  _filter_list).  
+00009c80: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00009c90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009ca0: 2020 2020 2020 2020 6772 6f75 7062 795f          groupby_
+00009cb0: 7365 6c65 6374 5f70 7265 6669 7865 645f  select_prefixed_
+00009cc0: 7374 7220 3d20 2222 0a20 2020 2020 2020  str = "".       
+00009cd0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
+00009ce0: 7570 6279 5f67 726f 7570 6279 5f70 7265  upby_groupby_pre
+00009cf0: 6669 7865 645f 7374 7220 3d20 2222 0a20  fixed_str = "". 
+00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d10: 2020 2067 726f 7570 6279 5f66 696c 7465     groupby_filte
+00009d20: 725f 7374 7220 3d20 2222 0a0a 2020 2020  r_str = ""..    
+00009d30: 2020 2020 2020 2020 2020 2020 2320 5072              # Pr
+00009d40: 6570 6172 6520 7374 7269 6e67 7320 746f  epare strings to
+00009d50: 2075 7365 2069 6e20 7365 6c65 6374 2062   use in select b
+00009d60: 6173 6564 206f 6e20 6167 675f 636f 6c75  ased on agg_colu
+00009d70: 6d6e 730a 2020 2020 2020 2020 2020 2020  mns.            
+00009d80: 2020 2020 6167 675f 636f 6c75 6d6e 735f      agg_columns_
+00009d90: 7374 7220 3d20 2222 0a20 2020 2020 2020  str = "".       
+00009da0: 2020 2020 2020 2020 2069 6620 6167 675f           if agg_
+00009db0: 636f 6c75 6d6e 7320 6973 206e 6f74 204e  columns is not N
+00009dc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00009dd0: 2020 2020 2020 2020 2069 6620 226a 736f           if "jso
+00009de0: 6e22 2069 6e20 6167 675f 636f 6c75 6d6e  n" in agg_column
+00009df0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00009e00: 2020 2020 2020 2020 2020 2023 2054 6865             # The
+00009e10: 2061 6767 7265 6761 7469 6f6e 2069 7320   aggregation is 
+00009e20: 746f 2061 206a 736f 6e20 636f 6c75 6d6e  to a json column
+00009e30: 2c20 736f 2061 6464 0a20 2020 2020 2020  , so add.       
+00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e50: 2061 6767 5f63 6f6c 756d 6e73 5f73 7472   agg_columns_str
+00009e60: 202b 3d20 280a 2020 2020 2020 2020 2020   += (.          
+00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e80: 2020 222c 6a73 6f6e 5f67 726f 7570 5f61    ",json_group_a
+00009e90: 7272 6179 2844 4953 5449 4e43 5420 6a73  rray(DISTINCT js
+00009ea0: 6f6e 5f64 6174 612e 6a73 6f6e 5f72 6f77  on_data.json_row
+00009eb0: 2920 6173 206a 736f 6e22 0a20 2020 2020  ) as json".     
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ed0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00009ee0: 2020 2020 2020 2020 2065 6c69 6620 2263           elif "c
+00009ef0: 6f6c 756d 6e73 2220 696e 2061 6767 5f63  olumns" in agg_c
+00009f00: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
+00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f20: 666f 7220 6167 675f 636f 6c75 6d6e 2069  for agg_column i
+00009f30: 6e20 6167 675f 636f 6c75 6d6e 735b 2263  n agg_columns["c
+00009f40: 6f6c 756d 6e73 225d 3a0a 2020 2020 2020  olumns"]:.      
 00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f60: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00009f60: 2020 2020 2020 2320 496e 6974 0a20 2020        # Init.   
 00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f80: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-00009f90: 2064 6973 7469 6e63 7420 6973 2073 7065   distinct is spe
-00009fa0: 6369 6669 6564 2c20 6164 6420 7468 6520  cified, add the 
-00009fb0: 6469 7374 696e 6374 206b 6579 776f 7264  distinct keyword
-00009fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009fd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009fe0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a000: 2020 2264 6973 7469 6e63 7422 2069 6e20    "distinct" in 
-0000a010: 6167 675f 636f 6c75 6d6e 0a20 2020 2020  agg_column.     
-0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a030: 2020 2020 2020 2020 2020 2061 6e64 2061             and a
-0000a040: 6767 5f63 6f6c 756d 6e5b 2264 6973 7469  gg_column["disti
-0000a050: 6e63 7422 5d20 6973 2054 7275 650a 2020  nct"] is True.  
-0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a070: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a090: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-0000a0a0: 7469 6e63 745f 7374 7220 3d20 2244 4953  tinct_str = "DIS
-0000a0b0: 5449 4e43 5420 220a 0a20 2020 2020 2020  TINCT "..       
+00009f80: 2020 2020 2020 2020 2064 6973 7469 6e63           distinc
+00009f90: 745f 7374 7220 3d20 2222 0a20 2020 2020  t_str = "".     
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 2020 2020 2020 2065 7874 7261 5f70 6172         extra_par
+00009fc0: 616d 5f73 7472 203d 2022 220a 0a20 2020  am_str = ""..   
+00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fe0: 2020 2020 2020 2020 2023 2050 7265 7061           # Prepa
+00009ff0: 7265 2061 6767 7265 6761 7469 6f6e 206b  re aggregation k
+0000a000: 6579 776f 7264 2e0a 2020 2020 2020 2020  eyword..        
+0000a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a020: 2020 2020 6966 2061 6767 5f63 6f6c 756d      if agg_colum
+0000a030: 6e5b 2261 6767 225d 2e6c 6f77 6572 2829  n["agg"].lower()
+0000a040: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
+0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a060: 2020 2020 2020 2263 6f75 6e74 222c 0a20        "count",. 
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a080: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000a090: 7375 6d22 2c0a 2020 2020 2020 2020 2020  sum",.          
+0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0b0: 2020 2020 2020 226d 696e 222c 0a20 2020        "min",.   
 0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0d0: 2020 2020 2023 2050 7265 7061 7265 2063       # Prepare c
-0000a0e0: 6f6c 756d 6e20 6e61 6d65 2073 7472 696e  olumn name strin
-0000a0f0: 672e 0a20 2020 2020 2020 2020 2020 2020  g..             
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000a110: 6f6c 756d 6e5f 7374 7220 3d20 280a 2020  olumn_str = (.  
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 2020 2020 2020 2020 2020 2020 2020 226a                "j
-0000a140: 736f 6e5f 6578 7472 6163 7428 6a73 6f6e  son_extract(json
-0000a150: 5f64 6174 612e 6a73 6f6e 5f72 6f77 2c20  _data.json_row, 
-0000a160: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 6627 2224 2e7b 6167 675f 636f 6c75    f'"$.{agg_colu
-0000a190: 6d6e 5b22 636f 6c75 6d6e 225d 7d22 2927  mn["column"]}")'
-0000a1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a1b0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+0000a0d0: 2020 2020 2020 2020 2020 2020 2022 6d61               "ma
+0000a0e0: 7822 2c0a 2020 2020 2020 2020 2020 2020  x",.            
+0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a100: 2020 2020 226d 6564 6961 6e22 2c0a 2020      "median",.  
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a120: 2020 2020 2020 2020 2020 5d3a 0a20 2020            ]:.   
+0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a140: 2020 2020 2020 2020 2020 2020 2061 6767               agg
+0000a150: 7265 6761 7469 6f6e 5f73 7472 203d 2061  regation_str = a
+0000a160: 6767 5f63 6f6c 756d 6e5b 2261 6767 225d  gg_column["agg"]
+0000a170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a180: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000a190: 6620 6167 675f 636f 6c75 6d6e 5b22 6167  f agg_column["ag
+0000a1a0: 6722 5d2e 6c6f 7765 7228 2920 696e 205b  g"].lower() in [
+0000a1b0: 226d 6561 6e22 2c20 2261 7667 225d 3a0a  "mean", "avg"]:.
 0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1d0: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
-0000a1e0: 7720 7075 7420 6576 6572 7974 6869 6e67  w put everything
-0000a1f0: 2074 6f67 6574 6865 720a 2020 2020 2020   together.      
+0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1e0: 6167 6772 6567 6174 696f 6e5f 7374 7220  aggregation_str 
+0000a1f0: 3d20 2261 7667 220a 2020 2020 2020 2020  = "avg".        
 0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a210: 2020 2020 2020 6167 675f 636f 6c75 6d6e        agg_column
-0000a220: 735f 7374 7220 2b3d 2028 0a20 2020 2020  s_str += (.     
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2020 2020 2020 2020 2020 2066 222c 207b             f", {
-0000a250: 6167 6772 6567 6174 696f 6e5f 7374 727d  aggregation_str}
-0000a260: 287b 6469 7374 696e 6374 5f73 7472 7d7b  ({distinct_str}{
-0000a270: 636f 6c75 6d6e 5f73 7472 7d22 0a20 2020  column_str}".   
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
-0000a2a0: 6578 7472 615f 7061 7261 6d5f 7374 727d  extra_param_str}
-0000a2b0: 2920 4153 2022 7b61 6767 5f63 6f6c 756d  ) AS "{agg_colum
-0000a2c0: 6e5b 2261 7322 5d7d 2227 0a20 2020 2020  n["as"]}"'.     
-0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000a2f0: 2020 2020 2020 2020 2020 2320 4164 6420            # Add 
-0000a300: 6120 636f 6c75 6d6e 2074 6f20 6f72 6465  a column to orde
-0000a310: 7220 7468 6520 7265 7375 6c74 2062 7920  r the result by 
-0000a320: 746f 2065 7661 6465 2068 6176 696e 6720  to evade having 
-0000a330: 616c 6c0a 2020 2020 2020 2020 2020 2020  all.            
-0000a340: 2020 2020 2320 636f 6d70 6c65 7820 6765      # complex ge
-0000a350: 6f6d 6574 7269 6573 2074 6f67 6574 6865  ometries togethe
-0000a360: 7220 696e 2074 6865 206f 7574 7075 7420  r in the output 
-0000a370: 6669 6c65 2e0a 2020 2020 2020 2020 2020  file..          
-0000a380: 2020 2020 2020 6f72 6465 7262 795f 636f        orderby_co
-0000a390: 6c75 6d6e 203d 2022 7465 6d70 5f6f 7264  lumn = "temp_ord
-0000a3a0: 6572 636f 6c75 6d6e 5f67 656f 6861 7368  ercolumn_geohash
-0000a3b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000a3c0: 2020 5f61 6464 5f6f 7264 6572 6279 5f63    _add_orderby_c
-0000a3d0: 6f6c 756d 6e28 0a20 2020 2020 2020 2020  olumn(.         
-0000a3e0: 2020 2020 2020 2020 2020 2070 6174 683d             path=
-0000a3f0: 6f75 7470 7574 5f74 6d70 5f70 6174 682c  output_tmp_path,
-0000a400: 206c 6179 6572 3d6f 7574 7075 745f 6c61   layer=output_la
-0000a410: 7965 722c 206e 616d 653d 6f72 6465 7262  yer, name=orderb
-0000a420: 795f 636f 6c75 6d6e 0a20 2020 2020 2020  y_column.       
-0000a430: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000a440: 2020 2020 2020 2020 2020 2020 2320 5072              # Pr
-0000a450: 6570 6172 6520 5351 4c20 7374 6174 656d  epare SQL statem
-0000a460: 656e 7420 666f 7220 6669 6e61 6c20 6f75  ent for final ou
-0000a470: 7470 7574 2066 696c 652e 0a20 2020 2020  tput file..     
-0000a480: 2020 2020 2020 2020 2020 2023 2041 6c6c             # All
-0000a490: 2074 696c 6573 2061 7265 2061 6c72 6561   tiles are alrea
-0000a4a0: 6479 2064 6973 736f 6c76 6564 2074 6f20  dy dissolved to 
-0000a4b0: 6772 6f75 7073 2c20 6275 7420 6e6f 7720  groups, but now 
-0000a4c0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-0000a4d0: 2020 2020 2320 7265 7375 6c74 7320 6672      # results fr
-0000a4e0: 6f6d 2061 6c6c 2074 696c 6573 2073 7469  om all tiles sti
-0000a4f0: 6c6c 206e 6565 6420 746f 2062 650a 2020  ll need to be.  
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000a510: 6772 6f75 7065 642f 636f 6c6c 6563 7465  grouped/collecte
-0000a520: 6420 746f 6765 7468 6572 2e0a 2020 2020  d together..    
-0000a530: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000a540: 6572 2e69 6e66 6f28 2250 6f73 7470 726f  er.info("Postpro
-0000a550: 6365 7373 2070 7265 7061 7265 6420 6665  cess prepared fe
-0000a560: 6174 7572 6573 2e2e 2e22 290a 2020 2020  atures...").    
-0000a570: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0000a580: 6767 5f63 6f6c 756d 6e73 2069 7320 4e6f  gg_columns is No
-0000a590: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a5a0: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
-0000a5b0: 7265 2061 7265 206e 6f20 6167 6772 6567  re are no aggreg
-0000a5c0: 6174 696f 6e20 636f 6c75 6d6e 732c 2074  ation columns, t
-0000a5d0: 6869 6e67 7320 6172 6520 6e6f 7420 746f  hings are not to
-0000a5e0: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
-0000a5f0: 2020 2020 2020 2320 636f 6d70 6c69 6361        # complica
-0000a600: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
-0000a610: 2020 2020 2020 2020 2069 6620 6578 706c           if expl
-0000a620: 6f64 6563 6f6c 6c65 6374 696f 6e73 2069  odecollections i
-0000a630: 7320 5472 7565 3a0a 2020 2020 2020 2020  s True:.        
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a650: 2320 4966 2065 7870 6c6f 6465 636f 6c6c  # If explodecoll
-0000a660: 6563 7469 6f6e 7320 6973 2074 7275 652c  ections is true,
-0000a670: 2069 7420 6973 2075 7365 6c65 7373 2074   it is useless t
-0000a680: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
-0000a690: 2020 2020 2020 2020 2020 2320 6669 7273            # firs
-0000a6a0: 7420 6772 6f75 7020 7468 656d 2068 6572  t group them her
-0000a6b0: 652c 2061 7320 7468 6579 2077 696c 6c20  e, as they will 
-0000a6c0: 6265 2065 7870 6c6f 6465 6420 6167 6169  be exploded agai
-0000a6d0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000a6e0: 2020 2020 2020 2020 2020 2320 696e 2074            # in t
-0000a6f0: 6865 2073 656c 6563 7428 2920 6361 6c6c  he select() call
-0000a700: 206c 6174 6572 206f 6e2e 2e2e 2073 6f20   later on... so 
-0000a710: 6a75 7374 206f 7264 6572 2074 6865 6d2e  just order them.
-0000a720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a730: 2020 2020 2020 2020 2023 2049 6620 6120           # If a 
-0000a740: 7469 6c65 6420 7265 7375 6c74 2069 7320  tiled result is 
-0000a750: 6173 6b65 642c 2061 6c73 6f20 646f 6e27  asked, also don'
-0000a760: 7420 636f 6c6c 6563 742e 0a20 2020 2020  t collect..     
-0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a780: 2020 2073 716c 5f73 746d 7420 3d20 6622     sql_stmt = f"
-0000a790: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
-0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000a7b0: 454c 4543 5420 7b7b 6765 6f6d 6574 7279  ELECT {{geometry
-0000a7c0: 636f 6c75 6d6e 7d7d 0a20 2020 2020 2020  column}}.       
-0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7e0: 2020 2020 2020 2020 2020 207b 6772 6f75             {grou
-0000a7f0: 7062 795f 7365 6c65 6374 5f70 7265 6669  pby_select_prefi
-0000a800: 7865 645f 7374 722e 666f 726d 6174 2870  xed_str.format(p
-0000a810: 7265 6669 783d 226c 6179 6572 2e22 297d  refix="layer.")}
-0000a820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-0000a840: 524f 4d20 227b 7b69 6e70 7574 5f6c 6179  ROM "{{input_lay
-0000a850: 6572 7d7d 2220 6c61 7965 720a 2020 2020  er}}" layer.    
-0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a870: 2020 2020 2020 2020 204f 5244 4552 2042           ORDER B
-0000a880: 5920 6c61 7965 722e 7b6f 7264 6572 6279  Y layer.{orderby
-0000a890: 5f63 6f6c 756d 6e7d 0a20 2020 2020 2020  _column}.       
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8b0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
-0000a8c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 2020 2020 2020 2023 204e 6f20 6578 706c         # No expl
-0000a8f0: 6f64 6563 6f6c 6c65 6374 696f 6e73 2c20  odecollections, 
-0000a900: 736f 2063 6f6c 6c65 6374 2074 6f20 6f6e  so collect to on
-0000a910: 6520 6765 6f6d 6574 7279 0a20 2020 2020  e geometry.     
-0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a930: 2020 2023 2028 7065 7220 6772 6f75 7062     # (per groupb
-0000a940: 7920 6966 2061 7070 6c69 6361 626c 6529  y if applicable)
-0000a950: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a960: 2020 2020 2020 2020 2020 7371 6c5f 7374            sql_st
-0000a970: 6d74 203d 2066 2222 220a 2020 2020 2020  mt = f""".      
-0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a990: 2020 2020 2020 5345 4c45 4354 2053 545f        SELECT ST_
-0000a9a0: 436f 6c6c 6563 7428 7b7b 6765 6f6d 6574  Collect({{geomet
-0000a9b0: 7279 636f 6c75 6d6e 7d7d 2920 4153 207b  rycolumn}}) AS {
-0000a9c0: 7b67 656f 6d65 7472 7963 6f6c 756d 6e7d  {geometrycolumn}
-0000a9d0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9f0: 2020 2020 7b67 726f 7570 6279 5f73 656c      {groupby_sel
-0000aa00: 6563 745f 7072 6566 6978 6564 5f73 7472  ect_prefixed_str
-0000aa10: 2e66 6f72 6d61 7428 7072 6566 6978 3d22  .format(prefix="
-0000aa20: 6c61 7965 722e 2229 7d0a 2020 2020 2020  layer.")}.      
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa40: 2020 2020 2020 2020 4652 4f4d 2022 7b7b          FROM "{{
-0000aa50: 696e 7075 745f 6c61 7965 727d 7d22 206c  input_layer}}" l
-0000aa60: 6179 6572 0a20 2020 2020 2020 2020 2020  ayer.           
+0000a210: 2020 2020 656c 6966 2061 6767 5f63 6f6c      elif agg_col
+0000a220: 756d 6e5b 2261 6767 225d 2e6c 6f77 6572  umn["agg"].lower
+0000a230: 2829 203d 3d20 2263 6f6e 6361 7422 3a0a  () == "concat":.
+0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 6167 6772 6567 6174 696f 6e5f 7374 7220  aggregation_str 
+0000a270: 3d20 2267 726f 7570 5f63 6f6e 6361 7422  = "group_concat"
+0000a280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2a0: 2069 6620 2273 6570 2220 696e 2061 6767   if "sep" in agg
+0000a2b0: 5f63 6f6c 756d 6e3a 0a20 2020 2020 2020  _column:.       
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 2020 2020 2020 2020 2020 2065 7874               ext
+0000a2e0: 7261 5f70 6172 616d 5f73 7472 203d 2066  ra_param_str = f
+0000a2f0: 222c 2027 7b61 6767 5f63 6f6c 756d 6e5b  ", '{agg_column[
+0000a300: 2773 6570 275d 7d27 220a 2020 2020 2020  'sep']}'".      
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000a350: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a380: 2020 6622 6167 6772 6567 6174 696f 6e20    f"aggregation 
+0000a390: 7b61 6767 5f63 6f6c 756d 6e5b 2761 6767  {agg_column['agg
+0000a3a0: 275d 7d20 6973 206e 6f74 2073 7570 706f  ']} is not suppo
+0000a3b0: 7274 6564 220a 2020 2020 2020 2020 2020  rted".          
+0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3f0: 2020 2020 2023 2049 6620 6469 7374 696e       # If distin
+0000a400: 6374 2069 7320 7370 6563 6966 6965 642c  ct is specified,
+0000a410: 2061 6464 2074 6865 2064 6973 7469 6e63   add the distinc
+0000a420: 7420 6b65 7977 6f72 640a 2020 2020 2020  t keyword.      
+0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a440: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a460: 2020 2020 2020 2020 2020 2022 6469 7374             "dist
+0000a470: 696e 6374 2220 696e 2061 6767 5f63 6f6c  inct" in agg_col
+0000a480: 756d 6e0a 2020 2020 2020 2020 2020 2020  umn.            
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 616e 6420 6167 675f 636f 6c75      and agg_colu
+0000a4b0: 6d6e 5b22 6469 7374 696e 6374 225d 2069  mn["distinct"] i
+0000a4c0: 7320 5472 7565 0a20 2020 2020 2020 2020  s True.         
+0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4e0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a500: 2020 2020 2020 6469 7374 696e 6374 5f73        distinct_s
+0000a510: 7472 203d 2022 4449 5354 494e 4354 2022  tr = "DISTINCT "
+0000a520: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000a540: 5072 6570 6172 6520 636f 6c75 6d6e 206e  Prepare column n
+0000a550: 616d 6520 7374 7269 6e67 2e0a 2020 2020  ame string..    
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2020 2020 2020 636f 6c75 6d6e 5f73          column_s
+0000a580: 7472 203d 2028 0a20 2020 2020 2020 2020  tr = (.         
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5a0: 2020 2020 2020 2022 6a73 6f6e 5f65 7874         "json_ext
+0000a5b0: 7261 6374 286a 736f 6e5f 6461 7461 2e6a  ract(json_data.j
+0000a5c0: 736f 6e5f 726f 772c 2022 0a20 2020 2020  son_row, ".     
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 2020 2020 2020 2020 2020 2066 2722 242e             f'"$.
+0000a5f0: 7b61 6767 5f63 6f6c 756d 6e5b 2263 6f6c  {agg_column["col
+0000a600: 756d 6e22 5d7d 2229 270a 2020 2020 2020  umn"]}")'.      
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a620: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2020 2023 204e 6f77 2070 7574 2065       # Now put e
+0000a650: 7665 7279 7468 696e 6720 746f 6765 7468  verything togeth
+0000a660: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000a680: 6767 5f63 6f6c 756d 6e73 5f73 7472 202b  gg_columns_str +
+0000a690: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6b0: 2020 2020 6622 2c20 7b61 6767 7265 6761      f", {aggrega
+0000a6c0: 7469 6f6e 5f73 7472 7d28 7b64 6973 7469  tion_str}({disti
+0000a6d0: 6e63 745f 7374 727d 7b63 6f6c 756d 6e5f  nct_str}{column_
+0000a6e0: 7374 727d 220a 2020 2020 2020 2020 2020  str}".          
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2020 2020 6627 7b65 7874 7261 5f70        f'{extra_p
+0000a710: 6172 616d 5f73 7472 7d29 2041 5320 227b  aram_str}) AS "{
+0000a720: 6167 675f 636f 6c75 6d6e 5b22 6173 225d  agg_column["as"]
+0000a730: 7d22 270a 2020 2020 2020 2020 2020 2020  }"'.            
+0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a750: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a760: 2020 2023 2041 6464 2061 2063 6f6c 756d     # Add a colum
+0000a770: 6e20 746f 206f 7264 6572 2074 6865 2072  n to order the r
+0000a780: 6573 756c 7420 6279 2074 6f20 6576 6164  esult by to evad
+0000a790: 6520 6861 7669 6e67 2061 6c6c 0a20 2020  e having all.   
+0000a7a0: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+0000a7b0: 6f6d 706c 6578 2067 656f 6d65 7472 6965  omplex geometrie
+0000a7c0: 7320 746f 6765 7468 6572 2069 6e20 7468  s together in th
+0000a7d0: 6520 6f75 7470 7574 2066 696c 652e 0a20  e output file.. 
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000a7f0: 7264 6572 6279 5f63 6f6c 756d 6e20 3d20  rderby_column = 
+0000a800: 2274 656d 705f 6f72 6465 7263 6f6c 756d  "temp_ordercolum
+0000a810: 6e5f 6765 6f68 6173 6822 0a20 2020 2020  n_geohash".     
+0000a820: 2020 2020 2020 2020 2020 205f 6164 645f             _add_
+0000a830: 6f72 6465 7262 795f 636f 6c75 6d6e 280a  orderby_column(.
+0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a850: 2020 2020 7061 7468 3d6f 7574 7075 745f      path=output_
+0000a860: 746d 705f 7061 7468 2c20 6c61 7965 723d  tmp_path, layer=
+0000a870: 6f75 7470 7574 5f6c 6179 6572 2c20 6e61  output_layer, na
+0000a880: 6d65 3d6f 7264 6572 6279 5f63 6f6c 756d  me=orderby_colum
+0000a890: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0000a8a0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0000a8b0: 2020 2020 2023 2050 7265 7061 7265 2053       # Prepare S
+0000a8c0: 514c 2073 7461 7465 6d65 6e74 2066 6f72  QL statement for
+0000a8d0: 2066 696e 616c 206f 7574 7075 7420 6669   final output fi
+0000a8e0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+0000a8f0: 2020 2020 2320 416c 6c20 7469 6c65 7320      # All tiles 
+0000a900: 6172 6520 616c 7265 6164 7920 6469 7373  are already diss
+0000a910: 6f6c 7665 6420 746f 2067 726f 7570 732c  olved to groups,
+0000a920: 2062 7574 206e 6f77 2074 6865 0a20 2020   but now the.   
+0000a930: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+0000a940: 6573 756c 7473 2066 726f 6d20 616c 6c20  esults from all 
+0000a950: 7469 6c65 7320 7374 696c 6c20 6e65 6564  tiles still need
+0000a960: 2074 6f20 6265 0a20 2020 2020 2020 2020   to be.         
+0000a970: 2020 2020 2020 2023 2067 726f 7570 6564         # grouped
+0000a980: 2f63 6f6c 6c65 6374 6564 2074 6f67 6574  /collected toget
+0000a990: 6865 722e 0a20 2020 2020 2020 2020 2020  her..           
+0000a9a0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0000a9b0: 2822 506f 7374 7072 6f63 6573 7320 7072  ("Postprocess pr
+0000a9c0: 6570 6172 6564 2066 6561 7475 7265 732e  epared features.
+0000a9d0: 2e2e 2229 0a20 2020 2020 2020 2020 2020  ..").           
+0000a9e0: 2020 2020 2069 6620 6167 675f 636f 6c75       if agg_colu
+0000a9f0: 6d6e 7320 6973 204e 6f6e 653a 0a20 2020  mns is None:.   
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2023 2049 6620 7468 6572 6520 6172 6520   # If there are 
+0000aa20: 6e6f 2061 6767 7265 6761 7469 6f6e 2063  no aggregation c
+0000aa30: 6f6c 756d 6e73 2c20 7468 696e 6773 2061  olumns, things a
+0000aa40: 7265 206e 6f74 2074 6f6f 0a20 2020 2020  re not too.     
+0000aa50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000aa60: 2063 6f6d 706c 6963 6174 6564 2e0a 2020   complicated..  
 0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa80: 2020 207b 6772 6f75 7062 795f 6772 6f75     {groupby_grou
-0000aa90: 7062 795f 7072 6566 6978 6564 5f73 7472  pby_prefixed_str
-0000aaa0: 2e66 6f72 6d61 7428 7072 6566 6978 3d22  .format(prefix="
-0000aab0: 6c61 7965 722e 2229 7d0a 2020 2020 2020  layer.")}.      
-0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aad0: 2020 2020 2020 204f 5244 4552 2042 5920         ORDER BY 
-0000aae0: 4d49 4e28 6c61 7965 722e 7b6f 7264 6572  MIN(layer.{order
-0000aaf0: 6279 5f63 6f6c 756d 6e7d 290a 2020 2020  by_column}).    
-0000ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ab20: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2020 2320 4966 2061 6767 5f63 6f6c 756d    # If agg_colum
-0000ab50: 6e73 2073 7065 6369 6669 6564 2c20 706f  ns specified, po
-0000ab60: 7374 7072 6f63 6573 7369 6e67 2069 7320  stprocessing is 
-0000ab70: 6120 6269 7420 6d6f 7265 0a20 2020 2020  a bit more.     
-0000ab80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ab90: 2063 6f6d 706c 6963 6174 6564 2e0a 2020   complicated..  
-0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2020 7371 6c5f 7374 6d74 203d 2066 2222    sql_stmt = f""
-0000abc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000abd0: 2020 2020 2020 2020 2020 5345 4c45 4354            SELECT
-0000abe0: 2067 656f 5f64 6174 612e 7b7b 6765 6f6d   geo_data.{{geom
-0000abf0: 6574 7279 636f 6c75 6d6e 7d7d 0a20 2020  etrycolumn}}.   
+0000aa80: 2020 6966 2065 7870 6c6f 6465 636f 6c6c    if explodecoll
+0000aa90: 6563 7469 6f6e 7320 6973 2054 7275 653a  ections is True:
+0000aaa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aab0: 2020 2020 2020 2020 2023 2049 6620 6578           # If ex
+0000aac0: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
+0000aad0: 2069 7320 7472 7565 2c20 6974 2069 7320   is true, it is 
+0000aae0: 7573 656c 6573 7320 746f 0a20 2020 2020  useless to.     
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab00: 2020 2023 2066 6972 7374 2067 726f 7570     # first group
+0000ab10: 2074 6865 6d20 6865 7265 2c20 6173 2074   them here, as t
+0000ab20: 6865 7920 7769 6c6c 2062 6520 6578 706c  hey will be expl
+0000ab30: 6f64 6564 2061 6761 696e 0a20 2020 2020  oded again.     
+0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab50: 2020 2023 2069 6e20 7468 6520 7365 6c65     # in the sele
+0000ab60: 6374 2829 2063 616c 6c20 6c61 7465 7220  ct() call later 
+0000ab70: 6f6e 2e2e 2e20 736f 206a 7573 7420 6f72  on... so just or
+0000ab80: 6465 7220 7468 656d 2e0a 2020 2020 2020  der them..      
+0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aba0: 2020 2320 4966 2061 2074 696c 6564 2072    # If a tiled r
+0000abb0: 6573 756c 7420 6973 2061 736b 6564 2c20  esult is asked, 
+0000abc0: 616c 736f 2064 6f6e 2774 2063 6f6c 6c65  also don't colle
+0000abd0: 6374 2e0a 2020 2020 2020 2020 2020 2020  ct..            
+0000abe0: 2020 2020 2020 2020 2020 2020 7371 6c5f              sql_
+0000abf0: 7374 6d74 203d 2066 2222 220a 2020 2020  stmt = f""".    
 0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 2020 2020 2020 2020 2020 207b 6772 6f75             {grou
-0000ac20: 7062 795f 7365 6c65 6374 5f70 7265 6669  pby_select_prefi
-0000ac30: 7865 645f 7374 722e 666f 726d 6174 2870  xed_str.format(p
-0000ac40: 7265 6669 783d 2267 656f 5f64 6174 612e  refix="geo_data.
-0000ac50: 2229 7d0a 2020 2020 2020 2020 2020 2020  ")}.            
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac70: 2020 7b61 6767 5f63 6f6c 756d 6e73 5f73    {agg_columns_s
-0000ac80: 7472 7d0a 2020 2020 2020 2020 2020 2020  tr}.            
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 4652                FR
-0000aca0: 4f4d 2028 0a20 2020 2020 2020 2020 2020  OM (.           
-0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acc0: 2053 454c 4543 5420 5354 5f43 6f6c 6c65   SELECT ST_Colle
-0000acd0: 6374 286c 6179 6572 5f67 656f 2e7b 7b67  ct(layer_geo.{{g
-0000ace0: 656f 6d65 7472 7963 6f6c 756d 6e7d 7d0a  eometrycolumn}}.
-0000acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad10: 2020 2029 2041 5320 7b7b 6765 6f6d 6574     ) AS {{geomet
-0000ad20: 7279 636f 6c75 6d6e 7d7d 0a20 2020 2020  rycolumn}}.     
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad40: 2020 2020 2020 2020 2020 2020 207b 6772               {gr
-0000ad50: 6f75 7062 795f 7365 6c65 6374 5f70 7265  oupby_select_pre
-0000ad60: 6669 7865 645f 7374 722e 666f 726d 6174  fixed_str.format
-0000ad70: 2870 7265 6669 783d 226c 6179 6572 5f67  (prefix="layer_g
-0000ad80: 656f 2e22 297d 0a20 2020 2020 2020 2020  eo.")}.         
-0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ada0: 2020 2020 2020 2020 202c 4d49 4e28 6c61           ,MIN(la
-0000adb0: 7965 725f 6765 6f2e 7b6f 7264 6572 6279  yer_geo.{orderby
-0000adc0: 5f63 6f6c 756d 6e7d 2920 6173 207b 6f72  _column}) as {or
-0000add0: 6465 7262 795f 636f 6c75 6d6e 7d0a 2020  derby_column}.  
-0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adf0: 2020 2020 2020 2020 2020 2020 4652 4f4d              FROM
-0000ae00: 2022 7b7b 696e 7075 745f 6c61 7965 727d   "{{input_layer}
-0000ae10: 7d22 206c 6179 6572 5f67 656f 0a20 2020  }" layer_geo.   
-0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae30: 2020 2020 2020 2020 2020 207b 6772 6f75             {grou
-0000ae40: 7062 795f 6772 6f75 7062 795f 7072 6566  pby_groupby_pref
-0000ae50: 6978 6564 5f73 7472 2e66 6f72 6d61 7428  ixed_str.format(
-0000ae60: 7072 6566 6978 3d22 6c61 7965 725f 6765  prefix="layer_ge
-0000ae70: 6f2e 2229 7d0a 2020 2020 2020 2020 2020  o.")}.          
-0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae90: 2020 2920 6765 6f5f 6461 7461 0a20 2020    ) geo_data.   
+0000ac10: 2020 2020 2020 2020 5345 4c45 4354 207b          SELECT {
+0000ac20: 7b67 656f 6d65 7472 7963 6f6c 756d 6e7d  {geometrycolumn}
+0000ac30: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 2020 2020 7b67 726f 7570 6279 5f73 656c      {groupby_sel
+0000ac60: 6563 745f 7072 6566 6978 6564 5f73 7472  ect_prefixed_str
+0000ac70: 2e66 6f72 6d61 7428 7072 6566 6978 3d22  .format(prefix="
+0000ac80: 6c61 7965 722e 2229 7d0a 2020 2020 2020  layer.")}.      
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aca0: 2020 2020 2020 2020 4652 4f4d 2022 7b7b          FROM "{{
+0000acb0: 696e 7075 745f 6c61 7965 727d 7d22 206c  input_layer}}" l
+0000acc0: 6179 6572 0a20 2020 2020 2020 2020 2020  ayer.           
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ace0: 2020 4f52 4445 5220 4259 206c 6179 6572    ORDER BY layer
+0000acf0: 2e7b 6f72 6465 7262 795f 636f 6c75 6d6e  .{orderby_column
+0000ad00: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000ad10: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad50: 2320 4e6f 2065 7870 6c6f 6465 636f 6c6c  # No explodecoll
+0000ad60: 6563 7469 6f6e 732c 2073 6f20 636f 6c6c  ections, so coll
+0000ad70: 6563 7420 746f 206f 6e65 2067 656f 6d65  ect to one geome
+0000ad80: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
+0000ad90: 2020 2020 2020 2020 2020 2020 2320 2870              # (p
+0000ada0: 6572 2067 726f 7570 6279 2069 6620 6170  er groupby if ap
+0000adb0: 706c 6963 6162 6c65 292e 0a20 2020 2020  plicable)..     
+0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000add0: 2020 2073 716c 5f73 746d 7420 3d20 6622     sql_stmt = f"
+0000ade0: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+0000adf0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000ae00: 454c 4543 5420 5354 5f43 6f6c 6c65 6374  ELECT ST_Collect
+0000ae10: 287b 7b67 656f 6d65 7472 7963 6f6c 756d  ({{geometrycolum
+0000ae20: 6e7d 7d29 2041 5320 7b7b 6765 6f6d 6574  n}}) AS {{geomet
+0000ae30: 7279 636f 6c75 6d6e 7d7d 0a20 2020 2020  rycolumn}}.     
+0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae50: 2020 2020 2020 2020 2020 2020 207b 6772               {gr
+0000ae60: 6f75 7062 795f 7365 6c65 6374 5f70 7265  oupby_select_pre
+0000ae70: 6669 7865 645f 7374 722e 666f 726d 6174  fixed_str.format
+0000ae80: 2870 7265 6669 783d 226c 6179 6572 2e22  (prefix="layer."
+0000ae90: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
 0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aeb0: 2020 2020 2020 204a 4f49 4e20 280a 2020         JOIN (.  
-0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aed0: 2020 2020 2020 2020 2020 5345 4c45 4354            SELECT
-0000aee0: 2044 4953 5449 4e43 5420 6a73 6f6e 5f72   DISTINCT json_r
-0000aef0: 6f77 735f 7461 626c 652e 7661 6c75 6520  ows_table.value 
-0000af00: 6173 206a 736f 6e5f 726f 770a 2020 2020  as json_row.    
-0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af20: 2020 2020 2020 2020 2020 2020 7b67 726f              {gro
-0000af30: 7570 6279 5f73 656c 6563 745f 7072 6566  upby_select_pref
-0000af40: 6978 6564 5f73 7472 2e66 6f72 6d61 7428  ixed_str.format(
-0000af50: 7072 6566 6978 3d22 6c61 7965 725f 666f  prefix="layer_fo
-0000af60: 725f 6a73 6f6e 2e22 297d 0a20 2020 2020  r_json.")}.     
-0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af80: 2020 2020 2020 2020 2046 524f 4d20 227b           FROM "{
-0000af90: 7b69 6e70 7574 5f6c 6179 6572 7d7d 2220  {input_layer}}" 
-0000afa0: 6c61 7965 725f 666f 725f 6a73 6f6e 0a20  layer_for_json. 
-0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afc0: 2020 2020 2020 2020 2020 2020 2043 524f               CRO
-0000afd0: 5353 204a 4f49 4e20 6a73 6f6e 5f65 6163  SS JOIN json_eac
-0000afe0: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
-0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b000: 2020 2020 206c 6179 6572 5f66 6f72 5f6a       layer_for_j
-0000b010: 736f 6e2e 5f5f 4449 5353 4f4c 5645 5f54  son.__DISSOLVE_T
-0000b020: 4f4a 534f 4e2c 2022 2422 2920 6a73 6f6e  OJSON, "$") json
-0000b030: 5f72 6f77 735f 7461 626c 650a 2020 2020  _rows_table.    
-0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b050: 2020 2020 2020 2020 2920 6a73 6f6e 5f64          ) json_d
-0000b060: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-0000b070: 2020 2020 2020 2020 2020 2020 2057 4845               WHE
-0000b080: 5245 2031 3d31 0a20 2020 2020 2020 2020  RE 1=1.         
-0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0a0: 2020 207b 6772 6f75 7062 795f 6669 6c74     {groupby_filt
-0000b0b0: 6572 5f73 7472 7d0a 2020 2020 2020 2020  er_str}.        
+0000aeb0: 2046 524f 4d20 227b 7b69 6e70 7574 5f6c   FROM "{{input_l
+0000aec0: 6179 6572 7d7d 2220 6c61 7965 720a 2020  ayer}}" layer.  
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aee0: 2020 2020 2020 2020 2020 2020 7b67 726f              {gro
+0000aef0: 7570 6279 5f67 726f 7570 6279 5f70 7265  upby_groupby_pre
+0000af00: 6669 7865 645f 7374 722e 666f 726d 6174  fixed_str.format
+0000af10: 2870 7265 6669 783d 226c 6179 6572 2e22  (prefix="layer."
+0000af20: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
+0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af40: 4f52 4445 5220 4259 204d 494e 286c 6179  ORDER BY MIN(lay
+0000af50: 6572 2e7b 6f72 6465 7262 795f 636f 6c75  er.{orderby_colu
+0000af60: 6d6e 7d29 0a20 2020 2020 2020 2020 2020  mn}).           
+0000af70: 2020 2020 2020 2020 2020 2020 2022 2222               """
+0000af80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000af90: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000afa0: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+0000afb0: 6167 675f 636f 6c75 6d6e 7320 7370 6563  agg_columns spec
+0000afc0: 6966 6965 642c 2070 6f73 7470 726f 6365  ified, postproce
+0000afd0: 7373 696e 6720 6973 2061 2062 6974 206d  ssing is a bit m
+0000afe0: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
+0000aff0: 2020 2020 2020 2020 2320 636f 6d70 6c69          # compli
+0000b000: 6361 7465 642e 0a20 2020 2020 2020 2020  cated..         
+0000b010: 2020 2020 2020 2020 2020 2073 716c 5f73             sql_s
+0000b020: 746d 7420 3d20 6622 2222 0a20 2020 2020  tmt = f""".     
+0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b040: 2020 2053 454c 4543 5420 6765 6f5f 6461     SELECT geo_da
+0000b050: 7461 2e7b 7b67 656f 6d65 7472 7963 6f6c  ta.{{geometrycol
+0000b060: 756d 6e7d 7d0a 2020 2020 2020 2020 2020  umn}}.          
+0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b080: 2020 2020 7b67 726f 7570 6279 5f73 656c      {groupby_sel
+0000b090: 6563 745f 7072 6566 6978 6564 5f73 7472  ect_prefixed_str
+0000b0a0: 2e66 6f72 6d61 7428 7072 6566 6978 3d22  .format(prefix="
+0000b0b0: 6765 6f5f 6461 7461 2e22 297d 0a20 2020  geo_data.")}.   
 0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0d0: 2020 7b67 726f 7570 6279 5f67 726f 7570    {groupby_group
-0000b0e0: 6279 5f70 7265 6669 7865 645f 7374 722e  by_prefixed_str.
-0000b0f0: 666f 726d 6174 2870 7265 6669 783d 2267  format(prefix="g
-0000b100: 656f 5f64 6174 612e 2229 7d0a 2020 2020  eo_data.")}.    
+0000b0d0: 2020 2020 2020 2020 2020 207b 6167 675f             {agg_
+0000b0e0: 636f 6c75 6d6e 735f 7374 727d 0a20 2020  columns_str}.   
+0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b100: 2020 2020 2020 2046 524f 4d20 280a 2020         FROM (.  
 0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b120: 2020 2020 2020 4f52 4445 5220 4259 2067        ORDER BY g
-0000b130: 656f 5f64 6174 612e 7b6f 7264 6572 6279  eo_data.{orderby
-0000b140: 5f63 6f6c 756d 6e7d 0a20 2020 2020 2020  _column}.       
-0000b150: 2020 2020 2020 2020 2020 2020 2022 2222               """
-0000b160: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b170: 2020 2320 476f 210a 2020 2020 2020 2020    # Go!.        
-0000b180: 2020 2020 2020 2020 5f67 656f 6f70 735f          _geoops_
-0000b190: 7371 6c2e 7365 6c65 6374 280a 2020 2020  sql.select(.    
+0000b120: 2020 2020 2020 2020 2020 5345 4c45 4354            SELECT
+0000b130: 2053 545f 436f 6c6c 6563 7428 6c61 7965   ST_Collect(laye
+0000b140: 725f 6765 6f2e 7b7b 6765 6f6d 6574 7279  r_geo.{{geometry
+0000b150: 636f 6c75 6d6e 7d7d 0a20 2020 2020 2020  column}}.       
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2020 2020 2020 2020 2020 2920 4153              ) AS
+0000b180: 207b 7b67 656f 6d65 7472 7963 6f6c 756d   {{geometrycolum
+0000b190: 6e7d 7d0a 2020 2020 2020 2020 2020 2020  n}}.            
 0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1b0: 696e 7075 745f 7061 7468 3d6f 7574 7075  input_path=outpu
-0000b1c0: 745f 746d 705f 7061 7468 2c0a 2020 2020  t_tmp_path,.    
-0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1e0: 6f75 7470 7574 5f70 6174 683d 6f75 7470  output_path=outp
-0000b1f0: 7574 5f70 6174 682c 0a20 2020 2020 2020  ut_path,.       
-0000b200: 2020 2020 2020 2020 2020 2020 2073 716c               sql
-0000b210: 5f73 746d 743d 7371 6c5f 7374 6d74 2c0a  _stmt=sql_stmt,.
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 6f75 7470 7574 5f6c 6179 6572      output_layer
-0000b240: 3d6f 7574 7075 745f 6c61 7965 722c 0a20  =output_layer,. 
+0000b1b0: 2020 2020 2020 7b67 726f 7570 6279 5f73        {groupby_s
+0000b1c0: 656c 6563 745f 7072 6566 6978 6564 5f73  elect_prefixed_s
+0000b1d0: 7472 2e66 6f72 6d61 7428 7072 6566 6978  tr.format(prefix
+0000b1e0: 3d22 6c61 7965 725f 6765 6f2e 2229 7d0a  ="layer_geo.")}.
+0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b210: 2020 2c4d 494e 286c 6179 6572 5f67 656f    ,MIN(layer_geo
+0000b220: 2e7b 6f72 6465 7262 795f 636f 6c75 6d6e  .{orderby_column
+0000b230: 7d29 2061 7320 7b6f 7264 6572 6279 5f63  }) as {orderby_c
+0000b240: 6f6c 756d 6e7d 0a20 2020 2020 2020 2020  olumn}.         
 0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b260: 2020 2065 7870 6c6f 6465 636f 6c6c 6563     explodecollec
-0000b270: 7469 6f6e 733d 6578 706c 6f64 6563 6f6c  tions=explodecol
-0000b280: 6c65 6374 696f 6e73 2c0a 2020 2020 2020  lections,.      
-0000b290: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000b2a0: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
-0000b2b0: 2020 2020 2020 2020 2020 2320 436c 6561            # Clea
-0000b2c0: 6e20 746d 7020 6469 7220 6966 2069 7420  n tmp dir if it 
-0000b2d0: 6578 6973 7473 2e2e 2e0a 2020 2020 2020  exists....      
-0000b2e0: 2020 2020 2020 6966 2074 656d 7064 6972        if tempdir
-0000b2f0: 2e65 7869 7374 7328 293a 0a20 2020 2020  .exists():.     
-0000b300: 2020 2020 2020 2020 2020 2073 6875 7469             shuti
-0000b310: 6c2e 726d 7472 6565 2874 656d 7064 6972  l.rmtree(tempdir
-0000b320: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-0000b330: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-0000b340: 6c65 6d65 6e74 6564 4572 726f 7228 0a20  lementedError(. 
-0000b350: 2020 2020 2020 2020 2020 2066 2255 6e73             f"Uns
-0000b360: 7570 706f 7274 6564 2069 6e70 7574 2067  upported input g
-0000b370: 656f 6d65 7472 7974 7970 653a 207b 696e  eometrytype: {in
-0000b380: 7075 745f 6c61 7965 7269 6e66 6f2e 6765  put_layerinfo.ge
-0000b390: 6f6d 6574 7279 7479 7065 7d22 0a20 2020  ometrytype}".   
-0000b3a0: 2020 2020 2029 0a0a 2020 2020 2320 5265       )..    # Re
-0000b3b0: 7475 726e 2072 6573 756c 7420 696e 666f  turn result info
-0000b3c0: 0a20 2020 2072 6573 756c 745f 696e 666f  .    result_info
-0000b3d0: 5b0a 2020 2020 2020 2020 226d 6573 7361  [.        "messa
-0000b3e0: 6765 220a 2020 2020 5d20 3d20 6622 4469  ge".    ] = f"Di
-0000b3f0: 7373 6f6c 7665 2063 6f6d 706c 6574 656c  ssolve completel
-0000b400: 7920 7265 6164 792c 2074 6f6f 6b20 7b64  y ready, took {d
-0000b410: 6174 6574 696d 652e 6e6f 7728 292d 7374  atetime.now()-st
-0000b420: 6172 745f 7469 6d65 7d21 220a 2020 2020  art_time}!".    
-0000b430: 6c6f 6767 6572 2e69 6e66 6f28 7265 7375  logger.info(resu
-0000b440: 6c74 5f69 6e66 6f5b 226d 6573 7361 6765  lt_info["message
-0000b450: 225d 290a 2020 2020 7265 7475 726e 2072  "]).    return r
-0000b460: 6573 756c 745f 696e 666f 0a0a 0a64 6566  esult_info...def
-0000b470: 205f 6469 7373 6f6c 7665 5f70 6f6c 7967   _dissolve_polyg
-0000b480: 6f6e 735f 7061 7373 280a 2020 2020 696e  ons_pass(.    in
-0000b490: 7075 745f 7061 7468 3a20 5061 7468 2c0a  put_path: Path,.
-0000b4a0: 2020 2020 6f75 7470 7574 5f6e 6f74 6f6e      output_noton
-0000b4b0: 626f 7264 6572 5f70 6174 683a 2050 6174  border_path: Pat
-0000b4c0: 682c 0a20 2020 206f 7574 7075 745f 6f6e  h,.    output_on
-0000b4d0: 626f 7264 6572 5f70 6174 683a 2050 6174  border_path: Pat
-0000b4e0: 682c 0a20 2020 2065 7870 6c6f 6465 636f  h,.    explodeco
-0000b4f0: 6c6c 6563 7469 6f6e 733a 2062 6f6f 6c2c  llections: bool,
-0000b500: 0a20 2020 2067 726f 7570 6279 5f63 6f6c  .    groupby_col
-0000b510: 756d 6e73 3a20 4f70 7469 6f6e 616c 5b49  umns: Optional[I
-0000b520: 7465 7261 626c 655b 7374 725d 5d2c 0a20  terable[str]],. 
-0000b530: 2020 2061 6767 5f63 6f6c 756d 6e73 3a20     agg_columns: 
-0000b540: 4f70 7469 6f6e 616c 5b64 6963 745d 2c0a  Optional[dict],.
-0000b550: 2020 2020 7469 6c65 735f 6764 663a 2067      tiles_gdf: g
-0000b560: 7064 2e47 656f 4461 7461 4672 616d 652c  pd.GeoDataFrame,
-0000b570: 0a20 2020 2069 6e70 7574 5f6c 6179 6572  .    input_layer
-0000b580: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d2c  : Optional[str],
-0000b590: 0a20 2020 206f 7574 7075 745f 6c61 7965  .    output_laye
-0000b5a0: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
-0000b5b0: 2c0a 2020 2020 6e62 5f70 6172 616c 6c65  ,.    nb_paralle
-0000b5c0: 6c3a 2069 6e74 2c0a 2920 2d3e 2064 6963  l: int,.) -> dic
-0000b5d0: 743a 0a20 2020 2023 204d 616b 6520 7375  t:.    # Make su
-0000b5e0: 7265 2074 6865 2069 6e70 7574 2066 696c  re the input fil
-0000b5f0: 6520 6861 7320 6120 7370 6174 6961 6c20  e has a spatial 
-0000b600: 696e 6465 780a 2020 2020 6766 6f2e 6372  index.    gfo.cr
-0000b610: 6561 7465 5f73 7061 7469 616c 5f69 6e64  eate_spatial_ind
-0000b620: 6578 2869 6e70 7574 5f70 6174 682c 2065  ex(input_path, e
-0000b630: 7869 7374 5f6f 6b3d 5472 7565 290a 0a20  xist_ok=True).. 
-0000b640: 2020 2023 2053 7461 7274 2063 616c 6375     # Start calcu
-0000b650: 6c61 7469 6f6e 2069 6e20 7061 7261 6c6c  lation in parall
-0000b660: 656c 0a20 2020 2073 7461 7274 5f74 696d  el.    start_tim
-0000b670: 6520 3d20 6461 7465 7469 6d65 2e6e 6f77  e = datetime.now
-0000b680: 2829 0a20 2020 2072 6573 756c 745f 696e  ().    result_in
-0000b690: 666f 203d 207b 7d0a 2020 2020 7374 6172  fo = {}.    star
-0000b6a0: 745f 7469 6d65 203d 2064 6174 6574 696d  t_time = datetim
-0000b6b0: 652e 6e6f 7728 290a 2020 2020 696e 7075  e.now().    inpu
-0000b6c0: 745f 6c61 7965 7269 6e66 6f20 3d20 6766  t_layerinfo = gf
-0000b6d0: 6f2e 6765 745f 6c61 7965 7269 6e66 6f28  o.get_layerinfo(
-0000b6e0: 696e 7075 745f 7061 7468 2c20 696e 7075  input_path, inpu
-0000b6f0: 745f 6c61 7965 7229 0a0a 2020 2020 2320  t_layer)..    # 
-0000b700: 5072 6f63 6573 7369 6e67 2069 6e20 7468  Processing in th
-0000b710: 7265 6164 7320 6973 2032 7820 6661 7374  reads is 2x fast
-0000b720: 6572 2066 6f72 2073 6d61 6c6c 2064 6174  er for small dat
-0000b730: 6173 6574 7320 286f 6e20 5769 6e64 6f77  asets (on Window
-0000b740: 7329 0a20 2020 2063 616c 6375 6c61 7465  s).    calculate
-0000b750: 5f69 6e5f 7468 7265 6164 7320 3d20 5472  _in_threads = Tr
-0000b760: 7565 2069 6620 696e 7075 745f 6c61 7965  ue if input_laye
-0000b770: 7269 6e66 6f2e 6665 6174 7572 6563 6f75  rinfo.featurecou
-0000b780: 6e74 203c 3d20 3130 3020 656c 7365 2046  nt <= 100 else F
-0000b790: 616c 7365 0a20 2020 2077 6974 6820 5f70  alse.    with _p
-0000b7a0: 726f 6365 7373 696e 675f 7574 696c 2e50  rocessing_util.P
-0000b7b0: 6f6f 6c65 6445 7865 6375 746f 7246 6163  ooledExecutorFac
-0000b7c0: 746f 7279 280a 2020 2020 2020 2020 7468  tory(.        th
-0000b7d0: 7265 6164 706f 6f6c 3d63 616c 6375 6c61  readpool=calcula
-0000b7e0: 7465 5f69 6e5f 7468 7265 6164 732c 0a20  te_in_threads,. 
-0000b7f0: 2020 2020 2020 206d 6178 5f77 6f72 6b65         max_worke
-0000b800: 7273 3d6e 625f 7061 7261 6c6c 656c 2c0a  rs=nb_parallel,.
-0000b810: 2020 2020 2020 2020 696e 6974 6961 6c69          initiali
-0000b820: 7a65 723d 5f70 726f 6365 7373 696e 675f  zer=_processing_
-0000b830: 7574 696c 2e69 6e69 7469 616c 697a 655f  util.initialize_
-0000b840: 776f 726b 6572 2829 2c0a 2020 2020 2920  worker(),.    ) 
-0000b850: 6173 2063 616c 6375 6c61 7465 5f70 6f6f  as calculate_poo
-0000b860: 6c3a 0a20 2020 2020 2020 2023 2050 7265  l:.        # Pre
-0000b870: 7061 7265 206f 7574 7075 7420 6669 6c65  pare output file
-0000b880: 6e61 6d65 0a20 2020 2020 2020 2074 656d  name.        tem
-0000b890: 7064 6972 203d 206f 7574 7075 745f 6f6e  pdir = output_on
-0000b8a0: 626f 7264 6572 5f70 6174 682e 7061 7265  border_path.pare
-0000b8b0: 6e74 0a0a 2020 2020 2020 2020 6261 7463  nt..        batc
-0000b8c0: 6865 7320 3d20 7b7d 0a20 2020 2020 2020  hes = {}.       
-0000b8d0: 206e 625f 6261 7463 6865 7320 3d20 6c65   nb_batches = le
-0000b8e0: 6e28 7469 6c65 735f 6764 6629 0a20 2020  n(tiles_gdf).   
-0000b8f0: 2020 2020 206e 625f 6261 7463 6865 735f       nb_batches_
-0000b900: 646f 6e65 203d 2030 0a20 2020 2020 2020  done = 0.       
-0000b910: 2066 7574 7572 655f 746f 5f62 6174 6368   future_to_batch
-0000b920: 5f69 6420 3d20 7b7d 0a20 2020 2020 2020  _id = {}.       
-0000b930: 206e 625f 726f 7773 5f64 6f6e 6520 3d20   nb_rows_done = 
-0000b940: 300a 2020 2020 2020 2020 666f 7220 6261  0.        for ba
-0000b950: 7463 685f 6964 2c20 7469 6c65 5f72 6f77  tch_id, tile_row
-0000b960: 2069 6e20 656e 756d 6572 6174 6528 7469   in enumerate(ti
-0000b970: 6c65 735f 6764 662e 6974 6572 7475 706c  les_gdf.itertupl
-0000b980: 6573 2829 293a 0a20 2020 2020 2020 2020  es()):.         
-0000b990: 2020 2062 6174 6368 6573 5b62 6174 6368     batches[batch
-0000b9a0: 5f69 645d 203d 207b 7d0a 2020 2020 2020  _id] = {}.      
-0000b9b0: 2020 2020 2020 6261 7463 6865 735b 6261        batches[ba
-0000b9c0: 7463 685f 6964 5d5b 226c 6179 6572 225d  tch_id]["layer"]
-0000b9d0: 203d 206f 7574 7075 745f 6c61 7965 720a   = output_layer.
-0000b9e0: 2020 2020 2020 2020 2020 2020 6261 7463              batc
-0000b9f0: 6865 735b 6261 7463 685f 6964 5d5b 2262  hes[batch_id]["b
-0000ba00: 6f75 6e64 7322 5d20 3d20 7469 6c65 5f72  ounds"] = tile_r
-0000ba10: 6f77 2e67 656f 6d65 7472 792e 626f 756e  ow.geometry.boun
-0000ba20: 6473 0a0a 2020 2020 2020 2020 2020 2020  ds..            
-0000ba30: 2320 4f75 7470 7574 2065 6163 6820 6261  # Output each ba
-0000ba40: 7463 6820 746f 2061 2073 6570 6572 6174  tch to a seperat
-0000ba50: 6520 7465 6d70 6f72 6172 7920 6669 6c65  e temporary file
-0000ba60: 2c20 6f74 6865 7277 6973 6520 7468 6572  , otherwise ther
-0000ba70: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
-0000ba80: 6172 6520 7469 6d65 6f75 7420 6973 7375  are timeout issu
-0000ba90: 6573 2077 6865 6e20 7072 6f63 6573 7369  es when processi
-0000baa0: 6e67 206c 6172 6765 2066 696c 6573 0a20  ng large files. 
-0000bab0: 2020 2020 2020 2020 2020 2073 7566 6669             suffi
-0000bac0: 7820 3d20 6f75 7470 7574 5f6e 6f74 6f6e  x = output_noton
-0000bad0: 626f 7264 6572 5f70 6174 682e 7375 6666  border_path.suff
-0000bae0: 6978 0a20 2020 2020 2020 2020 2020 206e  ix.            n
-0000baf0: 616d 6520 3d20 6622 7b6f 7574 7075 745f  ame = f"{output_
-0000bb00: 6e6f 746f 6e62 6f72 6465 725f 7061 7468  notonborder_path
-0000bb10: 2e73 7465 6d7d 5f7b 6261 7463 685f 6964  .stem}_{batch_id
-0000bb20: 7d7b 7375 6666 6978 7d22 0a20 2020 2020  }{suffix}".     
-0000bb30: 2020 2020 2020 206f 7574 7075 745f 6e6f         output_no
-0000bb40: 746f 6e62 6f72 6465 725f 746d 705f 7061  tonborder_tmp_pa
-0000bb50: 7274 6961 6c5f 7061 7468 203d 2074 656d  rtial_path = tem
-0000bb60: 7064 6972 202f 206e 616d 650a 2020 2020  pdir / name.    
-0000bb70: 2020 2020 2020 2020 6261 7463 6865 735b          batches[
-0000bb80: 6261 7463 685f 6964 5d5b 0a20 2020 2020  batch_id][.     
-0000bb90: 2020 2020 2020 2020 2020 2022 6f75 7470             "outp
-0000bba0: 7574 5f6e 6f74 6f6e 626f 7264 6572 5f74  ut_notonborder_t
-0000bbb0: 6d70 5f70 6172 7469 616c 5f70 6174 6822  mp_partial_path"
-0000bbc0: 0a20 2020 2020 2020 2020 2020 205d 203d  .            ] =
-0000bbd0: 206f 7574 7075 745f 6e6f 746f 6e62 6f72   output_notonbor
-0000bbe0: 6465 725f 746d 705f 7061 7274 6961 6c5f  der_tmp_partial_
-0000bbf0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-0000bc00: 206e 616d 6520 3d20 6622 7b6f 7574 7075   name = f"{outpu
-0000bc10: 745f 6f6e 626f 7264 6572 5f70 6174 682e  t_onborder_path.
-0000bc20: 7374 656d 7d5f 7b62 6174 6368 5f69 647d  stem}_{batch_id}
-0000bc30: 7b73 7566 6669 787d 220a 2020 2020 2020  {suffix}".      
-0000bc40: 2020 2020 2020 6f75 7470 7574 5f6f 6e62        output_onb
-0000bc50: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
-0000bc60: 6c5f 7061 7468 203d 2074 656d 7064 6972  l_path = tempdir
-0000bc70: 202f 206e 616d 650a 2020 2020 2020 2020   / name.        
-0000bc80: 2020 2020 6261 7463 6865 735b 6261 7463      batches[batc
-0000bc90: 685f 6964 5d5b 0a20 2020 2020 2020 2020  h_id][.         
-0000bca0: 2020 2020 2020 2022 6f75 7470 7574 5f6f         "output_o
-0000bcb0: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
-0000bcc0: 6961 6c5f 7061 7468 220a 2020 2020 2020  ial_path".      
-0000bcd0: 2020 2020 2020 5d20 3d20 6f75 7470 7574        ] = output
-0000bce0: 5f6f 6e62 6f72 6465 725f 746d 705f 7061  _onborder_tmp_pa
-0000bcf0: 7274 6961 6c5f 7061 7468 0a0a 2020 2020  rtial_path..    
-0000bd00: 2020 2020 2020 2020 2320 4765 7420 7469          # Get ti
-0000bd10: 6c65 5f69 6420 6966 2070 7265 7365 6e74  le_id if present
-0000bd20: 0a20 2020 2020 2020 2020 2020 2074 696c  .            til
-0000bd30: 655f 6964 203d 2074 696c 655f 726f 772e  e_id = tile_row.
-0000bd40: 7469 6c65 5f69 6420 6966 2022 7469 6c65  tile_id if "tile
-0000bd50: 5f69 6422 2069 6e20 7469 6c65 5f72 6f77  _id" in tile_row
-0000bd60: 2e5f 6669 656c 6473 2065 6c73 6520 4e6f  ._fields else No
-0000bd70: 6e65 0a0a 2020 2020 2020 2020 2020 2020  ne..            
-0000bd80: 6675 7475 7265 203d 2063 616c 6375 6c61  future = calcula
-0000bd90: 7465 5f70 6f6f 6c2e 7375 626d 6974 280a  te_pool.submit(.
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 5f64 6973 736f 6c76 655f 706f 6c79 676f  _dissolve_polygo
-0000bdc0: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-0000bdd0: 2020 2020 696e 7075 745f 7061 7468 3d69      input_path=i
-0000bde0: 6e70 7574 5f70 6174 682c 0a20 2020 2020  nput_path,.     
-0000bdf0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-0000be00: 745f 6e6f 746f 6e62 6f72 6465 725f 7061  t_notonborder_pa
-0000be10: 7468 3d6f 7574 7075 745f 6e6f 746f 6e62  th=output_notonb
-0000be20: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
-0000be30: 6c5f 7061 7468 2c0a 2020 2020 2020 2020  l_path,.        
-0000be40: 2020 2020 2020 2020 6f75 7470 7574 5f6f          output_o
-0000be50: 6e62 6f72 6465 725f 7061 7468 3d6f 7574  nborder_path=out
-0000be60: 7075 745f 6f6e 626f 7264 6572 5f74 6d70  put_onborder_tmp
-0000be70: 5f70 6172 7469 616c 5f70 6174 682c 0a20  _partial_path,. 
-0000be80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000be90: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
-0000bea0: 733d 6578 706c 6f64 6563 6f6c 6c65 6374  s=explodecollect
-0000beb0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-0000bec0: 2020 2020 2020 6772 6f75 7062 795f 636f        groupby_co
-0000bed0: 6c75 6d6e 733d 6772 6f75 7062 795f 636f  lumns=groupby_co
-0000bee0: 6c75 6d6e 732c 0a20 2020 2020 2020 2020  lumns,.         
-0000bef0: 2020 2020 2020 2061 6767 5f63 6f6c 756d         agg_colum
-0000bf00: 6e73 3d61 6767 5f63 6f6c 756d 6e73 2c0a  ns=agg_columns,.
-0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf20: 696e 7075 745f 6765 6f6d 6574 7279 7479  input_geometryty
-0000bf30: 7065 3d69 6e70 7574 5f6c 6179 6572 696e  pe=input_layerin
-0000bf40: 666f 2e67 656f 6d65 7472 7974 7970 652c  fo.geometrytype,
-0000bf50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bf60: 2069 6e70 7574 5f6c 6179 6572 3d69 6e70   input_layer=inp
-0000bf70: 7574 5f6c 6179 6572 2c0a 2020 2020 2020  ut_layer,.      
-0000bf80: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-0000bf90: 5f6c 6179 6572 3d6f 7574 7075 745f 6c61  _layer=output_la
-0000bfa0: 7965 722c 0a20 2020 2020 2020 2020 2020  yer,.           
-0000bfb0: 2020 2020 2062 626f 783d 7469 6c65 5f72       bbox=tile_r
-0000bfc0: 6f77 2e67 656f 6d65 7472 792e 626f 756e  ow.geometry.boun
-0000bfd0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-0000bfe0: 2020 2020 7469 6c65 5f69 643d 7469 6c65      tile_id=tile
-0000bff0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0000c000: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
-0000c010: 7574 7572 655f 746f 5f62 6174 6368 5f69  uture_to_batch_i
-0000c020: 645b 6675 7475 7265 5d20 3d20 6261 7463  d[future] = batc
-0000c030: 685f 6964 0a0a 2020 2020 2020 2020 2320  h_id..        # 
-0000c040: 4c6f 6f70 2074 696c 6c20 616c 6c20 7061  Loop till all pa
-0000c050: 7261 6c6c 656c 2070 726f 6365 7373 6573  rallel processes
-0000c060: 2061 7265 2072 6561 6479 2c20 6275 7420   are ready, but 
-0000c070: 7072 6f63 6573 7320 6561 6368 206f 6e65  process each one
-0000c080: 0a20 2020 2020 2020 2023 2074 6861 7420  .        # that 
-0000c090: 6973 2072 6561 6479 2061 6c72 6561 6479  is ready already
-0000c0a0: 0a20 2020 2020 2020 205f 6765 6e65 7261  .        _genera
-0000c0b0: 6c5f 7574 696c 2e72 6570 6f72 745f 7072  l_util.report_pr
-0000c0c0: 6f67 7265 7373 280a 2020 2020 2020 2020  ogress(.        
-0000c0d0: 2020 2020 7374 6172 745f 7469 6d65 2c20      start_time, 
-0000c0e0: 6e62 5f62 6174 6368 6573 5f64 6f6e 652c  nb_batches_done,
-0000c0f0: 206e 625f 6261 7463 6865 732c 2022 6469   nb_batches, "di
-0000c100: 7373 6f6c 7665 220a 2020 2020 2020 2020  ssolve".        
-0000c110: 290a 2020 2020 2020 2020 666f 7220 6675  ).        for fu
-0000c120: 7475 7265 2069 6e20 6675 7475 7265 732e  ture in futures.
-0000c130: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-0000c140: 7572 655f 746f 5f62 6174 6368 5f69 6429  ure_to_batch_id)
-0000c150: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-0000c160: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000c170: 2020 2023 2049 6620 7468 6520 6361 6c63     # If the calc
-0000c180: 756c 6174 6520 6761 7665 2072 6573 756c  ulate gave resul
-0000c190: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
-0000c1a0: 2020 206e 625f 6261 7463 6865 735f 646f     nb_batches_do
-0000c1b0: 6e65 202b 3d20 310a 2020 2020 2020 2020  ne += 1.        
-0000c1c0: 2020 2020 2020 2020 6261 7463 685f 6964          batch_id
-0000c1d0: 203d 2066 7574 7572 655f 746f 5f62 6174   = future_to_bat
-0000c1e0: 6368 5f69 645b 6675 7475 7265 5d0a 2020  ch_id[future].  
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000c200: 7375 6c74 203d 2066 7574 7572 652e 7265  sult = future.re
-0000c210: 7375 6c74 2829 0a0a 2020 2020 2020 2020  sult()..        
-0000c220: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
-0000c230: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-0000c240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c250: 2020 206e 625f 726f 7773 5f64 6f6e 6520     nb_rows_done 
-0000c260: 2b3d 2072 6573 756c 745b 226e 625f 726f  += result["nb_ro
-0000c270: 7773 5f64 6f6e 6522 5d0a 2020 2020 2020  ws_done"].      
-0000c280: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c290: 2072 6573 756c 745b 226e 625f 726f 7773   result["nb_rows
-0000c2a0: 5f64 6f6e 6522 5d20 3e20 3020 616e 6420  _done"] > 0 and 
-0000c2b0: 7265 7375 6c74 5b22 746f 7461 6c5f 7469  result["total_ti
-0000c2c0: 6d65 225d 203e 2030 3a0a 2020 2020 2020  me"] > 0:.      
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 2020 726f 7773 5f70 6572 5f73 6563 203d    rows_per_sec =
-0000c2f0: 2072 6f75 6e64 280a 2020 2020 2020 2020   round(.        
-0000c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c310: 2020 2020 7265 7375 6c74 5b22 6e62 5f72      result["nb_r
-0000c320: 6f77 735f 646f 6e65 225d 202f 2072 6573  ows_done"] / res
-0000c330: 756c 745b 2274 6f74 616c 5f74 696d 6522  ult["total_time"
-0000c340: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000c350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c370: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000c380: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000c390: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000c3a0: 4261 7463 6820 7b62 6174 6368 5f69 647d  Batch {batch_id}
-0000c3b0: 2070 726f 6365 7373 6564 207b 7265 7375   processed {resu
-0000c3c0: 6c74 5b27 6e62 5f72 6f77 735f 646f 6e65  lt['nb_rows_done
-0000c3d0: 275d 7d20 726f 7773 2022 0a20 2020 2020  ']} rows ".     
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 2020 2020 2020 2066 2228 7b72 6f77 735f         f"({rows_
-0000c400: 7065 725f 7365 637d 2f73 6563 2922 0a20  per_sec}/sec)". 
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c420: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c440: 2069 6620 2270 6572 6673 7472 696e 6722   if "perfstring"
-0000c450: 2069 6e20 7265 7375 6c74 3a0a 2020 2020   in result:.    
-0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c470: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000c480: 6562 7567 2866 2250 6572 6673 7472 696e  ebug(f"Perfstrin
-0000c490: 673a 207b 7265 7375 6c74 5b27 7065 7266  g: {result['perf
-0000c4a0: 7374 7269 6e67 275d 7d22 290a 0a20 2020  string']}")..   
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4c0: 2023 2053 7461 7274 2063 6f70 7920 6f66   # Start copy of
-0000c4d0: 2074 6865 2072 6573 756c 7420 746f 2061   the result to a
-0000c4e0: 2063 6f6d 6d6f 6e20 6669 6c65 0a20 2020   common file.   
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c500: 2062 6174 6368 5f69 6420 3d20 6675 7475   batch_id = futu
-0000c510: 7265 5f74 6f5f 6261 7463 685f 6964 5b66  re_to_batch_id[f
-0000c520: 7574 7572 655d 0a0a 2020 2020 2020 2020  uture]..        
-0000c530: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-0000c540: 2063 616c 6375 6c61 7465 2067 6176 6520   calculate gave 
-0000c550: 6e6f 746f 6e62 6f72 6465 7220 7265 7375  notonborder resu
-0000c560: 6c74 732c 2061 7070 656e 6420 746f 206f  lts, append to o
-0000c570: 7574 7075 740a 2020 2020 2020 2020 2020  utput.          
-0000c580: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-0000c590: 5f6e 6f74 6f6e 626f 7264 6572 5f74 6d70  _notonborder_tmp
-0000c5a0: 5f70 6172 7469 616c 5f70 6174 6820 3d20  _partial_path = 
-0000c5b0: 6261 7463 6865 735b 6261 7463 685f 6964  batches[batch_id
-0000c5c0: 5d5b 0a20 2020 2020 2020 2020 2020 2020  ][.             
-0000c5d0: 2020 2020 2020 2020 2020 2022 6f75 7470             "outp
-0000c5e0: 7574 5f6e 6f74 6f6e 626f 7264 6572 5f74  ut_notonborder_t
-0000c5f0: 6d70 5f70 6172 7469 616c 5f70 6174 6822  mp_partial_path"
-0000c600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c610: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-0000c620: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 2020 2020 2020 6f75 7470 7574 5f6e          output_n
-0000c650: 6f74 6f6e 626f 7264 6572 5f74 6d70 5f70  otonborder_tmp_p
-0000c660: 6172 7469 616c 5f70 6174 682e 6578 6973  artial_path.exis
-0000c670: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-0000c680: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-0000c690: 206f 7574 7075 745f 6e6f 746f 6e62 6f72   output_notonbor
-0000c6a0: 6465 725f 746d 705f 7061 7274 6961 6c5f  der_tmp_partial_
-0000c6b0: 7061 7468 2e73 7461 7428 292e 7374 5f73  path.stat().st_s
-0000c6c0: 697a 6520 3e20 300a 2020 2020 2020 2020  ize > 0.        
-0000c6d0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+0000b260: 2020 2020 2046 524f 4d20 227b 7b69 6e70       FROM "{{inp
+0000b270: 7574 5f6c 6179 6572 7d7d 2220 6c61 7965  ut_layer}}" laye
+0000b280: 725f 6765 6f0a 2020 2020 2020 2020 2020  r_geo.          
+0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2a0: 2020 2020 7b67 726f 7570 6279 5f67 726f      {groupby_gro
+0000b2b0: 7570 6279 5f70 7265 6669 7865 645f 7374  upby_prefixed_st
+0000b2c0: 722e 666f 726d 6174 2870 7265 6669 783d  r.format(prefix=
+0000b2d0: 226c 6179 6572 5f67 656f 2e22 297d 0a20  "layer_geo.")}. 
+0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2f0: 2020 2020 2020 2020 2020 2029 2067 656f             ) geo
+0000b300: 5f64 6174 610a 2020 2020 2020 2020 2020  _data.          
+0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b320: 4a4f 494e 2028 0a20 2020 2020 2020 2020  JOIN (.         
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2053 454c 4543 5420 4449 5354 494e     SELECT DISTIN
+0000b350: 4354 206a 736f 6e5f 726f 7773 5f74 6162  CT json_rows_tab
+0000b360: 6c65 2e76 616c 7565 2061 7320 6a73 6f6e  le.value as json
+0000b370: 5f72 6f77 0a20 2020 2020 2020 2020 2020  _row.           
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2020 2020 207b 6772 6f75 7062 795f 7365       {groupby_se
+0000b3a0: 6c65 6374 5f70 7265 6669 7865 645f 7374  lect_prefixed_st
+0000b3b0: 722e 666f 726d 6174 2870 7265 6669 783d  r.format(prefix=
+0000b3c0: 226c 6179 6572 5f66 6f72 5f6a 736f 6e2e  "layer_for_json.
+0000b3d0: 2229 7d0a 2020 2020 2020 2020 2020 2020  ")}.            
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 4652 4f4d 2022 7b7b 696e 7075 745f    FROM "{{input_
+0000b400: 6c61 7965 727d 7d22 206c 6179 6572 5f66  layer}}" layer_f
+0000b410: 6f72 5f6a 736f 6e0a 2020 2020 2020 2020  or_json.        
+0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b430: 2020 2020 2020 4352 4f53 5320 4a4f 494e        CROSS JOIN
+0000b440: 206a 736f 6e5f 6561 6368 280a 2020 2020   json_each(.    
+0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b460: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0000b470: 7965 725f 666f 725f 6a73 6f6e 2e5f 5f44  yer_for_json.__D
+0000b480: 4953 534f 4c56 455f 544f 4a53 4f4e 2c20  ISSOLVE_TOJSON, 
+0000b490: 2224 2229 206a 736f 6e5f 726f 7773 5f74  "$") json_rows_t
+0000b4a0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+0000b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4c0: 2029 206a 736f 6e5f 6461 7461 0a20 2020   ) json_data.   
+0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4e0: 2020 2020 2020 5748 4552 4520 313d 310a        WHERE 1=1.
+0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b500: 2020 2020 2020 2020 2020 2020 7b67 726f              {gro
+0000b510: 7570 6279 5f66 696c 7465 725f 7374 727d  upby_filter_str}
+0000b520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b530: 2020 2020 2020 2020 2020 207b 6772 6f75             {grou
+0000b540: 7062 795f 6772 6f75 7062 795f 7072 6566  pby_groupby_pref
+0000b550: 6978 6564 5f73 7472 2e66 6f72 6d61 7428  ixed_str.format(
+0000b560: 7072 6566 6978 3d22 6765 6f5f 6461 7461  prefix="geo_data
+0000b570: 2e22 297d 0a20 2020 2020 2020 2020 2020  .")}.           
+0000b580: 2020 2020 2020 2020 2020 2020 2020 204f                 O
+0000b590: 5244 4552 2042 5920 6765 6f5f 6461 7461  RDER BY geo_data
+0000b5a0: 2e7b 6f72 6465 7262 795f 636f 6c75 6d6e  .{orderby_column
+0000b5b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000b5c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000b5d0: 2020 2020 2020 2020 2020 2023 2047 6f21             # Go!
+0000b5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5f0: 205f 6765 6f6f 7073 5f73 716c 2e73 656c   _geoops_sql.sel
+0000b600: 6563 7428 0a20 2020 2020 2020 2020 2020  ect(.           
+0000b610: 2020 2020 2020 2020 2069 6e70 7574 5f70           input_p
+0000b620: 6174 683d 6f75 7470 7574 5f74 6d70 5f70  ath=output_tmp_p
+0000b630: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+0000b640: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+0000b650: 7061 7468 3d6f 7574 7075 745f 7061 7468  path=output_path
+0000b660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b670: 2020 2020 2020 7371 6c5f 7374 6d74 3d73        sql_stmt=s
+0000b680: 716c 5f73 746d 742c 0a20 2020 2020 2020  ql_stmt,.       
+0000b690: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0000b6a0: 7075 745f 6c61 7965 723d 6f75 7470 7574  put_layer=output
+0000b6b0: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+0000b6c0: 2020 2020 2020 2020 2020 2020 6578 706c              expl
+0000b6d0: 6f64 6563 6f6c 6c65 6374 696f 6e73 3d65  odecollections=e
+0000b6e0: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
+0000b6f0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000b700: 2020 2029 0a0a 2020 2020 2020 2020 6669     )..        fi
+0000b710: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+0000b720: 2020 2023 2043 6c65 616e 2074 6d70 2064     # Clean tmp d
+0000b730: 6972 2069 6620 6974 2065 7869 7374 732e  ir if it exists.
+0000b740: 2e2e 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0000b750: 6620 7465 6d70 6469 722e 6578 6973 7473  f tempdir.exists
+0000b760: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000b770: 2020 2020 7368 7574 696c 2e72 6d74 7265      shutil.rmtre
+0000b780: 6528 7465 6d70 6469 7229 0a20 2020 2065  e(tempdir).    e
+0000b790: 6c73 653a 0a20 2020 2020 2020 2072 6169  lse:.        rai
+0000b7a0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+0000b7b0: 6445 7272 6f72 280a 2020 2020 2020 2020  dError(.        
+0000b7c0: 2020 2020 6622 556e 7375 7070 6f72 7465      f"Unsupporte
+0000b7d0: 6420 696e 7075 7420 6765 6f6d 6574 7279  d input geometry
+0000b7e0: 7479 7065 3a20 7b69 6e70 7574 5f6c 6179  type: {input_lay
+0000b7f0: 6572 696e 666f 2e67 656f 6d65 7472 7974  erinfo.geometryt
+0000b800: 7970 657d 220a 2020 2020 2020 2020 290a  ype}".        ).
+0000b810: 0a20 2020 2023 2052 6574 7572 6e20 7265  .    # Return re
+0000b820: 7375 6c74 2069 6e66 6f0a 2020 2020 7265  sult info.    re
+0000b830: 7375 6c74 5f69 6e66 6f5b 0a20 2020 2020  sult_info[.     
+0000b840: 2020 2022 6d65 7373 6167 6522 0a20 2020     "message".   
+0000b850: 205d 203d 2066 2244 6973 736f 6c76 6520   ] = f"Dissolve 
+0000b860: 636f 6d70 6c65 7465 6c79 2072 6561 6479  completely ready
+0000b870: 2c20 746f 6f6b 207b 6461 7465 7469 6d65  , took {datetime
+0000b880: 2e6e 6f77 2829 2d73 7461 7274 5f74 696d  .now()-start_tim
+0000b890: 657d 2122 0a20 2020 206c 6f67 6765 722e  e}!".    logger.
+0000b8a0: 696e 666f 2872 6573 756c 745f 696e 666f  info(result_info
+0000b8b0: 5b22 6d65 7373 6167 6522 5d29 0a20 2020  ["message"]).   
+0000b8c0: 2072 6574 7572 6e20 7265 7375 6c74 5f69   return result_i
+0000b8d0: 6e66 6f0a 0a0a 6465 6620 5f64 6973 736f  nfo...def _disso
+0000b8e0: 6c76 655f 706f 6c79 676f 6e73 5f70 6173  lve_polygons_pas
+0000b8f0: 7328 0a20 2020 2069 6e70 7574 5f70 6174  s(.    input_pat
+0000b900: 683a 2050 6174 682c 0a20 2020 206f 7574  h: Path,.    out
+0000b910: 7075 745f 6e6f 746f 6e62 6f72 6465 725f  put_notonborder_
+0000b920: 7061 7468 3a20 5061 7468 2c0a 2020 2020  path: Path,.    
+0000b930: 6f75 7470 7574 5f6f 6e62 6f72 6465 725f  output_onborder_
+0000b940: 7061 7468 3a20 5061 7468 2c0a 2020 2020  path: Path,.    
+0000b950: 6578 706c 6f64 6563 6f6c 6c65 6374 696f  explodecollectio
+0000b960: 6e73 3a20 626f 6f6c 2c0a 2020 2020 6772  ns: bool,.    gr
+0000b970: 6f75 7062 795f 636f 6c75 6d6e 733a 204f  oupby_columns: O
+0000b980: 7074 696f 6e61 6c5b 4974 6572 6162 6c65  ptional[Iterable
+0000b990: 5b73 7472 5d5d 2c0a 2020 2020 6167 675f  [str]],.    agg_
+0000b9a0: 636f 6c75 6d6e 733a 204f 7074 696f 6e61  columns: Optiona
+0000b9b0: 6c5b 6469 6374 5d2c 0a20 2020 2074 696c  l[dict],.    til
+0000b9c0: 6573 5f67 6466 3a20 6770 642e 4765 6f44  es_gdf: gpd.GeoD
+0000b9d0: 6174 6146 7261 6d65 2c0a 2020 2020 696e  ataFrame,.    in
+0000b9e0: 7075 745f 6c61 7965 723a 204f 7074 696f  put_layer: Optio
+0000b9f0: 6e61 6c5b 7374 725d 2c0a 2020 2020 6f75  nal[str],.    ou
+0000ba00: 7470 7574 5f6c 6179 6572 3a20 4f70 7469  tput_layer: Opti
+0000ba10: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2067  onal[str],.    g
+0000ba20: 7269 6473 697a 653a 2066 6c6f 6174 2c0a  ridsize: float,.
+0000ba30: 2020 2020 6e62 5f70 6172 616c 6c65 6c3a      nb_parallel:
+0000ba40: 2069 6e74 2c0a 2920 2d3e 2064 6963 743a   int,.) -> dict:
+0000ba50: 0a20 2020 2023 204d 616b 6520 7375 7265  .    # Make sure
+0000ba60: 2074 6865 2069 6e70 7574 2066 696c 6520   the input file 
+0000ba70: 6861 7320 6120 7370 6174 6961 6c20 696e  has a spatial in
+0000ba80: 6465 780a 2020 2020 6766 6f2e 6372 6561  dex.    gfo.crea
+0000ba90: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
+0000baa0: 2869 6e70 7574 5f70 6174 682c 2065 7869  (input_path, exi
+0000bab0: 7374 5f6f 6b3d 5472 7565 290a 0a20 2020  st_ok=True)..   
+0000bac0: 2023 2053 7461 7274 2063 616c 6375 6c61   # Start calcula
+0000bad0: 7469 6f6e 2069 6e20 7061 7261 6c6c 656c  tion in parallel
+0000bae0: 0a20 2020 2073 7461 7274 5f74 696d 6520  .    start_time 
+0000baf0: 3d20 6461 7465 7469 6d65 2e6e 6f77 2829  = datetime.now()
+0000bb00: 0a20 2020 2072 6573 756c 745f 696e 666f  .    result_info
+0000bb10: 203d 207b 7d0a 2020 2020 7374 6172 745f   = {}.    start_
+0000bb20: 7469 6d65 203d 2064 6174 6574 696d 652e  time = datetime.
+0000bb30: 6e6f 7728 290a 2020 2020 696e 7075 745f  now().    input_
+0000bb40: 6c61 7965 7269 6e66 6f20 3d20 6766 6f2e  layerinfo = gfo.
+0000bb50: 6765 745f 6c61 7965 7269 6e66 6f28 696e  get_layerinfo(in
+0000bb60: 7075 745f 7061 7468 2c20 696e 7075 745f  put_path, input_
+0000bb70: 6c61 7965 7229 0a0a 2020 2020 2320 5072  layer)..    # Pr
+0000bb80: 6f63 6573 7369 6e67 2069 6e20 7468 7265  ocessing in thre
+0000bb90: 6164 7320 6973 2032 7820 6661 7374 6572  ads is 2x faster
+0000bba0: 2066 6f72 2073 6d61 6c6c 2064 6174 6173   for small datas
+0000bbb0: 6574 7320 286f 6e20 5769 6e64 6f77 7329  ets (on Windows)
+0000bbc0: 0a20 2020 2063 616c 6375 6c61 7465 5f69  .    calculate_i
+0000bbd0: 6e5f 7468 7265 6164 7320 3d20 5472 7565  n_threads = True
+0000bbe0: 2069 6620 696e 7075 745f 6c61 7965 7269   if input_layeri
+0000bbf0: 6e66 6f2e 6665 6174 7572 6563 6f75 6e74  nfo.featurecount
+0000bc00: 203c 3d20 3130 3020 656c 7365 2046 616c   <= 100 else Fal
+0000bc10: 7365 0a20 2020 2077 6974 6820 5f70 726f  se.    with _pro
+0000bc20: 6365 7373 696e 675f 7574 696c 2e50 6f6f  cessing_util.Poo
+0000bc30: 6c65 6445 7865 6375 746f 7246 6163 746f  ledExecutorFacto
+0000bc40: 7279 280a 2020 2020 2020 2020 7468 7265  ry(.        thre
+0000bc50: 6164 706f 6f6c 3d63 616c 6375 6c61 7465  adpool=calculate
+0000bc60: 5f69 6e5f 7468 7265 6164 732c 0a20 2020  _in_threads,.   
+0000bc70: 2020 2020 206d 6178 5f77 6f72 6b65 7273       max_workers
+0000bc80: 3d6e 625f 7061 7261 6c6c 656c 2c0a 2020  =nb_parallel,.  
+0000bc90: 2020 2020 2020 696e 6974 6961 6c69 7a65        initialize
+0000bca0: 723d 5f70 726f 6365 7373 696e 675f 7574  r=_processing_ut
+0000bcb0: 696c 2e69 6e69 7469 616c 697a 655f 776f  il.initialize_wo
+0000bcc0: 726b 6572 2829 2c0a 2020 2020 2920 6173  rker(),.    ) as
+0000bcd0: 2063 616c 6375 6c61 7465 5f70 6f6f 6c3a   calculate_pool:
+0000bce0: 0a20 2020 2020 2020 2023 2050 7265 7061  .        # Prepa
+0000bcf0: 7265 206f 7574 7075 7420 6669 6c65 6e61  re output filena
+0000bd00: 6d65 0a20 2020 2020 2020 2074 656d 7064  me.        tempd
+0000bd10: 6972 203d 206f 7574 7075 745f 6f6e 626f  ir = output_onbo
+0000bd20: 7264 6572 5f70 6174 682e 7061 7265 6e74  rder_path.parent
+0000bd30: 0a0a 2020 2020 2020 2020 6261 7463 6865  ..        batche
+0000bd40: 7320 3d20 7b7d 0a20 2020 2020 2020 206e  s = {}.        n
+0000bd50: 625f 6261 7463 6865 7320 3d20 6c65 6e28  b_batches = len(
+0000bd60: 7469 6c65 735f 6764 6629 0a20 2020 2020  tiles_gdf).     
+0000bd70: 2020 206e 625f 6261 7463 6865 735f 646f     nb_batches_do
+0000bd80: 6e65 203d 2030 0a20 2020 2020 2020 2066  ne = 0.        f
+0000bd90: 7574 7572 655f 746f 5f62 6174 6368 5f69  uture_to_batch_i
+0000bda0: 6420 3d20 7b7d 0a20 2020 2020 2020 206e  d = {}.        n
+0000bdb0: 625f 726f 7773 5f64 6f6e 6520 3d20 300a  b_rows_done = 0.
+0000bdc0: 2020 2020 2020 2020 666f 7220 6261 7463          for batc
+0000bdd0: 685f 6964 2c20 7469 6c65 5f72 6f77 2069  h_id, tile_row i
+0000bde0: 6e20 656e 756d 6572 6174 6528 7469 6c65  n enumerate(tile
+0000bdf0: 735f 6764 662e 6974 6572 7475 706c 6573  s_gdf.itertuples
+0000be00: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+0000be10: 2062 6174 6368 6573 5b62 6174 6368 5f69   batches[batch_i
+0000be20: 645d 203d 207b 7d0a 2020 2020 2020 2020  d] = {}.        
+0000be30: 2020 2020 6261 7463 6865 735b 6261 7463      batches[batc
+0000be40: 685f 6964 5d5b 226c 6179 6572 225d 203d  h_id]["layer"] =
+0000be50: 206f 7574 7075 745f 6c61 7965 720a 2020   output_layer.  
+0000be60: 2020 2020 2020 2020 2020 6261 7463 6865            batche
+0000be70: 735b 6261 7463 685f 6964 5d5b 2262 6f75  s[batch_id]["bou
+0000be80: 6e64 7322 5d20 3d20 7469 6c65 5f72 6f77  nds"] = tile_row
+0000be90: 2e67 656f 6d65 7472 792e 626f 756e 6473  .geometry.bounds
+0000bea0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000beb0: 4f75 7470 7574 2065 6163 6820 6261 7463  Output each batc
+0000bec0: 6820 746f 2061 2073 6570 6572 6174 6520  h to a seperate 
+0000bed0: 7465 6d70 6f72 6172 7920 6669 6c65 2c20  temporary file, 
+0000bee0: 6f74 6865 7277 6973 6520 7468 6572 650a  otherwise there.
+0000bef0: 2020 2020 2020 2020 2020 2020 2320 6172              # ar
+0000bf00: 6520 7469 6d65 6f75 7420 6973 7375 6573  e timeout issues
+0000bf10: 2077 6865 6e20 7072 6f63 6573 7369 6e67   when processing
+0000bf20: 206c 6172 6765 2066 696c 6573 0a20 2020   large files.   
+0000bf30: 2020 2020 2020 2020 2073 7566 6669 7820           suffix 
+0000bf40: 3d20 6f75 7470 7574 5f6e 6f74 6f6e 626f  = output_notonbo
+0000bf50: 7264 6572 5f70 6174 682e 7375 6666 6978  rder_path.suffix
+0000bf60: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+0000bf70: 6520 3d20 6622 7b6f 7574 7075 745f 6e6f  e = f"{output_no
+0000bf80: 746f 6e62 6f72 6465 725f 7061 7468 2e73  tonborder_path.s
+0000bf90: 7465 6d7d 5f7b 6261 7463 685f 6964 7d7b  tem}_{batch_id}{
+0000bfa0: 7375 6666 6978 7d22 0a20 2020 2020 2020  suffix}".       
+0000bfb0: 2020 2020 206f 7574 7075 745f 6e6f 746f       output_noto
+0000bfc0: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
+0000bfd0: 6961 6c5f 7061 7468 203d 2074 656d 7064  ial_path = tempd
+0000bfe0: 6972 202f 206e 616d 650a 2020 2020 2020  ir / name.      
+0000bff0: 2020 2020 2020 6261 7463 6865 735b 6261        batches[ba
+0000c000: 7463 685f 6964 5d5b 0a20 2020 2020 2020  tch_id][.       
+0000c010: 2020 2020 2020 2020 2022 6f75 7470 7574           "output
+0000c020: 5f6e 6f74 6f6e 626f 7264 6572 5f74 6d70  _notonborder_tmp
+0000c030: 5f70 6172 7469 616c 5f70 6174 6822 0a20  _partial_path". 
+0000c040: 2020 2020 2020 2020 2020 205d 203d 206f             ] = o
+0000c050: 7574 7075 745f 6e6f 746f 6e62 6f72 6465  utput_notonborde
+0000c060: 725f 746d 705f 7061 7274 6961 6c5f 7061  r_tmp_partial_pa
+0000c070: 7468 0a20 2020 2020 2020 2020 2020 206e  th.            n
+0000c080: 616d 6520 3d20 6622 7b6f 7574 7075 745f  ame = f"{output_
+0000c090: 6f6e 626f 7264 6572 5f70 6174 682e 7374  onborder_path.st
+0000c0a0: 656d 7d5f 7b62 6174 6368 5f69 647d 7b73  em}_{batch_id}{s
+0000c0b0: 7566 6669 787d 220a 2020 2020 2020 2020  uffix}".        
+0000c0c0: 2020 2020 6f75 7470 7574 5f6f 6e62 6f72      output_onbor
+0000c0d0: 6465 725f 746d 705f 7061 7274 6961 6c5f  der_tmp_partial_
+0000c0e0: 7061 7468 203d 2074 656d 7064 6972 202f  path = tempdir /
+0000c0f0: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+0000c100: 2020 6261 7463 6865 735b 6261 7463 685f    batches[batch_
+0000c110: 6964 5d5b 0a20 2020 2020 2020 2020 2020  id][.           
+0000c120: 2020 2020 2022 6f75 7470 7574 5f6f 6e62       "output_onb
+0000c130: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
+0000c140: 6c5f 7061 7468 220a 2020 2020 2020 2020  l_path".        
+0000c150: 2020 2020 5d20 3d20 6f75 7470 7574 5f6f      ] = output_o
+0000c160: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
+0000c170: 6961 6c5f 7061 7468 0a0a 2020 2020 2020  ial_path..      
+0000c180: 2020 2020 2020 2320 4765 7420 7469 6c65        # Get tile
+0000c190: 5f69 6420 6966 2070 7265 7365 6e74 0a20  _id if present. 
+0000c1a0: 2020 2020 2020 2020 2020 2074 696c 655f             tile_
+0000c1b0: 6964 203d 2074 696c 655f 726f 772e 7469  id = tile_row.ti
+0000c1c0: 6c65 5f69 6420 6966 2022 7469 6c65 5f69  le_id if "tile_i
+0000c1d0: 6422 2069 6e20 7469 6c65 5f72 6f77 2e5f  d" in tile_row._
+0000c1e0: 6669 656c 6473 2065 6c73 6520 4e6f 6e65  fields else None
+0000c1f0: 0a0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
+0000c200: 7475 7265 203d 2063 616c 6375 6c61 7465  ture = calculate
+0000c210: 5f70 6f6f 6c2e 7375 626d 6974 280a 2020  _pool.submit(.  
+0000c220: 2020 2020 2020 2020 2020 2020 2020 5f64                _d
+0000c230: 6973 736f 6c76 655f 706f 6c79 676f 6e73  issolve_polygons
+0000c240: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c250: 2020 696e 7075 745f 7061 7468 3d69 6e70    input_path=inp
+0000c260: 7574 5f70 6174 682c 0a20 2020 2020 2020  ut_path,.       
+0000c270: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+0000c280: 6e6f 746f 6e62 6f72 6465 725f 7061 7468  notonborder_path
+0000c290: 3d6f 7574 7075 745f 6e6f 746f 6e62 6f72  =output_notonbor
+0000c2a0: 6465 725f 746d 705f 7061 7274 6961 6c5f  der_tmp_partial_
+0000c2b0: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000c2c0: 2020 2020 2020 6f75 7470 7574 5f6f 6e62        output_onb
+0000c2d0: 6f72 6465 725f 7061 7468 3d6f 7574 7075  order_path=outpu
+0000c2e0: 745f 6f6e 626f 7264 6572 5f74 6d70 5f70  t_onborder_tmp_p
+0000c2f0: 6172 7469 616c 5f70 6174 682c 0a20 2020  artial_path,.   
+0000c300: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+0000c310: 6c6f 6465 636f 6c6c 6563 7469 6f6e 733d  lodecollections=
+0000c320: 6578 706c 6f64 6563 6f6c 6c65 6374 696f  explodecollectio
+0000c330: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+0000c340: 2020 2020 6772 6f75 7062 795f 636f 6c75      groupby_colu
+0000c350: 6d6e 733d 6772 6f75 7062 795f 636f 6c75  mns=groupby_colu
+0000c360: 6d6e 732c 0a20 2020 2020 2020 2020 2020  mns,.           
+0000c370: 2020 2020 2061 6767 5f63 6f6c 756d 6e73       agg_columns
+0000c380: 3d61 6767 5f63 6f6c 756d 6e73 2c0a 2020  =agg_columns,.  
+0000c390: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000c3a0: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
+0000c3b0: 3d69 6e70 7574 5f6c 6179 6572 696e 666f  =input_layerinfo
+0000c3c0: 2e67 656f 6d65 7472 7974 7970 652c 0a20  .geometrytype,. 
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c3e0: 6e70 7574 5f6c 6179 6572 3d69 6e70 7574  nput_layer=input
+0000c3f0: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+0000c400: 2020 2020 2020 2020 6f75 7470 7574 5f6c          output_l
+0000c410: 6179 6572 3d6f 7574 7075 745f 6c61 7965  ayer=output_laye
+0000c420: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000c430: 2020 2062 626f 783d 7469 6c65 5f72 6f77     bbox=tile_row
+0000c440: 2e67 656f 6d65 7472 792e 626f 756e 6473  .geometry.bounds
+0000c450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c460: 2020 7469 6c65 5f69 643d 7469 6c65 5f69    tile_id=tile_i
+0000c470: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0000c480: 2020 2067 7269 6473 697a 653d 6772 6964     gridsize=grid
+0000c490: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
+0000c4a0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000c4b0: 6675 7475 7265 5f74 6f5f 6261 7463 685f  future_to_batch_
+0000c4c0: 6964 5b66 7574 7572 655d 203d 2062 6174  id[future] = bat
+0000c4d0: 6368 5f69 640a 0a20 2020 2020 2020 2023  ch_id..        #
+0000c4e0: 204c 6f6f 7020 7469 6c6c 2061 6c6c 2070   Loop till all p
+0000c4f0: 6172 616c 6c65 6c20 7072 6f63 6573 7365  arallel processe
+0000c500: 7320 6172 6520 7265 6164 792c 2062 7574  s are ready, but
+0000c510: 2070 726f 6365 7373 2065 6163 6820 6f6e   process each on
+0000c520: 650a 2020 2020 2020 2020 2320 7468 6174  e.        # that
+0000c530: 2069 7320 7265 6164 7920 616c 7265 6164   is ready alread
+0000c540: 790a 2020 2020 2020 2020 5f67 656e 6572  y.        _gener
+0000c550: 616c 5f75 7469 6c2e 7265 706f 7274 5f70  al_util.report_p
+0000c560: 726f 6772 6573 7328 0a20 2020 2020 2020  rogress(.       
+0000c570: 2020 2020 2073 7461 7274 5f74 696d 652c       start_time,
+0000c580: 206e 625f 6261 7463 6865 735f 646f 6e65   nb_batches_done
+0000c590: 2c20 6e62 5f62 6174 6368 6573 2c20 2264  , nb_batches, "d
+0000c5a0: 6973 736f 6c76 6522 0a20 2020 2020 2020  issolve".       
+0000c5b0: 2029 0a20 2020 2020 2020 2066 6f72 2066   ).        for f
+0000c5c0: 7574 7572 6520 696e 2066 7574 7572 6573  uture in futures
+0000c5d0: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+0000c5e0: 7475 7265 5f74 6f5f 6261 7463 685f 6964  ture_to_batch_id
+0000c5f0: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+0000c600: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000c610: 2020 2020 2320 4966 2074 6865 2063 616c      # If the cal
+0000c620: 6375 6c61 7465 2067 6176 6520 7265 7375  culate gave resu
+0000c630: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
+0000c640: 2020 2020 6e62 5f62 6174 6368 6573 5f64      nb_batches_d
+0000c650: 6f6e 6520 2b3d 2031 0a20 2020 2020 2020  one += 1.       
+0000c660: 2020 2020 2020 2020 2062 6174 6368 5f69           batch_i
+0000c670: 6420 3d20 6675 7475 7265 5f74 6f5f 6261  d = future_to_ba
+0000c680: 7463 685f 6964 5b66 7574 7572 655d 0a20  tch_id[future]. 
+0000c690: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000c6a0: 6573 756c 7420 3d20 6675 7475 7265 2e72  esult = future.r
+0000c6b0: 6573 756c 7428 290a 0a20 2020 2020 2020  esult()..       
+0000c6c0: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
+0000c6d0: 6c74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  lt is not None:.
 0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6f0: 2020 2020 2020 2066 696c 656f 7073 2e5f         fileops._
-0000c700: 6170 7065 6e64 5f74 6f5f 6e6f 6c6f 636b  append_to_nolock
-0000c710: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000c720: 2020 2020 2020 2020 2020 2020 2020 7372                sr
-0000c730: 633d 6f75 7470 7574 5f6e 6f74 6f6e 626f  c=output_notonbo
-0000c740: 7264 6572 5f74 6d70 5f70 6172 7469 616c  rder_tmp_partial
-0000c750: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2064 7374 3d6f 7574 7075 745f 6e6f     dst=output_no
-0000c780: 746f 6e62 6f72 6465 725f 7061 7468 2c0a  tonborder_path,.
-0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2020 2020 2020 2020 6372 6561              crea
-0000c7b0: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
-0000c7c0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c7f0: 2020 2020 2020 2020 2020 6766 6f2e 7265            gfo.re
-0000c800: 6d6f 7665 286f 7574 7075 745f 6e6f 746f  move(output_noto
-0000c810: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
-0000c820: 6961 6c5f 7061 7468 290a 0a20 2020 2020  ial_path)..     
-0000c830: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000c840: 2049 6620 6361 6c63 756c 6174 6520 6761   If calculate ga
-0000c850: 7665 206f 6e62 6f72 6465 7220 7265 7375  ve onborder resu
-0000c860: 6c74 732c 2061 7070 656e 6420 746f 206f  lts, append to o
-0000c870: 7574 7075 740a 2020 2020 2020 2020 2020  utput.          
-0000c880: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-0000c890: 5f6f 6e62 6f72 6465 725f 746d 705f 7061  _onborder_tmp_pa
-0000c8a0: 7274 6961 6c5f 7061 7468 203d 2062 6174  rtial_path = bat
-0000c8b0: 6368 6573 5b62 6174 6368 5f69 645d 5b0a  ches[batch_id][.
-0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8d0: 2020 2020 2020 2020 226f 7574 7075 745f          "output_
-0000c8e0: 6f6e 626f 7264 6572 5f74 6d70 5f70 6172  onborder_tmp_par
-0000c8f0: 7469 616c 5f70 6174 6822 0a20 2020 2020  tial_path".     
-0000c900: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-0000c910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c920: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c940: 2020 6f75 7470 7574 5f6f 6e62 6f72 6465    output_onborde
-0000c950: 725f 746d 705f 7061 7274 6961 6c5f 7061  r_tmp_partial_pa
-0000c960: 7468 2e65 7869 7374 7328 290a 2020 2020  th.exists().    
-0000c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c980: 2020 2020 616e 6420 6f75 7470 7574 5f6f      and output_o
-0000c990: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
-0000c9a0: 6961 6c5f 7061 7468 2e73 7461 7428 292e  ial_path.stat().
-0000c9b0: 7374 5f73 697a 6520 3e20 300a 2020 2020  st_size > 0.    
-0000c9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c9e0: 2020 2020 2020 2020 2020 2066 696c 656f             fileo
-0000c9f0: 7073 2e5f 6170 7065 6e64 5f74 6f5f 6e6f  ps._append_to_no
-0000ca00: 6c6f 636b 280a 2020 2020 2020 2020 2020  lock(.          
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca20: 2020 7372 633d 6f75 7470 7574 5f6f 6e62    src=output_onb
-0000ca30: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
-0000ca40: 6c5f 7061 7468 2c0a 2020 2020 2020 2020  l_path,.        
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca60: 2020 2020 6473 743d 6f75 7470 7574 5f6f      dst=output_o
-0000ca70: 6e62 6f72 6465 725f 7061 7468 2c0a 2020  nborder_path,.  
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca90: 2020 2020 2020 2020 2020 6372 6561 7465            create
-0000caa0: 5f73 7061 7469 616c 5f69 6e64 6578 3d46  _spatial_index=F
-0000cab0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0000cac0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cae0: 2020 2020 2020 2020 6766 6f2e 7265 6d6f          gfo.remo
-0000caf0: 7665 286f 7574 7075 745f 6f6e 626f 7264  ve(output_onbord
-0000cb00: 6572 5f74 6d70 5f70 6172 7469 616c 5f70  er_tmp_partial_p
-0000cb10: 6174 6829 0a0a 2020 2020 2020 2020 2020  ath)..          
-0000cb20: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-0000cb30: 6f6e 2061 7320 6578 3a0a 2020 2020 2020  on as ex:.      
-0000cb40: 2020 2020 2020 2020 2020 6261 7463 685f            batch_
-0000cb50: 6964 203d 2066 7574 7572 655f 746f 5f62  id = future_to_b
-0000cb60: 6174 6368 5f69 645b 6675 7475 7265 5d0a  atch_id[future].
-0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb80: 6d65 7373 6167 6520 3d20 6622 4572 726f  message = f"Erro
-0000cb90: 7220 6578 6563 7574 696e 6720 7b62 6174  r executing {bat
-0000cba0: 6368 6573 5b62 6174 6368 5f69 645d 7d3a  ches[batch_id]}:
-0000cbb0: 207b 6578 7d22 0a20 2020 2020 2020 2020   {ex}".         
-0000cbc0: 2020 2020 2020 206c 6f67 6765 722e 6578         logger.ex
-0000cbd0: 6365 7074 696f 6e28 6d65 7373 6167 6529  ception(message)
-0000cbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cbf0: 2063 616c 6375 6c61 7465 5f70 6f6f 6c2e   calculate_pool.
-0000cc00: 7368 7574 646f 776e 2829 0a20 2020 2020  shutdown().     
-0000cc10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000cc20: 2045 7863 6570 7469 6f6e 286d 6573 7361   Exception(messa
-0000cc30: 6765 2920 6672 6f6d 2065 780a 0a20 2020  ge) from ex..   
-0000cc40: 2020 2020 2020 2020 2023 204c 6f67 2074           # Log t
-0000cc50: 6865 2070 726f 6772 6573 7320 616e 6420  he progress and 
-0000cc60: 7072 6564 6963 7469 6f6e 2073 7065 6564  prediction speed
-0000cc70: 0a20 2020 2020 2020 2020 2020 205f 6765  .            _ge
-0000cc80: 6e65 7261 6c5f 7574 696c 2e72 6570 6f72  neral_util.repor
-0000cc90: 745f 7072 6f67 7265 7373 280a 2020 2020  t_progress(.    
-0000cca0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-0000ccb0: 745f 7469 6d65 2c20 6e62 5f62 6174 6368  t_time, nb_batch
-0000ccc0: 6573 5f64 6f6e 652c 206e 625f 6261 7463  es_done, nb_batc
-0000ccd0: 6865 732c 2022 6469 7373 6f6c 7665 220a  hes, "dissolve".
-0000cce0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000ccf0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-0000cd00: 2244 6973 736f 6c76 6520 7061 7373 2072  "Dissolve pass r
-0000cd10: 6561 6479 2c20 746f 6f6b 207b 6461 7465  eady, took {date
-0000cd20: 7469 6d65 2e6e 6f77 2829 2d73 7461 7274  time.now()-start
-0000cd30: 5f74 696d 657d 2122 290a 0a20 2020 2072  _time}!")..    r
-0000cd40: 6574 7572 6e20 7265 7375 6c74 5f69 6e66  eturn result_inf
-0000cd50: 6f0a 0a0a 6465 6620 5f64 6973 736f 6c76  o...def _dissolv
-0000cd60: 655f 706f 6c79 676f 6e73 280a 2020 2020  e_polygons(.    
-0000cd70: 696e 7075 745f 7061 7468 3a20 5061 7468  input_path: Path
-0000cd80: 2c0a 2020 2020 6f75 7470 7574 5f6e 6f74  ,.    output_not
-0000cd90: 6f6e 626f 7264 6572 5f70 6174 683a 2050  onborder_path: P
-0000cda0: 6174 682c 0a20 2020 206f 7574 7075 745f  ath,.    output_
-0000cdb0: 6f6e 626f 7264 6572 5f70 6174 683a 2050  onborder_path: P
-0000cdc0: 6174 682c 0a20 2020 2065 7870 6c6f 6465  ath,.    explode
-0000cdd0: 636f 6c6c 6563 7469 6f6e 733a 2062 6f6f  collections: boo
-0000cde0: 6c2c 0a20 2020 2067 726f 7570 6279 5f63  l,.    groupby_c
-0000cdf0: 6f6c 756d 6e73 3a20 4f70 7469 6f6e 616c  olumns: Optional
-0000ce00: 5b49 7465 7261 626c 655b 7374 725d 5d2c  [Iterable[str]],
-0000ce10: 0a20 2020 2061 6767 5f63 6f6c 756d 6e73  .    agg_columns
-0000ce20: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
-0000ce30: 2c0a 2020 2020 696e 7075 745f 6765 6f6d  ,.    input_geom
-0000ce40: 6574 7279 7479 7065 3a20 4765 6f6d 6574  etrytype: Geomet
-0000ce50: 7279 5479 7065 2c0a 2020 2020 696e 7075  ryType,.    inpu
-0000ce60: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
-0000ce70: 6c5b 7374 725d 2c0a 2020 2020 6f75 7470  l[str],.    outp
-0000ce80: 7574 5f6c 6179 6572 3a20 4f70 7469 6f6e  ut_layer: Option
-0000ce90: 616c 5b73 7472 5d2c 0a20 2020 2062 626f  al[str],.    bbo
-0000cea0: 783a 2054 7570 6c65 5b66 6c6f 6174 2c20  x: Tuple[float, 
-0000ceb0: 666c 6f61 742c 2066 6c6f 6174 2c20 666c  float, float, fl
-0000cec0: 6f61 745d 2c0a 2020 2020 7469 6c65 5f69  oat],.    tile_i
-0000ced0: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
-0000cee0: 2c0a 2920 2d3e 2064 6963 743a 0a20 2020  ,.) -> dict:.   
-0000cef0: 2023 2049 6e69 740a 2020 2020 7065 7266   # Init.    perf
-0000cf00: 696e 666f 203d 207b 7d0a 2020 2020 7374  info = {}.    st
-0000cf10: 6172 745f 7469 6d65 203d 2064 6174 6574  art_time = datet
-0000cf20: 696d 652e 6e6f 7728 290a 2020 2020 7265  ime.now().    re
-0000cf30: 7475 726e 5f69 6e66 6f20 3d20 7b0a 2020  turn_info = {.  
-0000cf40: 2020 2020 2020 2269 6e70 7574 5f70 6174        "input_pat
-0000cf50: 6822 3a20 696e 7075 745f 7061 7468 2c0a  h": input_path,.
-0000cf60: 2020 2020 2020 2020 226f 7574 7075 745f          "output_
-0000cf70: 6e6f 746f 6e62 6f72 6465 725f 7061 7468  notonborder_path
-0000cf80: 223a 206f 7574 7075 745f 6e6f 746f 6e62  ": output_notonb
-0000cf90: 6f72 6465 725f 7061 7468 2c0a 2020 2020  order_path,.    
-0000cfa0: 2020 2020 226f 7574 7075 745f 6f6e 626f      "output_onbo
-0000cfb0: 7264 6572 5f70 6174 6822 3a20 6f75 7470  rder_path": outp
-0000cfc0: 7574 5f6f 6e62 6f72 6465 725f 7061 7468  ut_onborder_path
-0000cfd0: 2c0a 2020 2020 2020 2020 2262 626f 7822  ,.        "bbox"
-0000cfe0: 3a20 6262 6f78 2c0a 2020 2020 2020 2020  : bbox,.        
-0000cff0: 2274 696c 655f 6964 223a 2074 696c 655f  "tile_id": tile_
-0000d000: 6964 2c0a 2020 2020 2020 2020 226e 625f  id,.        "nb_
-0000d010: 726f 7773 5f64 6f6e 6522 3a20 302c 0a20  rows_done": 0,. 
-0000d020: 2020 2020 2020 2022 746f 7461 6c5f 7469         "total_ti
-0000d030: 6d65 223a 2030 2c0a 2020 2020 2020 2020  me": 0,.        
-0000d040: 2270 6572 6669 6e66 6f22 3a20 2222 2c0a  "perfinfo": "",.
-0000d050: 2020 2020 7d0a 0a20 2020 2023 2052 6561      }..    # Rea
-0000d060: 6420 616c 6c20 7265 636f 7264 7320 7468  d all records th
-0000d070: 6174 2061 7265 2069 6e20 7468 6520 6262  at are in the bb
-0000d080: 6f78 0a20 2020 2072 6574 7279 5f63 6f75  ox.    retry_cou
-0000d090: 6e74 203d 2030 0a20 2020 2073 7461 7274  nt = 0.    start
-0000d0a0: 5f72 6561 6420 3d20 6461 7465 7469 6d65  _read = datetime
-0000d0b0: 2e6e 6f77 2829 0a20 2020 2061 6767 5f63  .now().    agg_c
-0000d0c0: 6f6c 756d 6e73 5f6e 6565 6465 6420 3d20  olumns_needed = 
-0000d0d0: 4e6f 6e65 0a20 2020 2077 6869 6c65 2054  None.    while T
-0000d0e0: 7275 653a 0a20 2020 2020 2020 2074 7279  rue:.        try
-0000d0f0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-0000d100: 6c75 6d6e 735f 746f 5f72 6561 6420 3d20  lumns_to_read = 
-0000d110: 7365 7428 290a 2020 2020 2020 2020 2020  set().          
-0000d120: 2020 696e 666f 203d 2067 666f 2e67 6574    info = gfo.get
-0000d130: 5f6c 6179 6572 696e 666f 2869 6e70 7574  _layerinfo(input
-0000d140: 5f70 6174 682c 2069 6e70 7574 5f6c 6179  _path, input_lay
-0000d150: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-0000d160: 6966 2067 726f 7570 6279 5f63 6f6c 756d  if groupby_colum
-0000d170: 6e73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ns is not None:.
-0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d190: 636f 6c75 6d6e 735f 746f 5f72 6561 642e  columns_to_read.
-0000d1a0: 7570 6461 7465 2867 726f 7570 6279 5f63  update(groupby_c
-0000d1b0: 6f6c 756d 6e73 290a 2020 2020 2020 2020  olumns).        
-0000d1c0: 2020 2020 6669 645f 6173 5f69 6e64 6578      fid_as_index
-0000d1d0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-0000d1e0: 2020 2020 2069 6620 6167 675f 636f 6c75       if agg_colu
-0000d1f0: 6d6e 7320 6973 206e 6f74 204e 6f6e 653a  mns is not None:
-0000d200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d210: 2066 6964 5f61 735f 696e 6465 7820 3d20   fid_as_index = 
-0000d220: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000d230: 2020 2020 2069 6620 225f 5f44 4953 534f       if "__DISSO
-0000d240: 4c56 455f 544f 4a53 4f4e 2220 696e 2069  LVE_TOJSON" in i
-0000d250: 6e66 6f2e 636f 6c75 6d6e 733a 0a20 2020  nfo.columns:.   
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2023 2049 6620 7765 2061 7265 206e 6f74   # If we are not
-0000d280: 2069 6e20 7468 6520 6669 7273 7420 7061   in the first pa
-0000d290: 7373 2c20 7468 6520 636f 6c75 6d6e 7320  ss, the columns 
-0000d2a0: 746f 2062 6520 7265 6164 0a20 2020 2020  to be read.     
-0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000d2c0: 2061 7265 2061 6c72 6561 6479 2069 6e20   are already in 
-0000d2d0: 7468 6520 6a73 6f6e 2063 6f6c 756d 6e0a  the json column.
-0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2f0: 2020 2020 636f 6c75 6d6e 735f 746f 5f72      columns_to_r
-0000d300: 6561 642e 6164 6428 225f 5f44 4953 534f  ead.add("__DISSO
-0000d310: 4c56 455f 544f 4a53 4f4e 2229 0a20 2020  LVE_TOJSON").   
-0000d320: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000d330: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000d340: 2020 2020 2020 2023 2054 6865 2066 6972         # The fir
-0000d350: 7374 2070 6173 732c 2073 6f20 7265 6164  st pass, so read
-0000d360: 2061 6c6c 2072 656c 6576 616e 7420 636f   all relevant co
-0000d370: 6c75 6d6e 7320 746f 2063 6f64 650a 2020  lumns to code.  
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 2320 7468 656d 2069 6e20 6a73 6f6e    # them in json
-0000d3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d3b0: 2020 2020 2069 6620 226a 736f 6e22 2069       if "json" i
-0000d3c0: 6e20 6167 675f 636f 6c75 6d6e 733a 0a20  n agg_columns:. 
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 2020 2020 2061 6767 5f63 6f6c 756d         agg_colum
-0000d3f0: 6e73 5f6e 6565 6465 6420 3d20 6167 675f  ns_needed = agg_
-0000d400: 636f 6c75 6d6e 735b 226a 736f 6e22 5d0a  columns["json"].
-0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d420: 2020 2020 656c 6966 2022 636f 6c75 6d6e      elif "column
-0000d430: 7322 2069 6e20 6167 675f 636f 6c75 6d6e  s" in agg_column
-0000d440: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000d450: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
-0000d460: 6f6c 756d 6e73 5f6e 6565 6465 6420 3d20  olumns_needed = 
-0000d470: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0000d480: 2020 2020 2020 2020 2020 2020 2020 6167                ag
-0000d490: 675f 636f 6c75 6d6e 5b22 636f 6c75 6d6e  g_column["column
-0000d4a0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d4c0: 6f72 2061 6767 5f63 6f6c 756d 6e20 696e  or agg_column in
-0000d4d0: 2061 6767 5f63 6f6c 756d 6e73 5b22 636f   agg_columns["co
-0000d4e0: 6c75 6d6e 7322 5d0a 2020 2020 2020 2020  lumns"].        
-0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d500: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000d510: 2020 2020 2020 6966 2061 6767 5f63 6f6c        if agg_col
-0000d520: 756d 6e73 5f6e 6565 6465 6420 6973 206e  umns_needed is n
-0000d530: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d550: 2063 6f6c 756d 6e73 5f74 6f5f 7265 6164   columns_to_read
-0000d560: 2e75 7064 6174 6528 6167 675f 636f 6c75  .update(agg_colu
-0000d570: 6d6e 735f 6e65 6564 6564 290a 0a20 2020  mns_needed)..   
-0000d580: 2020 2020 2020 2020 2069 6e70 7574 5f67           input_g
-0000d590: 6466 203d 2067 666f 2e72 6561 645f 6669  df = gfo.read_fi
-0000d5a0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-0000d5b0: 2020 2020 7061 7468 3d69 6e70 7574 5f70      path=input_p
-0000d5c0: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0000d5d0: 2020 2020 206c 6179 6572 3d69 6e70 7574       layer=input
-0000d5e0: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
-0000d5f0: 2020 2020 2020 2020 6262 6f78 3d62 626f          bbox=bbo
-0000d600: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
-0000d610: 2020 2063 6f6c 756d 6e73 3d63 6f6c 756d     columns=colum
-0000d620: 6e73 5f74 6f5f 7265 6164 2c0a 2020 2020  ns_to_read,.    
-0000d630: 2020 2020 2020 2020 2020 2020 6669 645f              fid_
-0000d640: 6173 5f69 6e64 6578 3d66 6964 5f61 735f  as_index=fid_as_
-0000d650: 696e 6465 782c 0a20 2020 2020 2020 2020  index,.         
-0000d660: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0000d670: 2020 6966 2061 6767 5f63 6f6c 756d 6e73    if agg_columns
-0000d680: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000d690: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000d6a0: 7075 745f 6764 665b 2266 6964 5f6f 7269  put_gdf["fid_ori
-0000d6b0: 6722 5d20 3d20 696e 7075 745f 6764 662e  g"] = input_gdf.
-0000d6c0: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
-0000d6d0: 2020 2020 2020 6966 2061 6767 5f63 6f6c        if agg_col
-0000d6e0: 756d 6e73 5f6e 6565 6465 6420 6973 206e  umns_needed is n
-0000d6f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000d700: 2020 2020 2020 2020 2020 2020 2061 6767               agg
-0000d710: 5f63 6f6c 756d 6e73 5f6e 6565 6465 642e  _columns_needed.
-0000d720: 6170 7065 6e64 2822 6669 645f 6f72 6967  append("fid_orig
-0000d730: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-0000d740: 6272 6561 6b0a 2020 2020 2020 2020 6578  break.        ex
-0000d750: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0000d760: 7320 6578 3a0a 2020 2020 2020 2020 2020  s ex:.          
-0000d770: 2020 6966 2073 7472 2865 7829 203d 3d20    if str(ex) == 
-0000d780: 2264 6174 6162 6173 6520 6973 206c 6f63  "database is loc
-0000d790: 6b65 6422 3a0a 2020 2020 2020 2020 2020  ked":.          
-0000d7a0: 2020 2020 2020 6966 2072 6574 7279 5f63        if retry_c
-0000d7b0: 6f75 6e74 203c 2031 303a 0a20 2020 2020  ount < 10:.     
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d7d0: 6574 7279 5f63 6f75 6e74 202b 3d20 310a  etry_count += 1.
-0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7f0: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
-0000d800: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000d810: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000d820: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000d830: 6520 4578 6365 7074 696f 6e28 2272 6574  e Exception("ret
-0000d840: 7269 6564 2031 3020 7469 6d65 732c 2064  ried 10 times, d
-0000d850: 6174 6162 6173 6520 7374 696c 6c20 6c6f  atabase still lo
-0000d860: 636b 6564 2229 2066 726f 6d20 6578 0a20  cked") from ex. 
-0000d870: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000d880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d890: 2072 6169 7365 2065 780a 0a20 2020 2023   raise ex..    #
-0000d8a0: 2043 6865 636b 2072 6573 756c 740a 2020   Check result.  
-0000d8b0: 2020 7065 7266 696e 666f 5b22 7469 6d65    perfinfo["time
-0000d8c0: 5f72 6561 6422 5d20 3d20 2864 6174 6574  _read"] = (datet
-0000d8d0: 696d 652e 6e6f 7728 2920 2d20 7374 6172  ime.now() - star
-0000d8e0: 745f 7265 6164 292e 746f 7461 6c5f 7365  t_read).total_se
-0000d8f0: 636f 6e64 7328 290a 2020 2020 7265 7475  conds().    retu
-0000d900: 726e 5f69 6e66 6f5b 226e 625f 726f 7773  rn_info["nb_rows
-0000d910: 5f64 6f6e 6522 5d20 3d20 6c65 6e28 696e  _done"] = len(in
-0000d920: 7075 745f 6764 6629 0a20 2020 2069 6620  put_gdf).    if 
-0000d930: 7265 7475 726e 5f69 6e66 6f5b 226e 625f  return_info["nb_
-0000d940: 726f 7773 5f64 6f6e 6522 5d20 3d3d 2030  rows_done"] == 0
-0000d950: 3a0a 2020 2020 2020 2020 6d65 7373 6167  :.        messag
-0000d960: 6520 3d20 6622 4e6f 2069 6e70 7574 2067  e = f"No input g
-0000d970: 656f 6d65 7472 6965 7320 666f 756e 6420  eometries found 
-0000d980: 696e 207b 696e 7075 745f 7061 7468 7d22  in {input_path}"
-0000d990: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000d9a0: 696e 666f 286d 6573 7361 6765 290a 2020  info(message).  
-0000d9b0: 2020 2020 2020 7265 7475 726e 5f69 6e66        return_inf
-0000d9c0: 6f5b 226d 6573 7361 6765 225d 203d 206d  o["message"] = m
-0000d9d0: 6573 7361 6765 0a20 2020 2020 2020 2072  essage.        r
-0000d9e0: 6574 7572 6e5f 696e 666f 5b22 746f 7461  eturn_info["tota
-0000d9f0: 6c5f 7469 6d65 225d 203d 2028 6461 7465  l_time"] = (date
-0000da00: 7469 6d65 2e6e 6f77 2829 202d 2073 7461  time.now() - sta
-0000da10: 7274 5f74 696d 6529 2e74 6f74 616c 5f73  rt_time).total_s
-0000da20: 6563 6f6e 6473 2829 0a20 2020 2020 2020  econds().       
-0000da30: 2072 6574 7572 6e20 7265 7475 726e 5f69   return return_i
-0000da40: 6e66 6f0a 0a20 2020 2023 204e 6f77 2074  nfo..    # Now t
-0000da50: 6865 2072 6561 6c20 7072 6f63 6573 7369  he real processi
-0000da60: 6e67 0a20 2020 2069 6620 6167 675f 636f  ng.    if agg_co
-0000da70: 6c75 6d6e 7320 6973 206e 6f74 204e 6f6e  lumns is not Non
-0000da80: 653a 0a20 2020 2020 2020 2069 6620 225f  e:.        if "_
-0000da90: 5f44 4953 534f 4c56 455f 544f 4a53 4f4e  _DISSOLVE_TOJSON
-0000daa0: 2220 6e6f 7420 696e 2069 6e70 7574 5f67  " not in input_g
-0000dab0: 6466 2e63 6f6c 756d 6e73 3a0a 2020 2020  df.columns:.    
-0000dac0: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
-0000dad0: 7061 7373 202d 3e20 7075 7420 7265 6c65  pass -> put rele
-0000dae0: 7661 6e74 2063 6f6c 756d 6e73 2069 6e20  vant columns in 
-0000daf0: 6a73 6f6e 2066 6965 6c64 0a20 2020 2020  json field.     
-0000db00: 2020 2020 2020 2061 6767 6675 6e63 203d         aggfunc =
-0000db10: 207b 2274 6f5f 6a73 6f6e 223a 2061 6767   {"to_json": agg
-0000db20: 5f63 6f6c 756d 6e73 5f6e 6565 6465 647d  _columns_needed}
-0000db30: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000db40: 2020 2020 2020 2020 2020 2023 2043 6f6c             # Col
-0000db50: 756d 6e73 2061 6c72 6561 6479 2063 6f64  umns already cod
-0000db60: 6564 2069 6e20 6120 6a73 6f6e 2063 6f6c  ed in a json col
-0000db70: 756d 6e2c 2073 6f20 6d65 7267 6520 6a73  umn, so merge js
-0000db80: 6f6e 206c 6973 7473 0a20 2020 2020 2020  on lists.       
-0000db90: 2020 2020 2061 6767 6675 6e63 203d 2022       aggfunc = "
-0000dba0: 6d65 7267 655f 6a73 6f6e 5f6c 6973 7473  merge_json_lists
-0000dbb0: 220a 2020 2020 656c 7365 3a0a 2020 2020  ".    else:.    
-0000dbc0: 2020 2020 6167 6766 756e 6320 3d20 2266      aggfunc = "f
-0000dbd0: 6972 7374 220a 2020 2020 7374 6172 745f  irst".    start_
-0000dbe0: 6469 7373 6f6c 7665 203d 2064 6174 6574  dissolve = datet
-0000dbf0: 696d 652e 6e6f 7728 290a 2020 2020 6469  ime.now().    di
-0000dc00: 7373 5f67 6466 203d 205f 6469 7373 6f6c  ss_gdf = _dissol
-0000dc10: 7665 280a 2020 2020 2020 2020 6466 3d69  ve(.        df=i
-0000dc20: 6e70 7574 5f67 6466 2c20 6279 3d67 726f  nput_gdf, by=gro
-0000dc30: 7570 6279 5f63 6f6c 756d 6e73 2c20 6167  upby_columns, ag
-0000dc40: 6766 756e 633d 6167 6766 756e 632c 2061  gfunc=aggfunc, a
-0000dc50: 735f 696e 6465 783d 4661 6c73 652c 2064  s_index=False, d
-0000dc60: 726f 706e 613d 4661 6c73 650a 2020 2020  ropna=False.    
-0000dc70: 290a 2020 2020 7065 7266 696e 666f 5b22  ).    perfinfo["
-0000dc80: 7469 6d65 5f64 6973 736f 6c76 6522 5d20  time_dissolve"] 
-0000dc90: 3d20 2864 6174 6574 696d 652e 6e6f 7728  = (datetime.now(
-0000dca0: 2920 2d20 7374 6172 745f 6469 7373 6f6c  ) - start_dissol
-0000dcb0: 7665 292e 746f 7461 6c5f 7365 636f 6e64  ve).total_second
-0000dcc0: 7328 290a 0a20 2020 2023 2049 6620 6578  s()..    # If ex
-0000dcd0: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
-0000dce0: 2069 7320 5472 7565 2061 6e64 2046 6f72   is True and For
-0000dcf0: 2070 6f6c 7967 6f6e 732c 2065 7870 6c6f   polygons, explo
-0000dd00: 6465 206d 756c 7469 2d67 656f 6d65 7472  de multi-geometr
-0000dd10: 6965 732e 0a20 2020 2023 2049 6620 6e65  ies..    # If ne
-0000dd20: 6564 6564 2074 6865 7920 7769 6c6c 2062  eded they will b
-0000dd30: 6520 2763 6f6c 6c65 6374 6564 2720 6166  e 'collected' af
-0000dd40: 7465 7277 6172 6473 2074 6f20 6d75 6c74  terwards to mult
-0000dd50: 6970 6f6c 7967 6f6e 7320 6167 6169 6e2e  ipolygons again.
-0000dd60: 0a20 2020 2069 6620 6578 706c 6f64 6563  .    if explodec
-0000dd70: 6f6c 6c65 6374 696f 6e73 2069 7320 5472  ollections is Tr
-0000dd80: 7565 206f 7220 696e 7075 745f 6765 6f6d  ue or input_geom
-0000dd90: 6574 7279 7479 7065 2069 6e20 5b0a 2020  etrytype in [.  
-0000dda0: 2020 2020 2020 4765 6f6d 6574 7279 5479        GeometryTy
-0000ddb0: 7065 2e50 4f4c 5947 4f4e 2c0a 2020 2020  pe.POLYGON,.    
-0000ddc0: 2020 2020 4765 6f6d 6574 7279 5479 7065      GeometryType
-0000ddd0: 2e4d 554c 5449 504f 4c59 474f 4e2c 0a20  .MULTIPOLYGON,. 
-0000dde0: 2020 205d 3a0a 2020 2020 2020 2020 2320     ]:.        # 
-0000ddf0: 6173 7365 7274 2074 6f20 6576 6164 6520  assert to evade 
-0000de00: 7079 4c61 6e63 6520 7761 726e 696e 670a  pyLance warning.
-0000de10: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-0000de20: 7369 6e73 7461 6e63 6528 6469 7373 5f67  sinstance(diss_g
-0000de30: 6466 2c20 6770 642e 4765 6f44 6174 6146  df, gpd.GeoDataF
-0000de40: 7261 6d65 290a 2020 2020 2020 2020 6469  rame).        di
-0000de50: 7373 5f67 6466 203d 2064 6973 735f 6764  ss_gdf = diss_gd
-0000de60: 662e 6578 706c 6f64 6528 6967 6e6f 7265  f.explode(ignore
-0000de70: 5f69 6e64 6578 3d54 7275 6529 0a0a 2020  _index=True)..  
-0000de80: 2020 2320 436c 6970 2074 6865 2072 6573    # Clip the res
-0000de90: 756c 7420 6f6e 2074 6865 2062 6f72 6465  ult on the borde
-0000dea0: 7273 206f 6620 7468 6520 6262 6f78 206e  rs of the bbox n
-0000deb0: 6f74 2074 6f20 6861 7665 206f 7665 726c  ot to have overl
-0000dec0: 6170 730a 2020 2020 2320 6265 7477 6565  aps.    # betwee
-0000ded0: 6e20 7468 6520 6469 6666 6572 656e 7420  n the different 
-0000dee0: 7469 6c65 732e 0a20 2020 2023 2049 6620  tiles..    # If 
-0000def0: 7468 6973 2069 7320 6e6f 7420 6170 706c  this is not appl
-0000df00: 6965 642c 2074 6869 7320 7265 7375 6c74  ied, this result
-0000df10: 7320 696e 2073 6f6d 6520 6765 6f6d 6574  s in some geomet
-0000df20: 7269 6573 206e 6f74 2062 6569 6e67 206d  ries not being m
-0000df30: 6572 6765 640a 2020 2020 2320 6f72 2069  erged.    # or i
-0000df40: 6e20 6475 706c 6963 6174 6573 2e0a 2020  n duplicates..  
-0000df50: 2020 2320 5245 4d41 524b 3a20 666f 7220    # REMARK: for 
-0000df60: 286d 756c 7469 296c 696e 6573 7472 696e  (multi)linestrin
-0000df70: 6773 2c20 7468 6520 656e 6470 6f69 6e74  gs, the endpoint
-0000df80: 7320 6372 6561 7465 6420 6279 2074 6865  s created by the
-0000df90: 2063 6c69 7020 6172 6520 6e6f 740a 2020   clip are not.  
-0000dfa0: 2020 2320 616c 7761 7973 2074 6865 2073    # always the s
-0000dfb0: 616d 6520 6475 6520 746f 2072 6f75 6e64  ame due to round
-0000dfc0: 696e 672c 2073 6f20 6469 7373 6f6c 7669  ing, so dissolvi
-0000dfd0: 6e67 2069 6e20 6120 6e65 7874 2070 6173  ng in a next pas
-0000dfe0: 7320 646f 6573 6e27 740a 2020 2020 2320  s doesn't.    # 
-0000dff0: 616c 7761 7973 2072 6573 756c 7420 696e  always result in
-0000e000: 206c 696e 6573 7472 696e 6773 2062 6569   linestrings bei
-0000e010: 6e67 2072 652d 636f 6e6e 6563 7465 642e  ng re-connected.
-0000e020: 2e2e 2042 6563 6175 7365 2064 6973 736f  .. Because disso
-0000e030: 6c76 696e 670a 2020 2020 2320 6c69 6e65  lving.    # line
-0000e040: 7320 6973 6e27 7420 736f 2063 6f6d 7075  s isn't so compu
-0000e050: 7461 7469 6f6e 616c 6c79 2068 6561 7679  tationally heavy
-0000e060: 2061 6e79 7761 792c 2064 726f 7020 7375   anyway, drop su
-0000e070: 7070 6f72 7420 6865 7265 2e0a 2020 2020  pport here..    
-0000e080: 6966 2062 626f 7820 6973 206e 6f74 204e  if bbox is not N
-0000e090: 6f6e 653a 0a20 2020 2020 2020 2073 7461  one:.        sta
-0000e0a0: 7274 5f63 6c69 7020 3d20 6461 7465 7469  rt_clip = dateti
-0000e0b0: 6d65 2e6e 6f77 2829 0a20 2020 2020 2020  me.now().       
-0000e0c0: 2062 626f 785f 706f 6c79 676f 6e20 3d20   bbox_polygon = 
-0000e0d0: 7368 5f67 656f 6d2e 506f 6c79 676f 6e28  sh_geom.Polygon(
-0000e0e0: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000e100: 6262 6f78 5b30 5d2c 2062 626f 785b 315d  bbox[0], bbox[1]
-0000e110: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000e120: 2020 2028 6262 6f78 5b30 5d2c 2062 626f     (bbox[0], bbo
-0000e130: 785b 335d 292c 0a20 2020 2020 2020 2020  x[3]),.         
-0000e140: 2020 2020 2020 2028 6262 6f78 5b32 5d2c         (bbox[2],
-0000e150: 2062 626f 785b 335d 292c 0a20 2020 2020   bbox[3]),.     
-0000e160: 2020 2020 2020 2020 2020 2028 6262 6f78             (bbox
-0000e170: 5b32 5d2c 2062 626f 785b 315d 292c 0a20  [2], bbox[1]),. 
-0000e180: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000e190: 6262 6f78 5b30 5d2c 2062 626f 785b 315d  bbox[0], bbox[1]
-0000e1a0: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
-0000e1b0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000e1c0: 2020 2062 626f 785f 6764 6620 3d20 6770     bbox_gdf = gp
-0000e1d0: 642e 4765 6f44 6174 6146 7261 6d65 280a  d.GeoDataFrame(.
-0000e1e0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000e1f0: 3d5b 315d 2c20 6765 6f6d 6574 7279 3d5b  =[1], geometry=[
-0000e200: 6262 6f78 5f70 6f6c 7967 6f6e 5d2c 2063  bbox_polygon], c
-0000e210: 7273 3d69 6e70 7574 5f67 6466 2e63 7273  rs=input_gdf.crs
-0000e220: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-0000e230: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000e240: 2020 2020 2320 4361 7463 6820 6972 7265      # Catch irre
-0000e250: 6c65 7661 6e74 2070 616e 6461 7320 6675  levant pandas fu
-0000e260: 7475 7265 2077 6172 6e69 6e67 0a20 2020  ture warning.   
-0000e270: 2020 2020 2023 2054 4f44 4f3a 2077 6865       # TODO: whe
-0000e280: 6e20 7265 6d6f 7665 6420 696e 206c 6174  n removed in lat
-0000e290: 6572 2076 6572 7369 6f6e 206f 6620 7061  er version of pa
-0000e2a0: 6e64 6173 2c20 6361 6e20 6265 2072 656d  ndas, can be rem
-0000e2b0: 6f76 6564 2068 6572 650a 2020 2020 2020  oved here.      
-0000e2c0: 2020 7769 7468 2077 6172 6e69 6e67 732e    with warnings.
-0000e2d0: 6361 7463 685f 7761 726e 696e 6773 2829  catch_warnings()
-0000e2e0: 3a0a 2020 2020 2020 2020 2020 2020 6d65  :.            me
-0000e2f0: 7373 6167 6520 3d20 280a 2020 2020 2020  ssage = (.      
-0000e300: 2020 2020 2020 2020 2020 2249 6e20 6120            "In a 
-0000e310: 6675 7475 7265 2076 6572 7369 6f6e 2c20  future version, 
-0000e320: 6064 662e 696c 6f63 5b3a 2c20 695d 203d  `df.iloc[:, i] =
-0000e330: 206e 6577 7661 6c73 6020 7769 6c6c 2061   newvals` will a
-0000e340: 7474 656d 7074 2074 6f20 220a 2020 2020  ttempt to ".    
-0000e350: 2020 2020 2020 2020 2020 2020 2273 6574              "set
-0000e360: 2074 6865 2076 616c 7565 7320 696e 706c   the values inpl
-0000e370: 6163 6520 696e 7374 6561 6420 6f66 2061  ace instead of a
-0000e380: 6c77 6179 7320 7365 7474 696e 6720 6120  lways setting a 
-0000e390: 6e65 7720 6172 7261 792e 220a 2020 2020  new array.".    
-0000e3a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e3b0: 2020 2020 2020 7761 726e 696e 6773 2e66        warnings.f
-0000e3c0: 696c 7465 7277 6172 6e69 6e67 7328 0a20  ilterwarnings(. 
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000e3e0: 6374 696f 6e3d 2269 676e 6f72 6522 2c20  ction="ignore", 
-0000e3f0: 6361 7465 676f 7279 3d46 7574 7572 6557  category=FutureW
-0000e400: 6172 6e69 6e67 2c20 6d65 7373 6167 653d  arning, message=
-0000e410: 7265 2e65 7363 6170 6528 6d65 7373 6167  re.escape(messag
-0000e420: 6529 0a20 2020 2020 2020 2020 2020 2029  e).            )
-0000e430: 0a20 2020 2020 2020 2020 2020 2023 206b  .            # k
-0000e440: 6565 705f 6765 6f6d 5f74 7970 653d 5472  eep_geom_type=Tr
-0000e450: 7565 2067 6176 6520 736f 6d65 7469 6d65  ue gave sometime
-0000e460: 7320 6572 726f 722c 2061 6e64 2073 7469  s error, and sti
-0000e470: 6c6c 2064 6f65 7320 696e 2030 2e39 2e30  ll does in 0.9.0
-0000e480: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-0000e490: 6f20 7573 6520 6f77 6e20 696d 706c 656d  o use own implem
-0000e4a0: 656e 7461 7469 6f6e 206f 6620 6b65 6570  entation of keep
-0000e4b0: 5f67 656f 6d5f 7479 7065 0a20 2020 2020  _geom_type.     
-0000e4c0: 2020 2020 2020 2064 6973 735f 6764 6620         diss_gdf 
-0000e4d0: 3d20 6770 642e 636c 6970 2864 6973 735f  = gpd.clip(diss_
-0000e4e0: 6764 662c 2062 626f 785f 6764 6629 2020  gdf, bbox_gdf)  
-0000e4f0: 2320 2c20 6b65 6570 5f67 656f 6d5f 7479  # , keep_geom_ty
-0000e500: 7065 3d54 7275 6529 0a20 2020 2020 2020  pe=True).       
-0000e510: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
-0000e520: 7374 616e 6365 2864 6973 735f 6764 662c  stance(diss_gdf,
-0000e530: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-0000e540: 6529 0a0a 2020 2020 2020 2020 2320 4f6e  e)..        # On
-0000e550: 6c79 206b 6565 7020 6765 6f6d 6574 7269  ly keep geometri
-0000e560: 6573 206f 6620 7468 6520 7072 696d 6974  es of the primit
-0000e570: 6976 6520 7479 7065 2073 7065 6369 6669  ive type specifi
-0000e580: 6564 2061 6674 6572 2063 6c69 702e 2e2e  ed after clip...
-0000e590: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000e5a0: 6973 696e 7374 616e 6365 2864 6973 735f  isinstance(diss_
-0000e5b0: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
-0000e5c0: 4672 616d 6529 0a20 2020 2020 2020 2064  Frame).        d
-0000e5d0: 6973 735f 6764 662e 6765 6f6d 6574 7279  iss_gdf.geometry
-0000e5e0: 203d 2067 656f 7365 7269 6573 5f75 7469   = geoseries_uti
-0000e5f0: 6c2e 6765 6f6d 6574 7279 5f63 6f6c 6c65  l.geometry_colle
-0000e600: 6374 696f 6e5f 6578 7472 6163 7428 0a20  ction_extract(. 
-0000e610: 2020 2020 2020 2020 2020 2064 6973 735f             diss_
-0000e620: 6764 662e 6765 6f6d 6574 7279 2c20 696e  gdf.geometry, in
-0000e630: 7075 745f 6765 6f6d 6574 7279 7479 7065  put_geometrytype
-0000e640: 2e74 6f5f 7072 696d 6974 6976 6574 7970  .to_primitivetyp
-0000e650: 650a 2020 2020 2020 2020 290a 0a20 2020  e.        )..   
-0000e660: 2020 2020 2070 6572 6669 6e66 6f5b 2274       perfinfo["t
-0000e670: 696d 655f 636c 6970 225d 203d 2028 6461  ime_clip"] = (da
-0000e680: 7465 7469 6d65 2e6e 6f77 2829 202d 2073  tetime.now() - s
-0000e690: 7461 7274 5f63 6c69 7029 2e74 6f74 616c  tart_clip).total
-0000e6a0: 5f73 6563 6f6e 6473 2829 0a0a 2020 2020  _seconds()..    
-0000e6b0: 2320 4472 6f70 2072 6f77 7320 7769 7468  # Drop rows with
-0000e6c0: 204e 6f6e 652f 656d 7074 7920 6765 6f6d   None/empty geom
-0000e6d0: 6574 7269 6573 0a20 2020 2064 6973 735f  etries.    diss_
-0000e6e0: 6764 6620 3d20 6469 7373 5f67 6466 5b7e  gdf = diss_gdf[~
-0000e6f0: 6469 7373 5f67 6466 2e67 656f 6d65 7472  diss_gdf.geometr
-0000e700: 792e 6973 6e61 2829 5d0a 2020 2020 6469  y.isna()].    di
-0000e710: 7373 5f67 6466 203d 2064 6973 735f 6764  ss_gdf = diss_gd
-0000e720: 665b 7e64 6973 735f 6764 662e 6765 6f6d  f[~diss_gdf.geom
-0000e730: 6574 7279 2e69 735f 656d 7074 795d 0a0a  etry.is_empty]..
-0000e740: 2020 2020 2320 4966 2074 6865 7265 2069      # If there i
-0000e750: 7320 6e6f 2072 6573 756c 742c 2072 6574  s no result, ret
-0000e760: 7572 6e0a 2020 2020 6966 206c 656e 2864  urn.    if len(d
-0000e770: 6973 735f 6764 6629 203d 3d20 303a 0a20  iss_gdf) == 0:. 
-0000e780: 2020 2020 2020 206d 6573 7361 6765 203d         message =
-0000e790: 2066 2252 6573 756c 7420 6973 2065 6d70   f"Result is emp
-0000e7a0: 7479 2066 6f72 207b 696e 7075 745f 7061  ty for {input_pa
-0000e7b0: 7468 7d22 0a20 2020 2020 2020 2072 6574  th}".        ret
-0000e7c0: 7572 6e5f 696e 666f 5b22 6d65 7373 6167  urn_info["messag
-0000e7d0: 6522 5d20 3d20 6d65 7373 6167 650a 2020  e"] = message.  
-0000e7e0: 2020 2020 2020 7265 7475 726e 5f69 6e66        return_inf
-0000e7f0: 6f5b 2270 6572 6669 6e66 6f22 5d20 3d20  o["perfinfo"] = 
-0000e800: 7065 7266 696e 666f 0a20 2020 2020 2020  perfinfo.       
-0000e810: 2072 6574 7572 6e5f 696e 666f 5b22 746f   return_info["to
-0000e820: 7461 6c5f 7469 6d65 225d 203d 2028 6461  tal_time"] = (da
-0000e830: 7465 7469 6d65 2e6e 6f77 2829 202d 2073  tetime.now() - s
-0000e840: 7461 7274 5f74 696d 6529 2e74 6f74 616c  tart_time).total
-0000e850: 5f73 6563 6f6e 6473 2829 0a20 2020 2020  _seconds().     
-0000e860: 2020 2072 6574 7572 6e20 7265 7475 726e     return return
-0000e870: 5f69 6e66 6f0a 0a20 2020 2023 2041 6464  _info..    # Add
-0000e880: 2063 6f6c 756d 6e20 7769 7468 2074 696c   column with til
-0000e890: 655f 6964 0a20 2020 2069 6620 7469 6c65  e_id.    if tile
-0000e8a0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0000e8b0: 0a20 2020 2020 2020 2064 6973 735f 6764  .        diss_gd
-0000e8c0: 665b 2274 696c 655f 6964 225d 203d 2074  f["tile_id"] = t
-0000e8d0: 696c 655f 6964 0a0a 2020 2020 2320 5361  ile_id..    # Sa
-0000e8e0: 7665 2074 6865 2072 6573 756c 7420 746f  ve the result to
-0000e8f0: 2064 6573 7469 6e61 7469 6f6e 2066 696c   destination fil
-0000e900: 6528 7329 0a20 2020 2073 7461 7274 5f74  e(s).    start_t
-0000e910: 6f5f 6669 6c65 203d 2064 6174 6574 696d  o_file = datetim
-0000e920: 652e 6e6f 7728 290a 0a20 2020 2023 2049  e.now()..    # I
-0000e930: 6620 7468 6520 7469 6c65 7320 646f 6e27  f the tiles don'
-0000e940: 7420 6e65 6564 2074 6f20 6265 206d 6572  t need to be mer
-0000e950: 6765 6420 6166 7465 7277 6172 6473 2c20  ged afterwards, 
-0000e960: 7765 2063 616e 206a 7573 7420 7361 7665  we can just save
-0000e970: 2074 6865 2072 6573 756c 7420 6173 0a20   the result as. 
-0000e980: 2020 2023 2069 7420 6973 2e0a 2020 2020     # it is..    
-0000e990: 6966 2073 7472 286f 7574 7075 745f 6e6f  if str(output_no
-0000e9a0: 746f 6e62 6f72 6465 725f 7061 7468 2920  tonborder_path) 
-0000e9b0: 3d3d 2073 7472 286f 7574 7075 745f 6f6e  == str(output_on
-0000e9c0: 626f 7264 6572 5f70 6174 6829 3a0a 2020  border_path):.  
-0000e9d0: 2020 2020 2020 2320 6173 7365 7274 2074        # assert t
-0000e9e0: 6f20 6576 6164 6520 7079 4c61 6e63 6520  o evade pyLance 
-0000e9f0: 7761 726e 696e 670a 2020 2020 2020 2020  warning.        
-0000ea00: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
-0000ea10: 6528 6469 7373 5f67 6466 2c20 6770 642e  e(diss_gdf, gpd.
-0000ea20: 4765 6f44 6174 6146 7261 6d65 290a 2020  GeoDataFrame).  
-0000ea30: 2020 2020 2020 2320 5573 6520 666f 7263        # Use forc
-0000ea40: 655f 6d75 6c74 6974 7970 652c 2074 6f20  e_multitype, to 
-0000ea50: 6576 6164 6520 7761 726e 696e 6773 2077  evade warnings w
-0000ea60: 6865 6e20 736f 6d65 2062 6174 6368 6573  hen some batches
-0000ea70: 2063 6f6e 7461 696e 0a20 2020 2020 2020   contain.       
-0000ea80: 2023 2073 696e 676c 6574 7970 6520 616e   # singletype an
-0000ea90: 6420 736f 6d65 2063 6f6e 7461 696e 206d  d some contain m
-0000eaa0: 756c 7469 7479 7065 2067 656f 6d65 7472  ultitype geometr
-0000eab0: 6965 730a 2020 2020 2020 2020 6766 6f2e  ies.        gfo.
-0000eac0: 746f 5f66 696c 6528 0a20 2020 2020 2020  to_file(.       
-0000ead0: 2020 2020 2064 6973 735f 6764 662c 0a20       diss_gdf,. 
-0000eae0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-0000eaf0: 745f 6e6f 746f 6e62 6f72 6465 725f 7061  t_notonborder_pa
-0000eb00: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0000eb10: 6c61 7965 723d 6f75 7470 7574 5f6c 6179  layer=output_lay
-0000eb20: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-0000eb30: 666f 7263 655f 6d75 6c74 6974 7970 653d  force_multitype=
-0000eb40: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000eb50: 2020 696e 6465 783d 4661 6c73 652c 0a20    index=False,. 
-0000eb60: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-0000eb70: 655f 7370 6174 6961 6c5f 696e 6465 783d  e_spatial_index=
-0000eb80: 4661 6c73 652c 0a20 2020 2020 2020 2029  False,.        )
-0000eb90: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000eba0: 2020 2023 2049 6620 6e6f 742c 2073 6176     # If not, sav
-0000ebb0: 6520 7468 6520 706f 6c79 676f 6e73 206f  e the polygons o
-0000ebc0: 6e20 7468 6520 626f 7264 6572 2073 6570  n the border sep
-0000ebd0: 6572 6174 656c 790a 2020 2020 2020 2020  erately.        
-0000ebe0: 6262 6f78 5f6c 696e 6573 5f67 6466 203d  bbox_lines_gdf =
-0000ebf0: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-0000ec00: 6528 0a20 2020 2020 2020 2020 2020 2067  e(.            g
-0000ec10: 656f 6d65 7472 793d 6765 6f73 6572 6965  eometry=geoserie
-0000ec20: 735f 7574 696c 2e70 6f6c 7967 6f6e 735f  s_util.polygons_
-0000ec30: 746f 5f6c 696e 6573 2820 2023 2074 7970  to_lines(  # typ
-0000ec40: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
-0000ec50: 2020 2020 2020 2020 2020 6770 642e 4765            gpd.Ge
-0000ec60: 6f53 6572 6965 7328 5b73 685f 6765 6f6d  oSeries([sh_geom
-0000ec70: 2e62 6f78 2862 626f 785b 305d 2c20 6262  .box(bbox[0], bb
-0000ec80: 6f78 5b31 5d2c 2062 626f 785b 325d 2c20  ox[1], bbox[2], 
-0000ec90: 6262 6f78 5b33 5d29 5d29 0a20 2020 2020  bbox[3])]).     
-0000eca0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-0000ecb0: 2020 2020 2020 6372 733d 696e 7075 745f        crs=input_
-0000ecc0: 6764 662e 6372 732c 2020 2320 7479 7065  gdf.crs,  # type
-0000ecd0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-0000ece0: 2029 0a20 2020 2020 2020 206f 6e62 6f72   ).        onbor
-0000ecf0: 6465 725f 6764 6620 3d20 6770 642e 736a  der_gdf = gpd.sj
-0000ed00: 6f69 6e28 6469 7373 5f67 6466 2c20 6262  oin(diss_gdf, bb
-0000ed10: 6f78 5f6c 696e 6573 5f67 6466 2c20 7072  ox_lines_gdf, pr
-0000ed20: 6564 6963 6174 653d 2269 6e74 6572 7365  edicate="interse
-0000ed30: 6374 7322 290a 2020 2020 2020 2020 6f6e  cts").        on
-0000ed40: 626f 7264 6572 5f67 6466 2e64 726f 7028  border_gdf.drop(
-0000ed50: 2269 6e64 6578 5f72 6967 6874 222c 2061  "index_right", a
-0000ed60: 7869 733d 312c 2069 6e70 6c61 6365 3d54  xis=1, inplace=T
-0000ed70: 7275 6529 0a20 2020 2020 2020 2069 6620  rue).        if 
-0000ed80: 6c65 6e28 6f6e 626f 7264 6572 5f67 6466  len(onborder_gdf
-0000ed90: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
-0000eda0: 2020 2023 2061 7373 6572 7420 746f 2065     # assert to e
-0000edb0: 7661 6465 2070 794c 616e 6365 2077 6172  vade pyLance war
-0000edc0: 6e69 6e67 0a20 2020 2020 2020 2020 2020  ning.           
-0000edd0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-0000ede0: 6365 286f 6e62 6f72 6465 725f 6764 662c  ce(onborder_gdf,
-0000edf0: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-0000ee00: 6529 0a20 2020 2020 2020 2020 2020 2023  e).            #
-0000ee10: 2055 7365 2066 6f72 6365 5f6d 756c 7469   Use force_multi
-0000ee20: 7479 7065 2c20 746f 2065 7661 6465 2077  type, to evade w
-0000ee30: 6172 6e69 6e67 7320 7768 656e 2073 6f6d  arnings when som
-0000ee40: 6520 6261 7463 6865 7320 636f 6e74 6169  e batches contai
-0000ee50: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
-0000ee60: 7369 6e67 6c65 7479 7065 2061 6e64 2073  singletype and s
-0000ee70: 6f6d 6520 636f 6e74 6169 6e20 6d75 6c74  ome contain mult
-0000ee80: 6974 7970 6520 6765 6f6d 6574 7269 6573  itype geometries
-0000ee90: 0a20 2020 2020 2020 2020 2020 2067 666f  .            gfo
-0000eea0: 2e74 6f5f 6669 6c65 280a 2020 2020 2020  .to_file(.      
-0000eeb0: 2020 2020 2020 2020 2020 6f6e 626f 7264            onbord
-0000eec0: 6572 5f67 6466 2c0a 2020 2020 2020 2020  er_gdf,.        
-0000eed0: 2020 2020 2020 2020 6f75 7470 7574 5f6f          output_o
-0000eee0: 6e62 6f72 6465 725f 7061 7468 2c0a 2020  nborder_path,.  
-0000eef0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0000ef00: 7965 723d 6f75 7470 7574 5f6c 6179 6572  yer=output_layer
-0000ef10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ef20: 2020 666f 7263 655f 6d75 6c74 6974 7970    force_multityp
-0000ef30: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
-0000ef40: 2020 2020 2020 2020 6372 6561 7465 5f73          create_s
-0000ef50: 7061 7469 616c 5f69 6e64 6578 3d46 616c  patial_index=Fal
-0000ef60: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0000ef70: 290a 0a20 2020 2020 2020 206e 6f74 6f6e  )..        noton
-0000ef80: 626f 7264 6572 5f67 6466 203d 2064 6973  border_gdf = dis
-0000ef90: 735f 6764 665b 7e64 6973 735f 6764 662e  s_gdf[~diss_gdf.
-0000efa0: 696e 6465 782e 6973 696e 286f 6e62 6f72  index.isin(onbor
-0000efb0: 6465 725f 6764 662e 696e 6465 7829 5d0a  der_gdf.index)].
-0000efc0: 2020 2020 2020 2020 6966 206c 656e 286e          if len(n
-0000efd0: 6f74 6f6e 626f 7264 6572 5f67 6466 2920  otonborder_gdf) 
-0000efe0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-0000eff0: 2023 2061 7373 6572 7420 746f 2065 7661   # assert to eva
-0000f000: 6465 2070 794c 616e 6365 2077 6172 6e69  de pyLance warni
-0000f010: 6e67 0a20 2020 2020 2020 2020 2020 2061  ng.            a
-0000f020: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-0000f030: 286e 6f74 6f6e 626f 7264 6572 5f67 6466  (notonborder_gdf
-0000f040: 2c20 6770 642e 4765 6f44 6174 6146 7261  , gpd.GeoDataFra
-0000f050: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0000f060: 2320 5573 6520 666f 7263 655f 6d75 6c74  # Use force_mult
-0000f070: 6974 7970 652c 2074 6f20 6576 6164 6520  itype, to evade 
-0000f080: 7761 726e 696e 6773 2077 6865 6e20 736f  warnings when so
-0000f090: 6d65 2062 6174 6368 6573 2063 6f6e 7461  me batches conta
-0000f0a0: 696e 0a20 2020 2020 2020 2020 2020 2023  in.            #
-0000f0b0: 2073 696e 676c 6574 7970 6520 616e 6420   singletype and 
-0000f0c0: 736f 6d65 2063 6f6e 7461 696e 206d 756c  some contain mul
-0000f0d0: 7469 7479 7065 2067 656f 6d65 7472 6965  titype geometrie
-0000f0e0: 730a 2020 2020 2020 2020 2020 2020 6766  s.            gf
-0000f0f0: 6f2e 746f 5f66 696c 6528 0a20 2020 2020  o.to_file(.     
-0000f100: 2020 2020 2020 2020 2020 206e 6f74 6f6e             noton
-0000f110: 626f 7264 6572 5f67 6466 2c0a 2020 2020  border_gdf,.    
-0000f120: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-0000f130: 7574 5f6e 6f74 6f6e 626f 7264 6572 5f70  ut_notonborder_p
-0000f140: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0000f150: 2020 2020 206c 6179 6572 3d6f 7574 7075       layer=outpu
-0000f160: 745f 6c61 7965 722c 0a20 2020 2020 2020  t_layer,.       
-0000f170: 2020 2020 2020 2020 2066 6f72 6365 5f6d           force_m
-0000f180: 756c 7469 7479 7065 3d54 7275 652c 0a20  ultitype=True,. 
-0000f190: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f1a0: 6e64 6578 3d46 616c 7365 2c0a 2020 2020  ndex=False,.    
-0000f1b0: 2020 2020 2020 2020 2020 2020 6372 6561              crea
-0000f1c0: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
-0000f1d0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0000f1e0: 2020 2020 290a 2020 2020 7065 7266 696e      ).    perfin
-0000f1f0: 666f 5b22 7469 6d65 5f74 6f5f 6669 6c65  fo["time_to_file
-0000f200: 225d 203d 2028 6461 7465 7469 6d65 2e6e  "] = (datetime.n
-0000f210: 6f77 2829 202d 2073 7461 7274 5f74 6f5f  ow() - start_to_
-0000f220: 6669 6c65 292e 746f 7461 6c5f 7365 636f  file).total_seco
-0000f230: 6e64 7328 290a 0a20 2020 2023 2046 696e  nds()..    # Fin
-0000f240: 616c 6973 652e 2e2e 0a20 2020 206d 6573  alise....    mes
-0000f250: 7361 6765 203d 2066 2264 6973 736f 6c76  sage = f"dissolv
-0000f260: 6520 7265 6164 7920 696e 207b 6461 7465  e ready in {date
-0000f270: 7469 6d65 2e6e 6f77 2829 2d73 7461 7274  time.now()-start
-0000f280: 5f74 696d 657d 206f 6e20 7b69 6e70 7574  _time} on {input
-0000f290: 5f70 6174 687d 2122 0a20 2020 206c 6f67  _path}!".    log
-0000f2a0: 6765 722e 6465 6275 6728 6d65 7373 6167  ger.debug(messag
-0000f2b0: 6529 0a0a 2020 2020 2320 436f 6c6c 6563  e)..    # Collec
-0000f2c0: 7420 7065 7266 696e 666f 0a20 2020 2074  t perfinfo.    t
-0000f2d0: 6f74 616c 5f70 6572 665f 7469 6d65 203d  otal_perf_time =
-0000f2e0: 2030 0a20 2020 2070 6572 6673 7472 696e   0.    perfstrin
-0000f2f0: 6720 3d20 2222 0a20 2020 2066 6f72 2070  g = "".    for p
-0000f300: 6572 6663 6f64 6520 696e 2070 6572 6669  erfcode in perfi
-0000f310: 6e66 6f3a 0a20 2020 2020 2020 2074 6f74  nfo:.        tot
-0000f320: 616c 5f70 6572 665f 7469 6d65 202b 3d20  al_perf_time += 
-0000f330: 7065 7266 696e 666f 5b70 6572 6663 6f64  perfinfo[perfcod
-0000f340: 655d 0a20 2020 2020 2020 2070 6572 6673  e].        perfs
-0000f350: 7472 696e 6720 2b3d 2066 227b 7065 7266  tring += f"{perf
-0000f360: 636f 6465 7d3a 207b 7065 7266 696e 666f  code}: {perfinfo
-0000f370: 5b70 6572 6663 6f64 655d 3a2e 3266 7d2c  [perfcode]:.2f},
-0000f380: 2022 0a20 2020 2072 6574 7572 6e5f 696e   ".    return_in
-0000f390: 666f 5b22 746f 7461 6c5f 7469 6d65 225d  fo["total_time"]
-0000f3a0: 203d 2028 6461 7465 7469 6d65 2e6e 6f77   = (datetime.now
-0000f3b0: 2829 202d 2073 7461 7274 5f74 696d 6529  () - start_time)
-0000f3c0: 2e74 6f74 616c 5f73 6563 6f6e 6473 2829  .total_seconds()
-0000f3d0: 0a20 2020 2070 6572 6669 6e66 6f5b 2275  .    perfinfo["u
-0000f3e0: 6e61 6363 6f75 6e74 6564 225d 203d 2072  naccounted"] = r
-0000f3f0: 6574 7572 6e5f 696e 666f 5b22 746f 7461  eturn_info["tota
-0000f400: 6c5f 7469 6d65 225d 202d 2074 6f74 616c  l_time"] - total
-0000f410: 5f70 6572 665f 7469 6d65 0a20 2020 2070  _perf_time.    p
-0000f420: 6572 6673 7472 696e 6720 2b3d 2066 2275  erfstring += f"u
-0000f430: 6e61 6363 6f75 6e74 6564 3a20 7b70 6572  naccounted: {per
-0000f440: 6669 6e66 6f5b 2775 6e61 6363 6f75 6e74  finfo['unaccount
-0000f450: 6564 275d 3a2e 3266 7d22 0a0a 2020 2020  ed']:.2f}"..    
-0000f460: 2320 5265 7475 726e 0a20 2020 2072 6574  # Return.    ret
-0000f470: 7572 6e5f 696e 666f 5b22 7065 7266 696e  urn_info["perfin
-0000f480: 666f 225d 203d 2070 6572 6669 6e66 6f0a  fo"] = perfinfo.
-0000f490: 2020 2020 7265 7475 726e 5f69 6e66 6f5b      return_info[
-0000f4a0: 2270 6572 6673 7472 696e 6722 5d20 3d20  "perfstring"] = 
-0000f4b0: 7065 7266 7374 7269 6e67 0a20 2020 2072  perfstring.    r
-0000f4c0: 6574 7572 6e5f 696e 666f 5b22 6d65 7373  eturn_info["mess
-0000f4d0: 6167 6522 5d20 3d20 6d65 7373 6167 650a  age"] = message.
-0000f4e0: 2020 2020 7265 7475 726e 2072 6574 7572      return retur
-0000f4f0: 6e5f 696e 666f 0a0a 0a64 6566 205f 6469  n_info...def _di
-0000f500: 7373 6f6c 7665 280a 2020 2020 6466 3a20  ssolve(.    df: 
-0000f510: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
-0000f520: 2c0a 2020 2020 6279 3d4e 6f6e 652c 0a20  ,.    by=None,. 
-0000f530: 2020 2061 6767 6675 6e63 3a20 4f70 7469     aggfunc: Opti
-0000f540: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
-0000f550: 6469 6374 5d5d 203d 2022 6669 7273 7422  dict]] = "first"
-0000f560: 2c0a 2020 2020 6173 5f69 6e64 6578 3d54  ,.    as_index=T
-0000f570: 7275 652c 0a20 2020 206c 6576 656c 3d4e  rue,.    level=N
-0000f580: 6f6e 652c 0a20 2020 2073 6f72 743d 5472  one,.    sort=Tr
-0000f590: 7565 2c0a 2020 2020 6f62 7365 7276 6564  ue,.    observed
-0000f5a0: 3d46 616c 7365 2c0a 2020 2020 6472 6f70  =False,.    drop
-0000f5b0: 6e61 3d54 7275 652c 0a29 202d 3e20 6770  na=True,.) -> gp
-0000f5c0: 642e 4765 6f44 6174 6146 7261 6d65 3a0a  d.GeoDataFrame:.
-0000f5d0: 2020 2020 2222 220a 2020 2020 4469 7373      """.    Diss
-0000f5e0: 6f6c 7665 2067 656f 6d65 7472 6965 7320  olve geometries 
-0000f5f0: 7769 7468 696e 2060 6772 6f75 7062 7960  within `groupby`
-0000f600: 2069 6e74 6f20 7369 6e67 6c65 206f 6273   into single obs
-0000f610: 6572 7661 7469 6f6e 2e0a 2020 2020 5468  ervation..    Th
-0000f620: 6973 2069 7320 6163 636f 6d70 6c69 7368  is is accomplish
-0000f630: 6564 2062 7920 6170 706c 7969 6e67 2074  ed by applying t
-0000f640: 6865 2060 756e 6172 795f 756e 696f 6e60  he `unary_union`
-0000f650: 206d 6574 686f 640a 2020 2020 746f 2061   method.    to a
-0000f660: 6c6c 2067 656f 6d65 7472 6965 7320 7769  ll geometries wi
-0000f670: 7468 696e 2061 2067 726f 7570 7365 6c66  thin a groupself
-0000f680: 2e0a 2020 2020 4f62 7365 7276 6174 696f  ..    Observatio
-0000f690: 6e73 2061 7373 6f63 6961 7465 6420 7769  ns associated wi
-0000f6a0: 7468 2065 6163 6820 6067 726f 7570 6279  th each `groupby
-0000f6b0: 6020 6772 6f75 7020 7769 6c6c 2062 6520  ` group will be 
-0000f6c0: 6167 6772 6567 6174 6564 0a20 2020 2075  aggregated.    u
-0000f6d0: 7369 6e67 2074 6865 2060 6167 6766 756e  sing the `aggfun
-0000f6e0: 6360 2e0a 2020 2020 5061 7261 6d65 7465  c`..    Paramete
-0000f6f0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0000f700: 2d0a 2020 2020 6279 203a 2073 7472 696e  -.    by : strin
-0000f710: 672c 2064 6566 6175 6c74 204e 6f6e 650a  g, default None.
-0000f720: 2020 2020 2020 2020 436f 6c75 6d6e 2077          Column w
-0000f730: 686f 7365 2076 616c 7565 7320 6465 6669  hose values defi
-0000f740: 6e65 2067 726f 7570 7320 746f 2062 6520  ne groups to be 
-0000f750: 6469 7373 6f6c 7665 642e 2049 6620 4e6f  dissolved. If No
-0000f760: 6e65 2c0a 2020 2020 2020 2020 7768 6f6c  ne,.        whol
-0000f770: 6520 4765 6f44 6174 6146 7261 6d65 2069  e GeoDataFrame i
-0000f780: 7320 636f 6e73 6964 6572 6564 2061 2073  s considered a s
-0000f790: 696e 676c 6520 6772 6f75 702e 0a20 2020  ingle group..   
-0000f7a0: 2061 6767 6675 6e63 203a 2066 756e 6374   aggfunc : funct
-0000f7b0: 696f 6e2c 2073 7472 696e 6720 6f72 2064  ion, string or d
-0000f7c0: 6963 742c 2064 6566 6175 6c74 2022 6669  ict, default "fi
-0000f7d0: 7273 7422 0a20 2020 2020 2020 2041 6767  rst".        Agg
-0000f7e0: 7265 6761 7469 6f6e 2066 756e 6374 696f  regation functio
-0000f7f0: 6e20 666f 7220 6d61 6e69 7075 6c61 7469  n for manipulati
-0000f800: 6f6e 206f 6620 6461 7461 2061 7373 6f63  on of data assoc
-0000f810: 6961 7465 640a 2020 2020 2020 2020 7769  iated.        wi
-0000f820: 7468 2065 6163 6820 6772 6f75 702e 2050  th each group. P
-0000f830: 6173 7365 6420 746f 2070 616e 6461 7320  assed to pandas 
-0000f840: 6067 726f 7570 6279 2e61 6767 6020 6d65  `groupby.agg` me
-0000f850: 7468 6f64 2e0a 2020 2020 6173 5f69 6e64  thod..    as_ind
-0000f860: 6578 203a 2062 6f6f 6c65 616e 2c20 6465  ex : boolean, de
-0000f870: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
-0000f880: 2020 2049 6620 7472 7565 2c20 6772 6f75     If true, grou
-0000f890: 7062 7920 636f 6c75 6d6e 7320 6265 636f  pby columns beco
-0000f8a0: 6d65 2069 6e64 6578 206f 6620 7265 7375  me index of resu
-0000f8b0: 6c74 2e0a 2020 2020 6c65 7665 6c20 3a20  lt..    level : 
-0000f8c0: 696e 7420 6f72 2073 7472 206f 7220 7365  int or str or se
-0000f8d0: 7175 656e 6365 206f 6620 696e 7420 6f72  quence of int or
-0000f8e0: 2073 6571 7565 6e63 6520 6f66 2073 7472   sequence of str
-0000f8f0: 2c20 6465 6661 756c 7420 4e6f 6e65 0a20  , default None. 
-0000f900: 2020 2020 2020 2049 6620 7468 6520 6178         If the ax
-0000f910: 6973 2069 7320 6120 4d75 6c74 6949 6e64  is is a MultiInd
-0000f920: 6578 2028 6869 6572 6172 6368 6963 616c  ex (hierarchical
-0000f930: 292c 2067 726f 7570 2062 7920 610a 2020  ), group by a.  
-0000f940: 2020 2020 2020 7061 7274 6963 756c 6172        particular
-0000f950: 206c 6576 656c 206f 7220 6c65 7665 6c73   level or levels
-0000f960: 2e0a 2020 2020 2020 2020 2e2e 2076 6572  ..        .. ver
-0000f970: 7369 6f6e 6164 6465 643a 3a20 302e 392e  sionadded:: 0.9.
-0000f980: 300a 2020 2020 736f 7274 203a 2062 6f6f  0.    sort : boo
-0000f990: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
-0000f9a0: 2020 2020 2020 2020 536f 7274 2067 726f          Sort gro
-0000f9b0: 7570 206b 6579 732e 2047 6574 2062 6574  up keys. Get bet
-0000f9c0: 7465 7220 7065 7266 6f72 6d61 6e63 6520  ter performance 
-0000f9d0: 6279 2074 7572 6e69 6e67 2074 6869 7320  by turning this 
-0000f9e0: 6f66 662e 0a20 2020 2020 2020 204e 6f74  off..        Not
-0000f9f0: 6520 7468 6973 2064 6f65 7320 6e6f 7420  e this does not 
-0000fa00: 696e 666c 7565 6e63 6520 7468 6520 6f72  influence the or
-0000fa10: 6465 7220 6f66 206f 6273 6572 7661 7469  der of observati
-0000fa20: 6f6e 7320 7769 7468 696e 0a20 2020 2020  ons within.     
-0000fa30: 2020 2065 6163 6820 6772 6f75 702e 2047     each group. G
-0000fa40: 726f 7570 6279 2070 7265 7365 7276 6573  roupby preserves
-0000fa50: 2074 6865 206f 7264 6572 206f 6620 726f   the order of ro
-0000fa60: 7773 2077 6974 6869 6e20 6561 6368 2067  ws within each g
-0000fa70: 726f 7570 2e0a 2020 2020 2020 2020 2e2e  roup..        ..
-0000fa80: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
-0000fa90: 302e 392e 300a 2020 2020 6f62 7365 7276  0.9.0.    observ
-0000faa0: 6564 203a 2062 6f6f 6c2c 2064 6566 6175  ed : bool, defau
-0000fab0: 6c74 2046 616c 7365 0a20 2020 2020 2020  lt False.       
-0000fac0: 2054 6869 7320 6f6e 6c79 2061 7070 6c69   This only appli
-0000fad0: 6573 2069 6620 616e 7920 6f66 2074 6865  es if any of the
-0000fae0: 2067 726f 7570 6572 7320 6172 6520 4361   groupers are Ca
-0000faf0: 7465 676f 7269 6361 6c73 2e0a 2020 2020  tegoricals..    
-0000fb00: 2020 2020 4966 2054 7275 653a 206f 6e6c      If True: onl
-0000fb10: 7920 7368 6f77 206f 6273 6572 7665 6420  y show observed 
-0000fb20: 7661 6c75 6573 2066 6f72 2063 6174 6567  values for categ
-0000fb30: 6f72 6963 616c 2067 726f 7570 6572 732e  orical groupers.
-0000fb40: 0a20 2020 2020 2020 2049 6620 4661 6c73  .        If Fals
-0000fb50: 653a 2073 686f 7720 616c 6c20 7661 6c75  e: show all valu
-0000fb60: 6573 2066 6f72 2063 6174 6567 6f72 6963  es for categoric
-0000fb70: 616c 2067 726f 7570 6572 732e 0a20 2020  al groupers..   
-0000fb80: 2020 2020 202e 2e20 7665 7273 696f 6e61       .. versiona
-0000fb90: 6464 6564 3a3a 2030 2e39 2e30 0a20 2020  dded:: 0.9.0.   
-0000fba0: 2064 726f 706e 6120 3a20 626f 6f6c 2c20   dropna : bool, 
-0000fbb0: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-0000fbc0: 2020 2020 2049 6620 5472 7565 2c20 616e       If True, an
-0000fbd0: 6420 6966 2067 726f 7570 206b 6579 7320  d if group keys 
-0000fbe0: 636f 6e74 6169 6e20 4e41 2076 616c 7565  contain NA value
-0000fbf0: 732c 204e 4120 7661 6c75 6573 0a20 2020  s, NA values.   
-0000fc00: 2020 2020 2074 6f67 6574 6865 7220 7769       together wi
-0000fc10: 7468 2072 6f77 2f63 6f6c 756d 6e20 7769  th row/column wi
-0000fc20: 6c6c 2062 6520 6472 6f70 7065 642e 2049  ll be dropped. I
-0000fc30: 6620 4661 6c73 652c 204e 410a 2020 2020  f False, NA.    
-0000fc40: 2020 2020 7661 6c75 6573 2077 696c 6c20      values will 
-0000fc50: 616c 736f 2062 6520 7472 6561 7465 6420  also be treated 
-0000fc60: 6173 2074 6865 206b 6579 2069 6e20 6772  as the key in gr
-0000fc70: 6f75 7073 2e0a 2020 2020 2020 2020 5468  oups..        Th
-0000fc80: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
-0000fc90: 6e6f 7420 7375 7070 6f72 7465 6420 666f  not supported fo
-0000fca0: 7220 7061 6e64 6173 203c 2031 2e31 2e30  r pandas < 1.1.0
-0000fcb0: 2e0a 2020 2020 2020 2020 4120 7761 726e  ..        A warn
-0000fcc0: 696e 6720 7769 6c6c 2062 6520 656d 6974  ing will be emit
-0000fcd0: 7465 6420 666f 7220 6561 726c 6965 7220  ted for earlier 
-0000fce0: 7061 6e64 6173 2076 6572 7369 6f6e 730a  pandas versions.
-0000fcf0: 2020 2020 2020 2020 6966 2061 206e 6f6e          if a non
-0000fd00: 2d64 6566 6175 6c74 2076 616c 7565 2069  -default value i
-0000fd10: 7320 6769 7665 6e20 666f 7220 7468 6973  s given for this
-0000fd20: 2070 6172 616d 6574 6572 2e0a 2020 2020   parameter..    
-0000fd30: 2020 2020 2e2e 2076 6572 7369 6f6e 6164      .. versionad
-0000fd40: 6465 643a 3a20 302e 392e 300a 2020 2020  ded:: 0.9.0.    
-0000fd50: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000fd60: 2d2d 2d0a 2020 2020 4765 6f44 6174 6146  ---.    GeoDataF
-0000fd70: 7261 6d65 0a20 2020 2045 7861 6d70 6c65  rame.    Example
-0000fd80: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-0000fd90: 2020 203e 3e3e 2066 726f 6d20 7368 6170     >>> from shap
-0000fda0: 656c 792e 6765 6f6d 6574 7279 2069 6d70  ely.geometry imp
-0000fdb0: 6f72 7420 506f 696e 740a 2020 2020 3e3e  ort Point.    >>
-0000fdc0: 3e20 6420 3d20 7b0a 2020 2020 2e2e 2e20  > d = {.    ... 
-0000fdd0: 2020 2020 2263 6f6c 3122 3a20 5b22 6e61      "col1": ["na
-0000fde0: 6d65 3122 2c20 226e 616d 6532 222c 2022  me1", "name2", "
-0000fdf0: 6e61 6d65 3122 5d2c 0a20 2020 202e 2e2e  name1"],.    ...
-0000fe00: 2020 2020 2022 6765 6f6d 6574 7279 223a       "geometry":
-0000fe10: 205b 506f 696e 7428 312c 2032 292c 2050   [Point(1, 2), P
-0000fe20: 6f69 6e74 2832 2c20 3129 2c20 506f 696e  oint(2, 1), Poin
-0000fe30: 7428 302c 2031 295d 2c0a 2020 2020 2e2e  t(0, 1)],.    ..
-0000fe40: 2e20 7d0a 2020 2020 3e3e 3e20 6764 6620  . }.    >>> gdf 
-0000fe50: 3d20 6765 6f70 616e 6461 732e 4765 6f44  = geopandas.GeoD
-0000fe60: 6174 6146 7261 6d65 2864 2c20 6372 733d  ataFrame(d, crs=
-0000fe70: 3433 3236 290a 2020 2020 3e3e 3e20 6764  4326).    >>> gd
-0000fe80: 660a 2020 2020 2020 2020 636f 6c31 2020  f.        col1  
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0000fea0: 656f 6d65 7472 790a 2020 2020 3020 206e  eometry.    0  n
-0000feb0: 616d 6531 2020 504f 494e 5420 2831 2e30  ame1  POINT (1.0
-0000fec0: 3030 3030 2032 2e30 3030 3030 290a 2020  0000 2.00000).  
-0000fed0: 2020 3120 206e 616d 6532 2020 504f 494e    1  name2  POIN
-0000fee0: 5420 2832 2e30 3030 3030 2031 2e30 3030  T (2.00000 1.000
-0000fef0: 3030 290a 2020 2020 3220 206e 616d 6531  00).    2  name1
-0000ff00: 2020 504f 494e 5420 2830 2e30 3030 3030    POINT (0.00000
-0000ff10: 2031 2e30 3030 3030 290a 2020 2020 3e3e   1.00000).    >>
-0000ff20: 3e20 6469 7373 6f6c 7665 6420 3d20 6764  > dissolved = gd
-0000ff30: 662e 6469 7373 6f6c 7665 2827 636f 6c31  f.dissolve('col1
-0000ff40: 2729 0a20 2020 203e 3e3e 2064 6973 736f  ').    >>> disso
-0000ff50: 6c76 6564 2020 2320 646f 6374 6573 743a  lved  # doctest:
-0000ff60: 202b 534b 4950 0a20 2020 2020 2020 2020   +SKIP.         
-0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff90: 2020 2020 2020 2067 656f 6d65 7472 790a         geometry.
-0000ffa0: 2020 2020 636f 6c31 0a20 2020 206e 616d      col1.    nam
-0000ffb0: 6531 2020 4d55 4c54 4950 4f49 4e54 2028  e1  MULTIPOINT (
-0000ffc0: 302e 3030 3030 3020 312e 3030 3030 302c  0.00000 1.00000,
-0000ffd0: 2031 2e30 3030 3030 2032 2e30 3030 3030   1.00000 2.00000
-0000ffe0: 290a 2020 2020 6e61 6d65 3220 2020 2020  ).    name2     
-0000fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010000: 2020 2050 4f49 4e54 2028 322e 3030 3030     POINT (2.0000
-00010010: 3020 312e 3030 3030 3029 0a20 2020 2053  0 1.00000).    S
-00010020: 6565 2061 6c73 6f0a 2020 2020 2d2d 2d2d  ee also.    ----
-00010030: 2d2d 2d2d 0a20 2020 2047 656f 4461 7461  ----.    GeoData
-00010040: 4672 616d 652e 6578 706c 6f64 6520 3a20  Frame.explode : 
-00010050: 6578 706c 6f64 6520 6d75 6c74 692d 7061  explode multi-pa
-00010060: 7274 2067 656f 6d65 7472 6965 7320 696e  rt geometries in
-00010070: 746f 2073 696e 676c 6520 6765 6f6d 6574  to single geomet
-00010080: 7269 6573 0a20 2020 2022 2222 0a0a 2020  ries.    """..  
-00010090: 2020 6966 2062 7920 6973 204e 6f6e 6520    if by is None 
-000100a0: 616e 6420 6c65 7665 6c20 6973 204e 6f6e  and level is Non
-000100b0: 653a 0a20 2020 2020 2020 2062 795f 6c6f  e:.        by_lo
-000100c0: 6361 6c20 3d20 6e70 2e7a 6572 6f73 286c  cal = np.zeros(l
-000100d0: 656e 2864 6629 2c20 6474 7970 653d 2269  en(df), dtype="i
-000100e0: 6e74 3634 2229 0a20 2020 2065 6c73 653a  nt64").    else:
-000100f0: 0a20 2020 2020 2020 2062 795f 6c6f 6361  .        by_loca
-00010100: 6c20 3d20 6279 0a0a 2020 2020 6772 6f75  l = by..    grou
-00010110: 7062 795f 6b77 6172 6773 203d 2064 6963  pby_kwargs = dic
-00010120: 7428 0a20 2020 2020 2020 2062 793d 6279  t(.        by=by
-00010130: 5f6c 6f63 616c 2c20 6c65 7665 6c3d 6c65  _local, level=le
-00010140: 7665 6c2c 2073 6f72 743d 736f 7274 2c20  vel, sort=sort, 
-00010150: 6f62 7365 7276 6564 3d6f 6273 6572 7665  observed=observe
-00010160: 642c 2064 726f 706e 613d 6472 6f70 6e61  d, dropna=dropna
-00010170: 0a20 2020 2029 0a20 2020 2022 2222 0a20  .    ).    """. 
-00010180: 2020 2069 6620 6e6f 7420 636f 6d70 6174     if not compat
-00010190: 2e50 414e 4441 535f 4745 5f31 313a 0a20  .PANDAS_GE_11:. 
-000101a0: 2020 2020 2020 2067 726f 7570 6279 5f6b         groupby_k
-000101b0: 7761 7267 732e 706f 7028 2264 726f 706e  wargs.pop("dropn
-000101c0: 6122 290a 0a20 2020 2020 2020 2069 6620  a")..        if 
-000101d0: 6e6f 7420 6472 6f70 6e61 3a20 2023 2049  not dropna:  # I
-000101e0: 6620 7468 6579 2070 6173 7365 6420 6120  f they passed a 
-000101f0: 6e6f 6e2d 6465 6661 756c 7420 6472 6f70  non-default drop
-00010200: 6e61 2076 616c 7565 0a20 2020 2020 2020  na value.       
-00010210: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00010220: 726e 2822 6472 6f70 6e61 206b 7761 7267  rn("dropna kwarg
+0000c6f0: 2020 2020 6e62 5f72 6f77 735f 646f 6e65      nb_rows_done
+0000c700: 202b 3d20 7265 7375 6c74 5b22 6e62 5f72   += result["nb_r
+0000c710: 6f77 735f 646f 6e65 225d 0a20 2020 2020  ows_done"].     
+0000c720: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c730: 6620 7265 7375 6c74 5b22 6e62 5f72 6f77  f result["nb_row
+0000c740: 735f 646f 6e65 225d 203e 2030 2061 6e64  s_done"] > 0 and
+0000c750: 2072 6573 756c 745b 2274 6f74 616c 5f74   result["total_t
+0000c760: 696d 6522 5d20 3e20 303a 0a20 2020 2020  ime"] > 0:.     
+0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c780: 2020 2072 6f77 735f 7065 725f 7365 6320     rows_per_sec 
+0000c790: 3d20 726f 756e 6428 0a20 2020 2020 2020  = round(.       
+0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 2020 2072 6573 756c 745b 226e 625f       result["nb_
+0000c7c0: 726f 7773 5f64 6f6e 6522 5d20 2f20 7265  rows_done"] / re
+0000c7d0: 7375 6c74 5b22 746f 7461 6c5f 7469 6d65  sult["total_time
+0000c7e0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000c7f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c810: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000c820: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+0000c830: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000c840: 2242 6174 6368 207b 6261 7463 685f 6964  "Batch {batch_id
+0000c850: 7d20 7072 6f63 6573 7365 6420 7b72 6573  } processed {res
+0000c860: 756c 745b 276e 625f 726f 7773 5f64 6f6e  ult['nb_rows_don
+0000c870: 6527 5d7d 2072 6f77 7320 220a 2020 2020  e']} rows ".    
+0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c890: 2020 2020 2020 2020 6622 287b 726f 7773          f"({rows
+0000c8a0: 5f70 6572 5f73 6563 7d2f 7365 6329 220a  _per_sec}/sec)".
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 2020 6966 2022 7065 7266 7374 7269 6e67    if "perfstring
+0000c8f0: 2220 696e 2072 6573 756c 743a 0a20 2020  " in result:.   
+0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c910: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000c920: 6465 6275 6728 6622 5065 7266 7374 7269  debug(f"Perfstri
+0000c930: 6e67 3a20 7b72 6573 756c 745b 2770 6572  ng: {result['per
+0000c940: 6673 7472 696e 6727 5d7d 2229 0a0a 2020  fstring']}")..  
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c960: 2020 2320 5374 6172 7420 636f 7079 206f    # Start copy o
+0000c970: 6620 7468 6520 7265 7375 6c74 2074 6f20  f the result to 
+0000c980: 6120 636f 6d6d 6f6e 2066 696c 650a 2020  a common file.  
+0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9a0: 2020 6261 7463 685f 6964 203d 2066 7574    batch_id = fut
+0000c9b0: 7572 655f 746f 5f62 6174 6368 5f69 645b  ure_to_batch_id[
+0000c9c0: 6675 7475 7265 5d0a 0a20 2020 2020 2020  future]..       
+0000c9d0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
+0000c9e0: 6620 6361 6c63 756c 6174 6520 6761 7665  f calculate gave
+0000c9f0: 206e 6f74 6f6e 626f 7264 6572 2072 6573   notonborder res
+0000ca00: 756c 7473 2c20 6170 7065 6e64 2074 6f20  ults, append to 
+0000ca10: 6f75 7470 7574 0a20 2020 2020 2020 2020  output.         
+0000ca20: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0000ca30: 745f 6e6f 746f 6e62 6f72 6465 725f 746d  t_notonborder_tm
+0000ca40: 705f 7061 7274 6961 6c5f 7061 7468 203d  p_partial_path =
+0000ca50: 2062 6174 6368 6573 5b62 6174 6368 5f69   batches[batch_i
+0000ca60: 645d 5b0a 2020 2020 2020 2020 2020 2020  d][.            
+0000ca70: 2020 2020 2020 2020 2020 2020 226f 7574              "out
+0000ca80: 7075 745f 6e6f 746f 6e62 6f72 6465 725f  put_notonborder_
+0000ca90: 746d 705f 7061 7274 6961 6c5f 7061 7468  tmp_partial_path
+0000caa0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000cab0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0000cac0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0000cad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cae0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+0000caf0: 6e6f 746f 6e62 6f72 6465 725f 746d 705f  notonborder_tmp_
+0000cb00: 7061 7274 6961 6c5f 7061 7468 2e65 7869  partial_path.exi
+0000cb10: 7374 7328 290a 2020 2020 2020 2020 2020  sts().          
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0000cb30: 6420 6f75 7470 7574 5f6e 6f74 6f6e 626f  d output_notonbo
+0000cb40: 7264 6572 5f74 6d70 5f70 6172 7469 616c  rder_tmp_partial
+0000cb50: 5f70 6174 682e 7374 6174 2829 2e73 745f  _path.stat().st_
+0000cb60: 7369 7a65 203e 2030 0a20 2020 2020 2020  size > 0.       
+0000cb70: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+0000cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb90: 2020 2020 2020 2020 6669 6c65 6f70 732e          fileops.
+0000cba0: 5f61 7070 656e 645f 746f 5f6e 6f6c 6f63  _append_to_noloc
+0000cbb0: 6b28 0a20 2020 2020 2020 2020 2020 2020  k(.             
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cbd0: 7263 3d6f 7574 7075 745f 6e6f 746f 6e62  rc=output_notonb
+0000cbe0: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
+0000cbf0: 6c5f 7061 7468 2c0a 2020 2020 2020 2020  l_path,.        
+0000cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc10: 2020 2020 6473 743d 6f75 7470 7574 5f6e      dst=output_n
+0000cc20: 6f74 6f6e 626f 7264 6572 5f70 6174 682c  otonborder_path,
+0000cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc40: 2020 2020 2020 2020 2020 2020 2063 7265               cre
+0000cc50: 6174 655f 7370 6174 6961 6c5f 696e 6465  ate_spatial_inde
+0000cc60: 783d 4661 6c73 652c 0a20 2020 2020 2020  x=False,.       
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc80: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000cc90: 2020 2020 2020 2020 2020 2067 666f 2e72             gfo.r
+0000cca0: 656d 6f76 6528 6f75 7470 7574 5f6e 6f74  emove(output_not
+0000ccb0: 6f6e 626f 7264 6572 5f74 6d70 5f70 6172  onborder_tmp_par
+0000ccc0: 7469 616c 5f70 6174 6829 0a0a 2020 2020  tial_path)..    
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 2320 4966 2063 616c 6375 6c61 7465 2067  # If calculate g
+0000ccf0: 6176 6520 6f6e 626f 7264 6572 2072 6573  ave onborder res
+0000cd00: 756c 7473 2c20 6170 7065 6e64 2074 6f20  ults, append to 
+0000cd10: 6f75 7470 7574 0a20 2020 2020 2020 2020  output.         
+0000cd20: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0000cd30: 745f 6f6e 626f 7264 6572 5f74 6d70 5f70  t_onborder_tmp_p
+0000cd40: 6172 7469 616c 5f70 6174 6820 3d20 6261  artial_path = ba
+0000cd50: 7463 6865 735b 6261 7463 685f 6964 5d5b  tches[batch_id][
+0000cd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd70: 2020 2020 2020 2020 2022 6f75 7470 7574           "output
+0000cd80: 5f6f 6e62 6f72 6465 725f 746d 705f 7061  _onborder_tmp_pa
+0000cd90: 7274 6961 6c5f 7061 7468 220a 2020 2020  rtial_path".    
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000cdc0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0000cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cde0: 2020 206f 7574 7075 745f 6f6e 626f 7264     output_onbord
+0000cdf0: 6572 5f74 6d70 5f70 6172 7469 616c 5f70  er_tmp_partial_p
+0000ce00: 6174 682e 6578 6973 7473 2829 0a20 2020  ath.exists().   
+0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce20: 2020 2020 2061 6e64 206f 7574 7075 745f       and output_
+0000ce30: 6f6e 626f 7264 6572 5f74 6d70 5f70 6172  onborder_tmp_par
+0000ce40: 7469 616c 5f70 6174 682e 7374 6174 2829  tial_path.stat()
+0000ce50: 2e73 745f 7369 7a65 203e 2030 0a20 2020  .st_size > 0.   
+0000ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce70: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000ce80: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+0000ce90: 6f70 732e 5f61 7070 656e 645f 746f 5f6e  ops._append_to_n
+0000cea0: 6f6c 6f63 6b28 0a20 2020 2020 2020 2020  olock(.         
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cec0: 2020 2073 7263 3d6f 7574 7075 745f 6f6e     src=output_on
+0000ced0: 626f 7264 6572 5f74 6d70 5f70 6172 7469  border_tmp_parti
+0000cee0: 616c 5f70 6174 682c 0a20 2020 2020 2020  al_path,.       
+0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf00: 2020 2020 2064 7374 3d6f 7574 7075 745f       dst=output_
+0000cf10: 6f6e 626f 7264 6572 5f70 6174 682c 0a20  onborder_path,. 
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf30: 2020 2020 2020 2020 2020 2063 7265 6174             creat
+0000cf40: 655f 7370 6174 6961 6c5f 696e 6465 783d  e_spatial_index=
+0000cf50: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+0000cf60: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000cf70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cf80: 2020 2020 2020 2020 2067 666f 2e72 656d           gfo.rem
+0000cf90: 6f76 6528 6f75 7470 7574 5f6f 6e62 6f72  ove(output_onbor
+0000cfa0: 6465 725f 746d 705f 7061 7274 6961 6c5f  der_tmp_partial_
+0000cfb0: 7061 7468 290a 0a20 2020 2020 2020 2020  path)..         
+0000cfc0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+0000cfd0: 696f 6e20 6173 2065 783a 0a20 2020 2020  ion as ex:.     
+0000cfe0: 2020 2020 2020 2020 2020 2062 6174 6368             batch
+0000cff0: 5f69 6420 3d20 6675 7475 7265 5f74 6f5f  _id = future_to_
+0000d000: 6261 7463 685f 6964 5b66 7574 7572 655d  batch_id[future]
+0000d010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d020: 206d 6573 7361 6765 203d 2066 2245 7272   message = f"Err
+0000d030: 6f72 2065 7865 6375 7469 6e67 207b 6261  or executing {ba
+0000d040: 7463 6865 735b 6261 7463 685f 6964 5d7d  tches[batch_id]}
+0000d050: 3a20 7b65 787d 220a 2020 2020 2020 2020  : {ex}".        
+0000d060: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
+0000d070: 7863 6570 7469 6f6e 286d 6573 7361 6765  xception(message
+0000d080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d090: 2020 6361 6c63 756c 6174 655f 706f 6f6c    calculate_pool
+0000d0a0: 2e73 6875 7464 6f77 6e28 290a 2020 2020  .shutdown().    
+0000d0b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000d0c0: 6520 4578 6365 7074 696f 6e28 6d65 7373  e Exception(mess
+0000d0d0: 6167 6529 2066 726f 6d20 6578 0a0a 2020  age) from ex..  
+0000d0e0: 2020 2020 2020 2020 2020 2320 4c6f 6720            # Log 
+0000d0f0: 7468 6520 7072 6f67 7265 7373 2061 6e64  the progress and
+0000d100: 2070 7265 6469 6374 696f 6e20 7370 6565   prediction spee
+0000d110: 640a 2020 2020 2020 2020 2020 2020 5f67  d.            _g
+0000d120: 656e 6572 616c 5f75 7469 6c2e 7265 706f  eneral_util.repo
+0000d130: 7274 5f70 726f 6772 6573 7328 0a20 2020  rt_progress(.   
+0000d140: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0000d150: 7274 5f74 696d 652c 206e 625f 6261 7463  rt_time, nb_batc
+0000d160: 6865 735f 646f 6e65 2c20 6e62 5f62 6174  hes_done, nb_bat
+0000d170: 6368 6573 2c20 2264 6973 736f 6c76 6522  ches, "dissolve"
+0000d180: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+0000d190: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+0000d1a0: 6622 4469 7373 6f6c 7665 2070 6173 7320  f"Dissolve pass 
+0000d1b0: 7265 6164 792c 2074 6f6f 6b20 7b64 6174  ready, took {dat
+0000d1c0: 6574 696d 652e 6e6f 7728 292d 7374 6172  etime.now()-star
+0000d1d0: 745f 7469 6d65 7d21 2229 0a0a 2020 2020  t_time}!")..    
+0000d1e0: 7265 7475 726e 2072 6573 756c 745f 696e  return result_in
+0000d1f0: 666f 0a0a 0a64 6566 205f 6469 7373 6f6c  fo...def _dissol
+0000d200: 7665 5f70 6f6c 7967 6f6e 7328 0a20 2020  ve_polygons(.   
+0000d210: 2069 6e70 7574 5f70 6174 683a 2050 6174   input_path: Pat
+0000d220: 682c 0a20 2020 206f 7574 7075 745f 6e6f  h,.    output_no
+0000d230: 746f 6e62 6f72 6465 725f 7061 7468 3a20  tonborder_path: 
+0000d240: 5061 7468 2c0a 2020 2020 6f75 7470 7574  Path,.    output
+0000d250: 5f6f 6e62 6f72 6465 725f 7061 7468 3a20  _onborder_path: 
+0000d260: 5061 7468 2c0a 2020 2020 6578 706c 6f64  Path,.    explod
+0000d270: 6563 6f6c 6c65 6374 696f 6e73 3a20 626f  ecollections: bo
+0000d280: 6f6c 2c0a 2020 2020 6772 6f75 7062 795f  ol,.    groupby_
+0000d290: 636f 6c75 6d6e 733a 204f 7074 696f 6e61  columns: Optiona
+0000d2a0: 6c5b 4974 6572 6162 6c65 5b73 7472 5d5d  l[Iterable[str]]
+0000d2b0: 2c0a 2020 2020 6167 675f 636f 6c75 6d6e  ,.    agg_column
+0000d2c0: 733a 204f 7074 696f 6e61 6c5b 6469 6374  s: Optional[dict
+0000d2d0: 5d2c 0a20 2020 2069 6e70 7574 5f67 656f  ],.    input_geo
+0000d2e0: 6d65 7472 7974 7970 653a 2047 656f 6d65  metrytype: Geome
+0000d2f0: 7472 7954 7970 652c 0a20 2020 2069 6e70  tryType,.    inp
+0000d300: 7574 5f6c 6179 6572 3a20 4f70 7469 6f6e  ut_layer: Option
+0000d310: 616c 5b73 7472 5d2c 0a20 2020 206f 7574  al[str],.    out
+0000d320: 7075 745f 6c61 7965 723a 204f 7074 696f  put_layer: Optio
+0000d330: 6e61 6c5b 7374 725d 2c0a 2020 2020 6262  nal[str],.    bb
+0000d340: 6f78 3a20 5475 706c 655b 666c 6f61 742c  ox: Tuple[float,
+0000d350: 2066 6c6f 6174 2c20 666c 6f61 742c 2066   float, float, f
+0000d360: 6c6f 6174 5d2c 0a20 2020 2074 696c 655f  loat],.    tile_
+0000d370: 6964 3a20 4f70 7469 6f6e 616c 5b69 6e74  id: Optional[int
+0000d380: 5d2c 0a20 2020 2067 7269 6473 697a 653a  ],.    gridsize:
+0000d390: 2066 6c6f 6174 2c0a 2920 2d3e 2064 6963   float,.) -> dic
+0000d3a0: 743a 0a20 2020 2023 2049 6e69 740a 2020  t:.    # Init.  
+0000d3b0: 2020 7065 7266 696e 666f 203d 207b 7d0a    perfinfo = {}.
+0000d3c0: 2020 2020 7374 6172 745f 7469 6d65 203d      start_time =
+0000d3d0: 2064 6174 6574 696d 652e 6e6f 7728 290a   datetime.now().
+0000d3e0: 2020 2020 7265 7475 726e 5f69 6e66 6f20      return_info 
+0000d3f0: 3d20 7b0a 2020 2020 2020 2020 2269 6e70  = {.        "inp
+0000d400: 7574 5f70 6174 6822 3a20 696e 7075 745f  ut_path": input_
+0000d410: 7061 7468 2c0a 2020 2020 2020 2020 226f  path,.        "o
+0000d420: 7574 7075 745f 6e6f 746f 6e62 6f72 6465  utput_notonborde
+0000d430: 725f 7061 7468 223a 206f 7574 7075 745f  r_path": output_
+0000d440: 6e6f 746f 6e62 6f72 6465 725f 7061 7468  notonborder_path
+0000d450: 2c0a 2020 2020 2020 2020 226f 7574 7075  ,.        "outpu
+0000d460: 745f 6f6e 626f 7264 6572 5f70 6174 6822  t_onborder_path"
+0000d470: 3a20 6f75 7470 7574 5f6f 6e62 6f72 6465  : output_onborde
+0000d480: 725f 7061 7468 2c0a 2020 2020 2020 2020  r_path,.        
+0000d490: 2262 626f 7822 3a20 6262 6f78 2c0a 2020  "bbox": bbox,.  
+0000d4a0: 2020 2020 2020 2274 696c 655f 6964 223a        "tile_id":
+0000d4b0: 2074 696c 655f 6964 2c0a 2020 2020 2020   tile_id,.      
+0000d4c0: 2020 2267 7269 6473 697a 6522 3a20 6772    "gridsize": gr
+0000d4d0: 6964 7369 7a65 2c0a 2020 2020 2020 2020  idsize,.        
+0000d4e0: 226e 625f 726f 7773 5f64 6f6e 6522 3a20  "nb_rows_done": 
+0000d4f0: 302c 0a20 2020 2020 2020 2022 746f 7461  0,.        "tota
+0000d500: 6c5f 7469 6d65 223a 2030 2c0a 2020 2020  l_time": 0,.    
+0000d510: 2020 2020 2270 6572 6669 6e66 6f22 3a20      "perfinfo": 
+0000d520: 2222 2c0a 2020 2020 7d0a 0a20 2020 2023  "",.    }..    #
+0000d530: 2052 6561 6420 616c 6c20 7265 636f 7264   Read all record
+0000d540: 7320 7468 6174 2061 7265 2069 6e20 7468  s that are in th
+0000d550: 6520 6262 6f78 0a20 2020 2072 6574 7279  e bbox.    retry
+0000d560: 5f63 6f75 6e74 203d 2030 0a20 2020 2073  _count = 0.    s
+0000d570: 7461 7274 5f72 6561 6420 3d20 6461 7465  tart_read = date
+0000d580: 7469 6d65 2e6e 6f77 2829 0a20 2020 2061  time.now().    a
+0000d590: 6767 5f63 6f6c 756d 6e73 5f6e 6565 6465  gg_columns_neede
+0000d5a0: 6420 3d20 4e6f 6e65 0a20 2020 2077 6869  d = None.    whi
+0000d5b0: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
+0000d5c0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000d5d0: 2020 636f 6c75 6d6e 735f 746f 5f72 6561    columns_to_rea
+0000d5e0: 6420 3d20 7365 7428 290a 2020 2020 2020  d = set().      
+0000d5f0: 2020 2020 2020 696e 666f 203d 2067 666f        info = gfo
+0000d600: 2e67 6574 5f6c 6179 6572 696e 666f 2869  .get_layerinfo(i
+0000d610: 6e70 7574 5f70 6174 682c 2069 6e70 7574  nput_path, input
+0000d620: 5f6c 6179 6572 290a 2020 2020 2020 2020  _layer).        
+0000d630: 2020 2020 6966 2067 726f 7570 6279 5f63      if groupby_c
+0000d640: 6f6c 756d 6e73 2069 7320 6e6f 7420 4e6f  olumns is not No
+0000d650: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000d660: 2020 2020 636f 6c75 6d6e 735f 746f 5f72      columns_to_r
+0000d670: 6561 642e 7570 6461 7465 2867 726f 7570  ead.update(group
+0000d680: 6279 5f63 6f6c 756d 6e73 290a 2020 2020  by_columns).    
+0000d690: 2020 2020 2020 2020 6669 645f 6173 5f69          fid_as_i
+0000d6a0: 6e64 6578 203d 2046 616c 7365 0a20 2020  ndex = False.   
+0000d6b0: 2020 2020 2020 2020 2069 6620 6167 675f           if agg_
+0000d6c0: 636f 6c75 6d6e 7320 6973 206e 6f74 204e  columns is not N
+0000d6d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d6e0: 2020 2020 2066 6964 5f61 735f 696e 6465       fid_as_inde
+0000d6f0: 7820 3d20 5472 7565 0a20 2020 2020 2020  x = True.       
+0000d700: 2020 2020 2020 2020 2069 6620 225f 5f44           if "__D
+0000d710: 4953 534f 4c56 455f 544f 4a53 4f4e 2220  ISSOLVE_TOJSON" 
+0000d720: 696e 2069 6e66 6f2e 636f 6c75 6d6e 733a  in info.columns:
+0000d730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d740: 2020 2020 2023 2049 6620 7765 2061 7265       # If we are
+0000d750: 206e 6f74 2069 6e20 7468 6520 6669 7273   not in the firs
+0000d760: 7420 7061 7373 2c20 7468 6520 636f 6c75  t pass, the colu
+0000d770: 6d6e 7320 746f 2062 6520 7265 6164 0a20  mns to be read. 
+0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d790: 2020 2023 2061 7265 2061 6c72 6561 6479     # are already
+0000d7a0: 2069 6e20 7468 6520 6a73 6f6e 2063 6f6c   in the json col
+0000d7b0: 756d 6e0a 2020 2020 2020 2020 2020 2020  umn.            
+0000d7c0: 2020 2020 2020 2020 636f 6c75 6d6e 735f          columns_
+0000d7d0: 746f 5f72 6561 642e 6164 6428 225f 5f44  to_read.add("__D
+0000d7e0: 4953 534f 4c56 455f 544f 4a53 4f4e 2229  ISSOLVE_TOJSON")
+0000d7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d800: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d810: 2020 2020 2020 2020 2020 2023 2054 6865             # The
+0000d820: 2066 6972 7374 2070 6173 732c 2073 6f20   first pass, so 
+0000d830: 7265 6164 2061 6c6c 2072 656c 6576 616e  read all relevan
+0000d840: 7420 636f 6c75 6d6e 7320 746f 2063 6f64  t columns to cod
+0000d850: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000d860: 2020 2020 2020 2320 7468 656d 2069 6e20        # them in 
+0000d870: 6a73 6f6e 0a20 2020 2020 2020 2020 2020  json.           
+0000d880: 2020 2020 2020 2020 2069 6620 226a 736f           if "jso
+0000d890: 6e22 2069 6e20 6167 675f 636f 6c75 6d6e  n" in agg_column
+0000d8a0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000d8b0: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
+0000d8c0: 6f6c 756d 6e73 5f6e 6565 6465 6420 3d20  olumns_needed = 
+0000d8d0: 6167 675f 636f 6c75 6d6e 735b 226a 736f  agg_columns["jso
+0000d8e0: 6e22 5d0a 2020 2020 2020 2020 2020 2020  n"].            
+0000d8f0: 2020 2020 2020 2020 656c 6966 2022 636f          elif "co
+0000d900: 6c75 6d6e 7322 2069 6e20 6167 675f 636f  lumns" in agg_co
+0000d910: 6c75 6d6e 733a 0a20 2020 2020 2020 2020  lumns:.         
+0000d920: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000d930: 6767 5f63 6f6c 756d 6e73 5f6e 6565 6465  gg_columns_neede
+0000d940: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
+0000d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d960: 2020 6167 675f 636f 6c75 6d6e 5b22 636f    agg_column["co
+0000d970: 6c75 6d6e 225d 0a20 2020 2020 2020 2020  lumn"].         
+0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d990: 2020 2066 6f72 2061 6767 5f63 6f6c 756d     for agg_colum
+0000d9a0: 6e20 696e 2061 6767 5f63 6f6c 756d 6e73  n in agg_columns
+0000d9b0: 5b22 636f 6c75 6d6e 7322 5d0a 2020 2020  ["columns"].    
+0000d9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9d0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+0000d9e0: 2020 2020 2020 2020 2020 6966 2061 6767            if agg
+0000d9f0: 5f63 6f6c 756d 6e73 5f6e 6565 6465 6420  _columns_needed 
+0000da00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da20: 2020 2020 2063 6f6c 756d 6e73 5f74 6f5f       columns_to_
+0000da30: 7265 6164 2e75 7064 6174 6528 6167 675f  read.update(agg_
+0000da40: 636f 6c75 6d6e 735f 6e65 6564 6564 290a  columns_needed).
+0000da50: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
+0000da60: 7574 5f67 6466 203d 2067 666f 2e72 6561  ut_gdf = gfo.rea
+0000da70: 645f 6669 6c65 280a 2020 2020 2020 2020  d_file(.        
+0000da80: 2020 2020 2020 2020 7061 7468 3d69 6e70          path=inp
+0000da90: 7574 5f70 6174 682c 0a20 2020 2020 2020  ut_path,.       
+0000daa0: 2020 2020 2020 2020 206c 6179 6572 3d69           layer=i
+0000dab0: 6e70 7574 5f6c 6179 6572 2c0a 2020 2020  nput_layer,.    
+0000dac0: 2020 2020 2020 2020 2020 2020 6262 6f78              bbox
+0000dad0: 3d62 626f 782c 0a20 2020 2020 2020 2020  =bbox,.         
+0000dae0: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
+0000daf0: 6f6c 756d 6e73 5f74 6f5f 7265 6164 2c0a  olumns_to_read,.
+0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db10: 6669 645f 6173 5f69 6e64 6578 3d66 6964  fid_as_index=fid
+0000db20: 5f61 735f 696e 6465 782c 0a20 2020 2020  _as_index,.     
+0000db30: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000db40: 2020 2020 2020 6966 2061 6767 5f63 6f6c        if agg_col
+0000db50: 756d 6e73 2069 7320 6e6f 7420 4e6f 6e65  umns is not None
+0000db60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000db70: 2020 696e 7075 745f 6764 665b 2266 6964    input_gdf["fid
+0000db80: 5f6f 7269 6722 5d20 3d20 696e 7075 745f  _orig"] = input_
+0000db90: 6764 662e 696e 6465 780a 2020 2020 2020  gdf.index.      
+0000dba0: 2020 2020 2020 2020 2020 6966 2061 6767            if agg
+0000dbb0: 5f63 6f6c 756d 6e73 5f6e 6565 6465 6420  _columns_needed 
+0000dbc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2061 6767 5f63 6f6c 756d 6e73 5f6e 6565   agg_columns_nee
+0000dbf0: 6465 642e 6170 7065 6e64 2822 6669 645f  ded.append("fid_
+0000dc00: 6f72 6967 2229 0a0a 2020 2020 2020 2020  orig")..        
+0000dc10: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+0000dc20: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0000dc30: 6f6e 2061 7320 6578 3a0a 2020 2020 2020  on as ex:.      
+0000dc40: 2020 2020 2020 6966 2073 7472 2865 7829        if str(ex)
+0000dc50: 203d 3d20 2264 6174 6162 6173 6520 6973   == "database is
+0000dc60: 206c 6f63 6b65 6422 3a0a 2020 2020 2020   locked":.      
+0000dc70: 2020 2020 2020 2020 2020 6966 2072 6574            if ret
+0000dc80: 7279 5f63 6f75 6e74 203c 2031 303a 0a20  ry_count < 10:. 
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2072 6574 7279 5f63 6f75 6e74 202b     retry_count +
+0000dcb0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+0000dcc0: 2020 2020 2020 2020 7469 6d65 2e73 6c65          time.sle
+0000dcd0: 6570 2831 290a 2020 2020 2020 2020 2020  ep(1).          
+0000dce0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+0000dd10: 2272 6574 7269 6564 2031 3020 7469 6d65  "retried 10 time
+0000dd20: 732c 2064 6174 6162 6173 6520 7374 696c  s, database stil
+0000dd30: 6c20 6c6f 636b 6564 2229 2066 726f 6d20  l locked") from 
+0000dd40: 6578 0a20 2020 2020 2020 2020 2020 2065  ex.            e
+0000dd50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000dd60: 2020 2020 2072 6169 7365 2065 780a 0a20       raise ex.. 
+0000dd70: 2020 2023 2043 6865 636b 2072 6573 756c     # Check resul
+0000dd80: 740a 2020 2020 7065 7266 696e 666f 5b22  t.    perfinfo["
+0000dd90: 7469 6d65 5f72 6561 6422 5d20 3d20 2864  time_read"] = (d
+0000dda0: 6174 6574 696d 652e 6e6f 7728 2920 2d20  atetime.now() - 
+0000ddb0: 7374 6172 745f 7265 6164 292e 746f 7461  start_read).tota
+0000ddc0: 6c5f 7365 636f 6e64 7328 290a 2020 2020  l_seconds().    
+0000ddd0: 7265 7475 726e 5f69 6e66 6f5b 226e 625f  return_info["nb_
+0000dde0: 726f 7773 5f64 6f6e 6522 5d20 3d20 6c65  rows_done"] = le
+0000ddf0: 6e28 696e 7075 745f 6764 6629 0a20 2020  n(input_gdf).   
+0000de00: 2069 6620 7265 7475 726e 5f69 6e66 6f5b   if return_info[
+0000de10: 226e 625f 726f 7773 5f64 6f6e 6522 5d20  "nb_rows_done"] 
+0000de20: 3d3d 2030 3a0a 2020 2020 2020 2020 6d65  == 0:.        me
+0000de30: 7373 6167 6520 3d20 6622 4e6f 2069 6e70  ssage = f"No inp
+0000de40: 7574 2067 656f 6d65 7472 6965 7320 666f  ut geometries fo
+0000de50: 756e 6420 696e 207b 696e 7075 745f 7061  und in {input_pa
+0000de60: 7468 7d22 0a20 2020 2020 2020 206c 6f67  th}".        log
+0000de70: 6765 722e 696e 666f 286d 6573 7361 6765  ger.info(message
+0000de80: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000de90: 5f69 6e66 6f5b 226d 6573 7361 6765 225d  _info["message"]
+0000dea0: 203d 206d 6573 7361 6765 0a20 2020 2020   = message.     
+0000deb0: 2020 2072 6574 7572 6e5f 696e 666f 5b22     return_info["
+0000dec0: 746f 7461 6c5f 7469 6d65 225d 203d 2028  total_time"] = (
+0000ded0: 6461 7465 7469 6d65 2e6e 6f77 2829 202d  datetime.now() -
+0000dee0: 2073 7461 7274 5f74 696d 6529 2e74 6f74   start_time).tot
+0000def0: 616c 5f73 6563 6f6e 6473 2829 0a20 2020  al_seconds().   
+0000df00: 2020 2020 2072 6574 7572 6e20 7265 7475       return retu
+0000df10: 726e 5f69 6e66 6f0a 0a20 2020 2023 204e  rn_info..    # N
+0000df20: 6f77 2074 6865 2072 6561 6c20 7072 6f63  ow the real proc
+0000df30: 6573 7369 6e67 0a20 2020 2069 6620 6167  essing.    if ag
+0000df40: 675f 636f 6c75 6d6e 7320 6973 206e 6f74  g_columns is not
+0000df50: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+0000df60: 6620 225f 5f44 4953 534f 4c56 455f 544f  f "__DISSOLVE_TO
+0000df70: 4a53 4f4e 2220 6e6f 7420 696e 2069 6e70  JSON" not in inp
+0000df80: 7574 5f67 6466 2e63 6f6c 756d 6e73 3a0a  ut_gdf.columns:.
+0000df90: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
+0000dfa0: 7273 7420 7061 7373 202d 3e20 7075 7420  rst pass -> put 
+0000dfb0: 7265 6c65 7661 6e74 2063 6f6c 756d 6e73  relevant columns
+0000dfc0: 2069 6e20 6a73 6f6e 2066 6965 6c64 0a20   in json field. 
+0000dfd0: 2020 2020 2020 2020 2020 2061 6767 6675             aggfu
+0000dfe0: 6e63 203d 207b 2274 6f5f 6a73 6f6e 223a  nc = {"to_json":
+0000dff0: 2061 6767 5f63 6f6c 756d 6e73 5f6e 6565   agg_columns_nee
+0000e000: 6465 647d 0a20 2020 2020 2020 2065 6c73  ded}.        els
+0000e010: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+0000e020: 2043 6f6c 756d 6e73 2061 6c72 6561 6479   Columns already
+0000e030: 2063 6f64 6564 2069 6e20 6120 6a73 6f6e   coded in a json
+0000e040: 2063 6f6c 756d 6e2c 2073 6f20 6d65 7267   column, so merg
+0000e050: 6520 6a73 6f6e 206c 6973 7473 0a20 2020  e json lists.   
+0000e060: 2020 2020 2020 2020 2061 6767 6675 6e63           aggfunc
+0000e070: 203d 2022 6d65 7267 655f 6a73 6f6e 5f6c   = "merge_json_l
+0000e080: 6973 7473 220a 2020 2020 656c 7365 3a0a  ists".    else:.
+0000e090: 2020 2020 2020 2020 6167 6766 756e 6320          aggfunc 
+0000e0a0: 3d20 2266 6972 7374 220a 2020 2020 7374  = "first".    st
+0000e0b0: 6172 745f 6469 7373 6f6c 7665 203d 2064  art_dissolve = d
+0000e0c0: 6174 6574 696d 652e 6e6f 7728 290a 2020  atetime.now().  
+0000e0d0: 2020 6469 7373 5f67 6466 203d 205f 6469    diss_gdf = _di
+0000e0e0: 7373 6f6c 7665 280a 2020 2020 2020 2020  ssolve(.        
+0000e0f0: 6466 3d69 6e70 7574 5f67 6466 2c20 6279  df=input_gdf, by
+0000e100: 3d67 726f 7570 6279 5f63 6f6c 756d 6e73  =groupby_columns
+0000e110: 2c20 6167 6766 756e 633d 6167 6766 756e  , aggfunc=aggfun
+0000e120: 632c 2061 735f 696e 6465 783d 4661 6c73  c, as_index=Fals
+0000e130: 652c 2064 726f 706e 613d 4661 6c73 650a  e, dropna=False.
+0000e140: 2020 2020 290a 2020 2020 7065 7266 696e      ).    perfin
+0000e150: 666f 5b22 7469 6d65 5f64 6973 736f 6c76  fo["time_dissolv
+0000e160: 6522 5d20 3d20 2864 6174 6574 696d 652e  e"] = (datetime.
+0000e170: 6e6f 7728 2920 2d20 7374 6172 745f 6469  now() - start_di
+0000e180: 7373 6f6c 7665 292e 746f 7461 6c5f 7365  ssolve).total_se
+0000e190: 636f 6e64 7328 290a 0a20 2020 2023 2049  conds()..    # I
+0000e1a0: 6620 6578 706c 6f64 6563 6f6c 6c65 6374  f explodecollect
+0000e1b0: 696f 6e73 2069 7320 5472 7565 2061 6e64  ions is True and
+0000e1c0: 2046 6f72 2070 6f6c 7967 6f6e 732c 2065   For polygons, e
+0000e1d0: 7870 6c6f 6465 206d 756c 7469 2d67 656f  xplode multi-geo
+0000e1e0: 6d65 7472 6965 732e 0a20 2020 2023 2049  metries..    # I
+0000e1f0: 6620 6e65 6564 6564 2074 6865 7920 7769  f needed they wi
+0000e200: 6c6c 2062 6520 2763 6f6c 6c65 6374 6564  ll be 'collected
+0000e210: 2720 6166 7465 7277 6172 6473 2074 6f20  ' afterwards to 
+0000e220: 6d75 6c74 6970 6f6c 7967 6f6e 7320 6167  multipolygons ag
+0000e230: 6169 6e2e 0a20 2020 2069 6620 6578 706c  ain..    if expl
+0000e240: 6f64 6563 6f6c 6c65 6374 696f 6e73 2069  odecollections i
+0000e250: 7320 5472 7565 206f 7220 696e 7075 745f  s True or input_
+0000e260: 6765 6f6d 6574 7279 7479 7065 2069 6e20  geometrytype in 
+0000e270: 5b0a 2020 2020 2020 2020 4765 6f6d 6574  [.        Geomet
+0000e280: 7279 5479 7065 2e50 4f4c 5947 4f4e 2c0a  ryType.POLYGON,.
+0000e290: 2020 2020 2020 2020 4765 6f6d 6574 7279          Geometry
+0000e2a0: 5479 7065 2e4d 554c 5449 504f 4c59 474f  Type.MULTIPOLYGO
+0000e2b0: 4e2c 0a20 2020 205d 3a0a 2020 2020 2020  N,.    ]:.      
+0000e2c0: 2020 2320 6173 7365 7274 2074 6f20 6576    # assert to ev
+0000e2d0: 6164 6520 7079 4c61 6e63 6520 7761 726e  ade pyLance warn
+0000e2e0: 696e 670a 2020 2020 2020 2020 6173 7365  ing.        asse
+0000e2f0: 7274 2069 7369 6e73 7461 6e63 6528 6469  rt isinstance(di
+0000e300: 7373 5f67 6466 2c20 6770 642e 4765 6f44  ss_gdf, gpd.GeoD
+0000e310: 6174 6146 7261 6d65 290a 2020 2020 2020  ataFrame).      
+0000e320: 2020 6469 7373 5f67 6466 203d 2064 6973    diss_gdf = dis
+0000e330: 735f 6764 662e 6578 706c 6f64 6528 6967  s_gdf.explode(ig
+0000e340: 6e6f 7265 5f69 6e64 6578 3d54 7275 6529  nore_index=True)
+0000e350: 0a0a 2020 2020 2320 436c 6970 2074 6865  ..    # Clip the
+0000e360: 2072 6573 756c 7420 6f6e 2074 6865 2062   result on the b
+0000e370: 6f72 6465 7273 206f 6620 7468 6520 6262  orders of the bb
+0000e380: 6f78 206e 6f74 2074 6f20 6861 7665 206f  ox not to have o
+0000e390: 7665 726c 6170 730a 2020 2020 2320 6265  verlaps.    # be
+0000e3a0: 7477 6565 6e20 7468 6520 6469 6666 6572  tween the differ
+0000e3b0: 656e 7420 7469 6c65 732e 0a20 2020 2023  ent tiles..    #
+0000e3c0: 2049 6620 7468 6973 2069 7320 6e6f 7420   If this is not 
+0000e3d0: 6170 706c 6965 642c 2074 6869 7320 7265  applied, this re
+0000e3e0: 7375 6c74 7320 696e 2073 6f6d 6520 6765  sults in some ge
+0000e3f0: 6f6d 6574 7269 6573 206e 6f74 2062 6569  ometries not bei
+0000e400: 6e67 206d 6572 6765 640a 2020 2020 2320  ng merged.    # 
+0000e410: 6f72 2069 6e20 6475 706c 6963 6174 6573  or in duplicates
+0000e420: 2e0a 2020 2020 2320 5245 4d41 524b 3a20  ..    # REMARK: 
+0000e430: 666f 7220 286d 756c 7469 296c 696e 6573  for (multi)lines
+0000e440: 7472 696e 6773 2c20 7468 6520 656e 6470  trings, the endp
+0000e450: 6f69 6e74 7320 6372 6561 7465 6420 6279  oints created by
+0000e460: 2074 6865 2063 6c69 7020 6172 6520 6e6f   the clip are no
+0000e470: 740a 2020 2020 2320 616c 7761 7973 2074  t.    # always t
+0000e480: 6865 2073 616d 6520 6475 6520 746f 2072  he same due to r
+0000e490: 6f75 6e64 696e 672c 2073 6f20 6469 7373  ounding, so diss
+0000e4a0: 6f6c 7669 6e67 2069 6e20 6120 6e65 7874  olving in a next
+0000e4b0: 2070 6173 7320 646f 6573 6e27 740a 2020   pass doesn't.  
+0000e4c0: 2020 2320 616c 7761 7973 2072 6573 756c    # always resul
+0000e4d0: 7420 696e 206c 696e 6573 7472 696e 6773  t in linestrings
+0000e4e0: 2062 6569 6e67 2072 652d 636f 6e6e 6563   being re-connec
+0000e4f0: 7465 642e 2e2e 2042 6563 6175 7365 2064  ted... Because d
+0000e500: 6973 736f 6c76 696e 670a 2020 2020 2320  issolving.    # 
+0000e510: 6c69 6e65 7320 6973 6e27 7420 736f 2063  lines isn't so c
+0000e520: 6f6d 7075 7461 7469 6f6e 616c 6c79 2068  omputationally h
+0000e530: 6561 7679 2061 6e79 7761 792c 2064 726f  eavy anyway, dro
+0000e540: 7020 7375 7070 6f72 7420 6865 7265 2e0a  p support here..
+0000e550: 2020 2020 6966 2062 626f 7820 6973 206e      if bbox is n
+0000e560: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000e570: 2073 7461 7274 5f63 6c69 7020 3d20 6461   start_clip = da
+0000e580: 7465 7469 6d65 2e6e 6f77 2829 0a20 2020  tetime.now().   
+0000e590: 2020 2020 2062 626f 785f 706f 6c79 676f       bbox_polygo
+0000e5a0: 6e20 3d20 7368 5f67 656f 6d2e 506f 6c79  n = sh_geom.Poly
+0000e5b0: 676f 6e28 0a20 2020 2020 2020 2020 2020  gon(.           
+0000e5c0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0000e5d0: 2020 2028 6262 6f78 5b30 5d2c 2062 626f     (bbox[0], bbo
+0000e5e0: 785b 315d 292c 0a20 2020 2020 2020 2020  x[1]),.         
+0000e5f0: 2020 2020 2020 2028 6262 6f78 5b30 5d2c         (bbox[0],
+0000e600: 2062 626f 785b 335d 292c 0a20 2020 2020   bbox[3]),.     
+0000e610: 2020 2020 2020 2020 2020 2028 6262 6f78             (bbox
+0000e620: 5b32 5d2c 2062 626f 785b 335d 292c 0a20  [2], bbox[3]),. 
+0000e630: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0000e640: 6262 6f78 5b32 5d2c 2062 626f 785b 315d  bbox[2], bbox[1]
+0000e650: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000e660: 2020 2028 6262 6f78 5b30 5d2c 2062 626f     (bbox[0], bbo
+0000e670: 785b 315d 292c 0a20 2020 2020 2020 2020  x[1]),.         
+0000e680: 2020 205d 0a20 2020 2020 2020 2029 0a20     ].        ). 
+0000e690: 2020 2020 2020 2062 626f 785f 6764 6620         bbox_gdf 
+0000e6a0: 3d20 6770 642e 4765 6f44 6174 6146 7261  = gpd.GeoDataFra
+0000e6b0: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+0000e6c0: 6461 7461 3d5b 315d 2c20 6765 6f6d 6574  data=[1], geomet
+0000e6d0: 7279 3d5b 6262 6f78 5f70 6f6c 7967 6f6e  ry=[bbox_polygon
+0000e6e0: 5d2c 2063 7273 3d69 6e70 7574 5f67 6466  ], crs=input_gdf
+0000e6f0: 2e63 7273 2020 2320 7479 7065 3a20 6967  .crs  # type: ig
+0000e700: 6e6f 7265 0a20 2020 2020 2020 2029 0a0a  nore.        )..
+0000e710: 2020 2020 2020 2020 2320 4361 7463 6820          # Catch 
+0000e720: 6972 7265 6c65 7661 6e74 2070 616e 6461  irrelevant panda
+0000e730: 7320 6675 7475 7265 2077 6172 6e69 6e67  s future warning
+0000e740: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
+0000e750: 2077 6865 6e20 7265 6d6f 7665 6420 696e   when removed in
+0000e760: 206c 6174 6572 2076 6572 7369 6f6e 206f   later version o
+0000e770: 6620 7061 6e64 6173 2c20 6361 6e20 6265  f pandas, can be
+0000e780: 2072 656d 6f76 6564 2068 6572 650a 2020   removed here.  
+0000e790: 2020 2020 2020 7769 7468 2077 6172 6e69        with warni
+0000e7a0: 6e67 732e 6361 7463 685f 7761 726e 696e  ngs.catch_warnin
+0000e7b0: 6773 2829 3a0a 2020 2020 2020 2020 2020  gs():.          
+0000e7c0: 2020 6d65 7373 6167 6520 3d20 280a 2020    message = (.  
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2249                "I
+0000e7e0: 6e20 6120 6675 7475 7265 2076 6572 7369  n a future versi
+0000e7f0: 6f6e 2c20 6064 662e 696c 6f63 5b3a 2c20  on, `df.iloc[:, 
+0000e800: 695d 203d 206e 6577 7661 6c73 6020 7769  i] = newvals` wi
+0000e810: 6c6c 2061 7474 656d 7074 2074 6f20 220a  ll attempt to ".
+0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e830: 2273 6574 2074 6865 2076 616c 7565 7320  "set the values 
+0000e840: 696e 706c 6163 6520 696e 7374 6561 6420  inplace instead 
+0000e850: 6f66 2061 6c77 6179 7320 7365 7474 696e  of always settin
+0000e860: 6720 6120 6e65 7720 6172 7261 792e 220a  g a new array.".
+0000e870: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000e880: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+0000e890: 6773 2e66 696c 7465 7277 6172 6e69 6e67  gs.filterwarning
+0000e8a0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000e8b0: 2020 2061 6374 696f 6e3d 2269 676e 6f72     action="ignor
+0000e8c0: 6522 2c20 6361 7465 676f 7279 3d46 7574  e", category=Fut
+0000e8d0: 7572 6557 6172 6e69 6e67 2c20 6d65 7373  ureWarning, mess
+0000e8e0: 6167 653d 7265 2e65 7363 6170 6528 6d65  age=re.escape(me
+0000e8f0: 7373 6167 6529 0a20 2020 2020 2020 2020  ssage).         
+0000e900: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000e910: 2023 206b 6565 705f 6765 6f6d 5f74 7970   # keep_geom_typ
+0000e920: 653d 5472 7565 2067 6176 6520 736f 6d65  e=True gave some
+0000e930: 7469 6d65 7320 6572 726f 722c 2061 6e64  times error, and
+0000e940: 2073 7469 6c6c 2064 6f65 7320 696e 2030   still does in 0
+0000e950: 2e39 2e30 0a20 2020 2020 2020 2020 2020  .9.0.           
+0000e960: 2023 2073 6f20 7573 6520 6f77 6e20 696d   # so use own im
+0000e970: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+0000e980: 6b65 6570 5f67 656f 6d5f 7479 7065 0a20  keep_geom_type. 
+0000e990: 2020 2020 2020 2020 2020 2064 6973 735f             diss_
+0000e9a0: 6764 6620 3d20 6770 642e 636c 6970 2864  gdf = gpd.clip(d
+0000e9b0: 6973 735f 6764 662c 2062 626f 785f 6764  iss_gdf, bbox_gd
+0000e9c0: 6629 2020 2320 2c20 6b65 6570 5f67 656f  f)  # , keep_geo
+0000e9d0: 6d5f 7479 7065 3d54 7275 6529 0a20 2020  m_type=True).   
+0000e9e0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000e9f0: 6973 696e 7374 616e 6365 2864 6973 735f  isinstance(diss_
+0000ea00: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
+0000ea10: 4672 616d 6529 0a0a 2020 2020 2020 2020  Frame)..        
+0000ea20: 2320 4f6e 6c79 206b 6565 7020 6765 6f6d  # Only keep geom
+0000ea30: 6574 7269 6573 206f 6620 7468 6520 7072  etries of the pr
+0000ea40: 696d 6974 6976 6520 7479 7065 2073 7065  imitive type spe
+0000ea50: 6369 6669 6564 2061 6674 6572 2063 6c69  cified after cli
+0000ea60: 702e 2e2e 0a20 2020 2020 2020 2061 7373  p....        ass
+0000ea70: 6572 7420 6973 696e 7374 616e 6365 2864  ert isinstance(d
+0000ea80: 6973 735f 6764 662c 2067 7064 2e47 656f  iss_gdf, gpd.Geo
+0000ea90: 4461 7461 4672 616d 6529 0a20 2020 2020  DataFrame).     
+0000eaa0: 2020 2064 6973 735f 6764 662e 6765 6f6d     diss_gdf.geom
+0000eab0: 6574 7279 203d 2067 656f 7365 7269 6573  etry = geoseries
+0000eac0: 5f75 7469 6c2e 6765 6f6d 6574 7279 5f63  _util.geometry_c
+0000ead0: 6f6c 6c65 6374 696f 6e5f 6578 7472 6163  ollection_extrac
+0000eae0: 7428 0a20 2020 2020 2020 2020 2020 2064  t(.            d
+0000eaf0: 6973 735f 6764 662e 6765 6f6d 6574 7279  iss_gdf.geometry
+0000eb00: 2c20 696e 7075 745f 6765 6f6d 6574 7279  , input_geometry
+0000eb10: 7479 7065 2e74 6f5f 7072 696d 6974 6976  type.to_primitiv
+0000eb20: 6574 7970 650a 2020 2020 2020 2020 290a  etype.        ).
+0000eb30: 0a20 2020 2020 2020 2070 6572 6669 6e66  .        perfinf
+0000eb40: 6f5b 2274 696d 655f 636c 6970 225d 203d  o["time_clip"] =
+0000eb50: 2028 6461 7465 7469 6d65 2e6e 6f77 2829   (datetime.now()
+0000eb60: 202d 2073 7461 7274 5f63 6c69 7029 2e74   - start_clip).t
+0000eb70: 6f74 616c 5f73 6563 6f6e 6473 2829 0a0a  otal_seconds()..
+0000eb80: 2020 2020 2320 4472 6f70 2072 6f77 7320      # Drop rows 
+0000eb90: 7769 7468 204e 6f6e 652f 656d 7074 7920  with None/empty 
+0000eba0: 6765 6f6d 6574 7269 6573 0a20 2020 2064  geometries.    d
+0000ebb0: 6973 735f 6764 6620 3d20 6469 7373 5f67  iss_gdf = diss_g
+0000ebc0: 6466 5b7e 6469 7373 5f67 6466 2e67 656f  df[~diss_gdf.geo
+0000ebd0: 6d65 7472 792e 6973 6e61 2829 5d0a 2020  metry.isna()].  
+0000ebe0: 2020 6469 7373 5f67 6466 203d 2064 6973    diss_gdf = dis
+0000ebf0: 735f 6764 665b 7e64 6973 735f 6764 662e  s_gdf[~diss_gdf.
+0000ec00: 6765 6f6d 6574 7279 2e69 735f 656d 7074  geometry.is_empt
+0000ec10: 795d 0a0a 2020 2020 2320 4966 2074 6865  y]..    # If the
+0000ec20: 7265 2069 7320 6e6f 2072 6573 756c 742c  re is no result,
+0000ec30: 2072 6574 7572 6e0a 2020 2020 6966 206c   return.    if l
+0000ec40: 656e 2864 6973 735f 6764 6629 203d 3d20  en(diss_gdf) == 
+0000ec50: 303a 0a20 2020 2020 2020 206d 6573 7361  0:.        messa
+0000ec60: 6765 203d 2066 2252 6573 756c 7420 6973  ge = f"Result is
+0000ec70: 2065 6d70 7479 2066 6f72 207b 696e 7075   empty for {inpu
+0000ec80: 745f 7061 7468 7d22 0a20 2020 2020 2020  t_path}".       
+0000ec90: 2072 6574 7572 6e5f 696e 666f 5b22 6d65   return_info["me
+0000eca0: 7373 6167 6522 5d20 3d20 6d65 7373 6167  ssage"] = messag
+0000ecb0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000ecc0: 5f69 6e66 6f5b 2270 6572 6669 6e66 6f22  _info["perfinfo"
+0000ecd0: 5d20 3d20 7065 7266 696e 666f 0a20 2020  ] = perfinfo.   
+0000ece0: 2020 2020 2072 6574 7572 6e5f 696e 666f       return_info
+0000ecf0: 5b22 746f 7461 6c5f 7469 6d65 225d 203d  ["total_time"] =
+0000ed00: 2028 6461 7465 7469 6d65 2e6e 6f77 2829   (datetime.now()
+0000ed10: 202d 2073 7461 7274 5f74 696d 6529 2e74   - start_time).t
+0000ed20: 6f74 616c 5f73 6563 6f6e 6473 2829 0a20  otal_seconds(). 
+0000ed30: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000ed40: 7475 726e 5f69 6e66 6f0a 0a20 2020 2023  turn_info..    #
+0000ed50: 2041 6464 2063 6f6c 756d 6e20 7769 7468   Add column with
+0000ed60: 2074 696c 655f 6964 0a20 2020 2061 7373   tile_id.    ass
+0000ed70: 6572 7420 6973 696e 7374 616e 6365 2864  ert isinstance(d
+0000ed80: 6973 735f 6764 662c 2067 7064 2e47 656f  iss_gdf, gpd.Geo
+0000ed90: 4461 7461 4672 616d 6529 0a20 2020 2069  DataFrame).    i
+0000eda0: 6620 7469 6c65 5f69 6420 6973 206e 6f74  f tile_id is not
+0000edb0: 204e 6f6e 653a 0a20 2020 2020 2020 2064   None:.        d
+0000edc0: 6973 735f 6764 665b 2274 696c 655f 6964  iss_gdf["tile_id
+0000edd0: 225d 203d 2074 696c 655f 6964 0a0a 2020  "] = tile_id..  
+0000ede0: 2020 6966 2067 7269 6473 697a 6520 213d    if gridsize !=
+0000edf0: 2030 2e30 3a0a 2020 2020 2020 2020 6469   0.0:.        di
+0000ee00: 7373 5f67 6466 2e67 656f 6d65 7472 7920  ss_gdf.geometry 
+0000ee10: 3d20 7368 6170 656c 7932 5f6f 725f 7079  = shapely2_or_py
+0000ee20: 6765 6f73 2e73 6574 5f70 7265 6369 7369  geos.set_precisi
+0000ee30: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+0000ee40: 6469 7373 5f67 6466 2e67 656f 6d65 7472  diss_gdf.geometr
+0000ee50: 792e 6172 7261 792e 6461 7461 2c20 6772  y.array.data, gr
+0000ee60: 6964 5f73 697a 653d 6772 6964 7369 7a65  id_size=gridsize
+0000ee70: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000ee80: 2320 5361 7665 2074 6865 2072 6573 756c  # Save the resul
+0000ee90: 7420 746f 2064 6573 7469 6e61 7469 6f6e  t to destination
+0000eea0: 2066 696c 6528 7329 0a20 2020 2073 7461   file(s).    sta
+0000eeb0: 7274 5f74 6f5f 6669 6c65 203d 2064 6174  rt_to_file = dat
+0000eec0: 6574 696d 652e 6e6f 7728 290a 0a20 2020  etime.now()..   
+0000eed0: 2023 2049 6620 7468 6520 7469 6c65 7320   # If the tiles 
+0000eee0: 646f 6e27 7420 6e65 6564 2074 6f20 6265  don't need to be
+0000eef0: 206d 6572 6765 6420 6166 7465 7277 6172   merged afterwar
+0000ef00: 6473 2c20 7765 2063 616e 206a 7573 7420  ds, we can just 
+0000ef10: 7361 7665 2074 6865 2072 6573 756c 7420  save the result 
+0000ef20: 6173 0a20 2020 2023 2069 7420 6973 2e0a  as.    # it is..
+0000ef30: 2020 2020 6966 2073 7472 286f 7574 7075      if str(outpu
+0000ef40: 745f 6e6f 746f 6e62 6f72 6465 725f 7061  t_notonborder_pa
+0000ef50: 7468 2920 3d3d 2073 7472 286f 7574 7075  th) == str(outpu
+0000ef60: 745f 6f6e 626f 7264 6572 5f70 6174 6829  t_onborder_path)
+0000ef70: 3a0a 2020 2020 2020 2020 2320 6173 7365  :.        # asse
+0000ef80: 7274 2074 6f20 6576 6164 6520 7079 4c61  rt to evade pyLa
+0000ef90: 6e63 6520 7761 726e 696e 670a 2020 2020  nce warning.    
+0000efa0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+0000efb0: 7461 6e63 6528 6469 7373 5f67 6466 2c20  tance(diss_gdf, 
+0000efc0: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
+0000efd0: 290a 2020 2020 2020 2020 2320 5573 6520  ).        # Use 
+0000efe0: 666f 7263 655f 6d75 6c74 6974 7970 652c  force_multitype,
+0000eff0: 2074 6f20 6576 6164 6520 7761 726e 696e   to evade warnin
+0000f000: 6773 2077 6865 6e20 736f 6d65 2062 6174  gs when some bat
+0000f010: 6368 6573 2063 6f6e 7461 696e 0a20 2020  ches contain.   
+0000f020: 2020 2020 2023 2073 696e 676c 6574 7970       # singletyp
+0000f030: 6520 616e 6420 736f 6d65 2063 6f6e 7461  e and some conta
+0000f040: 696e 206d 756c 7469 7479 7065 2067 656f  in multitype geo
+0000f050: 6d65 7472 6965 730a 2020 2020 2020 2020  metries.        
+0000f060: 6766 6f2e 746f 5f66 696c 6528 0a20 2020  gfo.to_file(.   
+0000f070: 2020 2020 2020 2020 2064 6973 735f 6764           diss_gd
+0000f080: 662c 0a20 2020 2020 2020 2020 2020 206f  f,.            o
+0000f090: 7574 7075 745f 6e6f 746f 6e62 6f72 6465  utput_notonborde
+0000f0a0: 725f 7061 7468 2c0a 2020 2020 2020 2020  r_path,.        
+0000f0b0: 2020 2020 6c61 7965 723d 6f75 7470 7574      layer=output
+0000f0c0: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+0000f0d0: 2020 2020 666f 7263 655f 6d75 6c74 6974      force_multit
+0000f0e0: 7970 653d 5472 7565 2c0a 2020 2020 2020  ype=True,.      
+0000f0f0: 2020 2020 2020 696e 6465 783d 4661 6c73        index=Fals
+0000f100: 652c 0a20 2020 2020 2020 2020 2020 2063  e,.            c
+0000f110: 7265 6174 655f 7370 6174 6961 6c5f 696e  reate_spatial_in
+0000f120: 6465 783d 4661 6c73 652c 0a20 2020 2020  dex=False,.     
+0000f130: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
+0000f140: 2020 2020 2020 2023 2049 6620 6e6f 742c         # If not,
+0000f150: 2073 6176 6520 7468 6520 706f 6c79 676f   save the polygo
+0000f160: 6e73 206f 6e20 7468 6520 626f 7264 6572  ns on the border
+0000f170: 2073 6570 6572 6174 656c 790a 2020 2020   seperately.    
+0000f180: 2020 2020 6262 6f78 5f6c 696e 6573 5f67      bbox_lines_g
+0000f190: 6466 203d 2067 7064 2e47 656f 4461 7461  df = gpd.GeoData
+0000f1a0: 4672 616d 6528 0a20 2020 2020 2020 2020  Frame(.         
+0000f1b0: 2020 2067 656f 6d65 7472 793d 6765 6f73     geometry=geos
+0000f1c0: 6572 6965 735f 7574 696c 2e70 6f6c 7967  eries_util.polyg
+0000f1d0: 6f6e 735f 746f 5f6c 696e 6573 2820 2023  ons_to_lines(  #
+0000f1e0: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
+0000f1f0: 2020 2020 2020 2020 2020 2020 2020 6770                gp
+0000f200: 642e 4765 6f53 6572 6965 7328 5b73 685f  d.GeoSeries([sh_
+0000f210: 6765 6f6d 2e62 6f78 2862 626f 785b 305d  geom.box(bbox[0]
+0000f220: 2c20 6262 6f78 5b31 5d2c 2062 626f 785b  , bbox[1], bbox[
+0000f230: 325d 2c20 6262 6f78 5b33 5d29 5d29 0a20  2], bbox[3])]). 
+0000f240: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+0000f250: 2020 2020 2020 2020 2020 6372 733d 696e            crs=in
+0000f260: 7075 745f 6764 662e 6372 732c 2020 2320  put_gdf.crs,  # 
+0000f270: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+0000f280: 2020 2020 2029 0a20 2020 2020 2020 206f       ).        o
+0000f290: 6e62 6f72 6465 725f 6764 6620 3d20 6770  nborder_gdf = gp
+0000f2a0: 642e 736a 6f69 6e28 6469 7373 5f67 6466  d.sjoin(diss_gdf
+0000f2b0: 2c20 6262 6f78 5f6c 696e 6573 5f67 6466  , bbox_lines_gdf
+0000f2c0: 2c20 7072 6564 6963 6174 653d 2269 6e74  , predicate="int
+0000f2d0: 6572 7365 6374 7322 290a 2020 2020 2020  ersects").      
+0000f2e0: 2020 6f6e 626f 7264 6572 5f67 6466 2e64    onborder_gdf.d
+0000f2f0: 726f 7028 2269 6e64 6578 5f72 6967 6874  rop("index_right
+0000f300: 222c 2061 7869 733d 312c 2069 6e70 6c61  ", axis=1, inpla
+0000f310: 6365 3d54 7275 6529 0a20 2020 2020 2020  ce=True).       
+0000f320: 2069 6620 6c65 6e28 6f6e 626f 7264 6572   if len(onborder
+0000f330: 5f67 6466 2920 3e20 303a 0a20 2020 2020  _gdf) > 0:.     
+0000f340: 2020 2020 2020 2023 2061 7373 6572 7420         # assert 
+0000f350: 746f 2065 7661 6465 2070 794c 616e 6365  to evade pyLance
+0000f360: 2077 6172 6e69 6e67 0a20 2020 2020 2020   warning.       
+0000f370: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+0000f380: 7374 616e 6365 286f 6e62 6f72 6465 725f  stance(onborder_
+0000f390: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
+0000f3a0: 4672 616d 6529 0a20 2020 2020 2020 2020  Frame).         
+0000f3b0: 2020 2023 2055 7365 2066 6f72 6365 5f6d     # Use force_m
+0000f3c0: 756c 7469 7479 7065 2c20 746f 2065 7661  ultitype, to eva
+0000f3d0: 6465 2077 6172 6e69 6e67 7320 7768 656e  de warnings when
+0000f3e0: 2073 6f6d 6520 6261 7463 6865 7320 636f   some batches co
+0000f3f0: 6e74 6169 6e0a 2020 2020 2020 2020 2020  ntain.          
+0000f400: 2020 2320 7369 6e67 6c65 7479 7065 2061    # singletype a
+0000f410: 6e64 2073 6f6d 6520 636f 6e74 6169 6e20  nd some contain 
+0000f420: 6d75 6c74 6974 7970 6520 6765 6f6d 6574  multitype geomet
+0000f430: 7269 6573 0a20 2020 2020 2020 2020 2020  ries.           
+0000f440: 2067 666f 2e74 6f5f 6669 6c65 280a 2020   gfo.to_file(.  
+0000f450: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
+0000f460: 626f 7264 6572 5f67 6466 2c0a 2020 2020  border_gdf,.    
+0000f470: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+0000f480: 7574 5f6f 6e62 6f72 6465 725f 7061 7468  ut_onborder_path
+0000f490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f4a0: 2020 6c61 7965 723d 6f75 7470 7574 5f6c    layer=output_l
+0000f4b0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+0000f4c0: 2020 2020 2020 666f 7263 655f 6d75 6c74        force_mult
+0000f4d0: 6974 7970 653d 5472 7565 2c0a 2020 2020  itype=True,.    
+0000f4e0: 2020 2020 2020 2020 2020 2020 6372 6561              crea
+0000f4f0: 7465 5f73 7061 7469 616c 5f69 6e64 6578  te_spatial_index
+0000f500: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000f510: 2020 2020 290a 0a20 2020 2020 2020 206e      )..        n
+0000f520: 6f74 6f6e 626f 7264 6572 5f67 6466 203d  otonborder_gdf =
+0000f530: 2064 6973 735f 6764 665b 7e64 6973 735f   diss_gdf[~diss_
+0000f540: 6764 662e 696e 6465 782e 6973 696e 286f  gdf.index.isin(o
+0000f550: 6e62 6f72 6465 725f 6764 662e 696e 6465  nborder_gdf.inde
+0000f560: 7829 5d0a 2020 2020 2020 2020 6966 206c  x)].        if l
+0000f570: 656e 286e 6f74 6f6e 626f 7264 6572 5f67  en(notonborder_g
+0000f580: 6466 2920 3e20 303a 0a20 2020 2020 2020  df) > 0:.       
+0000f590: 2020 2020 2023 2061 7373 6572 7420 746f       # assert to
+0000f5a0: 2065 7661 6465 2070 794c 616e 6365 2077   evade pyLance w
+0000f5b0: 6172 6e69 6e67 0a20 2020 2020 2020 2020  arning.         
+0000f5c0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+0000f5d0: 616e 6365 286e 6f74 6f6e 626f 7264 6572  ance(notonborder
+0000f5e0: 5f67 6466 2c20 6770 642e 4765 6f44 6174  _gdf, gpd.GeoDat
+0000f5f0: 6146 7261 6d65 290a 2020 2020 2020 2020  aFrame).        
+0000f600: 2020 2020 2320 5573 6520 666f 7263 655f      # Use force_
+0000f610: 6d75 6c74 6974 7970 652c 2074 6f20 6576  multitype, to ev
+0000f620: 6164 6520 7761 726e 696e 6773 2077 6865  ade warnings whe
+0000f630: 6e20 736f 6d65 2062 6174 6368 6573 2063  n some batches c
+0000f640: 6f6e 7461 696e 0a20 2020 2020 2020 2020  ontain.         
+0000f650: 2020 2023 2073 696e 676c 6574 7970 6520     # singletype 
+0000f660: 616e 6420 736f 6d65 2063 6f6e 7461 696e  and some contain
+0000f670: 206d 756c 7469 7479 7065 2067 656f 6d65   multitype geome
+0000f680: 7472 6965 730a 2020 2020 2020 2020 2020  tries.          
+0000f690: 2020 6766 6f2e 746f 5f66 696c 6528 0a20    gfo.to_file(. 
+0000f6a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000f6b0: 6f74 6f6e 626f 7264 6572 5f67 6466 2c0a  otonborder_gdf,.
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6d0: 6f75 7470 7574 5f6e 6f74 6f6e 626f 7264  output_notonbord
+0000f6e0: 6572 5f70 6174 682c 0a20 2020 2020 2020  er_path,.       
+0000f6f0: 2020 2020 2020 2020 206c 6179 6572 3d6f           layer=o
+0000f700: 7574 7075 745f 6c61 7965 722c 0a20 2020  utput_layer,.   
+0000f710: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f720: 6365 5f6d 756c 7469 7479 7065 3d54 7275  ce_multitype=Tru
+0000f730: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000f740: 2020 2069 6e64 6578 3d46 616c 7365 2c0a     index=False,.
+0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f760: 6372 6561 7465 5f73 7061 7469 616c 5f69  create_spatial_i
+0000f770: 6e64 6578 3d46 616c 7365 2c0a 2020 2020  ndex=False,.    
+0000f780: 2020 2020 2020 2020 290a 2020 2020 7065          ).    pe
+0000f790: 7266 696e 666f 5b22 7469 6d65 5f74 6f5f  rfinfo["time_to_
+0000f7a0: 6669 6c65 225d 203d 2028 6461 7465 7469  file"] = (dateti
+0000f7b0: 6d65 2e6e 6f77 2829 202d 2073 7461 7274  me.now() - start
+0000f7c0: 5f74 6f5f 6669 6c65 292e 746f 7461 6c5f  _to_file).total_
+0000f7d0: 7365 636f 6e64 7328 290a 0a20 2020 2023  seconds()..    #
+0000f7e0: 2046 696e 616c 6973 652e 2e2e 0a20 2020   Finalise....   
+0000f7f0: 206d 6573 7361 6765 203d 2066 2264 6973   message = f"dis
+0000f800: 736f 6c76 6520 7265 6164 7920 696e 207b  solve ready in {
+0000f810: 6461 7465 7469 6d65 2e6e 6f77 2829 2d73  datetime.now()-s
+0000f820: 7461 7274 5f74 696d 657d 206f 6e20 7b69  tart_time} on {i
+0000f830: 6e70 7574 5f70 6174 687d 2122 0a20 2020  nput_path}!".   
+0000f840: 206c 6f67 6765 722e 6465 6275 6728 6d65   logger.debug(me
+0000f850: 7373 6167 6529 0a0a 2020 2020 2320 436f  ssage)..    # Co
+0000f860: 6c6c 6563 7420 7065 7266 696e 666f 0a20  llect perfinfo. 
+0000f870: 2020 2074 6f74 616c 5f70 6572 665f 7469     total_perf_ti
+0000f880: 6d65 203d 2030 0a20 2020 2070 6572 6673  me = 0.    perfs
+0000f890: 7472 696e 6720 3d20 2222 0a20 2020 2066  tring = "".    f
+0000f8a0: 6f72 2070 6572 6663 6f64 6520 696e 2070  or perfcode in p
+0000f8b0: 6572 6669 6e66 6f3a 0a20 2020 2020 2020  erfinfo:.       
+0000f8c0: 2074 6f74 616c 5f70 6572 665f 7469 6d65   total_perf_time
+0000f8d0: 202b 3d20 7065 7266 696e 666f 5b70 6572   += perfinfo[per
+0000f8e0: 6663 6f64 655d 0a20 2020 2020 2020 2070  fcode].        p
+0000f8f0: 6572 6673 7472 696e 6720 2b3d 2066 227b  erfstring += f"{
+0000f900: 7065 7266 636f 6465 7d3a 207b 7065 7266  perfcode}: {perf
+0000f910: 696e 666f 5b70 6572 6663 6f64 655d 3a2e  info[perfcode]:.
+0000f920: 3266 7d2c 2022 0a20 2020 2072 6574 7572  2f}, ".    retur
+0000f930: 6e5f 696e 666f 5b22 746f 7461 6c5f 7469  n_info["total_ti
+0000f940: 6d65 225d 203d 2028 6461 7465 7469 6d65  me"] = (datetime
+0000f950: 2e6e 6f77 2829 202d 2073 7461 7274 5f74  .now() - start_t
+0000f960: 696d 6529 2e74 6f74 616c 5f73 6563 6f6e  ime).total_secon
+0000f970: 6473 2829 0a20 2020 2070 6572 6669 6e66  ds().    perfinf
+0000f980: 6f5b 2275 6e61 6363 6f75 6e74 6564 225d  o["unaccounted"]
+0000f990: 203d 2072 6574 7572 6e5f 696e 666f 5b22   = return_info["
+0000f9a0: 746f 7461 6c5f 7469 6d65 225d 202d 2074  total_time"] - t
+0000f9b0: 6f74 616c 5f70 6572 665f 7469 6d65 0a20  otal_perf_time. 
+0000f9c0: 2020 2070 6572 6673 7472 696e 6720 2b3d     perfstring +=
+0000f9d0: 2066 2275 6e61 6363 6f75 6e74 6564 3a20   f"unaccounted: 
+0000f9e0: 7b70 6572 6669 6e66 6f5b 2775 6e61 6363  {perfinfo['unacc
+0000f9f0: 6f75 6e74 6564 275d 3a2e 3266 7d22 0a0a  ounted']:.2f}"..
+0000fa00: 2020 2020 2320 5265 7475 726e 0a20 2020      # Return.   
+0000fa10: 2072 6574 7572 6e5f 696e 666f 5b22 7065   return_info["pe
+0000fa20: 7266 696e 666f 225d 203d 2070 6572 6669  rfinfo"] = perfi
+0000fa30: 6e66 6f0a 2020 2020 7265 7475 726e 5f69  nfo.    return_i
+0000fa40: 6e66 6f5b 2270 6572 6673 7472 696e 6722  nfo["perfstring"
+0000fa50: 5d20 3d20 7065 7266 7374 7269 6e67 0a20  ] = perfstring. 
+0000fa60: 2020 2072 6574 7572 6e5f 696e 666f 5b22     return_info["
+0000fa70: 6d65 7373 6167 6522 5d20 3d20 6d65 7373  message"] = mess
+0000fa80: 6167 650a 2020 2020 7265 7475 726e 2072  age.    return r
+0000fa90: 6574 7572 6e5f 696e 666f 0a0a 0a64 6566  eturn_info...def
+0000faa0: 205f 6469 7373 6f6c 7665 280a 2020 2020   _dissolve(.    
+0000fab0: 6466 3a20 6770 642e 4765 6f44 6174 6146  df: gpd.GeoDataF
+0000fac0: 7261 6d65 2c0a 2020 2020 6279 3d4e 6f6e  rame,.    by=Non
+0000fad0: 652c 0a20 2020 2061 6767 6675 6e63 3a20  e,.    aggfunc: 
+0000fae0: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
+0000faf0: 7472 2c20 6469 6374 5d5d 203d 2022 6669  tr, dict]] = "fi
+0000fb00: 7273 7422 2c0a 2020 2020 6173 5f69 6e64  rst",.    as_ind
+0000fb10: 6578 3d54 7275 652c 0a20 2020 206c 6576  ex=True,.    lev
+0000fb20: 656c 3d4e 6f6e 652c 0a20 2020 2073 6f72  el=None,.    sor
+0000fb30: 743d 5472 7565 2c0a 2020 2020 6f62 7365  t=True,.    obse
+0000fb40: 7276 6564 3d46 616c 7365 2c0a 2020 2020  rved=False,.    
+0000fb50: 6472 6f70 6e61 3d54 7275 652c 0a29 202d  dropna=True,.) -
+0000fb60: 3e20 6770 642e 4765 6f44 6174 6146 7261  > gpd.GeoDataFra
+0000fb70: 6d65 3a0a 2020 2020 2222 220a 2020 2020  me:.    """.    
+0000fb80: 4469 7373 6f6c 7665 2067 656f 6d65 7472  Dissolve geometr
+0000fb90: 6965 7320 7769 7468 696e 2060 6772 6f75  ies within `grou
+0000fba0: 7062 7960 2069 6e74 6f20 7369 6e67 6c65  pby` into single
+0000fbb0: 206f 6273 6572 7661 7469 6f6e 2e0a 2020   observation..  
+0000fbc0: 2020 5468 6973 2069 7320 6163 636f 6d70    This is accomp
+0000fbd0: 6c69 7368 6564 2062 7920 6170 706c 7969  lished by applyi
+0000fbe0: 6e67 2074 6865 2060 756e 6172 795f 756e  ng the `unary_un
+0000fbf0: 696f 6e60 206d 6574 686f 640a 2020 2020  ion` method.    
+0000fc00: 746f 2061 6c6c 2067 656f 6d65 7472 6965  to all geometrie
+0000fc10: 7320 7769 7468 696e 2061 2067 726f 7570  s within a group
+0000fc20: 7365 6c66 2e0a 2020 2020 4f62 7365 7276  self..    Observ
+0000fc30: 6174 696f 6e73 2061 7373 6f63 6961 7465  ations associate
+0000fc40: 6420 7769 7468 2065 6163 6820 6067 726f  d with each `gro
+0000fc50: 7570 6279 6020 6772 6f75 7020 7769 6c6c  upby` group will
+0000fc60: 2062 6520 6167 6772 6567 6174 6564 0a20   be aggregated. 
+0000fc70: 2020 2075 7369 6e67 2074 6865 2060 6167     using the `ag
+0000fc80: 6766 756e 6360 2e0a 2020 2020 5061 7261  gfunc`..    Para
+0000fc90: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0000fca0: 2d2d 2d2d 2d0a 2020 2020 6279 203a 2073  -----.    by : s
+0000fcb0: 7472 696e 672c 2064 6566 6175 6c74 204e  tring, default N
+0000fcc0: 6f6e 650a 2020 2020 2020 2020 436f 6c75  one.        Colu
+0000fcd0: 6d6e 2077 686f 7365 2076 616c 7565 7320  mn whose values 
+0000fce0: 6465 6669 6e65 2067 726f 7570 7320 746f  define groups to
+0000fcf0: 2062 6520 6469 7373 6f6c 7665 642e 2049   be dissolved. I
+0000fd00: 6620 4e6f 6e65 2c0a 2020 2020 2020 2020  f None,.        
+0000fd10: 7768 6f6c 6520 4765 6f44 6174 6146 7261  whole GeoDataFra
+0000fd20: 6d65 2069 7320 636f 6e73 6964 6572 6564  me is considered
+0000fd30: 2061 2073 696e 676c 6520 6772 6f75 702e   a single group.
+0000fd40: 0a20 2020 2061 6767 6675 6e63 203a 2066  .    aggfunc : f
+0000fd50: 756e 6374 696f 6e2c 2073 7472 696e 6720  unction, string 
+0000fd60: 6f72 2064 6963 742c 2064 6566 6175 6c74  or dict, default
+0000fd70: 2022 6669 7273 7422 0a20 2020 2020 2020   "first".       
+0000fd80: 2041 6767 7265 6761 7469 6f6e 2066 756e   Aggregation fun
+0000fd90: 6374 696f 6e20 666f 7220 6d61 6e69 7075  ction for manipu
+0000fda0: 6c61 7469 6f6e 206f 6620 6461 7461 2061  lation of data a
+0000fdb0: 7373 6f63 6961 7465 640a 2020 2020 2020  ssociated.      
+0000fdc0: 2020 7769 7468 2065 6163 6820 6772 6f75    with each grou
+0000fdd0: 702e 2050 6173 7365 6420 746f 2070 616e  p. Passed to pan
+0000fde0: 6461 7320 6067 726f 7570 6279 2e61 6767  das `groupby.agg
+0000fdf0: 6020 6d65 7468 6f64 2e0a 2020 2020 6173  ` method..    as
+0000fe00: 5f69 6e64 6578 203a 2062 6f6f 6c65 616e  _index : boolean
+0000fe10: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+0000fe20: 2020 2020 2020 2049 6620 7472 7565 2c20         If true, 
+0000fe30: 6772 6f75 7062 7920 636f 6c75 6d6e 7320  groupby columns 
+0000fe40: 6265 636f 6d65 2069 6e64 6578 206f 6620  become index of 
+0000fe50: 7265 7375 6c74 2e0a 2020 2020 6c65 7665  result..    leve
+0000fe60: 6c20 3a20 696e 7420 6f72 2073 7472 206f  l : int or str o
+0000fe70: 7220 7365 7175 656e 6365 206f 6620 696e  r sequence of in
+0000fe80: 7420 6f72 2073 6571 7565 6e63 6520 6f66  t or sequence of
+0000fe90: 2073 7472 2c20 6465 6661 756c 7420 4e6f   str, default No
+0000fea0: 6e65 0a20 2020 2020 2020 2049 6620 7468  ne.        If th
+0000feb0: 6520 6178 6973 2069 7320 6120 4d75 6c74  e axis is a Mult
+0000fec0: 6949 6e64 6578 2028 6869 6572 6172 6368  iIndex (hierarch
+0000fed0: 6963 616c 292c 2067 726f 7570 2062 7920  ical), group by 
+0000fee0: 610a 2020 2020 2020 2020 7061 7274 6963  a.        partic
+0000fef0: 756c 6172 206c 6576 656c 206f 7220 6c65  ular level or le
+0000ff00: 7665 6c73 2e0a 2020 2020 2020 2020 2e2e  vels..        ..
+0000ff10: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
+0000ff20: 302e 392e 300a 2020 2020 736f 7274 203a  0.9.0.    sort :
+0000ff30: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
+0000ff40: 7275 650a 2020 2020 2020 2020 536f 7274  rue.        Sort
+0000ff50: 2067 726f 7570 206b 6579 732e 2047 6574   group keys. Get
+0000ff60: 2062 6574 7465 7220 7065 7266 6f72 6d61   better performa
+0000ff70: 6e63 6520 6279 2074 7572 6e69 6e67 2074  nce by turning t
+0000ff80: 6869 7320 6f66 662e 0a20 2020 2020 2020  his off..       
+0000ff90: 204e 6f74 6520 7468 6973 2064 6f65 7320   Note this does 
+0000ffa0: 6e6f 7420 696e 666c 7565 6e63 6520 7468  not influence th
+0000ffb0: 6520 6f72 6465 7220 6f66 206f 6273 6572  e order of obser
+0000ffc0: 7661 7469 6f6e 7320 7769 7468 696e 0a20  vations within. 
+0000ffd0: 2020 2020 2020 2065 6163 6820 6772 6f75         each grou
+0000ffe0: 702e 2047 726f 7570 6279 2070 7265 7365  p. Groupby prese
+0000fff0: 7276 6573 2074 6865 206f 7264 6572 206f  rves the order o
+00010000: 6620 726f 7773 2077 6974 6869 6e20 6561  f rows within ea
+00010010: 6368 2067 726f 7570 2e0a 2020 2020 2020  ch group..      
+00010020: 2020 2e2e 2076 6572 7369 6f6e 6164 6465    .. versionadde
+00010030: 643a 3a20 302e 392e 300a 2020 2020 6f62  d:: 0.9.0.    ob
+00010040: 7365 7276 6564 203a 2062 6f6f 6c2c 2064  served : bool, d
+00010050: 6566 6175 6c74 2046 616c 7365 0a20 2020  efault False.   
+00010060: 2020 2020 2054 6869 7320 6f6e 6c79 2061       This only a
+00010070: 7070 6c69 6573 2069 6620 616e 7920 6f66  pplies if any of
+00010080: 2074 6865 2067 726f 7570 6572 7320 6172   the groupers ar
+00010090: 6520 4361 7465 676f 7269 6361 6c73 2e0a  e Categoricals..
+000100a0: 2020 2020 2020 2020 4966 2054 7275 653a          If True:
+000100b0: 206f 6e6c 7920 7368 6f77 206f 6273 6572   only show obser
+000100c0: 7665 6420 7661 6c75 6573 2066 6f72 2063  ved values for c
+000100d0: 6174 6567 6f72 6963 616c 2067 726f 7570  ategorical group
+000100e0: 6572 732e 0a20 2020 2020 2020 2049 6620  ers..        If 
+000100f0: 4661 6c73 653a 2073 686f 7720 616c 6c20  False: show all 
+00010100: 7661 6c75 6573 2066 6f72 2063 6174 6567  values for categ
+00010110: 6f72 6963 616c 2067 726f 7570 6572 732e  orical groupers.
+00010120: 0a20 2020 2020 2020 202e 2e20 7665 7273  .        .. vers
+00010130: 696f 6e61 6464 6564 3a3a 2030 2e39 2e30  ionadded:: 0.9.0
+00010140: 0a20 2020 2064 726f 706e 6120 3a20 626f  .    dropna : bo
+00010150: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00010160: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00010170: 2c20 616e 6420 6966 2067 726f 7570 206b  , and if group k
+00010180: 6579 7320 636f 6e74 6169 6e20 4e41 2076  eys contain NA v
+00010190: 616c 7565 732c 204e 4120 7661 6c75 6573  alues, NA values
+000101a0: 0a20 2020 2020 2020 2074 6f67 6574 6865  .        togethe
+000101b0: 7220 7769 7468 2072 6f77 2f63 6f6c 756d  r with row/colum
+000101c0: 6e20 7769 6c6c 2062 6520 6472 6f70 7065  n will be droppe
+000101d0: 642e 2049 6620 4661 6c73 652c 204e 410a  d. If False, NA.
+000101e0: 2020 2020 2020 2020 7661 6c75 6573 2077          values w
+000101f0: 696c 6c20 616c 736f 2062 6520 7472 6561  ill also be trea
+00010200: 7465 6420 6173 2074 6865 206b 6579 2069  ted as the key i
+00010210: 6e20 6772 6f75 7073 2e0a 2020 2020 2020  n groups..      
+00010220: 2020 5468 6973 2070 6172 616d 6574 6572    This parameter
 00010230: 2069 7320 6e6f 7420 7375 7070 6f72 7465   is not supporte
 00010240: 6420 666f 7220 7061 6e64 6173 203c 2031  d for pandas < 1
-00010250: 2e31 2e30 2229 0a20 2020 2022 2222 0a0a  .1.0").    """..
-00010260: 2020 2020 2320 5072 6f63 6573 7320 6e6f      # Process no
-00010270: 6e2d 7370 6174 6961 6c20 636f 6d70 6f6e  n-spatial compon
-00010280: 656e 740a 2020 2020 6461 7461 203d 2070  ent.    data = p
-00010290: 642e 4461 7461 4672 616d 6528 6466 2e64  d.DataFrame(df.d
-000102a0: 726f 7028 636f 6c75 6d6e 733d 6466 2e67  rop(columns=df.g
-000102b0: 656f 6d65 7472 792e 6e61 6d65 2929 0a0a  eometry.name))..
-000102c0: 2020 2020 6966 2061 6767 6675 6e63 2069      if aggfunc i
-000102d0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2069  s not None and i
-000102e0: 7369 6e73 7461 6e63 6528 6167 6766 756e  sinstance(aggfun
-000102f0: 632c 2064 6963 7429 2061 6e64 2022 746f  c, dict) and "to
-00010300: 5f6a 736f 6e22 2069 6e20 6167 6766 756e  _json" in aggfun
-00010310: 633a 0a20 2020 2020 2020 2061 6767 5f63  c:.        agg_c
-00010320: 6f6c 756d 6e73 203d 206c 6973 7428 7365  olumns = list(se
-00010330: 7428 6167 6766 756e 635b 2274 6f5f 6a73  t(aggfunc["to_js
-00010340: 6f6e 225d 2929 0a20 2020 2020 2020 2061  on"])).        a
-00010350: 6767 7265 6761 7465 645f 6461 7461 203d  ggregated_data =
-00010360: 2028 0a20 2020 2020 2020 2020 2020 2064   (.            d
-00010370: 6174 612e 6772 6f75 7062 7928 2a2a 6772  ata.groupby(**gr
-00010380: 6f75 7062 795f 6b77 6172 6773 290a 2020  oupby_kwargs).  
-00010390: 2020 2020 2020 2020 2020 2e61 7070 6c79            .apply
-000103a0: 286c 616d 6264 6120 673a 2067 5b61 6767  (lambda g: g[agg
-000103b0: 5f63 6f6c 756d 6e73 5d2e 746f 5f6a 736f  _columns].to_jso
-000103c0: 6e28 6f72 6965 6e74 3d22 7265 636f 7264  n(orient="record
-000103d0: 7322 2929 0a20 2020 2020 2020 2020 2020  s")).           
-000103e0: 202e 746f 5f66 7261 6d65 286e 616d 653d   .to_frame(name=
-000103f0: 225f 5f44 4953 534f 4c56 455f 544f 4a53  "__DISSOLVE_TOJS
-00010400: 4f4e 2229 0a20 2020 2020 2020 2029 0a20  ON").        ). 
-00010410: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00010420: 6365 2861 6767 6675 6e63 2c20 7374 7229  ce(aggfunc, str)
-00010430: 2061 6e64 2061 6767 6675 6e63 203d 3d20   and aggfunc == 
-00010440: 226d 6572 6765 5f6a 736f 6e5f 6c69 7374  "merge_json_list
-00010450: 7322 3a0a 2020 2020 2020 2020 2320 4d65  s":.        # Me
-00010460: 7267 6520 616e 6420 666c 6174 7465 6e20  rge and flatten 
-00010470: 7468 6520 6a73 6f6e 206c 6973 7473 2069  the json lists i
-00010480: 6e20 7468 6520 6772 6f75 7073 0a20 2020  n the groups.   
-00010490: 2020 2020 2064 6566 2067 726f 7570 5f66       def group_f
-000104a0: 6c61 7474 656e 5f6a 736f 6e5f 6c69 7374  latten_json_list
-000104b0: 2867 293a 0a20 2020 2020 2020 2020 2020  (g):.           
-000104c0: 2023 2045 7661 6c75 6174 6520 616c 6c20   # Evaluate all 
-000104d0: 6772 6f75 7065 6420 726f 7773 2074 6f20  grouped rows to 
-000104e0: 6a73 6f6e 206f 626a 6563 7473 2e20 5468  json objects. Th
-000104f0: 6973 2072 6573 756c 7473 2069 6e20 6120  is results in a 
-00010500: 6c69 7374 206f 660a 2020 2020 2020 2020  list of.        
-00010510: 2020 2020 2320 6c69 7374 7320 6f66 206a      # lists of j
-00010520: 736f 6e20 6f62 6a65 6374 732e 0a20 2020  son objects..   
-00010530: 2020 2020 2020 2020 206a 736f 6e5f 6e65           json_ne
-00010540: 7374 6564 5f6c 6973 7473 203d 205b 0a20  sted_lists = [. 
-00010550: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-00010560: 736f 6e2e 6c6f 6164 7328 6a73 6f6e 5f76  son.loads(json_v
-00010570: 616c 7565 7329 2066 6f72 206a 736f 6e5f  alues) for json_
-00010580: 7661 6c75 6573 2069 6e20 675b 225f 5f44  values in g["__D
-00010590: 4953 534f 4c56 455f 544f 4a53 4f4e 225d  ISSOLVE_TOJSON"]
-000105a0: 0a20 2020 2020 2020 2020 2020 205d 0a0a  .            ]..
-000105b0: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
-000105c0: 7472 6163 7420 7468 6520 726f 7773 2066  tract the rows f
-000105d0: 726f 6d20 7468 6520 6e65 7374 6564 206c  rom the nested l
-000105e0: 6973 7473 202b 2070 7574 2069 6e20 6120  ists + put in a 
-000105f0: 666c 6174 206c 6973 7420 6173 2073 7472  flat list as str
-00010600: 696e 6773 0a20 2020 2020 2020 2020 2020  ings.           
-00010610: 206a 736f 6e73 7472 5f66 6c61 7420 3d20   jsonstr_flat = 
-00010620: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00010630: 2020 6a73 6f6e 2e64 756d 7073 286a 736f    json.dumps(jso
-00010640: 6e5f 7661 6c75 6529 0a20 2020 2020 2020  n_value).       
-00010650: 2020 2020 2020 2020 2066 6f72 206a 736f           for jso
-00010660: 6e5f 7661 6c75 6573 2069 6e20 6a73 6f6e  n_values in json
-00010670: 5f6e 6573 7465 645f 6c69 7374 730a 2020  _nested_lists.  
-00010680: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00010690: 7220 6a73 6f6e 5f76 616c 7565 2069 6e20  r json_value in 
-000106a0: 6a73 6f6e 5f76 616c 7565 730a 2020 2020  json_values.    
-000106b0: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
-000106c0: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
-000106d0: 6475 706c 6963 6174 6573 0a20 2020 2020  duplicates.     
-000106e0: 2020 2020 2020 206a 736f 6e73 7374 725f         jsonsstr_
-000106f0: 6469 7374 696e 6374 203d 2073 6574 286a  distinct = set(j
-00010700: 736f 6e73 7472 5f66 6c61 7429 0a0a 2020  sonstr_flat)..  
-00010710: 2020 2020 2020 2020 2020 2320 436f 6e76            # Conv
-00010720: 6572 7420 7468 6520 6461 7461 2061 6761  ert the data aga
-00010730: 696e 2074 6f20 6120 6c69 7374 206f 6620  in to a list of 
-00010740: 6a73 6f6e 206f 626a 6563 7473 0a20 2020  json objects.   
-00010750: 2020 2020 2020 2020 206a 736f 6e5f 6469           json_di
-00010760: 7374 696e 6374 203d 205b 6a73 6f6e 2e6c  stinct = [json.l
-00010770: 6f61 6473 286a 736f 6e5f 7661 6c75 6529  oads(json_value)
-00010780: 2066 6f72 206a 736f 6e5f 7661 6c75 6520   for json_value 
-00010790: 696e 206a 736f 6e73 7374 725f 6469 7374  in jsonsstr_dist
-000107a0: 696e 6374 5d0a 0a20 2020 2020 2020 2020  inct]..         
-000107b0: 2020 2023 2052 6574 7572 6e20 6173 206a     # Return as j
-000107c0: 736f 6e20 7374 7269 6e67 0a20 2020 2020  son string.     
-000107d0: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
-000107e0: 6f6e 2e64 756d 7073 286a 736f 6e5f 6469  on.dumps(json_di
-000107f0: 7374 696e 6374 290a 0a20 2020 2020 2020  stinct)..       
-00010800: 2061 6767 7265 6761 7465 645f 6461 7461   aggregated_data
-00010810: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00010820: 2064 6174 612e 6772 6f75 7062 7928 2a2a   data.groupby(**
-00010830: 6772 6f75 7062 795f 6b77 6172 6773 290a  groupby_kwargs).
-00010840: 2020 2020 2020 2020 2020 2020 2e61 7070              .app
-00010850: 6c79 286c 616d 6264 6120 673a 2067 726f  ly(lambda g: gro
-00010860: 7570 5f66 6c61 7474 656e 5f6a 736f 6e5f  up_flatten_json_
-00010870: 6c69 7374 2867 2929 0a20 2020 2020 2020  list(g)).       
-00010880: 2020 2020 202e 746f 5f66 7261 6d65 286e       .to_frame(n
-00010890: 616d 653d 225f 5f44 4953 534f 4c56 455f  ame="__DISSOLVE_
-000108a0: 544f 4a53 4f4e 2229 0a20 2020 2020 2020  TOJSON").       
-000108b0: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
-000108c0: 2020 2020 2061 6767 7265 6761 7465 645f       aggregated_
-000108d0: 6461 7461 203d 2064 6174 612e 6772 6f75  data = data.grou
-000108e0: 7062 7928 2a2a 6772 6f75 7062 795f 6b77  pby(**groupby_kw
-000108f0: 6172 6773 292e 6167 6728 6167 6766 756e  args).agg(aggfun
-00010900: 6329 2020 2320 7479 7065 3a20 6967 6e6f  c)  # type: igno
-00010910: 7265 0a20 2020 2020 2020 2023 2043 6865  re.        # Che
-00010920: 636b 2069 6620 616c 6c20 636f 6c75 6d6e  ck if all column
-00010930: 7320 7765 7265 2070 726f 7065 726c 7920  s were properly 
-00010940: 6167 6772 6567 6174 6564 0a20 2020 2020  aggregated.     
-00010950: 2020 2061 7373 6572 7420 6279 5f6c 6f63     assert by_loc
-00010960: 616c 2069 7320 6e6f 7420 4e6f 6e65 0a20  al is not None. 
-00010970: 2020 2020 2020 2063 6f6c 756d 6e73 5f74         columns_t
-00010980: 6f5f 6167 6720 3d20 5b63 6f6c 756d 6e20  o_agg = [column 
-00010990: 666f 7220 636f 6c75 6d6e 2069 6e20 6461  for column in da
-000109a0: 7461 2e63 6f6c 756d 6e73 2069 6620 636f  ta.columns if co
-000109b0: 6c75 6d6e 206e 6f74 2069 6e20 6279 5f6c  lumn not in by_l
-000109c0: 6f63 616c 5d0a 2020 2020 2020 2020 6966  ocal].        if
-000109d0: 206c 656e 2863 6f6c 756d 6e73 5f74 6f5f   len(columns_to_
-000109e0: 6167 6729 2021 3d20 6c65 6e28 6167 6772  agg) != len(aggr
-000109f0: 6567 6174 6564 5f64 6174 612e 636f 6c75  egated_data.colu
-00010a00: 6d6e 7329 3a0a 2020 2020 2020 2020 2020  mns):.          
-00010a10: 2020 6472 6f70 7065 645f 636f 6c75 6d6e    dropped_column
-00010a20: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-00010a30: 2020 2020 2020 636f 6c75 6d6e 0a20 2020        column.   
-00010a40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00010a50: 2063 6f6c 756d 6e20 696e 2063 6f6c 756d   column in colum
-00010a60: 6e73 5f74 6f5f 6167 670a 2020 2020 2020  ns_to_agg.      
-00010a70: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
-00010a80: 756d 6e20 6e6f 7420 696e 2061 6767 7265  umn not in aggre
-00010a90: 6761 7465 645f 6461 7461 2e63 6f6c 756d  gated_data.colum
-00010aa0: 6e73 0a20 2020 2020 2020 2020 2020 205d  ns.            ]
-00010ab0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00010ac0: 7365 2045 7863 6570 7469 6f6e 280a 2020  se Exception(.  
-00010ad0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00010ae0: 436f 6c75 6d6e 2873 2920 7b64 726f 7070  Column(s) {dropp
-00010af0: 6564 5f63 6f6c 756d 6e73 7d20 6172 6520  ed_columns} are 
-00010b00: 6e6f 7420 7375 7070 6f72 7465 6420 666f  not supported fo
-00010b10: 7220 6167 6772 6567 6174 696f 6e2c 2073  r aggregation, s
-00010b20: 746f 7022 0a20 2020 2020 2020 2020 2020  top".           
-00010b30: 2029 0a0a 2020 2020 2320 5072 6f63 6573   )..    # Proces
-00010b40: 7320 7370 6174 6961 6c20 636f 6d70 6f6e  s spatial compon
-00010b50: 656e 740a 2020 2020 6465 6620 6d65 7267  ent.    def merg
-00010b60: 655f 6765 6f6d 6574 7269 6573 2862 6c6f  e_geometries(blo
-00010b70: 636b 293a 0a20 2020 2020 2020 206d 6572  ck):.        mer
-00010b80: 6765 645f 6765 6f6d 203d 2062 6c6f 636b  ged_geom = block
-00010b90: 2e75 6e61 7279 5f75 6e69 6f6e 0a20 2020  .unary_union.   
-00010ba0: 2020 2020 2072 6574 7572 6e20 6d65 7267       return merg
-00010bb0: 6564 5f67 656f 6d0a 0a20 2020 2067 203d  ed_geom..    g =
-00010bc0: 2064 662e 6772 6f75 7062 7928 6772 6f75   df.groupby(grou
-00010bd0: 705f 6b65 7973 3d46 616c 7365 2c20 2a2a  p_keys=False, **
-00010be0: 6772 6f75 7062 795f 6b77 6172 6773 295b  groupby_kwargs)[
-00010bf0: 6466 2e67 656f 6d65 7472 792e 6e61 6d65  df.geometry.name
-00010c00: 5d2e 6167 6728 0a20 2020 2020 2020 206d  ].agg(.        m
-00010c10: 6572 6765 5f67 656f 6d65 7472 6965 730a  erge_geometries.
-00010c20: 2020 2020 290a 0a20 2020 2023 2041 6767      )..    # Agg
-00010c30: 7265 6761 7465 0a20 2020 2061 6767 7265  regate.    aggre
-00010c40: 6761 7465 645f 6765 6f6d 6574 7279 203d  gated_geometry =
-00010c50: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-00010c60: 6528 0a20 2020 2020 2020 2064 6174 613d  e(.        data=
-00010c70: 672c 2067 656f 6d65 7472 793d 6466 2e67  g, geometry=df.g
-00010c80: 656f 6d65 7472 792e 6e61 6d65 2c20 6372  eometry.name, cr
-00010c90: 733d 6466 2e63 7273 2020 2320 7479 7065  s=df.crs  # type
-00010ca0: 3a20 6967 6e6f 7265 0a20 2020 2029 0a20  : ignore.    ). 
-00010cb0: 2020 2023 2052 6563 6f6d 6269 6e65 0a20     # Recombine. 
-00010cc0: 2020 2061 6767 7265 6761 7465 6420 3d20     aggregated = 
-00010cd0: 6167 6772 6567 6174 6564 5f67 656f 6d65  aggregated_geome
-00010ce0: 7472 792e 6a6f 696e 2861 6767 7265 6761  try.join(aggrega
-00010cf0: 7465 645f 6461 7461 290a 0a20 2020 2023  ted_data)..    #
-00010d00: 2052 6573 6574 2069 6620 7265 7175 6573   Reset if reques
-00010d10: 7465 640a 2020 2020 6966 206e 6f74 2061  ted.    if not a
-00010d20: 735f 696e 6465 783a 0a20 2020 2020 2020  s_index:.       
-00010d30: 2061 6767 7265 6761 7465 6420 3d20 6167   aggregated = ag
-00010d40: 6772 6567 6174 6564 2e72 6573 6574 5f69  gregated.reset_i
-00010d50: 6e64 6578 2829 0a0a 2020 2020 2320 4d61  ndex()..    # Ma
-00010d60: 6b65 2073 7572 6520 6f75 7470 7574 2074  ke sure output t
-00010d70: 7970 6573 206f 6620 6772 6f75 7065 6420  ypes of grouped 
-00010d80: 636f 6c75 6d6e 7320 6172 6520 7468 6520  columns are the 
-00010d90: 7361 6d65 2061 7320 696e 7075 7420 7479  same as input ty
-00010da0: 7065 732e 0a20 2020 2023 2045 2e67 2e20  pes..    # E.g. 
-00010db0: 6f62 6a65 6374 2063 6f6c 756d 6e73 2062  object columns b
-00010dc0: 6563 6f6d 6520 666c 6f61 7420 6966 2061  ecome float if a
-00010dd0: 6c6c 2076 616c 7565 7320 6172 6520 4e6f  ll values are No
-00010de0: 6e65 2e0a 2020 2020 6966 2062 7920 6973  ne..    if by is
-00010df0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00010e00: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00010e10: 2862 792c 2073 7472 293a 0a20 2020 2020  (by, str):.     
-00010e20: 2020 2020 2020 2069 6620 6279 2069 6e20         if by in 
-00010e30: 6167 6772 6567 6174 6564 2e63 6f6c 756d  aggregated.colum
-00010e40: 6e73 2061 6e64 2064 665b 6279 5d2e 6474  ns and df[by].dt
-00010e50: 7970 6520 213d 2061 6767 7265 6761 7465  ype != aggregate
-00010e60: 645b 6279 5d2e 6474 7970 653a 0a20 2020  d[by].dtype:.   
-00010e70: 2020 2020 2020 2020 2020 2020 2061 6767               agg
-00010e80: 7265 6761 7465 645b 6279 5d20 3d20 6167  regated[by] = ag
-00010e90: 6772 6567 6174 6564 5b62 795d 2e61 7374  gregated[by].ast
-00010ea0: 7970 6528 6466 5b62 795d 2e64 7479 7065  ype(df[by].dtype
-00010eb0: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
-00010ec0: 650a 2020 2020 2020 2020 656c 6966 2069  e.        elif i
-00010ed0: 7369 6e73 7461 6e63 6528 6279 2c20 4974  sinstance(by, It
-00010ee0: 6572 6162 6c65 293a 0a20 2020 2020 2020  erable):.       
-00010ef0: 2020 2020 2066 6f72 2063 6f6c 2069 6e20       for col in 
-00010f00: 6279 3a0a 2020 2020 2020 2020 2020 2020  by:.            
-00010f10: 2020 2020 6966 2063 6f6c 2069 6e20 6167      if col in ag
-00010f20: 6772 6567 6174 6564 2e63 6f6c 756d 6e73  gregated.columns
-00010f30: 2061 6e64 2064 665b 636f 6c5d 2e64 7479   and df[col].dty
-00010f40: 7065 2021 3d20 6167 6772 6567 6174 6564  pe != aggregated
-00010f50: 5b63 6f6c 5d2e 6474 7970 653a 0a20 2020  [col].dtype:.   
-00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f70: 2061 6767 7265 6761 7465 645b 636f 6c5d   aggregated[col]
-00010f80: 203d 2061 6767 7265 6761 7465 645b 636f   = aggregated[co
-00010f90: 6c5d 2e61 7374 7970 6528 6466 5b63 6f6c  l].astype(df[col
-00010fa0: 5d2e 6474 7970 6529 0a0a 2020 2020 6173  ].dtype)..    as
-00010fb0: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
-00010fc0: 6167 6772 6567 6174 6564 2c20 6770 642e  aggregated, gpd.
-00010fd0: 4765 6f44 6174 6146 7261 6d65 290a 2020  GeoDataFrame).  
-00010fe0: 2020 7265 7475 726e 2061 6767 7265 6761    return aggrega
-00010ff0: 7465 640a 0a0a 6465 6620 5f61 6464 5f6f  ted...def _add_o
-00011000: 7264 6572 6279 5f63 6f6c 756d 6e28 7061  rderby_column(pa
-00011010: 7468 3a20 5061 7468 2c20 6c61 7965 723a  th: Path, layer:
-00011020: 2073 7472 2c20 6e61 6d65 3a20 7374 7229   str, name: str)
-00011030: 3a0a 2020 2020 2320 5072 6570 6172 6520  :.    # Prepare 
-00011040: 7468 6520 6578 7072 6573 7369 6f6e 2074  the expression t
-00011050: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-00011060: 6f72 6465 7262 7920 636f 6c75 6d6e 2e0a  orderby column..
-00011070: 2020 2020 2320 496e 2061 2073 7061 7469      # In a spati
-00011080: 616c 2066 696c 652c 2061 2073 7061 7469  al file, a spati
-00011090: 616c 206f 7264 6572 2077 696c 6c20 6d61  al order will ma
-000110a0: 6b65 206c 6174 6572 2075 7365 206d 6f72  ke later use mor
-000110b0: 6520 6566 6669 6369 c3ab 6e74 2c0a 2020  e effici..nt,.  
-000110c0: 2020 2320 736f 2075 7365 2061 2067 656f    # so use a geo
-000110d0: 6861 7368 2e0a 2020 2020 6c61 7965 7269  hash..    layeri
-000110e0: 6e66 6f20 3d20 6766 6f2e 6765 745f 6c61  nfo = gfo.get_la
-000110f0: 7965 7269 6e66 6f28 7061 7468 290a 2020  yerinfo(path).  
-00011100: 2020 6966 206c 6179 6572 696e 666f 2e63    if layerinfo.c
-00011110: 7273 2069 7320 6e6f 7420 4e6f 6e65 2061  rs is not None a
-00011120: 6e64 206c 6179 6572 696e 666f 2e63 7273  nd layerinfo.crs
-00011130: 2e69 735f 6765 6f67 7261 7068 6963 3a0a  .is_geographic:.
-00011140: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
-00011150: 2063 6f6f 7264 696e 6174 6573 2061 7265   coordinates are
-00011160: 2067 656f 6772 6170 6869 6320 2869 6e20   geographic (in 
-00011170: 6c61 742f 6c6f 6e20 6465 6772 6565 7329  lat/lon degrees)
-00011180: 2c20 6f6b 0a20 2020 2020 2020 2065 7870  , ok.        exp
-00011190: 7265 7373 696f 6e20 3d20 6622 5354 5f47  ression = f"ST_G
-000111a0: 656f 4861 7368 287b 6c61 7965 7269 6e66  eoHash({layerinf
-000111b0: 6f2e 6765 6f6d 6574 7279 636f 6c75 6d6e  o.geometrycolumn
-000111c0: 7d2c 2031 3029 220a 2020 2020 656c 7365  }, 10)".    else
-000111d0: 3a0a 2020 2020 2020 2020 2320 4966 2074  :.        # If t
-000111e0: 6865 7920 6172 6520 6e6f 7420 6765 6f67  hey are not geog
-000111f0: 7261 7068 6963 2028 696e 206c 6174 2f6c  raphic (in lat/l
-00011200: 6f6e 2064 6567 7265 6573 292c 2074 6865  on degrees), the
-00011210: 7920 6e65 6564 2074 6f20 6265 0a20 2020  y need to be.   
-00011220: 2020 2020 2023 2063 6f6e 7665 7274 6564       # converted
-00011230: 2074 6f20 7e20 6465 6772 6565 7320 746f   to ~ degrees to
-00011240: 2062 6520 6162 6c65 2074 6f20 6361 6c63   be able to calc
-00011250: 756c 6174 6520 6120 6765 6f68 6173 682e  ulate a geohash.
-00011260: 0a0a 2020 2020 2020 2020 2320 5072 6f70  ..        # Prop
-00011270: 6572 6c79 2063 616c 6375 6c61 7469 6e67  erly calculating
-00011280: 2074 6865 2074 7261 6e73 666f 726d 6174   the transformat
-00011290: 696f 6e20 746f 2065 672e 2057 4753 2069  ion to eg. WGS i
-000112a0: 7320 7465 7272 6962 6c79 2073 6c6f 772e  s terribly slow.
-000112b0: 2e2e 0a20 2020 2020 2020 2023 2065 7870  ...        # exp
-000112c0: 7265 7373 696f 6e20 3d20 6622 2222 5354  ression = f"""ST
-000112d0: 5f47 656f 4861 7368 2853 545f 5472 616e  _GeoHash(ST_Tran
-000112e0: 7366 6f72 6d28 4d61 6b65 506f 696e 7428  sform(MakePoint(
-000112f0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-00011300: 2028 4d62 724d 6178 5828 6765 6f6d 292b   (MbrMaxX(geom)+
-00011310: 4d62 724d 696e 5828 6765 6f6d 2929 2f32  MbrMinX(geom))/2
-00011320: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-00011330: 2020 284d 6272 4d69 6e59 2867 656f 6d29    (MbrMinY(geom)
-00011340: 2b4d 6272 4d61 7859 2867 656f 6d29 292f  +MbrMaxY(geom))/
-00011350: 322c 2053 545f 5352 4944 2867 656f 6d29  2, ST_SRID(geom)
-00011360: 292c 2034 3332 3629 2c20 3130 2922 2222  ), 4326), 10)"""
-00011370: 0a20 2020 2020 2020 2023 2053 6f2c 2064  .        # So, d
-00011380: 6f20 736f 6d65 7468 696e 6720 656c 7365  o something else
-00011390: 2074 6861 7427 7320 6661 7374 6572 2061   that's faster a
-000113a0: 6e64 2073 7469 6c6c 2067 6976 6573 2061  nd still gives a
-000113b0: 2067 6f6f 640a 2020 2020 2020 2020 2320   good.        # 
-000113c0: 6765 6f67 7261 7068 6963 2063 6c75 7374  geographic clust
-000113d0: 6572 696e 672e 0a20 2020 2020 2020 2074  ering..        t
-000113e0: 6f5f 6765 6f67 7261 7068 6963 5f66 6163  o_geographic_fac
-000113f0: 746f 725f 6170 7072 6f78 203d 2039 3020  tor_approx = 90 
-00011400: 2f20 6d61 7828 6c61 7965 7269 6e66 6f2e  / max(layerinfo.
-00011410: 746f 7461 6c5f 626f 756e 6473 290a 2020  total_bounds).  
-00011420: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
-00011430: 203d 2066 2222 2253 545f 4765 6f48 6173   = f"""ST_GeoHas
-00011440: 6828 4d61 6b65 506f 696e 7428 0a20 2020  h(MakePoint(.   
-00011450: 2020 2020 2020 2020 2020 2020 2028 284d               ((M
-00011460: 6272 4d61 7858 287b 6c61 7965 7269 6e66  brMaxX({layerinf
-00011470: 6f2e 6765 6f6d 6574 7279 636f 6c75 6d6e  o.geometrycolumn
-00011480: 7d29 0a20 2020 2020 2020 2020 2020 2020  }).             
-00011490: 2020 2020 202b 4d62 724d 696e 5828 7b6c       +MbrMinX({l
-000114a0: 6179 6572 696e 666f 2e67 656f 6d65 7472  ayerinfo.geometr
-000114b0: 7963 6f6c 756d 6e7d 2929 2f32 0a20 2020  ycolumn}))/2.   
-000114c0: 2020 2020 2020 2020 2020 2020 2029 2a7b               )*{
-000114d0: 746f 5f67 656f 6772 6170 6869 635f 6661  to_geographic_fa
-000114e0: 6374 6f72 5f61 7070 726f 787d 2c0a 2020  ctor_approx},.  
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2828                ((
-00011500: 4d62 724d 696e 5928 7b6c 6179 6572 696e  MbrMinY({layerin
-00011510: 666f 2e67 656f 6d65 7472 7963 6f6c 756d  fo.geometrycolum
-00011520: 6e7d 290a 2020 2020 2020 2020 2020 2020  n}).            
-00011530: 2020 2020 2020 2b4d 6272 4d61 7859 287b        +MbrMaxY({
-00011540: 6c61 7965 7269 6e66 6f2e 6765 6f6d 6574  layerinfo.geomet
-00011550: 7279 636f 6c75 6d6e 7d29 292f 320a 2020  rycolumn}))/2.  
-00011560: 2020 2020 2020 2020 2020 2020 2020 292a                )*
-00011570: 7b74 6f5f 6765 6f67 7261 7068 6963 5f66  {to_geographic_f
-00011580: 6163 746f 725f 6170 7072 6f78 7d2c 2034  actor_approx}, 4
-00011590: 3332 3629 2c20 3130 2922 2222 0a0a 2020  326), 10)"""..  
-000115a0: 2020 2320 4e6f 7720 7765 2063 616e 2061    # Now we can a
-000115b0: 6374 7561 6c6c 7920 6164 6420 7468 6520  ctually add the 
-000115c0: 636f 6c75 6d6e 2e0a 2020 2020 6766 6f2e  column..    gfo.
-000115d0: 6164 645f 636f 6c75 6d6e 2870 6174 683d  add_column(path=
-000115e0: 7061 7468 2c20 6e61 6d65 3d6e 616d 652c  path, name=name,
-000115f0: 2074 7970 653d 6766 6f2e 4461 7461 5479   type=gfo.DataTy
-00011600: 7065 2e54 4558 542c 2065 7870 7265 7373  pe.TEXT, express
-00011610: 696f 6e3d 6578 7072 6573 7369 6f6e 290a  ion=expression).
-00011620: 2020 2020 7371 6c69 7465 5f73 746d 7420      sqlite_stmt 
-00011630: 3d20 6627 4352 4541 5445 2049 4e44 4558  = f'CREATE INDEX
-00011640: 207b 6e61 6d65 7d5f 6964 7820 4f4e 2022   {name}_idx ON "
-00011650: 7b6c 6179 6572 7d22 287b 6e61 6d65 7d29  {layer}"({name})
-00011660: 270a 2020 2020 6766 6f2e 6578 6563 7574  '.    gfo.execut
-00011670: 655f 7371 6c28 7061 7468 3d70 6174 682c  e_sql(path=path,
-00011680: 2073 716c 5f73 746d 743d 7371 6c69 7465   sql_stmt=sqlite
-00011690: 5f73 746d 7429 0a                        _stmt).
+00010250: 2e31 2e30 2e0a 2020 2020 2020 2020 4120  .1.0..        A 
+00010260: 7761 726e 696e 6720 7769 6c6c 2062 6520  warning will be 
+00010270: 656d 6974 7465 6420 666f 7220 6561 726c  emitted for earl
+00010280: 6965 7220 7061 6e64 6173 2076 6572 7369  ier pandas versi
+00010290: 6f6e 730a 2020 2020 2020 2020 6966 2061  ons.        if a
+000102a0: 206e 6f6e 2d64 6566 6175 6c74 2076 616c   non-default val
+000102b0: 7565 2069 7320 6769 7665 6e20 666f 7220  ue is given for 
+000102c0: 7468 6973 2070 6172 616d 6574 6572 2e0a  this parameter..
+000102d0: 2020 2020 2020 2020 2e2e 2076 6572 7369          .. versi
+000102e0: 6f6e 6164 6465 643a 3a20 302e 392e 300a  onadded:: 0.9.0.
+000102f0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00010300: 2d2d 2d2d 2d2d 2d0a 2020 2020 4765 6f44  -------.    GeoD
+00010310: 6174 6146 7261 6d65 0a20 2020 2045 7861  ataFrame.    Exa
+00010320: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+00010330: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
+00010340: 7368 6170 656c 792e 6765 6f6d 6574 7279  shapely.geometry
+00010350: 2069 6d70 6f72 7420 506f 696e 740a 2020   import Point.  
+00010360: 2020 3e3e 3e20 6420 3d20 7b0a 2020 2020    >>> d = {.    
+00010370: 2e2e 2e20 2020 2020 2263 6f6c 3122 3a20  ...     "col1": 
+00010380: 5b22 6e61 6d65 3122 2c20 226e 616d 6532  ["name1", "name2
+00010390: 222c 2022 6e61 6d65 3122 5d2c 0a20 2020  ", "name1"],.   
+000103a0: 202e 2e2e 2020 2020 2022 6765 6f6d 6574   ...     "geomet
+000103b0: 7279 223a 205b 506f 696e 7428 312c 2032  ry": [Point(1, 2
+000103c0: 292c 2050 6f69 6e74 2832 2c20 3129 2c20  ), Point(2, 1), 
+000103d0: 506f 696e 7428 302c 2031 295d 2c0a 2020  Point(0, 1)],.  
+000103e0: 2020 2e2e 2e20 7d0a 2020 2020 3e3e 3e20    ... }.    >>> 
+000103f0: 6764 6620 3d20 6765 6f70 616e 6461 732e  gdf = geopandas.
+00010400: 4765 6f44 6174 6146 7261 6d65 2864 2c20  GeoDataFrame(d, 
+00010410: 6372 733d 3433 3236 290a 2020 2020 3e3e  crs=4326).    >>
+00010420: 3e20 6764 660a 2020 2020 2020 2020 636f  > gdf.        co
+00010430: 6c31 2020 2020 2020 2020 2020 2020 2020  l1              
+00010440: 2020 2067 656f 6d65 7472 790a 2020 2020     geometry.    
+00010450: 3020 206e 616d 6531 2020 504f 494e 5420  0  name1  POINT 
+00010460: 2831 2e30 3030 3030 2032 2e30 3030 3030  (1.00000 2.00000
+00010470: 290a 2020 2020 3120 206e 616d 6532 2020  ).    1  name2  
+00010480: 504f 494e 5420 2832 2e30 3030 3030 2031  POINT (2.00000 1
+00010490: 2e30 3030 3030 290a 2020 2020 3220 206e  .00000).    2  n
+000104a0: 616d 6531 2020 504f 494e 5420 2830 2e30  ame1  POINT (0.0
+000104b0: 3030 3030 2031 2e30 3030 3030 290a 2020  0000 1.00000).  
+000104c0: 2020 3e3e 3e20 6469 7373 6f6c 7665 6420    >>> dissolved 
+000104d0: 3d20 6764 662e 6469 7373 6f6c 7665 2827  = gdf.dissolve('
+000104e0: 636f 6c31 2729 0a20 2020 203e 3e3e 2064  col1').    >>> d
+000104f0: 6973 736f 6c76 6564 2020 2320 646f 6374  issolved  # doct
+00010500: 6573 743a 202b 534b 4950 0a20 2020 2020  est: +SKIP.     
+00010510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010530: 2020 2020 2020 2020 2020 2067 656f 6d65             geome
+00010540: 7472 790a 2020 2020 636f 6c31 0a20 2020  try.    col1.   
+00010550: 206e 616d 6531 2020 4d55 4c54 4950 4f49   name1  MULTIPOI
+00010560: 4e54 2028 302e 3030 3030 3020 312e 3030  NT (0.00000 1.00
+00010570: 3030 302c 2031 2e30 3030 3030 2032 2e30  000, 1.00000 2.0
+00010580: 3030 3030 290a 2020 2020 6e61 6d65 3220  0000).    name2 
+00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105a0: 2020 2020 2020 2050 4f49 4e54 2028 322e         POINT (2.
+000105b0: 3030 3030 3020 312e 3030 3030 3029 0a20  00000 1.00000). 
+000105c0: 2020 2053 6565 2061 6c73 6f0a 2020 2020     See also.    
+000105d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2047 656f  --------.    Geo
+000105e0: 4461 7461 4672 616d 652e 6578 706c 6f64  DataFrame.explod
+000105f0: 6520 3a20 6578 706c 6f64 6520 6d75 6c74  e : explode mult
+00010600: 692d 7061 7274 2067 656f 6d65 7472 6965  i-part geometrie
+00010610: 7320 696e 746f 2073 696e 676c 6520 6765  s into single ge
+00010620: 6f6d 6574 7269 6573 0a20 2020 2022 2222  ometries.    """
+00010630: 0a0a 2020 2020 6966 2062 7920 6973 204e  ..    if by is N
+00010640: 6f6e 6520 616e 6420 6c65 7665 6c20 6973  one and level is
+00010650: 204e 6f6e 653a 0a20 2020 2020 2020 2062   None:.        b
+00010660: 795f 6c6f 6361 6c20 3d20 6e70 2e7a 6572  y_local = np.zer
+00010670: 6f73 286c 656e 2864 6629 2c20 6474 7970  os(len(df), dtyp
+00010680: 653d 2269 6e74 3634 2229 0a20 2020 2065  e="int64").    e
+00010690: 6c73 653a 0a20 2020 2020 2020 2062 795f  lse:.        by_
+000106a0: 6c6f 6361 6c20 3d20 6279 0a0a 2020 2020  local = by..    
+000106b0: 6772 6f75 7062 795f 6b77 6172 6773 203d  groupby_kwargs =
+000106c0: 2064 6963 7428 0a20 2020 2020 2020 2062   dict(.        b
+000106d0: 793d 6279 5f6c 6f63 616c 2c20 6c65 7665  y=by_local, leve
+000106e0: 6c3d 6c65 7665 6c2c 2073 6f72 743d 736f  l=level, sort=so
+000106f0: 7274 2c20 6f62 7365 7276 6564 3d6f 6273  rt, observed=obs
+00010700: 6572 7665 642c 2064 726f 706e 613d 6472  erved, dropna=dr
+00010710: 6f70 6e61 0a20 2020 2029 0a20 2020 2022  opna.    ).    "
+00010720: 2222 0a20 2020 2069 6620 6e6f 7420 636f  "".    if not co
+00010730: 6d70 6174 2e50 414e 4441 535f 4745 5f31  mpat.PANDAS_GE_1
+00010740: 313a 0a20 2020 2020 2020 2067 726f 7570  1:.        group
+00010750: 6279 5f6b 7761 7267 732e 706f 7028 2264  by_kwargs.pop("d
+00010760: 726f 706e 6122 290a 0a20 2020 2020 2020  ropna")..       
+00010770: 2069 6620 6e6f 7420 6472 6f70 6e61 3a20   if not dropna: 
+00010780: 2023 2049 6620 7468 6579 2070 6173 7365   # If they passe
+00010790: 6420 6120 6e6f 6e2d 6465 6661 756c 7420  d a non-default 
+000107a0: 6472 6f70 6e61 2076 616c 7565 0a20 2020  dropna value.   
+000107b0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+000107c0: 732e 7761 726e 2822 6472 6f70 6e61 206b  s.warn("dropna k
+000107d0: 7761 7267 2069 7320 6e6f 7420 7375 7070  warg is not supp
+000107e0: 6f72 7465 6420 666f 7220 7061 6e64 6173  orted for pandas
+000107f0: 203c 2031 2e31 2e30 2229 0a20 2020 2022   < 1.1.0").    "
+00010800: 2222 0a0a 2020 2020 2320 5072 6f63 6573  ""..    # Proces
+00010810: 7320 6e6f 6e2d 7370 6174 6961 6c20 636f  s non-spatial co
+00010820: 6d70 6f6e 656e 740a 2020 2020 6461 7461  mponent.    data
+00010830: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+00010840: 6466 2e64 726f 7028 636f 6c75 6d6e 733d  df.drop(columns=
+00010850: 6466 2e67 656f 6d65 7472 792e 6e61 6d65  df.geometry.name
+00010860: 2929 0a0a 2020 2020 6966 2061 6767 6675  ))..    if aggfu
+00010870: 6e63 2069 7320 6e6f 7420 4e6f 6e65 2061  nc is not None a
+00010880: 6e64 2069 7369 6e73 7461 6e63 6528 6167  nd isinstance(ag
+00010890: 6766 756e 632c 2064 6963 7429 2061 6e64  gfunc, dict) and
+000108a0: 2022 746f 5f6a 736f 6e22 2069 6e20 6167   "to_json" in ag
+000108b0: 6766 756e 633a 0a20 2020 2020 2020 2061  gfunc:.        a
+000108c0: 6767 5f63 6f6c 756d 6e73 203d 206c 6973  gg_columns = lis
+000108d0: 7428 7365 7428 6167 6766 756e 635b 2274  t(set(aggfunc["t
+000108e0: 6f5f 6a73 6f6e 225d 2929 0a20 2020 2020  o_json"])).     
+000108f0: 2020 2061 6767 7265 6761 7465 645f 6461     aggregated_da
+00010900: 7461 203d 2028 0a20 2020 2020 2020 2020  ta = (.         
+00010910: 2020 2064 6174 612e 6772 6f75 7062 7928     data.groupby(
+00010920: 2a2a 6772 6f75 7062 795f 6b77 6172 6773  **groupby_kwargs
+00010930: 290a 2020 2020 2020 2020 2020 2020 2e61  ).            .a
+00010940: 7070 6c79 286c 616d 6264 6120 673a 2067  pply(lambda g: g
+00010950: 5b61 6767 5f63 6f6c 756d 6e73 5d2e 746f  [agg_columns].to
+00010960: 5f6a 736f 6e28 6f72 6965 6e74 3d22 7265  _json(orient="re
+00010970: 636f 7264 7322 2929 0a20 2020 2020 2020  cords")).       
+00010980: 2020 2020 202e 746f 5f66 7261 6d65 286e       .to_frame(n
+00010990: 616d 653d 225f 5f44 4953 534f 4c56 455f  ame="__DISSOLVE_
+000109a0: 544f 4a53 4f4e 2229 0a20 2020 2020 2020  TOJSON").       
+000109b0: 2029 0a20 2020 2065 6c69 6620 6973 696e   ).    elif isin
+000109c0: 7374 616e 6365 2861 6767 6675 6e63 2c20  stance(aggfunc, 
+000109d0: 7374 7229 2061 6e64 2061 6767 6675 6e63  str) and aggfunc
+000109e0: 203d 3d20 226d 6572 6765 5f6a 736f 6e5f   == "merge_json_
+000109f0: 6c69 7374 7322 3a0a 2020 2020 2020 2020  lists":.        
+00010a00: 2320 4d65 7267 6520 616e 6420 666c 6174  # Merge and flat
+00010a10: 7465 6e20 7468 6520 6a73 6f6e 206c 6973  ten the json lis
+00010a20: 7473 2069 6e20 7468 6520 6772 6f75 7073  ts in the groups
+00010a30: 0a20 2020 2020 2020 2064 6566 2067 726f  .        def gro
+00010a40: 7570 5f66 6c61 7474 656e 5f6a 736f 6e5f  up_flatten_json_
+00010a50: 6c69 7374 2867 293a 0a20 2020 2020 2020  list(g):.       
+00010a60: 2020 2020 2023 2045 7661 6c75 6174 6520       # Evaluate 
+00010a70: 616c 6c20 6772 6f75 7065 6420 726f 7773  all grouped rows
+00010a80: 2074 6f20 6a73 6f6e 206f 626a 6563 7473   to json objects
+00010a90: 2e20 5468 6973 2072 6573 756c 7473 2069  . This results i
+00010aa0: 6e20 6120 6c69 7374 206f 660a 2020 2020  n a list of.    
+00010ab0: 2020 2020 2020 2020 2320 6c69 7374 7320          # lists 
+00010ac0: 6f66 206a 736f 6e20 6f62 6a65 6374 732e  of json objects.
+00010ad0: 0a20 2020 2020 2020 2020 2020 206a 736f  .            jso
+00010ae0: 6e5f 6e65 7374 6564 5f6c 6973 7473 203d  n_nested_lists =
+00010af0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00010b00: 2020 206a 736f 6e2e 6c6f 6164 7328 6a73     json.loads(js
+00010b10: 6f6e 5f76 616c 7565 7329 2066 6f72 206a  on_values) for j
+00010b20: 736f 6e5f 7661 6c75 6573 2069 6e20 675b  son_values in g[
+00010b30: 225f 5f44 4953 534f 4c56 455f 544f 4a53  "__DISSOLVE_TOJS
+00010b40: 4f4e 225d 0a20 2020 2020 2020 2020 2020  ON"].           
+00010b50: 205d 0a0a 2020 2020 2020 2020 2020 2020   ]..            
+00010b60: 2320 4578 7472 6163 7420 7468 6520 726f  # Extract the ro
+00010b70: 7773 2066 726f 6d20 7468 6520 6e65 7374  ws from the nest
+00010b80: 6564 206c 6973 7473 202b 2070 7574 2069  ed lists + put i
+00010b90: 6e20 6120 666c 6174 206c 6973 7420 6173  n a flat list as
+00010ba0: 2073 7472 696e 6773 0a20 2020 2020 2020   strings.       
+00010bb0: 2020 2020 206a 736f 6e73 7472 5f66 6c61       jsonstr_fla
+00010bc0: 7420 3d20 5b0a 2020 2020 2020 2020 2020  t = [.          
+00010bd0: 2020 2020 2020 6a73 6f6e 2e64 756d 7073        json.dumps
+00010be0: 286a 736f 6e5f 7661 6c75 6529 0a20 2020  (json_value).   
+00010bf0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00010c00: 206a 736f 6e5f 7661 6c75 6573 2069 6e20   json_values in 
+00010c10: 6a73 6f6e 5f6e 6573 7465 645f 6c69 7374  json_nested_list
+00010c20: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00010c30: 2020 666f 7220 6a73 6f6e 5f76 616c 7565    for json_value
+00010c40: 2069 6e20 6a73 6f6e 5f76 616c 7565 730a   in json_values.
+00010c50: 2020 2020 2020 2020 2020 2020 5d0a 0a20              ].. 
+00010c60: 2020 2020 2020 2020 2020 2023 2052 656d             # Rem
+00010c70: 6f76 6520 6475 706c 6963 6174 6573 0a20  ove duplicates. 
+00010c80: 2020 2020 2020 2020 2020 206a 736f 6e73             jsons
+00010c90: 7374 725f 6469 7374 696e 6374 203d 2073  str_distinct = s
+00010ca0: 6574 286a 736f 6e73 7472 5f66 6c61 7429  et(jsonstr_flat)
+00010cb0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00010cc0: 436f 6e76 6572 7420 7468 6520 6461 7461  Convert the data
+00010cd0: 2061 6761 696e 2074 6f20 6120 6c69 7374   again to a list
+00010ce0: 206f 6620 6a73 6f6e 206f 626a 6563 7473   of json objects
+00010cf0: 0a20 2020 2020 2020 2020 2020 206a 736f  .            jso
+00010d00: 6e5f 6469 7374 696e 6374 203d 205b 6a73  n_distinct = [js
+00010d10: 6f6e 2e6c 6f61 6473 286a 736f 6e5f 7661  on.loads(json_va
+00010d20: 6c75 6529 2066 6f72 206a 736f 6e5f 7661  lue) for json_va
+00010d30: 6c75 6520 696e 206a 736f 6e73 7374 725f  lue in jsonsstr_
+00010d40: 6469 7374 696e 6374 5d0a 0a20 2020 2020  distinct]..     
+00010d50: 2020 2020 2020 2023 2052 6574 7572 6e20         # Return 
+00010d60: 6173 206a 736f 6e20 7374 7269 6e67 0a20  as json string. 
+00010d70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00010d80: 6e20 6a73 6f6e 2e64 756d 7073 286a 736f  n json.dumps(jso
+00010d90: 6e5f 6469 7374 696e 6374 290a 0a20 2020  n_distinct)..   
+00010da0: 2020 2020 2061 6767 7265 6761 7465 645f       aggregated_
+00010db0: 6461 7461 203d 2028 0a20 2020 2020 2020  data = (.       
+00010dc0: 2020 2020 2064 6174 612e 6772 6f75 7062       data.groupb
+00010dd0: 7928 2a2a 6772 6f75 7062 795f 6b77 6172  y(**groupby_kwar
+00010de0: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
+00010df0: 2e61 7070 6c79 286c 616d 6264 6120 673a  .apply(lambda g:
+00010e00: 2067 726f 7570 5f66 6c61 7474 656e 5f6a   group_flatten_j
+00010e10: 736f 6e5f 6c69 7374 2867 2929 0a20 2020  son_list(g)).   
+00010e20: 2020 2020 2020 2020 202e 746f 5f66 7261           .to_fra
+00010e30: 6d65 286e 616d 653d 225f 5f44 4953 534f  me(name="__DISSO
+00010e40: 4c56 455f 544f 4a53 4f4e 2229 0a20 2020  LVE_TOJSON").   
+00010e50: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
+00010e60: 0a20 2020 2020 2020 2061 6767 7265 6761  .        aggrega
+00010e70: 7465 645f 6461 7461 203d 2064 6174 612e  ted_data = data.
+00010e80: 6772 6f75 7062 7928 2a2a 6772 6f75 7062  groupby(**groupb
+00010e90: 795f 6b77 6172 6773 292e 6167 6728 6167  y_kwargs).agg(ag
+00010ea0: 6766 756e 6329 2020 2320 7479 7065 3a20  gfunc)  # type: 
+00010eb0: 6967 6e6f 7265 0a20 2020 2020 2020 2023  ignore.        #
+00010ec0: 2043 6865 636b 2069 6620 616c 6c20 636f   Check if all co
+00010ed0: 6c75 6d6e 7320 7765 7265 2070 726f 7065  lumns were prope
+00010ee0: 726c 7920 6167 6772 6567 6174 6564 0a20  rly aggregated. 
+00010ef0: 2020 2020 2020 2061 7373 6572 7420 6279         assert by
+00010f00: 5f6c 6f63 616c 2069 7320 6e6f 7420 4e6f  _local is not No
+00010f10: 6e65 0a20 2020 2020 2020 2063 6f6c 756d  ne.        colum
+00010f20: 6e73 5f74 6f5f 6167 6720 3d20 5b63 6f6c  ns_to_agg = [col
+00010f30: 756d 6e20 666f 7220 636f 6c75 6d6e 2069  umn for column i
+00010f40: 6e20 6461 7461 2e63 6f6c 756d 6e73 2069  n data.columns i
+00010f50: 6620 636f 6c75 6d6e 206e 6f74 2069 6e20  f column not in 
+00010f60: 6279 5f6c 6f63 616c 5d0a 2020 2020 2020  by_local].      
+00010f70: 2020 6966 206c 656e 2863 6f6c 756d 6e73    if len(columns
+00010f80: 5f74 6f5f 6167 6729 2021 3d20 6c65 6e28  _to_agg) != len(
+00010f90: 6167 6772 6567 6174 6564 5f64 6174 612e  aggregated_data.
+00010fa0: 636f 6c75 6d6e 7329 3a0a 2020 2020 2020  columns):.      
+00010fb0: 2020 2020 2020 6472 6f70 7065 645f 636f        dropped_co
+00010fc0: 6c75 6d6e 7320 3d20 5b0a 2020 2020 2020  lumns = [.      
+00010fd0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00010fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ff0: 2066 6f72 2063 6f6c 756d 6e20 696e 2063   for column in c
+00011000: 6f6c 756d 6e73 5f74 6f5f 6167 670a 2020  olumns_to_agg.  
+00011010: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011020: 2063 6f6c 756d 6e20 6e6f 7420 696e 2061   column not in a
+00011030: 6767 7265 6761 7465 645f 6461 7461 2e63  ggregated_data.c
+00011040: 6f6c 756d 6e73 0a20 2020 2020 2020 2020  olumns.         
+00011050: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00011060: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+00011070: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011080: 2020 6622 436f 6c75 6d6e 2873 2920 7b64    f"Column(s) {d
+00011090: 726f 7070 6564 5f63 6f6c 756d 6e73 7d20  ropped_columns} 
+000110a0: 6172 6520 6e6f 7420 7375 7070 6f72 7465  are not supporte
+000110b0: 6420 666f 7220 6167 6772 6567 6174 696f  d for aggregatio
+000110c0: 6e2c 2073 746f 7022 0a20 2020 2020 2020  n, stop".       
+000110d0: 2020 2020 2029 0a0a 2020 2020 2320 5072       )..    # Pr
+000110e0: 6f63 6573 7320 7370 6174 6961 6c20 636f  ocess spatial co
+000110f0: 6d70 6f6e 656e 740a 2020 2020 6465 6620  mponent.    def 
+00011100: 6d65 7267 655f 6765 6f6d 6574 7269 6573  merge_geometries
+00011110: 2862 6c6f 636b 293a 0a20 2020 2020 2020  (block):.       
+00011120: 206d 6572 6765 645f 6765 6f6d 203d 2062   merged_geom = b
+00011130: 6c6f 636b 2e75 6e61 7279 5f75 6e69 6f6e  lock.unary_union
+00011140: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011150: 6d65 7267 6564 5f67 656f 6d0a 0a20 2020  merged_geom..   
+00011160: 2067 203d 2064 662e 6772 6f75 7062 7928   g = df.groupby(
+00011170: 6772 6f75 705f 6b65 7973 3d46 616c 7365  group_keys=False
+00011180: 2c20 2a2a 6772 6f75 7062 795f 6b77 6172  , **groupby_kwar
+00011190: 6773 295b 6466 2e67 656f 6d65 7472 792e  gs)[df.geometry.
+000111a0: 6e61 6d65 5d2e 6167 6728 0a20 2020 2020  name].agg(.     
+000111b0: 2020 206d 6572 6765 5f67 656f 6d65 7472     merge_geometr
+000111c0: 6965 730a 2020 2020 290a 0a20 2020 2023  ies.    )..    #
+000111d0: 2041 6767 7265 6761 7465 0a20 2020 2061   Aggregate.    a
+000111e0: 6767 7265 6761 7465 645f 6765 6f6d 6574  ggregated_geomet
+000111f0: 7279 203d 2067 7064 2e47 656f 4461 7461  ry = gpd.GeoData
+00011200: 4672 616d 6528 0a20 2020 2020 2020 2064  Frame(.        d
+00011210: 6174 613d 672c 2067 656f 6d65 7472 793d  ata=g, geometry=
+00011220: 6466 2e67 656f 6d65 7472 792e 6e61 6d65  df.geometry.name
+00011230: 2c20 6372 733d 6466 2e63 7273 2020 2320  , crs=df.crs  # 
+00011240: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+00011250: 2029 0a20 2020 2023 2052 6563 6f6d 6269   ).    # Recombi
+00011260: 6e65 0a20 2020 2061 6767 7265 6761 7465  ne.    aggregate
+00011270: 6420 3d20 6167 6772 6567 6174 6564 5f67  d = aggregated_g
+00011280: 656f 6d65 7472 792e 6a6f 696e 2861 6767  eometry.join(agg
+00011290: 7265 6761 7465 645f 6461 7461 290a 0a20  regated_data).. 
+000112a0: 2020 2023 2052 6573 6574 2069 6620 7265     # Reset if re
+000112b0: 7175 6573 7465 640a 2020 2020 6966 206e  quested.    if n
+000112c0: 6f74 2061 735f 696e 6465 783a 0a20 2020  ot as_index:.   
+000112d0: 2020 2020 2061 6767 7265 6761 7465 6420       aggregated 
+000112e0: 3d20 6167 6772 6567 6174 6564 2e72 6573  = aggregated.res
+000112f0: 6574 5f69 6e64 6578 2829 0a0a 2020 2020  et_index()..    
+00011300: 2320 4d61 6b65 2073 7572 6520 6f75 7470  # Make sure outp
+00011310: 7574 2074 7970 6573 206f 6620 6772 6f75  ut types of grou
+00011320: 7065 6420 636f 6c75 6d6e 7320 6172 6520  ped columns are 
+00011330: 7468 6520 7361 6d65 2061 7320 696e 7075  the same as inpu
+00011340: 7420 7479 7065 732e 0a20 2020 2023 2045  t types..    # E
+00011350: 2e67 2e20 6f62 6a65 6374 2063 6f6c 756d  .g. object colum
+00011360: 6e73 2062 6563 6f6d 6520 666c 6f61 7420  ns become float 
+00011370: 6966 2061 6c6c 2076 616c 7565 7320 6172  if all values ar
+00011380: 6520 4e6f 6e65 2e0a 2020 2020 6966 2062  e None..    if b
+00011390: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+000113a0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+000113b0: 616e 6365 2862 792c 2073 7472 293a 0a20  ance(by, str):. 
+000113c0: 2020 2020 2020 2020 2020 2069 6620 6279             if by
+000113d0: 2069 6e20 6167 6772 6567 6174 6564 2e63   in aggregated.c
+000113e0: 6f6c 756d 6e73 2061 6e64 2064 665b 6279  olumns and df[by
+000113f0: 5d2e 6474 7970 6520 213d 2061 6767 7265  ].dtype != aggre
+00011400: 6761 7465 645b 6279 5d2e 6474 7970 653a  gated[by].dtype:
+00011410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011420: 2061 6767 7265 6761 7465 645b 6279 5d20   aggregated[by] 
+00011430: 3d20 6167 6772 6567 6174 6564 5b62 795d  = aggregated[by]
+00011440: 2e61 7374 7970 6528 6466 5b62 795d 2e64  .astype(df[by].d
+00011450: 7479 7065 2920 2023 2074 7970 653a 2069  type)  # type: i
+00011460: 676e 6f72 650a 2020 2020 2020 2020 656c  gnore.        el
+00011470: 6966 2069 7369 6e73 7461 6e63 6528 6279  if isinstance(by
+00011480: 2c20 4974 6572 6162 6c65 293a 0a20 2020  , Iterable):.   
+00011490: 2020 2020 2020 2020 2066 6f72 2063 6f6c           for col
+000114a0: 2069 6e20 6279 3a0a 2020 2020 2020 2020   in by:.        
+000114b0: 2020 2020 2020 2020 6966 2063 6f6c 2069          if col i
+000114c0: 6e20 6167 6772 6567 6174 6564 2e63 6f6c  n aggregated.col
+000114d0: 756d 6e73 2061 6e64 2064 665b 636f 6c5d  umns and df[col]
+000114e0: 2e64 7479 7065 2021 3d20 6167 6772 6567  .dtype != aggreg
+000114f0: 6174 6564 5b63 6f6c 5d2e 6474 7970 653a  ated[col].dtype:
+00011500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011510: 2020 2020 2061 6767 7265 6761 7465 645b       aggregated[
+00011520: 636f 6c5d 203d 2061 6767 7265 6761 7465  col] = aggregate
+00011530: 645b 636f 6c5d 2e61 7374 7970 6528 6466  d[col].astype(df
+00011540: 5b63 6f6c 5d2e 6474 7970 6529 0a0a 2020  [col].dtype)..  
+00011550: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00011560: 6e63 6528 6167 6772 6567 6174 6564 2c20  nce(aggregated, 
+00011570: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
+00011580: 290a 2020 2020 7265 7475 726e 2061 6767  ).    return agg
+00011590: 7265 6761 7465 640a 0a0a 6465 6620 5f61  regated...def _a
+000115a0: 6464 5f6f 7264 6572 6279 5f63 6f6c 756d  dd_orderby_colum
+000115b0: 6e28 7061 7468 3a20 5061 7468 2c20 6c61  n(path: Path, la
+000115c0: 7965 723a 2073 7472 2c20 6e61 6d65 3a20  yer: str, name: 
+000115d0: 7374 7229 3a0a 2020 2020 2320 5072 6570  str):.    # Prep
+000115e0: 6172 6520 7468 6520 6578 7072 6573 7369  are the expressi
+000115f0: 6f6e 2074 6f20 6361 6c63 756c 6174 6520  on to calculate 
+00011600: 7468 6520 6f72 6465 7262 7920 636f 6c75  the orderby colu
+00011610: 6d6e 2e0a 2020 2020 2320 496e 2061 2073  mn..    # In a s
+00011620: 7061 7469 616c 2066 696c 652c 2061 2073  patial file, a s
+00011630: 7061 7469 616c 206f 7264 6572 2077 696c  patial order wil
+00011640: 6c20 6d61 6b65 206c 6174 6572 2075 7365  l make later use
+00011650: 206d 6f72 6520 6566 6669 6369 c3ab 6e74   more effici..nt
+00011660: 2c0a 2020 2020 2320 736f 2075 7365 2061  ,.    # so use a
+00011670: 2067 656f 6861 7368 2e0a 2020 2020 6c61   geohash..    la
+00011680: 7965 7269 6e66 6f20 3d20 6766 6f2e 6765  yerinfo = gfo.ge
+00011690: 745f 6c61 7965 7269 6e66 6f28 7061 7468  t_layerinfo(path
+000116a0: 290a 2020 2020 6966 206c 6179 6572 696e  ).    if layerin
+000116b0: 666f 2e63 7273 2069 7320 6e6f 7420 4e6f  fo.crs is not No
+000116c0: 6e65 2061 6e64 206c 6179 6572 696e 666f  ne and layerinfo
+000116d0: 2e63 7273 2e69 735f 6765 6f67 7261 7068  .crs.is_geograph
+000116e0: 6963 3a0a 2020 2020 2020 2020 2320 4966  ic:.        # If
+000116f0: 2074 6865 2063 6f6f 7264 696e 6174 6573   the coordinates
+00011700: 2061 7265 2067 656f 6772 6170 6869 6320   are geographic 
+00011710: 2869 6e20 6c61 742f 6c6f 6e20 6465 6772  (in lat/lon degr
+00011720: 6565 7329 2c20 6f6b 0a20 2020 2020 2020  ees), ok.       
+00011730: 2065 7870 7265 7373 696f 6e20 3d20 6622   expression = f"
+00011740: 5354 5f47 656f 4861 7368 287b 6c61 7965  ST_GeoHash({laye
+00011750: 7269 6e66 6f2e 6765 6f6d 6574 7279 636f  rinfo.geometryco
+00011760: 6c75 6d6e 7d2c 2031 3029 220a 2020 2020  lumn}, 10)".    
+00011770: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+00011780: 4966 2074 6865 7920 6172 6520 6e6f 7420  If they are not 
+00011790: 6765 6f67 7261 7068 6963 2028 696e 206c  geographic (in l
+000117a0: 6174 2f6c 6f6e 2064 6567 7265 6573 292c  at/lon degrees),
+000117b0: 2074 6865 7920 6e65 6564 2074 6f20 6265   they need to be
+000117c0: 0a20 2020 2020 2020 2023 2063 6f6e 7665  .        # conve
+000117d0: 7274 6564 2074 6f20 7e20 6465 6772 6565  rted to ~ degree
+000117e0: 7320 746f 2062 6520 6162 6c65 2074 6f20  s to be able to 
+000117f0: 6361 6c63 756c 6174 6520 6120 6765 6f68  calculate a geoh
+00011800: 6173 682e 0a0a 2020 2020 2020 2020 2320  ash...        # 
+00011810: 5072 6f70 6572 6c79 2063 616c 6375 6c61  Properly calcula
+00011820: 7469 6e67 2074 6865 2074 7261 6e73 666f  ting the transfo
+00011830: 726d 6174 696f 6e20 746f 2065 672e 2057  rmation to eg. W
+00011840: 4753 2069 7320 7465 7272 6962 6c79 2073  GS is terribly s
+00011850: 6c6f 772e 2e2e 0a20 2020 2020 2020 2023  low....        #
+00011860: 2065 7870 7265 7373 696f 6e20 3d20 6622   expression = f"
+00011870: 2222 5354 5f47 656f 4861 7368 2853 545f  ""ST_GeoHash(ST_
+00011880: 5472 616e 7366 6f72 6d28 4d61 6b65 506f  Transform(MakePo
+00011890: 696e 7428 0a20 2020 2020 2020 2023 2020  int(.        #  
+000118a0: 2020 2020 2028 4d62 724d 6178 5828 6765       (MbrMaxX(ge
+000118b0: 6f6d 292b 4d62 724d 696e 5828 6765 6f6d  om)+MbrMinX(geom
+000118c0: 2929 2f32 2c0a 2020 2020 2020 2020 2320  ))/2,.        # 
+000118d0: 2020 2020 2020 284d 6272 4d69 6e59 2867        (MbrMinY(g
+000118e0: 656f 6d29 2b4d 6272 4d61 7859 2867 656f  eom)+MbrMaxY(geo
+000118f0: 6d29 292f 322c 2053 545f 5352 4944 2867  m))/2, ST_SRID(g
+00011900: 656f 6d29 292c 2034 3332 3629 2c20 3130  eom)), 4326), 10
+00011910: 2922 2222 0a20 2020 2020 2020 2023 2053  )""".        # S
+00011920: 6f2c 2064 6f20 736f 6d65 7468 696e 6720  o, do something 
+00011930: 656c 7365 2074 6861 7427 7320 6661 7374  else that's fast
+00011940: 6572 2061 6e64 2073 7469 6c6c 2067 6976  er and still giv
+00011950: 6573 2061 2067 6f6f 640a 2020 2020 2020  es a good.      
+00011960: 2020 2320 6765 6f67 7261 7068 6963 2063    # geographic c
+00011970: 6c75 7374 6572 696e 672e 0a20 2020 2020  lustering..     
+00011980: 2020 2074 6f5f 6765 6f67 7261 7068 6963     to_geographic
+00011990: 5f66 6163 746f 725f 6170 7072 6f78 203d  _factor_approx =
+000119a0: 2039 3020 2f20 6d61 7828 6c61 7965 7269   90 / max(layeri
+000119b0: 6e66 6f2e 746f 7461 6c5f 626f 756e 6473  nfo.total_bounds
+000119c0: 290a 2020 2020 2020 2020 6578 7072 6573  ).        expres
+000119d0: 7369 6f6e 203d 2066 2222 2253 545f 4765  sion = f"""ST_Ge
+000119e0: 6f48 6173 6828 4d61 6b65 506f 696e 7428  oHash(MakePoint(
+000119f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a00: 2028 284d 6272 4d61 7858 287b 6c61 7965   ((MbrMaxX({laye
+00011a10: 7269 6e66 6f2e 6765 6f6d 6574 7279 636f  rinfo.geometryco
+00011a20: 6c75 6d6e 7d29 0a20 2020 2020 2020 2020  lumn}).         
+00011a30: 2020 2020 2020 2020 202b 4d62 724d 696e           +MbrMin
+00011a40: 5828 7b6c 6179 6572 696e 666f 2e67 656f  X({layerinfo.geo
+00011a50: 6d65 7472 7963 6f6c 756d 6e7d 2929 2f32  metrycolumn}))/2
+00011a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a70: 2029 2a7b 746f 5f67 656f 6772 6170 6869   )*{to_geographi
+00011a80: 635f 6661 6374 6f72 5f61 7070 726f 787d  c_factor_approx}
+00011a90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011aa0: 2020 2828 4d62 724d 696e 5928 7b6c 6179    ((MbrMinY({lay
+00011ab0: 6572 696e 666f 2e67 656f 6d65 7472 7963  erinfo.geometryc
+00011ac0: 6f6c 756d 6e7d 290a 2020 2020 2020 2020  olumn}).        
+00011ad0: 2020 2020 2020 2020 2020 2b4d 6272 4d61            +MbrMa
+00011ae0: 7859 287b 6c61 7965 7269 6e66 6f2e 6765  xY({layerinfo.ge
+00011af0: 6f6d 6574 7279 636f 6c75 6d6e 7d29 292f  ometrycolumn}))/
+00011b00: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+00011b10: 2020 292a 7b74 6f5f 6765 6f67 7261 7068    )*{to_geograph
+00011b20: 6963 5f66 6163 746f 725f 6170 7072 6f78  ic_factor_approx
+00011b30: 7d2c 2034 3332 3629 2c20 3130 2922 2222  }, 4326), 10)"""
+00011b40: 0a0a 2020 2020 2320 4e6f 7720 7765 2063  ..    # Now we c
+00011b50: 616e 2061 6374 7561 6c6c 7920 6164 6420  an actually add 
+00011b60: 7468 6520 636f 6c75 6d6e 2e0a 2020 2020  the column..    
+00011b70: 6766 6f2e 6164 645f 636f 6c75 6d6e 2870  gfo.add_column(p
+00011b80: 6174 683d 7061 7468 2c20 6e61 6d65 3d6e  ath=path, name=n
+00011b90: 616d 652c 2074 7970 653d 6766 6f2e 4461  ame, type=gfo.Da
+00011ba0: 7461 5479 7065 2e54 4558 542c 2065 7870  taType.TEXT, exp
+00011bb0: 7265 7373 696f 6e3d 6578 7072 6573 7369  ression=expressi
+00011bc0: 6f6e 290a 2020 2020 7371 6c69 7465 5f73  on).    sqlite_s
+00011bd0: 746d 7420 3d20 6627 4352 4541 5445 2049  tmt = f'CREATE I
+00011be0: 4e44 4558 207b 6e61 6d65 7d5f 6964 7820  NDEX {name}_idx 
+00011bf0: 4f4e 2022 7b6c 6179 6572 7d22 287b 6e61  ON "{layer}"({na
+00011c00: 6d65 7d29 270a 2020 2020 6766 6f2e 6578  me})'.    gfo.ex
+00011c10: 6563 7574 655f 7371 6c28 7061 7468 3d70  ecute_sql(path=p
+00011c20: 6174 682c 2073 716c 5f73 746d 743d 7371  ath, sql_stmt=sq
+00011c30: 6c69 7465 5f73 746d 7429 0a              lite_stmt).
```

### Comparing `geofileops-0.8.0a4/geofileops/util/_geoops_ogr.py` & `geofileops-0.8.0a5/geofileops/util/_geoops_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/_geoops_sql.py` & `geofileops-0.8.0a5/geofileops/util/_geoops_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import logging.config
 import math
 import multiprocessing
 from pathlib import Path
 import shutil
 import string
 from typing import Iterable, List, Literal, Optional, Union
+import warnings
 
 import pandas as pd
 
 import geofileops as gfo
 from geofileops import GeofileType, GeometryType, PrimitiveType
 from geofileops import fileops
 from geofileops.fileops import _append_to_nolock
@@ -44,41 +45,38 @@
     output_path: Path,
     distance: float,
     quadrantsegments: int = 5,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Init + prepare sql template for this operation
     # ----------------------------------------------
+    operation = f"ST_Buffer({{geometrycolumn}}, {distance}, {quadrantsegments})"
+
+    # For a double sided buffer, a negative buffer is only relevant for polygon types,
+    # so only keep polygon results.
+    # Negative buffer creates invalid stuff, so use collectionextract to keep only
+    # polygons.
     if distance < 0:
-        # For a double sided buffer, a negative buffer is only relevant for polygon
-        # types, so only keep polygon results. Negative buffer creates invalid stuff,
-        # so use collectionextract to keep only polygons.
-        sql_template = f"""
-            SELECT ST_CollectionExtract(
-                       ST_buffer({{geometrycolumn}}, {distance}, {quadrantsegments}), 3
-                   ) AS geom
-                  {{columns_to_select_str}}
-              FROM "{{input_layer}}" layer
-             WHERE 1=1
-               {{batch_filter}}
-        """
-    else:
-        sql_template = f"""
-            SELECT ST_Buffer({{geometrycolumn}}, {distance}, {quadrantsegments}) AS geom
-                  {{columns_to_select_str}}
-              FROM "{{input_layer}}" layer
-             WHERE 1=1
-               {{batch_filter}}
-        """
+        operation = f"ST_CollectionExtract({operation}, 3)"
+
+    # Create the final template
+    sql_template = f"""
+        SELECT {operation} AS geom
+              {{columns_to_select_str}}
+            FROM "{{input_layer}}" layer
+            WHERE 1=1
+              {{batch_filter}}
+    """
 
     # Buffer operation always results in polygons...
     if explodecollections:
         force_output_geometrytype = GeometryType.POLYGON
     else:
         force_output_geometrytype = GeometryType.MULTIPOLYGON
 
@@ -90,14 +88,15 @@
         sql_template=sql_template,
         operation_name="buffer",
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         sql_dialect="SQLITE",
         filter_null_geoms=True,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
@@ -105,14 +104,15 @@
 def convexhull(
     input_path: Path,
     output_path: Path,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Init + prepare sql template for this operation
     # ----------------------------------------------
     input_layerinfo = gfo.get_layerinfo(input_path, input_layer)
@@ -133,14 +133,15 @@
         sql_template=sql_template,
         operation_name="convexhull",
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=input_layerinfo.geometrytype,
+        gridsize=gridsize,
         sql_dialect="SQLITE",
         filter_null_geoms=True,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
@@ -148,14 +149,15 @@
 def delete_duplicate_geometries(
     input_path: Path,
     output_path: Path,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     force: bool = False,
 ):
     # The query as written doesn't give correct results when parallellized,
     # but it isn't useful to do it for this operation.
     sql_template = """
         SELECT {geometrycolumn} AS geom
               {columns_to_select_str}
@@ -175,14 +177,15 @@
         sql_template=sql_template,
         operation_name="delete_duplicate_geometries",
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=input_layer_info.geometrytype,
+        gridsize=gridsize,
         sql_dialect="SQLITE",
         filter_null_geoms=True,
         nb_parallel=1,
         batchsize=-1,
         force=force,
     )
 
@@ -216,14 +219,15 @@
         sql_template=sql_template,
         operation_name="isvalid",
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=GeometryType.POINT,
+        gridsize=0.0,
         sql_dialect="SQLITE",
         filter_null_geoms=True,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
@@ -261,15 +265,15 @@
     input_path: Path,
     output_path: Path,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
     force_output_geometrytype: Optional[GeometryType] = None,
-    gridsize: Optional[float] = None,
+    gridsize: float = 0.0,
     validate_attribute_data: bool = False,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # If output file exists already, either clean up or return...
     operation_name = "makevalid"
@@ -278,15 +282,15 @@
         return
 
     # Init + prepare sql template for this operation
     # ----------------------------------------------
     operation = "{geometrycolumn}"
 
     # If the precision needs to be reduced, snap to grid
-    if gridsize is not None:
+    if gridsize != 0.0:
         operation = f"ST_SnapToGrid({operation}, {gridsize})"
 
     # Prepare sql template for this operation
     operation = f"ST_MakeValid({operation})"
 
     # Determine output_geometrytype if it wasn't specified. Otherwise makevalid results
     # in column type 'GEOMETRY'/'UNKNOWN(ANY)'
@@ -314,14 +318,15 @@
         sql_template=sql_template,
         operation_name=operation_name,
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=0.0,
         sql_dialect="SQLITE",
         filter_null_geoms=True,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
@@ -338,14 +343,15 @@
     sql_stmt: str,
     sql_dialect: Optional[Literal["SQLITE", "OGRSQL"]] = "SQLITE",
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
     force_output_geometrytype: Optional[GeometryType] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = 1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Check if output exists already here, to evade to much logging to be written
     if output_path.exists():
         if force is False:
@@ -370,14 +376,15 @@
         sql_template=sql_stmt,
         operation_name="select",
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         sql_dialect=sql_dialect,
         filter_null_geoms=False,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
@@ -386,14 +393,15 @@
     input_path: Path,
     output_path: Path,
     tolerance: float,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Init + prepare sql template for this operation
     # ----------------------------------------------
     sql_template = f"""
@@ -412,14 +420,15 @@
         sql_template=sql_template,
         operation_name="simplify",
         input_layer=input_layer,
         output_layer=output_layer,
         columns=columns,
         explodecollections=explodecollections,
         force_output_geometrytype=input_layer_info.geometrytype,
+        gridsize=gridsize,
         sql_dialect="SQLITE",
         filter_null_geoms=True,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
@@ -430,14 +439,15 @@
     sql_template: str,
     operation_name: str,
     input_layer: Optional[str],
     output_layer: Optional[str],
     columns: Optional[List[str]],
     explodecollections: bool,
     force_output_geometrytype: Optional[GeometryType],
+    gridsize: float,
     sql_dialect: Optional[Literal["SQLITE", "OGRSQL"]],
     filter_null_geoms: bool,
     nb_parallel: int,
     batchsize: int,
     force: bool,
 ):
     # Init
@@ -459,33 +469,37 @@
     if output_path.exists():
         if force is False:
             logger.info(f"Stop {operation_name}: output exists already {output_path}")
             return
         else:
             gfo.remove(output_path)
 
-    # Get layer info of the input layer
-    input_layerinfo = gfo.get_layerinfo(input_path, input_layer)
-
     # Calculate
     tempdir = _io_util.create_tempdir(f"geofileops/{operation_name.replace(' ', '_')}")
     try:
+        # If gridsize != 0.0 we need an sqlite file to be able to determine the columns
+        # later on.
+        convert_to_spatialite_based = False if gridsize == 0.0 else True
         processing_params = _prepare_processing_params(
             input1_path=input_path,
             input1_layer=input_layer,
             input1_layer_alias="layer",
             tempdir=tempdir,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
-            convert_to_spatialite_based=False,
+            convert_to_spatialite_based=convert_to_spatialite_based,
         )
         # If None is returned, just stop.
         if processing_params is None or processing_params.batches is None:
             return
 
+        # Get layer info of the input layer to use
+        assert processing_params.input1_path is not None
+        input_layerinfo = gfo.get_layerinfo(processing_params.input1_path, input_layer)
+
         # If multiple batches, there should be a batch_filter placeholder sql_template
         nb_batches = len(processing_params.batches)
         if nb_batches > 1:
             placeholders = [
                 name for _, name, _, _ in string.Formatter().parse(sql_template) if name
             ]
             if "batch_filter" not in placeholders:
@@ -497,14 +511,63 @@
         # Format column string for use in select
         column_formatter = _ogr_sql_util.ColumnFormatter(
             columns_asked=columns,
             columns_in_layer=input_layerinfo.columns,
             fid_column=input_layerinfo.fid_column,
         )
 
+        # Fill out/add to the sql_template what is already possible
+        # ---------------------------------------------------------
+        sql_template = sql_template.format(
+            geometrycolumn=input_layerinfo.geometrycolumn,
+            columns_to_select_str=column_formatter.prefixed_aliased(),
+            input_layer=processing_params.input1_layer,
+            batch_filter="{batch_filter}",
+        )
+
+        # Add snaptogrid around sql_template if gridsize specified
+        if gridsize != 0.0:
+            # Apply snaptogrid, but this results in invalid geometries, so also
+            # ST_Makevalid. It can also result in collapsed (pieces of)
+            # geometries, so also collectionextract.
+            gridsize_op = f"ST_MakeValid(SnapToGrid(sub_gridsize.geom, {gridsize}))"
+            if force_output_geometrytype is None:
+                warnings.warn(
+                    "a gridsize is specified but no force_output_geometrytype, this "
+                    "can result in inconsistent geometries in the output"
+                )
+            else:
+                primitivetypeid = force_output_geometrytype.to_primitivetype.value
+                gridsize_op = f"ST_CollectionExtract({gridsize_op}, {primitivetypeid})"
+
+            # Get all columns of the sql_template
+            sql_tmp = sql_template.format(batch_filter="")
+            cols = _sqlite_util.get_columns(
+                sql_stmt=sql_tmp,
+                input1_path=processing_params.input1_path,  # type: ignore
+            )
+            cols = [col for col in cols if col.lower() != "geom"]
+            columns_to_select = _ogr_sql_util.columns_quoted(cols)
+            sql_template = f"""
+                SELECT {gridsize_op} AS geom
+                      {columns_to_select}
+                  FROM ( {sql_template}
+                    ) sub_gridsize
+            """
+
+        # Add where filter around sql_template if relevant
+        if filter_null_geoms:
+            where = "sub_where.geom IS NOT NULL"
+            sql_template = f"""
+                SELECT sub_where.* FROM
+                    ( {sql_template}
+                    ) sub_where
+                    WHERE {where}
+            """
+
         # Prepare temp output filename
         tmp_output_path = tempdir / output_path.name
 
         # Processing in threads is 2x faster for small datasets (on Windows)
         calculate_in_threads = True if input_layerinfo.featurecount <= 100 else False
         with _processing_util.PooledExecutorFactory(
             threadpool=calculate_in_threads,
@@ -518,31 +581,18 @@
                 batches[batch_id]["layer"] = output_layer
 
                 tmp_partial_output_path = (
                     tempdir / f"{output_path.stem}_{batch_id}{output_path.suffix}"
                 )
                 batches[batch_id]["tmp_partial_output_path"] = tmp_partial_output_path
 
-                # Now we have everything to format sql statement
+                # Fill out sql_template
                 sql_stmt = sql_template.format(
-                    geometrycolumn=input_layerinfo.geometrycolumn,
-                    columns_to_select_str=column_formatter.prefixed_aliased(),
-                    input_layer=processing_params.batches[batch_id]["layer"],
-                    batch_filter=processing_params.batches[batch_id]["batch_filter"],
+                    batch_filter=processing_params.batches[batch_id]["batch_filter"]
                 )
-
-                # Make sure no NULL geoms are outputted...
-                if filter_null_geoms is True:
-                    sql_stmt = f"""
-                        SELECT sub.* FROM
-                          ( {sql_stmt}
-                          ) sub
-                         WHERE sub.geom IS NOT NULL
-                    """
-
                 batches[batch_id]["sql_stmt"] = sql_stmt
 
                 # If there is only one batch, it is faster to create the spatial index
                 # immediately. Otherwise no index needed, because partial files still
                 # need to be merged to one file later on.
                 create_spatial_index = False
                 if nb_batches == 1:
@@ -641,14 +691,15 @@
     clip_path: Path,
     output_path: Path,
     input_layer: Optional[str] = None,
     input_columns: Optional[List[str]] = None,
     clip_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
     input_columns_prefix: str = "",
     output_with_spatial_index: bool = True,
 ):
     # Init
@@ -722,14 +773,15 @@
         input1_columns=input_columns,
         input1_columns_prefix=input_columns_prefix,
         input2_layer=clip_layer,
         input2_columns=None,
         input2_columns_prefix="",
         output_layer=output_layer,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         force_output_geometrytype=force_output_geometrytype,
         output_with_spatial_index=output_with_spatial_index,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
@@ -739,14 +791,15 @@
     erase_path: Path,
     output_path: Path,
     input_layer: Optional[str] = None,
     input_columns: Optional[List[str]] = None,
     erase_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
     input_columns_prefix: str = "",
     output_with_spatial_index: bool = True,
 ):
     # Init
@@ -824,14 +877,15 @@
         input1_columns_prefix=input_columns_prefix,
         input2_layer=erase_layer,
         input2_columns=[],
         input2_columns_prefix="",
         output_layer=output_layer,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
         output_with_spatial_index=output_with_spatial_index,
     )
 
 
@@ -841,14 +895,15 @@
     output_path: Path,
     min_area_intersect: Optional[float] = None,
     area_inters_column_name: Optional[str] = "area_inters",
     input_layer: Optional[str] = None,
     input_columns: Optional[List[str]] = None,
     input_to_compare_with_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Prepare sql template for this operation
     # TODO: test performance difference between the following two queries
     input1_layer_rtree = "rtree_{input1_layer}_{input1_geometrycolumn}"
@@ -934,14 +989,15 @@
         input1_columns_prefix="",
         input2_layer=input_to_compare_with_layer,
         input2_columns=[],
         input2_columns_prefix="",
         output_layer=output_layer,
         explodecollections=False,
         force_output_geometrytype=input_layer_info.geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def export_by_distance(
@@ -949,14 +1005,15 @@
     input_to_compare_with_path: Path,
     output_path: Path,
     max_distance: float,
     input1_layer: Optional[str] = None,
     input1_columns: Optional[List[str]] = None,
     input2_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Prepare sql template for this operation
     input1_layer_rtree = "rtree_{input1_layer}_{input1_geometrycolumn}"
     input2_layer_rtree = "rtree_{input2_layer}_{input2_geometrycolumn}"
@@ -996,14 +1053,15 @@
         input1_columns_prefix="",
         input2_layer=input2_layer,
         input2_columns=[],
         input2_columns_prefix="",
         output_layer=output_layer,
         explodecollections=False,
         force_output_geometrytype=input_layer_info.geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def intersection(
@@ -1014,14 +1072,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # In the query, important to only extract the geometry types that are expected
     # TODO: test for geometrycollection, line, point,...
     input1_layer_info = gfo.get_layerinfo(input1_path, input1_layer)
@@ -1086,14 +1145,15 @@
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def join_by_location(
@@ -1108,14 +1168,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Prepare sql template for this operation
     # Prepare intersection area columns/filter
     area_inters_column_expression = ""
@@ -1228,14 +1289,15 @@
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
         force_output_geometrytype=input1_layer_info.geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def _prepare_spatial_relations_filter(query: str) -> str:
@@ -1311,14 +1373,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Init some things...
     # Because there is preprocessing done in this function, check output path
     # here already
@@ -1394,14 +1457,15 @@
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_tmp_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         force_output_geometrytype=input1_layer_info.geometrytype,
         explodecollections=explodecollections,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
         use_ogr=True,
     )
 
 
@@ -1415,14 +1479,15 @@
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     force_output_geometrytype: Optional[GeometryType] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = 1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # Go!
     return _two_layer_vector_operation(
         input1_path=input1_path,
@@ -1435,14 +1500,15 @@
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
     )
 
 
 def split(
@@ -1453,14 +1519,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = 1,
     batchsize: int = -1,
     force: bool = False,
     output_with_spatial_index: bool = True,
 ):
     # In the query, important to only extract the geometry types that are
     # expected, so the primitive type of input1_layer
@@ -1555,14 +1622,15 @@
         input1_columns_prefix=input1_columns_prefix,
         input2_layer=input2_layer,
         input2_columns=input2_columns,
         input2_columns_prefix=input2_columns_prefix,
         output_layer=output_layer,
         explodecollections=explodecollections,
         force_output_geometrytype=force_output_geometrytype,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
         force=force,
         output_with_spatial_index=output_with_spatial_index,
     )
 
 
@@ -1574,14 +1642,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # A symmetric difference can be simulated by doing an "erase" of input1
     # and input2 and then append the result of an erase of input2 with
     # input1...
@@ -1603,14 +1672,15 @@
             output_path=erase1_output_path,
             input_layer=input1_layer,
             input_columns=input1_columns,
             input_columns_prefix=input1_columns_prefix,
             erase_layer=input2_layer,
             output_layer=output_layer,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
             output_with_spatial_index=False,
         )
 
         if input2_columns is None or len(input2_columns) > 0:
@@ -1633,14 +1703,15 @@
             output_path=erase2_output_path,
             input_layer=input2_layer,
             input_columns=input2_columns,
             input_columns_prefix=input2_columns_prefix,
             erase_layer=input1_layer,
             output_layer=output_layer,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
             output_with_spatial_index=False,
         )
 
         # Now append
@@ -1678,14 +1749,15 @@
     input1_columns: Optional[List[str]] = None,
     input1_columns_prefix: str = "l1_",
     input2_layer: Optional[str] = None,
     input2_columns: Optional[List[str]] = None,
     input2_columns_prefix: str = "l2_",
     output_layer: Optional[str] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
 ):
     # A union can be simulated by doing a "split" of input1 and input2 and
     # then append the result of an erase of input2 with input1...
 
@@ -1709,14 +1781,15 @@
             input1_columns=input1_columns,
             input1_columns_prefix=input1_columns_prefix,
             input2_layer=input2_layer,
             input2_columns=input2_columns,
             input2_columns_prefix=input2_columns_prefix,
             output_layer=output_layer,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
             output_with_spatial_index=False,
         )
 
         # Now erase input1 from input2 to another temporary output gfo...
@@ -1727,14 +1800,15 @@
             output_path=erase_output_path,
             input_layer=input2_layer,
             input_columns=input2_columns,
             input_columns_prefix=input2_columns_prefix,
             erase_layer=input1_layer,
             output_layer=output_layer,
             explodecollections=explodecollections,
+            gridsize=gridsize,
             nb_parallel=nb_parallel,
             batchsize=batchsize,
             force=force,
             output_with_spatial_index=False,
         )
 
         # Now append
@@ -1777,14 +1851,15 @@
     input1_columns_prefix: str,
     input2_layer: Optional[str],
     input2_columns: Optional[List[str]],
     input2_columns_prefix: str,
     output_layer: Optional[str],
     explodecollections: bool,
     force_output_geometrytype: Optional[GeometryType],
+    gridsize: float,
     nb_parallel: int,
     batchsize: int,
     force: bool,
     use_ogr: bool = False,
     output_with_spatial_index: bool = True,
 ):
     """
@@ -1800,24 +1875,27 @@
         input2_layer (str, optional): [description]. Defaults to None.
         input2_columns
         input2_columns_prefix
         output_layer (str, optional): [description]. Defaults to None.
         explodecollections (bool, optional): Explode collecions in output.
             Defaults to False.
         force_output_geometrytype (GeometryType, optional): Defaults to None.
-        use_ogr (bool, optional): If True, ogr is used to do the processing,
-            In this case different input files (input1_path, input2_path) are
-            NOT supported. If False, sqlite3 is used directly.
-            Defaults to False.
+        gridsize (float, optional): the size of the grid the coordinates of the ouput
+            will be rounded to. Eg. 0.001 to keep 3 decimals. Value 0.0 doesn't change
+            the precision. Defaults to 0.0.
         nb_parallel (int, optional): [description]. Defaults to -1.
         batchsize (int, optional): indicative number of rows to process per
             batch. A smaller batch size, possibly in combination with a
             smaller nb_parallel, will reduce the memory usage.
             Defaults to -1: (try to) determine optimal size automatically.
         force (bool, optional): [description]. Defaults to False.
+        use_ogr (bool, optional): If True, ogr is used to do the processing,
+            In this case different input files (input1_path, input2_path) are
+            NOT supported. If False, sqlite3 is used directly.
+            Defaults to False.
         output_with_spatial_index (bool, optional): True to create output file with
             spatial index. Defaults to True.
 
     Raises:
         ValueError: [description]
     """
     # Init
@@ -1860,14 +1938,15 @@
     # Prepare output filename
     tmp_output_path = tempdir / output_path.name
     tmp_output_path.parent.mkdir(exist_ok=True, parents=True)
     gfo.remove(tmp_output_path)
 
     try:
         # Prepare tmp files/batches
+        # -------------------------
         logger.info(
             f"Prepare input (params) for {operation_name} with tempdir: {tempdir}"
         )
         processing_params = _prepare_processing_params(
             input1_path=input1_path,
             input1_layer=input1_layer,
             input1_layer_alias="layer1",
@@ -1890,14 +1969,15 @@
             if "batch_filter" not in placeholders:
                 raise ValueError(
                     "Number batches > 1 requires a batch_filter placeholder in "
                     f"sql_template {sql_template}"
                 )
 
         # Prepare column names,... to format the select
+        # ---------------------------------------------
         # Format column strings for use in select
         assert processing_params.input1_path is not None
         input1_tmp_layerinfo = gfo.get_layerinfo(
             processing_params.input1_path, processing_params.input1_layer
         )
         input1_col_strs = _ogr_sql_util.ColumnFormatter(
             columns_asked=input1_columns,
@@ -1921,15 +2001,73 @@
         # Check input crs'es
         if input1_tmp_layerinfo.crs != input2_tmp_layerinfo.crs:
             logger.warning(
                 "input1 has a different crs than input2: \n\tinput1: "
                 f"{input1_tmp_layerinfo.crs} \n\tinput2: {input2_tmp_layerinfo.crs}"
             )
 
+        # Fill out sql_template as much as possible already
+        # -------------------------------------------------
+        # Keep input1_tmp_layer and input2_tmp_layer for backwards compatibility
+        sql_template = sql_template.format(
+            input1_databasename="{input1_databasename}",
+            input2_databasename="{input2_databasename}",
+            layer1_columns_from_subselect_str=input1_col_strs.from_subselect(),
+            layer1_columns_prefix_alias_str=input1_col_strs.prefixed_aliased(),
+            layer1_columns_prefix_str=input1_col_strs.prefixed(),
+            input1_layer=processing_params.input1_layer,
+            input1_tmp_layer=processing_params.input1_layer,
+            input1_geometrycolumn=input1_tmp_layerinfo.geometrycolumn,
+            layer2_columns_from_subselect_str=input2_col_strs.from_subselect(),
+            layer2_columns_prefix_alias_str=input2_col_strs.prefixed_aliased(),
+            layer2_columns_prefix_str=input2_col_strs.prefixed(),
+            layer2_columns_prefix_alias_null_str=input2_col_strs.null_aliased(),
+            input2_layer=processing_params.input2_layer,
+            input2_tmp_layer=processing_params.input2_layer,
+            input2_geometrycolumn=input2_tmp_layerinfo.geometrycolumn,
+            batch_filter="{batch_filter}",
+        )
+
+        # Add snaptogrid around sql_template if gridsize specified
+        if gridsize != 0.0:
+            # Apply snaptogrid, but this results in invalid geometries, so also
+            # ST_Makevalid. It can also result in collapsed (pieces of)
+            # geometries, so also collectionextract.
+            gridsize_op = f"ST_MakeValid(SnapToGrid(sub_gridsize.geom, {gridsize}))"
+            if force_output_geometrytype is None:
+                warnings.warn(
+                    "a gridsize is specified but no force_output_geometrytype, this "
+                    "can result in inconsistent geometries in the output"
+                )
+            else:
+                primitivetypeid = force_output_geometrytype.to_primitivetype.value
+                gridsize_op = f"ST_CollectionExtract({gridsize_op}, {primitivetypeid})"
+
+            # Get all columns of the sql_template
+            sql_tmp = sql_template.format(
+                input1_databasename="{input1_databasename}",
+                input2_databasename="{input2_databasename}",
+                batch_filter="",
+            )
+            cols = _sqlite_util.get_columns(
+                sql_stmt=sql_tmp,
+                input1_path=processing_params.input1_path,
+                input2_path=processing_params.input2_path,
+            )
+            cols = [col for col in cols if col.lower() != "geom"]
+            columns_to_select = _ogr_sql_util.columns_quoted(cols)
+            sql_template = f"""
+                SELECT {gridsize_op} AS geom
+                        {columns_to_select}
+                    FROM ( {sql_template}
+                    ) sub_gridsize
+            """
+
         # Calculate
+        # ---------
         # Processing in threads is 2x faster for small datasets (on Windows)
         calculate_in_threads = (
             True if input1_tmp_layerinfo.featurecount <= 100 else False
         )
         logger.info(
             f"Start {operation_name} ({processing_params.nb_parallel} parallel workers)"
         )
@@ -1946,35 +2084,20 @@
                 batches[batch_id]["layer"] = output_layer
 
                 tmp_partial_output_path = (
                     tempdir / f"{output_path.stem}_{batch_id}.gpkg"
                 )
                 batches[batch_id]["tmp_partial_output_path"] = tmp_partial_output_path
 
-                # Keep input1_tmp_layer and input2_tmp_layer for backwards
-                # compatibility
+                # Fill out final things in sql_template
                 sql_stmt = sql_template.format(
                     input1_databasename="{input1_databasename}",
                     input2_databasename="{input2_databasename}",
-                    layer1_columns_from_subselect_str=input1_col_strs.from_subselect(),
-                    layer1_columns_prefix_alias_str=input1_col_strs.prefixed_aliased(),
-                    layer1_columns_prefix_str=input1_col_strs.prefixed(),
-                    input1_layer=processing_params.batches[batch_id]["layer"],
-                    input1_tmp_layer=processing_params.batches[batch_id]["layer"],
-                    input1_geometrycolumn=input1_tmp_layerinfo.geometrycolumn,
-                    layer2_columns_from_subselect_str=input2_col_strs.from_subselect(),
-                    layer2_columns_prefix_alias_str=input2_col_strs.prefixed_aliased(),
-                    layer2_columns_prefix_str=input2_col_strs.prefixed(),
-                    layer2_columns_prefix_alias_null_str=input2_col_strs.null_aliased(),
-                    input2_layer=processing_params.input2_layer,
-                    input2_tmp_layer=processing_params.input2_layer,
-                    input2_geometrycolumn=input2_tmp_layerinfo.geometrycolumn,
                     batch_filter=processing_params.batches[batch_id]["batch_filter"],
                 )
-
                 batches[batch_id]["sqlite_stmt"] = sql_stmt
 
                 # Remark: this temp file doesn't need spatial index
                 if use_ogr is False:
                     # Use an aggressive speedy sqlite profile
                     future = calculate_pool.submit(
                         _sqlite_util.create_table_as_sql,
@@ -2190,17 +2313,15 @@
 
     if convert_to_spatialite_based is False:
         returnvalue.input1_path = input1_path
         returnvalue.input2_path = input2_path
     else:
         # Check if the input files are of the correct geofiletype
         input1_geofiletype = GeofileType(input1_path)
-        input2_geofiletype = None
-        if input2_path is not None:
-            input2_geofiletype = GeofileType(input2_path)
+        input2_geofiletype = None if input2_path is None else GeofileType(input2_path)
 
         # If input files are of the same format + are spatialite compatible,
         # just use them
         if input1_geofiletype.is_spatialite_based and (
             input2_geofiletype is None or input1_geofiletype == input2_geofiletype
         ):
             returnvalue.input1_path = input1_path
@@ -2268,16 +2389,20 @@
             SELECT MIN(rowid) minmax_rowid FROM "{layer1_info.name}"
             UNION ALL
             SELECT MAX(rowid) minmax_rowid FROM "{layer1_info.name}"
         """
         batch_info_df = gfo.read_file(
             path=returnvalue.input1_path, sql_stmt=sql_stmt, sql_dialect="SQLITE"
         )
-        min_rowid = pd.to_numeric(batch_info_df["minmax_rowid"][0]).item()
-        max_rowid = pd.to_numeric(batch_info_df["minmax_rowid"][1]).item()
+        min_rowid = pd.to_numeric(
+            batch_info_df["minmax_rowid"][0]
+        ).item()  # type: ignore
+        max_rowid = pd.to_numeric(
+            batch_info_df["minmax_rowid"][1]
+        ).item()  # type: ignore
 
         # Determine the exact batches to use
         if ((max_rowid - min_rowid) / nb_rows_input_layer) < 1.1:
             # If the rowid's are quite consecutive, use an imperfect, but
             # fast distribution in batches
             batch_info_list = []
             nb_rows_per_batch = round(nb_rows_input_layer / nb_batches)
@@ -2352,14 +2477,15 @@
 
 def dissolve_singlethread(
     input_path: Path,
     output_path: Path,
     groupby_columns: Union[str, Iterable[str], None] = None,
     agg_columns: Optional[dict] = None,
     explodecollections: bool = False,
+    gridsize: float = 0.0,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     force: bool = False,
 ):
     """
     Remark: this is not a parallelized version!!!
     """
@@ -2511,14 +2637,29 @@
             force_output_geometrytype = GeometryType.LINESTRING
 
     # If there are no input features, the output geometry type needs to be specified
     # so gdal can create an empty output file with the right geometry type.
     if force_output_geometrytype is None and layerinfo.featurecount == 0:
         force_output_geometrytype = layerinfo.geometrytype
 
+    # Apply tolerance gridsize on result
+    if gridsize != 0.0:
+        # Apply snaptogrid, but this results in invalid geometries, so also
+        # ST_Makevalid. It can also result in collapsed (pieces of)
+        # geometries, so also collectionextract.
+        operation = f"ST_MakeValid(SnapToGrid({operation}, {gridsize}))"
+        if force_output_geometrytype is None:
+            warnings.warn(
+                "a gridsize is specified but no force_output_geometrytype, this "
+                "can result in inconsistent geometries in the output"
+            )
+        else:
+            primitivetypeid = force_output_geometrytype.to_primitivetype.value
+            operation = f"ST_CollectionExtract({operation}, {primitivetypeid})"
+
     sql_stmt = f"""
         SELECT {operation} AS geom
             {groupby_columns_for_select_str}
             {agg_columns_str}
         FROM "{input_layer}" layer
         GROUP BY {groupby_columns_for_groupby_str}
     """
```

### Comparing `geofileops-0.8.0a4/geofileops/util/_io_util.py` & `geofileops-0.8.0a5/geofileops/util/_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/_ogr_sql_util.py` & `geofileops-0.8.0a5/geofileops/util/_ogr_sql_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,7 +179,14 @@
     def from_subselect(self, subselect_alias: str = "sub"):
         if len(self._columns) == 0:
             return ""
 
         prefix = "" if subselect_alias == "" else f"{subselect_alias}."
         columns_from_subselect = [f'{prefix}"{alias}"' for alias in self._aliases()]
         return f",{', '.join(columns_from_subselect)}"
+
+
+def columns_quoted(columns: List[str]):
+    if len(columns) == 0:
+        return ""
+    columns_quoted = [f'"{column}"' for column in columns]
+    return f",{', '.join(columns_quoted)}"
```

### Comparing `geofileops-0.8.0a4/geofileops/util/_ogr_util.py` & `geofileops-0.8.0a5/geofileops/util/_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/_processing_util.py` & `geofileops-0.8.0a5/geofileops/util/_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/_sqlite_util.py` & `geofileops-0.8.0a5/geofileops/util/_sqlite_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,61 @@
 
     except Exception as ex:
         raise Exception(f"Error creating spatial db {path}") from ex
     finally:
         conn.close()
 
 
+def get_columns(
+    sql_stmt: str,
+    input1_path: Path,
+    input2_path: Optional[Path] = None,
+    use_spatialite: bool = True,
+) -> List[str]:
+    input1_databasename = "main"
+    conn = sqlite3.connect(str(input1_path), uri=True)
+    sql = None
+    try:
+        if use_spatialite is True:
+            load_spatialite(conn)
+            if input1_path.suffix.lower() == ".gpkg":
+                sql = "SELECT EnableGpkgMode();"
+                conn.execute(sql)
+
+        # If input2 isn't the same database input1, attach to it
+        input2_databasename = None
+        if input2_path is not None:
+            if input2_path == input1_path:
+                input2_databasename = input1_databasename
+            else:
+                input2_databasename = "input2"
+                sql = f"ATTACH DATABASE ? AS {input2_databasename}"
+                # dbSpec = (f"file:{input2_path.resolve().as_posix()}?mode=ro",)
+                dbSpec = (str(input2_path),)
+                conn.execute(sql, dbSpec)
+        # Prepare sql statement
+        sql = sql_stmt.format(
+            input1_databasename=input1_databasename,
+            input2_databasename=input2_databasename,
+        )
+
+        # Execute sql to be able to get the column names
+        cur = conn.cursor()
+        cur.execute(sql)
+        columns = [desc[0] for desc in cur.description]
+        conn.rollback()
+    except Exception as ex:
+        conn.rollback()
+        raise Exception(f"Error {ex} executing {sql}") from ex
+    finally:
+        conn.close()
+
+    return columns
+
+
 def create_table_as_sql(
     input1_path: Path,
     input1_layer: str,
     input2_path: Path,
     output_path: Path,
     sql_stmt: str,
     output_layer: str,
```

### Comparing `geofileops-0.8.0a4/geofileops/util/geodataframe_util.py` & `geofileops-0.8.0a5/geofileops/util/geodataframe_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/geofiletype.py` & `geofileops-0.8.0a5/geofileops/util/geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/geofiletypes.csv` & `geofileops-0.8.0a5/geofileops/util/geofiletypes.csv`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/geometry_util.py` & `geofileops-0.8.0a5/geofileops/util/geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/geoseries_util.py` & `geofileops-0.8.0a5/geofileops/util/geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/grid_util.py` & `geofileops-0.8.0a5/geofileops/util/grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops/util/test.gpkg` & `geofileops-0.8.0a5/geofileops/util/test.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/geofileops.egg-info/PKG-INFO` & `geofileops-0.8.0a5/geofileops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a4
+Version: 0.8.0a5
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a4/geofileops.egg-info/SOURCES.txt` & `geofileops-0.8.0a5/geofileops.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 benchmark/__init__.py
 benchmark/benchmark_all.py
 benchmark/benchmark_geofileops.py
 benchmark/benchmarker.py
 benchmark/reporter.py
```

### Comparing `geofileops-0.8.0a4/setup.py` & `geofileops-0.8.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/BEFL-kbl.gpkg` & `geofileops-0.8.0a5/tests/data/BEFL-kbl.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/geofileops_testdata.qgz` & `geofileops-0.8.0a5/tests/data/geofileops_testdata.qgz`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/linestring-row-trees.gpkg` & `geofileops-0.8.0a5/tests/data/linestring-row-trees.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/linestring-watercourse.gpkg` & `geofileops-0.8.0a5/tests/data/linestring-watercourse.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/linestrings_hedges.gpkg` & `geofileops-0.8.0a5/tests/data/linestrings_hedges.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/point.gpkg` & `geofileops-0.8.0a5/tests/data/point.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-invalid.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-invalid.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-no-rows.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-no-rows.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-all.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-overlappingcircles-all.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-one.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-overlappingcircles-one.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-overlappingcircles-two+three.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-overlappingcircles-two+three.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-parcel.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-parcel.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-simplify-onborder-testcase.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-simplify-onborder-testcase.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-twolayers.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-twolayers.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygon-zone.gpkg` & `geofileops-0.8.0a5/tests/data/polygon-zone.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygonstyle.qml` & `geofileops-0.8.0a5/tests/data/polygonstyle.qml`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/data/polygonstyle.sld` & `geofileops-0.8.0a5/tests/data/polygonstyle.sld`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_general_util.py` & `geofileops-0.8.0a5/tests/test_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_geofile.py` & `geofileops-0.8.0a5/tests/test_geofile.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_geofileops_singlelayer.py` & `geofileops-0.8.0a5/tests/test_geofileops_singlelayer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 """
 Tests for operations that are executed using a sql statement on one layer.
 """
 
 from importlib import import_module
 import logging
 import math
-from pathlib import Path
-import sys
 from typing import List
 
+import geopandas._compat as gpd_compat
 import pytest
 
-# Add path so the local geofileops packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+if gpd_compat.USE_PYGEOS:
+    import pygeos as shapely2_or_pygeos
+else:
+    import shapely as shapely2_or_pygeos
+
 from geofileops import geoops
 from geofileops import fileops
 from geofileops import GeometryType
 from geofileops.util import _io_util
 from tests import test_helper as test_helper
 from tests.test_helper import DEFAULT_EPSGS, DEFAULT_SUFFIXES, DEFAULT_TESTFILES
 from tests.test_helper import assert_geodataframe_equal
@@ -39,49 +41,62 @@
         print(f"gfo module switched to: {current_fileops_module}")
 
 
 def get_combinations_to_test(
     fileops_modules: List[str],
     testfiles: List[str] = ["polygon-parcel", "point", "linestring-row-trees"],
 ) -> list:
+    """
+    Return sensible combinations of parameters to be used in tests for following params:
+        suffix, epsg, fileops_module, testfile, empty_input, gridsize
+    """
     result = []
 
     # On .gpkg test:
     #   - all combinations of fileops_modules, testfiles and epsgs
     #   - fixed empty_input, suffix
     for epsg in DEFAULT_EPSGS:
         for fileops_module in fileops_modules:
             for testfile in testfiles:
-                result.append((".gpkg", epsg, fileops_module, testfile, False))
+                gridsize = 0.001 if epsg == 31370 else 0.0
+                result.append(
+                    (".gpkg", epsg, fileops_module, testfile, False, gridsize)
+                )
 
     # On other suffixes test:
     #   - all combinations of fileops_modules, testfiles
     #   - fixed epsg and empty_input
     other_suffixes = list(DEFAULT_SUFFIXES)
     other_suffixes.remove(".gpkg")
     for suffix in other_suffixes:
         for fileops_module in fileops_modules:
             for testfile in testfiles:
-                result.append((".shp", 31370, fileops_module, testfile, False))
+                gridsize = 0.001 if testfile == "polygon-parcel" else 0.0
+                result.append((suffix, 31370, fileops_module, testfile, False, 0.0))
 
     # Test empty_input=True on
     #   - all combinations of fileops_modules and DEFAULT_SUFFIXES
     #   - fixed epsg, testfile and empty_input
     for fileops_module in fileops_modules:
         for suffix in DEFAULT_SUFFIXES:
-            result.append((suffix, 31370, fileops_module, "polygon-parcel", True))
+            gridsize = 0.001 if suffix == ".gpkg" else 0.0
+            result.append(
+                (suffix, 31370, fileops_module, "polygon-parcel", True, gridsize)
+            )
 
     return result
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg, fileops_module, testfile, empty_input",
+    "suffix, epsg, fileops_module, testfile, empty_input, gridsize",
     get_combinations_to_test(["geofileops.geoops", "geofileops.util._geoops_gpd"]),
 )
-def test_buffer(tmp_path, suffix, epsg, fileops_module, testfile, empty_input):
+def test_buffer(
+    tmp_path, suffix, epsg, fileops_module, testfile, empty_input, gridsize
+):
     """Buffer basics are available both in the gpd and sql implementations."""
     # Prepare test data
     input_path = test_helper.get_testfile(
         testfile, suffix=suffix, epsg=epsg, empty=empty_input
     )
 
     # Now run test
@@ -96,14 +111,15 @@
         distance /= 111000
 
     # Test positive buffer
     geoops.buffer(
         input_path=input_path,
         output_path=output_path,
         distance=distance,
+        gridsize=gridsize,
         nb_parallel=2,
         batchsize=batchsize,
     )
 
     # Now check if the output file is correctly created
     assert output_path.exists()
     assert fileops.has_spatial_index(output_path)
@@ -116,14 +132,18 @@
         expected_gdf = fileops.read_file(input_path)
         expected_gdf.geometry = expected_gdf.geometry.buffer(
             distance=distance, resolution=5
         )
         check_less_precise = (
             True if input_layerinfo.crs.is_projected is False else False
         )
+        if gridsize != 0.0:
+            expected_gdf.geometry = shapely2_or_pygeos.set_precision(
+                expected_gdf.geometry.array.data, grid_size=gridsize
+            )
         assert_geodataframe_equal(
             output_gdf,
             expected_gdf,
             promote_to_multi=True,
             check_less_precise=check_less_precise,
             sort_values=True,
         )
@@ -371,16 +391,16 @@
     )
 
 
 @pytest.mark.parametrize(
     "fileops_module", ["geofileops.geoops", "geofileops.util._geoops_gpd"]
 )
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
-@pytest.mark.parametrize("empty_input", [True, False])
-def test_convexhull(tmp_path, fileops_module, suffix, empty_input):
+@pytest.mark.parametrize("empty_input, gridsize", [(True, 0.0), (False, 0.001)])
+def test_convexhull(tmp_path, fileops_module, suffix, empty_input, gridsize):
     logging.basicConfig(level=logging.DEBUG)
     input_path = test_helper.get_testfile(
         "polygon-parcel", suffix=suffix, empty=empty_input
     )
     output_path = tmp_path / f"{input_path.stem}-output{suffix}"
     set_geoops_module(fileops_module)
     input_layerinfo = fileops.get_layerinfo(input_path)
@@ -388,14 +408,15 @@
 
     # Also check if columns parameter works (case insensitive)
     columns = ["OIDN", "uidn", "HFDTLT", "lblhfdtlt", "GEWASGROEP", "lengte", "OPPERVL"]
     geoops.convexhull(
         input_path=input_path,
         columns=columns,
         output_path=output_path,
+        gridsize=gridsize,
         nb_parallel=2,
         batchsize=batchsize,
     )
 
     # Now check if the output file is correctly created
     assert output_path.exists()
     assert fileops.has_spatial_index(output_path)
@@ -409,25 +430,31 @@
         assert input_layerinfo.featurecount == layerinfo_output.featurecount
 
         # Read result for some more detailed checks
         output_gdf = fileops.read_file(output_path)
         assert output_gdf["geometry"][0] is not None
         expected_gdf = fileops.read_file(input_path, columns=columns)
         expected_gdf.geometry = expected_gdf.geometry.convex_hull
+        if gridsize != 0.0:
+            expected_gdf.geometry = shapely2_or_pygeos.set_precision(
+                expected_gdf.geometry.array.data, grid_size=gridsize
+            )
         assert_geodataframe_equal(output_gdf, expected_gdf, sort_values=True)
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg, fileops_module, testfile, empty_input",
+    "suffix, epsg, fileops_module, testfile, empty_input, gridsize",
     get_combinations_to_test(
         fileops_modules=["geofileops.geoops", "geofileops.util._geoops_gpd"],
         testfiles=["polygon-parcel", "linestring-row-trees"],
     ),
 )
-def test_simplify(tmp_path, suffix, epsg, fileops_module, testfile, empty_input):
+def test_simplify(
+    tmp_path, suffix, epsg, fileops_module, testfile, empty_input, gridsize
+):
     # Prepare test data
     tmp_dir = tmp_path / f"{fileops_module}_{epsg}"
     tmp_dir.mkdir(parents=True, exist_ok=True)
     input_path = test_helper.get_testfile(
         testfile, dst_dir=tmp_dir, suffix=suffix, epsg=epsg, empty=empty_input
     )
     output_path = tmp_dir / f"{input_path.stem}-output{suffix}"
@@ -443,14 +470,15 @@
 
     # Test default algorithm (rdp)
     output_path = _io_util.with_stem(input_path, output_path)
     geoops.simplify(
         input_path=input_path,
         output_path=output_path,
         tolerance=tolerance,
+        gridsize=gridsize,
         nb_parallel=2,
         batchsize=batchsize,
     )
 
     # Now check if the tmp file is correctly created
     assert output_path.exists()
     assert fileops.has_spatial_index(output_path)
@@ -459,8 +487,12 @@
 
     if not empty_input:
         output_gdf = fileops.read_file(output_path)
         expected_gdf = fileops.read_file(input_path)
         expected_gdf.geometry = expected_gdf.geometry.simplify(
             tolerance=tolerance, preserve_topology=True
         )
+        if gridsize != 0.0:
+            expected_gdf.geometry = shapely2_or_pygeos.set_precision(
+                expected_gdf.geometry.array.data, grid_size=gridsize
+            )
         assert_geodataframe_equal(output_gdf, expected_gdf, sort_values=True)
```

### Comparing `geofileops-0.8.0a4/tests/test_geofileops_singlelayer_gpd.py` & `geofileops-0.8.0a5/tests/test_geofileops_singlelayer_gpd.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 """
 Tests for operations using GeoPandas.
 """
 
 import json
 import math
 from pathlib import Path
-import sys
 
 import geopandas as gpd
+import geopandas._compat as gpd_compat
 import pytest
+
+if gpd_compat.USE_PYGEOS:
+    import pygeos as shapely2_or_pygeos
+else:
+    import shapely as shapely2_or_pygeos
 import shapely.geometry as sh_geom
 
-# Add path so the local geofileops packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
 import geofileops as gfo
 from geofileops import GeometryType
 from geofileops.util import _geoops_gpd, grid_util
 from geofileops.util import geometry_util
 from tests import test_helper
 from tests.test_helper import DEFAULT_EPSGS, DEFAULT_SUFFIXES
 
 
 def test_get_parallelization_params():
     parallelization_params = _geoops_gpd.get_parallelization_params(500000)
     assert parallelization_params is not None
 
 
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
-@pytest.mark.parametrize("only_geom_input", [True, False])
+@pytest.mark.parametrize("only_geom_input, gridsize", [(True, 0.0), (False, 0.001)])
 @pytest.mark.parametrize("force_output_geometrytype", [None, GeometryType.POLYGON])
-def test_apply(tmp_path, suffix, only_geom_input, force_output_geometrytype):
+def test_apply(tmp_path, suffix, only_geom_input, force_output_geometrytype, gridsize):
     # Prepare test data
     test_gdf = gpd.GeoDataFrame(
         geometry=[  # type: ignore
             test_helper.TestData.polygon_small_island,
             test_helper.TestData.polygon_with_island,
             None,
         ],
@@ -51,25 +54,27 @@
             input_path=input_path,
             output_path=output_path,
             func=lambda geom: geometry_util.remove_inner_rings(
                 geometry=geom, min_area_to_keep=2, crs=input_layerinfo.crs
             ),
             only_geom_input=True,
             force_output_geometrytype=force_output_geometrytype,
+            gridsize=gridsize,
             batchsize=batchsize,
         )
     else:
         gfo.apply(
             input_path=input_path,
             output_path=output_path,
             func=lambda row: geometry_util.remove_inner_rings(
                 row.geometry, min_area_to_keep=2, crs=input_layerinfo.crs
             ),
             only_geom_input=False,
             force_output_geometrytype=force_output_geometrytype,
+            gridsize=gridsize,
             batchsize=batchsize,
         )
 
     # Now check if the output file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     output_layerinfo = gfo.get_layerinfo(output_path)
@@ -160,85 +165,60 @@
     output_gdf = gfo.read_file(output_path)
     assert output_gdf["geometry"][0] is not None
     area_square_buffer = sum(output_gdf.area)
     assert area_square_buffer > area_default_buffer
 
 
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
-@pytest.mark.parametrize("epsg", DEFAULT_EPSGS)
-def test_dissolve_linestrings(tmp_path, suffix, epsg):
+@pytest.mark.parametrize(
+    "epsg, gridsize, explodecollections", [(31370, 0.001, True), (4326, 0.0, False)]
+)
+def test_dissolve_linestrings(tmp_path, suffix, epsg, gridsize, explodecollections):
     # Prepare test data
     input_path = test_helper.get_testfile(
         "linestring-watercourse", suffix=suffix, epsg=epsg
     )
     output_basepath = tmp_path / f"{input_path.stem}-output{suffix}"
     input_layerinfo = gfo.get_layerinfo(input_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
 
-    # Dissolve, no groupby, explodecollections=True
-    # ---------------------------------------------
+    # Dissolve, no groupby
     output_path = (
         output_basepath.parent / f"{output_basepath.stem}_expl{output_basepath.suffix}"
     )
     gfo.dissolve(
         input_path=input_path,
         output_path=output_path,
-        explodecollections=True,
+        explodecollections=explodecollections,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
     # Check if the result file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     output_layerinfo = gfo.get_layerinfo(output_path)
-    assert output_layerinfo.featurecount == 83
+    if explodecollections:
+        assert output_layerinfo.featurecount == 83
+    else:
+        assert output_layerinfo.featurecount == 1
     assert output_layerinfo.geometrytype in [
         GeometryType.LINESTRING,
         GeometryType.MULTILINESTRING,
     ]
     assert len(output_layerinfo.columns) >= 0
 
     # Now check the contents of the result file
     input_gdf = gfo.read_file(input_path)
     output_gdf = gfo.read_file(output_path)
     assert input_gdf.crs == output_gdf.crs
     assert len(output_gdf) == output_layerinfo.featurecount
     assert output_gdf["geometry"][0] is not None
     # TODO: add more in depth check of result
 
-    # Dissolve, no groupby, explodecollections=False
-    # ----------------------------------------------
-    output_path = (
-        output_basepath.parent
-        / f"{output_basepath.stem}_noexpl{output_basepath.suffix}"
-    )
-    gfo.dissolve(
-        input_path=input_path,
-        output_path=output_path,
-        explodecollections=False,
-        batchsize=batchsize,
-    )
-
-    # Check if the result file is correctly created
-    assert output_path.exists()
-    input_layerinfo = gfo.get_layerinfo(input_path)
-
-    output_layerinfo = gfo.get_layerinfo(output_path)
-    assert output_layerinfo.featurecount == 1
-    assert output_layerinfo.geometrytype is input_layerinfo.geometrytype
-    assert len(output_layerinfo.columns) >= 0
-
-    # Now check the contents of the result file
-    input_gdf = gfo.read_file(input_path)
-    output_gdf = gfo.read_file(output_path)
-    assert input_gdf.crs == output_gdf.crs
-    assert len(output_gdf) == output_layerinfo.featurecount
-    assert output_gdf["geometry"][0] is not None
-    # TODO: add more in depth check of result
-
 
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
 @pytest.mark.parametrize("epsg", DEFAULT_EPSGS)
 def test_dissolve_linestrings_groupby(tmp_path, suffix, epsg):
     # Prepare test data
     input_path = test_helper.get_testfile(
         "linestring-watercourse", suffix=suffix, epsg=epsg
@@ -410,45 +390,45 @@
         assert len(json_value[0]) == len(input_layerinfo.columns) + 1
     else:
         # fid_orig is added to json
         assert len(json_value[0]) == len(agg_columns["json"]) + 1
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg, groupby_columns, explode, expected_featurecount",
+    "suffix, epsg, groupby_columns, explode, gridsize, expected_featurecount",
     [
-        (".gpkg", 31370, ["GEWASGROEP"], True, 25),
-        (".gpkg", 31370, ["GEWASGROEP"], False, 6),
-        (".gpkg", 31370, ["gewasGROEP"], False, 6),
-        (".gpkg", 31370, [], True, 23),
-        (".gpkg", 31370, None, False, 1),
-        (".gpkg", 4326, ["GEWASGROEP"], True, 25),
-        (".shp", 31370, ["GEWASGROEP"], True, 25),
-        (".shp", 31370, [], True, 23),
+        (".gpkg", 31370, ["GEWASGROEP"], True, 0.0, 25),
+        (".gpkg", 31370, ["GEWASGROEP"], False, 0.0, 6),
+        (".gpkg", 31370, ["gewasGROEP"], False, 0.01, 6),
+        (".gpkg", 31370, [], True, 0.0, 23),
+        (".gpkg", 31370, None, False, 0.0, 1),
+        (".gpkg", 4326, ["GEWASGROEP"], True, 0.0, 25),
+        (".shp", 31370, ["GEWASGROEP"], True, 0.0, 25),
+        (".shp", 31370, [], True, 0.0, 23),
     ],
 )
 def test_dissolve_polygons(
-    tmp_path, suffix, epsg, groupby_columns, explode, expected_featurecount
+    tmp_path, suffix, epsg, groupby_columns, explode, gridsize, expected_featurecount
 ):
     # Prepare test data
     input_path = test_helper.get_testfile("polygon-parcel", suffix=suffix, epsg=epsg)
     input_layerinfo = gfo.get_layerinfo(input_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
 
     # Test dissolve polygons with different options for groupby and explodecollections
     # --------------------------------------------------------------------------------
     groupby = True if (groupby_columns is None or len(groupby_columns) == 0) else False
-    output_path = (
-        tmp_path / f"{input_path.stem}_groupby-{groupby}_explode-{explode}{suffix}"
-    )
+    name = f"{input_path.stem}_groupby-{groupby}_explode-{explode}_gridsize-{gridsize}"
+    output_path = tmp_path / f"{name}{suffix}"
     gfo.dissolve(
         input_path=input_path,
         output_path=output_path,
         groupby_columns=groupby_columns,
         explodecollections=explode,
+        gridsize=gridsize,
         nb_parallel=2,
         batchsize=batchsize,
     )
 
     # Now check if the tmp file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
@@ -482,14 +462,18 @@
         output_gpd_gdf = (
             input_gdf[columns]
             .dissolve(by=list(groupby_columns_upper))  # type: ignore
             .reset_index()
         ).rename(columns=groupby_columns_upper)
     if explode:
         output_gpd_gdf = output_gpd_gdf.explode(ignore_index=True)
+    if gridsize != 0.0:
+        output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
+            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+        )
     output_gpd_path = tmp_path / f"{input_path.stem}_gpd-output{suffix}"
     gfo.to_file(output_gpd_gdf, output_gpd_path)
 
     # Small differences with the geopandas result are expected, because gfo
     # adds points in the tiling process. So only basic checks possible.
     # assert_geodataframe_equal(
     #        output_gdf, output_gpd_gdf, promote_to_multi=True, sort_values=True,
@@ -590,14 +574,15 @@
 
             _geoops_sql.dissolve_singlethread(
                 input_path=input_path,
                 output_path=output_path,
                 groupby_columns=groupby_columns,
                 explodecollections=True,
                 agg_columns=agg_columns,
+                gridsize=0.0,
             )
         else:
             gfo.dissolve(
                 input_path=input_path,
                 output_path=output_path,
                 groupby_columns=groupby_columns,
                 explodecollections=True,
@@ -898,104 +883,106 @@
         assert len(grasland_json_firstrow) == len(input_layerinfo.columns)
     else:
         # fid_orig column is added in json
         assert len(grasland_json_firstrow) == len(agg_columns["json"]) + 1
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg, testfile",
+    "suffix, epsg, testfile, gridsize",
     [
-        (".gpkg", 31370, "polygon-parcel"),
-        (".gpkg", 31370, "linestring-row-trees"),
-        (".gpkg", 4326, "polygon-parcel"),
-        (".shp", 31370, "polygon-parcel"),
-        (".shp", 4326, "polygon-parcel"),
+        (".gpkg", 31370, "polygon-parcel", 0.001),
+        (".gpkg", 31370, "linestring-row-trees", 0.001),
+        (".gpkg", 4326, "polygon-parcel", 0.0),
+        (".shp", 31370, "polygon-parcel", 0.001),
+        (".shp", 4326, "polygon-parcel", 0.0),
     ],
 )
-def test_simplify_vw(tmp_path, suffix, epsg, testfile):
-    # Skip test if simplification is not available
-    _ = pytest.importorskip("simplification")
-
-    # Init
+def test_simplify_lang(tmp_path, suffix, epsg, testfile, gridsize):
     input_path = test_helper.get_testfile(testfile, suffix=suffix, epsg=epsg)
     input_layerinfo = gfo.get_layerinfo(input_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
     assert input_layerinfo.crs is not None
     if input_layerinfo.crs.is_projected:
         tolerance = 5
     else:
         # 1 degree = 111 km or 111000 m
         tolerance = 5 / 111000
-
-    # Test vw (visvalingam-whyatt) algorithm
-    output_path = tmp_path / f"{input_path.stem}-output_vw{suffix}"
+    # Test lang algorithm
+    output_path = tmp_path / f"{input_path.stem}-output_lang{suffix}"
     gfo.simplify(
         input_path=input_path,
         output_path=output_path,
         tolerance=tolerance,
-        algorithm=geometry_util.SimplifyAlgorithm.VISVALINGAM_WHYATT,
+        algorithm=geometry_util.SimplifyAlgorithm.LANG,
+        lookahead=8,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
-    # Check if the file is correctly created
+    # Check if the tmp file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     output_layerinfo = gfo.get_layerinfo(output_path)
     assert input_layerinfo.featurecount == output_layerinfo.featurecount
     assert len(input_layerinfo.columns) == len(output_layerinfo.columns)
     assert output_layerinfo.geometrytype == input_layerinfo.geometrytype
 
     # Check the contents of the result file
     input_gdf = gfo.read_file(input_path)
     output_gdf = gfo.read_file(output_path)
     assert input_gdf.crs == output_gdf.crs
     assert len(output_gdf) == output_layerinfo.featurecount
     assert output_gdf["geometry"][0] is not None
-    # TODO: a more in-depth check would be better
+    # TODO: some more in-depth validations would be better
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg, testfile",
+    "suffix, epsg, testfile, gridsize",
     [
-        (".gpkg", 31370, "polygon-parcel"),
-        (".gpkg", 31370, "linestring-row-trees"),
-        (".gpkg", 4326, "polygon-parcel"),
-        (".shp", 31370, "polygon-parcel"),
-        (".shp", 4326, "polygon-parcel"),
+        (".gpkg", 31370, "polygon-parcel", 0.001),
+        (".gpkg", 31370, "linestring-row-trees", 0.001),
+        (".gpkg", 4326, "polygon-parcel", 0.0),
+        (".shp", 31370, "polygon-parcel", 0.001),
+        (".shp", 4326, "polygon-parcel", 0.0),
     ],
 )
-def test_simplify_lang(tmp_path, suffix, epsg, testfile):
+def test_simplify_vw(tmp_path, suffix, epsg, testfile, gridsize):
+    # Skip test if simplification is not available
+    _ = pytest.importorskip("simplification")
+
+    # Init
     input_path = test_helper.get_testfile(testfile, suffix=suffix, epsg=epsg)
     input_layerinfo = gfo.get_layerinfo(input_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
     assert input_layerinfo.crs is not None
     if input_layerinfo.crs.is_projected:
         tolerance = 5
     else:
         # 1 degree = 111 km or 111000 m
         tolerance = 5 / 111000
-    # Test lang algorithm
-    output_path = tmp_path / f"{input_path.stem}-output_lang{suffix}"
+
+    # Test vw (visvalingam-whyatt) algorithm
+    output_path = tmp_path / f"{input_path.stem}-output_vw{suffix}"
     gfo.simplify(
         input_path=input_path,
         output_path=output_path,
         tolerance=tolerance,
-        algorithm=geometry_util.SimplifyAlgorithm.LANG,
-        lookahead=8,
+        algorithm=geometry_util.SimplifyAlgorithm.VISVALINGAM_WHYATT,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
-    # Check if the tmp file is correctly created
+    # Check if the file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     output_layerinfo = gfo.get_layerinfo(output_path)
     assert input_layerinfo.featurecount == output_layerinfo.featurecount
     assert len(input_layerinfo.columns) == len(output_layerinfo.columns)
     assert output_layerinfo.geometrytype == input_layerinfo.geometrytype
 
     # Check the contents of the result file
     input_gdf = gfo.read_file(input_path)
     output_gdf = gfo.read_file(output_path)
     assert input_gdf.crs == output_gdf.crs
     assert len(output_gdf) == output_layerinfo.featurecount
     assert output_gdf["geometry"][0] is not None
-    # TODO: some more in-depth validations would be better
+    # TODO: a more in-depth check would be better
```

### Comparing `geofileops-0.8.0a4/tests/test_geofileops_singlelayer_ogr.py` & `geofileops-0.8.0a5/tests/test_geofileops_singlelayer_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_geofileops_singlelayer_sql.py` & `geofileops-0.8.0a5/tests/test_geofileops_singlelayer_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,51 +2,67 @@
 """
 Tests for operations that are executed using a sql statement on one layer.
 """
 
 import math
 
 import geopandas as gpd
+import geopandas._compat as gpd_compat
 import pytest
+
+if gpd_compat.USE_PYGEOS:
+    import pygeos as shapely2_or_pygeos
+else:
+    import shapely as shapely2_or_pygeos
 from shapely.geometry import MultiPolygon, Polygon
 
 import geofileops as gfo
 from geofileops import GeometryType
 from geofileops.util import _geoops_sql
 from tests import test_helper
 from tests.test_helper import DEFAULT_EPSGS, DEFAULT_SUFFIXES
 from tests.test_helper import assert_geodataframe_equal
 
 
-def test_delete_duplicate_geometries(tmp_path):
+@pytest.mark.parametrize("gridsize", [0.0, 0.1])
+def test_delete_duplicate_geometries(tmp_path, gridsize):
     # Prepare test data
     test_gdf = gpd.GeoDataFrame(
         geometry=[  # type: ignore
             test_helper.TestData.polygon_with_island,
             test_helper.TestData.polygon_with_island,
             test_helper.TestData.polygon_no_islands,
             test_helper.TestData.polygon_no_islands,
             test_helper.TestData.polygon_with_island2,
         ],
         crs=test_helper.TestData.crs_epsg,  # type: ignore
     )
+    expected_gdf = test_gdf.iloc[[0, 2, 4]].reset_index(drop=True)
     suffix = ".gpkg"
     input_path = tmp_path / f"input_test_data{suffix}"
     gfo.to_file(test_gdf, input_path)
     input_info = gfo.get_layerinfo(input_path)
 
     # Run test
     output_path = tmp_path / f"{input_path.stem}-output{suffix}"
     print(f"Run test for suffix {suffix}")
     # delete_duplicate_geometries isn't multiprocess, so no batchsize needed
-    gfo.delete_duplicate_geometries(input_path=input_path, output_path=output_path)
+    gfo.delete_duplicate_geometries(
+        input_path=input_path, output_path=output_path, gridsize=gridsize
+    )
 
     # Check result, 2 duplicates should be removed
     result_info = gfo.get_layerinfo(output_path)
     assert result_info.featurecount == input_info.featurecount - 2
+    result_gdf = gfo.read_file(output_path)
+    if gridsize != 0.0:
+        expected_gdf.geometry = shapely2_or_pygeos.set_precision(
+            expected_gdf.geometry.array.data, grid_size=gridsize
+        )
+    assert_geodataframe_equal(result_gdf, expected_gdf)
 
 
 def test_dissolve_singlethread_output_exists(tmp_path):
     # Prepare test data
     input_path = test_helper.get_testfile("polygon-parcel")
     output_path = tmp_path / f"{input_path.stem}-output{input_path.suffix}"
     output_path.touch()
@@ -227,32 +243,40 @@
             gridsize=1,
             precision=1,
         )
 
 
 @pytest.mark.parametrize("input_suffix", DEFAULT_SUFFIXES)
 @pytest.mark.parametrize("output_suffix", DEFAULT_SUFFIXES)
-def test_select(tmp_path, input_suffix, output_suffix):
+@pytest.mark.parametrize("gridsize", [0.0, 0.01])
+def test_select(tmp_path, input_suffix, output_suffix, gridsize):
     # Prepare test data
     input_path = test_helper.get_testfile("polygon-parcel", suffix=input_suffix)
 
     # Now run test
-    output_path = (
-        tmp_path
-        / f"{input_path.stem}-{input_suffix.replace('.', '')}-output{output_suffix}"
-    )
+    name = f"{input_path.stem}-{input_suffix.replace('.', '')}-output{output_suffix}"
+    output_path = tmp_path / name
     layerinfo_input = gfo.get_layerinfo(input_path)
-    sql_stmt = 'SELECT {geometrycolumn}, oidn, uidn FROM "{input_layer}"'
-    gfo.select(input_path=input_path, output_path=output_path, sql_stmt=sql_stmt)
+    # Column casing seems to behave odd: without gridsize (=subselect) results in upper
+    # casing rgardless of quotes or not, with gridsize (=subselect) casing in select is
+    # retained in output.
+    sql_stmt = 'SELECT {geometrycolumn}, "oidn", "UIDN" FROM "{input_layer}"'
+    gfo.select(
+        input_path=input_path,
+        output_path=output_path,
+        sql_stmt=sql_stmt,
+        gridsize=gridsize,
+    )
 
     # Now check if the tmp file is correctly created
     layerinfo_output = gfo.get_layerinfo(output_path)
     assert layerinfo_input.featurecount == layerinfo_output.featurecount
-    assert "OIDN" in layerinfo_output.columns
-    assert "UIDN" in layerinfo_output.columns
+    columns_output_upper = [col.upper() for col in layerinfo_output.columns]
+    assert "OIDN" in columns_output_upper
+    assert "UIDN" in columns_output_upper
     assert len(layerinfo_output.columns) == 2
     assert layerinfo_output.geometrytype == GeometryType.MULTIPOLYGON
 
     # Now check the contents of the result file
     output_gdf = gfo.read_file(output_path)
     assert output_gdf["geometry"][0] is not None
```

### Comparing `geofileops-0.8.0a4/tests/test_geofileops_twolayers.py` & `geofileops-0.8.0a5/tests/test_geofileops_twolayers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Tests for operations that are executed using a sql statement on two layers.
 """
 
 import math
-from pathlib import Path
-import sys
 
 import geopandas as gpd
+import geopandas._compat as gpd_compat
 import pandas as pd
 import pytest
 
-# Add path so the local geofileops packages are found
-sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
+if gpd_compat.USE_PYGEOS:
+    import pygeos as shapely2_or_pygeos
+else:
+    import shapely as shapely2_or_pygeos
+
+
 import geofileops as gfo
 from geofileops import GeometryType, PrimitiveType
 from geofileops.util import _geoops_sql
 from tests import test_helper
 from tests.test_helper import DEFAULT_SUFFIXES, DEFAULT_TESTFILES
 from tests.test_helper import assert_geodataframe_equal
 
@@ -46,37 +49,43 @@
     assert_geodataframe_equal(
         output_gdf, output_gpd_gdf, promote_to_multi=True, sort_values=True
     )
 
 
 @pytest.mark.parametrize("testfile", DEFAULT_TESTFILES)
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
-def test_erase(tmp_path, testfile, suffix):
+@pytest.mark.parametrize("gridsize", [0.0, 0.001])
+def test_erase(tmp_path, testfile, suffix, gridsize):
     input_path = test_helper.get_testfile(testfile, suffix=suffix)
     erase_path = test_helper.get_testfile("polygon-zone", suffix=suffix)
     input_layerinfo = gfo.get_layerinfo(input_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
     output_path = tmp_path / f"{input_path.stem}-output{suffix}"
 
     gfo.erase(
         input_path=input_path,
         erase_path=erase_path,
         output_path=output_path,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
     # Compare result with geopandas
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     output_gdf = gfo.read_file(output_path)
     input_gdf = gfo.read_file(input_path)
     erase_gdf = gfo.read_file(erase_path)
     output_gpd_gdf = gpd.overlay(
         input_gdf, erase_gdf, how="difference", keep_geom_type=True
     )
+    if gridsize != 0.0:
+        output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
+            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+        )
     assert_geodataframe_equal(
         output_gdf,
         output_gpd_gdf,
         promote_to_multi=True,
         sort_values=True,
         check_less_precise=True,
         normalize=True,
@@ -115,28 +124,30 @@
         sort_values=True,
         check_less_precise=True,
         normalize=True,
     )
 
 
 @pytest.mark.parametrize("suffix", DEFAULT_SUFFIXES)
-def test_export_by_location(tmp_path, suffix):
+@pytest.mark.parametrize("gridsize", [0.0, 0.001])
+def test_export_by_location(tmp_path, suffix, gridsize):
     input_to_select_from_path = test_helper.get_testfile(
         "polygon-parcel", suffix=suffix
     )
     input_to_compare_with_path = test_helper.get_testfile("polygon-zone", suffix=suffix)
     output_path = tmp_path / f"{input_to_select_from_path.stem}-output{suffix}"
     input_layerinfo = gfo.get_layerinfo(input_to_select_from_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
 
     # Test
     gfo.export_by_location(
         input_to_select_from_path=input_to_select_from_path,
         input_to_compare_with_path=input_to_compare_with_path,
         output_path=output_path,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
     # Check if the output file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     output_layerinfo = gfo.get_layerinfo(output_path)
@@ -180,24 +191,25 @@
     # TODO: this test should be more elaborate...
     output_gdf = gfo.read_file(output_path)
     assert output_gdf["geometry"][0] is not None
 
 
 @pytest.mark.parametrize("testfile", ["polygon-parcel"])
 @pytest.mark.parametrize(
-    "suffix, epsg, nb_parallel",
+    "suffix, epsg, gridsize, nb_parallel",
     [
-        (".gpkg", 31370, 1),
-        (".gpkg", 31370, 2),
-        (".gpkg", 4326, 2),
-        (".shp", 31370, 1),
-        (".shp", 31370, 2),
+        (".gpkg", 31370, 0.0, 1),
+        (".gpkg", 31370, 0.01, 1),
+        (".gpkg", 31370, 0.0, 2),
+        (".gpkg", 4326, 0.0, 2),
+        (".shp", 31370, 0.0, 1),
+        (".shp", 31370, 0.0, 2),
     ],
 )
-def test_intersection(tmp_path, testfile, suffix, epsg, nb_parallel):
+def test_intersection(tmp_path, testfile, suffix, epsg, gridsize, nb_parallel):
     input1_path = test_helper.get_testfile(testfile, suffix=suffix, epsg=epsg)
     input2_path = test_helper.get_testfile("polygon-zone", suffix=suffix, epsg=epsg)
 
     # Now run test
     output_path = (
         tmp_path / f"{input1_path.stem}_intersection_{input2_path.stem}{suffix}"
     )
@@ -205,14 +217,15 @@
     input1_layerinfo = gfo.get_layerinfo(input1_path)
     if nb_parallel > 1:
         batchsize = math.ceil(input1_layerinfo.featurecount / 2)
     gfo.intersection(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
+        gridsize=gridsize,
         nb_parallel=nb_parallel,
         batchsize=batchsize,
     )
 
     # Check if the tmp file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
@@ -235,14 +248,18 @@
         input2_gdf, how=overlay_operation, keep_geom_type=True
     )
     renames = {
         name_gpd: name_gfo
         for name_gpd, name_gfo in zip(output_gpd_gdf.columns, output_gdf.columns)
     }
     output_gpd_gdf = output_gpd_gdf.rename(columns=renames)
+    if gridsize != 0.0:
+        output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
+            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+        )
     assert_geodataframe_equal(
         output_gdf, output_gpd_gdf, check_dtype=False, sort_values=True
     )
 
 
 def test_intersection_input_no_index(tmp_path):
     """
@@ -525,17 +542,18 @@
     output_gdf = gfo.read_file(output_path)
     assert len(output_gdf) == expected_featurecount
     if expected_featurecount > 0:
         assert output_gdf["geometry"][0] is not None
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg", [(".gpkg", 31370), (".gpkg", 4384), (".shp", 31370)]
+    "suffix, epsg, gridsize",
+    [(".gpkg", 31370, 0.001), (".gpkg", 4326, 0.0), (".shp", 31370, 0.001)],
 )
-def test_join_nearest(tmp_path, suffix, epsg):
+def test_join_nearest(tmp_path, suffix, epsg, gridsize):
     # Prepare test data
     input1_path = test_helper.get_testfile("polygon-parcel", suffix=suffix, epsg=epsg)
     input2_path = test_helper.get_testfile("polygon-zone", suffix=suffix, epsg=epsg)
     input1_layerinfo = gfo.get_layerinfo(input1_path)
     batchsize = math.ceil(input1_layerinfo.featurecount / 2)
 
     # Now run test
@@ -544,14 +562,15 @@
     input1_columns = ["OIDN", "UIDN", "HFDTLT", "fid"]
     gfo.join_nearest(
         input1_path=input1_path,
         input1_columns=input1_columns,
         input2_path=input2_path,
         output_path=output_path,
         nb_nearest=nb_nearest,
+        gridsize=gridsize,
         batchsize=batchsize,
         force=True,
     )
 
     # Check if the output file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
@@ -570,17 +589,18 @@
     if gfo.GeofileType(input1_path).is_fid_zerobased:
         assert output_gdf.l1_fid.min() == 0
     else:
         assert output_gdf.l1_fid.min() == 1
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg", [(".gpkg", 31370), (".gpkg", 4326), (".shp", 31370)]
+    "suffix, epsg, gridsize",
+    [(".gpkg", 31370, 0.001), (".gpkg", 4326, 0.0), (".shp", 31370, 0.001)],
 )
-def test_select_two_layers(tmp_path, suffix, epsg):
+def test_select_two_layers(tmp_path, suffix, epsg, gridsize):
     # Prepare test data
     input1_path = test_helper.get_testfile("polygon-parcel", suffix=suffix, epsg=epsg)
     input2_path = test_helper.get_testfile("polygon-zone", suffix=suffix, epsg=epsg)
     output_path = tmp_path / f"{input1_path.stem}-output{suffix}"
 
     # Prepare query to execute. At the moment this is just the query for the
     # intersection() operation.
@@ -625,14 +645,15 @@
                   layer1.{{input1_geometrycolumn}},
                   layer2.{{input2_geometrycolumn}}) = 0
     """
     gfo.select_two_layers(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
+        gridsize=gridsize,
         sql_stmt=sql_stmt,
     )
 
     # Check if the tmp file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     input1_layerinfo = gfo.get_layerinfo(input1_path)
@@ -674,15 +695,15 @@
             "select_two_layers: input2_path doesn't exist: not_existing_path",
             test_helper.get_testfile("polygon-zone"),
             "not_existing_path",
             "output.gpkg",
         ),
     ],
 )
-def test_select_two_layers_invalid_params(
+def test_select_two_layers_invalid_paths(
     tmp_path, input1_path, input2_path, output_path, expected_error
 ):
     """
     select_two_layers doesn't get info on input layers up-front, so this is the best
     function to test the lower level checks in _two_layer_vector_operation.
     """
     # Prepare query to execute. Doesn't really matter what as an error is normally raise
@@ -769,29 +790,31 @@
     else:
         gfo.select_two_layers(
             input1_path, input2_path, output_path, sql_stmt, nb_parallel=nb_parallel
         )
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg", [(".gpkg", 31370), (".gpkg", 4326), (".shp", 31370)]
+    "suffix, epsg, gridsize",
+    [(".gpkg", 31370, 0.001), (".gpkg", 4326, 0.0), (".shp", 31370, 0.001)],
 )
-def test_split(tmp_path, suffix, epsg):
+def test_split(tmp_path, suffix, epsg, gridsize):
     # Prepare test data
     input1_path = test_helper.get_testfile("polygon-parcel", suffix=suffix, epsg=epsg)
     input2_path = test_helper.get_testfile("polygon-zone", suffix=suffix, epsg=epsg)
     input1_layerinfo = gfo.get_layerinfo(input1_path)
     batchsize = math.ceil(input1_layerinfo.featurecount / 2)
     output_path = tmp_path / f"{input1_path.stem}-output{suffix}"
 
     # Test
     gfo.split(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
     # Check if the tmp file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     input2_layerinfo = gfo.get_layerinfo(input2_path)
@@ -810,41 +833,47 @@
     input2_gdf = gfo.read_file(input2_path)
     output_gpd_gdf = input1_gdf.overlay(input2_gdf, how="identity", keep_geom_type=True)
     renames = {
         name_gpd: name_gfo
         for name_gpd, name_gfo in zip(output_gpd_gdf.columns, output_gfo_gdf.columns)
     }
     output_gpd_gdf = output_gpd_gdf.rename(columns=renames)
+    if gridsize != 0.0:
+        output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
+            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+        )
     # OIDN is float vs int? -> check_column_type=False
     assert_geodataframe_equal(
         output_gfo_gdf,
         output_gpd_gdf,
         promote_to_multi=True,
         sort_values=True,
         check_less_precise=True,
         normalize=True,
         check_dtype=False,
     )
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg", [(".gpkg", 31370), (".gpkg", 4326), (".shp", 31370)]
+    "suffix, epsg, gridsize",
+    [(".gpkg", 31370, 0.001), (".gpkg", 4326, 0.0), (".shp", 31370, 0.0)],
 )
-def test_symmetric_difference(tmp_path, suffix, epsg):
+def test_symmetric_difference(tmp_path, suffix, epsg, gridsize):
     input1_path = test_helper.get_testfile("polygon-zone", suffix=suffix, epsg=epsg)
     input2_path = test_helper.get_testfile("polygon-parcel", suffix=suffix, epsg=epsg)
     input1_layerinfo = gfo.get_layerinfo(input1_path)
     batchsize = math.ceil(input1_layerinfo.featurecount / 2)
 
     # Test
     output_path = tmp_path / f"{input1_path.stem}_symmdiff_{input2_path.stem}{suffix}"
     gfo.symmetric_difference(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
     # Check if the tmp file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     output_gfo_gdf = gfo.read_file(output_path)
@@ -855,50 +884,56 @@
         input2_gdf, how="symmetric_difference", keep_geom_type=True
     )
     renames = {
         name_gpd: name_gfo
         for name_gpd, name_gfo in zip(output_gpd_gdf.columns, output_gfo_gdf.columns)
     }
     output_gpd_gdf = output_gpd_gdf.rename(columns=renames)
+    if gridsize != 0.0:
+        output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
+            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+        )
     assert_geodataframe_equal(
         output_gfo_gdf,
         output_gpd_gdf,
         promote_to_multi=True,
         sort_values=True,
         check_column_type=False,
         check_dtype=False,
         check_less_precise=True,
         normalize=True,
     )
 
 
 @pytest.mark.parametrize(
-    "suffix, epsg", [(".gpkg", 31370), (".gpkg", 4326), (".shp", 31370)]
+    "suffix, epsg, gridsize",
+    [(".gpkg", 31370, 0.001), (".gpkg", 4326, 0.0), (".shp", 31370, 0.0)],
 )
-def test_union(tmp_path, suffix, epsg):
+def test_union(tmp_path, suffix, epsg, gridsize):
     # Prepare test files
     input1_path = test_helper.get_testfile(
         "polygon-parcel", dst_dir=tmp_path, suffix=suffix, epsg=epsg
     )
     input2_path = test_helper.get_testfile(
         "polygon-zone", dst_dir=tmp_path, suffix=suffix, epsg=epsg
     )
     # Add null TEXT column to each file to make sure it stays TEXT type after union
     gfo.add_column(input1_path, name="test1_null", type=gfo.DataType.TEXT)
     gfo.add_column(input2_path, name="test2_null", type=gfo.DataType.TEXT)
 
     input1_layerinfo = gfo.get_layerinfo(input1_path)
     batchsize = math.ceil(input1_layerinfo.featurecount / 2)
+    output_path = tmp_path / f"{input1_path.stem}_union_{input2_path.stem}{suffix}"
 
     # Test
-    output_path = tmp_path / f"{input1_path.stem}_union_{input2_path.stem}{suffix}"
     gfo.union(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
+        gridsize=gridsize,
         batchsize=batchsize,
     )
 
     # Check if the tmp file is correctly created
     assert output_path.exists()
     assert gfo.has_spatial_index(output_path)
     input2_layerinfo = gfo.get_layerinfo(input2_path)
@@ -917,14 +952,18 @@
     output_gpd_gdf = input1_gdf.overlay(input2_gdf, how="union", keep_geom_type=True)
     renames = {
         name_gpd: name_gfo
         for name_gpd, name_gfo in zip(output_gpd_gdf.columns, output_gfo_gdf.columns)
     }
     output_gpd_gdf = output_gpd_gdf.rename(columns=renames)
     output_gpd_gdf["l1_DATUM"] = pd.to_datetime(output_gpd_gdf["l1_DATUM"])
+    if gridsize != 0.0:
+        output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
+            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+        )
     assert_geodataframe_equal(
         output_gfo_gdf,
         output_gpd_gdf,
         promote_to_multi=True,
         sort_values=True,
         check_less_precise=True,
         normalize=True,
```

### Comparing `geofileops-0.8.0a4/tests/test_geofiletype.py` & `geofileops-0.8.0a5/tests/test_geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_geometry_util.py` & `geofileops-0.8.0a5/tests/test_geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_geoseries_util.py` & `geofileops-0.8.0a5/tests/test_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_grid_util.py` & `geofileops-0.8.0a5/tests/test_grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_helper.py` & `geofileops-0.8.0a5/tests/test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,19 +135,19 @@
     point = sh_geom.Point((0, 0))
     multipoint = sh_geom.MultiPoint([(0, 0), (10, 10), (20, 20)])
     linestring = sh_geom.LineString([(0, 0), (10, 10), (20, 20)])
     multilinestring = sh_geom.MultiLineString(
         [linestring.coords, [(100, 100), (110, 110), (120, 120)]]
     )
     polygon_with_island = sh_geom.Polygon(
-        shell=[(0, 0), (0, 10), (1, 10), (10, 10), (10, 0), (0, 0)],
+        shell=[(0.01, 0), (0.01, 10), (1, 10), (10, 10), (10, 0), (0.01, 0)],
         holes=[[(2, 2), (2, 8), (8, 8), (8, 2), (2, 2)]],
     )
     polygon_no_islands = sh_geom.Polygon(
-        shell=[(100, 100), (100, 110), (110, 110), (110, 100), (100, 100)]
+        shell=[(100.01, 100), (100.01, 110), (110, 110), (110, 100), (100.01, 100)]
     )
     polygon_with_island2 = sh_geom.Polygon(
         shell=[(20, 20), (20, 30), (21, 30), (30, 30), (30, 20), (20, 20)],
         holes=[[(22, 22), (22, 28), (28, 28), (28, 22), (22, 22)]],
     )
     multipolygon = sh_geom.MultiPolygon([polygon_no_islands, polygon_with_island2])
     geometrycollection = sh_geom.GeometryCollection(
```

### Comparing `geofileops-0.8.0a4/tests/test_io_util.py` & `geofileops-0.8.0a5/tests/test_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_layerstyles.py` & `geofileops-0.8.0a5/tests/test_layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_ogr_sql_util.py` & `geofileops-0.8.0a5/tests/test_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_ogr_util.py` & `geofileops-0.8.0a5/tests/test_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_parameter_helper.py` & `geofileops-0.8.0a5/tests/test_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_processing_util.py` & `geofileops-0.8.0a5/tests/test_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_spatialite.py` & `geofileops-0.8.0a5/tests/test_spatialite.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a4/tests/test_sqlite_util.py` & `geofileops-0.8.0a5/tests/test_sqlite_util.py`

 * *Files identical despite different names*

