# Comparing `tmp/sioscgi-3.0.1.tar.gz` & `tmp/sioscgi-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sioscgi-3.0.1.tar", last modified: Thu Jan 26 07:26:46 2023, max compression
+gzip compressed data, was "sioscgi-4.0.0.tar", last modified: Thu May 11 05:03:02 2023, max compression
```

## Comparing `sioscgi-3.0.1.tar` & `sioscgi-4.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 07:26:46.264037 sioscgi-3.0.1/
--rw-r--r--   0 chead     (1000) chead     (1000)     1377 2023-01-26 07:12:51.000000 sioscgi-3.0.1/CHANGELOG.rst
--rw-r--r--   0 chead     (1000) chead     (1000)    35149 2019-04-21 18:53:48.000000 sioscgi-3.0.1/LICENSE
--rw-r--r--   0 chead     (1000) chead     (1000)       51 2020-06-16 06:10:44.000000 sioscgi-3.0.1/MANIFEST.in
--rw-r--r--   0 chead     (1000) chead     (1000)     4280 2023-01-26 07:26:46.264037 sioscgi-3.0.1/PKG-INFO
--rw-r--r--   0 chead     (1000) chead     (1000)     3607 2019-06-10 05:59:58.000000 sioscgi-3.0.1/README.rst
--rw-r--r--   0 chead     (1000) chead     (1000)      442 2023-01-26 07:10:21.000000 sioscgi-3.0.1/pyproject.toml
--rw-r--r--   0 chead     (1000) chead     (1000)      793 2023-01-26 07:26:46.265037 sioscgi-3.0.1/setup.cfg
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 07:26:46.260037 sioscgi-3.0.1/src/
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 07:26:46.262037 sioscgi-3.0.1/src/sioscgi/
--rw-r--r--   0 chead     (1000) chead     (1000)    23110 2023-01-26 06:55:12.000000 sioscgi-3.0.1/src/sioscgi/__init__.py
--rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-08-13 04:54:30.000000 sioscgi-3.0.1/src/sioscgi/py.typed
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 07:26:46.263037 sioscgi-3.0.1/src/sioscgi.egg-info/
--rw-r--r--   0 chead     (1000) chead     (1000)     4280 2023-01-26 07:26:46.000000 sioscgi-3.0.1/src/sioscgi.egg-info/PKG-INFO
--rw-r--r--   0 chead     (1000) chead     (1000)      324 2023-01-26 07:26:46.000000 sioscgi-3.0.1/src/sioscgi.egg-info/SOURCES.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-01-26 07:26:46.000000 sioscgi-3.0.1/src/sioscgi.egg-info/dependency_links.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        8 2023-01-26 07:26:46.000000 sioscgi-3.0.1/src/sioscgi.egg-info/top_level.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-01-26 07:26:45.000000 sioscgi-3.0.1/src/sioscgi.egg-info/zip-safe
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-01-26 07:26:46.264037 sioscgi-3.0.1/tests/
--rw-r--r--   0 chead     (1000) chead     (1000)        0 2020-06-16 06:00:09.000000 sioscgi-3.0.1/tests/__init__.py
--rw-r--r--   0 chead     (1000) chead     (1000)    15553 2020-06-16 06:00:09.000000 sioscgi-3.0.1/tests/test_sioscgi.py
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-11 05:03:02.892129 sioscgi-4.0.0/
+-rw-r--r--   0 chead     (1000) chead     (1000)     1562 2023-05-11 04:58:25.000000 sioscgi-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 chead     (1000) chead     (1000)    35149 2019-04-21 18:53:48.000000 sioscgi-4.0.0/LICENSE
+-rw-r--r--   0 chead     (1000) chead     (1000)       51 2020-06-16 06:10:44.000000 sioscgi-4.0.0/MANIFEST.in
+-rw-r--r--   0 chead     (1000) chead     (1000)     4303 2023-05-11 05:03:02.892129 sioscgi-4.0.0/PKG-INFO
+-rw-r--r--   0 chead     (1000) chead     (1000)     3607 2019-06-10 05:59:58.000000 sioscgi-4.0.0/README.rst
+-rw-r--r--   0 chead     (1000) chead     (1000)      442 2023-01-26 07:10:21.000000 sioscgi-4.0.0/pyproject.toml
+-rw-r--r--   0 chead     (1000) chead     (1000)      817 2023-05-11 05:03:02.893129 sioscgi-4.0.0/setup.cfg
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-11 05:03:02.890129 sioscgi-4.0.0/src/
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-11 05:03:02.891129 sioscgi-4.0.0/src/sioscgi/
+-rw-r--r--   0 chead     (1000) chead     (1000)    23272 2023-05-11 04:44:40.000000 sioscgi-4.0.0/src/sioscgi/__init__.py
+-rw-r--r--   0 chead     (1000) chead     (1000)        0 2019-08-13 04:54:30.000000 sioscgi-4.0.0/src/sioscgi/py.typed
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-11 05:03:02.892129 sioscgi-4.0.0/src/sioscgi.egg-info/
+-rw-r--r--   0 chead     (1000) chead     (1000)     4303 2023-05-11 05:03:02.000000 sioscgi-4.0.0/src/sioscgi.egg-info/PKG-INFO
+-rw-r--r--   0 chead     (1000) chead     (1000)      324 2023-05-11 05:03:02.000000 sioscgi-4.0.0/src/sioscgi.egg-info/SOURCES.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-05-11 05:03:02.000000 sioscgi-4.0.0/src/sioscgi.egg-info/dependency_links.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        8 2023-05-11 05:03:02.000000 sioscgi-4.0.0/src/sioscgi.egg-info/top_level.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-01-26 07:26:45.000000 sioscgi-4.0.0/src/sioscgi.egg-info/zip-safe
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-05-11 05:03:02.892129 sioscgi-4.0.0/tests/
+-rw-r--r--   0 chead     (1000) chead     (1000)        0 2020-06-16 06:00:09.000000 sioscgi-4.0.0/tests/__init__.py
+-rw-r--r--   0 chead     (1000) chead     (1000)    15553 2020-06-16 06:00:09.000000 sioscgi-4.0.0/tests/test_sioscgi.py
```

### Comparing `sioscgi-3.0.1/CHANGELOG.rst` & `sioscgi-4.0.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Changes in 4.0.0
+================
+
+CI configuration was updated. Very minor code cleanup was performed. This
+version requires Python 3.9 or higher due to updating to newer type hints.
+
 Changes in 3.0.1
 ================
 
 CI configuration, lint configuration, and build system configuration were
 updated. Very minor code cleanup was performed.
 
 Changes in 3.0.0
