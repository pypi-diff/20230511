# Comparing `tmp/unitlab-1.8.1.tar.gz` & `tmp/unitlab-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unitlab-1.8.1.tar", last modified: Thu May 11 05:47:09 2023, max compression
+gzip compressed data, was "dist/unitlab-1.8.2.tar", last modified: Thu May 11 05:55:42 2023, max compression
```

## Comparing `unitlab-1.8.1.tar` & `unitlab-1.8.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:47:09.000000 unitlab-1.8.1/
--rw-r--r--   0 max        (501) staff       (20)     1060 2023-05-11 05:38:06.000000 unitlab-1.8.1/LICENSE.md
--rw-r--r--   0 max        (501) staff       (20)       84 2023-05-11 05:38:06.000000 unitlab-1.8.1/MANIFEST.in
--rw-r--r--   0 max        (501) staff       (20)      634 2023-05-11 05:47:09.000000 unitlab-1.8.1/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     2016 2023-05-11 05:38:06.000000 unitlab-1.8.1/README.md
--rw-r--r--   0 max        (501) staff       (20)      106 2023-05-11 05:47:09.000000 unitlab-1.8.1/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)     1142 2023-05-11 05:47:04.000000 unitlab-1.8.1/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab/
--rw-r--r--   0 max        (501) staff       (20)       70 2023-05-11 05:38:06.000000 unitlab-1.8.1/src/unitlab/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     9702 2023-05-11 05:38:06.000000 unitlab-1.8.1/src/unitlab/client.py
--rw-r--r--   0 max        (501) staff       (20)     7950 2023-05-11 05:38:06.000000 unitlab-1.8.1/src/unitlab/core.py
--rw-r--r--   0 max        (501) staff       (20)      746 2023-05-11 05:38:06.000000 unitlab-1.8.1/src/unitlab/exceptions.py
--rw-r--r--   0 max        (501) staff       (20)     4109 2023-05-11 05:38:06.000000 unitlab-1.8.1/src/unitlab/pretty.py
--rw-r--r--   0 max        (501) staff       (20)     4444 2023-05-11 05:42:52.000000 unitlab-1.8.1/src/unitlab/run.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab.egg-info/
--rw-r--r--   0 max        (501) staff       (20)      634 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      396 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       46 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)       61 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        8 2023-05-11 05:47:09.000000 unitlab-1.8.1/src/unitlab.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:55:42.000000 unitlab-1.8.2/
+-rw-r--r--   0 max        (501) staff       (20)     1060 2023-05-11 05:38:06.000000 unitlab-1.8.2/LICENSE.md
+-rw-r--r--   0 max        (501) staff       (20)       84 2023-05-11 05:38:06.000000 unitlab-1.8.2/MANIFEST.in
+-rw-r--r--   0 max        (501) staff       (20)      603 2023-05-11 05:55:42.000000 unitlab-1.8.2/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     2016 2023-05-11 05:38:06.000000 unitlab-1.8.2/README.md
+-rw-r--r--   0 max        (501) staff       (20)      106 2023-05-11 05:55:42.000000 unitlab-1.8.2/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)     1142 2023-05-11 05:55:28.000000 unitlab-1.8.2/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab/
+-rw-r--r--   0 max        (501) staff       (20)       70 2023-05-11 05:38:06.000000 unitlab-1.8.2/src/unitlab/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     9702 2023-05-11 05:38:06.000000 unitlab-1.8.2/src/unitlab/client.py
+-rw-r--r--   0 max        (501) staff       (20)     7950 2023-05-11 05:38:06.000000 unitlab-1.8.2/src/unitlab/core.py
+-rw-r--r--   0 max        (501) staff       (20)      746 2023-05-11 05:38:06.000000 unitlab-1.8.2/src/unitlab/exceptions.py
+-rw-r--r--   0 max        (501) staff       (20)     4109 2023-05-11 05:38:06.000000 unitlab-1.8.2/src/unitlab/pretty.py
+-rw-r--r--   0 max        (501) staff       (20)     4451 2023-05-11 05:51:43.000000 unitlab-1.8.2/src/unitlab/run.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)      603 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      396 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       45 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)       61 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        8 2023-05-11 05:55:42.000000 unitlab-1.8.2/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.8.1/LICENSE.md` & `unitlab-1.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.1/PKG-INFO` & `unitlab-1.8.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.1
-Summary: UNKNOWN
+Version: 1.8.2
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
-Description: UNKNOWN
 Keywords: unitlab-sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.md
```

### Comparing `unitlab-1.8.1/README.md` & `unitlab-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.1/setup.py` & `unitlab-1.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.8.1",
+    version="1.8.2",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.8.1/src/unitlab/client.py` & `unitlab-1.8.2/src/unitlab/client.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.1/src/unitlab/core.py` & `unitlab-1.8.2/src/unitlab/core.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.1/src/unitlab/exceptions.py` & `unitlab-1.8.2/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.1/src/unitlab/pretty.py` & `unitlab-1.8.2/src/unitlab/pretty.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.1/src/unitlab/run.py` & `unitlab-1.8.2/src/unitlab/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     # Task List
     parser_task_list = subparsers.add_parser("tasks", help="Get task list")
     parser_task_list.add_argument("-k", "--api_key", **core.api_key_template)
     parser_task_list.set_defaults(func=core.task_list)
 
     # Task Detail
-    parser_task_detail = subparsers.add_parser("task", help="Get task detail")
+    parser_task_detail = subparsers.add_parser("task-detail", help="Get task detail")
     parser_task_detail.add_argument(
         "-id", "--uuid", type=core.validate_uuid, required=True, help="Task uuid"
     )
     parser_task_detail.add_argument("-k", "--api_key", **core.api_key_template)
     parser_task_detail.set_defaults(func=core.task_detail)
 
     # Task DataSources
```

### Comparing `unitlab-1.8.1/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.8.2/src/unitlab.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.1
-Summary: UNKNOWN
+Version: 1.8.2
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
-Description: UNKNOWN
 Keywords: unitlab-sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.md
```

