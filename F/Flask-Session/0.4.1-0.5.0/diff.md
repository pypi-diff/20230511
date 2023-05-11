# Comparing `tmp/Flask-Session-0.4.1.tar.gz` & `tmp/Flask-Session-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Session-0.4.1.tar", last modified: Sun Apr 30 05:18:57 2023, max compression
+gzip compressed data, was "Flask-Session-0.5.0.tar", last modified: Thu May 11 18:32:12 2023, max compression
```

## Comparing `Flask-Session-0.4.1.tar` & `Flask-Session-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/CHANGES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/Flask_Session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-30 05:18:57.000000 Flask-Session-0.4.1/Flask_Session.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/_static/flask-session.png
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/flask_session/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/flask_session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/flask_session/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-30 05:18:57.243419 Flask-Session-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-30 05:18:31.000000 Flask-Session-0.4.1/test_session.py
+-rw-r--r--   0        0        0     1593 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/CHANGES.rst
+-rw-r--r--   0        0        0     1495 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/LICENSE.rst
+-rw-r--r--   0        0        0      133 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/README.rst
+-rw-r--r--   0        0        0      634 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0      531 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/api.rst
+-rw-r--r--   0        0        0       45 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/changes.rst
+-rw-r--r--   0        0        0      676 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0     5541 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/config.rst
+-rw-r--r--   0        0        0      459 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0     1610 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/interfaces.rst
+-rw-r--r--   0        0        0       71 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/license.rst
+-rw-r--r--   0        0        0      893 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/docs/quickstart.rst
+-rw-r--r--   0        0        0     1498 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        7 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/requirements/docs.in
+-rw-r--r--   0        0        0      962 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/requirements/docs.txt
+-rw-r--r--   0        0        0     4008 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/src/flask_session/__init__.py
+-rw-r--r--   0        0        0    22354 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/src/flask_session/sessions.py
+-rw-r--r--   0        0        0     6365 2023-05-11 18:32:12.000000 Flask-Session-0.5.0/test_session.py
+-rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 Flask-Session-0.5.0/PKG-INFO
```

### Comparing `Flask-Session-0.4.1/LICENSE` & `Flask-Session-0.5.0/LICENSE.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-Copyright (c) 2014 by Shipeng Feng.
-
-Some rights reserved.
+Copyright 2014 Pallets Community Ecosystem
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
-* Redistributions of source code must retain the above copyright
-  notice, this list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above
-  copyright notice, this list of conditions and the following
-  disclaimer in the documentation and/or other materials provided
-  with the distribution.
+1.  Redistributions of source code must retain the above copyright
+    notice, this list of conditions and the following disclaimer.
 
-* The names of the contributors may not be used to endorse or
-  promote products derived from this software without specific
-  prior written permission.
+2.  Redistributions in binary form must reproduce the above copyright
+    notice, this list of conditions and the following disclaimer in the
+    documentation and/or other materials provided with the distribution.
+
+3.  Neither the name of the copyright holder nor the names of its
+    contributors may be used to endorse or promote products derived from
+    this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
+TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
+NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `Flask-Session-0.4.1/flask_session/__init__.py` & `Flask-Session-0.5.0/src/flask_session/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-# -*- coding: utf-8 -*-
-"""
-    flask_session
-    ~~~~~~~~~~~~~
-
-    Adds server session support to your application.
-
-    :copyright: (c) 2014 by Shipeng Feng.
-    :license: BSD, see LICENSE for more details.
-"""
-
-__version__ = '0.4.1'
-
 import os
 
 from .sessions import NullSessionInterface, RedisSessionInterface, \
     MemcachedSessionInterface, FileSystemSessionInterface, \
     MongoDBSessionInterface, SqlAlchemySessionInterface
 
+__version__ = '0.5.0'
+
 
 class Session(object):
     """This class is used to add Server-side Session to one or more Flask
     applications.
 
     There are two usage modes.  One is initialize the instance with a very
     specific Flask application::
```

