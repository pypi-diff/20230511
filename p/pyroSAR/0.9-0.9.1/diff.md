# Comparing `tmp/pyroSAR-0.9.tar.gz` & `tmp/pyroSAR-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroSAR-0.9.tar", last modified: Tue Jun 18 11:50:41 2019, max compression
+gzip compressed data, was "dist/pyroSAR-0.9.1.tar", last modified: Thu Jul  4 23:37:07 2019, max compression
```

## Comparing `pyroSAR-0.9.tar` & `pyroSAR-0.9.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/examples/
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/examples/scoop/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     3673 2019-01-14 10:02:26.000000 pyroSAR-0.9/examples/scoop/example_scoop_snap.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      179 2019-01-14 10:02:26.000000 pyroSAR-0.9/examples/scoop/start_gamma.sh
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     6428 2019-01-14 10:02:26.000000 pyroSAR-0.9/examples/scoop/example_scoop_gamma.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      177 2019-01-14 10:02:26.000000 pyroSAR-0.9/examples/scoop/start_snap.sh
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      328 2019-01-14 10:02:26.000000 pyroSAR-0.9/examples/scoop/scheduler
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      303 2019-01-14 10:02:26.000000 pyroSAR-0.9/examples/scoop/prolog
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1582 2019-01-14 10:02:26.000000 pyroSAR-0.9/examples/example_stacking.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2431 2019-04-08 07:29:29.000000 pyroSAR-0.9/examples/example_GAMMA_DEM_preparation.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    15917 2019-06-18 11:50:41.000000 pyroSAR-0.9/PKG-INFO
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       38 2019-06-18 11:50:41.000000 pyroSAR-0.9/setup.cfg
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    13484 2019-04-29 07:10:54.000000 pyroSAR-0.9/README.md
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      238 2019-02-12 17:23:37.000000 pyroSAR-0.9/pyroSAR/dev_incidence.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      129 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/__init__.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      363 2019-03-25 13:04:47.000000 pyroSAR-0.9/pyroSAR/dev_auxdata.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    82131 2019-04-29 07:10:54.000000 pyroSAR-0.9/pyroSAR/drivers.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    11779 2019-04-13 15:28:41.000000 pyroSAR-0.9/pyroSAR/_dev_config.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/gamma/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    17986 2019-06-14 09:24:33.000000 pyroSAR-0.9/pyroSAR/gamma/auxil.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      206 2019-04-08 07:29:29.000000 pyroSAR-0.9/pyroSAR/gamma/__init__.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)   252201 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/gamma/parser_demo.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    44953 2019-06-07 09:05:52.000000 pyroSAR-0.9/pyroSAR/gamma/util.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    30667 2019-04-29 07:10:54.000000 pyroSAR-0.9/pyroSAR/gamma/parser.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    21443 2019-04-29 12:47:58.000000 pyroSAR-0.9/pyroSAR/gamma/dem.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2263 2019-04-02 14:18:38.000000 pyroSAR-0.9/pyroSAR/gamma/dev_S1B.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      143 2019-03-06 16:05:41.000000 pyroSAR-0.9/pyroSAR/gamma/dev_parser.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     3845 2019-04-15 10:56:31.000000 pyroSAR-0.9/pyroSAR/gamma/error.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      206 2019-02-11 16:31:32.000000 pyroSAR-0.9/pyroSAR/gamma/dev_UTM.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      464 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/gamma/api.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/S1/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    24968 2019-04-29 07:10:54.000000 pyroSAR-0.9/pyroSAR/S1/auxil.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       66 2019-04-23 12:38:08.000000 pyroSAR-0.9/pyroSAR/S1/__init__.py
--rw-rw-r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     8238 2019-05-03 07:34:33.000000 pyroSAR-0.9/pyroSAR/S1/linesimplify.py
--rw-rw-r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    17306 2019-04-23 14:07:20.000000 pyroSAR-0.9/pyroSAR/S1/polysimplify.py
--rw-rw-r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     4231 2019-05-02 16:34:51.000000 pyroSAR-0.9/pyroSAR/S1/dev_bnr.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/ERS/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     4115 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/ERS/auxil.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       47 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/ERS/__init__.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/ERS/data/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851) 14274560 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/ERS/data/erspasses.db
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    25550 2019-02-17 12:44:58.000000 pyroSAR-0.9/pyroSAR/datacube_util.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/snap/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    36147 2019-06-04 13:05:32.000000 pyroSAR-0.9/pyroSAR/snap/auxil.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       62 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/__init__.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/snap/recipes/
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      189 2019-03-08 15:26:53.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Read.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      728 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Subset.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      376 2019-03-04 08:05:21.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Multilook.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      382 2019-03-29 07:46:48.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Remove-GRD-Border-Noise.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      700 2019-05-02 07:44:08.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Terrain-Flattening.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2663 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/SARSim-Terrain-Correction.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      386 2019-03-04 08:05:21.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/ThermalNoiseRemoval.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      215 2019-02-11 16:45:45.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Write.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2067 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Terrain-Correction.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      579 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/SAR-Simulation.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1342 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Cross-Correlation.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      292 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/recipes/nodes/lin2db.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2719 2019-05-02 07:11:11.000000 pyroSAR-0.9/pyroSAR/snap/recipes/base.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      141 2019-03-08 15:26:53.000000 pyroSAR-0.9/pyroSAR/snap/recipes/blank.xml
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    20881 2019-06-07 09:06:23.000000 pyroSAR-0.9/pyroSAR/snap/util.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1059 2019-02-25 12:28:21.000000 pyroSAR-0.9/pyroSAR/snap/dev_process.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR/snap/data/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     3095 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/snap/data/snap.auxdata.properties
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      628 2019-05-06 11:03:49.000000 pyroSAR-0.9/pyroSAR/snap/dev_split.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      281 2019-05-06 09:36:12.000000 pyroSAR-0.9/pyroSAR/snap/dev_del_wf_node.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1504 2019-04-08 15:18:09.000000 pyroSAR-0.9/pyroSAR/dev_auxdata_david.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     7723 2019-04-29 07:10:54.000000 pyroSAR-0.9/pyroSAR/ancillary.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    25663 2019-05-22 19:29:08.000000 pyroSAR-0.9/pyroSAR/auxdata.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2061 2019-01-14 10:02:26.000000 pyroSAR-0.9/pyroSAR/xml_util.py
-drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR.egg-info/
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1956 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR.egg-info/SOURCES.txt
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)        8 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR.egg-info/top_level.txt
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    15917 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR.egg-info/PKG-INFO
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)        1 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR.egg-info/dependency_links.txt
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       77 2019-06-18 11:50:41.000000 pyroSAR-0.9/pyroSAR.egg-info/requires.txt
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)        1 2019-02-11 16:59:36.000000 pyroSAR-0.9/pyroSAR.egg-info/not-zip-safe
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1513 2019-06-15 19:51:40.000000 pyroSAR-0.9/setup.py
--rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      140 2019-01-14 10:02:26.000000 pyroSAR-0.9/MANIFEST.in
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/examples/
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/examples/scoop/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     3673 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/examples/scoop/example_scoop_snap.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      179 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/examples/scoop/start_gamma.sh
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     6428 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/examples/scoop/example_scoop_gamma.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      177 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/examples/scoop/start_snap.sh
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      328 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/examples/scoop/scheduler
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      303 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/examples/scoop/prolog
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1582 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/examples/example_stacking.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2431 2019-04-08 07:29:29.000000 pyroSAR-0.9.1/examples/example_GAMMA_DEM_preparation.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    16488 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/PKG-INFO
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       38 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/setup.cfg
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    13925 2019-06-18 12:46:56.000000 pyroSAR-0.9.1/README.md
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      238 2019-02-12 17:23:37.000000 pyroSAR-0.9.1/pyroSAR/dev_incidence.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      129 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/__init__.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      363 2019-03-25 13:04:47.000000 pyroSAR-0.9.1/pyroSAR/dev_auxdata.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    82131 2019-04-29 07:10:54.000000 pyroSAR-0.9.1/pyroSAR/drivers.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    11779 2019-04-13 15:28:41.000000 pyroSAR-0.9.1/pyroSAR/_dev_config.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/gamma/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    17986 2019-06-14 09:24:33.000000 pyroSAR-0.9.1/pyroSAR/gamma/auxil.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      206 2019-04-08 07:29:29.000000 pyroSAR-0.9.1/pyroSAR/gamma/__init__.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)   252201 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/gamma/parser_demo.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    44953 2019-06-07 09:05:52.000000 pyroSAR-0.9.1/pyroSAR/gamma/util.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    30667 2019-04-29 07:10:54.000000 pyroSAR-0.9.1/pyroSAR/gamma/parser.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    21692 2019-06-21 11:00:40.000000 pyroSAR-0.9.1/pyroSAR/gamma/dem.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2263 2019-04-02 14:18:38.000000 pyroSAR-0.9.1/pyroSAR/gamma/dev_S1B.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      143 2019-03-06 16:05:41.000000 pyroSAR-0.9.1/pyroSAR/gamma/dev_parser.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     3845 2019-04-15 10:56:31.000000 pyroSAR-0.9.1/pyroSAR/gamma/error.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      206 2019-02-11 16:31:32.000000 pyroSAR-0.9.1/pyroSAR/gamma/dev_UTM.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      464 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/gamma/api.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/S1/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    24968 2019-04-29 07:10:54.000000 pyroSAR-0.9.1/pyroSAR/S1/auxil.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       66 2019-04-23 12:38:08.000000 pyroSAR-0.9.1/pyroSAR/S1/__init__.py
+-rw-rw-r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     8238 2019-05-03 07:34:33.000000 pyroSAR-0.9.1/pyroSAR/S1/linesimplify.py
+-rw-rw-r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    17306 2019-04-23 14:07:20.000000 pyroSAR-0.9.1/pyroSAR/S1/polysimplify.py
+-rw-rw-r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     4231 2019-05-02 16:34:51.000000 pyroSAR-0.9.1/pyroSAR/S1/dev_bnr.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/ERS/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     4115 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/ERS/auxil.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       47 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/ERS/__init__.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/ERS/data/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851) 14274560 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/ERS/data/erspasses.db
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    25550 2019-02-17 12:44:58.000000 pyroSAR-0.9.1/pyroSAR/datacube_util.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/snap/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    36147 2019-06-04 13:05:32.000000 pyroSAR-0.9.1/pyroSAR/snap/auxil.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       62 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/__init__.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      189 2019-03-08 15:26:53.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Read.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      728 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Subset.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      376 2019-03-04 08:05:21.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Multilook.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      382 2019-03-29 07:46:48.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Remove-GRD-Border-Noise.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      700 2019-05-02 07:44:08.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Terrain-Flattening.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2663 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/SARSim-Terrain-Correction.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      386 2019-03-04 08:05:21.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/ThermalNoiseRemoval.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      215 2019-02-11 16:45:45.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Write.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2067 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Terrain-Correction.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      579 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/SAR-Simulation.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1342 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Cross-Correlation.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      292 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/lin2db.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2719 2019-05-02 07:11:11.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/base.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      141 2019-03-08 15:26:53.000000 pyroSAR-0.9.1/pyroSAR/snap/recipes/blank.xml
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    20884 2019-06-30 13:11:07.000000 pyroSAR-0.9.1/pyroSAR/snap/util.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1059 2019-02-25 12:28:21.000000 pyroSAR-0.9.1/pyroSAR/snap/dev_process.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR/snap/data/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     3095 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/snap/data/snap.auxdata.properties
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      628 2019-05-06 11:03:49.000000 pyroSAR-0.9.1/pyroSAR/snap/dev_split.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      281 2019-05-06 09:36:12.000000 pyroSAR-0.9.1/pyroSAR/snap/dev_del_wf_node.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1504 2019-04-08 15:18:09.000000 pyroSAR-0.9.1/pyroSAR/dev_auxdata_david.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     7723 2019-04-29 07:10:54.000000 pyroSAR-0.9.1/pyroSAR/ancillary.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    25916 2019-06-21 10:57:54.000000 pyroSAR-0.9.1/pyroSAR/auxdata.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     2061 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/pyroSAR/xml_util.py
+drwxr-xr-x   0 truc_jh  (122958) dlr_truc_jh_p (423851)        0 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR.egg-info/
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1956 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR.egg-info/SOURCES.txt
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)        8 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR.egg-info/top_level.txt
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)    16488 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR.egg-info/PKG-INFO
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)        1 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR.egg-info/dependency_links.txt
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)       77 2019-07-04 23:37:07.000000 pyroSAR-0.9.1/pyroSAR.egg-info/requires.txt
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)        1 2019-02-11 16:59:36.000000 pyroSAR-0.9.1/pyroSAR.egg-info/not-zip-safe
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)     1515 2019-07-04 23:19:20.000000 pyroSAR-0.9.1/setup.py
+-rw-r--r--   0 truc_jh  (122958) dlr_truc_jh_p (423851)      140 2019-01-14 10:02:26.000000 pyroSAR-0.9.1/MANIFEST.in
```

### Comparing `pyroSAR-0.9/examples/scoop/example_scoop_snap.py` & `pyroSAR-0.9.1/examples/scoop/example_scoop_snap.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/examples/scoop/example_scoop_gamma.py` & `pyroSAR-0.9.1/examples/scoop/example_scoop_gamma.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/examples/example_stacking.py` & `pyroSAR-0.9.1/examples/example_stacking.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/examples/example_GAMMA_DEM_preparation.py` & `pyroSAR-0.9.1/examples/example_GAMMA_DEM_preparation.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/PKG-INFO` & `pyroSAR-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroSAR
-Version: 0.9
+Version: 0.9.1
 Summary: a framework for large-scale SAR satellite data processing
 Home-page: https://github.com/johntruckenbrodt/pyroSAR.git
 Author: John Truckenbrodt
 Author-email: john.truckenbrodt@uni-jena.de
 License: MIT
 Description: <h1 align="center">
           <br>
