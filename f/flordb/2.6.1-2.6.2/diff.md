# Comparing `tmp/flordb-2.6.1.tar.gz` & `tmp/flordb-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flordb-2.6.1.tar", last modified: Fri Apr 14 18:09:39 2023, max compression
+gzip compressed data, was "flordb-2.6.2.tar", last modified: Thu May 11 17:45:07 2023, max compression
```

## Comparing `flordb-2.6.1.tar` & `flordb-2.6.2.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.536112 flordb-2.6.1/
--rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.1/LICENSE
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-04-14 18:09:39.536006 flordb-2.6.1/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     7667 2023-03-12 20:12:23.000000 flordb-2.6.1/README.md
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.528533 flordb-2.6.1/flor/
--rw-r--r--   0 rogarcia   (501) staff       (20)      246 2023-04-04 22:53:53.000000 flordb-2.6.1/flor/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/constants.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     5339 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/flags.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.528991 flordb-2.6.1/flor/hlast/
--rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/hlast/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gtpropagate.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.529984 flordb-2.6.1/flor/hlast/gumtree/
--rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/adapter.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/idmap.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/priorityq.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/python.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/test.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/hlast/gumtree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/hlast/visitors.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/iterator.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.530106 flordb-2.6.1/flor/journal/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/journal/__init__.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.530479 flordb-2.6.1/flor/journal/entry/
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/constants.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.531432 flordb-2.6.1/flor/journal/entry/data/
--rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/journal/entry/data/dataframe.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/reference.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/torch_chkpt.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/data/value.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.532243 flordb-2.6.1/flor/journal/entry/metadata/
--rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/bracket.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/entry/metadata/eof.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.532843 flordb-2.6.1/flor/journal/tree/
--rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/block.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/group.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/journal/tree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/journal/tree/window.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1998 2023-04-14 18:08:18.000000 flordb-2.6.1/flor/kits.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.533558 flordb-2.6.1/flor/logger/
--rw-r--r--   0 rogarcia   (501) staff       (20)      897 2023-03-20 19:44:52.000000 flordb-2.6.1/flor/logger/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/logger/checkpoint_logger.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1318 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/logger/exp_json.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/logger/future.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.1/flor/logger/log_records.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.534454 flordb-2.6.1/flor/query/
--rw-r--r--   0 rogarcia   (501) staff       (20)     7921 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/query/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3658 2023-03-15 23:49:42.000000 flordb-2.6.1/flor/query/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1862 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/query/engine.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/query/pivot.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8773 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/query/unpack.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.534787 flordb-2.6.1/flor/shelf/
--rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.1/flor/shelf/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2382 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/shelf/cwd_shelf.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3148 2023-03-23 13:19:05.000000 flordb-2.6.1/flor/shelf/home_shelf.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.535378 flordb-2.6.1/flor/skipblock/
--rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.1/flor/skipblock/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.1/flor/skipblock/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/skipblock/readblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.1/flor/skipblock/seemblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.1/flor/skipblock/writeblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.1/flor/state.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      564 2023-04-04 22:53:53.000000 flordb-2.6.1/flor/utils.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-04-14 18:09:39.535865 flordb-2.6.1/flordb.egg-info/
--rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     1636 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/SOURCES.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/dependency_links.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/requires.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-04-14 18:09:39.000000 flordb-2.6.1/flordb.egg-info/top_level.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-04-14 18:09:39.536144 flordb-2.6.1/setup.cfg
--rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-04-14 18:09:20.000000 flordb-2.6.1/setup.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.447242 flordb-2.6.2/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.6.2/LICENSE
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-11 17:45:07.447132 flordb-2.6.2/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     7667 2023-03-12 20:12:23.000000 flordb-2.6.2/README.md
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.436805 flordb-2.6.2/flor/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      244 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      799 2023-05-10 13:21:04.000000 flordb-2.6.2/flor/__main__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/constants.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2330 2023-05-10 13:21:04.000000 flordb-2.6.2/flor/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6142 2023-05-04 17:16:10.000000 flordb-2.6.2/flor/flags.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.437800 flordb-2.6.2/flor/hlast/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4159 2023-03-23 13:19:05.000000 flordb-2.6.2/flor/hlast/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gtpropagate.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.439803 flordb-2.6.2/flor/hlast/gumtree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6322 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/adapter.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/idmap.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/priorityq.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/python.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/test.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/hlast/gumtree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2273 2023-03-23 13:19:05.000000 flordb-2.6.2/flor/hlast/visitors.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/iterator.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.439948 flordb-2.6.2/flor/journal/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2946 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/journal/__init__.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.440456 flordb-2.6.2/flor/journal/entry/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/constants.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.441577 flordb-2.6.2/flor/journal/entry/data/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.6.2/flor/journal/entry/data/dataframe.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/reference.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/torch_chkpt.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/data/value.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.442530 flordb-2.6.2/flor/journal/entry/metadata/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/bracket.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/entry/metadata/eof.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.443200 flordb-2.6.2/flor/journal/tree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/block.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/group.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/journal/tree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4231 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/journal/tree/window.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1998 2023-04-14 18:08:18.000000 flordb-2.6.2/flor/kits.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.444208 flordb-2.6.2/flor/logger/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2219 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/logger/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/logger/checkpoint_logger.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.6.2/flor/logger/exp_json.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/logger/future.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.6.2/flor/logger/log_records.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.445063 flordb-2.6.2/flor/query/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8262 2023-05-10 13:31:42.000000 flordb-2.6.2/flor/query/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3658 2023-03-15 23:49:42.000000 flordb-2.6.2/flor/query/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1862 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/query/engine.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2503 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/query/pivot.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8773 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/query/unpack.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.445664 flordb-2.6.2/flor/shelf/
+-rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.6.2/flor/shelf/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2492 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/shelf/cwd_shelf.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.6.2/flor/shelf/home_shelf.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.446414 flordb-2.6.2/flor/skipblock/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.6.2/flor/skipblock/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.6.2/flor/skipblock/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/skipblock/readblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.6.2/flor/skipblock/seemblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.6.2/flor/skipblock/writeblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      600 2023-03-22 14:08:08.000000 flordb-2.6.2/flor/state.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      564 2023-04-04 22:53:53.000000 flordb-2.6.2/flor/utils.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-05-11 17:45:07.446996 flordb-2.6.2/flordb.egg-info/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8099 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1670 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/SOURCES.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/dependency_links.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/requires.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-05-11 17:45:07.000000 flordb-2.6.2/flordb.egg-info/top_level.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-05-11 17:45:07.447294 flordb-2.6.2/setup.cfg
+-rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-05-11 17:44:55.000000 flordb-2.6.2/setup.py
```

### Comparing `flordb-2.6.1/LICENSE` & `flordb-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/PKG-INFO` & `flordb-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.1
+Version: 2.6.2
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `flordb-2.6.1/README.md` & `flordb-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/constants.py` & `flordb-2.6.2/flor/constants.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/flags.py` & `flordb-2.6.2/flor/flags.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from flor.shelf import home_shelf, cwd_shelf
 from flor.constants import *
 from flor.state import State
 from flor.logger import exp_json
 from flor.query.database import start_db
 
 import sys
-from typing import Dict, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Tuple, Union
 from pathlib import PurePath, Path
 from time import time
 
+from argparse import ArgumentParser, HelpFormatter, Namespace
+
+
 NAME: Optional[str] = None
 REPLAY: bool = False
 INDEX: Optional[PurePath] = None
 MODE: Optional[REPLAY_MODE] = None
 PID: REPLAY_PARALLEL = REPLAY_PARALLEL(1, 1)
 EPSILON: float = 1 / 15
 RESUMING: bool = False
@@ -51,22 +54,34 @@
         assert isinstance(p, int) and isinstance(n, int)
         assert p >= 0
         assert n >= 1
         assert p <= n
         PID = REPLAY_PARALLEL(*pid)
 
 
-class Parser:
-    """
-    --flor NAME [EPSILON]
-    --replay_flor [weak | strong] [i/n]
-    """
+class CLI_Args(ArgumentParser):
+    def __init__(self) -> None:
+        super().__init__(
+            prog=None,
+            usage=None,
+            description=None,
+            epilog="Arguments parsed by Flor",
+            parents=[],
+            formatter_class=HelpFormatter,
+            prefix_chars="-",
+            fromfile_prefix_chars=None,
+            argument_default=None,
+            conflict_handler="error",
+            add_help=False,
+            allow_abbrev=False,
+            exit_on_error=True,
+        )
+        self.nsp = Namespace()
 
-    @staticmethod
-    def _parse_name():
+    def parse_record(self):
         assert (
             "--replay_flor" not in sys.argv
         ), "Pick at most one of `--flor` or `--replay_flor` but not both"
         assert (
             cwd_shelf.in_shadow_branch()
         ), "Please invoke --flor from a `flor.shadow` branch."
         global NAME, EPSILON, DATALOGGING
@@ -104,16 +119,15 @@
         assert NAME is not None
         if exp_json.exists() and exp_json.get("NAME") == NAME:
             # IF previous name is same as this name
             DATALOGGING = False
         exp_json.put("NAME", NAME)
         home_shelf.mk_job(cwd_shelf.get_projid())
 
-    @staticmethod
-    def _parse_replay():
+    def parse_replay(self):
         assert (
             "--flor" not in sys.argv
         ), "Pick at most one of `--flor` or `--replay_flor` but not both"
         assert (
             cwd_shelf.in_shadow_branch()
         ), "Please invoke --replay_flor from a `flor.shadow` branch."
         try:
@@ -160,27 +174,41 @@
                 index=exp_json.get("MEMO"),
                 mode=mode,
                 pid=pid,
             )
             home_shelf.set_job(projid)
             start_db(projid)
 
-    @staticmethod
-    def parse():
-        State.import_time = time()
-        if "--flor" in sys.argv:
-            Parser._parse_name()
-        elif "--replay_flor" in sys.argv:
-            Parser._parse_replay()
+    def parse_remaining(self):
+        skip = True
+        for flg in [each for each in sys.argv if each[0:2] == "--"]:
+            skip = False
+            self.add_argument(flg)
+        if not skip:
+            self.nsp, sys.argv[:] = self.parse_known_args()
+
+
+parser = CLI_Args()
+
+
+def parse():
+    State.import_time = time()
+    if "--flor" in sys.argv:
+        parser.parse_record()
+    elif "--replay_flor" in sys.argv:
+        parser.parse_replay()
+    parser.parse_remaining()
 
 
 __all__ = [
     "NAME",
     "REPLAY",
     "INDEX",
     "MODE",
     "PID",
     "EPSILON",
     "DATALOGGING",
     "set_REPLAY",
-    "Parser",
+    "parse",
+    "parser",
+    "CLI_Args",
 ]
```

