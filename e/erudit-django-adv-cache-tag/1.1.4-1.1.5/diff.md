# Comparing `tmp/erudit-django-adv-cache-tag-1.1.4.tar.gz` & `tmp/erudit-django-adv-cache-tag-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erudit-django-adv-cache-tag-1.1.4.tar", last modified: Thu May 11 19:00:19 2023, max compression
+gzip compressed data, was "erudit-django-adv-cache-tag-1.1.5.tar", last modified: Thu May 11 19:39:39 2023, max compression
```

## Comparing `erudit-django-adv-cache-tag-1.1.4.tar` & `erudit-django-adv-cache-tag-1.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.620540 erudit-django-adv-cache-tag-1.1.4/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)       43 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/AUTHORS
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)     2409 2023-05-11 18:58:22.000000 erudit-django-adv-cache-tag-1.1.4/CHANGELOG.rst
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1086 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/LICENSE
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)       74 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/MANIFEST.in
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)    31573 2023-05-11 19:00:19.620540 erudit-django-adv-cache-tag-1.1.4/PKG-INFO
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)    30035 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/README.rst
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.619540 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)      808 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/__init__.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)      635 2023-05-11 18:29:28.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/compat.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/models.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)    27546 2023-05-11 18:28:41.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tag.py
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.619540 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/templatetags/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/templatetags/__init__.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)      293 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/templatetags/adv_cache.py
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.619540 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)      151 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/__init__.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)      442 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/compat.py
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.619540 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/__init__.py
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.619540 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/__init__.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/models.py
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.620540 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/__init__.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1959 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/adv_cache_test.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)      138 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/other_filters.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)      120 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/other_tags.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1204 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/settings.py
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)    38255 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/tests.py
-drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:00:19.620540 erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)    31573 2023-05-11 19:00:19.000000 erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/PKG-INFO
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1165 2023-05-11 19:00:19.000000 erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/SOURCES.txt
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        1 2023-05-11 19:00:19.000000 erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/dependency_links.txt
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)       14 2023-05-11 19:00:19.000000 erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/requires.txt
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)       14 2023-05-11 19:00:19.000000 erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/top_level.txt
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)        1 2023-05-11 18:35:22.000000 erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/zip-safe
--rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1497 2023-05-11 19:00:19.620540 erudit-django-adv-cache-tag-1.1.4/setup.cfg
--rwxr-xr-x   0 maxocub   (1000) maxocub   (1000)      272 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.4/setup.py
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.653999 erudit-django-adv-cache-tag-1.1.5/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)       43 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/AUTHORS
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)     2517 2023-05-11 19:37:59.000000 erudit-django-adv-cache-tag-1.1.5/CHANGELOG.rst
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1086 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/LICENSE
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)       74 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/MANIFEST.in
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)    31573 2023-05-11 19:39:39.653999 erudit-django-adv-cache-tag-1.1.5/PKG-INFO
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)    30035 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/README.rst
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.651999 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)      815 2023-05-11 19:37:00.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/__init__.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)      635 2023-05-11 18:29:28.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/compat.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/models.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)    27546 2023-05-11 18:28:41.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tag.py
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.652999 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/templatetags/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/templatetags/__init__.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)      293 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/templatetags/adv_cache.py
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.652999 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)      151 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/__init__.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)      442 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/compat.py
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.652999 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/__init__.py
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.652999 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/__init__.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/models.py
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.652999 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/__init__.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1959 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/adv_cache_test.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)      138 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/other_filters.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)      120 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/other_tags.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1204 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/settings.py
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)    38255 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/tests.py
+drwxr-xr-x   0 maxocub   (1000) maxocub   (1000)        0 2023-05-11 19:39:39.652999 erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)    31573 2023-05-11 19:39:39.000000 erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/PKG-INFO
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1165 2023-05-11 19:39:39.000000 erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        1 2023-05-11 19:39:39.000000 erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)       14 2023-05-11 19:39:39.000000 erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/requires.txt
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)       14 2023-05-11 19:39:39.000000 erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/top_level.txt
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)        1 2023-05-11 18:35:22.000000 erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/zip-safe
+-rw-r--r--   0 maxocub   (1000) maxocub   (1000)     1497 2023-05-11 19:39:39.653999 erudit-django-adv-cache-tag-1.1.5/setup.cfg
+-rwxr-xr-x   0 maxocub   (1000) maxocub   (1000)      272 2023-05-11 17:43:03.000000 erudit-django-adv-cache-tag-1.1.5/setup.py
```

### Comparing `erudit-django-adv-cache-tag-1.1.4/CHANGELOG.rst` & `erudit-django-adv-cache-tag-1.1.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Release *v1.1.5* - ``2023-05-11``
+---------------------------------
+* Fix project name in _extract_version
+
 Release *v1.1.4* - ``2023-05-11``
 ---------------------------------
 * Replace Django's urlquote (removed in Django 4.0) by Python's urllib.parse.quote
 * Support other template engines other than Django's
 
 Release *v1.1.3* - ``2020-05-01``
 ---------------------------------