@@ -38,36 +38,52 @@
         * Reading of data from various past and present satellite missions
         * Handling of acquisition metadata
         * User-friendly access to processing utilities in SNAP and GAMMA Remote Sensing software
         * Formatting of the preprocessed data for further analysis
         
         [Here](https://pyrosar.readthedocs.io/en/latest/?badge=latest) you can find the documentation.
         
+        pyroSAR is/was used in these projects:
+        * [BACI](http://www.baci-h2020.eu/index.php/Main/HomePage)
+        * [CCI Biomass](http://cci.esa.int/biomass)
+        * [GlobBiomass](http://globbiomass.org/)
+        * [SALDI](https://www.saldi.uni-jena.de/)
+        * [SenThIS](https://eos-jena.com/en/projects/)
+        * [Sentinel4REDD](https://www.dlr.de/rd/en/Portaldata/28/Resources/dokumente/re/Projektblatt_Sentinel4REDD_engl.pdf)
+        * [SWOS](https://www.swos-service.eu/)
+        
+        You know of other projects? We'd be happy to know.
+        
         # Installation
-        For the installation we need the Python tool pip and the version control system git. On Windows pip is 
-        installed together with Anaconda, git can be downloaded from [here](https://git-scm.com/downloads).
-        On Linux you can easily install both via command line:
+        First we need to install pip. On Windows pip is installed together with Anaconda, on Linux you can easily install it
+         via command line:
         ```sh
         sudo apt-get install python-pip
+        ```
+        The latest stable release of pyroSAR can then be installed:
+        ```sh
+        python -m pip install pyroSAR
+        ```
+        
+        For installation of the latest master branch on GitHub, we need the version control system git. On Windows, git can be 
+        downloaded from [here](https://git-scm.com/downloads). On Linux you can install it via command line:
+        ```sh
         sudo apt-get install git
         ```
         Once everything is set up, pyroSAR is ready to be installed:
         ```sh
-        sudo pip install git+https://github.com/johntruckenbrodt/pyroSAR.git
+        python -m pip install git+https://github.com/johntruckenbrodt/pyroSAR.git
         ```
-        On Windows you need to use the Anaconda Prompt and leave out `sudo` in the above command.
         
         # Dependencies
         If you are using Windows, the easiest way to work with pyroSAR and Python in general is by using 
         [Anaconda](https://www.anaconda.com/download/). It comes with all basic requirements of pyroSAR.
         The more specific instructions below are intended for Linux users.
         ### GDAL
-        pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as dependencies as well as the GDAL Python binding. 
-        Alternatively, one can use <a href="https://github.com/nextgis/pygdal">pygdal</a>, 
-        a virtualenv and setuptools friendly version of standard GDAL python bindings.
+        pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as dependencies as well as the GDAL Python binding.
         #### Ubuntu
         Starting with release Yakkety (16.10), Ubuntu comes with GDAL >2.1. 
         See <a href="https://launchpad.net/ubuntu/yakkety/amd64/gdal-bin">here</a>. 
         You can install it like this:
         ```bash
         sudo apt-get install python-gdal python3-gdal gdal-bin
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyroSAR Version: 0.9 Summary: a framework for
+Metadata-Version: 2.1 Name: pyroSAR Version: 0.9.1 Summary: a framework for
 large-scale SAR satellite data processing Home-page: https://github.com/
 johntruckenbrodt/pyroSAR.git Author: John Truckenbrodt Author-email:
 john.truckenbrodt@uni-jena.de License: MIT Description:
                                     ******
                                 pyroSAR ******
   **** A Python Framework for Large-Scale SAR Satellite Data Processing ****
 Description â¢ Installation â¢ Dependencies â¢ Example â¢ Notes â¢ Authors
@@ -10,33 +10,39 @@
  [Appveyor_Status] [Coveralls_Status] [Documentation_Status] [PIP_Status]
 # Description The pyroSAR package aims at providing a complete solution for the
 scalable organization and processing of SAR satellite data: * Reading of data
 from various past and present satellite missions * Handling of acquisition
 metadata * User-friendly access to processing utilities in SNAP and GAMMA
 Remote Sensing software * Formatting of the preprocessed data for further
 analysis [Here](https://pyrosar.readthedocs.io/en/latest/?badge=latest) you can
-find the documentation. # Installation For the installation we need the Python
-tool pip and the version control system git. On Windows pip is installed
-together with Anaconda, git can be downloaded from [here](https://git-scm.com/
-downloads). On Linux you can easily install both via command line: ```sh sudo
-apt-get install python-pip sudo apt-get install git ``` Once everything is set
-up, pyroSAR is ready to be installed: ```sh sudo pip install git+https://
-github.com/johntruckenbrodt/pyroSAR.git ``` On Windows you need to use the
-Anaconda Prompt and leave out `sudo` in the above command. # Dependencies If
-you are using Windows, the easiest way to work with pyroSAR and Python in
-general is by using [Anaconda](https://www.anaconda.com/download/). It comes
-with all basic requirements of pyroSAR. The more specific instructions below
-are intended for Linux users. ### GDAL pyroSAR requires GDAL version 2.1 with
-GEOS and PROJ4 as dependencies as well as the GDAL Python binding.
-Alternatively, one can use pygdal, a virtualenv and setuptools friendly version
-of standard GDAL python bindings. #### Ubuntu Starting with release Yakkety
-(16.10), Ubuntu comes with GDAL >2.1. See here. You can install it like this:
-```bash sudo apt-get install python-gdal python3-gdal gdal-bin ``` For older
-Ubuntu releases you can add the ubuntugis repository to apt prior to
-installation to install version >2.1: ```sh sudo add-apt-repository ppa:
+find the documentation. pyroSAR is/was used in these projects: * [BACI](http://
+www.baci-h2020.eu/index.php/Main/HomePage) * [CCI Biomass](http://cci.esa.int/
+biomass) * [GlobBiomass](http://globbiomass.org/) * [SALDI](https://
+www.saldi.uni-jena.de/) * [SenThIS](https://eos-jena.com/en/projects/) *
+[Sentinel4REDD](https://www.dlr.de/rd/en/Portaldata/28/Resources/dokumente/re/
+Projektblatt_Sentinel4REDD_engl.pdf) * [SWOS](https://www.swos-service.eu/) You
+know of other projects? We'd be happy to know. # Installation First we need to
+install pip. On Windows pip is installed together with Anaconda, on Linux you
+can easily install it via command line: ```sh sudo apt-get install python-pip
+``` The latest stable release of pyroSAR can then be installed: ```sh python -
+m pip install pyroSAR ``` For installation of the latest master branch on
+GitHub, we need the version control system git. On Windows, git can be
+downloaded from [here](https://git-scm.com/downloads). On Linux you can install
+it via command line: ```sh sudo apt-get install git ``` Once everything is set
+up, pyroSAR is ready to be installed: ```sh python -m pip install git+https://
+github.com/johntruckenbrodt/pyroSAR.git ``` # Dependencies If you are using
+Windows, the easiest way to work with pyroSAR and Python in general is by using
+[Anaconda](https://www.anaconda.com/download/). It comes with all basic
+requirements of pyroSAR. The more specific instructions below are intended for
+Linux users. ### GDAL pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as
+dependencies as well as the GDAL Python binding. #### Ubuntu Starting with
+release Yakkety (16.10), Ubuntu comes with GDAL >2.1. See here. You can install
+it like this: ```bash sudo apt-get install python-gdal python3-gdal gdal-bin
+``` For older Ubuntu releases you can add the ubuntugis repository to apt prior
+to installation to install version >2.1: ```sh sudo add-apt-repository ppa:
 ubuntugis/ppa sudo apt-get update ``` This way the required dependencies (GEOS
 and PROJ4 in particular) are also installed. You can check the version by
 typing: ```sh gdalinfo --version ``` #### Debian Starting with Debian 9
 (Stretch) GDAL is available in version >2.1 in the official repository. ####
 Building from source Alternatively, you can build GDAL and the dependencies
 from source. The script `pyroSAR/install/install_deps.sh` gives specific
 instructions on how to do it. It is not yet intended to run this script via
```

### Comparing `pyroSAR-0.9/README.md` & `pyroSAR-0.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,36 +30,52 @@
 * Reading of data from various past and present satellite missions
 * Handling of acquisition metadata
 * User-friendly access to processing utilities in SNAP and GAMMA Remote Sensing software
 * Formatting of the preprocessed data for further analysis
 
 [Here](https://pyrosar.readthedocs.io/en/latest/?badge=latest) you can find the documentation.
 
+pyroSAR is/was used in these projects:
+* [BACI](http://www.baci-h2020.eu/index.php/Main/HomePage)
+* [CCI Biomass](http://cci.esa.int/biomass)
+* [GlobBiomass](http://globbiomass.org/)
+* [SALDI](https://www.saldi.uni-jena.de/)
+* [SenThIS](https://eos-jena.com/en/projects/)
+* [Sentinel4REDD](https://www.dlr.de/rd/en/Portaldata/28/Resources/dokumente/re/Projektblatt_Sentinel4REDD_engl.pdf)
+* [SWOS](https://www.swos-service.eu/)
+
+You know of other projects? We'd be happy to know.
+
 # Installation
-For the installation we need the Python tool pip and the version control system git. On Windows pip is 
-installed together with Anaconda, git can be downloaded from [here](https://git-scm.com/downloads).
-On Linux you can easily install both via command line:
+First we need to install pip. On Windows pip is installed together with Anaconda, on Linux you can easily install it
+ via command line:
 ```sh
 sudo apt-get install python-pip
+```
+The latest stable release of pyroSAR can then be installed:
+```sh
+python -m pip install pyroSAR
+```
+
+For installation of the latest master branch on GitHub, we need the version control system git. On Windows, git can be 
+downloaded from [here](https://git-scm.com/downloads). On Linux you can install it via command line:
+```sh
 sudo apt-get install git
 ```
 Once everything is set up, pyroSAR is ready to be installed:
 ```sh
-sudo pip install git+https://github.com/johntruckenbrodt/pyroSAR.git
+python -m pip install git+https://github.com/johntruckenbrodt/pyroSAR.git
 ```
-On Windows you need to use the Anaconda Prompt and leave out `sudo` in the above command.
 
 # Dependencies
 If you are using Windows, the easiest way to work with pyroSAR and Python in general is by using 
 [Anaconda](https://www.anaconda.com/download/). It comes with all basic requirements of pyroSAR.
 The more specific instructions below are intended for Linux users.
 ### GDAL
-pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as dependencies as well as the GDAL Python binding. 
-Alternatively, one can use <a href="https://github.com/nextgis/pygdal">pygdal</a>, 
-a virtualenv and setuptools friendly version of standard GDAL python bindings.
+pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as dependencies as well as the GDAL Python binding.
 #### Ubuntu
 Starting with release Yakkety (16.10), Ubuntu comes with GDAL >2.1. 
 See <a href="https://launchpad.net/ubuntu/yakkety/amd64/gdal-bin">here</a>. 
 You can install it like this:
 ```bash
 sudo apt-get install python-gdal python3-gdal gdal-bin
 ```
```

#### html2text {}

```diff
@@ -6,33 +6,39 @@
  [Appveyor_Status] [Coveralls_Status] [Documentation_Status] [PIP_Status]
 # Description The pyroSAR package aims at providing a complete solution for the
 scalable organization and processing of SAR satellite data: * Reading of data
 from various past and present satellite missions * Handling of acquisition
 metadata * User-friendly access to processing utilities in SNAP and GAMMA
 Remote Sensing software * Formatting of the preprocessed data for further
 analysis [Here](https://pyrosar.readthedocs.io/en/latest/?badge=latest) you can
-find the documentation. # Installation For the installation we need the Python
-tool pip and the version control system git. On Windows pip is installed
-together with Anaconda, git can be downloaded from [here](https://git-scm.com/
-downloads). On Linux you can easily install both via command line: ```sh sudo
-apt-get install python-pip sudo apt-get install git ``` Once everything is set
-up, pyroSAR is ready to be installed: ```sh sudo pip install git+https://
-github.com/johntruckenbrodt/pyroSAR.git ``` On Windows you need to use the
-Anaconda Prompt and leave out `sudo` in the above command. # Dependencies If
-you are using Windows, the easiest way to work with pyroSAR and Python in
-general is by using [Anaconda](https://www.anaconda.com/download/). It comes
-with all basic requirements of pyroSAR. The more specific instructions below
-are intended for Linux users. ### GDAL pyroSAR requires GDAL version 2.1 with
-GEOS and PROJ4 as dependencies as well as the GDAL Python binding.
-Alternatively, one can use pygdal, a virtualenv and setuptools friendly version
-of standard GDAL python bindings. #### Ubuntu Starting with release Yakkety
-(16.10), Ubuntu comes with GDAL >2.1. See here. You can install it like this:
-```bash sudo apt-get install python-gdal python3-gdal gdal-bin ``` For older
-Ubuntu releases you can add the ubuntugis repository to apt prior to
-installation to install version >2.1: ```sh sudo add-apt-repository ppa:
+find the documentation. pyroSAR is/was used in these projects: * [BACI](http://
+www.baci-h2020.eu/index.php/Main/HomePage) * [CCI Biomass](http://cci.esa.int/
+biomass) * [GlobBiomass](http://globbiomass.org/) * [SALDI](https://
+www.saldi.uni-jena.de/) * [SenThIS](https://eos-jena.com/en/projects/) *
+[Sentinel4REDD](https://www.dlr.de/rd/en/Portaldata/28/Resources/dokumente/re/
+Projektblatt_Sentinel4REDD_engl.pdf) * [SWOS](https://www.swos-service.eu/) You
+know of other projects? We'd be happy to know. # Installation First we need to
+install pip. On Windows pip is installed together with Anaconda, on Linux you
+can easily install it via command line: ```sh sudo apt-get install python-pip
+``` The latest stable release of pyroSAR can then be installed: ```sh python -
+m pip install pyroSAR ``` For installation of the latest master branch on
+GitHub, we need the version control system git. On Windows, git can be
+downloaded from [here](https://git-scm.com/downloads). On Linux you can install
+it via command line: ```sh sudo apt-get install git ``` Once everything is set
+up, pyroSAR is ready to be installed: ```sh python -m pip install git+https://
+github.com/johntruckenbrodt/pyroSAR.git ``` # Dependencies If you are using
+Windows, the easiest way to work with pyroSAR and Python in general is by using
+[Anaconda](https://www.anaconda.com/download/). It comes with all basic
+requirements of pyroSAR. The more specific instructions below are intended for
+Linux users. ### GDAL pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as
+dependencies as well as the GDAL Python binding. #### Ubuntu Starting with
+release Yakkety (16.10), Ubuntu comes with GDAL >2.1. See here. You can install
+it like this: ```bash sudo apt-get install python-gdal python3-gdal gdal-bin
+``` For older Ubuntu releases you can add the ubuntugis repository to apt prior
+to installation to install version >2.1: ```sh sudo add-apt-repository ppa:
 ubuntugis/ppa sudo apt-get update ``` This way the required dependencies (GEOS
 and PROJ4 in particular) are also installed. You can check the version by
 typing: ```sh gdalinfo --version ``` #### Debian Starting with Debian 9
 (Stretch) GDAL is available in version >2.1 in the official repository. ####
 Building from source Alternatively, you can build GDAL and the dependencies
 from source. The script `pyroSAR/install/install_deps.sh` gives specific
 instructions on how to do it. It is not yet intended to run this script via
```

### Comparing `pyroSAR-0.9/pyroSAR/drivers.py` & `pyroSAR-0.9.1/pyroSAR/drivers.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/_dev_config.py` & `pyroSAR-0.9.1/pyroSAR/_dev_config.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/gamma/auxil.py` & `pyroSAR-0.9.1/pyroSAR/gamma/auxil.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/gamma/parser_demo.py` & `pyroSAR-0.9.1/pyroSAR/gamma/parser_demo.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/gamma/util.py` & `pyroSAR-0.9.1/pyroSAR/gamma/util.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/gamma/parser.py` & `pyroSAR-0.9.1/pyroSAR/gamma/parser.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/gamma/dem.py` & `pyroSAR-0.9.1/pyroSAR/gamma/dem.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                    DEM2_par=outfile + '.par',
                    DEM2=outfile,
                    bflg=1)
     par2hdr(outfile + '.par', outfile + '.hdr')
 
 
 def dem_autocreate(geometry, demType, outfile, buffer=0.01, t_srs=4326, tr=None, logpath=None,
-                   username=None, password=None, geoid_mode='gamma'):
+                   username=None, password=None, geoid_mode='gamma', resampling_method='bilinear'):
     """
     | automatically create a DEM in Gamma format for a defined spatial geometry
     | the following steps will be performed:
 
     - collect all tiles overlapping with the geometry
 
       * if they don't yet exist locally they will automatically be downloaded
@@ -196,14 +196,17 @@
         see :func:`~pyroSAR.auxdata.dem_autoload`
     password: str or None
         (optional) the password for the registration account
     geoid_mode: str
         the software to be used for converting geoid to ellipsoid heights; does not apply to demType TDX90m; options:
          - 'gamma'
          - 'gdal'
+    resampling_method: str
+        the gdalwarp resampling method; See `here <https://gdal.org/programs/gdalwarp.html#cmdoption-gdalwarp-r>`_
+        for options.
 
     Returns
     -------
 
     """
     
     epsg = crsConvert(t_srs, 'epsg') if t_srs != 4326 else t_srs
@@ -246,15 +249,16 @@
             if geoid_mode == 'gdal':
                 gdal_geoid = True
             elif geoid_mode == 'gamma':
                 gflg = 2
             else:
                 raise RuntimeError("'geoid_mode' not supported")
         
-        dem_create(vrt, dem, t_srs=epsg, tr=tr, geoid_convert=gdal_geoid)
+        dem_create(vrt, dem, t_srs=epsg, tr=tr, geoid_convert=gdal_geoid,
+                   resampling_method=resampling_method)
         
         outfile_tmp = os.path.join(tmpdir, os.path.basename(outfile))
         
         print(message)
         
         if epsg == 4326:
             # old approach for backwards compatibility
```

### Comparing `pyroSAR-0.9/pyroSAR/gamma/dev_S1B.py` & `pyroSAR-0.9.1/pyroSAR/gamma/dev_S1B.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/gamma/error.py` & `pyroSAR-0.9.1/pyroSAR/gamma/error.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/S1/auxil.py` & `pyroSAR-0.9.1/pyroSAR/S1/auxil.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/S1/linesimplify.py` & `pyroSAR-0.9.1/pyroSAR/S1/linesimplify.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/S1/polysimplify.py` & `pyroSAR-0.9.1/pyroSAR/S1/polysimplify.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/S1/dev_bnr.py` & `pyroSAR-0.9.1/pyroSAR/S1/dev_bnr.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/ERS/auxil.py` & `pyroSAR-0.9.1/pyroSAR/ERS/auxil.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/ERS/data/erspasses.db` & `pyroSAR-0.9.1/pyroSAR/ERS/data/erspasses.db`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/datacube_util.py` & `pyroSAR-0.9.1/pyroSAR/datacube_util.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/auxil.py` & `pyroSAR-0.9.1/pyroSAR/snap/auxil.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Subset.xml` & `pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Subset.xml`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Terrain-Flattening.xml` & `pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Terrain-Flattening.xml`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/recipes/nodes/SARSim-Terrain-Correction.xml` & `pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/SARSim-Terrain-Correction.xml`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Terrain-Correction.xml` & `pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Terrain-Correction.xml`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/recipes/nodes/SAR-Simulation.xml` & `pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/SAR-Simulation.xml`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/recipes/nodes/Cross-Correlation.xml` & `pyroSAR-0.9.1/pyroSAR/snap/recipes/nodes/Cross-Correlation.xml`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/recipes/base.xml` & `pyroSAR-0.9.1/pyroSAR/snap/recipes/base.xml`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/util.py` & `pyroSAR-0.9.1/pyroSAR/snap/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..ancillary import multilook_factors
 from .auxil import parse_recipe, parse_node, gpt, groupbyWorkers
 
 from spatialist import crsConvert, Vector, Raster, bbox, intersect
 
 
 def geocode(infile, outdir, t_srs=4326, tr=20, polarizations='all', shapefile=None, scaling='dB',
-            geocoding_type='Range-Doppler', removeS1BoderNoise=True, removeS1ThermalNoise=True, offset=None,
+            geocoding_type='Range-Doppler', removeS1BorderNoise=True, removeS1ThermalNoise=True, offset=None,
             externalDEMFile=None, externalDEMNoDataValue=None, externalDEMApplyEGM=True, terrainFlattening=True,
             basename_extensions=None, test=False, export_extra=None, groupsize=2, cleanup=True,
             gpt_exceptions=None, returnWF=False,
             demResamplingMethod='BILINEAR_INTERPOLATION', imgResamplingMethod='BILINEAR_INTERPOLATION'):
     """
     wrapper function for geocoding SAR images using ESA SNAP
 
@@ -37,15 +37,15 @@
         polarizations e.g. ['VV', 'VH']. Default is 'all'.
     shapefile: str or :py:class:`~spatialist.vector.Vector`, optional
         A vector geometry for subsetting the SAR scene to a test site. Default is None.
     scaling: {'dB', 'db', 'linear'}, optional
         Should the output be in linear or decibel scaling? Default is 'dB'.
     geocoding_type: {'Range-Doppler', 'SAR simulation cross correlation'}, optional
         The type of geocoding applied; can be either 'Range-Doppler' (default) or 'SAR simulation cross correlation'
-    removeS1BoderNoise: bool, optional
+    removeS1BorderNoise: bool, optional
         Enables removal of S1 GRD border noise (default).
     removeS1ThermalNoise: bool, optional
         Enables removal of S1 thermal noise (default).
     offset: tuple, optional
         A tuple defining offsets for left, right, top and bottom in pixels, e.g. (100, 100, 0, 0); this variable is
         overridden if a shapefile is defined. Default is None.
     externalDEMFile: str or None, optional
@@ -179,15 +179,15 @@
     # print('-- configuring Read Node')
     read = workflow['Read']
     read.parameters['file'] = id.scene
     read.parameters['formatName'] = formatName
     ############################################
     # Remove-GRD-Border-Noise node configuration
     # print('-- configuring Remove-GRD-Border-Noise Node')
-    if id.sensor in ['S1A', 'S1B'] and removeS1BoderNoise:
+    if id.sensor in ['S1A', 'S1B'] and removeS1BorderNoise:
         bn = parse_node('Remove-GRD-Border-Noise')
         workflow.insert_node(bn, before='Read')
         bn.parameters['selectedPolarisations'] = polarizations
     ############################################
     # ThermalNoiseRemoval node configuration
     # print('-- configuring ThermalNoiseRemoval Node')
     if id.sensor in ['S1A', 'S1B'] and removeS1ThermalNoise:
```

### Comparing `pyroSAR-0.9/pyroSAR/snap/dev_process.py` & `pyroSAR-0.9.1/pyroSAR/snap/dev_process.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/data/snap.auxdata.properties` & `pyroSAR-0.9.1/pyroSAR/snap/data/snap.auxdata.properties`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/snap/dev_split.py` & `pyroSAR-0.9.1/pyroSAR/snap/dev_split.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/dev_auxdata_david.py` & `pyroSAR-0.9.1/pyroSAR/dev_auxdata_david.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/ancillary.py` & `pyroSAR-0.9.1/pyroSAR/ancillary.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR/auxdata.py` & `pyroSAR-0.9.1/pyroSAR/auxdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                             username=username,
                             password=password,
                             vrt=vrt,
                             buffer=buffer,
                             product=product)
 
 
-def dem_create(src, dst, t_srs=None, tr=None, geoid_convert=False, geoid='EGM96'):
+def dem_create(src, dst, t_srs=None, tr=None, resampling_method='bilinear', geoid_convert=False, geoid='EGM96'):
     """
     create a new DEM GeoTiff file and optionally convert heights from geoid to ellipsoid
     
     Parameters
     ----------
     src: str
         the input dataset, e.g. a VRT from function :func:`dem_autoload`
@@ -150,14 +150,17 @@
         the output dataset
     t_srs: None, int, str or osr.SpatialReference
         A target geographic reference system in WKT, EPSG, PROJ4 or OPENGIS format.
         See function :func:`spatialist.auxil.crsConvert()` for details.
         Default (None): use the crs of ``src``.
     tr: None or tuple
         the target resolution as (xres, yres)
+    resampling_method: str
+        the gdalwarp resampling method; See `here <https://gdal.org/programs/gdalwarp.html#cmdoption-gdalwarp-r>`_
+        for options.
     geoid_convert: bool
         convert geoid heights?
     geoid: str
         the geoid model to be corrected, only used if ``geoid_convert == True``; current options:
          * 'EGM96'
 
     Returns
@@ -173,15 +176,17 @@
         epsg_out = epsg_in
     else:
         epsg_out = crsConvert(t_srs, 'epsg')
     
     gdalwarp_args = {'format': 'GTiff', 'multithread': True,
                      'srcNodata': nodata, 'dstNodata': nodata,
                      'srcSRS': 'EPSG:{}'.format(epsg_in),
-                     'dstSRS': 'EPSG:{}'.format(epsg_out)}
+                     'dstSRS': 'EPSG:{}'.format(epsg_out),
+                     'resampleAlg': resampling_method}
+    
     if tr is not None:
         gdalwarp_args.update({'xRes': tr[0],
                               'yRes': tr[1]})
     
     if geoid_convert:
         if gdal.__version__ < '2.2':
             raise RuntimeError('geoid conversion requires GDAL >= 2.2;'
```

### Comparing `pyroSAR-0.9/pyroSAR/xml_util.py` & `pyroSAR-0.9.1/pyroSAR/xml_util.py`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR.egg-info/SOURCES.txt` & `pyroSAR-0.9.1/pyroSAR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroSAR-0.9/pyroSAR.egg-info/PKG-INFO` & `pyroSAR-0.9.1/pyroSAR.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroSAR
-Version: 0.9
+Version: 0.9.1
 Summary: a framework for large-scale SAR satellite data processing
 Home-page: https://github.com/johntruckenbrodt/pyroSAR.git
 Author: John Truckenbrodt
 Author-email: john.truckenbrodt@uni-jena.de
 License: MIT
 Description: <h1 align="center">
           <br>
@@ -38,36 +38,52 @@
         * Reading of data from various past and present satellite missions
         * Handling of acquisition metadata
         * User-friendly access to processing utilities in SNAP and GAMMA Remote Sensing software
         * Formatting of the preprocessed data for further analysis
         
         [Here](https://pyrosar.readthedocs.io/en/latest/?badge=latest) you can find the documentation.
         
+        pyroSAR is/was used in these projects:
+        * [BACI](http://www.baci-h2020.eu/index.php/Main/HomePage)
+        * [CCI Biomass](http://cci.esa.int/biomass)
+        * [GlobBiomass](http://globbiomass.org/)
+        * [SALDI](https://www.saldi.uni-jena.de/)
+        * [SenThIS](https://eos-jena.com/en/projects/)
+        * [Sentinel4REDD](https://www.dlr.de/rd/en/Portaldata/28/Resources/dokumente/re/Projektblatt_Sentinel4REDD_engl.pdf)
+        * [SWOS](https://www.swos-service.eu/)
+        
+        You know of other projects? We'd be happy to know.
+        
         # Installation
-        For the installation we need the Python tool pip and the version control system git. On Windows pip is 
-        installed together with Anaconda, git can be downloaded from [here](https://git-scm.com/downloads).
-        On Linux you can easily install both via command line:
+        First we need to install pip. On Windows pip is installed together with Anaconda, on Linux you can easily install it
+         via command line:
         ```sh
         sudo apt-get install python-pip
+        ```
+        The latest stable release of pyroSAR can then be installed:
+        ```sh
+        python -m pip install pyroSAR
+        ```
+        
+        For installation of the latest master branch on GitHub, we need the version control system git. On Windows, git can be 
+        downloaded from [here](https://git-scm.com/downloads). On Linux you can install it via command line:
+        ```sh
         sudo apt-get install git
         ```
         Once everything is set up, pyroSAR is ready to be installed:
         ```sh
-        sudo pip install git+https://github.com/johntruckenbrodt/pyroSAR.git
+        python -m pip install git+https://github.com/johntruckenbrodt/pyroSAR.git
         ```
-        On Windows you need to use the Anaconda Prompt and leave out `sudo` in the above command.
         
         # Dependencies
         If you are using Windows, the easiest way to work with pyroSAR and Python in general is by using 
         [Anaconda](https://www.anaconda.com/download/). It comes with all basic requirements of pyroSAR.
         The more specific instructions below are intended for Linux users.
         ### GDAL
-        pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as dependencies as well as the GDAL Python binding. 
-        Alternatively, one can use <a href="https://github.com/nextgis/pygdal">pygdal</a>, 
-        a virtualenv and setuptools friendly version of standard GDAL python bindings.
+        pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as dependencies as well as the GDAL Python binding.
         #### Ubuntu
         Starting with release Yakkety (16.10), Ubuntu comes with GDAL >2.1. 
         See <a href="https://launchpad.net/ubuntu/yakkety/amd64/gdal-bin">here</a>. 
         You can install it like this:
         ```bash
         sudo apt-get install python-gdal python3-gdal gdal-bin
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyroSAR Version: 0.9 Summary: a framework for
+Metadata-Version: 2.1 Name: pyroSAR Version: 0.9.1 Summary: a framework for
 large-scale SAR satellite data processing Home-page: https://github.com/
 johntruckenbrodt/pyroSAR.git Author: John Truckenbrodt Author-email:
 john.truckenbrodt@uni-jena.de License: MIT Description:
                                     ******
                                 pyroSAR ******
   **** A Python Framework for Large-Scale SAR Satellite Data Processing ****
 Description â¢ Installation â¢ Dependencies â¢ Example â¢ Notes â¢ Authors
@@ -10,33 +10,39 @@
  [Appveyor_Status] [Coveralls_Status] [Documentation_Status] [PIP_Status]
 # Description The pyroSAR package aims at providing a complete solution for the
 scalable organization and processing of SAR satellite data: * Reading of data
 from various past and present satellite missions * Handling of acquisition
 metadata * User-friendly access to processing utilities in SNAP and GAMMA
 Remote Sensing software * Formatting of the preprocessed data for further
 analysis [Here](https://pyrosar.readthedocs.io/en/latest/?badge=latest) you can
-find the documentation. # Installation For the installation we need the Python
-tool pip and the version control system git. On Windows pip is installed
-together with Anaconda, git can be downloaded from [here](https://git-scm.com/
-downloads). On Linux you can easily install both via command line: ```sh sudo
-apt-get install python-pip sudo apt-get install git ``` Once everything is set
-up, pyroSAR is ready to be installed: ```sh sudo pip install git+https://
-github.com/johntruckenbrodt/pyroSAR.git ``` On Windows you need to use the
-Anaconda Prompt and leave out `sudo` in the above command. # Dependencies If
-you are using Windows, the easiest way to work with pyroSAR and Python in
-general is by using [Anaconda](https://www.anaconda.com/download/). It comes
-with all basic requirements of pyroSAR. The more specific instructions below
-are intended for Linux users. ### GDAL pyroSAR requires GDAL version 2.1 with
-GEOS and PROJ4 as dependencies as well as the GDAL Python binding.
-Alternatively, one can use pygdal, a virtualenv and setuptools friendly version
-of standard GDAL python bindings. #### Ubuntu Starting with release Yakkety
-(16.10), Ubuntu comes with GDAL >2.1. See here. You can install it like this:
-```bash sudo apt-get install python-gdal python3-gdal gdal-bin ``` For older
-Ubuntu releases you can add the ubuntugis repository to apt prior to
-installation to install version >2.1: ```sh sudo add-apt-repository ppa:
+find the documentation. pyroSAR is/was used in these projects: * [BACI](http://
+www.baci-h2020.eu/index.php/Main/HomePage) * [CCI Biomass](http://cci.esa.int/
+biomass) * [GlobBiomass](http://globbiomass.org/) * [SALDI](https://
+www.saldi.uni-jena.de/) * [SenThIS](https://eos-jena.com/en/projects/) *
+[Sentinel4REDD](https://www.dlr.de/rd/en/Portaldata/28/Resources/dokumente/re/
+Projektblatt_Sentinel4REDD_engl.pdf) * [SWOS](https://www.swos-service.eu/) You
+know of other projects? We'd be happy to know. # Installation First we need to
+install pip. On Windows pip is installed together with Anaconda, on Linux you
+can easily install it via command line: ```sh sudo apt-get install python-pip
+``` The latest stable release of pyroSAR can then be installed: ```sh python -
+m pip install pyroSAR ``` For installation of the latest master branch on
+GitHub, we need the version control system git. On Windows, git can be
+downloaded from [here](https://git-scm.com/downloads). On Linux you can install
+it via command line: ```sh sudo apt-get install git ``` Once everything is set
+up, pyroSAR is ready to be installed: ```sh python -m pip install git+https://
+github.com/johntruckenbrodt/pyroSAR.git ``` # Dependencies If you are using
+Windows, the easiest way to work with pyroSAR and Python in general is by using
+[Anaconda](https://www.anaconda.com/download/). It comes with all basic
+requirements of pyroSAR. The more specific instructions below are intended for
+Linux users. ### GDAL pyroSAR requires GDAL version 2.1 with GEOS and PROJ4 as
+dependencies as well as the GDAL Python binding. #### Ubuntu Starting with
+release Yakkety (16.10), Ubuntu comes with GDAL >2.1. See here. You can install
+it like this: ```bash sudo apt-get install python-gdal python3-gdal gdal-bin
+``` For older Ubuntu releases you can add the ubuntugis repository to apt prior
+to installation to install version >2.1: ```sh sudo add-apt-repository ppa:
 ubuntugis/ppa sudo apt-get update ``` This way the required dependencies (GEOS
 and PROJ4 in particular) are also installed. You can check the version by
 typing: ```sh gdalinfo --version ``` #### Debian Starting with Debian 9
 (Stretch) GDAL is available in version >2.1 in the official repository. ####
 Building from source Alternatively, you can build GDAL and the dependencies
 from source. The script `pyroSAR/install/install_deps.sh` gives specific
 instructions on how to do it. It is not yet intended to run this script via
```

### Comparing `pyroSAR-0.9/setup.py` & `pyroSAR-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 else:
     with open(os.path.join(directory, 'README.md')) as f:
         long_description = f.read()
 
 setup(name='pyroSAR',
       packages=find_packages(),
       include_package_data=True,
-      version='0.9',
+      version='0.9.1',
       description='a framework for large-scale SAR satellite data processing',
       classifiers=[
           'License :: OSI Approved :: MIT License',
           'Operating System :: Microsoft :: Windows',
           'Operating System :: POSIX :: Linux',
           'Programming Language :: Python',
       ],
```

