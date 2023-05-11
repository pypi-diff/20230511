# Comparing `tmp/bardapi-0.1.0.tar.gz` & `tmp/bardapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.0.tar", last modified: Thu May 11 17:06:43 2023, max compression
+gzip compressed data, was "bardapi-0.1.1.tar", last modified: Thu May 11 17:40:49 2023, max compression
```

## Comparing `bardapi-0.1.0.tar` & `bardapi-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 17:06:43.945634 bardapi-0.1.0/
--rw-rw-rw-   0        0        0      973 2023-05-11 17:06:43.944168 bardapi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-05-11 16:34:47.000000 bardapi-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 17:06:43.924762 bardapi-0.1.0/bardapi/
--rw-rw-rw-   0        0        0      194 2023-05-11 17:05:53.000000 bardapi-0.1.0/bardapi/__init__.py
--rw-rw-rw-   0        0        0     2807 2023-05-11 17:06:29.000000 bardapi-0.1.0/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:06:43.941748 bardapi-0.1.0/bardapi.egg-info/
--rw-rw-rw-   0        0        0      973 2023-05-11 17:06:43.000000 bardapi-0.1.0/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-11 17:06:43.000000 bardapi-0.1.0/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 17:06:43.000000 bardapi-0.1.0/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-11 17:06:43.000000 bardapi-0.1.0/bardapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 17:06:43.000000 bardapi-0.1.0/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 17:06:43.945634 bardapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1753 2023-05-11 17:05:09.000000 bardapi-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 17:40:49.826256 bardapi-0.1.1/
+-rw-rw-rw-   0        0        0     2352 2023-05-11 17:40:49.824757 bardapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2023-05-11 17:40:13.000000 bardapi-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 17:40:49.807428 bardapi-0.1.1/bardapi/
+-rw-rw-rw-   0        0        0      194 2023-05-11 17:40:43.000000 bardapi-0.1.1/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     2807 2023-05-11 17:07:14.000000 bardapi-0.1.1/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-11 17:40:49.822239 bardapi-0.1.1/bardapi.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-11 17:40:49.000000 bardapi-0.1.1/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 17:40:49.826256 bardapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1753 2023-05-11 17:40:30.000000 bardapi-0.1.1/setup.py
```

### Comparing `bardapi-0.1.0/bardapi/core.py` & `bardapi-0.1.1/bardapi/core.py`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.0/setup.py` & `bardapi-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.0",
+    version="0.1.1",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="A package that returns Response of Google BARD through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
-    url="https://github.com/dsdanielpark/bard_api",
+    url="https://github.com/dsdanielpark/BARD_API",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
     install_requires=[
     ],
     keywords="BARD, Python, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