### Comparing `Flask-Session-0.4.1/flask_session/sessions.py` & `Flask-Session-0.5.0/src/flask_session/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-    flask_session.sessions
-    ~~~~~~~~~~~~~~~~~~~~~~
-
-    Server-side Sessions and SessionInterfaces.
-
-    :copyright: (c) 2014 by Shipeng Feng.
-    :license: BSD, see LICENSE for more details.
-"""
 import sys
 import time
 from datetime import datetime
 from uuid import uuid4
 try:
     import cPickle as pickle
 except ImportError:
@@ -109,15 +99,15 @@
         self.redis = redis
         self.key_prefix = key_prefix
         self.use_signer = use_signer
         self.permanent = permanent
         self.has_same_site_capability = hasattr(self, "get_cookie_samesite")
 
     def open_session(self, app, request):
-        sid = request.cookies.get(app.session_cookie_name)
+        sid = request.cookies.get(app.config["SESSION_COOKIE_NAME"])
         if not sid:
             sid = self._generate_sid()
             return self.session_class(sid=sid, permanent=self.permanent)
         if self.use_signer:
             signer = self._get_signer(app)
             if signer is None:
                 return None
@@ -141,15 +131,15 @@
 
     def save_session(self, app, session, response):
         domain = self.get_cookie_domain(app)
         path = self.get_cookie_path(app)
         if not session:
             if session.modified:
                 self.redis.delete(self.key_prefix + session.sid)
-                response.delete_cookie(app.session_cookie_name,
+                response.delete_cookie(app.config["SESSION_COOKIE_NAME"],
                                        domain=domain, path=path)
             return
 
         # Modification case.  There are upsides and downsides to
         # emitting a set-cookie header each request.  The behavior
         # is controlled by the :meth:`should_set_cookie` method
         # which performs a quick check to figure out if the cookie
@@ -167,15 +157,15 @@
         val = self.serializer.dumps(dict(session))
         self.redis.setex(name=self.key_prefix + session.sid, value=val,
                          time=total_seconds(app.permanent_session_lifetime))
         if self.use_signer:
             session_id = self._get_signer(app).sign(want_bytes(session.sid))
         else:
             session_id = session.sid
-        response.set_cookie(app.session_cookie_name, session_id,
+        response.set_cookie(app.config["SESSION_COOKIE_NAME"], session_id,
                             expires=expires, httponly=httponly,
                             domain=domain, path=path, secure=secure,
                             **conditional_cookie_kwargs)
 
 
 class MemcachedSessionInterface(SessionInterface):
     """A Session interface that uses memcached as backend.
@@ -231,15 +221,15 @@
             # said date. This is a simple (but obscure) mechanic."
             #
             # This means that we have to switch to absolute timestamps.
             timeout += int(time.time())
         return timeout
 
     def open_session(self, app, request):
-        sid = request.cookies.get(app.session_cookie_name)
+        sid = request.cookies.get(app.config["SESSION_COOKIE_NAME"])
         if not sid:
             sid = self._generate_sid()
             return self.session_class(sid=sid, permanent=self.permanent)
         if self.use_signer:
             signer = self._get_signer(app)
             if signer is None:
                 return None
@@ -269,15 +259,15 @@
         path = self.get_cookie_path(app)
         full_session_key = self.key_prefix + session.sid
         if PY2 and isinstance(full_session_key, unicode):
             full_session_key = full_session_key.encode('utf-8')
         if not session:
             if session.modified:
                 self.client.delete(full_session_key)
