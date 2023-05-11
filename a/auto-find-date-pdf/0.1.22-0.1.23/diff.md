# Comparing `tmp/auto_find_date_pdf-0.1.22.tar.gz` & `tmp/auto_find_date_pdf-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_find_date_pdf-0.1.22.tar", last modified: Mon Apr 24 03:27:05 2023, max compression
+gzip compressed data, was "auto_find_date_pdf-0.1.23.tar", last modified: Thu May 11 02:27:25 2023, max compression
```

## Comparing `auto_find_date_pdf-0.1.22.tar` & `auto_find_date_pdf-0.1.23.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:27:05.757635 auto_find_date_pdf-0.1.22/
--rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.22/LICENSE
--rw-rw-rw-   0        0        0      236 2023-04-24 03:27:05.756637 auto_find_date_pdf-0.1.22/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-04-24 03:26:39.000000 auto_find_date_pdf-0.1.22/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 03:27:05.756637 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/
--rw-rw-rw-   0        0        0      236 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      921 2023-04-24 03:26:48.000000 auto_find_date_pdf-0.1.22/main.py
--rw-rw-rw-   0        0        0       42 2023-04-24 03:27:05.757635 auto_find_date_pdf-0.1.22/setup.cfg
--rw-rw-rw-   0        0        0      554 2023-04-24 03:26:54.000000 auto_find_date_pdf-0.1.22/setup.py
--rw-rw-rw-   0        0        0     6858 2023-04-24 03:24:11.000000 auto_find_date_pdf-0.1.22/text_search.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:27:25.062064 auto_find_date_pdf-0.1.23/
+-rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.23/LICENSE
+-rw-rw-rw-   0        0        0     2077 2023-05-11 02:27:25.062064 auto_find_date_pdf-0.1.23/PKG-INFO
+-rw-rw-rw-   0        0        0     1781 2023-05-10 20:43:13.000000 auto_find_date_pdf-0.1.23/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-10 20:30:13.000000 auto_find_date_pdf-0.1.23/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 02:27:25.061061 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/
+-rw-rw-rw-   0        0        0     2077 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-05-11 02:27:25.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      920 2023-05-11 00:11:23.000000 auto_find_date_pdf-0.1.23/main.py
+-rw-rw-rw-   0        0        0       42 2023-05-11 02:27:25.062064 auto_find_date_pdf-0.1.23/setup.cfg
+-rw-rw-rw-   0        0        0      732 2023-05-11 02:27:14.000000 auto_find_date_pdf-0.1.23/setup.py
+-rw-rw-rw-   0        0        0     2227 2023-04-24 03:02:35.000000 auto_find_date_pdf-0.1.23/test_fast.py
+-rw-rw-rw-   0        0        0     6858 2023-04-24 03:24:11.000000 auto_find_date_pdf-0.1.23/text_search.py
```

### Comparing `auto_find_date_pdf-0.1.22/LICENSE` & `auto_find_date_pdf-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.22/main.py` & `auto_find_date_pdf-0.1.23/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             value = value.isoformat()
         data[column.name] = value
     return data
 
 
 def image_rotate(imagename: str, rotateDegree: int):
     from PIL import Image
-    # Giving The Original image Directory
+    # Giving The Original image Director
     Original_Image = Image.open(imagename)
     rotated_image1 = Original_Image.transpose(Image.ROTATE_90)
     rotated_image1.save(imagename)
 
 
 def safe_naming(name):
     keepcharacters = ('.', '_')
```

### Comparing `auto_find_date_pdf-0.1.22/text_search.py` & `auto_find_date_pdf-0.1.23/text_search.py`

 * *Files identical despite different names*