```

### Comparing `sioscgi-3.0.1/LICENSE` & `sioscgi-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sioscgi-3.0.1/PKG-INFO` & `sioscgi-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sioscgi
-Version: 3.0.1
+Version: 4.0.0
 Summary: A sans-I/O implementation of the SCGI specification.
 Home-page: https://gitlab.com/Hawk777/sioscgi
 Author: Christopher Head
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 What is sioscgi?
 ================
 
 sioscgi is an implementation of the Simple Common Gateway Interface (SCGI)
```

### Comparing `sioscgi-3.0.1/README.rst` & `sioscgi-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sioscgi-3.0.1/setup.cfg` & `sioscgi-4.0.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sioscgi
-version = 3.0.1
+version = 4.0.0
 url = https://gitlab.com/Hawk777/sioscgi
 author = Christopher Head
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
@@ -13,14 +13,15 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 description = A sans-I/O implementation of the SCGI specification.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 
 [options]
 zip_safe = True
+python_requires = >=3.9
 packages = sioscgi
 package_dir = 
 	=src
 
 [options.package_data]
 * = py.typed
```

### Comparing `sioscgi-3.0.1/src/sioscgi/__init__.py` & `sioscgi-4.0.0/src/sioscgi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Implements the SCGI protocol.
 """
 
 import collections
 import enum
 import logging
-from typing import Deque, Dict, List, Optional, Tuple, Type
+from typing import Optional
 import wsgiref.headers
 import wsgiref.util
 
 
 @enum.unique
 class RXState(enum.Enum):
     """
@@ -38,26 +38,29 @@
 class ProtocolError(Exception):
     """
     Raised when a violation of protocol occurs, by either the remote peer or
     the local application.
 
     This is the base class of LocalProtocolError and RemoteProtocolError.
     """
+    __slots__ = ()
 
 
 class LocalProtocolError(ProtocolError):
     """
     Raised when the local application violates protocol.
     """
+    __slots__ = ()
 
 
 class RemoteProtocolError(ProtocolError):
     """
     Raised when the remote peer violates protocol.
     """
+    __slots__ = ()
 
 
 class Event:
     """
     The base class of all events returned by an SCGIConnection.
     """
     __slots__ = ()
@@ -65,17 +68,17 @@
 
 class RequestHeaders(Event):
     """
     Reports that a request has started and carries the environment data.
     """
     __slots__ = ("environment",)
 
-    environment: Dict[str, bytes]
+    environment: dict[str, bytes]
 
-    def __init__(self, environment: Dict[str, bytes]):
+    def __init__(self, environment: dict[str, bytes]):
         """
         Construct a new RequestHeaders.
 
         :param environment: The environment variables, as a dict from name to
             value.
         """
         self.environment = environment