-                response.delete_cookie(app.session_cookie_name,
+                response.delete_cookie(app.config["SESSION_COOKIE_NAME"],
                                        domain=domain, path=path)
             return
 
         conditional_cookie_kwargs = {}
         httponly = self.get_cookie_httponly(app)
         secure = self.get_cookie_secure(app)
         if self.has_same_site_capability:
@@ -289,15 +279,15 @@
             val = self.serializer.dumps(dict(session))
         self.client.set(full_session_key, val, self._get_memcache_timeout(
                         total_seconds(app.permanent_session_lifetime)))
         if self.use_signer:
             session_id = self._get_signer(app).sign(want_bytes(session.sid))
         else:
             session_id = session.sid
-        response.set_cookie(app.session_cookie_name, session_id,
+        response.set_cookie(app.config["SESSION_COOKIE_NAME"], session_id,
                             expires=expires, httponly=httponly,
                             domain=domain, path=path, secure=secure,
                             **conditional_cookie_kwargs)
 
 
 class FileSystemSessionInterface(SessionInterface):
     """Uses the :class:`cachelib.file.FileSystemCache` as a session backend.
@@ -322,15 +312,15 @@
         self.cache = FileSystemCache(cache_dir, threshold=threshold, mode=mode)
         self.key_prefix = key_prefix
         self.use_signer = use_signer
         self.permanent = permanent
         self.has_same_site_capability = hasattr(self, "get_cookie_samesite")
 
     def open_session(self, app, request):
-        sid = request.cookies.get(app.session_cookie_name)
+        sid = request.cookies.get(app.config["SESSION_COOKIE_NAME"])
         if not sid:
             sid = self._generate_sid()
             return self.session_class(sid=sid, permanent=self.permanent)
         if self.use_signer:
             signer = self._get_signer(app)
             if signer is None:
                 return None
@@ -348,15 +338,15 @@
 
     def save_session(self, app, session, response):
         domain = self.get_cookie_domain(app)
         path = self.get_cookie_path(app)
         if not session:
             if session.modified:
                 self.cache.delete(self.key_prefix + session.sid)
-                response.delete_cookie(app.session_cookie_name,
+                response.delete_cookie(app.config["SESSION_COOKIE_NAME"],
                                        domain=domain, path=path)
             return
 
         conditional_cookie_kwargs = {}
         httponly = self.get_cookie_httponly(app)
         secure = self.get_cookie_secure(app)
         if self.has_same_site_capability:
@@ -365,15 +355,15 @@
         data = dict(session)
         self.cache.set(self.key_prefix + session.sid, data,
                        total_seconds(app.permanent_session_lifetime))
         if self.use_signer:
             session_id = self._get_signer(app).sign(want_bytes(session.sid))
         else:
             session_id = session.sid
-        response.set_cookie(app.session_cookie_name, session_id,
+        response.set_cookie(app.config["SESSION_COOKIE_NAME"], session_id,
                             expires=expires, httponly=httponly,
                             domain=domain, path=path, secure=secure,
                             **conditional_cookie_kwargs)
 
 
 class MongoDBSessionInterface(SessionInterface):
     """A Session interface that uses mongodb as backend.
@@ -401,15 +391,15 @@
         self.store = client[db][collection]
         self.key_prefix = key_prefix
         self.use_signer = use_signer
         self.permanent = permanent
         self.has_same_site_capability = hasattr(self, "get_cookie_samesite")
 
     def open_session(self, app, request):
-        sid = request.cookies.get(app.session_cookie_name)
+        sid = request.cookies.get(app.config["SESSION_COOKIE_NAME"])
         if not sid:
             sid = self._generate_sid()
             return self.session_class(sid=sid, permanent=self.permanent)
         if self.use_signer:
             signer = self._get_signer(app)
             if signer is None:
                 return None
@@ -438,15 +428,15 @@
     def save_session(self, app, session, response):
         domain = self.get_cookie_domain(app)
         path = self.get_cookie_path(app)
         store_id = self.key_prefix + session.sid
         if not session:
             if session.modified:
                 self.store.remove({'id': store_id})
-                response.delete_cookie(app.session_cookie_name,
+                response.delete_cookie(app.config["SESSION_COOKIE_NAME"],
                                        domain=domain, path=path)
             return
 
         conditional_cookie_kwargs = {}
         httponly = self.get_cookie_httponly(app)
         secure = self.get_cookie_secure(app)
         if self.has_same_site_capability:
@@ -457,15 +447,15 @@
                           {'id': store_id,
                            'val': val,
                            'expiration': expires}, True)
         if self.use_signer:
             session_id = self._get_signer(app).sign(want_bytes(session.sid))
         else:
             session_id = session.sid
-        response.set_cookie(app.session_cookie_name, session_id,
+        response.set_cookie(app.config["SESSION_COOKIE_NAME"], session_id,
                             expires=expires, httponly=httponly,
                             domain=domain, path=path, secure=secure,
                             **conditional_cookie_kwargs)
 
 
 class SqlAlchemySessionInterface(SessionInterface):
     """Uses the Flask-SQLAlchemy from a flask app as a session backend.
@@ -510,15 +500,15 @@
             def __repr__(self):
                 return '<Session data %s>' % self.data
 
         # self.db.create_all()
         self.sql_session_model = Session
 
     def open_session(self, app, request):
-        sid = request.cookies.get(app.session_cookie_name)
+        sid = request.cookies.get(app.config["SESSION_COOKIE_NAME"])
         if not sid:
             sid = self._generate_sid()
             return self.session_class(sid=sid, permanent=self.permanent)
         if self.use_signer:
             signer = self._get_signer(app)
             if signer is None:
                 return None
@@ -553,15 +543,15 @@
         saved_session = self.sql_session_model.query.filter_by(
             session_id=store_id).first()
         if not session:
             if session.modified:
                 if saved_session:
                     self.db.session.delete(saved_session)
                     self.db.session.commit()
-                response.delete_cookie(app.session_cookie_name,
+                response.delete_cookie(app.config["SESSION_COOKIE_NAME"],
                                        domain=domain, path=path)
             return
 
         conditional_cookie_kwargs = {}
         httponly = self.get_cookie_httponly(app)
         secure = self.get_cookie_secure(app)
         if self.has_same_site_capability:
@@ -576,11 +566,11 @@
             new_session = self.sql_session_model(store_id, val, expires)
             self.db.session.add(new_session)
             self.db.session.commit()
         if self.use_signer:
             session_id = self._get_signer(app).sign(want_bytes(session.sid))
         else:
             session_id = session.sid
-        response.set_cookie(app.session_cookie_name, session_id,
+        response.set_cookie(app.config["SESSION_COOKIE_NAME"], session_id,
                             expires=expires, httponly=httponly,
                             domain=domain, path=path, secure=secure,
                             **conditional_cookie_kwargs)
```

### Comparing `Flask-Session-0.4.1/test_session.py` & `Flask-Session-0.5.0/test_session.py`

 * *Files identical despite different names*

