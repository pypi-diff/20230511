# Comparing `tmp/ja3requests-0.0.1.tar.gz` & `tmp/ja3requests-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja3requests-0.0.1.tar", last modified: Tue Apr 25 15:19:54 2023, max compression
+gzip compressed data, was "ja3requests-0.0.2.tar", last modified: Thu May 11 09:20:12 2023, max compression
```

## Comparing `ja3requests-0.0.1.tar` & `ja3requests-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:19:54.367676 ja3requests-0.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-24 15:06:22.000000 ja3requests-0.0.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      446 2023-04-25 15:19:54.367676 ja3requests-0.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2023-04-24 15:06:22.000000 ja3requests-0.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:19:54.363676 ja3requests-0.0.1/ja3requests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:15:17.000000 ja3requests-0.0.1/ja3requests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-04-25 15:15:17.000000 ja3requests-0.0.1/ja3requests/__version__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      665 2023-04-25 15:15:17.000000 ja3requests-0.0.1/ja3requests/const.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-04-25 15:15:17.000000 ja3requests-0.0.1/ja3requests/sessions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2118 2023-04-25 15:15:17.000000 ja3requests-0.0.1/ja3requests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:19:54.363676 ja3requests-0.0.1/ja3requests.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      446 2023-04-25 15:19:54.000000 ja3requests-0.0.1/ja3requests.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      351 2023-04-25 15:19:54.000000 ja3requests-0.0.1/ja3requests.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 15:19:54.000000 ja3requests-0.0.1/ja3requests.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 14:53:10.000000 ja3requests-0.0.1/ja3requests.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-04-25 15:19:54.000000 ja3requests-0.0.1/ja3requests.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      640 2023-04-25 15:15:17.000000 ja3requests-0.0.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 15:19:54.367676 ja3requests-0.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1890 2023-04-25 15:15:17.000000 ja3requests-0.0.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 15:19:54.363676 ja3requests-0.0.1/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2023-04-25 15:15:17.000000 ja3requests-0.0.1/test/test_utils.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.957403 ja3requests-0.0.2/
+-rw-r--r--   0 pledgebox   (501) staff       (20)    11357 2023-04-25 06:02:38.000000 ja3requests-0.0.2/LICENSE
+-rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-11 09:20:12.957089 ja3requests-0.0.2/PKG-INFO
+-rw-r--r--   0 pledgebox   (501) staff       (20)       75 2023-04-25 06:02:38.000000 ja3requests-0.0.2/README.md
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.952049 ja3requests-0.0.2/ja3requests/
+-rw-r--r--   0 pledgebox   (501) staff       (20)        0 2023-04-26 10:28:27.000000 ja3requests-0.0.2/ja3requests/__init__.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      395 2023-05-11 09:18:32.000000 ja3requests-0.0.2/ja3requests/__version__.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     3298 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/connections.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      665 2023-04-26 10:28:27.000000 ja3requests-0.0.2/ja3requests/const.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1184 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/exceptions.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     5848 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/request.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     4537 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/sessions.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     2118 2023-04-26 10:28:27.000000 ja3requests-0.0.2/ja3requests/utils.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.954583 ja3requests-0.0.2/ja3requests.egg-info/
+-rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/PKG-INFO
+-rw-r--r--   0 pledgebox   (501) staff       (20)      475 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/SOURCES.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/dependency_links.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/not-zip-safe
+-rw-r--r--   0 pledgebox   (501) staff       (20)       12 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/top_level.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)      640 2023-04-26 10:28:27.000000 ja3requests-0.0.2/pyproject.toml
+-rw-r--r--   0 pledgebox   (501) staff       (20)       38 2023-05-11 09:20:12.957490 ja3requests-0.0.2/setup.cfg
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1890 2023-04-26 10:28:27.000000 ja3requests-0.0.2/setup.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.956283 ja3requests-0.0.2/test/
+-rw-r--r--   0 pledgebox   (501) staff       (20)      431 2023-05-11 09:18:14.000000 ja3requests-0.0.2/test/test_ready_request.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      248 2023-05-11 09:18:14.000000 ja3requests-0.0.2/test/test_session.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      244 2023-04-26 10:28:27.000000 ja3requests-0.0.2/test/test_utils.py
```

### Comparing `ja3requests-0.0.1/LICENSE` & `ja3requests-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.1/ja3requests/const.py` & `ja3requests-0.0.2/ja3requests/const.py`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.1/ja3requests/utils.py` & `ja3requests-0.0.2/ja3requests/utils.py`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.1/pyproject.toml` & `ja3requests-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.1/setup.py` & `ja3requests-0.0.2/setup.py`

 * *Files identical despite different names*