### Comparing `flordb-2.6.1/flor/hlast/__init__.py` & `flordb-2.6.2/flor/hlast/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gtpropagate.py` & `flordb-2.6.2/flor/hlast/gtpropagate.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gumtree/__init__.py` & `flordb-2.6.2/flor/hlast/gumtree/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gumtree/adapter.py` & `flordb-2.6.2/flor/hlast/gumtree/adapter.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gumtree/idmap.py` & `flordb-2.6.2/flor/hlast/gumtree/idmap.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gumtree/priorityq.py` & `flordb-2.6.2/flor/hlast/gumtree/priorityq.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gumtree/python.py` & `flordb-2.6.2/flor/hlast/gumtree/python.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gumtree/test.py` & `flordb-2.6.2/flor/hlast/gumtree/test.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/gumtree/tree.py` & `flordb-2.6.2/flor/hlast/gumtree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/hlast/visitors.py` & `flordb-2.6.2/flor/hlast/visitors.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/iterator.py` & `flordb-2.6.2/flor/iterator.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/__init__.py` & `flordb-2.6.2/flor/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/__init__.py` & `flordb-2.6.2/flor/journal/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/abstract.py` & `flordb-2.6.2/flor/journal/entry/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/data/abstract.py` & `flordb-2.6.2/flor/journal/entry/data/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/data/dataframe.py` & `flordb-2.6.2/flor/journal/entry/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/data/reference.py` & `flordb-2.6.2/flor/journal/entry/data/reference.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/data/torch_chkpt.py` & `flordb-2.6.2/flor/journal/entry/data/torch_chkpt.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/data/value.py` & `flordb-2.6.2/flor/journal/entry/data/value.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/metadata/bracket.py` & `flordb-2.6.2/flor/journal/entry/metadata/bracket.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/entry/metadata/eof.py` & `flordb-2.6.2/flor/journal/entry/metadata/eof.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/tree/block.py` & `flordb-2.6.2/flor/journal/tree/block.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/tree/group.py` & `flordb-2.6.2/flor/journal/tree/group.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/tree/tree.py` & `flordb-2.6.2/flor/journal/tree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/journal/tree/window.py` & `flordb-2.6.2/flor/journal/tree/window.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/kits.py` & `flordb-2.6.2/flor/kits.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/logger/checkpoint_logger.py` & `flordb-2.6.2/flor/logger/checkpoint_logger.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/logger/exp_json.py` & `flordb-2.6.2/flor/logger/exp_json.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from flor.constants import REPLAY_JSON, SECONDS_JSON
 from flor import flags
 from flor.state import State
 from typing import Optional, Dict, Any
 
 import json, os
 from pathlib import Path
