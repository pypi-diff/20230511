# Comparing `tmp/simpleparallelize-0.1.1.tar.gz` & `tmp/simpleparallelize-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleparallelize-0.1.1.tar", max compression
+gzip compressed data, was "simpleparallelize-0.1.2.tar", max compression
```

## Comparing `simpleparallelize-0.1.1.tar` & `simpleparallelize-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      377 2023-05-11 02:49:24.017939 simpleparallelize-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 02:41:06.830983 simpleparallelize-0.1.1/simpleparallelize/__init__.py
--rw-r--r--   0        0        0     1253 2023-05-11 02:40:55.170659 simpleparallelize-0.1.1/simpleparallelize/simple.py
--rw-r--r--   0        0        0      653 2023-05-11 02:49:30.278631 simpleparallelize-0.1.1/setup.py
--rw-r--r--   0        0        0      455 2023-05-11 02:49:30.278922 simpleparallelize-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-05-11 03:02:59.224104 simpleparallelize-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 02:41:06.830983 simpleparallelize-0.1.2/simpleparallelize/__init__.py
+-rw-r--r--   0        0        0     1252 2023-05-11 03:02:52.881600 simpleparallelize-0.1.2/simpleparallelize/simple.py
+-rw-r--r--   0        0        0      653 2023-05-11 03:03:01.863458 simpleparallelize-0.1.2/setup.py
+-rw-r--r--   0        0        0      455 2023-05-11 03:03:01.863810 simpleparallelize-0.1.2/PKG-INFO
```

### Comparing `simpleparallelize-0.1.1/simpleparallelize/simple.py` & `simpleparallelize-0.1.2/simpleparallelize/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,9 @@
             update_thread.start()
             partial_func = partial(wrapper_request, func=func)
             responses = pool.map(partial_func, requests)
             update_thread.join()
 
     return responses
 
-def run_requests(requests, func):
+def parallelize(requests, func):
     return mp_progress_bar(requests, func)
```

### Comparing `simpleparallelize-0.1.1/setup.py` & `simpleparallelize-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'simpleparallelize',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A package that makes it easy to parallelize for loops',
     'long_description': None,
     'author': 'ericaleman',
     'author_email': 'mail@ericaleman.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

