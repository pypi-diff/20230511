# Comparing `tmp/requests-raw-0.1.0.tar.gz` & `tmp/requests-raw-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\requests-raw-0.1.0.tar", last modified: Thu May 28 11:23:04 2020, max compression
+gzip compressed data, was "dist\requests-raw-0.2.1.tar", last modified: Fri May 29 18:13:57 2020, max compression
```

## Comparing `requests-raw-0.1.0.tar` & `requests-raw-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2020-05-28 11:23:04.193825 requests-raw-0.1.0/
--rw-rw-rw-   0        0        0    11541 2020-05-28 08:54:20.000000 requests-raw-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2109 2020-05-28 11:23:04.193825 requests-raw-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      534 2020-05-28 10:54:42.000000 requests-raw-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2020-05-28 11:23:04.177953 requests-raw-0.1.0/requests_raw/
--rw-rw-rw-   0        0        0      412 2020-05-28 07:56:30.000000 requests-raw-0.1.0/requests_raw/__init__.py
--rw-rw-rw-   0        0        0      360 2020-05-28 07:34:13.000000 requests-raw-0.1.0/requests_raw/__version__.py
--rw-rw-rw-   0        0        0      601 2020-05-27 18:21:50.000000 requests-raw-0.1.0/requests_raw/adapters.py
--rw-rw-rw-   0        0        0     2479 2020-05-28 08:14:25.000000 requests-raw-0.1.0/requests_raw/connection.py
--rw-rw-rw-   0        0        0      557 2020-05-27 17:07:52.000000 requests-raw-0.1.0/requests_raw/connectionpool.py
-drwxrwxrwx   0        0        0        0 2020-05-28 11:23:04.192858 requests-raw-0.1.0/requests_raw.egg-info/
--rw-rw-rw-   0        0        0     2109 2020-05-28 11:23:04.000000 requests-raw-0.1.0/requests_raw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2020-05-28 11:23:04.000000 requests-raw-0.1.0/requests_raw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-28 11:23:04.000000 requests-raw-0.1.0/requests_raw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-05-28 10:59:27.000000 requests-raw-0.1.0/requests_raw.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2020-05-28 11:23:04.000000 requests-raw-0.1.0/requests_raw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2020-05-28 11:23:04.000000 requests-raw-0.1.0/requests_raw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2020-05-28 11:23:04.196837 requests-raw-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2180 2020-05-28 11:22:42.000000 requests-raw-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2020-05-29 18:13:57.052561 requests-raw-0.2.1/
+-rw-rw-rw-   0        0        0    11541 2020-05-28 08:54:20.000000 requests-raw-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2891 2020-05-29 18:13:57.052697 requests-raw-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1098 2020-05-29 17:41:12.000000 requests-raw-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2020-05-29 18:13:57.042650 requests-raw-0.2.1/requests_raw/
+-rw-rw-rw-   0        0        0      553 2020-05-29 17:06:29.000000 requests-raw-0.2.1/requests_raw/__init__.py
+-rw-rw-rw-   0        0        0      360 2020-05-29 18:12:04.000000 requests-raw-0.2.1/requests_raw/__version__.py
+-rw-rw-rw-   0        0        0      601 2020-05-27 18:21:50.000000 requests-raw-0.2.1/requests_raw/adapters.py
+-rw-rw-rw-   0        0        0      203 2020-05-29 13:43:27.000000 requests-raw-0.2.1/requests_raw/api.py
+-rw-rw-rw-   0        0        0     3463 2020-05-29 18:00:44.000000 requests-raw-0.2.1/requests_raw/connection.py
+-rw-rw-rw-   0        0        0      557 2020-05-27 17:07:52.000000 requests-raw-0.2.1/requests_raw/connectionpool.py
+-rw-rw-rw-   0        0        0      485 2020-05-29 13:42:32.000000 requests-raw-0.2.1/requests_raw/sessions.py
+drwxrwxrwx   0        0        0        0 2020-05-29 18:13:57.050563 requests-raw-0.2.1/requests_raw.egg-info/
+-rw-rw-rw-   0        0        0     2891 2020-05-29 18:13:56.000000 requests-raw-0.2.1/requests_raw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2020-05-29 18:13:56.000000 requests-raw-0.2.1/requests_raw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-05-29 18:13:56.000000 requests-raw-0.2.1/requests_raw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-05-28 10:59:27.000000 requests-raw-0.2.1/requests_raw.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      172 2020-05-29 18:13:56.000000 requests-raw-0.2.1/requests_raw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2020-05-29 18:13:56.000000 requests-raw-0.2.1/requests_raw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2020-05-29 18:13:57.053592 requests-raw-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2381 2020-05-28 14:34:28.000000 requests-raw-0.2.1/setup.py
```

### Comparing `requests-raw-0.1.0/LICENSE` & `requests-raw-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-raw-0.1.0/requests_raw/adapters.py` & `requests-raw-0.2.1/requests_raw/adapters.py`

 * *Files identical despite different names*

### Comparing `requests-raw-0.1.0/requests_raw/connection.py` & `requests-raw-0.2.1/requests_raw/connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,91 @@
-from http import client
+from .__version__ import __title__
 from requests.utils import urlparse
 from urllib3.connection import HTTPConnection, HTTPSConnection
 
