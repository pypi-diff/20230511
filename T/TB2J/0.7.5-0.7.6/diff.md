# Comparing `tmp/TB2J-0.7.5.tar.gz` & `tmp/TB2J-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.7.5.tar", last modified: Tue May  9 15:34:38 2023, max compression
+gzip compressed data, was "TB2J-0.7.6.tar", last modified: Wed May 10 13:11:09 2023, max compression
```

## Comparing `TB2J-0.7.5.tar` & `TB2J-0.7.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1327 2023-05-09 15:15:14.000000 TB2J-0.7.5/LICENSE
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2023-05-09 15:34:38.145051 TB2J-0.7.5/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     1902 2023-05-09 15:15:38.000000 TB2J-0.7.5/README.md
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/
--rw-r--r--   0 hexu      (1032) phythema   (500)     7121 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/Jdownfolder.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1771 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/Jtensor.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3994 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/Oiju.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7423 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/Oiju_epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       22 2023-05-09 15:34:33.000000 TB2J-0.7.5/TB2J/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2884 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/citation.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2489 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/contour.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3518 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    29412 2023-05-09 15:33:43.000000 TB2J-0.7.5/TB2J/exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11701 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/exchangeCL2.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8372 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/exchange_pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9017 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/exchange_qspace.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/external/
--rw-r--r--   0 hexu      (1032) phythema   (500)      137 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/external/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5943 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/external/p_tqdm.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6630 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/gpaw_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    12286 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/green.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1571 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/greentest.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/io_exchange/
--rw-r--r--   0 hexu      (1032) phythema   (500)       32 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    16870 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/io_exchange/io_exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6720 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_multibinit.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4024 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_tomsasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10198 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_txt.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3190 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_exchange/io_uppasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5639 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/io_exchange/io_vampire.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6921 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/io_merge.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      533 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/kpoints.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    18356 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/manager.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    17974 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/myTB.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4756 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/orbmap.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/pauli.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1223 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1435 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/plot.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1126 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/rotate_atoms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11639 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/sisl_wrapper.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/spinham/
--rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.7.5/TB2J/spinham/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2234 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/base_parser.py
--rw-rw-r--   0 hexu      (1032) phythema   (500)      741 2020-07-08 14:12:19.000000 TB2J-0.7.5/TB2J/spinham/constants.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    13323 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/spinham/hamiltonian.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9870 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/hamiltonian_terms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7011 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/plot.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2215 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/spinham/qsolver.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2238 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/spin_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10923 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/spinham/spin_xml.py
--rw-rw-r--   0 hexu      (1032) phythema   (500)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.5/TB2J/spinham/supercell.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3896 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/utest.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9358 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/utils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      276 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/versioninfo.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J/wannier/
--rw-r--r--   0 hexu      (1032) phythema   (500)       70 2023-05-09 15:15:14.000000 TB2J-0.7.5/TB2J/wannier/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:38.000000 TB2J-0.7.5/TB2J/wannier/w90_parser.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/TB2J.egg-info/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     1367 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        1 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)       68 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/requires.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        5 2023-05-09 15:34:38.000000 TB2J-0.7.5/TB2J.egg-info/top_level.txt
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-09 15:34:38.145051 TB2J-0.7.5/scripts/
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     2160 2023-05-09 15:15:38.000000 TB2J-0.7.5/scripts/TB2J_downfold.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1186 2023-05-09 15:15:38.000000 TB2J-0.7.5/scripts/TB2J_eigen.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3379 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/TB2J_magnon.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1475 2023-05-09 15:15:38.000000 TB2J-0.7.5/scripts/TB2J_merge.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      715 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/TB2J_rotate.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     5083 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/siesta2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     7092 2023-05-09 15:15:14.000000 TB2J-0.7.5/scripts/wann2J.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       38 2023-05-09 15:34:38.145051 TB2J-0.7.5/setup.cfg
--rw-r--r--   0 hexu      (1032) phythema   (500)     1785 2023-05-09 15:34:15.000000 TB2J-0.7.5/setup.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1327 2023-05-09 15:15:14.000000 TB2J-0.7.6/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2023-05-10 13:11:09.344772 TB2J-0.7.6/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1902 2023-05-09 15:15:38.000000 TB2J-0.7.6/README.md
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/TB2J/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7121 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/Jdownfolder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1771 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/Jtensor.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3994 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/Oiju.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7423 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/Oiju_epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       22 2023-05-10 13:04:21.000000 TB2J-0.7.6/TB2J/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2884 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/citation.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2489 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/contour.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3518 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    29406 2023-05-09 16:31:10.000000 TB2J-0.7.6/TB2J/exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11701 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/exchangeCL2.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8372 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/exchange_pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9017 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/exchange_qspace.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/TB2J/external/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      137 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/external/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5943 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/external/p_tqdm.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6630 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/gpaw_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12286 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/green.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1571 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/greentest.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/TB2J/io_exchange/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       32 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/io_exchange/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16870 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/io_exchange/io_exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6720 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/io_exchange/io_multibinit.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4024 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/io_exchange/io_tomsasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10198 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/io_exchange/io_txt.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3190 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/io_exchange/io_uppasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5639 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/io_exchange/io_vampire.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6921 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/io_merge.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      533 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/kpoints.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    18356 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/manager.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    17974 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/myTB.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4756 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/orbmap.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/pauli.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1223 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1435 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/plot.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1126 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/rotate_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11639 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/sisl_wrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/TB2J/spinham/
+-rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.7.6/TB2J/spinham/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2234 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/spinham/base_parser.py
+-rw-rw-r--   0 hexu      (1032) phythema   (500)      741 2020-07-08 14:12:19.000000 TB2J-0.7.6/TB2J/spinham/constants.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16532 2023-05-10 13:00:19.000000 TB2J-0.7.6/TB2J/spinham/hamiltonian.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9870 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/spinham/hamiltonian_terms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7011 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/spinham/plot.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2215 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/spinham/qsolver.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2238 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/spinham/spin_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10923 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/spinham/spin_xml.py
+-rw-rw-r--   0 hexu      (1032) phythema   (500)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.6/TB2J/spinham/supercell.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3896 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/utest.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9358 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      276 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/versioninfo.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/TB2J/wannier/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       70 2023-05-09 15:15:14.000000 TB2J-0.7.6/TB2J/wannier/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4092 2023-05-09 15:15:38.000000 TB2J-0.7.6/TB2J/wannier/w90_parser.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/TB2J.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2023-05-10 13:11:09.000000 TB2J-0.7.6/TB2J.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1367 2023-05-10 13:11:09.000000 TB2J-0.7.6/TB2J.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2023-05-10 13:11:09.000000 TB2J-0.7.6/TB2J.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)       68 2023-05-10 13:11:09.000000 TB2J-0.7.6/TB2J.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        5 2023-05-10 13:11:09.000000 TB2J-0.7.6/TB2J.egg-info/top_level.txt
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2023-05-10 13:11:09.344772 TB2J-0.7.6/scripts/
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     2160 2023-05-09 15:15:38.000000 TB2J-0.7.6/scripts/TB2J_downfold.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1186 2023-05-09 15:15:38.000000 TB2J-0.7.6/scripts/TB2J_eigen.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3415 2023-05-10 13:02:58.000000 TB2J-0.7.6/scripts/TB2J_magnon.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1475 2023-05-09 15:15:38.000000 TB2J-0.7.6/scripts/TB2J_merge.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      715 2023-05-09 15:15:14.000000 TB2J-0.7.6/scripts/TB2J_rotate.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     5083 2023-05-09 15:15:14.000000 TB2J-0.7.6/scripts/siesta2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     7092 2023-05-09 15:15:14.000000 TB2J-0.7.6/scripts/wann2J.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2023-05-10 13:11:09.344772 TB2J-0.7.6/setup.cfg
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1785 2023-05-10 13:04:10.000000 TB2J-0.7.6/setup.py
```

### Comparing `TB2J-0.7.5/LICENSE` & `TB2J-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/PKG-INFO` & `TB2J-0.7.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.5
+Version: 0.7.6
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.5/README.md` & `TB2J-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/Jdownfolder.py` & `TB2J-0.7.6/TB2J/Jdownfolder.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/Jtensor.py` & `TB2J-0.7.6/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/Oiju.py` & `TB2J-0.7.6/TB2J/Oiju.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/Oiju_epc.py` & `TB2J-0.7.6/TB2J/Oiju_epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/citation.py` & `TB2J-0.7.6/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/contour.py` & `TB2J-0.7.6/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/epc.py` & `TB2J-0.7.6/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/exchange.py` & `TB2J-0.7.6/TB2J/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             if iatom not in self.orb_dict:
                 raise ValueError(
                     f"""Cannot find any orbital for atom {iatom}, which is supposed to be magnetic. Please check the Wannier functions."""
                 )
         if not self._is_collinear:
             for iatom, orb in self.orb_dict.items():
                 nsorb = len(self.orb_dict[iatom])
