# Comparing `tmp/simpleparallelize-0.1.3.tar.gz` & `tmp/simpleparallelize-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleparallelize-0.1.3.tar", max compression
+gzip compressed data, was "simpleparallelize-0.1.4.tar", max compression
```

## Comparing `simpleparallelize-0.1.3.tar` & `simpleparallelize-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      382 2023-05-11 03:09:44.498306 simpleparallelize-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 02:41:06.830983 simpleparallelize-0.1.3/simpleparallelize/__init__.py
--rw-r--r--   0        0        0     1252 2023-05-11 03:02:52.881600 simpleparallelize-0.1.3/simpleparallelize/simple.py
--rw-r--r--   0        0        0      658 2023-05-11 03:10:08.952422 simpleparallelize-0.1.3/setup.py
--rw-r--r--   0        0        0      460 2023-05-11 03:10:08.952654 simpleparallelize-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      382 2023-05-11 03:11:16.657732 simpleparallelize-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 02:41:06.830983 simpleparallelize-0.1.4/simpleparallelize/__init__.py
+-rw-r--r--   0        0        0     1251 2023-05-11 03:11:06.963342 simpleparallelize-0.1.4/simpleparallelize/simple.py
+-rw-r--r--   0        0        0      658 2023-05-11 03:11:20.179528 simpleparallelize-0.1.4/setup.py
+-rw-r--r--   0        0        0      460 2023-05-11 03:11:20.179756 simpleparallelize-0.1.4/PKG-INFO
```

### Comparing `simpleparallelize-0.1.3/simpleparallelize/simple.py` & `simpleparallelize-0.1.4/simpleparallelize/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from tqdm import tqdm
+
 import multiprocessing as mp
 import threading
 from functools import partial
 
 def init_progress_bar(shared_value):
     global shared_progress
     shared_progress = shared_value
 
-
 def update_progress_bar(pbar, shared_progress):
     while not pbar.n >= pbar.total:
         with shared_progress.get_lock():
             current_progress = shared_progress.value
             pbar.update(current_progress - pbar.n)
 
-
 def wrapper_request(request, func):
     response = func(request)
     with shared_progress.get_lock():
         shared_progress.value += 1
     return response
 
 def mp_progress_bar(requests, func):
```

### Comparing `simpleparallelize-0.1.3/setup.py` & `simpleparallelize-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'simpleparallelize',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Easy processsing pool setup with a spark-like progress bar',
     'long_description': None,
     'author': 'ericaleman',
     'author_email': 'mail@ericaleman.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

