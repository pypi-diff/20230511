# Comparing `tmp/calfps-0.0.1.tar.gz` & `tmp/calfps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfps-0.0.1.tar", last modified: Thu May 11 02:30:08 2023, max compression
+gzip compressed data, was "calfps-0.0.2.tar", last modified: Thu May 11 04:53:29 2023, max compression
```

## Comparing `calfps-0.0.1.tar` & `calfps-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 02:30:08.845248 calfps-0.0.1/
--rw-rw-r--   0 alyce     (1000) alyce     (1000)     1065 2023-05-11 02:13:38.000000 calfps-0.0.1/LICENSE.txt
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-05-11 02:30:08.845248 calfps-0.0.1/PKG-INFO
--rw-rw-r--   0 alyce     (1000) alyce     (1000)       73 2023-05-11 02:14:48.000000 calfps-0.0.1/README.md
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      103 2023-05-11 02:12:02.000000 calfps-0.0.1/pyproject.toml
--rw-rw-r--   0 alyce     (1000) alyce     (1000)       38 2023-05-11 02:30:08.845248 calfps-0.0.1/setup.cfg
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      792 2023-05-11 02:28:18.000000 calfps-0.0.1/setup.py
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 02:30:08.841248 calfps-0.0.1/src/
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 02:30:08.845248 calfps-0.0.1/src/calculate/
--rw-rw-r--   0 alyce     (1000) alyce     (1000)        0 2023-05-11 01:50:42.000000 calfps-0.0.1/src/calculate/__init__.py
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      146 2023-05-11 02:02:34.000000 calfps-0.0.1/src/calculate/fps.py
-drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 02:30:08.845248 calfps-0.0.1/src/calfps.egg-info/
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-05-11 02:30:08.000000 calfps-0.0.1/src/calfps.egg-info/PKG-INFO
--rw-rw-r--   0 alyce     (1000) alyce     (1000)      228 2023-05-11 02:30:08.000000 calfps-0.0.1/src/calfps.egg-info/SOURCES.txt
--rw-rw-r--   0 alyce     (1000) alyce     (1000)        1 2023-05-11 02:30:08.000000 calfps-0.0.1/src/calfps.egg-info/dependency_links.txt
--rw-rw-r--   0 alyce     (1000) alyce     (1000)       10 2023-05-11 02:30:08.000000 calfps-0.0.1/src/calfps.egg-info/top_level.txt
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 04:53:29.893578 calfps-0.0.2/
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)     1065 2023-05-11 02:13:38.000000 calfps-0.0.2/LICENSE.txt
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-05-11 04:53:29.893578 calfps-0.0.2/PKG-INFO
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)       73 2023-05-11 02:14:48.000000 calfps-0.0.2/README.md
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      103 2023-05-11 02:12:02.000000 calfps-0.0.2/pyproject.toml
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)       38 2023-05-11 04:53:29.893578 calfps-0.0.2/setup.cfg
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      792 2023-05-11 04:53:17.000000 calfps-0.0.2/setup.py
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 04:53:29.889578 calfps-0.0.2/src/
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 04:53:29.893578 calfps-0.0.2/src/calculate/
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)        0 2023-05-11 01:50:42.000000 calfps-0.0.2/src/calculate/__init__.py
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      148 2023-05-11 04:53:03.000000 calfps-0.0.2/src/calculate/fps.py
+drwxrwxr-x   0 alyce     (1000) alyce     (1000)        0 2023-05-11 04:53:29.893578 calfps-0.0.2/src/calfps.egg-info/
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      570 2023-05-11 04:53:29.000000 calfps-0.0.2/src/calfps.egg-info/PKG-INFO
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)      228 2023-05-11 04:53:29.000000 calfps-0.0.2/src/calfps.egg-info/SOURCES.txt
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)        1 2023-05-11 04:53:29.000000 calfps-0.0.2/src/calfps.egg-info/dependency_links.txt
+-rw-rw-r--   0 alyce     (1000) alyce     (1000)       10 2023-05-11 04:53:29.000000 calfps-0.0.2/src/calfps.egg-info/top_level.txt
```

### Comparing `calfps-0.0.1/LICENSE.txt` & `calfps-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `calfps-0.0.1/PKG-INFO` & `calfps-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfps
-Version: 0.0.1
+Version: 0.0.2
 Summary: calculating fps as simple
 Home-page: https://github.com/Junhojuno/test-fps
 Author: Junhojuno
 Author-email: rlawnsgh2245@gmail.com
 Project-URL: Bug Tracker, https://github.com/Junhojuno/test-fps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calfps-0.0.1/setup.py` & `calfps-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="calfps",
-    version="0.0.1",
+    version="0.0.2",
     author="Junhojuno",
     author_email="rlawnsgh2245@gmail.com",
     description="calculating fps as simple",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Junhojuno/test-fps",
     project_urls={
```

### Comparing `calfps-0.0.1/src/calfps.egg-info/PKG-INFO` & `calfps-0.0.2/src/calfps.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfps
-Version: 0.0.1
+Version: 0.0.2
 Summary: calculating fps as simple
 Home-page: https://github.com/Junhojuno/test-fps
 Author: Junhojuno
 Author-email: rlawnsgh2245@gmail.com
 Project-URL: Bug Tracker, https://github.com/Junhojuno/test-fps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

