# Comparing `tmp/cbcmgr-1.2.1.tar.gz` & `tmp/cbcmgr-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.2.1.tar", last modified: Wed May 10 18:49:52 2023, max compression
+gzip compressed data, was "cbcmgr-1.2.2.tar", last modified: Wed May 10 22:27:35 2023, max compression
```

## Comparing `cbcmgr-1.2.1.tar` & `cbcmgr-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 18:49:52.490512 cbcmgr-1.2.1/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.1/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-10 18:49:52.490390 cbcmgr-1.2.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 18:49:52.487526 cbcmgr-1.2.1/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.1/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.1/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.1/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.1/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     4098 2023-05-02 21:24:28.000000 cbcmgr-1.2.1/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    10824 2023-05-10 18:40:42.000000 cbcmgr-1.2.1/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.1/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.1/cbcmgr/schema.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 18:49:52.490205 cbcmgr-1.2.1/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      343 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-10 18:49:52.490555 cbcmgr-1.2.1/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      705 2023-05-10 18:40:59.000000 cbcmgr-1.2.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 22:27:35.532161 cbcmgr-1.2.2/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.2/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-10 22:27:35.532018 cbcmgr-1.2.2/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.2/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 22:27:35.530299 cbcmgr-1.2.2/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.2/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.2/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.2/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.2/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     4098 2023-05-02 21:24:28.000000 cbcmgr-1.2.2/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    10824 2023-05-10 18:40:42.000000 cbcmgr-1.2.2/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.2/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.2/cbcmgr/schema.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 22:27:35.531798 cbcmgr-1.2.2/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-10 22:27:35.000000 cbcmgr-1.2.2/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      343 2023-05-10 22:27:35.000000 cbcmgr-1.2.2/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-10 22:27:35.000000 cbcmgr-1.2.2/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       57 2023-05-10 22:27:35.000000 cbcmgr-1.2.2/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-05-10 22:27:35.000000 cbcmgr-1.2.2/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-10 22:27:35.532215 cbcmgr-1.2.2/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      705 2023-05-10 22:09:16.000000 cbcmgr-1.2.2/setup.py
```

### Comparing `cbcmgr-1.2.1/LICENSE.txt` & `cbcmgr-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/PKG-INFO` & `cbcmgr-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.1
+Version: 1.2.2
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.1/README.md` & `cbcmgr-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr/cb_connect.py` & `cbcmgr-1.2.2/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr/cb_management.py` & `cbcmgr-1.2.2/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr/cb_session.py` & `cbcmgr-1.2.2/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr/exceptions.py` & `cbcmgr-1.2.2/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.2.2/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr/retry.py` & `cbcmgr-1.2.2/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr/schema.py` & `cbcmgr-1.2.2/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.1/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.2.2/cbcmgr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.1
+Version: 1.2.2
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.1/setup.py` & `cbcmgr-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.2.1',
+    version='1.2.2',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