-                if and (nsorb % 2 != 0):
+                if nsorb % 2 != 0:
                     raise ValueError(
                         f"""The number of spin-orbitals for atom {iatom} is not even,
 {nsorb} spin-orbitals are found near this atom.
 which means the spin up/down does not have same number of orbitals. 
 This is often because the Wannier functions are wrongly defined,
 or badly localized. Please check the Wannier centers in the Wannier90 output file. 
 """)
```

### Comparing `TB2J-0.7.5/TB2J/exchangeCL2.py` & `TB2J-0.7.6/TB2J/exchangeCL2.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/exchange_pert.py` & `TB2J-0.7.6/TB2J/exchange_pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/exchange_qspace.py` & `TB2J-0.7.6/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/external/p_tqdm.py` & `TB2J-0.7.6/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/gpaw_wrapper.py` & `TB2J-0.7.6/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/green.py` & `TB2J-0.7.6/TB2J/green.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/greentest.py` & `TB2J-0.7.6/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/io_exchange/io_exchange.py` & `TB2J-0.7.6/TB2J/io_exchange/io_exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.7.6/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.7.6/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/io_exchange/io_txt.py` & `TB2J-0.7.6/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.7.6/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/io_exchange/io_vampire.py` & `TB2J-0.7.6/TB2J/io_exchange/io_vampire.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/io_merge.py` & `TB2J-0.7.6/TB2J/io_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/kpoints.py` & `TB2J-0.7.6/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/manager.py` & `TB2J-0.7.6/TB2J/manager.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/myTB.py` & `TB2J-0.7.6/TB2J/myTB.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/orbmap.py` & `TB2J-0.7.6/TB2J/orbmap.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/pauli.py` & `TB2J-0.7.6/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/pert.py` & `TB2J-0.7.6/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/plot.py` & `TB2J-0.7.6/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/rotate_atoms.py` & `TB2J-0.7.6/TB2J/rotate_atoms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/sisl_wrapper.py` & `TB2J-0.7.6/TB2J/sisl_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/base_parser.py` & `TB2J-0.7.6/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/constants.py` & `TB2J-0.7.6/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/hamiltonian.py` & `TB2J-0.7.6/TB2J/spinham/hamiltonian.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,121 @@
 #!/usr/bin/env python
 import numpy as np
 from collections.abc import Iterable
 from collections import defaultdict
 import matplotlib.pyplot as plt
 from ase.dft.kpoints import bandpath, monkhorst_pack
