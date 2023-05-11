# Comparing `tmp/pyfsdb-2.1.2.tar.gz` & `tmp/pyfsdb-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfsdb-2.1.2.tar", last modified: Thu Dec 15 00:12:20 2022, max compression
+gzip compressed data, was "pyfsdb-2.1.3.tar", last modified: Thu May 11 20:24:18 2023, max compression
```

## Comparing `pyfsdb-2.1.2.tar` & `pyfsdb-2.1.3.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-12-15 00:12:20.550680 pyfsdb-2.1.2/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-04-12 16:27:12.000000 pyfsdb-2.1.2/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5452 2022-12-15 00:12:20.550680 pyfsdb-2.1.2/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5010 2022-12-15 00:11:27.000000 pyfsdb-2.1.2/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-12-15 00:12:20.546680 pyfsdb-2.1.2/mod/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2020-10-09 02:50:07.000000 pyfsdb-2.1.2/mod/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       21 2020-10-09 02:49:47.000000 pyfsdb-2.1.2/mod/ick.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-12-15 00:12:20.546680 pyfsdb-2.1.2/pyfsdb/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/__init__.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    35063 2022-10-13 16:00:42.000000 pyfsdb-2.1.2/pyfsdb/fsdb.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-12-15 00:12:20.548679 pyfsdb-2.1.2/pyfsdb/obsolete/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/db2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbdatetoepoch.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbensure.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbformat.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbfullpivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbheatmap.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbnormalize.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbreescape.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbreversepivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbsplitter.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbtopn.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/obsolete/dbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-12-15 00:12:20.550680 pyfsdb-2.1.2/pyfsdb/tools/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/__init__.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/bro2fsdb.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/fsdb2json.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/fsdb2many.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/json2fsdb.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-10-25 20:28:42.000000 pyfsdb-2.1.2/pyfsdb/tools/pdb2sql.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2843 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdb2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdb2to1.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbaddtypes.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbcdf.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3430 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbdatetoepoch.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2111 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbensure.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbepochtodate.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbformat.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbfullpivot.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbheatmap.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2364 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbj2.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbnormalize.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbreescape.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2663 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbreversepivot.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-15 21:23:13.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbroc.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2263 2022-12-15 00:11:27.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbrow.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2910 2022-12-15 00:11:27.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbroweval.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbsplitter.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbtopn.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2242 2022-07-13 23:54:39.000000 pyfsdb-2.1.2/pyfsdb/tools/pdbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2022-12-15 00:12:20.547680 pyfsdb-2.1.2/pyfsdb.egg-info/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     5452 2022-12-15 00:12:20.000000 pyfsdb-2.1.2/pyfsdb.egg-info/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1529 2022-12-15 00:12:20.000000 pyfsdb-2.1.2/pyfsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2022-12-15 00:12:20.000000 pyfsdb-2.1.2/pyfsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1856 2022-12-15 00:12:20.000000 pyfsdb-2.1.2/pyfsdb.egg-info/entry_points.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       11 2022-12-15 00:12:20.000000 pyfsdb-2.1.2/pyfsdb.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2022-12-15 00:12:20.550680 pyfsdb-2.1.2/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3317 2022-12-15 00:11:58.000000 pyfsdb-2.1.2/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-03-18 13:10:45.000000 pyfsdb-2.1.3/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5649 2023-01-17 14:56:42.000000 pyfsdb-2.1.3/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.190106 pyfsdb-2.1.3/pyfsdb/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/__init__.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    35086 2023-01-25 14:19:32.000000 pyfsdb-2.1.3/pyfsdb/fsdb.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.195106 pyfsdb-2.1.3/pyfsdb/obsolete/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.3/pyfsdb/obsolete/__init__.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/db2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbdatetoepoch.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbensure.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbformat.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbfullpivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbheatmap.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbnormalize.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbreescape.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbreversepivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbsplitter.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbtopn.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/obsolete/dbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/pyfsdb/tools/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.3/pyfsdb/tools/__init__.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/bro2fsdb.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/fsdb2json.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/fsdb2many.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/json2fsdb.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-11-12 21:47:13.000000 pyfsdb-2.1.3/pyfsdb/tools/pdb2sql.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2845 2023-01-05 01:36:03.000000 pyfsdb-2.1.3/pyfsdb/tools/pdb2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdb2to1.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbaddtypes.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2023-01-06 15:32:58.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbcdf.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3430 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbdatetoepoch.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2134 2023-01-05 01:16:54.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbensure.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbepochtodate.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbformat.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbfullpivot.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbheatmap.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2373 2023-01-21 22:46:03.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbjinja.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbnormalize.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbreescape.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2663 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbreversepivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-21 13:26:37.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbroc.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2601 2023-05-10 21:40:55.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbrow.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3325 2023-05-10 21:42:43.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbroweval.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbsplitter.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-08-02 01:33:45.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbtopn.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2297 2023-02-06 19:45:06.000000 pyfsdb-2.1.3/pyfsdb/tools/pdbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-11 20:24:18.191106 pyfsdb-2.1.3/pyfsdb.egg-info/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1505 2023-05-11 20:24:18.000000 pyfsdb-2.1.3/pyfsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1861 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/entry_points.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        7 2023-05-11 20:24:17.000000 pyfsdb-2.1.3/pyfsdb.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-05-11 20:24:18.202106 pyfsdb-2.1.3/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3323 2023-05-11 20:17:26.000000 pyfsdb-2.1.3/setup.py
```

### Comparing `pyfsdb-2.1.2/LICENSE` & `pyfsdb-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/PKG-INFO` & `pyfsdb-2.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.2
+Version: 2.1.3
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Objective
 
