# Comparing `tmp/python-upbit-api-1.0.0a0.tar.gz` & `tmp/python-upbit-api-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-upbit-api-1.0.0a0.tar", last modified: Mon May  1 07:32:02 2023, max compression
+gzip compressed data, was "dist/python-upbit-api-1.0.0a2.tar", last modified: Mon May  1 08:37:07 2023, max compression
```

## Comparing `python-upbit-api-1.0.0a0.tar` & `python-upbit-api-1.0.0a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 07:32:02.588703 python-upbit-api-1.0.0a0/
--rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python-upbit-api-1.0.0a0/LICENSE
--rw-r--r--   0 jihye      (501) staff       (20)      928 2023-05-01 07:32:02.588504 python-upbit-api-1.0.0a0/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)       47 2023-04-28 04:46:27.000000 python-upbit-api-1.0.0a0/README.md
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 07:32:02.586404 python-upbit-api-1.0.0a0/python_upbit_api.egg-info/
--rw-r--r--   0 jihye      (501) staff       (20)      928 2023-05-01 07:32:02.000000 python-upbit-api-1.0.0a0/python_upbit_api.egg-info/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)      349 2023-05-01 07:32:02.000000 python-upbit-api-1.0.0a0/python_upbit_api.egg-info/SOURCES.txt
--rw-r--r--   0 jihye      (501) staff       (20)        1 2023-05-01 07:32:02.000000 python-upbit-api-1.0.0a0/python_upbit_api.egg-info/dependency_links.txt
--rw-r--r--   0 jihye      (501) staff       (20)       44 2023-05-01 07:32:02.000000 python-upbit-api-1.0.0a0/python_upbit_api.egg-info/requires.txt
--rw-r--r--   0 jihye      (501) staff       (20)       12 2023-05-01 07:32:02.000000 python-upbit-api-1.0.0a0/python_upbit_api.egg-info/top_level.txt
--rw-r--r--   0 jihye      (501) staff       (20)       38 2023-05-01 07:32:02.588756 python-upbit-api-1.0.0a0/setup.cfg
--rw-r--r--   0 jihye      (501) staff       (20)     1764 2023-05-01 03:58:05.000000 python-upbit-api-1.0.0a0/setup.py
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 07:32:02.586949 python-upbit-api-1.0.0a0/tests/
--rw-r--r--   0 jihye      (501) staff       (20)        0 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a0/tests/__init__.py
--rw-r--r--   0 jihye      (501) staff       (20)      548 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a0/tests/test_exceptions.py
--rw-r--r--   0 jihye      (501) staff       (20)      947 2023-05-01 04:26:36.000000 python-upbit-api-1.0.0a0/tests/test_remaining_req.py
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 07:32:02.587796 python-upbit-api-1.0.0a0/upbit/
--rw-r--r--   0 jihye      (501) staff       (20)      753 2023-05-01 03:34:38.000000 python-upbit-api-1.0.0a0/upbit/__init__.py
--rw-r--r--   0 jihye      (501) staff       (20)     3375 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a0/upbit/exceptions.py
--rw-r--r--   0 jihye      (501) staff       (20)    50349 2023-05-01 02:20:15.000000 python-upbit-api-1.0.0a0/upbit/upbit.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.600436 python-upbit-api-1.0.0a2/
+-rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python-upbit-api-1.0.0a2/LICENSE
+-rw-r--r--   0 jihye      (501) staff       (20)      928 2023-05-01 08:37:07.600218 python-upbit-api-1.0.0a2/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)       47 2023-04-28 04:46:27.000000 python-upbit-api-1.0.0a2/README.md
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.597771 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/
+-rw-r--r--   0 jihye      (501) staff       (20)      928 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)      349 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jihye      (501) staff       (20)        1 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       44 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/requires.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       12 2023-05-01 08:37:07.000000 python-upbit-api-1.0.0a2/python_upbit_api.egg-info/top_level.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       38 2023-05-01 08:37:07.600499 python-upbit-api-1.0.0a2/setup.cfg
+-rw-r--r--   0 jihye      (501) staff       (20)     1599 2023-05-01 08:36:54.000000 python-upbit-api-1.0.0a2/setup.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.598430 python-upbit-api-1.0.0a2/tests/
+-rw-r--r--   0 jihye      (501) staff       (20)        0 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a2/tests/__init__.py
+-rw-r--r--   0 jihye      (501) staff       (20)      548 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a2/tests/test_exceptions.py
+-rw-r--r--   0 jihye      (501) staff       (20)      947 2023-05-01 04:26:36.000000 python-upbit-api-1.0.0a2/tests/test_remaining_req.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-01 08:37:07.599345 python-upbit-api-1.0.0a2/upbit/
+-rw-r--r--   0 jihye      (501) staff       (20)      753 2023-05-01 03:34:38.000000 python-upbit-api-1.0.0a2/upbit/__init__.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3375 2023-04-30 10:41:14.000000 python-upbit-api-1.0.0a2/upbit/exceptions.py
+-rw-r--r--   0 jihye      (501) staff       (20)    50349 2023-05-01 02:20:15.000000 python-upbit-api-1.0.0a2/upbit/upbit.py
```

### Comparing `python-upbit-api-1.0.0a0/LICENSE` & `python-upbit-api-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.0a0/PKG-INFO` & `python-upbit-api-1.0.0a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-upbit-api
-Version: 1.0.0a0
+Version: 1.0.0a2
 Summary: Python Upbit API Wrapper
 Home-page: https://github.com/designmeme/python-upbit-api
 Author: 이지혜 Lee Jihye
 Author-email: ghe.lee19@gmail.com
 Project-URL: Source, https://github.com/designmeme/python-upbit-api
 Project-URL: Tracker, https://github.com/designmeme/python-upbit-api/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-upbit-api-1.0.0a0/python_upbit_api.egg-info/PKG-INFO` & `python-upbit-api-1.0.0a2/python_upbit_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-upbit-api