@@ -137,15 +140,15 @@
     __slots__ = ("status", "content_type", "location", "other_headers")
 
     status: Optional[str]
     content_type: Optional[str]
     location: Optional[str]
     other_headers: wsgiref.headers.Headers
 
-    def __init__(self, status: Optional[str], headers: List[Tuple[str, str]]):
+    def __init__(self, status: Optional[str], headers: list[tuple[str, str]]):
         """
         Construct a ResponseHeaders.
 
         :param status: The HTTP status code and string (e.g. “200 OK”), or None
             if a local redirect or client redirect without document is being
             generated.
         :param headers: A list of (name, value) tuples of HTTP headers.
@@ -288,18 +291,18 @@
         "_rx_eof",
         "_rx_env_length",
         "_rx_body_remaining",
     )
 
     _rx_state: RXState
     _tx_state: TXState
-    _error_class: Optional[Type[ProtocolError]]
+    _error_class: Optional[type[ProtocolError]]
     _error_msg: Optional[str]
-    _event_queue: Deque[Event]
-    _rx_buffer: Deque[bytes]
+    _event_queue: collections.deque[Event]
+    _rx_buffer: collections.deque[bytes]
     _rx_buffer_length: int
     _rx_buffer_limit: int
     _rx_eof: bool
     _rx_env_length: int
     _rx_body_remaining: int
 
     def __init__(self, rx_buffer_limit: int = 65536):
@@ -352,15 +355,15 @@
         passed in after a zero-length data has previously been passed. It does
         not raise exceptions for any other reason.
         """
         if data:
             if self._rx_eof:
                 logging.getLogger(__name__).debug("Received %d bytes after EOF", len(data))
                 raise self._report_local_error("Data received after EOF")
-            if self._rx_state != RXState.ERROR:
+            if self._rx_state is not RXState.ERROR:
                 logging.getLogger(__name__).debug("Received %d bytes", len(data))
                 self._rx_buffer.append(data)
                 self._rx_buffer_length += len(data)
         else:
             logging.getLogger(__name__).debug("Received EOF")
             self._rx_eof = True
         self._parse_events()
@@ -492,29 +495,30 @@
                     # Split the environment block into NUL-terminated chunks.
                     split_environment = environment[:-1].split(B"\x00")
                     # Check that there are an even number of parts.
                     if len(split_environment) % 2 == 1:
                         self._report_remote_error("Environment block missing final value")
                     else:
                         # Build the dictionary.
-                        env_dict: Dict[str, bytes] = {}
+                        env_dict: dict[str, bytes] = {}
                         for i in range(0, len(split_environment), 2):
                             try:
                                 key = split_environment[i].decode("ISO-8859-1")
                             except UnicodeError:
                                 self._report_remote_error("Environment variable name is not ISO-8859-1")
                                 break
                             if not key:
                                 self._report_remote_error("Environment variable with empty name")
                                 break
                             if key in env_dict:
                                 self._report_remote_error(f"Duplicate environment variable {key}")
                                 break
                             env_dict[key] = split_environment[i + 1]
-                        if self._rx_state != RXState.ERROR:
+                        # https://github.com/python/mypy/issues/9005
+                        if self._rx_state is not RXState.ERROR:  # type: ignore[comparison-overlap]
                             # Check for mandatory environment variables.
                             if env_dict.get("SCGI", None) != B"1":
                                 self._report_remote_error("Mandatory variable SCGI not set to 1")
                             else:
                                 # Advance the state machine, keeping any residual
                                 # bytes.
                                 self._rx_state = RXState.BODY
@@ -568,15 +572,15 @@
         during calls to receive_data but should be reported during calls to
         next_event.
 
         :param msg: The error message.
         """
         self._report_error(RemoteProtocolError, msg)
 
-    def _report_error(self, error_class: Type[ProtocolError], msg: str) -> None:
+    def _report_error(self, error_class: type[ProtocolError], msg: str) -> None:
         """
         Record an error for later reporting.
 
         :param error_class: The class of protocol error, either
             LocalProtocolError or RemoteProtocolError.
         :param msg: The error message.
         """
```

### Comparing `sioscgi-3.0.1/src/sioscgi.egg-info/PKG-INFO` & `sioscgi-4.0.0/src/sioscgi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sioscgi
-Version: 3.0.1
+Version: 4.0.0
 Summary: A sans-I/O implementation of the SCGI specification.
 Home-page: https://gitlab.com/Hawk777/sioscgi
 Author: Christopher Head
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 What is sioscgi?
 ================
 
 sioscgi is an implementation of the Simple Common Gateway Interface (SCGI)
```

### Comparing `sioscgi-3.0.1/tests/test_sioscgi.py` & `sioscgi-4.0.0/tests/test_sioscgi.py`

 * *Files identical despite different names*

