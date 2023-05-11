# Comparing `tmp/therapi-0.0.3.tar.gz` & `tmp/therapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therapi-0.0.3.tar", max compression
+gzip compressed data, was "therapi-0.0.4.tar", max compression
```

## Comparing `therapi-0.0.3.tar` & `therapi-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-01-13 19:00:07.545628 therapi-0.0.3/LICENSE
--rw-r--r--   0        0        0      840 2023-02-27 19:39:42.386036 therapi-0.0.3/README.md
--rw-r--r--   0        0        0      418 2023-02-27 19:40:09.730087 therapi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      778 2023-02-27 19:29:25.868946 therapi-0.0.3/therapi/__init__.py
--rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 therapi-0.0.3/setup.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 therapi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-01-13 19:00:07.545628 therapi-0.0.4/LICENSE
+-rw-r--r--   0        0        0      840 2023-02-27 19:39:42.386036 therapi-0.0.4/README.md
+-rw-r--r--   0        0        0      418 2023-05-11 19:59:48.069059 therapi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2431 2023-05-11 19:56:17.028787 therapi-0.0.4/therapi/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-09 19:24:06.394049 therapi-0.0.4/therapi/authentication.py
+-rw-r--r--   0        0        0       47 2023-05-09 19:24:06.382049 therapi-0.0.4/therapi/exceptions.py
+-rw-r--r--   0        0        0     1205 2023-05-11 19:32:05.813097 therapi-0.0.4/therapi/thingipy.py
+-rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 therapi-0.0.4/setup.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 therapi-0.0.4/PKG-INFO
```

### Comparing `therapi-0.0.3/LICENSE` & `therapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `therapi-0.0.3/README.md` & `therapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `therapi-0.0.3/setup.py` & `therapi-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'therapi',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Therapy to ease the pain of writing boilerplate JSON API consumers.',
     'long_description': '# python-therapi\nTherapy to ease the pain of writing boilerplate JSON API consumers.\n\n---\n\nTired of writing the same code to consume JSON APIs, over and over? Let\'s solve that!\n\n## Query a basic, public JSON API\n\nTo query any basic, public JSON API, we create our consumer class and inherit from `BaseAPIConsumer`, as follows:\n\n```python\nfrom therapi import BaseAPIConsumer\n\nclass MyAPIConsumer(BaseAPIConsumer):\n    base_url = "https://www.an-awesome-service.com/api"\n```\n\nNow we can use this class to make API calls to different endpoints, as follows:\n\n```python\nconsumer = MyAPIConsumer()\nresult = consumer.json_request(method="get", path="items", params={"id": 123})\nprint(result)\n```\n\nWe would see, for example, this response:\n\n```json\n{\n  "data": [\n    {"name": "Laptop", "price": 239},\n    {"name": "Printer", "price": 99}\n  ]\n}\n```\n',
     'author': 'Helmut Irle',
     'author_email': 'me@helmut.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `therapi-0.0.3/PKG-INFO` & `therapi-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: therapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Therapy to ease the pain of writing boilerplate JSON API consumers.
 License: MIT
 Author: Helmut Irle
 Author-email: me@helmut.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

