# Comparing `tmp/bp_data_fabric-1.0.8.tar.gz` & `tmp/bp_data_fabric-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-1.0.8.tar", last modified: Tue May  9 06:28:07 2023, max compression
+gzip compressed data, was "bp_data_fabric-1.0.9.tar", last modified: Wed May 10 10:58:23 2023, max compression
```

## Comparing `bp_data_fabric-1.0.8.tar` & `bp_data_fabric-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 06:28:07.877772 bp_data_fabric-1.0.8/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.8/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-09 06:28:07.877269 bp_data_fabric-1.0.8/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.8/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 06:28:07.874405 bp_data_fabric-1.0.8/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-09 06:28:07.000000 bp_data_fabric-1.0.8/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-09 06:28:07.000000 bp_data_fabric-1.0.8/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-09 06:28:07.000000 bp_data_fabric-1.0.8/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-09 06:28:07.000000 bp_data_fabric-1.0.8/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-09 06:28:07.000000 bp_data_fabric-1.0.8/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-09 06:28:07.876181 bp_data_fabric-1.0.8/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1158 2023-05-04 10:06:32.000000 bp_data_fabric-1.0.8/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2811 2023-05-04 09:57:35.000000 bp_data_fabric-1.0.8/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-09 06:28:07.877966 bp_data_fabric-1.0.8/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-09 06:27:47.000000 bp_data_fabric-1.0.8/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:58:23.018560 bp_data_fabric-1.0.9/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.9/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     4467 2023-05-10 10:58:23.018234 bp_data_fabric-1.0.9/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3211 2023-05-10 06:55:05.000000 bp_data_fabric-1.0.9/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:58:23.016934 bp_data_fabric-1.0.9/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     4467 2023-05-10 10:58:22.000000 bp_data_fabric-1.0.9/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-10 10:58:22.000000 bp_data_fabric-1.0.9/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-10 10:58:22.000000 bp_data_fabric-1.0.9/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-10 10:58:22.000000 bp_data_fabric-1.0.9/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-10 10:58:22.000000 bp_data_fabric-1.0.9/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:58:23.017699 bp_data_fabric-1.0.9/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1158 2023-05-04 10:06:32.000000 bp_data_fabric-1.0.9/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2811 2023-05-04 09:57:35.000000 bp_data_fabric-1.0.9/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-10 10:58:23.018671 bp_data_fabric-1.0.9/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-10 10:58:14.000000 bp_data_fabric-1.0.9/setup.py
```

### Comparing `bp_data_fabric-1.0.8/LICENSE` & `bp_data_fabric-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.8/data_fabric/__init__.py` & `bp_data_fabric-1.0.9/data_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.8/data_fabric/components.py` & `bp_data_fabric-1.0.9/data_fabric/components.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.8/setup.py` & `bp_data_fabric-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="1.0.8",
+    version="1.0.9",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",    
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

