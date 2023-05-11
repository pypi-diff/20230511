# Comparing `tmp/smartjs-0.1.2.tar.gz` & `tmp/smartjs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.1.2.tar", max compression
+gzip compressed data, was "smartjs-0.1.3.tar", max compression
```

## Comparing `smartjs-0.1.2.tar` & `smartjs-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      376 2023-05-11 05:41:55.559326 smartjs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      243 2023-05-11 01:47:48.346629 smartjs-0.1.2/smartjs/__init__.py
--rw-r--r--   0        0        0    16232 2023-05-11 05:02:23.341856 smartjs-0.1.2/smartjs/base.py
--rw-r--r--   0        0        0     1277 2023-05-11 05:35:54.145444 smartjs-0.1.2/smartjs/collection.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.2/smartjs/constants.py
--rw-r--r--   0        0        0     4970 2023-05-10 13:03:07.134383 smartjs-0.1.2/smartjs/elements.py
--rw-r--r--   0        0        0     6296 2023-05-11 01:14:16.811102 smartjs-0.1.2/smartjs/functions.py
--rw-r--r--   0        0        0    11908 2023-05-10 11:42:41.551886 smartjs-0.1.2/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.2/smartjs/page.py
--rw-r--r--   0        0        0     1782 2023-05-11 05:41:46.920516 smartjs-0.1.2/smartjs/path.py
--rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.2/smartjs/style.py
--rw-r--r--   0        0        0      658 2023-05-11 05:42:09.593527 smartjs-0.1.2/setup.py
--rw-r--r--   0        0        0      407 2023-05-11 05:42:09.593741 smartjs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      376 2023-05-11 06:31:31.467987 smartjs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-05-11 01:47:48.346629 smartjs-0.1.3/smartjs/__init__.py
+-rw-r--r--   0        0        0    16232 2023-05-11 05:02:23.341856 smartjs-0.1.3/smartjs/base.py
+-rw-r--r--   0        0        0     1277 2023-05-11 05:35:54.145444 smartjs-0.1.3/smartjs/collection.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.3/smartjs/constants.py
+-rw-r--r--   0        0        0     5057 2023-05-11 06:31:31.464870 smartjs-0.1.3/smartjs/elements.py
+-rw-r--r--   0        0        0     6296 2023-05-11 01:14:16.811102 smartjs-0.1.3/smartjs/functions.py
+-rw-r--r--   0        0        0    11908 2023-05-10 11:42:41.551886 smartjs-0.1.3/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.3/smartjs/page.py
+-rw-r--r--   0        0        0     1782 2023-05-11 05:41:46.920516 smartjs-0.1.3/smartjs/path.py
+-rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.3/smartjs/style.py
+-rw-r--r--   0        0        0      658 2023-05-11 06:31:41.861688 smartjs-0.1.3/setup.py
+-rw-r--r--   0        0        0      407 2023-05-11 06:31:41.862117 smartjs-0.1.3/PKG-INFO
```

### Comparing `smartjs-0.1.2/smartjs/base.py` & `smartjs-0.1.3/smartjs/base.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/smartjs/collection.py` & `smartjs-0.1.3/smartjs/collection.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/smartjs/constants.py` & `smartjs-0.1.3/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/smartjs/elements.py` & `smartjs-0.1.3/smartjs/elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 		'H2',
 		'H1',
 		'H3',
 		'H4',
 		'H5',
 		'H6',
 		'BR',
-		'HR'
+		'HR',
+		'Title'
 ]
 
 from typing import Collection
 from smartjs.base import *
 from smartjs.functions import *
 from smartjs.javascript import *
 
@@ -170,16 +171,15 @@
 	TAG = Tag('a')
 	KLASS = 'nav-link'
 	
 
 class Input(BaseElement):
 	def __init__(self, *args, _type: str = 'text', **kwargs):
 		self.type = InputType(_type)
-		super().__init__(*args, **kwargs)
-		self.dict_kwargs['type'] = self.type.value
+		super().__init__(*args, Kwarg('type', self.type.value), **kwargs)
 		
 		
 class Textarea(BaseElement):
 	pass
 
 
 class Select(BaseElement):
@@ -243,18 +243,19 @@
 	def __init__(self, value: str):
 		super().__init__(elements=[value])
 
 
 class Head(BaseElement):
 	def __init__(self, title: str, *args, **kwargs):
 		self.head_title = title
-		super().__init__(*args, **kwargs)
+		elements = SmartList(*self.get_elements, kwargs.get('elements', None))
+		super().__init__(*args, elements=[*elements], **kwargs)
 	
 	@property
-	def post_init_elements(self):
+	def get_elements(self):
 		return [
 				Meta(charset='utf-8'),
 				Meta(name="viewport", content="width=device-width, initial-scale=1"),
 				Title(self.head_title),
 				Link(
 						href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css",
 						rel="stylesheet",
```

### Comparing `smartjs-0.1.2/smartjs/functions.py` & `smartjs-0.1.3/smartjs/functions.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/smartjs/javascript.py` & `smartjs-0.1.3/smartjs/javascript.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/smartjs/page.py` & `smartjs-0.1.3/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/smartjs/path.py` & `smartjs-0.1.3/smartjs/path.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/smartjs/style.py` & `smartjs-0.1.3/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.2/setup.py` & `smartjs-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Project for creation of javascript, html and style elements for web pages.',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