-from .hamiltonian_terms import (ZeemanTerm, UniaxialMCATerm, ExchangeTerm,
-                                DMITerm, BilinearTerm)
+from .hamiltonian_terms import (
+    ZeemanTerm,
+    UniaxialMCATerm,
+    ExchangeTerm,
+    DMITerm,
+    BilinearTerm,
+)
 from .constants import mu_B, gyromagnetic_ratio
 from .supercell import SupercellMaker
 from .spin_xml import SpinXmlParser, SpinXmlWriter
 from .plot import group_band_path
 from ase.cell import Cell
 from .qsolver import QSolver
+import json
 
 
+class NumpyEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, np.ndarray):
+            return obj.tolist()
+        return json.JSONEncoder.default(self, obj)
+
+plot_script="""\
+#!/usr/bin/env python
+\"\"\"
+Parse the json file generated by the magnon band calculation. 
+And plot the magnon band structure from the json file. 
+You can modify this file to plot the magnon band structure, all plot 
+multiple magnon band structures in one figure.
+\"\"\"
+import numpy as np
+import matplotlib.pyplot as plt
+import json
+
+def load_magnon_json(filename):
+    \"\"\"
+    Load the magnon band structure from the json file.
+    args:
+        filename: the json file generated by the magnon band calculation.
+    return:
+        kptlist: all the kpoints
+        xlist: the x coordinates of the kpoints in the plot
+        knames: names of the high symmetry points
+        Xs: The x coordinates of the high symmetry points in the plot
+        allevals: eigenvalues, in meV
+            Note that the eigenvalues are splitted into groups of kpoints.
+            the first index is the index of the group of kpoints
+            the second index is the index of the kpoint in the group 
+            the third index is the index of the band
+    \"\"\"
+    with open(filename) as f:
+        data = json.load(f)
+    kptlist = data["kptlist"]
+    xlist = data["xlist"]
+    knames = data["knames"]
+    Xs = data["X_for_highsym_kpoints"]
+    allevals = np.array(data["evals"])
+    return kptlist, xlist, knames, Xs, allevals
+
+def plot_magnon_json(filename, ax, color="k", show=True):
+    \"\"\"
+    Plot the magnon band structure from the json file.
+    args:
+        filename: the json file generated by the magnon band calculation.
+        ax: the matplotlib ax to plot the band structure.
+            If None, a new figure will be created.
+        color: the color of the band structure.
+        show: whether to show the plot. 
+    \"\"\"
+    if ax is None:
+        fig, ax = plt.subplots()
+
+    kptlist, xlist, knames, Xs, allevals = load_magnon_json(filename)
+    for i, (kpts, xs) in enumerate(zip(kptlist, xlist)):
+        evals=allevals[i]
+        # Plot band structure
+        nbands = evals.shape[1]
+        emin = np.min(evals[:, 0])
+        for i in range(nbands):
+            ax.plot(xs, (evals[:, i]) / 1.6e-22, color=color)
+
+    ax.set_ylabel("Energy (meV)")
+    ax.set_xlim(xlist[0][0], xlist[-1][-1])
+    ax.set_xticks(Xs)
+    knames = [x if x != "G" else "$\Gamma$" for x in knames]
+    ax.set_xticklabels(knames)
+    for x in Xs:
+        ax.axvline(x, linewidth=0.6, color="gray")
+    if show:
+        plt.show()
+
+
+if __name__ == "__main__":
+    plot_magnon_json("magnon_band.json", ax=None, color="k", show=True)
+
+"""
+
 class SpinHamiltonian(object):
