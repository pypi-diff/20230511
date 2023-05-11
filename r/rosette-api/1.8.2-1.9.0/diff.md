# Comparing `tmp/rosette_api-1.8.2.tar.gz` & `tmp/rosette_api-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rosette_api-1.8.2.tar", last modified: Wed Dec 13 18:39:40 2017, max compression
+gzip compressed data, was "dist/rosette_api-1.9.0.tar", last modified: Wed Jan 17 19:51:16 2018, max compression
```

## Comparing `rosette_api-1.8.2.tar` & `rosette_api-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-12-13 18:39:40.000000 rosette_api-1.8.2/
--rw-r--r--   0 root         (0) root         (0)      579 2017-12-13 18:39:40.000000 rosette_api-1.8.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       38 2017-12-13 18:39:40.000000 rosette_api-1.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3046 2017-12-13 18:39:40.000000 rosette_api-1.8.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette/
--rw-r--r--   0 root         (0) root         (0)      638 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40611 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette/api.py
--rw-r--r--   0 root         (0) root         (0)     1878 2017-12-13 18:39:40.000000 rosette_api-1.8.2/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1452 2017-12-13 18:39:40.000000 rosette_api-1.8.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3046 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2017-12-13 18:39:40.000000 rosette_api-1.8.2/rosette_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-17 19:51:16.000000 rosette_api-1.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette/
+-rw-r--r--   0 root         (0) root         (0)      638 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36380 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3044 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      239 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2018-01-17 19:51:16.000000 rosette_api-1.9.0/rosette_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      579 2018-01-17 19:51:16.000000 rosette_api-1.9.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1876 2018-01-17 19:51:16.000000 rosette_api-1.9.0/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1452 2018-01-17 19:51:16.000000 rosette_api-1.9.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3044 2018-01-17 19:51:16.000000 rosette_api-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2018-01-17 19:51:16.000000 rosette_api-1.9.0/setup.cfg
```

### Comparing `rosette_api-1.8.2/LICENSE.txt` & `rosette_api-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rosette_api-1.8.2/PKG-INFO` & `rosette_api-1.9.0/rosette_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
-Name: rosette_api
-Version: 1.8.2
+Name: rosette-api
+Version: 1.9.0
 Summary: Rosette API Python client SDK
 Home-page: https://developer.rosette.com
 Author: Basis Technology Corp.
 Author-email: rosette_api@basistech.com
 License: Apache License
 Description-Content-Type: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/rosette-api/python.svg?branch=master)](https://travis-ci.org/rosette-api/python)
         
         ## This is the Python client binding for Rosette API.
         Please check out the [wiki](https://github.com/rosette-api/python/wiki) for additional information
         
         ### Installation
         
-        The Python binding requires Python 2.6 or greater and is available through pip:
+        The Python binding requires Python 2.7+ or 3.4+ and is available through pip:
         
         `pip install rosette_api`
         
         If the version you are using is not [the latest from PyPI](https://pypi.org/project/rosette_api/#history),
         please check for its [**compatibilty with api.rosette.com**](https://developer.rosette.com/features-and-functions?python).
         If you have an on-premise version of Rosette API server, please contact support for
         binding compatibility with your installation.
```

### Comparing `rosette_api-1.8.2/rosette/__init__.py` & `rosette_api-1.9.0/rosette/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = '1.8.2'
+__version__ = '1.9.0'
```

### Comparing `rosette_api-1.8.2/rosette/api.py` & `rosette_api-1.9.0/rosette/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 import json
 import logging
 import sys
 import os
 import re
 import warnings
 import requests
+import platform
 
-_BINDING_VERSION = '1.8.2'
+_BINDING_VERSION = '1.9.0'
 _GZIP_BYTEARRAY = bytearray([0x1F, 0x8b, 0x08])
 
 _ISPY3 = sys.version_info[0] == 3
 
 
 if _ISPY3:
     _GZIP_SIGNATURE = _GZIP_BYTEARRAY
@@ -78,58 +79,14 @@
     def __str__(self):
         sst = self.status
         if not isinstance(sst, str):
             sst = repr(sst)
         return sst + ": " + self.message + ":\n  " + self.response_message
 
 
-class _PseudoEnum(object):
-    """ Base class for MorphologyOutput """
-
-    def __init__(self):
-        pass
-
-    @classmethod
-    def validate(cls, value, name):
-        """ validation method """
-        values = []
-        for (key, value) in vars(cls).items():
-            if not key.startswith("__"):
-                values += [value]
-
-        # this is still needed to make sure that the parameter NAMES are known.
-        # If python didn't allow setting unknown values, this would be a
-        # language error.
-        if value not in values:
-            raise RosetteException(
-                "unknownVariable",
-                "The value supplied for " +
-                name +
-                " is not one of " +
-                ", ".join(values) +
-                ".",
-                repr(value))
-
-
-class MorphologyOutput(_PseudoEnum):
-    """ Class to provide Morphology sub-endpoints """
-
-    def __init__(self):
-        warnings.warn('MorphologyOutput to be removed in version 1.9.0. '
-                      'Please use API.morphology_output',
-                      DeprecationWarning)
-        _PseudoEnum.__init__()
-
-    LEMMAS = "lemmas"
-    PARTS_OF_SPEECH = "parts-of-speech"
-    COMPOUND_COMPONENTS = "compound-components"
-    HAN_READINGS = "han-readings"
-    COMPLETE = "complete"
-
-
 class _DocumentParamSetBase(object):
 
     def __init__(self, repertoire):
         self.__params = {}
         for k in repertoire:
             self.__params[k] = None
 
@@ -578,14 +535,15 @@
 
         self.connection_refresh_duration = refresh_duration
         self.options = {}
         self.custom_headers = {}
         self.url_parameters = {}
         self.max_pool_size = 1
         self.session = requests.Session()
+        self.user_agent_string = 'RosetteAPIPython/' + _BINDING_VERSION + '/' + platform.python_version()
 
         self.morphology_output = {
             'LEMMAS': 'lemmas',
             'PARTS_OF_SPEECH': 'parts-of-speech',
             'COMPOUND_COMPONENTS': 'compound-components',
             'HAN_READINGS': 'han-readings',
             'COMPLETE': 'complete'
@@ -613,14 +571,18 @@
 
     def __del__(self):
         try:
             self.session.close()
         except ReferenceError:
             pass
 
+    def get_user_agent_string(self):
+        """ Return the User-Agent string """
+        return self.user_agent_string
+
     def _set_pool_size(self):
         adapter = requests.adapters.HTTPAdapter(
             pool_maxsize=self.max_pool_size)
         if 'https:' in self.service_url:
             self.session.mount('https://', adapter)
         else:
             self.session.mount('http://', adapter)
@@ -628,15 +590,15 @@
     def _make_request(self, operation, url, data, headers):
         """
         @param operation: POST or GET
         @param url: endpoing URL
         @param data: request data
         @param headers: request headers
         """
-        headers['User-Agent'] = "RosetteAPIPython/" + _BINDING_VERSION
+        headers['User-Agent'] = self.get_user_agent_string()
 
         message = None
         code = "unknownError"
         rdata = None
         response_headers = {}
 
         payload = None
@@ -714,197 +676,99 @@
 
         if len(rdata) > 3 and rdata[0:3] == _GZIP_SIGNATURE:
             buf = BytesIO(rdata)
             rdata = gzip.GzipFile(fileobj=buf).read()
 
         return _ReturnObject(_my_loads(rdata, response_headers), status)
 
-    def getPoolSize(self):
-        """
-        Returns the maximum pool size, which is the returned x-rosetteapi-concurrency value
-        """
-        warnings.warn('Method renamed to API.get_pool_size(). To be removed in version 1.9.0',
-                      DeprecationWarning)
-        return self.get_pool_size()
-
     def get_pool_size(self):
         """
         Returns the maximum pool size, which is the returned x-rosetteapi-concurrency value
         """
         return int(self.max_pool_size)
 
-    def setOption(self, name, value):
-        """
-        Sets an option
-
-        @param name: name of option
-        @param value: value of option
-        """
-        warnings.warn('Method renamed to API.set_option().  To be removed in version 1.9.0',
-                      DeprecationWarning)
-        return self.set_option(name, value)
-
     def set_option(self, name, value):
         """
         Sets an option
 
         @param name: name of option
         @param value: value of option
         """
         if value is None:
             self.options.pop(name, None)
         else:
             self.options[name] = value
 
-    def getOption(self, name):
-        """
-        Gets an option
-
-        @param name: name of option
-
-        @return: value of option
-        """
-        warnings.warn('Method renamed to API.get_option().  To be removed in version 1.9.0',
-                      DeprecationWarning)
-        return self.get_option(name)
-
     def get_option(self, name):
         """
         Gets an option
 
         @param name: name of option
 
         @return: value of option
         """
         if name in self.options.keys():
             return self.options[name]
         else:
             return None
 
-    def clearOptions(self):
-        """
-        Clears all options
-        """
-        warnings.warn('Method renamed to API.clear_options().  To be removed in version 1.9.0',
-                      DeprecationWarning)
-        self.clear_options()
-
     def clear_options(self):
         """
         Clears all options
         """
         self.options.clear()
 
-    def setUrlParameter(self, name, value):
-        """
-        Sets a URL parameter
-
-        @param name: name of parameter
-        @param value: value of parameter
-        """
-        warnings.warn('Method renamed to API.set_url_parameter().  To be removed in version 1.9.0',
-                      DeprecationWarning)
-        return self.set_url_parameter(name, value)
-
     def set_url_parameter(self, name, value):
         """
         Sets a URL parameter
 
         @param name: name of parameter
         @param value: value of parameter
         """
         if value is None:
             self.url_parameters.pop(name, None)
         else:
             self.url_parameters[name] = value
 
-    def getUrlParameter(self, name):
-        """
-        Gets a URL parameter
-
-        @param name: name of parameter
-
-        @return: value of parameter
-        """
-        warnings.warn('Method renamed to API.get_url_parameter().  To be removed in version 1.9.0',
-                      DeprecationWarning)
-        return self.get_url_parameter(name)
-
     def get_url_parameter(self, name):
         """
         Gets a URL parameter
 
         @param name: name of parameter
 
         @return: value of parameter
         """
         if name in self.url_parameters.keys():
             return self.url_parameters[name]
         else:
             return None
 
-    def clearUrlParameters(self):
-        """
-        Clears all options
-        """
-        warnings.warn('Method renamed to API.clear_url_parameters(). '
-                      'To be removed in version 1.9.0',
-                      DeprecationWarning)
-        self.clear_url_parameters()
-
     def clear_url_parameters(self):
         """
         Clears all options
         """
         self.url_parameters.clear()
 
-    def setCustomHeaders(self, name, value):
-        """
-        Sets custom headers
-
-        @param headers: array of custom headers to be set
-        """
-        warnings.warn('Method renamed to API.set_custom_headers().  To be removed in version 1.9.0',
-                      DeprecationWarning)
-        return self.set_custom_headers(name, value)
-
     def set_custom_headers(self, name, value):
         """
         Sets custom headers
 
         @param headers: array of custom headers to be set
         """
         if value is None:
             self.custom_headers.pop(name, None)
         else:
             self.custom_headers[name] = value
 
-    def getCustomHeaders(self):
-        """
-        Get custom headers
-        """
-        warnings.warn('Method renamed to API.get_custom_headers().  To be removed in version 1.9.0',
-                      DeprecationWarning)
-        return self.get_custom_headers()
-
     def get_custom_headers(self):
         """
         Get custom headers
         """
         return self.custom_headers
 
-    def clearCustomHeaders(self):
-        """
-        Clears custom headers
-        """
-        warnings.warn('Method renamed to API.clear_custom_headers(). '
-                      'To be removed in version 1.9.0',
-                      DeprecationWarning)
-        self.clear_custom_headers()
-
     def clear_custom_headers(self):
         """
         Clears custom headers
         """
 
         self.custom_headers.clear()
```

### Comparing `rosette_api-1.8.2/README.md` & `rosette_api-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![Build Status](https://travis-ci.org/rosette-api/python.svg?branch=master)](https://travis-ci.org/rosette-api/python)
 
 ## This is the Python client binding for Rosette API.
 Please check out the [wiki](https://github.com/rosette-api/python/wiki) for additional information
 
 ### Installation
 
-The Python binding requires Python 2.6 or greater and is available through pip:
+The Python binding requires Python 2.7+ or 3.4+ and is available through pip:
 
 `pip install rosette_api`
 
 If the version you are using is not [the latest from PyPI](https://pypi.org/project/rosette_api/#history),
 please check for its [**compatibilty with api.rosette.com**](https://developer.rosette.com/features-and-functions?python).
 If you have an on-premise version of Rosette API server, please contact support for
 binding compatibility with your installation.
```

### Comparing `rosette_api-1.8.2/setup.py` & `rosette_api-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `rosette_api-1.8.2/rosette_api.egg-info/PKG-INFO` & `rosette_api-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
-Name: rosette-api
-Version: 1.8.2
+Name: rosette_api
+Version: 1.9.0
 Summary: Rosette API Python client SDK
 Home-page: https://developer.rosette.com
 Author: Basis Technology Corp.
 Author-email: rosette_api@basistech.com
 License: Apache License
 Description-Content-Type: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/rosette-api/python.svg?branch=master)](https://travis-ci.org/rosette-api/python)
         
         ## This is the Python client binding for Rosette API.
         Please check out the [wiki](https://github.com/rosette-api/python/wiki) for additional information
         
         ### Installation
         
-        The Python binding requires Python 2.6 or greater and is available through pip:
+        The Python binding requires Python 2.7+ or 3.4+ and is available through pip:
         
         `pip install rosette_api`
         
         If the version you are using is not [the latest from PyPI](https://pypi.org/project/rosette_api/#history),
         please check for its [**compatibilty with api.rosette.com**](https://developer.rosette.com/features-and-functions?python).
         If you have an on-premise version of Rosette API server, please contact support for
         binding compatibility with your installation.
```

