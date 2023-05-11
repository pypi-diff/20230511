# Comparing `tmp/stactools-sentinel1-0.7.0.tar.gz` & `tmp/stactools-sentinel1-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-sentinel1-0.7.0.tar", last modified: Wed May 10 17:01:08 2023, max compression
+gzip compressed data, was "stactools-sentinel1-0.7.1.tar", last modified: Thu May 11 18:39:25 2023, max compression
```

## Comparing `stactools-sentinel1-0.7.0.tar` & `stactools-sentinel1-0.7.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:08.102771 stactools-sentinel1-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-10 17:01:08.102771 stactools-sentinel1-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-10 17:01:08.106771 stactools-sentinel1-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:08.098771 stactools-sentinel1-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:08.098771 stactools-sentinel1-0.7.0/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:08.098771 stactools-sentinel1-0.7.0/src/stactools/sentinel1/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:08.102771 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/metadata_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/product_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:08.102771 stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/rtc_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-10 17:00:46.000000 stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:01:08.102771 stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-10 17:01:08.000000 stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-10 17:01:08.000000 stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:01:08.000000 stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 17:01:08.000000 stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 17:01:08.000000 stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:25.311723 stactools-sentinel1-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-11 18:39:25.311723 stactools-sentinel1-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 18:39:25.311723 stactools-sentinel1-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:25.299722 stactools-sentinel1-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:25.299722 stactools-sentinel1-0.7.1/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:25.303722 stactools-sentinel1-0.7.1/src/stactools/sentinel1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:25.307723 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/metadata_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/product_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:25.307723 stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/rtc_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-11 18:39:01.000000 stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:39:25.311723 stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-11 18:39:25.000000 stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-11 18:39:25.000000 stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:39:25.000000 stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 18:39:25.000000 stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 18:39:25.000000 stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/top_level.txt
```

### Comparing `stactools-sentinel1-0.7.0/LICENSE` & `stactools-sentinel1-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/PKG-INFO` & `stactools-sentinel1-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel1
-Version: 0.7.0
+Version: 0.7.1
 Summary: stactools subpackage for creating sentinel1 STACs
 Home-page: https://github.com/stactools-packages/sentinel1
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://github.com/stactools-packages/sentinel1
 Project-URL: Issues, https://github.com/stactools-packages/sentinel1/issues
 Keywords: stactools,pystac,catalog,STAC,sentinel,GRD,radar
```

### Comparing `stactools-sentinel1-0.7.0/README.md` & `stactools-sentinel1-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/setup.cfg` & `stactools-sentinel1-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/bands.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/bands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/commands.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/constants.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/metadata_links.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/metadata_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     + "-([0-9a-f]{6})"
     + ".*$"
 )
 
 
 def extract_polarisation(href: str) -> str:
     if match := (
-        re.search(r"ew-(hh|hv|vv|vh)\.(?:tiff|xml)$", href)
+        re.search(r"-(hh|hv|vv|vh)\.(?:tiff|xml)$", href)
         or re.search(r"s1(?:a|b)-iw-grd-(hh|hv|vv|vh)-[-\w]+\.(?:tiff|xml)$", href)
     ):
         return match.group(1).upper()
 
     raise RuntimeError(f"Failed to match polarisation: {href}")
```

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/product_metadata.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/product_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/properties.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/properties.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/grd/stac.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/grd/stac.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/commands.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/constants.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/rtc_metadata.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/rtc_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools/sentinel1/rtc/stac.py` & `stactools-sentinel1-0.7.1/src/stactools/sentinel1/rtc/stac.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/PKG-INFO` & `stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel1
-Version: 0.7.0
+Version: 0.7.1
 Summary: stactools subpackage for creating sentinel1 STACs
 Home-page: https://github.com/stactools-packages/sentinel1
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://github.com/stactools-packages/sentinel1
 Project-URL: Issues, https://github.com/stactools-packages/sentinel1/issues
 Keywords: stactools,pystac,catalog,STAC,sentinel,GRD,radar
```

### Comparing `stactools-sentinel1-0.7.0/src/stactools_sentinel1.egg-info/SOURCES.txt` & `stactools-sentinel1-0.7.1/src/stactools_sentinel1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