-A python implementation of the (perl) [FSDB] flat-file streaming
-database.  Also, so my [C implementation].
+The [FSDB] "flat-file streaming database" is a structured data file
+that includes column names, formatting specifications (e.g. tab vs
+space vs comma), and a command history that generated each file.
+PyFSDB is a a python implementation of the original functionality that
+was implemented in perl.  Both the perl and python version come with a
+long list of [command line tools] that can be used to quickly process
+datasets using traditional unix pipeline processing.  There is also a
+[C implementation] and a Go implementation (ref needed) of FSDB.
+
+Getting started documentation is below, but also see the [full
+documentation] over on readthedocs.
 
 [FSDB]: https://www.isi.edu/~johnh/SOFTWARE/FSDB/
 [C implementation]: https://github.com/hardaker/fsdb-clib
+[full documentation]: https://fsdb.readthedocs.io/en/latest/
+[command line tools]: https://fsdb.readthedocs.io/en/latest/tools/index.html
 
 # Installation
 
 Using pip (or pipx):
 
 ```
 pip3 install pyfsdb
@@ -88,15 +97,15 @@
 # Additional Usage Details
 
 The real power of the FSDB comes from the build up of tool-suites that
 all interchange FSDB formatted files.  This allows chaining multiple
 commands together to achieve a goal.  Though the original base set of
 tools are in perl, you don't need to know perl for most of them.
 
-## Let's create a ./mydemo command:
+## Let's create a ./mydemo.py script:
 
 ``` python
 import sys, pyfsdb
 
 db = pyfsdb.Fsdb(file_handle=sys.stdin, out_file_handle=sys.stdout)
 value_column = db.get_column_number('value')
 
@@ -115,34 +124,32 @@
 2	123.0
 ```
 
 We can run it thus'ly:
 
 
 ``` sh
-# cat test.fsdb | ./mydemo
+# cat test.fsdb | ./mydemo.py
 #fsdb -F t col1 value
 1	84.0
 2	246.0
-#   | ./test.py
+#   | ./mydemo.py
 ```
 
 Or chain it together with multiple FSDB commands:
 
 ```
-# cat test.fsdb | ./mydemo | dbcolstats valueq
-cat test.fsdb | ./test.py | dbcolstats value | dbcol mean stddev sum min max | dbfilealter -R C
+# cat test.fsdb | ./mydemo | dbcolstats value | dbcol mean stddev sum min max | dbfilealter -R C
 #fsdb -R C mean stddev sum min max
 mean: 165
 stddev: 114.55
 sum: 330
 min: 84
 max: 246
