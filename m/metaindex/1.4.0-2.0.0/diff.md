# Comparing `tmp/metaindex-1.4.0.tar.gz` & `tmp/metaindex-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaindex-1.4.0.tar", last modified: Thu Jun 30 13:09:45 2022, max compression
+gzip compressed data, was "metaindex-2.0.0.tar", last modified: Thu May 11 18:12:32 2023, max compression
```

## Comparing `metaindex-1.4.0.tar` & `metaindex-2.0.0.tar`

### file list

```diff
@@ -1,170 +1,171 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/
--rw-r--r--   0 robert    (1000) robert    (1000)     4326 2022-06-30 13:09:05.000000 metaindex-1.4.0/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-1.4.0/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-1.4.0/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     4747 2022-06-30 13:09:45.774698 metaindex-1.4.0/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     3879 2022-06-28 22:15:16.000000 metaindex-1.4.0/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.758031 metaindex-1.4.0/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-1.4.0/doc/Makefile
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.758031 metaindex-1.4.0/doc/build/
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.764698 metaindex-1.4.0/doc/build/doctrees/
--rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/addons.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/changelog.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/cmdoptions.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/cmdusage.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/configuration.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/description.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/doctrees/environment.pickle
--rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/examples.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/extrametadata.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/index.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/indexers.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/install.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-1.4.0/doc/build/doctrees/license.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/doctrees/reference.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/doctrees/searchsyntax.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/doctrees/synopsis.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/doctrees/usage.doctree
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.768031 metaindex-1.4.0/doc/build/html/
--rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/.buildinfo
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.768031 metaindex-1.4.0/doc/build/html/_sources/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-1.4.0/doc/build/html/_sources/addons.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-1.4.0/doc/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-1.4.0/doc/build/html/_sources/cmdoptions.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-1.4.0/doc/build/html/_sources/cmdusage.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-1.4.0/doc/build/html/_sources/configuration.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-1.4.0/doc/build/html/_sources/description.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-1.4.0/doc/build/html/_sources/examples.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-1.4.0/doc/build/html/_sources/extrametadata.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-1.4.0/doc/build/html/_sources/index.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-1.4.0/doc/build/html/_sources/indexers.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-1.4.0/doc/build/html/_sources/install.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-1.4.0/doc/build/html/_sources/license.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-1.4.0/doc/build/html/_sources/reference.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-1.4.0/doc/build/html/_sources/searchsyntax.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-1.4.0/doc/build/html/_sources/synopsis.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-1.4.0/doc/build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.771365 metaindex-1.4.0/doc/build/html/_static/
--rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/_static/basic.css
--rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/doctools.js
--rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/_static/documentation_options.js
--rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/file.png
--rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/jquery.js
--rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/_static/language_data.js
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/minus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/_static/nature.css
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/plus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/_static/pygments.css
--rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/searchtools.js
--rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-1.4.0/doc/build/html/_static/underscore.js
--rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/addons.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/changelog.html
--rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/cmdusage.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/configuration.html
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/description.html
--rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/examples.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/extrametadata.html
--rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/genindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/index.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/indexers.html
--rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/install.html
--rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/license.html
--rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/objects.inv
--rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/reference.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/search.html
--rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/searchindex.js
--rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/searchsyntax.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/synopsis.html
--rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-1.4.0/doc/build/html/usage.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-1.4.0/doc/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-1.4.0/doc/make.bat
--rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-1.4.0/doc/metaindex.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-1.4.0/doc/requirements.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.771365 metaindex-1.4.0/doc/source/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-1.4.0/doc/source/addons.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-1.4.0/doc/source/changelog.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     4299 2022-06-27 12:14:12.000000 metaindex-1.4.0/doc/source/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-1.4.0/doc/source/cmdusage.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-1.4.0/doc/source/conf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     7890 2022-06-19 09:12:03.000000 metaindex-1.4.0/doc/source/configuration.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-1.4.0/doc/source/description.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-1.4.0/doc/source/examples.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-1.4.0/doc/source/extrametadata.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-1.4.0/doc/source/index.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-1.4.0/doc/source/indexers.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-1.4.0/doc/source/install.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-1.4.0/doc/source/license.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-1.4.0/doc/source/reference.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-1.4.0/doc/source/searchsyntax.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-1.4.0/doc/source/synopsis.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-1.4.0/doc/source/usage.rst
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.771365 metaindex-1.4.0/examples/
--rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-1.4.0/examples/indexing.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.771365 metaindex-1.4.0/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    34173 2022-06-30 13:09:45.000000 metaindex-1.4.0/man/metaindex.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)      241 2022-05-11 16:29:10.000000 metaindex-1.4.0/metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    28241 2022-06-27 09:42:56.000000 metaindex-1.4.0/metaindex/cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)    23187 2022-06-28 22:01:56.000000 metaindex-1.4.0/metaindex/configuration.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/metaindex/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    13548 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex/docs/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)    50783 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex/docs/metaindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     2880 2022-06-19 08:49:08.000000 metaindex-1.4.0/metaindex/find.py
--rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-1.4.0/metaindex/fuse.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-1.4.0/metaindex/humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)    17892 2022-05-29 12:08:18.000000 metaindex-1.4.0/metaindex/indexer.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/metaindex/indexers/
--rw-r--r--   0 robert    (1000) robert    (1000)      472 2022-06-28 21:59:17.000000 metaindex-1.4.0/metaindex/indexers/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1189 2022-05-04 19:09:05.000000 metaindex-1.4.0/metaindex/indexers/abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-1.4.0/metaindex/indexers/audio.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4930 2022-04-30 13:11:52.000000 metaindex-1.4.0/metaindex/indexers/collections.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6003 2022-06-27 12:23:21.000000 metaindex-1.4.0/metaindex/indexers/comicbook.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-1.4.0/metaindex/indexers/epub.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3810 2022-04-30 12:58:34.000000 metaindex-1.4.0/metaindex/indexers/filetags.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4354 2022-06-27 12:21:13.000000 metaindex-1.4.0/metaindex/indexers/gpx.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1686 2022-05-04 19:09:52.000000 metaindex-1.4.0/metaindex/indexers/html.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3238 2022-05-29 12:11:11.000000 metaindex-1.4.0/metaindex/indexers/images.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2711 2022-06-28 22:04:20.000000 metaindex-1.4.0/metaindex/indexers/ooxml.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2799 2022-06-28 22:03:27.000000 metaindex-1.4.0/metaindex/indexers/opendocument.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6824 2022-05-11 17:43:40.000000 metaindex-1.4.0/metaindex/indexers/pdf.py
--rw-r--r--   0 robert    (1000) robert    (1000)    10686 2022-03-15 20:14:03.000000 metaindex-1.4.0/metaindex/indexers/ruleindexer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4544 2022-06-12 13:26:36.000000 metaindex-1.4.0/metaindex/json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1497 2022-06-24 05:14:18.000000 metaindex-1.4.0/metaindex/logger.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6538 2022-06-27 12:11:23.000000 metaindex-1.4.0/metaindex/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3407 2022-05-10 20:51:51.000000 metaindex-1.4.0/metaindex/ocr.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1980 2022-06-27 12:22:12.000000 metaindex-1.4.0/metaindex/opf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     7384 2022-06-19 09:06:14.000000 metaindex-1.4.0/metaindex/query.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12579 2022-06-24 08:59:55.000000 metaindex-1.4.0/metaindex/shared.py
--rw-r--r--   0 robert    (1000) robert    (1000)    15243 2022-06-19 09:01:06.000000 metaindex-1.4.0/metaindex/sql.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3194 2022-03-09 18:56:27.000000 metaindex-1.4.0/metaindex/stores.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2022-06-30 13:08:55.000000 metaindex-1.4.0/metaindex/version.py
--rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-1.4.0/metaindex/xmlproxy.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3904 2022-04-30 13:45:18.000000 metaindex-1.4.0/metaindex/yaml.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/metaindex.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     4747 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4369 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       49 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      241 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       29 2022-06-30 13:09:45.000000 metaindex-1.4.0/metaindex.egg-info/top_level.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/misc/
--rw-r--r--   0 robert    (1000) robert    (1000)     1900 2022-06-19 08:21:37.000000 metaindex-1.4.0/misc/metaindex.conf
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/misc/ranger_metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-1.4.0/misc/ranger_metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)      737 2021-09-01 18:34:21.000000 metaindex-1.4.0/misc/ranger_metaindex/linemode.py
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2022-06-30 13:09:45.774698 metaindex-1.4.0/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     3586 2022-05-20 13:17:14.000000 metaindex-1.4.0/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2022-06-30 13:09:45.774698 metaindex-1.4.0/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     4679 2022-05-26 07:51:15.000000 metaindex-1.4.0/tests/test_cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-1.4.0/tests/test_cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-1.4.0/tests/test_cleanup.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-1.4.0/tests/test_collect.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-1.4.0/tests/test_humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-1.4.0/tests/test_indexers.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-1.4.0/tests/test_json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8020 2022-05-26 08:16:32.000000 metaindex-1.4.0/tests/test_query.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-1.4.0/tests/test_ruleindexer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     5001 2022-03-07 12:01:02.000000 metaindex-1.4.0/tests/test_sqlaccess.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)     4488 2023-05-11 18:10:58.000000 metaindex-2.0.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.0.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.0.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     5107 2023-05-11 18:12:32.776761 metaindex-2.0.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4284 2023-05-11 18:09:52.000000 metaindex-2.0.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.763427 metaindex-2.0.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.0.0/doc/Makefile
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.763427 metaindex-2.0.0/doc/build/
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.766761 metaindex-2.0.0/doc/build/doctrees/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/addons.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/changelog.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/cmdoptions.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/cmdusage.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/configuration.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/description.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/examples.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/extrametadata.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/index.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/indexers.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/install.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.0.0/doc/build/doctrees/license.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/reference.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/searchsyntax.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/synopsis.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/doctrees/usage.doctree
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.766761 metaindex-2.0.0/doc/build/html/
+-rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/.buildinfo
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.770094 metaindex-2.0.0/doc/build/html/_sources/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.0.0/doc/build/html/_sources/addons.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.0.0/doc/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.0.0/doc/build/html/_sources/cmdoptions.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.0.0/doc/build/html/_sources/cmdusage.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.0.0/doc/build/html/_sources/configuration.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.0.0/doc/build/html/_sources/description.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.0.0/doc/build/html/_sources/examples.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.0.0/doc/build/html/_sources/extrametadata.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.0.0/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.0.0/doc/build/html/_sources/indexers.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.0.0/doc/build/html/_sources/install.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.0.0/doc/build/html/_sources/license.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.0.0/doc/build/html/_sources/reference.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.0.0/doc/build/html/_sources/searchsyntax.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.0.0/doc/build/html/_sources/synopsis.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.0.0/doc/build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.770094 metaindex-2.0.0/doc/build/html/_static/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/basic.css
+-rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/doctools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/documentation_options.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/file.png
+-rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/jquery.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/language_data.js
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/minus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/nature.css
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/plus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/_static/pygments.css
+-rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.0.0/doc/build/html/_static/underscore.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/addons.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/changelog.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/cmdusage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/configuration.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/description.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/examples.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/extrametadata.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/genindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/index.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/indexers.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/install.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/license.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/objects.inv
+-rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/reference.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/search.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/searchindex.js
+-rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/searchsyntax.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/synopsis.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.0.0/doc/build/html/usage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.0.0/doc/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.0.0/doc/make.bat
+-rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.0.0/doc/metaindex.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.0.0/doc/requirements.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.770094 metaindex-2.0.0/doc/source/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.0.0/doc/source/addons.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.0.0/doc/source/changelog.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     5130 2023-05-11 18:09:52.000000 metaindex-2.0.0/doc/source/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.0.0/doc/source/cmdusage.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.0.0/doc/source/conf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     7739 2023-05-11 18:09:52.000000 metaindex-2.0.0/doc/source/configuration.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.0.0/doc/source/description.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.0.0/doc/source/examples.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.0.0/doc/source/extrametadata.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.0.0/doc/source/index.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.0.0/doc/source/indexers.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.0.0/doc/source/install.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.0.0/doc/source/license.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.0.0/doc/source/reference.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.0.0/doc/source/searchsyntax.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.0.0/doc/source/synopsis.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.0.0/doc/source/usage.rst
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/examples/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.0.0/examples/indexing.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    34927 2023-05-11 18:12:32.000000 metaindex-2.0.0/man/metaindex.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)      247 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    15817 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12235 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/client.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    23509 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/configuration.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/metaindex/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex/docs/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    52404 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex/docs/metaindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/find.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.0.0/metaindex/fuse.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.0.0/metaindex/humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    15257 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/indexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/metaindex/indexers/
+-rw-r--r--   0 robert    (1000) robert    (1000)      472 2022-06-28 21:59:17.000000 metaindex-2.0.0/metaindex/indexers/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.0.0/metaindex/indexers/abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.0.0/metaindex/indexers/audio.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4953 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/indexers/collections.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6003 2022-06-27 12:23:21.000000 metaindex-2.0.0/metaindex/indexers/comicbook.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.0.0/metaindex/indexers/epub.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3810 2022-04-30 12:58:34.000000 metaindex-2.0.0/metaindex/indexers/filetags.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4354 2022-06-27 12:21:13.000000 metaindex-2.0.0/metaindex/indexers/gpx.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1686 2022-05-04 19:09:52.000000 metaindex-2.0.0/metaindex/indexers/html.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3238 2022-05-29 12:11:11.000000 metaindex-2.0.0/metaindex/indexers/images.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2711 2022-06-28 22:04:20.000000 metaindex-2.0.0/metaindex/indexers/ooxml.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2799 2022-06-28 22:03:27.000000 metaindex-2.0.0/metaindex/indexers/opendocument.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6824 2022-05-11 17:43:40.000000 metaindex-2.0.0/metaindex/indexers/pdf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    10686 2022-03-15 20:14:03.000000 metaindex-2.0.0/metaindex/indexers/ruleindexer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4560 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/logger.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8767 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3407 2022-05-10 20:51:51.000000 metaindex-2.0.0/metaindex/ocr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2017 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/opf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/proto.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    25764 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/server.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4214 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/shared.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/stores.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-11 18:10:04.000000 metaindex-2.0.0/metaindex/version.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.0.0/metaindex/xmlproxy.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3920 2023-05-11 18:09:52.000000 metaindex-2.0.0/metaindex/yaml.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.773427 metaindex-2.0.0/metaindex.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     5107 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      241 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-05-11 18:12:32.000000 metaindex-2.0.0/metaindex.egg-info/top_level.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/misc/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.0.0/misc/metaindex.conf
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/misc/ranger_metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.0.0/misc/ranger_metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.0.0/misc/ranger_metaindex/linemode.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-11 18:12:32.776761 metaindex-2.0.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     3667 2023-05-11 18:09:52.000000 metaindex-2.0.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 18:12:32.776761 metaindex-2.0.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.0.0/tests/test_abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.0.0/tests/test_cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.0.0/tests/test_cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.0.0/tests/test_cleanup.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.0.0/tests/test_collect.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.0.0/tests/test_humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.0.0/tests/test_indexers.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.0.0/tests/test_json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.0.0/tests/test_ruleindexer.py
```

### Comparing `metaindex-1.4.0/CHANGELOG.md` & `metaindex-2.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
 