+import time
 
 replay_d: Optional[Dict[str, Any]] = None
 record_d = {}
 
 
 def _get_path(p=REPLAY_JSON):
     assert State.common_dir is not None
@@ -40,13 +41,20 @@
     assert replay_d is not None
     return replay_d.get(name, None)
 
 
 def flush():
     if flags.NAME and not flags.REPLAY:
         assert State.common_dir is not None
+        record_d['CLI'] = vars(flags.parser.nsp)
         with open(_get_path(), "w", encoding="utf-8") as f:
             json.dump(record_d, f, ensure_ascii=False, indent=4)
-        
+
+        assert State.import_time is not None
+        State.seconds["PREP"] = (
+            State.seconds["PREP"]
+            if State.seconds["PREP"] is not None
+            else time.time() - State.import_time
+        )
         assert State.seconds["PREP"] is not None
         with open(_get_path(SECONDS_JSON), "w", encoding="utf-8") as f:
             json.dump(State.seconds, f, indent=4)
```

### Comparing `flordb-2.6.1/flor/logger/future.py` & `flordb-2.6.2/flor/logger/future.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/logger/log_records.py` & `flordb-2.6.2/flor/logger/log_records.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/query/__init__.py` & `flordb-2.6.2/flor/query/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from IPython.display import display
 
 from flor.query.pivot import *
 from flor.query.engine import *
 from flor.constants import *
 from flor.state import State
 