```

### Comparing `erudit-django-adv-cache-tag-1.1.4/LICENSE` & `erudit-django-adv-cache-tag-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/PKG-INFO` & `erudit-django-adv-cache-tag-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erudit-django-adv-cache-tag
-Version: 1.1.4
+Version: 1.1.5
 Summary: An advanced template tag for caching in django: versioning, compress, partial caching, easy inheritance
 Home-page: https://github.com/erudit/django-adv-cache-tag
 Author: Stephane "Twidi" Angel
 Author-email: s.angel@twidi.com
 License: MIT
 Keywords: django,cache,templatetag,template
 Platform: any
```

### Comparing `erudit-django-adv-cache-tag-1.1.4/README.rst` & `erudit-django-adv-cache-tag-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/__init__.py` & `erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,9 +15,9 @@
             path.dirname(__file__), '..', 'setup.cfg')
         )
         version = _conf['metadata']['version']
 
     return version
 
 
-EXACT_VERSION = _extract_version('django_adv_cache_tag')
+EXACT_VERSION = _extract_version('erudit_django_adv_cache_tag')
 VERSION = tuple(int(part) for part in EXACT_VERSION.split('.') if str(part).isnumeric())
```

### Comparing `erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/compat.py` & `erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/compat.py`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tag.py` & `erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tag.py`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/adv_cache_test.py` & `erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/adv_cache_test_app/templatetags/adv_cache_test.py`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/testproject/settings.py` & `erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/testproject/settings.py`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/adv_cache_tag/tests/tests.py` & `erudit-django-adv-cache-tag-1.1.5/adv_cache_tag/tests/tests.py`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/PKG-INFO` & `erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erudit-django-adv-cache-tag
-Version: 1.1.4
+Version: 1.1.5
 Summary: An advanced template tag for caching in django: versioning, compress, partial caching, easy inheritance
 Home-page: https://github.com/erudit/django-adv-cache-tag
 Author: Stephane "Twidi" Angel
 Author-email: s.angel@twidi.com
 License: MIT
 Keywords: django,cache,templatetag,template
 Platform: any
```

### Comparing `erudit-django-adv-cache-tag-1.1.4/erudit_django_adv_cache_tag.egg-info/SOURCES.txt` & `erudit-django-adv-cache-tag-1.1.5/erudit_django_adv_cache_tag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erudit-django-adv-cache-tag-1.1.4/setup.cfg` & `erudit-django-adv-cache-tag-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erudit-django-adv-cache-tag
-version = 1.1.4
+version = 1.1.5
 author = Stephane "Twidi" Angel
 author_email = s.angel@twidi.com
 url = https://github.com/erudit/django-adv-cache-tag
 description = An advanced template tag for caching in django: versioning, compress, partial caching, easy inheritance
 long_description = file: README.rst
 license = MIT
 license_file = LICENSE
```