+## 2.0.0
+### Changed
+- Drastic refactoring, back-end changed to xapian
+
+## 1.5.0
+### Changed
+- Updated the ABC indexer to match the specs of version 2.1 better
+
+
 ## 1.4.0
 ### Changed
 - `Cache.cleanup` accepts a list of paths to limit the clean-up to
 - `metaindex index -m` expects a list of paths to clean up.
 
 ### Added
 - Support for metadata from GPX files
```

### Comparing `metaindex-1.4.0/LICENSE` & `metaindex-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/PKG-INFO` & `metaindex-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 1.4.0
+Version: 2.0.0
 Summary: Utilities to tag files
-Home-page: https://github.com/vonshednob/metaindex
+Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
@@ -56,15 +54,15 @@
 
 To install metaindex either install it directly through pypi:
 
     pip install metaindex
 
 Or clone the repository and install that then through pip:
 
-    git clone https://github.com/vonshednob/metaindex
+    git clone https://codeberg.org/vonshednob/metaindex
     cd metaindex
     pip install .
 
 Most modules are optional. If you, for example, want to use metaindex for audio
 files and PDFs, you will have to install it like this:
 
     pip install metaindex[pdf,audio]
@@ -91,24 +89,36 @@
 
 There is also an experimental FuseFS filesystem. To be able to use it, you
 will have to specify ``fuse`` as an additional module:
 
     pip install .[all,fuse]
 
 
