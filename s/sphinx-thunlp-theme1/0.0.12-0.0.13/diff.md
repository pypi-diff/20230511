# Comparing `tmp/sphinx_thunlp_theme1-0.0.12.tar.gz` & `tmp/sphinx_thunlp_theme1-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_thunlp_theme1-0.0.12.tar", last modified: Thu May 11 15:21:14 2023, max compression
+gzip compressed data, was "sphinx_thunlp_theme1-0.0.13.tar", last modified: Thu May 11 15:25:43 2023, max compression
```

## Comparing `sphinx_thunlp_theme1-0.0.12.tar` & `sphinx_thunlp_theme1-0.0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:21:14.768678 sphinx_thunlp_theme1-0.0.12/
--rw-rw-rw-   0        0        0     1192 2023-05-11 15:21:14.768678 sphinx_thunlp_theme1-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-05-11 14:56:13.000000 sphinx_thunlp_theme1-0.0.12/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 15:21:14.768678 sphinx_thunlp_theme1-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-11 15:20:21.000000 sphinx_thunlp_theme1-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:21:14.749728 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1/
--rw-rw-rw-   0        0        0      607 2023-05-11 15:20:11.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:21:14.766683 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/
--rw-rw-rw-   0        0        0     1192 2023-05-11 15:21:14.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-05-11 15:21:14.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:21:14.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-11 15:21:14.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-11 15:20:51.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-11 15:21:14.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-11 15:21:14.000000 sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:25:43.484863 sphinx_thunlp_theme1-0.0.13/
+-rw-rw-rw-   0        0        0     1192 2023-05-11 15:25:43.484863 sphinx_thunlp_theme1-0.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-05-11 14:56:13.000000 sphinx_thunlp_theme1-0.0.13/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:25:43.485861 sphinx_thunlp_theme1-0.0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-11 15:25:32.000000 sphinx_thunlp_theme1-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:25:43.466687 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1/
+-rw-rw-rw-   0        0        0      607 2023-05-11 15:20:11.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:25:43.482869 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/
+-rw-rw-rw-   0        0        0     1192 2023-05-11 15:25:43.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-11 15:25:43.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:25:43.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-11 15:25:43.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-11 15:25:43.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-11 15:25:43.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-11 15:25:43.000000 sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/top_level.txt
```

### Comparing `sphinx_thunlp_theme1-0.0.12/PKG-INFO` & `sphinx_thunlp_theme1-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_thunlp_theme1
-Version: 0.0.12
+Version: 0.0.13
 Summary: THUNLP open-source project theme for Sphinx
 Home-page: https://github.com/a710128/sphinx_thunlp_docs
 Author: a710128
 Author-email: qbjooo@qq.com
 License: MIT
 Description: # Thunlp Project Template
```

### Comparing `sphinx_thunlp_theme1-0.0.12/setup.py` & `sphinx_thunlp_theme1-0.0.13/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sphinx_thunlp_theme1',
-    version='0.0.12',
+    version='0.0.13',
     url='https://github.com/a710128/sphinx_thunlp_docs',
     license='MIT',
     author='a710128',
     author_email='qbjooo@qq.com',
     description='THUNLP open-source project theme for Sphinx',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
```

### Comparing `sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1/__init__.py` & `sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_thunlp_theme1-0.0.12/sphinx_thunlp_theme1.egg-info/PKG-INFO` & `sphinx_thunlp_theme1-0.0.13/sphinx_thunlp_theme1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-thunlp-theme1
-Version: 0.0.12
+Version: 0.0.13
 Summary: THUNLP open-source project theme for Sphinx
 Home-page: https://github.com/a710128/sphinx_thunlp_docs
 Author: a710128
 Author-email: qbjooo@qq.com
 License: MIT
 Description: # Thunlp Project Template
```

