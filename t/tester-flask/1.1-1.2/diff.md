# Comparing `tmp/tester_flask-1.1.tar.gz` & `tmp/tester_flask-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tester_flask-1.1.tar", last modified: Mon Jun  3 17:11:11 2019, max compression
+gzip compressed data, was "tester_flask-1.2.tar", last modified: Thu May 11 13:59:00 2023, max compression
```

## Comparing `tester_flask-1.1.tar` & `tester_flask-1.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2019-06-03 17:11:11.000000 tester_flask-1.1/
--rw-rw-rw-   0        0        0      719 2019-06-03 17:11:11.000000 tester_flask-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2019-06-03 17:08:43.000000 tester_flask-1.1/README.md
--rw-rw-rw-   0        0        0       42 2019-06-03 17:11:11.000000 tester_flask-1.1/setup.cfg
--rw-rw-rw-   0        0        0      859 2019-06-03 17:08:43.000000 tester_flask-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2019-06-03 17:11:11.000000 tester_flask-1.1/tester_flask/
--rw-rw-rw-   0        0        0     3602 2019-06-03 17:08:43.000000 tester_flask-1.1/tester_flask/__init__.py
-drwxrwxrwx   0        0        0        0 2019-06-03 17:11:11.000000 tester_flask-1.1/tester_flask.egg-info/
--rw-rw-rw-   0        0        0        1 2019-06-03 17:11:11.000000 tester_flask-1.1/tester_flask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      719 2019-06-03 17:11:11.000000 tester_flask-1.1/tester_flask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2019-06-03 17:11:11.000000 tester_flask-1.1/tester_flask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2019-06-03 17:11:11.000000 tester_flask-1.1/tester_flask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 13:59:00.556324 tester_flask-1.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-11 18:26:01.000000 tester_flask-1.2/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-04-12 05:46:44.000000 tester_flask-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2858 2023-05-11 13:59:00.556826 tester_flask-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-05-11 13:52:34.000000 tester_flask-1.2/README.md
+-rw-rw-rw-   0        0        0      110 2023-02-11 14:05:41.000000 tester_flask-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      608 2023-05-11 13:59:00.558827 tester_flask-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 13:59:00.527747 tester_flask-1.2/tester_flask/
+-rw-rw-rw-   0        0        0     3418 2023-05-11 13:47:30.000000 tester_flask-1.2/tester_flask/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:59:00.541757 tester_flask-1.2/tester_flask.egg-info/
+-rw-rw-rw-   0        0        0     2858 2023-05-11 13:59:00.000000 tester_flask-1.2/tester_flask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-11 13:59:00.000000 tester_flask-1.2/tester_flask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 13:59:00.000000 tester_flask-1.2/tester_flask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-11 13:59:00.000000 tester_flask-1.2/tester_flask.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tester_flask-1.1/tester_flask/__init__.py` & `tester_flask-1.2/tester_flask/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,91 @@
-"""
+"""Test helper for Flask app.
+
 http://flask.pocoo.org/docs/1.0/testing/
 https://cloud.google.com/appengine/docs/standard/python/getting-started/python-standard-env
 """
 import unittest
 try:  # pragma: no cover
     from urllib import urlencode
     from urlparse import urlparse
 except ImportError:  # pragma: no cover
     from urllib.parse import urlparse, urlencode  # pylint: disable=ungrouped-imports
 
 
 class RequestFactory:  # pylint: disable=too-few-public-methods
-    """
-    requests generator
-    """
+    """Generator of the requests."""
+
     def __init__(self, app):
+        """Save Flask app instance."""
         self.app = app
 
     def post(self, url, data='', content_type='application/octet-stream'):
-        """
-        post requests tests
-        """
+        """Post requests tests."""
         return self.app.test_request_context(url, data=data, method='POST', content_type=content_type)
 
 
 class TestFlask(unittest.TestCase):
-    """
-    Flask apps tester
-    """
-    def setUp(self, app):  # pylint: disable=arguments-differ
-        unittest.TestCase.setUp(self)
+    """Flask apps tester."""
+
+    app = None
+    client = None
+    factory = None
+
+    def set_up(self, app):
+        """Set defaults for Flask testing."""
         self.app = app
         self.app.config['TESTING'] = True
         self.client = self.app.test_client()
         self.factory = RequestFactory(self.app)
 
-    def tearDown(self):
-        unittest.TestCase.tearDown(self)
-
     def get_url(self, view_name, **kwargs):
-        """
-        generate url for view in app test context
-        """
+        """Generate url for view in app test context."""
         with self.app.test_request_context():
             from flask import url_for
             url = url_for(view_name, **kwargs)
 
         return url
 
     def guest_view(self, url, return_code=200, follow_redirects=False):
-        """
-        generic get request
-        """
+        """Make generic get request."""
         response = self.client.get(url, follow_redirects=follow_redirects)
 
-        self.assertEqual(
-          response.status_code,
-          return_code,
-          "guest_view {}: {} -> {}".format(return_code, url, response.status_code)
+        assert response.status_code == return_code, "guest_view {}: {} -> {}".format(
+          return_code, url, response.status_code
         )
         return response
 
     def simple_view(self, view_name, return_code=200, follow=False, get_param=None):
-        """
-        simple get request
-        """
+        """Make simple get request."""
         url = self.get_url(view_name)
         if get_param:
             url = url + "?" + urlencode(get_param)
         return self.guest_view(url, return_code=return_code, follow_redirects=follow)
 
     def param_view(
       self, view_name, params, return_code=200, follow=False, get_param=None
-    ):  # pylint: disable=too-many-arguments
-        """
-        get request with parameters
-        """
+    ):
+        """Get request with parameters."""
         url = self.get_url(view_name, **params)
         if get_param:
             url = url + "?" + urlencode(get_param)
         return self.guest_view(url, return_code=return_code, follow_redirects=follow)
 
     def simple_post(self, view_name, post_dict, follow=True, content_type=None):
-        """
-        simple post request
-        """
+        """Make simple post request."""
         url = self.get_url(view_name)
         return self.client.post(url, data=post_dict, follow_redirects=follow, content_type=content_type)
 
     def param_post(
       self, view_name, params, post_dict, follow=True, get_param=None, content_type=None
     ):  # pylint: disable=too-many-arguments
-        """
-        post request with parameters
-        """
+        """Post request with parameters."""
         url = self.get_url(view_name, **params)
         if get_param:
             url = url + "?" + urlencode(get_param)
         return self.client.post(url, data=post_dict, follow_redirects=follow, content_type=content_type)
 
-    def final_url(self, response):
-        """
-        return final url after redirect
-        """
-        self.assertEqual(response.status_code, 302)
+    @staticmethod
+    def final_url(response):
+        """Return final url after redirect."""
+        assert response.status_code == 302
         return urlparse(response.location).path
```