+### Server dependencies
+
+If you just want to connect to another instance of the metaindex server,
+you are ready to go.  
+More likely though you will have to install [Xapian](https://xapian.org/)
+and its Python3 bindings. Please follow the usual way of your OS to install
+both.
+
+For example, on Archlinux you'd `pacman -S xapian python-xapian`. On
+debian-likes it would be `apt install python3-xapian`.
+
+
 ## Usage
 
 Before you can use metaindex to search for files, you have to initialize the
 cache by telling it where your files to index are, for example:
 
     metaindex index --recursive --index ~/Pictures
 
 Afterwards you can start searching for files by metadata, like this:
 
-    metaindex find 
+    metaindex find
 
 
 ## Searching
 
 Search queries for use with `metaindex find` allow you to search
 
  - for files that have a metadata tag: `metaindex find resolution?`
@@ -146,9 +156,7 @@
     cache.wait_for_reload()
 
     searchquery = 'mimetype:image title?'
 
     for entry in cache.find(searchquery):
         print(entry.path)
 
-
-
```

### Comparing `metaindex-1.4.0/README.md` & `metaindex-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 To install metaindex either install it directly through pypi:
 
     pip install metaindex
 
 Or clone the repository and install that then through pip:
 
-    git clone https://github.com/vonshednob/metaindex
+    git clone https://codeberg.org/vonshednob/metaindex
     cd metaindex
     pip install .
 
 Most modules are optional. If you, for example, want to use metaindex for audio
 files and PDFs, you will have to install it like this:
 
     pip install metaindex[pdf,audio]
@@ -61,24 +61,36 @@
 
 There is also an experimental FuseFS filesystem. To be able to use it, you
 will have to specify ``fuse`` as an additional module:
 
     pip install .[all,fuse]
 
 
+### Server dependencies
+
+If you just want to connect to another instance of the metaindex server,
+you are ready to go.  
+More likely though you will have to install [Xapian](https://xapian.org/)
+and its Python3 bindings. Please follow the usual way of your OS to install
+both.
+
+For example, on Archlinux you'd `pacman -S xapian python-xapian`. On
+debian-likes it would be `apt install python3-xapian`.
+
+
 ## Usage
 
 Before you can use metaindex to search for files, you have to initialize the
 cache by telling it where your files to index are, for example:
 
     metaindex index --recursive --index ~/Pictures
 
 Afterwards you can start searching for files by metadata, like this:
 
-    metaindex find 
+    metaindex find
 
 
 ## Searching
 
 Search queries for use with `metaindex find` allow you to search
 
  - for files that have a metadata tag: `metaindex find resolution?`
```

### Comparing `metaindex-1.4.0/doc/Makefile` & `metaindex-2.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/addons.doctree` & `metaindex-2.0.0/doc/build/doctrees/addons.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/changelog.doctree` & `metaindex-2.0.0/doc/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/cmdoptions.doctree` & `metaindex-2.0.0/doc/build/doctrees/cmdoptions.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/cmdusage.doctree` & `metaindex-2.0.0/doc/build/doctrees/cmdusage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/configuration.doctree` & `metaindex-2.0.0/doc/build/doctrees/configuration.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/description.doctree` & `metaindex-2.0.0/doc/build/doctrees/description.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/environment.pickle` & `metaindex-2.0.0/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/examples.doctree` & `metaindex-2.0.0/doc/build/doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/extrametadata.doctree` & `metaindex-2.0.0/doc/build/doctrees/extrametadata.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/index.doctree` & `metaindex-2.0.0/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/indexers.doctree` & `metaindex-2.0.0/doc/build/doctrees/indexers.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/install.doctree` & `metaindex-2.0.0/doc/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/license.doctree` & `metaindex-2.0.0/doc/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/reference.doctree` & `metaindex-2.0.0/doc/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/searchsyntax.doctree` & `metaindex-2.0.0/doc/build/doctrees/searchsyntax.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/synopsis.doctree` & `metaindex-2.0.0/doc/build/doctrees/synopsis.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/doctrees/usage.doctree` & `metaindex-2.0.0/doc/build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/addons.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/addons.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/cmdoptions.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/cmdoptions.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/cmdusage.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/cmdusage.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/configuration.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/configuration.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/description.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/description.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/examples.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/extrametadata.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/extrametadata.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/indexers.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/indexers.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/install.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/reference.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_sources/searchsyntax.rst.txt` & `metaindex-2.0.0/doc/build/html/_sources/searchsyntax.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/basic.css` & `metaindex-2.0.0/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/doctools.js` & `metaindex-2.0.0/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/jquery-3.5.1.js` & `metaindex-2.0.0/doc/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/jquery.js` & `metaindex-2.0.0/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/language_data.js` & `metaindex-2.0.0/doc/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/nature.css` & `metaindex-2.0.0/doc/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/pygments.css` & `metaindex-2.0.0/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/searchtools.js` & `metaindex-2.0.0/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/underscore-1.13.1.js` & `metaindex-2.0.0/doc/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/_static/underscore.js` & `metaindex-2.0.0/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/addons.html` & `metaindex-2.0.0/doc/build/html/addons.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/changelog.html` & `metaindex-2.0.0/doc/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/cmdoptions.html` & `metaindex-2.0.0/doc/build/html/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/cmdusage.html` & `metaindex-2.0.0/doc/build/html/cmdusage.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/configuration.html` & `metaindex-2.0.0/doc/build/html/configuration.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/description.html` & `metaindex-2.0.0/doc/build/html/description.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/examples.html` & `metaindex-2.0.0/doc/build/html/examples.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/extrametadata.html` & `metaindex-2.0.0/doc/build/html/extrametadata.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/genindex.html` & `metaindex-2.0.0/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/index.html` & `metaindex-2.0.0/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/indexers.html` & `metaindex-2.0.0/doc/build/html/indexers.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/install.html` & `metaindex-2.0.0/doc/build/html/install.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/license.html` & `metaindex-2.0.0/doc/build/html/license.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/objects.inv` & `metaindex-2.0.0/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/reference.html` & `metaindex-2.0.0/doc/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/search.html` & `metaindex-2.0.0/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/searchindex.js` & `metaindex-2.0.0/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/searchsyntax.html` & `metaindex-2.0.0/doc/build/html/searchsyntax.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/synopsis.html` & `metaindex-2.0.0/doc/build/html/synopsis.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/build/html/usage.html` & `metaindex-2.0.0/doc/build/html/usage.html`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/cmdoptions.rst` & `metaindex-2.0.0/doc/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/make.bat` & `metaindex-2.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/metaindex.rst` & `metaindex-2.0.0/doc/metaindex.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/addons.rst` & `metaindex-2.0.0/doc/source/addons.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/cmdusage.rst` & `metaindex-2.0.0/doc/source/cmdusage.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 Index some directories
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To index you ``Documents`` and ``Pictures`` folder recursively::
 
-  metaindex index -r -i ~/Documents ~/Pictures
-
-
-Reindex all files
-~~~~~~~~~~~~~~~~~
-
-To only update the metadata from all known files::
-
-  metaindex index -i
+  metaindex index -r ~/Documents ~/Pictures
 
 
 Find all files
 ~~~~~~~~~~~~~~
 
 List all files that are in cache::
 
@@ -23,22 +15,21 @@
 
 
 Find file by mimetype
 ~~~~~~~~~~~~~~~~~~~~~
 
 Searching for all ``image/*`` mimetypes can be accomplished by this::
 
-  metaindex find mimetype:^image/
+  metaindex find mimetype:image/
 
 
 Listing metadata
 ~~~~~~~~~~~~~~~~
 
-To list all metadata tags and values of all odt files::
+To list all metadata tags and values of all image files::
 
-  metaindex find -t -- "filename:odt$"
+  metaindex find -t -- "ext:odt$"
 
 List the resolutions of all files that have the ``resolution`` metadata tag::
 
   metaindex find -t resolution -- "resolution?"
 
-
```

### Comparing `metaindex-1.4.0/doc/source/conf.py` & `metaindex-2.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/configuration.rst` & `metaindex-2.0.0/doc/source/configuration.rst`

 * *Files 7% similar despite different names*

```diff
@@ -65,27 +65,14 @@
 
   ``index-unknown``
     Whether or not to add files to the index for which no meaningful
     metadata could be extracted from the indexers or any sidecar files.
 
     Defaults to ``yes``.
 
-  ``ignore-tags``
-    What (automatically extracted) tags to not add to the cache and thus
-    prevent them being searchable. Comma-separated list of the tags.
-    To add to the ignored tags, instead of redefining them, include the
-    special value ``*`` in the listing.
-
-    If you want to exclude a group of tags that have the same prefix or
-    suffix, you can add a ``*`` to the end or start of the tag
-    respectively. E.g. to exclude all tags that come from Nikon in the EXIF
-    metadata group, this would do what you want: ``exif.nikon*``.
-
-    Defaults to: ``Exif.Image.StripByteCounts, Exif.Image.StripOffsets, Exif.Photo.makernote, Exif.Thumbnail.*, Exif.Sony1.0x*, Exif.Nikonsi*, Exif.Nikoncb*, Exif.Nikon3.linearizationtable, Exif.Nikon3.contrastcurve, Exif.Nikon3.0x*, Exif.Nikonfi.0x*, Exif.Canon.0x*, Exif.Canon.camerainfo, Exif.Canon.afinfo3``.
-
   ``ignore-indexers``
     A comma separated list of indexers by name that you do not want to use.
     By default this list is empty.
 
     Run ``metaindex --list`` to see what indexers will be used by default.
 
   ``preferred-sidecar-format``
@@ -99,14 +86,26 @@
 
   ``mimetypes``
     If you have additional mimetypes that you would like metaindex to know,
     this is the option you can use to point to additional mimetype files.
     To add multiple files, separate them by a newline. No matter what files
     you provide here, you system's mimetype file will always be used.
 
+  ``implicit-tags``
+    Some tags should be accessible during search, even when not searching
+    explicitly for that tag (e.g. searching for "the two towers" should
+    find the book, even if you don't explicitly search for ``title:"the
+    two towers"``). This option selects the tags that should always be
+    included in the search.
+
+    Note that this option applies during indexing. Changing it after
+    indexing will not change the behaviour of the search.
+
+    Defaults to: ``author, title, tag, type, series, filename``.
+
   ``ocr``
     Whether or not OCR (optical character recognition) should be enabled.
     For this to work you must have installed the ``ocr`` requirements.
 
     This option can be set to ``yes`` to enable OCR for everything, but you
     can also fine-tune it by setting the option to a list of mimetypes,
     file suffices, or names of indexers that are allowed to run OCR. For
@@ -138,20 +137,24 @@
 Synonyms
 ~~~~~~~~
 
 Some metadata fields have less convenient names than others, but might
 semantically be the same. For example, ``Xmp.xmp.CreatorTool`` and
 ``pdf.Creator`` both mean "The program that was used to create this file".
 
-For convenience it is possible to define synonyms, so you only have to
-search for ``author`` when you mean to search for ``id3.artist``,
-``pdf.Author``, or ``Exif.Image.Artist``.
+To simplify the search it is possible to define synonyms for these metadata fields.
+For example the tag ``author`` could point to the fields ``id3.artist``,
+``pdf.Author``, and ``Exif.Image.Artist``.
+
+Note that metaindex will only allow you to search metadata fields by their
+synonym. That means you can search for ``author:tim``, but not for
+``pdf.Author:tim``.
 
 The section ``[Synonyms]`` in the configuration file is the place to define
-these synonyms. Here are the defaults, that you don’t have to set up::
+the synonyms. Here are the defaults, that you don’t have to set up::
 
   [Synonyms]
   author = extra.author, extra.artist, extra.creator, id3.artist, pdf.Author, rules.author, Exif.Image.Artist, comicbook.writer, xmp.dc.name
   type = extra.type, rules.type, xmp.dc.type
   date = extra.date, rules.date, comicbook.date
   title = extra.title, opf.title, id3.title, rules.title, pdf.Title, filetags.title, abs.title, comicbook.title, Xmp.dc.title
   tag = extra.tag, extra.tags, pdf.Keywords, pdf.Categories, Xmp.dc.subject, extra.subject, rules.tags, rules.tag, rules.subject, pdf.Subject, comicbook.tags, opf.subject
```

### Comparing `metaindex-1.4.0/doc/source/description.rst` & `metaindex-2.0.0/doc/source/description.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/examples.rst` & `metaindex-2.0.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/extrametadata.rst` & `metaindex-2.0.0/doc/source/extrametadata.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/indexers.rst` & `metaindex-2.0.0/doc/source/indexers.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/install.rst` & `metaindex-2.0.0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/reference.rst` & `metaindex-2.0.0/doc/source/reference.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/doc/source/searchsyntax.rst` & `metaindex-2.0.0/doc/source/searchsyntax.rst`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/examples/indexing.py` & `metaindex-2.0.0/examples/indexing.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/man/metaindex.1` & `metaindex-2.0.0/man/metaindex.1`

 * *Files 4% similar despite different names*

```diff
@@ -94,17 +94,41 @@
 .UNINDENT
 .UNINDENT
 .sp
 More file types can be supported through the use of addons.
 .sp
 User provided extra metadata is supported, if it’s provided in the same
 directory as the file and the metadata file is \fB\&.metadata.json\fP\&.
+.SH SERVER
+.sp
+Starting with version \fB0.2.0dev0\fP, requires that the \fBmetaindexserver\fP
+is running to perform any operations like searching or indexing.
+.sp
+In the default configuration the server will be started automatically as soon
+as metaindex needs to connect to the server, but none is running.
+.sp
+However, you may also launch the server process ahead in time like this:
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+metaindexserver \-\-detach
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.sp
+It supports a few parameters like \fB\-c\fP to change the configuration file
+and \fB\-l\fP to change the log level.
+.sp
+To stop a running server, run \fBmetaindexserver \-\-stop\fP or send it a \fBTERM\fP signal.
 .SH OPTIONS
 .sp
-General parameters are:
+General parameters for \fBmetaindex\fP are:
 .INDENT 0.0
 .INDENT 3.5
 .INDENT 0.0
 .TP
 .B \fB\-c configuration file\fP
 Use this configuration file instead of the one from the default
 location.
@@ -114,14 +138,17 @@
 .TP
 .B \fB\-l loglevel\fP
 Set the level of details shown in logging. Your options are \fBfatal\fP,
 \fBerror\fP, \fBwarning\fP, \fBinfo\fP, and \fBdebug\fP\&. Defaults to \fBwarning\fP\&.
 .TP
 .B \fB\-\-list\fP
 List all available indexers and exit.
+.TP
+.B \fB\-\-compact\fP
+Compact the backend database.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
 metaindex operates in one of the modes \fBindex\fP or \fBfind\fP\&.
 .sp
 If you want to try the experimental filesystem mode, there is also \fBfs\fP\&.
@@ -178,15 +205,15 @@
 This is the operation to index files and store that information in the
 cache:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-metaindex index [\-C] [\-r] [\-p processes] [\-m [paths]] [\-i [paths]]
+metaindex index [\-v[v[v[v]]]] [\-C] [\-r] paths
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 The options to this command are
 .INDENT 0.0
@@ -203,34 +230,48 @@
 option is enabled.
 If \fB\-m\fP is provided, but no paths, all paths in cache will be checked
 for their existence and cleaned up if not found.
 If \fBpaths\fP is \fB\-\fP, the list of files will be read from stdin, one
 file per line.
 By default this option is disabled.
 .TP
-.B \fB\-i [paths]\fP
-Run the indexer on these paths. If no paths are provided, all paths in
-the cache are revisited and checked for changes.
-If \fBpaths\fP is \fB\-\fP, the list of files will be read from stdin, one
-file per line.
-.TP
-.B \fB\-p processes\fP
-By default metaindex will run as many indexer processes in parallel as
-CPUs are available on the computer. This parameter allows you to define
-how many indexers may be run at the same time.
-.TP
 .B \fB\-r\fP
 Run the indexer recursively. That means to visit all files in all
 subdirectories of the paths in the \fB\-i\fP parameter.
+.TP
+.B \fB\-v\fP
+Make the output more verbose. This option can be provided up to four
+times (\fB\-vvvv\fP). The steps are:
+.INDENT 7.0
+.INDENT 3.5
+.INDENT 0.0
+.IP \(bu 2
+No \fB\-v\fP: no output other than errors or information from certain indexers
+.IP \(bu 2
+\fB\-v\fP: print a \fB\&.\fP per file indexed
+.IP \(bu 2
+\fB\-vv\fP: same as \fB\-v\fP and print how many files were indexed in the end
+.IP \(bu 2
+\fB\-vvv\fP: same as \fB\-vv\fP but also show how long it took
+.IP \(bu 2
+\fB\-vvvv\fP: same as \fB\-vvv\fP but print the path of each indexed file instead of just a \fB\&.\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.TP
+.B \fBpaths\fP
+Run the indexer on these paths.
+If \fBpaths\fP is \fB\-\fP, the list of files will be read from stdin, one
+file per line.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS Filesystem (fs)
 .sp
-On Linux you can try the experimental feature of mounting a FuseFS that
+On Linux you can try the \fBexperimental\fP feature of mounting a FuseFS that
 will give you a structured access to your files through their metadata:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 metaindex fs [command] [mount point]
@@ -334,27 +375,14 @@
 .TP
 .B \fBindex\-unknown\fP
 Whether or not to add files to the index for which no meaningful
 metadata could be extracted from the indexers or any sidecar files.
 .sp
 Defaults to \fByes\fP\&.
 .TP
-.B \fBignore\-tags\fP
-What (automatically extracted) tags to not add to the cache and thus
-prevent them being searchable. Comma\-separated list of the tags.
-To add to the ignored tags, instead of redefining them, include the
-special value \fB*\fP in the listing.
-.sp
-If you want to exclude a group of tags that have the same prefix or
-suffix, you can add a \fB*\fP to the end or start of the tag
-respectively. E.g. to exclude all tags that come from Nikon in the EXIF
-metadata group, this would do what you want: \fBexif.nikon*\fP\&.
-.sp
-Defaults to: \fBExif.Image.StripByteCounts, Exif.Image.StripOffsets, Exif.Photo.makernote, Exif.Thumbnail.*, Exif.Sony1.0x*, Exif.Nikonsi*, Exif.Nikoncb*, Exif.Nikon3.linearizationtable, Exif.Nikon3.contrastcurve, Exif.Nikon3.0x*, Exif.Nikonfi.0x*, Exif.Canon.0x*, Exif.Canon.camerainfo, Exif.Canon.afinfo3\fP\&.
-.TP
 .B \fBignore\-indexers\fP
 A comma separated list of indexers by name that you do not want to use.
 By default this list is empty.
 .sp
 Run \fBmetaindex \-\-list\fP to see what indexers will be used by default.
 .TP
 .B \fBpreferred\-sidecar\-format\fP
@@ -368,14 +396,26 @@
 .TP
 .B \fBmimetypes\fP
 If you have additional mimetypes that you would like metaindex to know,
 this is the option you can use to point to additional mimetype files.
 To add multiple files, separate them by a newline. No matter what files
 you provide here, you system\(aqs mimetype file will always be used.
 .TP
+.B \fBimplicit\-tags\fP
+Some tags should be accessible during search, even when not searching
+explicitly for that tag (e.g. searching for \(dqthe two towers\(dq should
+find the book, even if you don\(aqt explicitly search for \fBtitle:\(dqthe
+two towers\(dq\fP). This option selects the tags that should always be
+included in the search.
+.sp
+Note that this option applies during indexing. Changing it after
+indexing will not change the behaviour of the search.
+.sp
+Defaults to: \fBauthor, title, tag, type, series, filename\fP\&.
+.TP
 .B \fBocr\fP
 Whether or not OCR (optical character recognition) should be enabled.
 For this to work you must have installed the \fBocr\fP requirements.
 .sp
 This option can be set to \fByes\fP to enable OCR for everything, but you
 can also fine\-tune it by setting the option to a list of mimetypes,
 file suffices, or names of indexers that are allowed to run OCR. For
@@ -407,20 +447,24 @@
 .UNINDENT
 .SS Synonyms
 .sp
 Some metadata fields have less convenient names than others, but might
 semantically be the same. For example, \fBXmp.xmp.CreatorTool\fP and
 \fBpdf.Creator\fP both mean \(dqThe program that was used to create this file\(dq.
 .sp
-For convenience it is possible to define synonyms, so you only have to
-search for \fBauthor\fP when you mean to search for \fBid3.artist\fP,
-\fBpdf.Author\fP, or \fBExif.Image.Artist\fP\&.
+To simplify the search it is possible to define synonyms for these metadata fields.
+For example the tag \fBauthor\fP could point to the fields \fBid3.artist\fP,
+\fBpdf.Author\fP, and \fBExif.Image.Artist\fP\&.
+.sp
+Note that metaindex will only allow you to search metadata fields by their
+synonym. That means you can search for \fBauthor:tim\fP, but not for
+\fBpdf.Author:tim\fP\&.
 .sp
 The section \fB[Synonyms]\fP in the configuration file is the place to define
-these synonyms. Here are the defaults, that you don’t have to set up:
+the synonyms. Here are the defaults, that you don’t have to set up:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 [Synonyms]
 author = extra.author, extra.artist, extra.creator, id3.artist, pdf.Author, rules.author, Exif.Image.Artist, comicbook.writer, xmp.dc.name
@@ -1146,28 +1190,15 @@
 .sp
 To index you \fBDocuments\fP and \fBPictures\fP folder recursively:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-metaindex index \-r \-i ~/Documents ~/Pictures
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.SS Reindex all files
-.sp
-To only update the metadata from all known files:
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-metaindex index \-i
+metaindex index \-r ~/Documents ~/Pictures
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Find all files
 .sp
 List all files that are in cache:
@@ -1185,28 +1216,28 @@
 .sp
 Searching for all \fBimage/*\fP mimetypes can be accomplished by this:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-metaindex find mimetype:^image/
+metaindex find mimetype:image/
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Listing metadata
 .sp
-To list all metadata tags and values of all odt files:
+To list all metadata tags and values of all image files:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-metaindex find \-t \-\- \(dqfilename:odt$\(dq
+metaindex find \-t \-\- \(dqext:odt$\(dq
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 List the resolutions of all files that have the \fBresolution\fP metadata tag:
 .INDENT 0.0
```

### Comparing `metaindex-1.4.0/metaindex/configuration.py` & `metaindex-2.0.0/metaindex/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,54 +17,42 @@
 
 HOME = pathlib.Path().home()
 PROGRAMNAME = 'metaindex'
 CONFFILENAME = PROGRAMNAME + os.path.extsep + 'conf'
 CONFIGFILE = HOME / ".config" / CONFFILENAME
 CACHEPATH = HOME / ".cache" / PROGRAMNAME
 DATAPATH = HOME / ".local" / "share" / PROGRAMNAME
+SOCKETPATH = HOME / ".local" / "state"
 
 IGNORE_DIRS = [".git", ".svn", ".hg", ".bzr",
                "System Volume Information",
                ".stfolder",
                "__pycache__",
                "__MACOSX"]
 IGNORE_FILES = ['*.aux', '*.toc', '*.out', '*.log', '*.nav',
                 '*.exe', '*.sys',
                 '*.bat', '*.ps',
                 '*.sh', '*.fish',
                 '*~', '*.swp', '*.bak', '*.sav', '*.backup', '*.old',
                 '*.old', '*.orig', '*.rej',
                 'tags', '*.log',
                 '*.a', '*.out', '*.o', '*.obj', '*.so']
-IGNORE_TAGS = {"Exif.Image.StripByteCounts",
-               "Exif.Image.StripOffsets",
-               "Exif.Photo.makernote",
-               "Exif.Thumbnail.*",
-               "Exif.Canon.0x*",
-               "Exif.Canon.camerainfo",
-               "Exif.Canon.afinfo3",
-               "Exif.Sony1.0x*",
-               "Exif.Nikonsi*",
-               "Exif.Nikoncb*",
-               "Exif.Nikon3.linearizationtable",
-               "Exif.Nikon3.contrastcurve",
-               "Exif.Nikon3.0x*",
-               "Exif.Nikonfi.0x*",
-               }
+IMPLICIT_TAGS = ['author', 'type', 'title', 'tag', 'series', 'filename']
 SYNONYMS = {'author': {
                 "extra.author",
                 "extra.artist",
                 "extra.creator",
                 "id3.artist",
                 "pdf.author",
                 "rules.author",
                 "exif.image.artist",
                 "comicbook.writer",
                 "xmp.dc.name",
                 "gpx.author",
+                "opf.creator",
                 "opendocument.creator",
                 "officeopenxml.creator",
                 },
             'type': {
                 "extra.type",
                 "rules.type",
                 "xmp.dc.type",
@@ -90,18 +78,18 @@
                 "gpx.name",
                 "opendocument.title",
                 "officeopenxml.title",
                 },
             'tag': {
                 "extra.tag",
                 "extra.tags",
+                "extra.subject",
                 "pdf.keywords",
                 "pdf.categories",
                 "xmp.dc.subject",
-                "extra.subject",
                 "rules.tags",
                 "rules.tag",
                 "rules.subject",
                 "pdf.Subject",
                 "comicbook.tags",
                 "opf.subject",
                 "gpx.keyword",
@@ -127,59 +115,74 @@
             'series': {
                 'extra.series',
                 'comicbook.series',
                 },
             'series_index': {
                 'extra.series_index',
                 'comicbook.number',
-                }
+                },
             }
 
 
 try:
     from xdg import BaseDirectory
     CONFIGFILE = pathlib.Path(BaseDirectory.load_first_config(CONFFILENAME) or CONFIGFILE)
     CACHEPATH = pathlib.Path(BaseDirectory.save_cache_path(PROGRAMNAME) or CACHEPATH)
     DATAPATH = pathlib.Path(BaseDirectory.save_data_path(PROGRAMNAME) or DATAPATH)
+    SOCKETPATH = pathlib.Path(BaseDirectory.get_runtime_dir() or SOCKETPATH)
 except ImportError:
     BaseDirectory = None
 
+SOCKETPATH /= SOCKETPATH / (PROGRAMNAME + '.sock')
 
 ADDONSPATH = DATAPATH / "addons"
+LOGFILEPATH = CACHEPATH / "metaindex.log"
+LOGLEVEL = 'WARNING'
 
 SECTION_GENERAL = 'General'
 SECTION_SYNONYMS = 'Synonyms'
 SECTION_INCLUDE = 'Include'
+SECTION_SERVER = 'Server'
 CONFIG_CACHE = 'cache'
+CONFIG_SOCKET = 'socket'
 CONFIG_RECURSIVE_EXTRA_METADATA = 'recursive-extra-metadata'
 CONFIG_COLLECTION_METADATA = 'collection-metadata'
 CONFIG_IGNORE_DIRS = 'ignore-dirs'
 CONFIG_IGNORE_FILES = 'ignore-files'
 CONFIG_ACCEPT_FILES = 'accept-files'
 CONFIG_INDEX_UNKNOWN = 'index-unknown'
 CONFIG_IGNORE_INDEXERS = 'ignore-indexers'
-CONFIG_IGNORE_TAGS = 'ignore-tags'
 CONFIG_PREFERRED_SIDECAR_FORMAT = 'preferred-sidecar-format'
 CONFIG_OCR = 'ocr'
 CONFIG_FULLTEXT = 'fulltext'
 CONFIG_MIMETYPES = 'mimetypes'
+CONFIG_IMPLICIT_TAGS = 'implicit-tags'
+CONFIG_LOGFILE = 'logfile'
+CONFIG_LOGLEVEL = 'loglevel'
+CONFIG_AUTOSTART = 'autostart'
 
 CONF_DEFAULTS = {SECTION_GENERAL: {
                     CONFIG_CACHE: str(CACHEPATH),
+                    CONFIG_SOCKET: str(SOCKETPATH),
                     CONFIG_RECURSIVE_EXTRA_METADATA: "yes",
                     CONFIG_COLLECTION_METADATA: ".metadata, metadata",
                     CONFIG_IGNORE_DIRS: "\n".join(IGNORE_DIRS),
                     CONFIG_IGNORE_FILES: "\n".join(IGNORE_FILES),
                     CONFIG_ACCEPT_FILES: '',
                     CONFIG_INDEX_UNKNOWN: 'yes',
                     CONFIG_IGNORE_INDEXERS: '',
-                    CONFIG_IGNORE_TAGS: ", ".join(IGNORE_TAGS),
                     CONFIG_PREFERRED_SIDECAR_FORMAT: '.json, .opf',
                     CONFIG_OCR: 'no',
                     CONFIG_FULLTEXT: 'no',
+                    CONFIG_IMPLICIT_TAGS: ', '.join(IMPLICIT_TAGS),
+                 },
+                 SECTION_SERVER: {
+                    CONFIG_LOGFILE: str(LOGFILEPATH),
+                    CONFIG_LOGLEVEL: str(LOGLEVEL),
+                    CONFIG_AUTOSTART: 'yes',
                  },
                  SECTION_SYNONYMS: {k: ', '.join(v)
                                     for k, v in SYNONYMS.items()},
                  SECTION_INCLUDE: {
                  },
                 }
 
@@ -188,15 +191,14 @@
     """Convenience wrapper for configparser"""
     TRUE = ['y', 'yes', '1', 'true', 'on']
     FALSE = ['n', 'no', '0', 'false', 'off']
 
     def __init__(self, conf=None):
         self.conf = conf or configparser.ConfigParser(interpolation=None)
         self._userfile = None
-        self._synonyms = None
 
     def __getitem__(self, group):
         return self.conf[group]
 
     def __contains__(self, item):
         return item in self.conf
 
@@ -278,23 +280,48 @@
         """The OCR facility, as configured by the user"""
         self._update_property(SECTION_GENERAL, CONFIG_OCR)
 
         self.ignore_indexers = []
         """List of all indexers by name that should be ignored"""
         self._update_property(SECTION_GENERAL, CONFIG_IGNORE_INDEXERS)
 
-        self.ignore_tags = set()
-        """List of all tags that should be ignored"""
-        self._update_property(SECTION_GENERAL, CONFIG_IGNORE_TAGS)
+        self.synonyms = {}
+        """Mapping of synonym -> synonymized tags (e.g. author -> pdf.creator)"""
+        self.synonymized = {}
+        """Mapping of synonymized -> synonym (e.g. pdf.creator -> author)"""
+        self._update_property(SECTION_SYNONYMS, None)
+
+        self.accepted_tags = set(sum(list(list(t) for t in self.synonyms.values()),
+                                     start=[]))
+        """The tags that are accepted, ie. not discarded during indexing"""
+
+        self.implicit_tags = set()
+        """Tags whose values should be indexed without a prefix, too"""
+        self._update_property(SECTION_GENERAL, CONFIG_IMPLICIT_TAGS)
 
     def set(self, group, key, value):
         super().set(group, key, value)
         self._update_property(group, key)
 
     def _update_property(self, section, key):
+        if section == SECTION_SYNONYMS:
+            self.synonyms = {}
+            for name in self[SECTION_SYNONYMS]:
+                synonyms = {s for s in self.list(SECTION_SYNONYMS, name) if len(s) > 0}
+                if '*' in synonyms:
+                    synonyms.remove('*')
+                    synonyms |= SYNONYMS.get(name, set())
+                self.synonyms[name] = synonyms
+
+            self.synonymized = {}
+            for synonym, tags in self.synonyms.items():
+                self.synonymized.update({t: synonym for t in tags})
+
+            return
+
         if section != SECTION_GENERAL:
             return
 
         if key == CONFIG_IGNORE_DIRS:
             self.ignore_dirs = self.list(section, key, "", separator="\n")
 
         if key == CONFIG_FULLTEXT:
@@ -343,23 +370,16 @@
                 self.ocr = ocr.TesseractOCR(ocr_opts)
 
         if key == CONFIG_IGNORE_INDEXERS:
             self.ignore_indexers = [indexer
                                     for indexer in self.list(section, key, '')
                                     if len(indexer) > 0]
 
-        if key == CONFIG_IGNORE_TAGS:
-            ignore_tags = {tag.lower()
-                           for tag in self.list(section, key, '')
-                           if len(tag) > 0}
-            if '*' in ignore_tags:
-                ignore_tags.remove('*')
-                ignore_tags |= self.ignore_tags
-                ignore_tags |= IGNORE_TAGS
-            self.ignore_tags = ignore_tags
+        if key == CONFIG_IMPLICIT_TAGS:
+            self.implicit_tags = {t.lower() for t in self.list(section, key)}
 
     @property
     def collection_metadata(self):
         """Return a list of all valid filenames for collection metadata.
 
         The list is ordered by user's preference for sidecar file format and
         name of collection metadata file.
@@ -369,30 +389,14 @@
             if len(lst) > 0:
                 lst = sum([[fn + store.SUFFIX for store in self.get_preferred_sidecar_stores()]
                            for fn in lst
                            if len(fn) > 0], start=[])
             self._collection_metadata = lst
         return self._collection_metadata
 
-    @property
-    def synonyms(self):
-        """Returns a dict of all synonyms and the attributes that they stand for
-
-        E.g. might contain the entry 'title', mapping to ['opf.title', 'id3.title']
-        """
-        if self._synonyms is None:
-            self._synonyms = {}
-            for name in self[SECTION_SYNONYMS]:
-                synonyms = {s for s in self.list(SECTION_SYNONYMS, name) if len(s) > 0}
-                if '*' in synonyms:
-                    synonyms.remove('*')
-                    synonyms |= SYNONYMS.get(name, set())
-                self._synonyms[name] = synonyms
-        return self._synonyms
-
     def expand_synonyms(self, tags):
         """Expand all synonyms of this iterable of tags (or a single tag)
 
         This function will return a set of tags (at least the one(s) you passed
         in), expanding all those tags that are synonyms.
 
         You might call this with a single tag, to expand it to its actual tags,
```

### Comparing `metaindex-1.4.0/metaindex/docs/cmdoptions.html` & `metaindex-2.0.0/metaindex/docs/cmdoptions.html`

 * *Files 2% similar despite different names*

#### Comparing `metaindex-1.4.0/metaindex/docs/cmdoptions.html` & `metaindex-2.0.0/metaindex/docs/cmdoptions.html`

```diff
@@ -1,24 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/"/>
     <title>Options</title>
     <style type="text/css">/*
 :Author: David Goodger (goodger@python.org)
-:Id: $Id: html4css1.css 7952 2016-07-26 18:15:59Z milde $
+:Id: $Id: html4css1.css 8954 2022-01-20 10:10:25Z milde $
 :Copyright: This stylesheet has been placed in the public domain.
 
 Default cascading style sheet for the HTML output of Docutils.
 
-See http://docutils.sf.net/docs/howto/html-stylesheets.html for how to
+See https://docutils.sourceforge.io/docs/howto/html-stylesheets.html for how to
 customize this style sheet.
 */
 
 /* used to remove borders from tables and images */
 .borderless, table.borderless td, table.borderless th {
   border: 0 }
```

### Comparing `metaindex-1.4.0/metaindex/docs/metaindex.html` & `metaindex-2.0.0/metaindex/docs/metaindex.html`

 * *Files 2% similar despite different names*

#### Comparing `metaindex-1.4.0/metaindex/docs/metaindex.html` & `metaindex-2.0.0/metaindex/docs/metaindex.html`

```diff
@@ -1,24 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/"/>
     <title>metaindex</title>
     <style type="text/css">/*
 :Author: David Goodger (goodger@python.org)
-:Id: $Id: html4css1.css 7952 2016-07-26 18:15:59Z milde $
+:Id: $Id: html4css1.css 8954 2022-01-20 10:10:25Z milde $
 :Copyright: This stylesheet has been placed in the public domain.
 
 Default cascading style sheet for the HTML output of Docutils.
 
-See http://docutils.sf.net/docs/howto/html-stylesheets.html for how to
+See https://docutils.sourceforge.io/docs/howto/html-stylesheets.html for how to
 customize this style sheet.
 */
 
 /* used to remove borders from tables and images */
 .borderless, table.borderless td, table.borderless th {
   border: 0 }
 
@@ -409,17 +409,57 @@
         <p>
           User provided extra metadata is supported, if it’s provided in the same
 directory as the file and the metadata file is
           <tt class="docutils literal">.metadata.json</tt>
           .
         </p>
       </div>
+      <div class="section" id="server">
+        <h1>Server</h1>
+        <p>
+          Starting with version
+          <tt class="docutils literal">0.2.0dev0</tt>
+          , requires that the
+          <tt class="docutils literal">metaindexserver</tt>
+          is running to perform any operations like searching or indexing.
+        </p>
+        <p>In the default configuration the server will be started automatically as soon
+as metaindex needs to connect to the server, but none is running.</p>
+        <p>However, you may also launch the server process ahead in time like this:</p>
+        <pre class="literal-block">metaindexserver --detach</pre>
+        <p>
+          It supports a few parameters like
+          <tt class="docutils literal">
+            <span class="pre">-c</span>
+          </tt>
+          to change the configuration file
+and
+          <tt class="docutils literal">
+            <span class="pre">-l</span>
+          </tt>
+          to change the log level.
+        </p>
+        <p>
+          To stop a running server, run
+          <tt class="docutils literal">
+            metaindexserver
+            <span class="pre">--stop</span>
+          </tt>
+          or send it a
+          <tt class="docutils literal">TERM</tt>
+          signal.
+        </p>
+      </div>
       <div class="section" id="options">
         <h1>Options</h1>
-        <p>General parameters are:</p>
+        <p>
+          General parameters for
+          <tt class="docutils literal">metaindex</tt>
+          are:
+        </p>
         <blockquote>
           <dl class="docutils">
             <dt>
               <tt class="docutils literal">
                 <span class="pre">-c</span>
                 configuration file
               </tt>
@@ -455,14 +495,20 @@
             </dd>
             <dt>
               <tt class="docutils literal">
                 <span class="pre">--list</span>
               </tt>
             </dt>
             <dd>List all available indexers and exit.</dd>
+            <dt>
+              <tt class="docutils literal">
+                <span class="pre">--compact</span>
+              </tt>
+            </dt>
+            <dd>Compact the backend database.</dd>
           </dl>
         </blockquote>
         <p>
           metaindex operates in one of the modes
           <tt class="docutils literal">index</tt>
           or
           <tt class="docutils literal">find</tt>
@@ -557,15 +603,15 @@
             </dl>
           </blockquote>
         </div>
         <div class="section" id="index">
           <h2>Index</h2>
           <p>This is the operation to index files and store that information in the
 cache:</p>
-          <pre class="literal-block">metaindex index [-C] [-r] [-p processes] [-m [paths]] [-i [paths]]</pre>
+          <pre class="literal-block">metaindex index [-v[v[v[v]]]] [-C] [-r] paths</pre>
           <p>The options to this command are</p>
           <blockquote>
             <dl class="docutils">
               <dt>
                 <tt class="docutils literal">
                   <span class="pre">-C</span>
                 </tt>
@@ -594,57 +640,113 @@
                 <tt class="docutils literal">-</tt>
                 , the list of files will be read from stdin, one
 file per line.
 By default this option is disabled.
               </dd>
               <dt>
                 <tt class="docutils literal">
-                  <span class="pre">-i</span>
-                  [paths]
+                  <span class="pre">-r</span>
                 </tt>
               </dt>
               <dd>
-                Run the indexer on these paths. If no paths are provided, all paths in
-the cache are revisited and checked for changes.
-If
-                <tt class="docutils literal">paths</tt>
-                is
-                <tt class="docutils literal">-</tt>
-                , the list of files will be read from stdin, one
-file per line.
+                Run the indexer recursively. That means to visit all files in all
+subdirectories of the paths in the
+                <tt class="docutils literal">
+                  <span class="pre">-i</span>
+                </tt>
+                parameter.
               </dd>
               <dt>
                 <tt class="docutils literal">
-                  <span class="pre">-p</span>
-                  processes
+                  <span class="pre">-v</span>
                 </tt>
               </dt>
-              <dd>By default metaindex will run as many indexer processes in parallel as
-CPUs are available on the computer. This parameter allows you to define
-how many indexers may be run at the same time.</dd>
+              <dd>
+                <p class="first">
+                  Make the output more verbose. This option can be provided up to four
+times (
+                  <tt class="docutils literal">
+                    <span class="pre">-vvvv</span>
+                  </tt>
+                  ). The steps are:
+                </p>
+                <blockquote class="last">
+                  <ul class="simple">
+                    <li>
+                      No
+                      <tt class="docutils literal">
+                        <span class="pre">-v</span>
+                      </tt>
+                      : no output other than errors or information from certain indexers
+                    </li>
+                    <li>
+                      <tt class="docutils literal">
+                        <span class="pre">-v</span>
+                      </tt>
+                      : print a
+                      <tt class="docutils literal">.</tt>
+                      per file indexed
+                    </li>
+                    <li>
+                      <tt class="docutils literal">
+                        <span class="pre">-vv</span>
+                      </tt>
+                      : same as
+                      <tt class="docutils literal">
+                        <span class="pre">-v</span>
+                      </tt>
+                      and print how many files were indexed in the end
+                    </li>
+                    <li>
+                      <tt class="docutils literal">
+                        <span class="pre">-vvv</span>
+                      </tt>
+                      : same as
+                      <tt class="docutils literal">
+                        <span class="pre">-vv</span>
+                      </tt>
+                      but also show how long it took
+                    </li>
+                    <li>
+                      <tt class="docutils literal">
+                        <span class="pre">-vvvv</span>
+                      </tt>
+                      : same as
+                      <tt class="docutils literal">
+                        <span class="pre">-vvv</span>
+                      </tt>
+                      but print the path of each indexed file instead of just a
+                      <tt class="docutils literal">.</tt>
+                    </li>
+                  </ul>
+                </blockquote>
+              </dd>
               <dt>
-                <tt class="docutils literal">
-                  <span class="pre">-r</span>
-                </tt>
+                <tt class="docutils literal">paths</tt>
               </dt>
               <dd>
-                Run the indexer recursively. That means to visit all files in all
-subdirectories of the paths in the
-                <tt class="docutils literal">
-                  <span class="pre">-i</span>
-                </tt>
-                parameter.
+                Run the indexer on these paths.
+If
+                <tt class="docutils literal">paths</tt>
+                is
+                <tt class="docutils literal">-</tt>
+                , the list of files will be read from stdin, one
+file per line.
               </dd>
             </dl>
           </blockquote>
         </div>
         <div class="section" id="filesystem-fs">
           <h2>Filesystem (fs)</h2>
-          <p>On Linux you can try the experimental feature of mounting a FuseFS that
-will give you a structured access to your files through their metadata:</p>
+          <p>
+            On Linux you can try the
+            <strong>experimental</strong>
+            feature of mounting a FuseFS that
+will give you a structured access to your files through their metadata:
+          </p>
           <pre class="literal-block">metaindex fs [command] [mount point]</pre>
           <p>
             The only supported command so far is
             <tt class="docutils literal">mount</tt>
             .
           </p>
           <p>It is very experimental and not very useful, but at the same time will not
@@ -832,48 +934,14 @@
                     Defaults to
                     <tt class="docutils literal">yes</tt>
                     .
                   </p>
                 </dd>
                 <dt>
                   <tt class="docutils literal">
-                    <span class="pre">ignore-tags</span>
-                  </tt>
-                </dt>
-                <dd>
-                  <p class="first">
-                    What (automatically extracted) tags to not add to the cache and thus
-prevent them being searchable. Comma-separated list of the tags.
-To add to the ignored tags, instead of redefining them, include the
-special value
-                    <tt class="docutils literal">*</tt>
-                    in the listing.
-                  </p>
-                  <p>
-                    If you want to exclude a group of tags that have the same prefix or
-suffix, you can add a
-                    <tt class="docutils literal">*</tt>
-                    to the end or start of the tag
-respectively. E.g. to exclude all tags that come from Nikon in the EXIF
-metadata group, this would do what you want:
-                    <tt class="docutils literal">exif.nikon*</tt>
-                    .
-                  </p>
-                  <p class="last">
-                    Defaults to:
-                    <tt class="docutils literal">
-                      Exif.Image.StripByteCounts, Exif.Image.StripOffsets, Exif.Photo.makernote,
-                      <span class="pre">Exif.Thumbnail.*,</span>
-                      Exif.Sony1.0x*, Exif.Nikonsi*, Exif.Nikoncb*, Exif.Nikon3.linearizationtable, Exif.Nikon3.contrastcurve, Exif.Nikon3.0x*, Exif.Nikonfi.0x*, Exif.Canon.0x*, Exif.Canon.camerainfo, Exif.Canon.afinfo3
-                    </tt>
-                    .
-                  </p>
-                </dd>
-                <dt>
-                  <tt class="docutils literal">
                     <span class="pre">ignore-indexers</span>
                   </tt>
                 </dt>
                 <dd>
                   <p class="first">A comma separated list of indexers by name that you do not want to use.
 By default this list is empty.</p>
                   <p class="last">
@@ -911,14 +979,39 @@
                   <tt class="docutils literal">mimetypes</tt>
                 </dt>
                 <dd>If you have additional mimetypes that you would like metaindex to know,
 this is the option you can use to point to additional mimetype files.
 To add multiple files, separate them by a newline. No matter what files
 you provide here, you system's mimetype file will always be used.</dd>
                 <dt>
+                  <tt class="docutils literal">
+                    <span class="pre">implicit-tags</span>
+                  </tt>
+                </dt>
+                <dd>
+                  <p class="first">
+                    Some tags should be accessible during search, even when not searching
+explicitly for that tag (e.g. searching for &quot;the two towers&quot; should
+find the book, even if you don't explicitly search for
+                    <tt class="docutils literal">
+                      <span class="pre">title:&quot;the</span>
+                      two towers&quot;
+                    </tt>
+                    ). This option selects the tags that should always be
+included in the search.
+                  </p>
+                  <p>Note that this option applies during indexing. Changing it after
+indexing will not change the behaviour of the search.</p>
+                  <p class="last">
+                    Defaults to:
+                    <tt class="docutils literal">author, title, tag, type, series, filename</tt>
+                    .
+                  </p>
+                </dd>
+                <dt>
                   <tt class="docutils literal">ocr</tt>
                 </dt>
                 <dd>
                   <p class="first">
                     Whether or not OCR (optical character recognition) should be enabled.
 For this to work you must have installed the
                     <tt class="docutils literal">ocr</tt>
@@ -989,30 +1082,38 @@
 semantically be the same. For example,
               <tt class="docutils literal">Xmp.xmp.CreatorTool</tt>
               and
               <tt class="docutils literal">pdf.Creator</tt>
               both mean &quot;The program that was used to create this file&quot;.
             </p>
             <p>
-              For convenience it is possible to define synonyms, so you only have to
-search for
+              To simplify the search it is possible to define synonyms for these metadata fields.
+For example the tag
               <tt class="docutils literal">author</tt>
-              when you mean to search for
+              could point to the fields
               <tt class="docutils literal">id3.artist</tt>
               ,
               <tt class="docutils literal">pdf.Author</tt>
-              , or
+              , and
               <tt class="docutils literal">Exif.Image.Artist</tt>
               .
             </p>
             <p>
+              Note that metaindex will only allow you to search metadata fields by their
+synonym. That means you can search for
+              <tt class="docutils literal">author:tim</tt>
+              , but not for
+              <tt class="docutils literal">pdf.Author:tim</tt>
+              .
+            </p>
+            <p>
               The section
               <tt class="docutils literal">[Synonyms]</tt>
               in the configuration file is the place to define
-these synonyms. Here are the defaults, that you don’t have to set up:
+the synonyms. Here are the defaults, that you don’t have to set up:
             </p>
             <pre class="literal-block">[Synonyms]
 author = extra.author, extra.artist, extra.creator, id3.artist, pdf.Author, rules.author, Exif.Image.Artist, comicbook.writer, xmp.dc.name
 type = extra.type, rules.type, xmp.dc.type
 date = extra.date, rules.date, comicbook.date
 title = extra.title, opf.title, id3.title, rules.title, pdf.Title, filetags.title, abs.title, comicbook.title, Xmp.dc.title
 tag = extra.tag, extra.tags, pdf.Keywords, pdf.Categories, Xmp.dc.subject, extra.subject, rules.tags, rules.tag, rules.subject, pdf.Subject, comicbook.tags, opf.subject
@@ -1830,39 +1931,34 @@
             <p>
               To index you
               <tt class="docutils literal">Documents</tt>
               and
               <tt class="docutils literal">Pictures</tt>
               folder recursively:
             </p>
-            <pre class="literal-block">metaindex index -r -i ~/Documents ~/Pictures</pre>
-          </div>
-          <div class="section" id="reindex-all-files">
-            <h3>Reindex all files</h3>
-            <p>To only update the metadata from all known files:</p>
-            <pre class="literal-block">metaindex index -i</pre>
+            <pre class="literal-block">metaindex index -r ~/Documents ~/Pictures</pre>
           </div>
           <div class="section" id="find-all-files">
             <h3>Find all files</h3>
             <p>List all files that are in cache:</p>
             <pre class="literal-block">metaindex find</pre>
           </div>
           <div class="section" id="find-file-by-mimetype">
             <h3>Find file by mimetype</h3>
             <p>
               Searching for all
               <tt class="docutils literal">image/*</tt>
               mimetypes can be accomplished by this:
             </p>
-            <pre class="literal-block">metaindex find mimetype:^image/</pre>
+            <pre class="literal-block">metaindex find mimetype:image/</pre>
           </div>
           <div class="section" id="listing-metadata">
             <h3>Listing metadata</h3>
-            <p>To list all metadata tags and values of all odt files:</p>
-            <pre class="literal-block">metaindex find -t -- &quot;filename:odt$&quot;</pre>
+            <p>To list all metadata tags and values of all image files:</p>
+            <pre class="literal-block">metaindex find -t -- &quot;ext:odt$&quot;</pre>
             <p>
               List the resolutions of all files that have the
               <tt class="docutils literal">resolution</tt>
               metadata tag:
             </p>
             <pre class="literal-block">metaindex find -t resolution -- &quot;resolution?&quot;</pre>
           </div>
```

### Comparing `metaindex-1.4.0/metaindex/find.py` & `metaindex-2.0.0/metaindex/find.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import os
 import sys
 
 from metaindex import logger
 from metaindex.cache import Cache
 
 
-def find(config, args):
-    cache = Cache(config)
+def find(cache, args):
     query = args.query or []
     symlink_folder = None
 
     if args.link is not None:
         symlink_folder = pathlib.Path(args.link).expanduser().resolve()
 
         if symlink_folder.exists() and not symlink_folder.is_dir():
@@ -70,15 +69,15 @@
                 os.symlink(target, fn)
 
         show_keys = set(result.keys())
         if args.tags is None:
             continue
 
         if len(args.tags) > 0:
-            show_keys = config.expand_synonyms(args.tags)
+            show_keys = cache.config.expand_synonyms(args.tags)
 
         for key in sorted(show_keys):
             values = result[key]
             if len(values) == 0:
                 continue
 
             if len(values) == 1:
```

### Comparing `metaindex-1.4.0/metaindex/fuse.py` & `metaindex-2.0.0/metaindex/fuse.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/humanizer.py` & `metaindex-2.0.0/metaindex/humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexer.py` & `metaindex-2.0.0/metaindex/indexer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """File indexer base class and API"""
 import datetime
 import pathlib
 import mimetypes
-import time
 import sys
-import os
 from collections import namedtuple
 from multiprocessing import Queue, Process, Event
 from enum import IntEnum
 try:
     from signal import SIGINT
 except ImportError:
     SIGINT = None
@@ -16,14 +14,15 @@
     from signal import CTRL_C_EVENT
 except ImportError:
     CTRL_C_EVENT = None
 
 from metaindex import shared
 from metaindex import logger
 from metaindex import configuration
+from metaindex.cacheentry import CacheEntry
 from metaindex.ocr import Dummy
 
 
 _registered_indexers = {}
 _indexer_by_suffix = {}
 _indexer_by_mimetype = {}
 _generic_indexers = []
@@ -280,61 +279,58 @@
         if name not in self.cached:
             self.cached[name] = self.registered_indexers[name](self)
         return self.cached[name]
 
     def index(self, files):
         """Index the given files
 
+        Yields each indexed file
+
         :param files: The files to index
         :type files: ``list[pathlib.Path]``
-        :return: a list of ``IndexerResult``
         """
-        results = []
-
         for filename in files:
             filename = pathlib.Path(filename)
 
             if not filename.is_file():
                 continue
 
             try:
                 result = self.get_metadata(filename)
             except KeyboardInterrupt:
-                return results
+                break
             except Exception as exc:
                 logger.error("Indexing %s failed: %s", filename, exc)
-                result = IndexerResult(filename, False, shared.CacheEntry(filename))
+                result = IndexerResult(filename, False, CacheEntry(filename))
 
-            results.append(result)
-
-        return results
+            yield result
 
     def get_metadata(self, path):
         """Extract metadata from the file at `filename`"""
         logger.debug(f"Going for {path}")
 
         stat = path.stat()
         suffix = path.suffix[1:]
         mimetype, _ = mimetypes.guess_type(path, strict=False)
-        info = shared.CacheEntry(path)
+        info = CacheEntry(path)
         info.add('size', stat.st_size)
         info.last_modified = datetime.datetime.fromtimestamp(stat.st_mtime)
 
         if mimetype is not None:
-            info.add('mimetype', mimetype)
+            info.mimetype = mimetype
 
         delete_keys = set()
         applied_indexers = 0
         indexers = self.generic_indexers[:] \
                  + self.indexer_by_suffix.get(path.suffix.lower(), [])
         if mimetype is not None:
             for mtype in [mimetype, mimetype.split('/', 1)[0]]:
                 indexers += self.indexer_by_mimetype.get(mtype, [])
 
-        base_info = self.base_info.get(path, shared.CacheEntry(path))
+        base_info = self.base_info.get(path, CacheEntry(path))
         for handler in sorted(set(self.get(indexer) for indexer in indexers)):
             logger.debug(f"... running {type(handler).__name__}")
 
             initial_fields = len(info)
             handler.run(path, info, base_info)
 
             # Some fields have been added since?
@@ -343,28 +339,14 @@
 
                 # if an 'extra.' key's value is set to None explicitely,
                 # it WILL be removed after the last indexer ran
                 delete_keys |= {key_.split('.', 1)[1]
                                 for key_, value in info
                                 if value is None and key_.startswith(shared.EXTRA)}
 
-        # remove ignored tags
-        for keyname in self.config.ignore_tags:
-            keyname = keyname.lower()
-            if keyname.startswith('*'):
-                for other, _ in info:
-                    if other.endswith(keyname[1:]):
-                        delete_keys.add(other)
-            elif keyname.endswith('*'):
-                for other, _ in info:
-                    if other.startswith(keyname[:-1]):
-                        delete_keys.add(other)
-            else:
-                delete_keys.add(keyname)
-
         for key_ in delete_keys | {shared.IS_RECURSIVE}:
             if key_ in info:
                 del info[key_]
 
         success = applied_indexers > 0
         return IndexerResult(path, success, info)
 
@@ -427,82 +409,21 @@
     :rtype: ``list[IndexerResult]``
     """
     from metaindex import indexers as _
 
     if baseconfig is None:
         baseconfig = configuration.load()
 
-    if processes is None:
-        processes = len(os.sched_getaffinity(0))
-    if processes > len(files):
-        processes = len(files)
-    processes = 1
-
-    results = []
-    if processes > 1:
-        logger.info("Using %s processes", processes)
-        runners = []
-        for _ in range(processes):
-            runners.append(IndexerRunnerProcess(baseconfig,
-                                                fulltext=fulltext,
-                                                last_modified=last_modified,
-                                                base_info=last_cached))
-
-        for pos, file_ in enumerate(files):
-            runner = pos % len(runners)
-            runners[runner].files.append(file_)
-
-        then = datetime.datetime.now()
-        for runner in runners:
-            runner.start()
-
-        try:
-            for runner in runners:
-                runner.join()
-        except KeyboardInterrupt:
-            logger.fatal("Cancelling all running processes")
-            for runner in runners:
-                runner.cancel.set()
-            time.sleep(0.5)
-            signal = SIGINT
-            if sys.platform.startswith('win'):
-                signal = CTRL_C_EVENT
-            for runner in runners:
-                if runner.is_alive():
-                    os.kill(runner.pid, signal)
-
-        for runner in runners:
-            try:
-                if runner.is_alive():
-                    runner.join()
-            except KeyboardInterrupt:
-                pass
-
-        for runner in runners:
-            while not runner.results.empty():
-                item = runner.results.get_nowait()
-                if item is not None:
-                    results += [item]
-
-    else:
-        runner = IndexerRunner(baseconfig,
-                               fulltext=fulltext,
-                               last_modified=last_modified,
-                               base_info=last_cached)
-
-        then = datetime.datetime.now()
-        results = runner.index(files)
-
-    logger.info("Processed %s files in %s",
-                len([v for v in results if v[1]]),
-                datetime.datetime.now() - then)
-    logger.debug("Successfully indexed: %s",
-                 ', '.join([str(v[0]) for v in results if v[1]]))
+    runner = IndexerRunner(baseconfig,
+                           fulltext=fulltext,
+                           last_modified=last_modified,
+                           base_info=last_cached)
 
-    return results
+    for result in runner.index(files):
+        yield result
 
 
 if __name__ == '__main__':
     import sys
 
     logger.setup('DEBUG')
     config = configuration.load()
```

### Comparing `metaindex-1.4.0/metaindex/indexers/audio.py` & `metaindex-2.0.0/metaindex/indexers/audio.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/collections.py` & `metaindex-2.0.0/metaindex/indexers/collections.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Collection sidecar file indexers"""
 from metaindex import logger
 from metaindex import json
 from metaindex import opf
 from metaindex import configuration
 from metaindex import shared
+from metaindex.cacheentry import CacheEntry
 from metaindex.indexer import IndexerBase, Order
 
 try:
     from metaindex import yaml
 except ImportError:
     yaml = None
 
@@ -57,22 +58,22 @@
         """Fill the cache with the sidecar files' contents"""
         assert self.PREFIX is not None
         for sidecar in self.find_collection_sidecars(path, store.SUFFIX):
             if sidecar in self.cached_sidecar_files:
                 continue
             self.cached_sidecar_files.add(sidecar)
 
-            self.collection_cache[sidecar.parent] = shared.CacheEntry(sidecar.parent)
+            self.collection_cache[sidecar.parent] = CacheEntry(sidecar.parent)
             for filepath, extra in store.get_for_collection(sidecar).items():
                 if filepath not in self.collection_cache:
-                    self.collection_cache[filepath] = shared.CacheEntry(filepath)
+                    self.collection_cache[filepath] = CacheEntry(filepath)
                 self.collection_cache[filepath].update(extra)
 
     def get_collection_metadata(self, path, suffix):
-        meta = shared.CacheEntry(path)
+        meta = CacheEntry(path)
 
         for sidecar in reversed(self.find_collection_sidecars(path, suffix)):
             if sidecar.parent not in self.collection_cache:
                 logger.info("A sidecar file has been added while the indexer was running. "
                             "That file is ignored until the next rerun.")
                 continue
             extra = self.collection_cache[sidecar.parent]
```

### Comparing `metaindex-1.4.0/metaindex/indexers/comicbook.py` & `metaindex-2.0.0/metaindex/indexers/comicbook.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/epub.py` & `metaindex-2.0.0/metaindex/indexers/epub.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/filetags.py` & `metaindex-2.0.0/metaindex/indexers/filetags.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/gpx.py` & `metaindex-2.0.0/metaindex/indexers/gpx.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/html.py` & `metaindex-2.0.0/metaindex/indexers/html.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/images.py` & `metaindex-2.0.0/metaindex/indexers/images.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/ooxml.py` & `metaindex-2.0.0/metaindex/indexers/ooxml.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/opendocument.py` & `metaindex-2.0.0/metaindex/indexers/opendocument.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/pdf.py` & `metaindex-2.0.0/metaindex/indexers/pdf.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/indexers/ruleindexer.py` & `metaindex-2.0.0/metaindex/indexers/ruleindexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/json.py` & `metaindex-2.0.0/metaindex/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import json
 import pathlib
 import datetime
 
 from metaindex import logger
 from metaindex import shared
+from metaindex.cacheentry import CacheEntry
 
 
 SUFFIX = '.json'
 
 
 def get(filename):
     if isinstance(filename, (str, pathlib.Path)):
         logger.debug(f"Reading JSON metadata from {filename}")
         with open(filename, "rt", encoding="utf-8") as fh:
             return get(fh)
 
-    entry = shared.CacheEntry(None)
+    entry = CacheEntry(None)
     if hasattr(filename, 'name'):
         entry.path = pathlib.Path(filename.name)
 
     success, data = _read_json_file(filename)
 
     if not success:
         return entry
@@ -64,15 +65,15 @@
 
         if targetfile in ['*', '**']:
             fulltargetname = basepath
         else:
             fulltargetname = basepath / targetfile
 
         if fulltargetname not in result:
-            result[fulltargetname] = shared.CacheEntry(pathlib.Path(fulltargetname))
+            result[fulltargetname] = CacheEntry(pathlib.Path(fulltargetname))
 
         for key in data[targetfile].keys():
             values = data[targetfile][key]
 
             if not isinstance(values, list):
                 values = [values]
 
@@ -86,18 +87,18 @@
 
 def store(metadata, filename):
     """Store this metadata information in that metadata file"""
     if isinstance(filename, (str, pathlib.Path)):
         with open(filename, 'wt', encoding='utf-8') as fh:
             return store(metadata, fh)
 
-    if isinstance(metadata, shared.CacheEntry):
+    if isinstance(metadata, CacheEntry):
         data = _cacheentry_as_dict(metadata)
     elif isinstance(metadata, list) and \
-         all(isinstance(e, shared.CacheEntry) for e in metadata):
+         all(isinstance(e, CacheEntry) for e in metadata):
         data = {}
         for item in sorted(metadata):
             if item.path.is_dir():
                 key = '*'
                 if item[shared.IS_RECURSIVE] == [True]:
                     key = '**'
             else:
```

### Comparing `metaindex-1.4.0/metaindex/logger.py` & `metaindex-2.0.0/metaindex/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def setup(level=pythonlogging.WARNING, filename=None):
     global _logger
     global _handler
     global _formatter
 
     _formatter = None
-    if filename is None:
+    if filename is None or filename == '-':
         _handler = pythonlogging.StreamHandler()
         _formatter = pythonlogging.Formatter("[%(levelname)s] %(message)s")
     elif isinstance(filename, pythonlogging.Handler):
         _handler = filename
     else:
         _handler = RotatingFileHandler(filename,
                                        encoding='utf-8',
@@ -30,14 +30,18 @@
 
     _logger = pythonlogging.getLogger('metaindex')
     _logger.propagate = False
     _logger.setLevel(level)
     _logger.addHandler(_handler)
 
 
+def is_set_up():
+    return _logger is not None
+
+
 def debug(*args, **kwargs):
     if _logger:
         return _logger.debug(*args, **kwargs)
 
 
 def info(*args, **kwargs):
     if _logger:
```

### Comparing `metaindex-1.4.0/metaindex/main.py` & `metaindex-2.0.0/metaindex/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import argparse
 import sys
+import time
+import datetime
+import subprocess
+from pathlib import Path
 
 from metaindex import configuration
 from metaindex import stores
 from metaindex import indexer
 from metaindex import indexers
 from metaindex import logger
+from metaindex import version
 from metaindex.cache import Cache
 from metaindex.find import find
 
 try:
     from metaindex.fuse import metaindex_fs
 except ImportError:
     metaindex_fs = None
@@ -35,14 +40,24 @@
                         help="Write the log to this file instead of stderr.")
 
     parser.add_argument('--list',
                         action="store_true",
                         default=False,
                         help="List all available file indexers")
 
+    parser.add_argument('--compact',
+                        action="store_true",
+                        default=False,
+                        help="Compact the database")
+
+    parser.add_argument('-V', '--version',
+                        action="version",
+                        version='%(prog)s ' + version.__version__,
+                        help="Show the version of metaindex and exit")
+
     subparsers = parser.add_subparsers(dest='command')
 
     indexparser = subparsers.add_parser('index')
 
     indexparser.add_argument('-r', '--recursive',
                              default=False,
                              action='store_true',
@@ -57,15 +72,22 @@
     indexparser.add_argument('-m', '--flush-missing',
                              default=False,
                              type=str,
                              nargs='*',
                              help="Remove files from cache that can no longer be "
                                   "found in the given paths.")
 
-    indexparser.add_argument('-i', '--index',
+    indexparser.add_argument('-v', '--verbose',
+                             default=0,
+                             action='count',
+                             help="Increase verbosity level. Can be passed "
+                                  "multiple times. By default the indexer will "
+                                  "be very quiet.")
+
+    indexparser.add_argument('index',
                              nargs='*',
                              type=str,
                              default=False,
                              help="Path(s) to index. If you provide none, all "
                                   "cached items will be refreshed. If you pass "
                                   "- the files will be read from stdin, one "
                                   "file per line.")
@@ -122,33 +144,62 @@
                               type=str,
                               help="Where to mount the metaindex filesystem.")
 
     result = parser.parse_args()
 
     if result.list:
         pass
-    elif result.command is None:
+    elif result.command is None and not result.compact:
         parser.print_help()
 
     return result
 
 
+indexed_files_count = 0
+
+
+def index_status(config, entry):
+    global indexed_files_count
+    indexed_files_count += 1
+    if 0 < config.verbose <= 3:
+        print(".", end="", flush=True)
+    if config.verbose >= 4:
+        print(entry.path)
+
+
 def run():
     args = parse_args()
     logger.setup(level=args.log_level.upper(), filename=args.log_file)
 
     config = configuration.load(args.config)
 
     if args.list:
         for name in sorted(indexer._registered_indexers.keys()):
             print(name)
         return 0
 
+    cache = Cache(config)
+    if config.bool(configuration.SECTION_SERVER, configuration.CONFIG_AUTOSTART):
+        configfile = configuration.CONFIGFILE
+        if args.config is not None:
+            configfile = Path(args.config).expanduser()
+        attempt = 0
+        while not cache.connection_ok() and attempt < 1:
+            attempt += 1
+            subprocess.Popen(["metaindexserver", "-c", str(configfile), "-d"])
+            time.sleep(1)
+
+    if not cache.connection_ok():
+        logger.error("Server is not running")
+        return -1
+
+    if args.compact:
+        cache.compact()
+
     if args.command == "index":
-        cache = Cache(config)
         if args.clear:
             cache.clear()
 
         cleanpaths = args.flush_missing
         if args.flush_missing == ['-']:
             cleanpaths = [file_ for file_ in sys.stdin.read().split("\n")
                           if len(file_) > 0]
@@ -167,18 +218,34 @@
         elif index == []:
             index = None
 
         if args.force:
             cache.expire_metadata(index)
 
         if index is not False:
-            cache.refresh(index, args.recursive, args.processes)
+            global indexed_files_count
+            indexed_files_count = 0
+
+            then = datetime.datetime.now()
+
+            cache.refresh(index,
+                          args.recursive,
+                          args.processes,
+                          callback=lambda e: index_status(args, e))
+
+            if args.verbose > 0:
+                feedback = ""
+                if args.verbose >= 2:
+                    feedback = f"\nIndexed {indexed_files_count} files"
+                if args.verbose >= 3:
+                    feedback += f" in {datetime.datetime.now() - then}"
+                print(feedback)
 
         return 0
 
     if args.command == "find":
-        return find(config, args)
+        return find(cache, args)
 
     if args.command == 'fs' and metaindex_fs is not None:
         return metaindex_fs(config, args)
 
     return -1
```

### Comparing `metaindex-1.4.0/metaindex/ocr.py` & `metaindex-2.0.0/metaindex/ocr.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/opf.py` & `metaindex-2.0.0/metaindex/opf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pathlib
 
 from metaindex import shared
+from metaindex.cacheentry import CacheEntry
 from metaindex.xmlproxy import etree, check_defusedxml
 
 
 SUFFIX = '.opf'
 
 
 def get(metadatafile):
@@ -29,15 +30,15 @@
     data.add(shared.IS_RECURSIVE, True)
 
     return {basepath: data}
 
 
 def parse_opf(content, prefix='opf.'):
     check_defusedxml()
-    result = shared.CacheEntry(None)
+    result = CacheEntry(None)
 
     try:
         root = etree.fromstring(content)
     except:
         return result
 
     for node in root.findall('.//{http://purl.org/dc/elements/1.1/}*'):
```

### Comparing `metaindex-1.4.0/metaindex/shared.py` & `metaindex-2.0.0/metaindex/cacheentry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,13 @@
-"""Functions, names, and identifiers shared in the code"""
-import codecs
+"""File cache entry and metadata grouping classes"""
 import datetime
 from pathlib import Path
 
-from .humanizer import humanize
-
-
-EXTRA = 'extra.'
-IS_RECURSIVE = 'extra_metadata_is_recursive'
-LAST_MODIFIED = 'extra_metadata_last_modified'
-
-DUBLINCORE_TAGS = {
-    'contributor',
-    'coverage',
-    'creator',
-    'date',
-    'description',
-    'format',
-    'identifier',
-    'language',
-    'publisher',
-    'relation',
-    'rights',
-    'source',
-    'subject',
-    'title',
-    'type',
-}
+from metaindex.shared import get_last_modified, strfdt, strpdt, jsonify
+from metaindex.humanizer import humanize
 
 
 class MetadataValue:
     """A metadata value
 
     This value consists of the ``raw_value``, as it was found by the
     indexer in the source or sidecar file, and the ``humanized_value`` as
@@ -55,14 +32,18 @@
         """The raw, not humanized value"""
         self.humanized_value = humanized
 
     def humanized(self):
         """The humanized version of the value"""
         return self.humanized_value or str(self.raw_value)
 
+    def copy(self):
+        """Return a deep copy of this value"""
+        return MetadataValue(self.raw_value, self.humanized())
+
     def __eq__(self, other):
         if isinstance(other, MetadataValue):
             return self.raw_value == other.raw_value and \
                    self.humanized_value == other.humanized_value
         if isinstance(other, str):
             return self.humanized() == other
         if isinstance(other, type(self.raw_value)):
@@ -84,27 +65,47 @@
     def __hash__(self):
         return hash(self.humanized())
 
 
 class CacheEntry:
     """A cached metadata entry for an item in the filesystem"""
 
-    AUTO_KEYS = {'filename', 'last_modified'}
+    AUTO_KEYS = {'filename', 'last_modified', 'rel_path', 'storage_label'}
     FILENAME = 'filename'
     LAST_MODIFIED = 'last_modified'
+    STORAGE_LABEL = 'storage_label'
+    REL_PATH = 'rel_path'
 
-    def __init__(self, path, metadata=None, last_modified=None):
+    def __init__(self,
+                 path,
+                 metadata=None,
+                 last_modified=None,
+                 rel_path=None,
+                 storage_label=None):
         self.path = Path(path) if isinstance(path, str) else path
         """The path to the file object in the filesystem.
         Does not need to exist."""
 
+        self.last_modified = last_modified or datetime.datetime.min
+        """The time stamp of when the file was modified most recently"""
+
+        self.rel_path = rel_path
+        """Path relative to mount point of this file object.
+        Optional."""
+
+        self.storage_label = storage_label
+        """Human-readable (and provided) label what storage device this file is residing on"""
+
         self.metadata = metadata or {}
         """The dictionary of lower-case keys,
         mapping to a list of ``MetadataValue``."""
 
+        self.mimetype = None
+        """The mimetype of the file object"""
+
         if isinstance(metadata, (list, set)):
             self.metadata = {}
             for key, value in metadata:
                 if key not in self.metadata:
                     self.metadata[key] = []
                 self.add(key, value)
         elif isinstance(metadata, dict):
@@ -113,16 +114,24 @@
                 if not isinstance(values, (list, tuple, set)):
                     values = [values]
                 for value in values:
                     self.add(key, value)
         elif metadata is not None:
             raise TypeError()
 
-        self.last_modified = last_modified or datetime.datetime.min
-        """The time stamp of when the file was modified most recently"""
+    @classmethod
+    def from_dict(cls, data):
+        """Recreate a CacheEntry from data, as generated by 'as_dict'"""
+        that = cls(data['path'],
+                   data.get('metadata', {}),
+                   strpdt(data.get('last_modified', '000010101T000000')),
+                   data.get('rpath', None),
+                   data.get('slbl', None))
+        that.mimetype = data.get('mime', None)
+        return that
 
     def __lt__(self, other):
         return str(self.path) < str(other.path)
 
     def __len__(self):
         """The number of metadata key/value pairs"""
         return sum(len(values) for values in self.metadata.values())
@@ -165,14 +174,36 @@
         """Get the list of ``MetadataValue`` of ``key``
 
         :param key: The key to look for
         :return: A list of ``MetadataValue``s, may be empty.
         """
         return self.get(key)
 
+    def as_dict(self):
+        """Return this cache entry as a plain old dictionary"""
+        result = {'path': str(self.path),
+                  'last_modified': strfdt(self.last_modified),
+                  'slbl': self.storage_label,
+                  'rpath': jsonify(self.rel_path),
+                  'mime': self.mimetype,
+                  'metadata': {key: [jsonify(v.raw_value) for v in values]
+                               for key, values in self.metadata.items()}}
+        return result
+
+    def copy(self):
+        """Create a deep copy of this cache entry"""
+        that = CacheEntry(str(self.path))
+        that.metadata = {key: [v.copy() for v in values]
+                         for key, values in self.metadata.items()}
+        that.last_modified = self.last_modified
+        that.mimetype = self.mimetype
+        that.storage_label = self.storage_label
+        that.rel_path = self.rel_path
+        return that
+
     def get(self, key):
         """Get the list of ``MetadataValue`` of ``key``
 
         :param key: The key to look for
         :return: A list of ``MetadataValue``, may be empty.
         """
         if key == type(self).FILENAME and self.path is not None:
@@ -300,79 +331,7 @@
                          for v in self.metadata[key]
                          if v == value]
             for item in to_delete:
                 self.metadata[key].remove(item)
 
         if len(self.metadata[key]) == 0 or value is None:
             del self.metadata[key]
-
-
-def get_last_modified(file_):
-    """Return the last_modified datetime of the given file.
-
-    This will drop the microsecond part of the timestamp! The reasoning is that
-    last_modified will be taken during database cache updates. If a change
-    happens at the same second to a file, just after the indexer passed it,
-    there's probably a good chance the file gets modified again in the near
-    future at which point the indexer will pick up the change.
-    Other than that, the cache can forcefully be cleared, too.
-    """
-    return datetime.datetime.fromtimestamp(file_.stat().st_mtime).replace(microsecond=0)
-
-
-def find_files(paths, recursive=True, ignore_dirs=None):
-    """Find all files in these paths"""
-    if not isinstance(paths, list):
-        paths = [paths]
-    if ignore_dirs is None:
-        ignore_dirs = []
-
-    pathqueue = list(paths)
-    filenames = []
-
-    while len(pathqueue) > 0:
-        path = pathqueue.pop(0)
-
-        if not isinstance(path, Path):
-            path = Path(path)
-
-        if not path.exists():
-            continue
-
-        for item in path.iterdir():
-            if item.is_dir() and recursive and item.parts[-1] not in ignore_dirs:
-                pathqueue.append(item)
-                continue
-
-            if item.is_file():
-                filenames.append(item)
-
-    return filenames
-
-
-def to_utf8(raw):
-    if isinstance(raw, str):
-        return raw
-    encoding = None
-    skip = 1
-
-    if raw.startswith(codecs.BOM_UTF8):
-        encoding = 'utf-8'
-    elif raw.startswith(codecs.BOM_UTF16_BE):
-        encoding = 'utf-16-be'
-    elif raw.startswith(codecs.BOM_UTF16_LE):
-        encoding = 'utf-16-le'
-    elif raw.startswith(codecs.BOM_UTF32_BE):
-        encoding = 'utf-32-be'
-    elif raw.startswith(codecs.BOM_UTF32_LE):
-        encoding = 'utf-32-le'
-    else:
-        # just best efford
-        encoding = 'utf-8'
-        skip = 0
-
-    try:
-        text = str(raw, encoding=encoding).strip()
-        return text[skip:]  # drop the BOM, if applicable
-    except UnicodeError:
-        pass
-    return None
```

### Comparing `metaindex-1.4.0/metaindex/stores.py` & `metaindex-2.0.0/metaindex/stores.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """General access to all methods of metadata storage"""
 import pathlib
 
 from metaindex import json
 from metaindex import opf
-from metaindex.shared import CacheEntry
+from metaindex.cacheentry import CacheEntry
 
 try:
     from metaindex import yaml
 except ImportError:
     yaml = None
```

### Comparing `metaindex-1.4.0/metaindex/xmlproxy.py` & `metaindex-2.0.0/metaindex/xmlproxy.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/metaindex/yaml.py` & `metaindex-2.0.0/metaindex/yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import pathlib
 
 import yaml
 
 from metaindex import shared
 from metaindex import logger
+from metaindex.cacheentry import CacheEntry
 
 
 SUFFIX = '.yaml'
 
 
 def get(filename):
     if isinstance(filename, (pathlib.Path, str)):
         logger.debug(f"Reading YAML metadata from {filename}")
         with open(filename, "rt", encoding="utf-8") as fh:
             return get(fh)
 
-    result = shared.CacheEntry(None)
+    result = CacheEntry(None)
     if hasattr(filename, 'name'):
         result.path = pathlib.Path(filename.name)
 
     success, data = _read_yaml_file(filename)
 
     if not success:
         return result
@@ -65,15 +66,15 @@
 
         if targetfile in ['*', '**']:
             fulltargetname = basepath
         else:
             fulltargetname = basepath / targetfile
 
         if fulltargetname not in result:
-            result[fulltargetname] = shared.CacheEntry(pathlib.Path(fulltargetname))
+            result[fulltargetname] = CacheEntry(pathlib.Path(fulltargetname))
 
         for key in data[targetfile].keys():
             values = data[targetfile][key]
 
             if not isinstance(values, list):
                 values = [values]
 
@@ -87,18 +88,18 @@
 
 def store(metadata, filename):
     """Store this metadata information in that metadata file"""
     if isinstance(filename, (str, pathlib.Path)):
         with open(filename, 'wt', encoding='utf-8') as fh:
             return store(metadata, fh)
 
-    if isinstance(metadata, shared.CacheEntry):
+    if isinstance(metadata, CacheEntry):
         data = _cacheentry_as_dict(metadata)
     elif isinstance(metadata, list) and \
-         all(isinstance(e, shared.CacheEntry) for e in metadata):
+         all(isinstance(e, CacheEntry) for e in metadata):
         data = {}
         for item in sorted(metadata):
             if item.path.is_dir():
                 key = '*'
                 if item[shared.IS_RECURSIVE] == [True]:
                     key = '**'
             else:
```

### Comparing `metaindex-1.4.0/metaindex.egg-info/PKG-INFO` & `metaindex-2.0.0/metaindex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 1.4.0
+Version: 2.0.0
 Summary: Utilities to tag files
-Home-page: https://github.com/vonshednob/metaindex
+Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
@@ -56,15 +54,15 @@
 
 To install metaindex either install it directly through pypi:
 
     pip install metaindex
 
 Or clone the repository and install that then through pip:
 
-    git clone https://github.com/vonshednob/metaindex
+    git clone https://codeberg.org/vonshednob/metaindex
     cd metaindex
     pip install .
 
 Most modules are optional. If you, for example, want to use metaindex for audio
 files and PDFs, you will have to install it like this:
 
     pip install metaindex[pdf,audio]
@@ -91,24 +89,36 @@
 
 There is also an experimental FuseFS filesystem. To be able to use it, you
 will have to specify ``fuse`` as an additional module:
 
     pip install .[all,fuse]
 
 
+### Server dependencies
+
+If you just want to connect to another instance of the metaindex server,
+you are ready to go.  
+More likely though you will have to install [Xapian](https://xapian.org/)
+and its Python3 bindings. Please follow the usual way of your OS to install
+both.
+
+For example, on Archlinux you'd `pacman -S xapian python-xapian`. On
+debian-likes it would be `apt install python3-xapian`.
+
+
 ## Usage
 
 Before you can use metaindex to search for files, you have to initialize the
 cache by telling it where your files to index are, for example:
 
     metaindex index --recursive --index ~/Pictures
 
 Afterwards you can start searching for files by metadata, like this:
 
-    metaindex find 
+    metaindex find
 
 
 ## Searching
 
 Search queries for use with `metaindex find` allow you to search
 
  - for files that have a metadata tag: `metaindex find resolution?`
@@ -146,9 +156,7 @@
     cache.wait_for_reload()
 
     searchquery = 'mimetype:image title?'
 
     for entry in cache.find(searchquery):
         print(entry.path)
 
-
-
```

### Comparing `metaindex-1.4.0/metaindex.egg-info/SOURCES.txt` & `metaindex-2.0.0/metaindex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -93,27 +93,29 @@
 doc/source/searchsyntax.rst
 doc/source/synopsis.rst
 doc/source/usage.rst
 examples/indexing.py
 man/metaindex.1
 metaindex/__init__.py
 metaindex/cache.py
+metaindex/cacheentry.py
+metaindex/client.py
 metaindex/configuration.py
 metaindex/find.py
 metaindex/fuse.py
 metaindex/humanizer.py
 metaindex/indexer.py
 metaindex/json.py
 metaindex/logger.py
 metaindex/main.py
 metaindex/ocr.py
 metaindex/opf.py
-metaindex/query.py
+metaindex/proto.py
+metaindex/server.py
 metaindex/shared.py
-metaindex/sql.py
 metaindex/stores.py
 metaindex/version.py
 metaindex/xmlproxy.py
 metaindex/yaml.py
 metaindex.egg-info/PKG-INFO
 metaindex.egg-info/SOURCES.txt
 metaindex.egg-info/dependency_links.txt
@@ -135,17 +137,16 @@
 metaindex/indexers/ooxml.py
 metaindex/indexers/opendocument.py
 metaindex/indexers/pdf.py
 metaindex/indexers/ruleindexer.py
 misc/metaindex.conf
 misc/ranger_metaindex/__init__.py
 misc/ranger_metaindex/linemode.py
+tests/test_abc.py
 tests/test_cache.py
 tests/test_cacheentry.py
 tests/test_cleanup.py
 tests/test_collect.py
 tests/test_humanizer.py
 tests/test_indexers.py
 tests/test_json.py
-tests/test_query.py
-tests/test_ruleindexer.py
-tests/test_sqlaccess.py
+tests/test_ruleindexer.py
```

### Comparing `metaindex-1.4.0/misc/metaindex.conf` & `metaindex-2.0.0/misc/metaindex.conf`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 ## Example configuration file
 
 [General]
 ## Location of the cache file
 ## Default value is:
 # cache = ~/.cache/metaindex/index.db
 
+## Location of the server socket that local clients may
+## connect to. On modern systems it will default to /var/run/<uid>.
+## But if that doesn't exist, $HOME/.local/state will be used.
+# socket =
+
 ## Whether or not to look for metadata files in
 ## all parent directories of a file.
 # recursive-extra-metadata = yes
 
 ## What sidecar metadata files may apply collection
 ## metadata in their subdirectories, too.
 # recursive-collection-metadata = .metadata.json
@@ -18,14 +23,20 @@
 # ignore-dirs = .git
 #     System Volume Information
 
 ## What tags to not include in the index in a
 ## comma-separated list.
 # ignore-tags = Exif.Image.StripByteCounts, Exif.Image.StripOffsets
 
+[Server]
+# logfile =
+
+# loglevel = warning
+
+# autostart = yes
 
 [Synonyms]
 ## This section defines synonyms for metadata tags.
 ## For example, if you search for 'author', the following
 ## rule will make sure that also things like 'Exif.Image.Artist'
 ## is found (this is a default value):
 #author = extra.author, extra.artist, extra.creator, id3.artist, pdf.Author, rules.author, Exif.Image.Artist, comicbook.writer, xmp.dc.name
```

### Comparing `metaindex-1.4.0/misc/ranger_metaindex/linemode.py` & `metaindex-2.0.0/misc/ranger_metaindex/linemode.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/setup.py` & `metaindex-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import setuptools
 import pathlib
+import sys
 
 
 try:
     import docutils.core
     from docutils.writers import manpage
 except ImportError:
     docutils = None
@@ -76,18 +77,19 @@
     name='metaindex',
     version=version.__version__,
     description="Utilities to tag files",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license_file="LICENSE",
     license_files="LICENSE",
-    url="https://github.com/vonshednob/metaindex",
+    url="https://vonshednob.cc/metaindex",
     author="R",
     author_email="devel+metaindex@kakaomilchkuh.de",
-    entry_points={'console_scripts': ['metaindex=metaindex.main:run']},
+    entry_points={'console_scripts': ['metaindex=metaindex.main:run',
+                                      'metaindexserver=metaindex.server:run']},
     packages=['metaindex', 'metaindex/indexers'],
     package_data={'metaindex': compile_documentation()},
     data_files=[('share/man/man1', ['man/metaindex.1']),
                 ('share/applications', []),
                 ('share/doc/metaindex', ['misc/metaindex.conf']),
                 ('share/doc/metaindex/examples', example_files())],
     install_requires=[],
```

### Comparing `metaindex-1.4.0/tests/test_cache.py` & `metaindex-2.0.0/tests/test_cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -144,21 +144,7 @@
 
     def test_refresh(self):
         assert isinstance(self.cache, cache.CacheBase)
         self.cache.refresh(HERE)
         result = self.cache.get(THIS)
         self.assertEqual(len(result), 1)
         self.assertIn('mimetype', result[0].metadata)
-
-
-class TestMemoryCache(TestCacheBase):
-    """The tests for the MemoryCache"""
-
-    def cache_setup(self):
-        memcache = cache.MemoryCache(self.config)
-        memcache.tcache = NoCacheBackend()
-        memcache.start()
-        memcache.wait_for_reload()
-        return memcache
-
-    def tearDown(self):
-        self.cache.quit()
```

### Comparing `metaindex-1.4.0/tests/test_cacheentry.py` & `metaindex-2.0.0/tests/test_cacheentry.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/tests/test_cleanup.py` & `metaindex-2.0.0/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/tests/test_collect.py` & `metaindex-2.0.0/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/tests/test_humanizer.py` & `metaindex-2.0.0/tests/test_humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/tests/test_indexers.py` & `metaindex-2.0.0/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/tests/test_json.py` & `metaindex-2.0.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metaindex-1.4.0/tests/test_ruleindexer.py` & `metaindex-2.0.0/tests/test_ruleindexer.py`

 * *Files identical despite different names*