-    def __init__(self,
-                 cell=None,
-                 pos=None,
-                 xcart=None,
-                 spinat=None,
-                 zion=None,
-                 Rlist=None,
-                 iprim=None):
+    def __init__(
+        self,
+        cell=None,
+        pos=None,
+        xcart=None,
+        spinat=None,
+        zion=None,
+        Rlist=None,
+        iprim=None,
+    ):
         if xcart is None:
             self.xcart = np.dot(pos, cell)
             self.pos = pos
         elif pos is None:
             self.pos = np.dot(xcart, np.linalg.inv(cell))
             self.xcart = xcart
         self.cell = cell
@@ -36,15 +125,15 @@
 
         self._spin = np.array(spinat) * mu_B
         self._map_to_magnetic_only()
         # spin interaction parameters
 
         # Homogeneous H eff_field
         self.has_external_hfield = False
-        self.zeeman_H = np.zeros(3, dtype='float64')
+        self.zeeman_H = np.zeros(3, dtype="float64")
 
         # uniaxial single ion anisotropy
         self.has_uniaxial_anisotropy = False
 
         # cubic Anistropy (Not implemented yet)
         self.has_cubic_anistropy = False
 
@@ -106,33 +195,39 @@
         # self.S = np.array(
         #    [S[i] / self.ms[i] for i in range(self.nspin)],
         #    dtype='float64')
         self.s = S / self.ms[:, None]
 
     @property
     def spin(self):
