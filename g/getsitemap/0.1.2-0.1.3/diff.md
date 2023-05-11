# Comparing `tmp/getsitemap-0.1.2.tar.gz` & `tmp/getsitemap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getsitemap-0.1.2.tar", last modified: Fri Mar 10 13:07:26 2023, max compression
+gzip compressed data, was "getsitemap-0.1.3.tar", last modified: Thu May 11 21:40:40 2023, max compression
```

## Comparing `getsitemap-0.1.2.tar` & `getsitemap-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-03-10 13:07:26.917266 getsitemap-0.1.2/
--rw-r--r--   0 james      (501) staff       (20)     1048 2023-03-10 13:06:01.000000 getsitemap-0.1.2/LICENSE.md
--rw-r--r--   0 james      (501) staff       (20)     1523 2023-03-10 13:07:26.917333 getsitemap-0.1.2/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      967 2023-03-10 13:06:01.000000 getsitemap-0.1.2/README.rst
--rw-r--r--   0 james      (501) staff       (20)      285 2023-03-10 13:06:01.000000 getsitemap-0.1.2/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)      642 2023-03-10 13:07:26.918016 getsitemap-0.1.2/setup.cfg
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-03-10 13:07:26.915890 getsitemap-0.1.2/src/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-03-10 13:07:26.917056 getsitemap-0.1.2/src/getsitemap.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     1523 2023-03-10 13:07:26.000000 getsitemap-0.1.2/src/getsitemap.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      229 2023-03-10 13:07:26.000000 getsitemap-0.1.2/src/getsitemap.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-03-10 13:07:26.000000 getsitemap-0.1.2/src/getsitemap.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-03-10 13:07:26.000000 getsitemap-0.1.2/src/getsitemap.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-03-10 13:07:26.917172 getsitemap-0.1.2/tests/
--rw-r--r--   0 james      (501) staff       (20)     1059 2023-03-10 13:06:01.000000 getsitemap-0.1.2/tests/test_retrieve_sitemap.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.277587 getsitemap-0.1.3/
+-rw-r--r--   0 james      (501) staff       (20)     1048 2023-05-11 21:19:35.000000 getsitemap-0.1.3/LICENSE.md
+-rw-r--r--   0 james      (501) staff       (20)     1523 2023-05-11 21:40:40.277648 getsitemap-0.1.3/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      967 2023-05-11 21:19:35.000000 getsitemap-0.1.3/README.rst
+-rw-r--r--   0 james      (501) staff       (20)      285 2023-05-11 21:19:35.000000 getsitemap-0.1.3/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)      642 2023-05-11 21:40:40.277897 getsitemap-0.1.3/setup.cfg
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.275972 getsitemap-0.1.3/src/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.277252 getsitemap-0.1.3/src/getsitemap.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     1523 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      229 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-05-11 21:40:40.000000 getsitemap-0.1.3/src/getsitemap.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-11 21:40:40.277378 getsitemap-0.1.3/tests/
+-rw-r--r--   0 james      (501) staff       (20)     1059 2023-05-11 21:19:35.000000 getsitemap-0.1.3/tests/test_retrieve_sitemap.py
```

### Comparing `getsitemap-0.1.2/LICENSE.md` & `getsitemap-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `getsitemap-0.1.2/PKG-INFO` & `getsitemap-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsitemap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library that retrieves all URLs in the sitemaps on a website.
 Home-page: https://github.com/capjamesg/getsitemap
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Project-URL: Bug Tracker, https://github.com/capjamesg/getsitemap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `getsitemap-0.1.2/README.rst` & `getsitemap-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `getsitemap-0.1.2/setup.cfg` & `getsitemap-0.1.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = getsitemap
-version = 0.1.2
+version = 0.1.3
 author = capjamesg
 author_email = jamesg@jamesg.blog
 description = A Python library that retrieves all URLs in the sitemaps on a website.
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/capjamesg/getsitemap
 project_urls =
```

### Comparing `getsitemap-0.1.2/src/getsitemap.egg-info/PKG-INFO` & `getsitemap-0.1.3/src/getsitemap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getsitemap
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library that retrieves all URLs in the sitemaps on a website.
 Home-page: https://github.com/capjamesg/getsitemap
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Project-URL: Bug Tracker, https://github.com/capjamesg/getsitemap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `getsitemap-0.1.2/tests/test_retrieve_sitemap.py` & `getsitemap-0.1.3/tests/test_retrieve_sitemap.py`

 * *Files identical despite different names*

