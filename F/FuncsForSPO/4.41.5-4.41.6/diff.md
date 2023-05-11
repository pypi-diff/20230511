# Comparing `tmp/FuncsForSPO-4.41.5.tar.gz` & `tmp/FuncsForSPO-4.41.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.41.5.tar", last modified: Wed May 10 14:23:08 2023, max compression
+gzip compressed data, was "FuncsForSPO-4.41.6.tar", last modified: Thu May 11 16:24:17 2023, max compression
```

## Comparing `FuncsForSPO-4.41.5.tar` & `FuncsForSPO-4.41.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.453839 FuncsForSPO-4.41.5/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.550184 FuncsForSPO-4.41.5/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.681483 FuncsForSPO-4.41.5/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.5/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.5/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.705228 FuncsForSPO-4.41.5/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.5/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.731466 FuncsForSPO-4.41.5/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.5/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.761403 FuncsForSPO-4.41.5/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.534764 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.808787 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.885851 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.904001 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.952927 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5017 2023-05-08 20:46:58.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.019847 FuncsForSPO-4.41.5/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.057196 FuncsForSPO-4.41.5/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69543 2023-05-10 14:22:37.000000 FuncsForSPO-4.41.5/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.171044 FuncsForSPO-4.41.5/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.5/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.205977 FuncsForSPO-4.41.5/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38180 2023-03-31 19:28:24.000000 FuncsForSPO-4.41.5/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.234329 FuncsForSPO-4.41.5/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.5/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.5/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.256723 FuncsForSPO-4.41.5/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.5/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.5/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:08.268361 FuncsForSPO-4.41.5/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.5/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:23:07.649978 FuncsForSPO-4.41.5/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-05-10 14:23:07.000000 FuncsForSPO-4.41.5/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-05-10 14:23:07.000000 FuncsForSPO-4.41.5/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:23:07.000000 FuncsForSPO-4.41.5/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-05-10 14:23:07.000000 FuncsForSPO-4.41.5/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-05-10 14:23:07.000000 FuncsForSPO-4.41.5/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.5/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-05-10 14:23:08.445517 FuncsForSPO-4.41.5/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 14:23:08.453839 FuncsForSPO-4.41.5/setup.cfg
--rw-rw-rw-   0        0        0     2150 2023-05-10 14:22:49.000000 FuncsForSPO-4.41.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.835623 FuncsForSPO-4.41.6/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.433119 FuncsForSPO-4.41.6/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.492286 FuncsForSPO-4.41.6/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.6/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.6/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.502469 FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.514999 FuncsForSPO-4.41.6/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.6/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.526733 FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.426682 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.598677 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.619199 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.627403 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.648415 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5017 2023-05-08 20:46:58.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.661082 FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.674362 FuncsForSPO-4.41.6/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    69543 2023-05-10 14:22:37.000000 FuncsForSPO-4.41.6/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.683934 FuncsForSPO-4.41.6/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.6/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.695520 FuncsForSPO-4.41.6/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.41.6/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.708750 FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.716673 FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.724924 FuncsForSPO-4.41.6/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.6/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 16:24:17.478895 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      350 2023-05-11 16:24:17.000000 FuncsForSPO-4.41.6/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.6/LICENSE
+-rw-rw-rw-   0        0        0     8027 2023-05-11 16:24:17.833547 FuncsForSPO-4.41.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 16:24:17.837186 FuncsForSPO-4.41.6/setup.cfg
+-rw-rw-rw-   0        0        0     2150 2023-05-11 16:24:12.000000 FuncsForSPO-4.41.6/setup.py
```

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/femails/femails.py` & `FuncsForSPO-4.41.6/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,20 +51,37 @@
     else:
         wdw.until(EC.presence_of_all_elements_located(locator))
     elements = driver.find_elements(*locator)
     len_elements = len(elements)
 
     for i in range(len_elements):
         elements[i].click()
+        sleep(0.5)
         
         
-def verifica_se_baixou_o_arquivo(diretorio_de_download, palavra_chave, sleep_time=2, return_file=False) -> bool:
+        
+def verifica_se_baixou_o_arquivo(diretorio_de_download, palavra_chave, sleep_time=0, return_file=False, timeout=30) -> bool|str:
+    """
+    Verifica se um arquivo com uma palavra-chave foi baixado para um diretório especificado.
+    :param diretorio_de_download: O caminho para o diretório de download.
+    :param palavra_chave: A palavra-chave a ser procurada nos nomes dos arquivos baixados.
+    :param sleep_time: O tempo a ser aguardado antes de verificar novamente o diretório de download.
+    :param return_file: Se deve ou não retornar o caminho do arquivo baixado.
+    :param timeout: O tempo máximo para esperar o arquivo ser baixado.
+    :return: Retorna True se o arquivo for baixado com sucesso, False caso contrário. Se return_file for True, 
+    ele retorna o caminho absoluto do arquivo baixado.
+    """
+
     _LOCAL_DE_DOWNLOAD = os.path.abspath(diretorio_de_download)
     baixou = False
+    start_time = time.time()
     while not baixou:
+        current_time = time.time()
+        if current_time - start_time > timeout:
+            return False
         lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
         lista_arquivos = [x.lower() for x in lista_arquivos]
         if len(lista_arquivos) == 0:
             sleep(sleep_time)
             baixou = False
             lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
             lista_arquivos = [x.lower() for x in lista_arquivos]
```

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-4.41.6/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO/utils/utils.py` & `FuncsForSPO-4.41.6/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-4.41.6/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.5
+Version: 4.41.6
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.5/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-4.41.6/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/LICENSE` & `FuncsForSPO-4.41.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/PKG-INFO` & `FuncsForSPO-4.41.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.41.5
+Version: 4.41.6
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.41.5/README.md` & `FuncsForSPO-4.41.6/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.41.5/setup.py` & `FuncsForSPO-4.41.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.41.5'
+version = '4.41.6'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