-        self._spin[self.magsites] = np.multiply(self.ms[:, np.newaxis],
-                                                self.s) / mu_B
+        self._spin[self.magsites] = np.multiply(self.ms[:, np.newaxis], self.s) / mu_B
         return self._spin
 
     @spin.setter
     def spin(self, spin):
         self._spin = np.array(spin) * mu_B
         self._map_to_magnetic_only()
 
     def normalize_S(self):
         """
         normalize so the norm of self.S[i] is 1
         """
         snorm = np.linalg.norm(self.s, axis=1)
         self.s /= np.expand_dims(snorm, axis=1)
 
-    def set(self, gilbert_damping=None, gyro_ratio=None,
-            has_exchange=None, has_dmi=None, has_bilinear=None,
-            has_external_hfield=None, has_uniaxial_anisotropy=None):
+    def set(
+        self,
+        gilbert_damping=None,
+        gyro_ratio=None,
+        has_exchange=None,
+        has_dmi=None,
+        has_bilinear=None,
+        has_external_hfield=None,
+        has_uniaxial_anisotropy=None,
+    ):
         """
         set parameters for simulation:
         args:
         ====================
         timestep: in ps
         temperature: in K, default 0K.
         damping factor: Gilbert damping factor, default: 0.01
@@ -142,41 +237,43 @@
             self.gilbert_damping = np.array(gilbert_damping)
         if gyro_ratio is not None:
             self.gyro_ratio = np.array(gyro_ratio)
         self.has_exchange = self.has_exchange and bool(has_exchange)
         self.has_dmi = self.has_dmi and bool(has_dmi)
         self.has_bilinear = self.has_bilinear and bool(has_bilinear)
         self.has_external_hfield = self.has_external_hfield and bool(
-            has_external_hfield)
+            has_external_hfield
+        )
         self.has_uniaxial_anisotropy = self.has_uniaxial_anisotropy and bool(
-            has_uniaxial_anisotropy)
+            has_uniaxial_anisotropy
+        )
 
     def set_exchange_ijR(self, exchange_Jdict):
         """
         J: [(i,j, R, J_{ijR})] J_{ijR} is a scalar
         """
         self.has_exchange = True
         self.exchange_Jdict = exchange_Jdict
         exchange = ExchangeTerm(self.exchange_Jdict, ms=self.ms)
-        self.hamiltonians['exchange'] = exchange
+        self.hamiltonians["exchange"] = exchange
 
     def set_dmi_ijR(self, dmi_ddict):
         """
         D: [(i,j, R, D_{ijR})], D_{ijR} is a vector
         """
         self.has_dmi = True
         self.dmi_ddict = dmi_ddict
         DMI = DMITerm(self.dmi_ddict, self.ms)
-        self.hamiltonians['DMI'] = DMI
+        self.hamiltonians["DMI"] = DMI
 
     def set_bilinear_ijR(self, bilinear_dict):
         self.has_bilinear = True
         self.bilinear_dict = bilinear_dict
         Bi = BilinearTerm(self.bilinear_dict, self.ms)
-        self.hamiltonians['Bilinear'] = Bi
+        self.hamiltonians["Bilinear"] = Bi
 
     def set_dipdip(self):
         """
         add the dipole dipole interaction term.
         """
 
     def set_external_hfield(self, H):
@@ -186,35 +283,36 @@
         """
         self.has_external_hfield = True
         if isinstance(H, Iterable):
             self.H_ext = np.asarray(H)
         else:
             self.H_ext = np.ones([self.nspin, 3]) * H
         zeeman = ZeemanTerm(H=self.H_ext, ms=self.ms)
-        self.hamiltonians['zeeman'] = zeeman
+        self.hamiltonians["zeeman"] = zeeman
 
     def set_uniaxial_mca(self, k1, k1dir):
         """
         Add homogenoues uniaxial anisotropy
         """
         self.has_uniaxial_anisotropy = True
 
         self.k1 = k1
         self.k1dir = k1dir
         umcaterm = UniaxialMCATerm(k1, k1dir, ms=self.ms)
