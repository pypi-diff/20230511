# Comparing `tmp/smartjs-0.1.5.tar.gz` & `tmp/smartjs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.1.5.tar", max compression
+gzip compressed data, was "smartjs-0.1.6.tar", max compression
```

## Comparing `smartjs-0.1.5.tar` & `smartjs-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      376 2023-05-11 12:30:37.914421 smartjs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      243 2023-05-11 01:47:48.346629 smartjs-0.1.5/smartjs/__init__.py
--rw-r--r--   0        0        0    16804 2023-05-11 12:30:37.909091 smartjs-0.1.5/smartjs/base.py
--rw-r--r--   0        0        0     1277 2023-05-11 05:35:54.145444 smartjs-0.1.5/smartjs/collection.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.5/smartjs/constants.py
--rw-r--r--   0        0        0     5050 2023-05-11 12:30:37.912377 smartjs-0.1.5/smartjs/elements.py
--rw-r--r--   0        0        0     6296 2023-05-11 01:14:16.811102 smartjs-0.1.5/smartjs/functions.py
--rw-r--r--   0        0        0    11508 2023-05-11 12:30:37.905091 smartjs-0.1.5/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.5/smartjs/page.py
--rw-r--r--   0        0        0     1782 2023-05-11 05:41:46.920516 smartjs-0.1.5/smartjs/path.py
--rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.5/smartjs/style.py
--rw-r--r--   0        0        0      658 2023-05-11 12:30:50.330078 smartjs-0.1.5/setup.py
--rw-r--r--   0        0        0      407 2023-05-11 12:30:50.330279 smartjs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      376 2023-05-11 12:49:03.519465 smartjs-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-05-11 01:47:48.346629 smartjs-0.1.6/smartjs/__init__.py
+-rw-r--r--   0        0        0    16804 2023-05-11 12:30:37.909091 smartjs-0.1.6/smartjs/base.py
+-rw-r--r--   0        0        0     1277 2023-05-11 05:35:54.145444 smartjs-0.1.6/smartjs/collection.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.6/smartjs/constants.py
+-rw-r--r--   0        0        0     5139 2023-05-11 12:48:44.028584 smartjs-0.1.6/smartjs/elements.py
+-rw-r--r--   0        0        0     6296 2023-05-11 01:14:16.811102 smartjs-0.1.6/smartjs/functions.py
+-rw-r--r--   0        0        0    11508 2023-05-11 12:30:37.905091 smartjs-0.1.6/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.6/smartjs/page.py
+-rw-r--r--   0        0        0     1782 2023-05-11 05:41:46.920516 smartjs-0.1.6/smartjs/path.py
+-rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.6/smartjs/style.py
+-rw-r--r--   0        0        0      658 2023-05-11 12:49:11.241060 smartjs-0.1.6/setup.py
+-rw-r--r--   0        0        0      407 2023-05-11 12:49:11.241469 smartjs-0.1.6/PKG-INFO
```

### Comparing `smartjs-0.1.5/smartjs/base.py` & `smartjs-0.1.6/smartjs/base.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/smartjs/collection.py` & `smartjs-0.1.6/smartjs/collection.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/smartjs/constants.py` & `smartjs-0.1.6/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/smartjs/elements.py` & `smartjs-0.1.6/smartjs/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,20 +267,20 @@
 
 
 class Meta(BaseElement):
 	pass
 
 
 class Body(BaseUniqueElement):
-	def __init__(self, nav: Nav, main: Main, footer: Footer, scripts: list[Script] = None, **kwargs):
-		self.nav = nav
-		self.main = main
-		self.footer = footer
-		super().__init__(nav, main, footer, *parse_list(scripts), **kwargs)
-
+	def __init__(self, *args, **kwargs):
+	# 	self.nav = list_of_type(args, Nav)
+	# 	self.main = list_of_type(args, Main)
+	# 	self.footer = list_of_type(args, Footer)
+	# 	args = list_filtered(parse_list(args), lambda x: x if not isinstance(x (Nav, Main, Footer)) else None)
+		super().__init__(Id('body'), *args, **kwargs)
 
 
 class InstanceOption(BaseElement):
 	TAG = Tag('option')
 	def __init__(self, instance, *args, **kwargs):
 		self.instance = instance
 		super().__init__(*args, **kwargs)
```

### Comparing `smartjs-0.1.5/smartjs/functions.py` & `smartjs-0.1.6/smartjs/functions.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/smartjs/javascript.py` & `smartjs-0.1.6/smartjs/javascript.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/smartjs/page.py` & `smartjs-0.1.6/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/smartjs/path.py` & `smartjs-0.1.6/smartjs/path.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/smartjs/style.py` & `smartjs-0.1.6/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.5/setup.py` & `smartjs-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Project for creation of javascript, html and style elements for web pages.',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