+try:
+    from http import client
+except ImportError:
+    import httplib as client
+
 
 class RawHTTPConnection(HTTPConnection):
     def __init__(self, *args, **kwargs):
         super(RawHTTPConnection, self).__init__(*args, **kwargs)
+        self.__url = None
+        self.__method = None
+
+    def putrequest(self, method, url, *args, **kwargs):
+        self.__method = method.lower()
+        if self.__method != __title__:
+            return super(RawHTTPConnection, self).putrequest(
+                method, url, *args, **kwargs
+            )
 
-    def putrequest(self, method, url, skip_host=False, skip_accept_encoding=False):
         self.__url = urlparse(url)
         if self._HTTPConnection__response and self._HTTPConnection__response.isclosed():
             self._HTTPConnection__response = None
 
         if self._HTTPConnection__state == client._CS_IDLE:
             self._HTTPConnection__state = client._CS_REQ_STARTED
         else:
             raise client.CannotSendRequest(self._HTTPConnection__state)
 
     def putheader(self, header, *values):
+        if self.__method != __title__:
+            return super(RawHTTPConnection, self).putheader(header, *values)
+
         if self._HTTPConnection__state != client._CS_REQ_STARTED:
             raise client.CannotSendHeader()
 
-    def endheaders(self, message_body=None, *, encode_chunked=False):
+    def endheaders(self, message_body=None, **kwargs):
+        if self.__method != __title__:
+            return super(RawHTTPConnection, self).endheaders(message_body=message_body, **kwargs)
+
         buffer = message_body
         # HTTP Proxy
         if self.__url.scheme and self.__url.netloc:
             _buffer = buffer.split(b"/", 1)
-            _buffer.insert(1, f"{self.__url.scheme}://{self.__url.netloc}/".encode())
+            _buffer.insert(1, "{url.scheme}://{url.netloc}/".format(url=self.__url).encode())
             buffer = b"".join(_buffer)
         if self._HTTPConnection__state == client._CS_REQ_STARTED:
             self._HTTPConnection__state = client._CS_REQ_SENT
         else:
             raise client.CannotSendHeader()
         self.send(buffer)
 
 
 class RawHTTPSConnection(HTTPSConnection):
     def __init__(self, *args, **kwargs):
         super(RawHTTPSConnection, self).__init__(*args, **kwargs)
 
-    def putrequest(self, method, url, skip_host=False, skip_accept_encoding=False):
+    def putrequest(self, method, url, *args, **kwargs):
+        self.__method = method.lower()
+        if self.__method != __title__:
+            return super(RawHTTPSConnection, self).putrequest(
+                method, url, *args, **kwargs
+            )
+
         if self._HTTPConnection__response and self._HTTPConnection__response.isclosed():
             self._HTTPConnection__response = None
 
         if self._HTTPConnection__state == client._CS_IDLE:
             self._HTTPConnection__state = client._CS_REQ_STARTED
         else:
             raise client.CannotSendRequest(self._HTTPConnection__state)
 
     def putheader(self, header, *values):
+        if self.__method != __title__:
+            return super(RawHTTPSConnection, self).putheader(header, *values)
+
         if self._HTTPConnection__state != client._CS_REQ_STARTED:
             raise client.CannotSendHeader()
 
-    def endheaders(self, message_body=None, *, encode_chunked=False):
+    def endheaders(self, message_body=None, **kwargs):
+        if self.__method != __title__:
+            return super(RawHTTPSConnection, self).endheaders(message_body=message_body, **kwargs)
+
         if self._HTTPConnection__state == client._CS_REQ_STARTED:
             self._HTTPConnection__state = client._CS_REQ_SENT
         else:
             raise client.CannotSendHeader()
         self.send(message_body)
```

### Comparing `requests-raw-0.1.0/requests_raw/connectionpool.py` & `requests-raw-0.2.1/requests_raw/connectionpool.py`

 * *Files identical despite different names*

### Comparing `requests-raw-0.1.0/setup.py` & `requests-raw-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,39 +20,42 @@
     version=about['__version__'],
     description=about['__description__'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=about['__author__'],
     author_email=about['__author_email__'],
     packages=find_packages(exclude=['examples', 'tests']),
-    python_requires=">2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
+    python_requires=">=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
     install_requires=install_requires,
     license=about['__license__'],
     platforms='any',
     url='https://github.com/realgam3/requests-raw',
     zip_safe=False,
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
+        'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     extras_require={
         'security': ['pyOpenSSL >= 0.14', 'cryptography>=1.3.4'],
         'socks': ['PySocks>=1.5.6, !=1.5.7'],
+        'socks:sys_platform == "win32" and python_version == "2.7"': ['win_inet_pton'],
     },
     project_urls={
         'Source': 'https://github.com/realgam3/requests-raw',
     },
 )
```

