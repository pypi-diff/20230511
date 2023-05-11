# Comparing `tmp/gandai-1.1.2.tar.gz` & `tmp/gandai-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.2.tar", last modified: Wed May 10 05:24:57 2023, max compression
+gzip compressed data, was "gandai-1.1.3.tar", last modified: Thu May 11 12:12:21 2023, max compression
```

## Comparing `gandai-1.1.2.tar` & `gandai-1.1.3.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.152320 gandai-1.1.2/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.2/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-10 05:24:57.151903 gandai-1.1.2/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.147821 gandai-1.1.2/gandai/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-02 13:58:25.000000 gandai-1.1.2/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.150184 gandai-1.1.2/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      179 2023-04-07 16:05:45.000000 gandai-1.1.2/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.2/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.2/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-1.1.2/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.2/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3736 2023-05-09 18:28:28.000000 gandai-1.1.2/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5999 2023-05-09 18:36:56.000000 gandai-1.1.2/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16707 2023-05-10 05:05:31.000000 gandai-1.1.2/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.2/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7725 2023-05-09 18:21:29.000000 gandai-1.1.2/gandai/__pycache__/sources.cpython-311.pyc
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.150894 gandai-1.1.2/gandai/adapters/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-1.1.2/gandai/adapters/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.151387 gandai-1.1.2/gandai/adapters/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      188 2023-04-07 16:05:45.000000 gandai-1.1.2/gandai/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1875 2023-04-10 12:31:26.000000 gandai-1.1.2/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      924 2023-04-07 16:06:33.000000 gandai-1.1.2/gandai/adapters/__pycache__/filters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    14686 2023-04-14 19:20:28.000000 gandai-1.1.2/gandai/adapters/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1223 2023-05-05 19:45:58.000000 gandai-1.1.2/gandai/adapters/dealcloud.py
--rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-1.1.2/gandai/adapters/filters.py
--rw-r--r--   0 parker     (501) staff       (20)    10094 2023-05-04 03:54:50.000000 gandai-1.1.2/gandai/adapters/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1704 2023-03-30 16:03:27.000000 gandai-1.1.2/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-12 13:11:26.000000 gandai-1.1.2/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     3089 2023-05-09 18:28:27.000000 gandai-1.1.2/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.151733 gandai-1.1.2/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.2/gandai/migrations/__init__.py
--rw-r--r--   0 parker     (501) staff       (20)     2536 2023-05-09 21:46:03.000000 gandai-1.1.2/gandai/migrations/create_db.sql
--rw-r--r--   0 parker     (501) staff       (20)     1764 2023-04-12 12:53:47.000000 gandai-1.1.2/gandai/migrations/dealcloud_to_gandai.py
--rw-r--r--   0 parker     (501) staff       (20)     2560 2023-05-09 18:36:54.000000 gandai-1.1.2/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    17549 2023-05-10 03:03:20.000000 gandai-1.1.2/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5348 2023-05-09 18:21:27.000000 gandai-1.1.2/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.148270 gandai-1.1.2/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1120 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-10 05:24:38.000000 gandai-1.1.2/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-10 05:24:57.152363 gandai-1.1.2/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.2/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.742109 gandai-1.1.3/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.3/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-11 12:12:21.741998 gandai-1.1.3/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.738617 gandai-1.1.3/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-05-11 12:03:39.000000 gandai-1.1.3/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.740565 gandai-1.1.3/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      179 2023-04-07 16:05:45.000000 gandai-1.1.3/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.3/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.3/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-1.1.3/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.3/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3736 2023-05-09 18:28:28.000000 gandai-1.1.3/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5999 2023-05-09 18:36:56.000000 gandai-1.1.3/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16707 2023-05-10 05:05:31.000000 gandai-1.1.3/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.3/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7725 2023-05-09 18:21:29.000000 gandai-1.1.3/gandai/__pycache__/sources.cpython-311.pyc
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.741019 gandai-1.1.3/gandai/adapters/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-1.1.3/gandai/adapters/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.741548 gandai-1.1.3/gandai/adapters/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      188 2023-04-07 16:05:45.000000 gandai-1.1.3/gandai/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1875 2023-04-10 12:31:26.000000 gandai-1.1.3/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      924 2023-04-07 16:06:33.000000 gandai-1.1.3/gandai/adapters/__pycache__/filters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    14686 2023-04-14 19:20:28.000000 gandai-1.1.3/gandai/adapters/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1223 2023-05-05 19:45:58.000000 gandai-1.1.3/gandai/adapters/dealcloud.py
+-rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-1.1.3/gandai/adapters/filters.py
+-rw-r--r--   0 parker     (501) staff       (20)    10094 2023-05-04 03:54:50.000000 gandai-1.1.3/gandai/adapters/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1704 2023-03-30 16:03:27.000000 gandai-1.1.3/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-12 13:11:26.000000 gandai-1.1.3/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     2382 2023-05-11 11:58:58.000000 gandai-1.1.3/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     3089 2023-05-09 18:28:27.000000 gandai-1.1.3/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.741859 gandai-1.1.3/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.3/gandai/migrations/__init__.py
+-rw-r--r--   0 parker     (501) staff       (20)     2536 2023-05-09 21:46:03.000000 gandai-1.1.3/gandai/migrations/create_db.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1764 2023-04-12 12:53:47.000000 gandai-1.1.3/gandai/migrations/dealcloud_to_gandai.py
+-rw-r--r--   0 parker     (501) staff       (20)     2560 2023-05-09 18:36:54.000000 gandai-1.1.3/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)     8110 2023-05-11 12:01:31.000000 gandai-1.1.3/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5348 2023-05-09 18:21:27.000000 gandai-1.1.3/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.739166 gandai-1.1.3/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1133 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-11 12:12:10.000000 gandai-1.1.3/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-11 12:12:21.742137 gandai-1.1.3/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.3/setup.py
```

### Comparing `gandai-1.1.2/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.1.3/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.1.3/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/adapters/__pycache__/filters.cpython-311.pyc` & `gandai-1.1.3/gandai/adapters/__pycache__/filters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/adapters/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.3/gandai/adapters/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/adapters/dealcloud.py` & `gandai-1.1.3/gandai/adapters/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/adapters/filters.py` & `gandai-1.1.3/gandai/adapters/filters.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/adapters/grata.py` & `gandai-1.1.3/gandai/adapters/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/auth.py` & `gandai-1.1.3/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/datastore.py` & `gandai-1.1.3/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/main.py` & `gandai-1.1.3/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/migrations/create_db.sql` & `gandai-1.1.3/gandai/migrations/create_db.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/migrations/dealcloud_to_gandai.py` & `gandai-1.1.3/gandai/migrations/dealcloud_to_gandai.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/models.py` & `gandai-1.1.3/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai/sources.py` & `gandai-1.1.3/gandai/sources.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.2/gandai.egg-info/SOURCES.txt` & `gandai-1.1.3/gandai.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 MANIFEST.in
 pyproject.toml
 setup.py
 gandai/__init__.py
 gandai/auth.py
 gandai/datastore.py
+gandai/db.py
 gandai/main.py
 gandai/models.py
 gandai/query.py
 gandai/sources.py
 gandai.egg-info/PKG-INFO
 gandai.egg-info/SOURCES.txt
 gandai.egg-info/dependency_links.txt
```