-
-#   | ./test.py
+#   | ./mydemo.py
 #   | dbcolstats value
 #   | dbcol mean stddev sum min max
 #   | dbfilealter -R C
 ```
 
 # Command line tools included
 
@@ -203,9 +210,7 @@
 Wes Hardaker @ USC/ISI
 
 # See also
 
 The FSDB website and manual page for the original perl module:
 
 https://www.isi.edu/~johnh/SOFTWARE/FSDB/
-
-
```

### Comparing `pyfsdb-2.1.2/README.md` & `pyfsdb-2.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Objective
 
-A python implementation of the (perl) [FSDB] flat-file streaming
-database.  Also, so my [C implementation].
+The [FSDB] "flat-file streaming database" is a structured data file
+that includes column names, formatting specifications (e.g. tab vs
+space vs comma), and a command history that generated each file.
+PyFSDB is a a python implementation of the original functionality that
+was implemented in perl.  Both the perl and python version come with a
+long list of [command line tools] that can be used to quickly process
+datasets using traditional unix pipeline processing.  There is also a
+[C implementation] and a Go implementation (ref needed) of FSDB.
+
+Getting started documentation is below, but also see the [full
+documentation] over on readthedocs.
 
 [FSDB]: https://www.isi.edu/~johnh/SOFTWARE/FSDB/
 [C implementation]: https://github.com/hardaker/fsdb-clib
+[full documentation]: https://fsdb.readthedocs.io/en/latest/
+[command line tools]: https://fsdb.readthedocs.io/en/latest/tools/index.html
 
 # Installation
 
 Using pip (or pipx):
 
 ```
 pip3 install pyfsdb
@@ -73,15 +84,15 @@
 # Additional Usage Details
 
 The real power of the FSDB comes from the build up of tool-suites that
 all interchange FSDB formatted files.  This allows chaining multiple
 commands together to achieve a goal.  Though the original base set of
 tools are in perl, you don't need to know perl for most of them.
 
-## Let's create a ./mydemo command:
+## Let's create a ./mydemo.py script:
 
 ``` python
 import sys, pyfsdb
 
 db = pyfsdb.Fsdb(file_handle=sys.stdin, out_file_handle=sys.stdout)
 value_column = db.get_column_number('value')
 
@@ -100,34 +111,32 @@
 2	123.0
 ```
 
 We can run it thus'ly:
 
 
 ``` sh
-# cat test.fsdb | ./mydemo
+# cat test.fsdb | ./mydemo.py
 #fsdb -F t col1 value
 1	84.0
 2	246.0
-#   | ./test.py
+#   | ./mydemo.py
 ```
 
 Or chain it together with multiple FSDB commands:
 
 ```
-# cat test.fsdb | ./mydemo | dbcolstats valueq
-cat test.fsdb | ./test.py | dbcolstats value | dbcol mean stddev sum min max | dbfilealter -R C
+# cat test.fsdb | ./mydemo | dbcolstats value | dbcol mean stddev sum min max | dbfilealter -R C
 #fsdb -R C mean stddev sum min max
 mean: 165
 stddev: 114.55
 sum: 330
 min: 84
 max: 246
-
-#   | ./test.py
+#   | ./mydemo.py
 #   | dbcolstats value
 #   | dbcol mean stddev sum min max
 #   | dbfilealter -R C
 ```
 
 # Command line tools included
```

### Comparing `pyfsdb-2.1.2/pyfsdb/fsdb.py` & `pyfsdb-2.1.3/pyfsdb/fsdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,20 +64,22 @@
     "l": int,
     "L": int,
     "q": int,
     "Q": int,
     # python doesn't have different float/double sizes
     "f": float,
     "d": float,
-    # we leave strings (c and C) alone
+    # we leave strings as strings
+    "a": str,
 }
 
 outgoing_type_converters = {
     int: "l",
     float: "d",
+    str: "a",
 }
 
 
 class Fsdb(object):
     """Reads FSDB files from the perl FSDB module.
 
     (see the fsdb module documentation for full details)
```

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/bro2fsdb.py` & `pyfsdb-2.1.3/pyfsdb/tools/bro2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/fsdb2json.py` & `pyfsdb-2.1.3/pyfsdb/tools/fsdb2json.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/fsdb2many.py` & `pyfsdb-2.1.3/pyfsdb/tools/fsdb2many.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/json2fsdb.py` & `pyfsdb-2.1.3/pyfsdb/tools/json2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdb2sql.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdb2sql.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdb2tex.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdb2tex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 
 """db2tex converts any FSDB file into a latex table.