-        self.hamiltonians['UMCA'] = umcaterm
+        self.hamiltonians["UMCA"] = umcaterm
 
     def add_Hamiltonian_term(self, Hamiltonian_term, name=None):
         """
         add Hamiltonian term which is not pre_defined.
         """
         if name in self.hamiltonians:
             raise ValueError(
-                'Hamiltonian name %s already defined. The defined names are %s'
-                % (name, self.hamiltonians.keys()))
+                "Hamiltonian name %s already defined. The defined names are %s"
+                % (name, self.hamiltonians.keys())
+            )
         else:
             self.hamiltonians[name] = Hamiltonian_term
 
     # @profile
     def get_effective_field(self, S):
         """
         calculate the effective field Heff=-1/ms * \partial H / \partial S
@@ -239,56 +337,54 @@
             smaker.sc_trans_invariant(self.index_spin)
 
         sc_Rlist = np.repeat(smaker.R_sc, self.nspin, axis=0)
         sc_iprim = smaker.sc_trans_invariant(list(range(self.nspin)))
 
         sc_spinat = np.array(smaker.sc_trans_invariant(self.spinat))
 
-        sc_ham = SpinHamiltonian(cell=sc_cell,
-                                 pos=sc_pos,
-                                 spinat=sc_spinat,
-                                 zion=sc_zion,
-                                 Rlist=sc_Rlist,
-                                 iprim=sc_iprim)
+        sc_ham = SpinHamiltonian(
+            cell=sc_cell,
+            pos=sc_pos,
+            spinat=sc_spinat,
+            zion=sc_zion,
+            Rlist=sc_Rlist,
+            iprim=sc_iprim,
+        )
 
         sc_gyro_ratio = np.array(smaker.sc_trans_invariant(self.gyro_ratio))
         sc_ham.gyro_ratio = sc_gyro_ratio
 
-        sc_gilbert_damping = np.array(
-            smaker.sc_trans_invariant(self.gilbert_damping))
+        sc_gilbert_damping = np.array(smaker.sc_trans_invariant(self.gilbert_damping))
         sc_ham.gilbert_damping = sc_gilbert_damping
 
         if self.has_external_hfield:
             sc_Hext = smaker.sc_trans_invariant(self.H_ext)
             sc_ham.set_external_hfield(sc_Hext)
 
         if self.has_uniaxial_anisotropy:
             sc_k1 = smaker.sc_trans_invariant(self.k1)
             sc_k1dir = smaker.sc_trans_invariant(self.k1dir)
             sc_ham.set_uniaxial_mca(sc_k1, np.array(sc_k1dir))
 
         if self.has_exchange:
-            sc_Jdict = smaker.sc_ijR(self.exchange_Jdict,
-                                     n_basis=len(self.pos))
+            sc_Jdict = smaker.sc_ijR(self.exchange_Jdict, n_basis=len(self.pos))
             sc_ham.set_exchange_ijR(exchange_Jdict=sc_Jdict)
 
         if self.has_dmi:
             sc_dmi_ddict = smaker.sc_ijR(self.dmi_ddict, n_basis=len(self.pos))
             sc_ham.set_dmi_ijR(sc_dmi_ddict)
 
         if self.has_bilinear:
-            sc_bilinear_dict = smaker.sc_ijR(self.bilinear_dict,
-                                             n_basis=len(self.pos))
+            sc_bilinear_dict = smaker.sc_ijR(self.bilinear_dict, n_basis=len(self.pos))
             sc_ham.set_bilinear_ijR(sc_bilinear_dict)
 
         return sc_ham
 
     def calc_total_HijR(self):
-        self._total_hessian_ijR = defaultdict(lambda: np.zeros(
-            (3, 3), dtype=float))
+        self._total_hessian_ijR = defaultdict(lambda: np.zeros((3, 3), dtype=float))
         for tname, term in self.hamiltonians.items():
             if term.is_twobody_term():
                 for key, val in term.hessian_ijR().items():
                     self._total_hessian_ijR[key] += val
         return self._total_hessian_ijR
 
     def get_total_hessian_ijR(self):
@@ -303,28 +399,30 @@
         qsolver = QSolver(hamiltonian=self)
         evals, evecs = qsolver.solve_all(kpts, eigen_vectors=True, Jq=Jq)
         return evals, evecs
 
     def find_ground_state_from_kmesh(self, kmesh, myfile):
         kpts = monkhorst_pack(kmesh)
         evals, evecs = self.solve_k(kpts, Jq=True)
-        #write_magnon_info(self, kpts, evals, evecs, myfile)
+        # write_magnon_info(self, kpts, evals, evecs, myfile)
 
-    def plot_magnon_band(self,
-                         kvectors=np.array([[0, 0, 0], [0.5, 0, 0],
-                                            [0.5, 0.5, 0], [0, 0, 0],
-                                            [.5, .5, .5]]),
-                         knames=['$\Gamma$', 'X', 'M', '$\Gamma$', 'R'],
-                         supercell_matrix=None,
-                         npoints=50,
-                         color='red',
-                         kpath_fname=None,
-                         Jq=False,
-                         ax=None,
-                         ):
+    def plot_magnon_band(
+        self,
+        kvectors=np.array(
+            [[0, 0, 0], [0.5, 0, 0], [0.5, 0.5, 0], [0, 0, 0], [0.5, 0.5, 0.5]]
+        ),
+        knames=["$\Gamma$", "X", "M", "$\Gamma$", "R"],
+        supercell_matrix=None,
+        npoints=50,
+        color="red",
+        kpath_fname=None,
+        Jq=False,
+        ax=None,
+        output_fname="magnon_band.json",
+    ):
         if ax is None:
             fig, ax = plt.subplots()
         kptlist = kvectors
         if knames is None and kvectors is None:
             # fully automatic k-path
             bp = Cell(self.cell).bandpath(npoints=npoints)
             spk = bp.special_points
@@ -342,48 +440,77 @@
             xlist = [x]
             kptlist = [kpts]
 
         if supercell_matrix is not None:
             kptlist = [np.dot(k, supercell_matrix) for k in kptlist]
         print("High symmetry k-points:")
         for name, k in spk.items():
-            if name == 'G':
-                name = 'Gamma'
+            if name == "G":
+                name = "Gamma"
             print(f"{name}: {k}")
 
+        allevals=[]
         for kpts, xs in zip(kptlist, xlist):
             evals, evecs = self.solve_k(kpts, Jq=Jq)
+            allevals.append(evals)
             # Plot band structure
             nbands = evals.shape[1]
             emin = np.min(evals[:, 0])
             for i in range(nbands):
                 ax.plot(xs, (evals[:, i]) / 1.6e-22, color=color)
 
-        ax.set_ylabel('Energy (meV)')
+        ax.set_ylabel("Energy (meV)")
         ax.set_xlim(xlist[0][0], xlist[-1][-1])
         ax.set_xticks(Xs)
-        knames = [x if x != 'G' else '$\Gamma$' for x in knames]
+        knames = [x if x != "G" else "$\Gamma$" for x in knames]
         ax.set_xticklabels(knames)
         for x in Xs:
-            ax.axvline(x, linewidth=0.6, color='gray')
+            ax.axvline(x, linewidth=0.6, color="gray")
+
+        self.magnon_info = {
+            "kptlist": kptlist,
+            "xlist": xlist,
+            "knames": knames,
+            "X_for_highsym_kpoints": Xs,
+            "knames": knames,
+            "nbands":nbands,
+            "nkpts": len(kptlist),
+            "evals": allevals,
+        }
+        if  output_fname is not None:
+            self.save_magnon_json(output_fname)
         return ax
 
+    def save_magnon_json(self, fname):
+        with open(fname, "w") as myfile:
+            json.dump(self.magnon_info, myfile, cls=NumpyEncoder, indent=4)
+        print(f"""Saved magnon info to {fname}.
+Use the following script to plot: 
+python plot_magnon_from_json_file.py
+Or modify the script to plot in the way you want. 
+""")
+        with open("plot_magnon_from_json_file.py", "w") as myfile:
+            myfile.write(plot_script)
+
     def write_xml(self, fname):
         writer = SpinXmlWriter()
         writer._write(self, fname)
 
 
 def read_spin_ham_from_file(fname):
     parser = SpinXmlParser(fname)
-    ham = SpinHamiltonian(cell=parser.cell,
-                          xcart=parser.spin_positions,
-                          spinat=parser.spin_spinat,
-                          zion=parser.spin_zions)
-    ham.set(gilbert_damping=parser.spin_damping_factors,
-            gyro_ratio=parser.spin_gyro_ratios)
+    ham = SpinHamiltonian(
+        cell=parser.cell,
+        xcart=parser.spin_positions,
+        spinat=parser.spin_spinat,
+        zion=parser.spin_zions,
+    )
+    ham.set(
+        gilbert_damping=parser.spin_damping_factors, gyro_ratio=parser.spin_gyro_ratios
+    )
     if parser.has_exchange:
         ham.set_exchange_ijR(parser.exchange(isotropic=True))
     if parser.has_dmi:
         ham.set_dmi_ijR(parser.dmi)
     if parser.has_bilinear:
         ham.set_bilinear_ijR(parser.bilinear)
     return ham
```

### Comparing `TB2J-0.7.5/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.7.6/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/plot.py` & `TB2J-0.7.6/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/qsolver.py` & `TB2J-0.7.6/TB2J/spinham/qsolver.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/spin_api.py` & `TB2J-0.7.6/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/spin_xml.py` & `TB2J-0.7.6/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/spinham/supercell.py` & `TB2J-0.7.6/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/utest.py` & `TB2J-0.7.6/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/utils.py` & `TB2J-0.7.6/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J/wannier/w90_parser.py` & `TB2J-0.7.6/TB2J/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/TB2J.egg-info/PKG-INFO` & `TB2J-0.7.6/TB2J.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.5
+Version: 0.7.6
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.5/TB2J.egg-info/SOURCES.txt` & `TB2J-0.7.6/TB2J.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/scripts/TB2J_downfold.py` & `TB2J-0.7.6/scripts/TB2J_downfold.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/scripts/TB2J_eigen.py` & `TB2J-0.7.6/scripts/TB2J_eigen.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/scripts/TB2J_magnon.py` & `TB2J-0.7.6/scripts/TB2J_magnon.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,26 +60,26 @@
     parser.add_argument("--show",
                         action="store_true",
                         help="whether to show magnon band structure.",
                         default=False)
 
     args = parser.parse_args()
     if args.Jq:
+        if args.figfname is None:
+            args.figfname = 'Eigen_Jq.pdf'
         print(
             "Plotting the eigenvalues of -J(q). The figure is written to %s" %
             (args.figfname))
-        if args.figfname is None:
-            args.figfname = 'Eigen_Jq.pdf'
     else:
+        if args.figfname is None:
+            args.figfname = 'magnon_band.pdf'
         print(
             "Plotting the magnon band structure. The figure is written to %s" %
             (args.figfname))
-        if args.figfname is None:
-            args.figfname = 'magnon_band.pdf'
-
+        
     def nonone(x):
         if x is None:
             return x
         else:
             return not x
 
     if args.write_emin:
@@ -93,9 +93,9 @@
                          Jq=args.Jq,
                          figfname=args.figfname,
                          show=args.show,
                          has_exchange=nonone(args.no_Jiso),
                          has_dmi=nonone(args.no_dmi),
                          has_bilinear=nonone(args.no_Jani))
 
-
-plot_magnon()
+if __name__=="__main__":
+    plot_magnon()
```

### Comparing `TB2J-0.7.5/scripts/TB2J_merge.py` & `TB2J-0.7.6/scripts/TB2J_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/scripts/TB2J_rotate.py` & `TB2J-0.7.6/scripts/TB2J_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/scripts/siesta2J.py` & `TB2J-0.7.6/scripts/siesta2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/scripts/wann2J.py` & `TB2J-0.7.6/scripts/wann2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.5/setup.py` & `TB2J-0.7.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.7.5"
+__version__ = "0.7.6"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name='TB2J',
     version=__version__,
     description='TB2J: First principle to Heisenberg exchange J using tight-binding Green function method',
```