+import math
+
 pivot_vars: Dict[str, Set[str]] = {
     "DATA_PREP": set([]),
     "OUTR_LOOP": set([]),
     "INNR_LOOP": set([]),
 }
 
 
@@ -132,15 +134,15 @@
     where_clause: stated in Pandas/SQL, passed to full_pivot
     path: `train_rnn.py` or such denoting main python script
     """
     assert Path(path).suffix == ".py"
     facts = log_records(skip_unpack=True)
     df = full_pivot(facts)
     assert df is not None
-    assert all([v in facts['name'].values for v in apply_vars])
+    assert all([v in facts["name"].values for v in apply_vars])
 
     loglvl = get_dims(pivot_vars, apply_vars)
     dp_schedule = (
         df.query(where_clause)[list(DATA_PREP)]
         .drop_duplicates()
         .merge(
             pd.DataFrame(database.get_schedule(DATA_PREP)).astype(
@@ -236,8 +238,21 @@
         res = input("Continue [Y/n]? ")
         if res.strip().lower() != "n":
             batch_replay(apply_vars, path, versions, INNR_LOOP)
     else:
         raise
 
 
-__all__ = ["log_records", "full_pivot", "clear_stash", "replay"]
+def batch(table: pd.DataFrame):
+    cli_args = []
+    records = table.to_dict(orient="records")
+    for record in records:
+        s = ""
+        for k, v in record.items():
+            if v is None or math.isnan(v):
+                continue
+            s += f"--{k} {v} "
+        cli_args.append(s)
+        print(s)
+
+
+__all__ = ["log_records", "full_pivot", "clear_stash", "replay", "batch"]
```

### Comparing `flordb-2.6.1/flor/query/database.py` & `flordb-2.6.2/flor/query/database.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/query/engine.py` & `flordb-2.6.2/flor/query/engine.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/query/pivot.py` & `flordb-2.6.2/flor/query/pivot.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/query/unpack.py` & `flordb-2.6.2/flor/query/unpack.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/shelf/cwd_shelf.py` & `flordb-2.6.2/flor/shelf/cwd_shelf.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 import atexit
 
 PATH = Path(".flor")
 
 
 def get_projid():
+    if flags.NAME is None:
+        return ""
     if State.common_dir is None:
         r = Repo()
         State.common_dir = Path(r.common_dir)
     return (
         os.path.basename(os.path.dirname(str(State.common_dir)))
         + "_"
         + str(State.active_branch)
@@ -47,14 +49,17 @@
         cond = check_branch_cond()
         if cond:
             PATH.mkdir(exist_ok=True)
             get_projid()
         return cond
     except InvalidGitRepositoryError:
         return False
+    except Exception as e:
+        print(e)
+        return False
 
 
 def check_branch_cond():
     if State.repo is not None:
         return "RECORD::" in str(
             State.repo.head.commit.message
         ) or "flor.shadow" in State.repo.git.branch(
```

### Comparing `flordb-2.6.1/flor/shelf/home_shelf.py` & `flordb-2.6.2/flor/shelf/home_shelf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 florin: Path = home / ".flor"
 florin.mkdir(exist_ok=True)
 
 job: Optional[Path] = None
 data: Optional[Path] = None
 timestamp: Optional[str] = None
 
+def server_init():
+    pass
 
 def get_checkpoint_bytes_per_epoch(projid: str):
     pkl_paths = []
     with open(florin / projid / "latest.json", "r") as f:
         for jstring in f.readlines():
             d = json.loads(jstring)
             if "metadata" in d and d["metadata"] == "LBRACKET" and pkl_paths:
```

### Comparing `flordb-2.6.1/flor/skipblock/abstract.py` & `flordb-2.6.2/flor/skipblock/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/skipblock/readblock.py` & `flordb-2.6.2/flor/skipblock/readblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/skipblock/writeblock.py` & `flordb-2.6.2/flor/skipblock/writeblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/state.py` & `flordb-2.6.2/flor/state.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flor/utils.py` & `flordb-2.6.2/flor/utils.py`

 * *Files identical despite different names*

### Comparing `flordb-2.6.1/flordb.egg-info/PKG-INFO` & `flordb-2.6.2/flordb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.6.1
+Version: 2.6.2
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `flordb-2.6.1/flordb.egg-info/SOURCES.txt` & `flordb-2.6.2/flordb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 setup.py
 flor/__init__.py
+flor/__main__.py
 flor/constants.py
+flor/database.py
 flor/flags.py
 flor/iterator.py
 flor/kits.py
 flor/state.py
 flor/utils.py
 flor/hlast/__init__.py
 flor/hlast/gtpropagate.py
```

### Comparing `flordb-2.6.1/setup.py` & `flordb-2.6.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flordb",
-    version="2.6.1",
+    version="2.6.2",
     author="Rolando Garcia",
     author_email="rogarcia@berkeley.edu",
     description="Fast Low-Overhead Recovery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ucbrise/flor",
     packages=setuptools.find_packages(),
```