-WARNING: very little escaping is done -- watch out for mallicious input files."
+WARNING: very little escaping is done -- watch out for mallicious input files."""
 
 import argparse
 import sys
 import pyfsdb
 
 def parse_args():
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter,
```

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdb2to1.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdb2to1.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbaddtypes.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbaddtypes.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbaugment.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbaugment.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbcdf.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbcdf.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbcoluniq.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbcoluniq.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbdatetoepoch.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbdatetoepoch.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbensure.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbensure.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     args = parser.parse_args()
     return args
 
 
 def filter_row(row, columns, fill_value, print_error):
     for column in columns:
-        if row[column] == "":
+        if row[column] == "" or row[column] is None:
             if fill_value:
                 row[column] = fill_value
             else:
                 if print_error:
                     sys.stderr.write("# dbensure dropping row:" + str(row) + "\n")
                 return
     return row
```

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbepochtodate.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbepochtodate.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbformat.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbformat.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbfullpivot.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbfullpivot.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbheatmap.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbheatmap.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbj2.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbjinja.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import jinja2
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description=__doc__,
-        epilog="Example: pdbj2 -j report.j2 input.fsdb output.txt",
+        epilog="Example: pdbjinja -j report.jinja input.fsdb output.txt",
     )
 
     parser.add_argument(
         "-j",
         "--jinja2-template",
         type=argparse.FileType("r"),
         help="The jinja2 template file to use",
@@ -77,15 +77,15 @@
             include_file_path += "/"  # think required?
         loader = jinja2.FileStreamLoader(include_file_path)
 
     # create the actual template
     template = jinja2.Environment(loader=loader)
     template = template.from_string(jinja_template_data)
 
-    # call j2 and write the results out to the file
+    # call jinja and write the results out to the file
     output_file_handle.write(template.render({"rows": rows}))
 
 
 def main():
     args = parse_args()
     process(args.input_file, args.jinja2_template, args.output_file)
```

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbkeyedsort.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbkeyedsort.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbnormalize.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbnormalize.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbreescape.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbreescape.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbreversepivot.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbreversepivot.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbroc.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbroc.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbrow.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbrow.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,24 @@
 def parse_args():
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         description=__doc__,
         epilog="Exmaple Usage: pdbrow 'column_a == 5' input.fsdb output.fsdb",
     )
 
-    parser.add_argument("-i", "--init-code",
-                        help="Initialization code to execute first (eg, imports)")
+    parser.add_argument(
+        "-u",
+        "--underbars",
+        action="store_true",
+        help="Use variable names with _ prefixes to the column names",
+    )
+
+    parser.add_argument(
+        "-i", "--init-code", help="Initialization code to execute first (eg, imports)"
+    )
 
     parser.add_argument(
         "--log-level", default="info", help="Define the logging verbosity level."
     )
 
     parser.add_argument(
         "expression",
@@ -45,51 +53,58 @@
     args = parser.parse_args()
     log_level = args.log_level.upper()
     logging.basicConfig(level=log_level, format="%(levelname)-10s:\t%(message)s")
     return args
 
 
 def process_pdbrow(
-        input_file,
-        output_file,
-        expression,
-        init_code = None,
+    input_file,
+    output_file,
+    expression,
+    init_code=None,
+    use_underbars=False,
 ):
 
     # open input and output fsdb handles
     fh = pyfsdb.Fsdb(file_handle=input_file, return_type=pyfsdb.RETURN_AS_DICTIONARY)
     oh = pyfsdb.Fsdb(out_file_handle=output_file)
 
     # crate output columns
     oh.out_column_names = fh.column_names
 
     globals = {}
 
     if init_code:
-        exec(compile(init_code, '<string>', 'exec'), globals)
+        exec(compile(init_code, "<string>", "exec"), globals)
 
-    compiled_expression = compile(f"{expression}", '<string>', 'eval')
+    compiled_expression = compile(f"{expression}", "<string>", "eval")
 
     # process the rows
     for row in fh:
 
-        # execute the expression and check its result
-        result = eval(compiled_expression, globals, row)
+        # if they wanted under-bar based names, add them
+        if use_underbars:
+            result = eval(
+                compiled_expression, globals, {"_" + k: v for k, v in row.items()}
+            )
+        else:
+            result = eval(compiled_expression, globals, row)
+
         if result:
             oh.append(row)
 
     oh.close()
 
+
 def main():
     args = parse_args()
 
     process_pdbrow(
         args.input_file,
         args.output_file,
         args.expression,
         args.init_code,
     )
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbroweval.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbroweval.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,38 @@
 def get_parse_args():
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         description=__doc__,
         epilog="Exmaple Usage: pdbroweval 'column_a = column_a * 5' input.fsdb output.fsdb",
     )
 
-    parser.add_argument("-i", "--init-code",
-                        help="Initialization code to execute first (eg, imports)")
+    parser.add_argument(
+        "-u",
+        "--underbars",
+        action="store_true",
+        help="Use variable names with _ prefixes to the column names",
+    )
 
-    parser.add_argument("-f", "--expression-is-file", action="store_true",
-                        help="The expression is actually a python code file to lead")
+    parser.add_argument(
+        "-i", "--init-code", help="Initialization code to execute first (eg, imports)"
+    )
 
-    parser.add_argument("-I", "--init-code-is-file", action="store_true",
-                        help="The expression is actually a python code file to lead")
+    parser.add_argument(
+        "-f",
+        "--expression-is-file",
+        action="store_true",
+        help="The expression is actually a python code file to load",
+    )
+
+    parser.add_argument(
+        "-I",
+        "--init-code-is-file",
+        action="store_true",
+        help="The expression is actually a python code file to load",
+    )
 
     parser.add_argument(
         "--log-level", default="info", help="Define the logging verbosity level."
     )
 
     parser.add_argument(
         "expression",
@@ -46,67 +62,76 @@
         nargs="?",
         default=sys.stdout,
         help="Where to write the output FSDB to",
     )
 
     return parser
 
+
 def parse_args():
     parser = get_parse_args()
     args = parser.parse_args()
     log_level = args.log_level.upper()
     logging.basicConfig(level=log_level, format="%(levelname)-10s:\t%(message)s")
     return args
 
 
 def process_pdbroweval(
-        input_file,
-        output_file,
-        expression,
-        init_code = None,
-        from_file = False,
-        init_code_file = False,
+    input_file,
+    output_file,
+    expression,
+    init_code=None,
+    from_file=False,
+    init_code_file=False,
+    use_underbars=False,
 ):
 
     # open input and output fsdb handles
     fh = pyfsdb.Fsdb(file_handle=input_file, return_type=pyfsdb.RETURN_AS_DICTIONARY)
     oh = pyfsdb.Fsdb(out_file_handle=output_file)
 
     # crate output columns
     oh.out_column_names = fh.column_names
 
     globals = {}
 
     if init_code:
         if init_code_file:
             init_code = init_code.read()
-        exec(compile(init_code, '<string>', 'exec'), globals)
+        exec(compile(init_code, "<string>", "exec"), globals)
 
     if from_file:
         expression = expression.read()
         error(expression)
-    compiled_expression = compile(f"{expression}", '<string>', 'exec')
+    compiled_expression = compile(f"{expression}", "<string>", "exec")
+
+    # if they wanted under-bar based names
+    if use_underbars:
+        fh.column_names = ["_" + x for x in fh.column_names]
 
     # process the rows
     for row in fh:
 
         # execute the expression and check its result
         exec(compiled_expression, globals, row)
+        if use_underbars:
+            row = {k[1:]: v for k, v in row.items()}
         oh.append(row)
 
     oh.close()
 
+
 def main():
     args = parse_args()
 
     process_pdbroweval(
         args.input_file,
         args.output_file,
         args.expression,
         args.init_code,
         args.expression_is_file,
+        args.underbars,
     )
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbsplitter.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbsplitter.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbsum.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbsum.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbtopn.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbtopn.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.2/pyfsdb/tools/pdbzerofill.py` & `pyfsdb-2.1.3/pyfsdb/tools/pdbzerofill.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 
-"""Fills a column with zeros if it was otherwise blank"""
+"""Fills a row that is missing in a series of rows with a numerical
+increasing (frequently a timestamp) index"""
 
 import sys
 import argparse
 import pyfsdb
 
 
 def parse_args():
```

### Comparing `pyfsdb-2.1.2/pyfsdb.egg-info/PKG-INFO` & `pyfsdb-2.1.3/pyfsdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.2
+Version: 2.1.3
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Objective
 
-A python implementation of the (perl) [FSDB] flat-file streaming
-database.  Also, so my [C implementation].
+The [FSDB] "flat-file streaming database" is a structured data file
+that includes column names, formatting specifications (e.g. tab vs
+space vs comma), and a command history that generated each file.
+PyFSDB is a a python implementation of the original functionality that
+was implemented in perl.  Both the perl and python version come with a
+long list of [command line tools] that can be used to quickly process
+datasets using traditional unix pipeline processing.  There is also a
+[C implementation] and a Go implementation (ref needed) of FSDB.
+
+Getting started documentation is below, but also see the [full
+documentation] over on readthedocs.
 
 [FSDB]: https://www.isi.edu/~johnh/SOFTWARE/FSDB/
 [C implementation]: https://github.com/hardaker/fsdb-clib
+[full documentation]: https://fsdb.readthedocs.io/en/latest/
+[command line tools]: https://fsdb.readthedocs.io/en/latest/tools/index.html
 
 # Installation
 
 Using pip (or pipx):
 
 ```
 pip3 install pyfsdb
@@ -88,15 +97,15 @@
 # Additional Usage Details
 
 The real power of the FSDB comes from the build up of tool-suites that
 all interchange FSDB formatted files.  This allows chaining multiple
 commands together to achieve a goal.  Though the original base set of
 tools are in perl, you don't need to know perl for most of them.
 
-## Let's create a ./mydemo command:
+## Let's create a ./mydemo.py script:
 
 ``` python
 import sys, pyfsdb
 
 db = pyfsdb.Fsdb(file_handle=sys.stdin, out_file_handle=sys.stdout)
 value_column = db.get_column_number('value')
 
@@ -115,34 +124,32 @@
 2	123.0
 ```
 
 We can run it thus'ly:
 
 
 ``` sh
-# cat test.fsdb | ./mydemo
+# cat test.fsdb | ./mydemo.py
 #fsdb -F t col1 value
 1	84.0
 2	246.0
-#   | ./test.py
+#   | ./mydemo.py
 ```
 
 Or chain it together with multiple FSDB commands:
 
 ```
-# cat test.fsdb | ./mydemo | dbcolstats valueq
-cat test.fsdb | ./test.py | dbcolstats value | dbcol mean stddev sum min max | dbfilealter -R C
+# cat test.fsdb | ./mydemo | dbcolstats value | dbcol mean stddev sum min max | dbfilealter -R C
 #fsdb -R C mean stddev sum min max
 mean: 165
 stddev: 114.55
 sum: 330
 min: 84
 max: 246
-
-#   | ./test.py
+#   | ./mydemo.py
 #   | dbcolstats value
 #   | dbcol mean stddev sum min max
 #   | dbfilealter -R C
 ```
 
 # Command line tools included
 
@@ -203,9 +210,7 @@
 Wes Hardaker @ USC/ISI
 
 # See also
 
 The FSDB website and manual page for the original perl module:
 
 https://www.isi.edu/~johnh/SOFTWARE/FSDB/
-
-
```

### Comparing `pyfsdb-2.1.2/pyfsdb.egg-info/SOURCES.txt` & `pyfsdb-2.1.3/pyfsdb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENSE
 README.md
 setup.py
-mod/__init__.py
-mod/ick.py
 pyfsdb/__init__.py
 pyfsdb/fsdb.py
 pyfsdb.egg-info/PKG-INFO
 pyfsdb.egg-info/SOURCES.txt
 pyfsdb.egg-info/dependency_links.txt
 pyfsdb.egg-info/entry_points.txt
 pyfsdb.egg-info/top_level.txt
@@ -41,15 +39,15 @@
 pyfsdb/tools/pdbcoluniq.py
 pyfsdb/tools/pdbdatetoepoch.py
 pyfsdb/tools/pdbensure.py
 pyfsdb/tools/pdbepochtodate.py
 pyfsdb/tools/pdbformat.py
 pyfsdb/tools/pdbfullpivot.py
 pyfsdb/tools/pdbheatmap.py
-pyfsdb/tools/pdbj2.py
+pyfsdb/tools/pdbjinja.py
 pyfsdb/tools/pdbkeyedsort.py
 pyfsdb/tools/pdbnormalize.py
 pyfsdb/tools/pdbreescape.py
 pyfsdb/tools/pdbreversepivot.py
 pyfsdb/tools/pdbroc.py
 pyfsdb/tools/pdbrow.py
 pyfsdb/tools/pdbroweval.py
```

### Comparing `pyfsdb-2.1.2/pyfsdb.egg-info/entry_points.txt` & `pyfsdb-2.1.3/pyfsdb.egg-info/entry_points.txt`

 * *Files 17% similar despite different names*

```diff
@@ -27,20 +27,19 @@
 pdbcoluniq = pyfsdb.tools.pdbcoluniq:main
 pdbdatetoepoch = pyfsdb.tools.pdbdatetoepoch:main
 pdbensure = pyfsdb.tools.pdbensure:main
 pdbepochtodate = pyfsdb.tools.pdbepochtodate:main
 pdbformat = pyfsdb.tools.pdbformat:main
 pdbfullpivot = pyfsdb.tools.pdbfullpivot:main
 pdbheatmap = pyfsdb.tools.pdbheatmap:main
-pdbj2 = pyfsdb.tools.pdbj2:main
+pdbjinja = pyfsdb.tools.pdbjinja:main
 pdbkeyedsort = pyfsdb.tools.pdbkeyedsort:main
 pdbnormalize = pyfsdb.tools.pdbnormalize:main
 pdbreescape = pyfsdb.tools.pdbreescape:main
 pdbreversepivot = pyfsdb.tools.pdbreversepivot:main
 pdbroc = pyfsdb.tools.pdbroc:main
 pdbrow = pyfsdb.tools.pdbrow:main
 pdbroweval = pyfsdb.tools.pdbroweval:main
 pdbsplitter = pyfsdb.tools.pdbsplitter:main
 pdbsum = pyfsdb.tools.pdbsum:main
 pdbtopn = pyfsdb.tools.pdbtopn:main
 pdbzerofill = pyfsdb.tools.pdbzerofill:main
-
```

### Comparing `pyfsdb-2.1.2/setup.py` & `pyfsdb-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfsdb",
-    version="2.1.2",
+    version="2.1.3",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A python implementation of the flat-file streaming database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gawseed/pyfsdb",
     packages=setuptools.find_packages(),
@@ -33,15 +33,15 @@
             "pdbreescape = pyfsdb.tools.pdbreescape:main",
             "pdbensure = pyfsdb.tools.pdbensure:main",
             "pdbheatmap = pyfsdb.tools.pdbheatmap:main",
             "pdbdatetoepoch = pyfsdb.tools.pdbdatetoepoch:main",
             "pdbepochtodate = pyfsdb.tools.pdbepochtodate:main",
             "pdbnormalize = pyfsdb.tools.pdbnormalize:main",
             "pdbsum = pyfsdb.tools.pdbsum:main",
-            "pdbj2 = pyfsdb.tools.pdbj2:main",
+            "pdbjinja = pyfsdb.tools.pdbjinja:main",
             "pdbcdf = pyfsdb.tools.pdbcdf:main",
             "pdbroc = pyfsdb.tools.pdbroc:main",
             "pdb2sql = pyfsdb.tools.pdb2sql:main",
             "pdb2to1 = pyfsdb.tools.pdb2to1:main",
             "pdbaddtypes = pyfsdb.tools.pdbaddtypes:main",
             "pdbrow = pyfsdb.tools.pdbrow:main",
             "pdbroweval = pyfsdb.tools.pdbroweval:main",
```

