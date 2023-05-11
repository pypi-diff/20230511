# Comparing `tmp/markl-0.0.3.tar.gz` & `tmp/markl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markl-0.0.3.tar", last modified: Tue Nov  1 12:28:58 2022, max compression
+gzip compressed data, was "markl-0.0.4.tar", last modified: Thu May 11 15:17:44 2023, max compression
```

## Comparing `markl-0.0.3.tar` & `markl-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 12:28:58.211046 markl-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-11-01 12:28:47.000000 markl-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-01 12:28:58.207046 markl-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-11-01 12:28:47.000000 markl-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 12:28:58.207046 markl-0.0.3/markl/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-01 12:28:47.000000 markl-0.0.3/markl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-01 12:28:47.000000 markl-0.0.3/markl/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-01 12:28:47.000000 markl-0.0.3/markl/get_tsxs.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-01 12:28:47.000000 markl-0.0.3/markl/mark.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-11-01 12:28:47.000000 markl-0.0.3/markl/rollback.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 12:28:58.207046 markl-0.0.3/markl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-01 12:28:58.000000 markl-0.0.3/markl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-01 12:28:58.000000 markl-0.0.3/markl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 12:28:58.000000 markl-0.0.3/markl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-01 12:28:58.000000 markl-0.0.3/markl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-01 12:28:58.000000 markl-0.0.3/markl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 12:28:58.211046 markl-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-11-01 12:28:47.000000 markl-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:17:44.481596 markl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-11 15:17:33.000000 markl-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-11 15:17:44.481596 markl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 15:17:33.000000 markl-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:17:44.481596 markl-0.0.4/markl/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 15:17:33.000000 markl-0.0.4/markl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 15:17:33.000000 markl-0.0.4/markl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-11 15:17:33.000000 markl-0.0.4/markl/get_tsxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-11 15:17:33.000000 markl-0.0.4/markl/mark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-11 15:17:33.000000 markl-0.0.4/markl/rollback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:17:44.481596 markl-0.0.4/markl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-11 15:17:44.000000 markl-0.0.4/markl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 15:17:44.000000 markl-0.0.4/markl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:17:44.000000 markl-0.0.4/markl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 15:17:44.000000 markl-0.0.4/markl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 15:17:44.000000 markl-0.0.4/markl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:17:44.481596 markl-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-11 15:17:33.000000 markl-0.0.4/setup.py
```

### Comparing `markl-0.0.3/LICENSE` & `markl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `markl-0.0.3/markl/mark.py` & `markl-0.0.4/markl/mark.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         for tag in Config.TAGS:
             idx = 0
             while (idx := file_body.find('<' + tag, idx + 1)) != -1:
                 uuid = uuid4()
                 next_word = file_body[idx + 1 + len(tag):idx + 1 + len(tag) + 5]
                 next_symbol = file_body[idx + 1 + len(tag):idx + 1 + len(tag) + 1]
                 if next_word != f' {Config.ATTR}' and (next_symbol == ' ' or next_symbol == '\n'):
-                    file_body = file_body[:idx + 1 + len(tag)] + f' {Config.ATTR}="{uuid}" ' + file_body[idx + 1 + len(tag):]
+                    file_body = file_body[:idx + 1 + len(tag)] + f' {Config.ATTR}="{Config.ATTR_PREFIX}{uuid}"' + file_body[idx + 1 + len(tag):]
 
         # Write the file out again
         with open(file_name, 'w') as file:
             file.write(file_body)
```

### Comparing `markl-0.0.3/setup.py` & `markl-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 README = open("README.md").read()
 setup(
     name="markl",
-    version="0.0.3",
+    version="0.0.4",
     description=".tsx locator marker",
     long_description=README,
     long_description_content_type="text/markdown",
-    author="2GIS Test Labs",
-    author_email="test-labs@2gis.ru",
+    author="Yuriy Sagitov",
+    author_email="pro100.ko10ok@gmail.com",
     python_requires=">=3.8.0",
-    url="https://github.com/2gis-test-labs/markl",
+    url="https://github.com/ko10ok/markl",
     license="Apache-2.0",
     packages=find_packages(exclude=("tests",)),
     install_requires=[],
     entry_points={
         "console_scripts": [
             "markl-do = markl:mark",
             "markl-rollback = markl:rollback"
```