-Version: 1.0.0a0
+Version: 1.0.0a2
 Summary: Python Upbit API Wrapper
 Home-page: https://github.com/designmeme/python-upbit-api
 Author: 이지혜 Lee Jihye
 Author-email: ghe.lee19@gmail.com
 Project-URL: Source, https://github.com/designmeme/python-upbit-api
 Project-URL: Tracker, https://github.com/designmeme/python-upbit-api/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-upbit-api-1.0.0a0/setup.py` & `python-upbit-api-1.0.0a2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-from pathlib import Path
-
 from setuptools import setup, find_packages
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 3 - Alpha"
-version = '1.0.0-alpha'
+version = '1.0.0-alpha.2'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-def get_requirements():
-    """Build the requirements list for this project"""
-    requirements_list = []
-
-    with Path("requirements.txt").open() as reqs:
-        for install in reqs:
-            if install.startswith("#"):
-                continue
-            requirements_list.append(install.strip())
-
-    return requirements_list
-
+install_requires = []
+with open("requirements.txt", "r") as reqs:
+    for install in reqs:
+        if install.startswith("#"):
+            continue
+        install_requires.append(install.strip())
 
 setup(
     name='python-upbit-api',
     version=version,
     description='Python Upbit API Wrapper',
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -37,15 +29,15 @@
         'Source': 'https://github.com/designmeme/python-upbit-api',
         'Tracker': 'https://github.com/designmeme/python-upbit-api/issues',
     },
     author='이지혜 Lee Jihye',
     author_email='ghe.lee19@gmail.com',
     python_requires='>=3.8',
     packages=find_packages(),
-    install_requires=get_requirements(),
+    install_requires=install_requires,
     # 참고: https://pypi.org/classifiers/
     classifiers=[
         release_status,
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `python-upbit-api-1.0.0a0/tests/test_exceptions.py` & `python-upbit-api-1.0.0a2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.0a0/tests/test_remaining_req.py` & `python-upbit-api-1.0.0a2/tests/test_remaining_req.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.0a0/upbit/__init__.py` & `python-upbit-api-1.0.0a2/upbit/__init__.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.0a0/upbit/exceptions.py` & `python-upbit-api-1.0.0a2/upbit/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.0a0/upbit/upbit.py` & `python-upbit-api-1.0.0a2/upbit/upbit.py`

 * *Files identical despite different names*

