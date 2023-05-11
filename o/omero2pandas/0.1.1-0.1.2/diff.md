# Comparing `tmp/omero2pandas-0.1.1.tar.gz` & `tmp/omero2pandas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero2pandas-0.1.1.tar", last modified: Wed May  3 10:20:39 2023, max compression
+gzip compressed data, was "omero2pandas-0.1.2.tar", last modified: Thu May 11 13:26:06 2023, max compression
```

## Comparing `omero2pandas-0.1.1.tar` & `omero2pandas-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:20:39.263049 omero2pandas-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 10:20:31.000000 omero2pandas-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-03 10:20:39.263049 omero2pandas-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-03 10:20:31.000000 omero2pandas-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:20:39.263049 omero2pandas-0.1.1/omero2pandas/
--rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-05-03 10:20:31.000000 omero2pandas-0.1.1/omero2pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-03 10:20:31.000000 omero2pandas-0.1.1/omero2pandas/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-03 10:20:31.000000 omero2pandas-0.1.1/omero2pandas/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 10:20:35.000000 omero2pandas-0.1.1/omero2pandas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:20:39.263049 omero2pandas-0.1.1/omero2pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-03 10:20:39.000000 omero2pandas-0.1.1/omero2pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-03 10:20:39.000000 omero2pandas-0.1.1/omero2pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:20:39.000000 omero2pandas-0.1.1/omero2pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 10:20:39.000000 omero2pandas-0.1.1/omero2pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 10:20:39.000000 omero2pandas-0.1.1/omero2pandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:20:39.000000 omero2pandas-0.1.1/omero2pandas.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:20:39.263049 omero2pandas-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 10:20:31.000000 omero2pandas-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:26:06.850347 omero2pandas-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 13:25:52.000000 omero2pandas-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-11 13:26:06.850347 omero2pandas-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-11 13:25:52.000000 omero2pandas-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:26:06.850347 omero2pandas-0.1.2/omero2pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-05-11 13:25:52.000000 omero2pandas-0.1.2/omero2pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-11 13:25:52.000000 omero2pandas-0.1.2/omero2pandas/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-11 13:25:52.000000 omero2pandas-0.1.2/omero2pandas/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 13:26:01.000000 omero2pandas-0.1.2/omero2pandas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:26:06.850347 omero2pandas-0.1.2/omero2pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-11 13:26:06.000000 omero2pandas-0.1.2/omero2pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-11 13:26:06.000000 omero2pandas-0.1.2/omero2pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:26:06.000000 omero2pandas-0.1.2/omero2pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 13:26:06.000000 omero2pandas-0.1.2/omero2pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 13:26:06.000000 omero2pandas-0.1.2/omero2pandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:26:06.000000 omero2pandas-0.1.2/omero2pandas.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:26:06.850347 omero2pandas-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-11 13:25:52.000000 omero2pandas-0.1.2/setup.py
```

### Comparing `omero2pandas-0.1.1/LICENSE` & `omero2pandas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omero2pandas-0.1.1/PKG-INFO` & `omero2pandas-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero2pandas
-Version: 0.1.1
+Version: 0.1.2
 Summary: OMERO.tables to pandas bridge
 Home-page: https://github.com/glencoesoftware/omero2pandas
 Author: Glencoe Software, Inc.
 Author-email: info@glencoesoftware.com
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,20 +14,35 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: token
 License-File: LICENSE
 
 # omero2pandas
 
 A convenience package to download data from OMERO.tables into Pandas dataframes.
 
+# Installation
+
+omero2pandas can be installed with pip on Python 3.6+:
+```
+pip install omero2pandas
+```
+omero2pandas also supports authentication using tokens generated by `omero-user-token`. 
+Compatible versions can be installed as follows:
+```
+pip install omero2pandas[token]
+```
+See the [omero-user-token documentation](https://github.com/glencoesoftware/omero-user-token) for more information.
+
+
 # Usage
 
 ```python
 import omero2pandas
 df = omero2pandas.read_table(file_id=402)
 df.head()
 ```
```

### Comparing `omero2pandas-0.1.1/README.md` & `omero2pandas-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # omero2pandas
 
 A convenience package to download data from OMERO.tables into Pandas dataframes.
 
+# Installation
+
+omero2pandas can be installed with pip on Python 3.6+:
+```
+pip install omero2pandas
+```
+omero2pandas also supports authentication using tokens generated by `omero-user-token`. 
+Compatible versions can be installed as follows:
+```
+pip install omero2pandas[token]
+```
+See the [omero-user-token documentation](https://github.com/glencoesoftware/omero-user-token) for more information.
+
+
 # Usage
 
 ```python
 import omero2pandas
 df = omero2pandas.read_table(file_id=402)
 df.head()
 ```
```

### Comparing `omero2pandas-0.1.1/omero2pandas/__init__.py` & `omero2pandas-0.1.2/omero2pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `omero2pandas-0.1.1/omero2pandas/connect.py` & `omero2pandas-0.1.2/omero2pandas/connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 #
 # This software is distributed under the terms described by the LICENCE file
 # you can find at the root of the distribution bundle.
 # If the file is missing please request a copy by contacting
 # support@glencoesoftware.com.
 import atexit
 import getpass
+import importlib.util
 import logging
+import weakref
 
 import omero
 from omero.gateway import BlitzGateway
 
 LOGGER = logging.getLogger(__name__)
 
+ACTIVE_CONNECTORS = weakref.WeakSet()
+
 
 class OMEROConnection:
     """
     A class designed to handle OMERO connections and manage sessions gracefully
     """
     def __init__(self, client=None, server=None, port=4064, username=None,
                  password=None, session_key=None, allow_token=True):
@@ -42,15 +46,15 @@
         self.port = port
         self.username = username
         self.password = password
         self.session_key = session_key
         if allow_token and self.need_connection_details():
             self.get_user_token()
         # Make sure that session closer runs on interpreter exit.
-        atexit.register(self.shutdown)
+        ACTIVE_CONNECTORS.add(self)
 
     def __getattr__(self, attr):
         # Forward function calls to the client object, if one exists.
         if self.client is None:
             raise ValueError("Client is not initialised")
         return getattr(self.client, attr)
 
@@ -113,15 +117,15 @@
                 raise Exception("Insufficient details to create a connection")
 
         self.client = omero.client(host=self.server, port=self.port)
         if self.session_key is not None:
             try:
                 self.client.joinSession(self.session_key)
             except Exception as e:
-                print(f"Failed to join session: {e}")
+                print(f"Failed to join session, token may have expired: {e}")
                 self.client = None
                 return False
         elif self.username is not None:
             try:
                 self.session = self.client.createSession(
                     username=self.username, password=self.password)
                 self.client.enableKeepAlive(60)
@@ -229,22 +233,24 @@
 
     def get_user_token(self):
         # Check for user token and apply to class
         if self.server is None and self.username is None:
             try:
                 import omero_user_token
                 LOGGER.info("Requesting token info")
-                token = omero_user_token.getter()
+                token = omero_user_token.get_token()
                 self.server, port = token[token.find('@') + 1:].split(':')
                 self.port = int(port)
                 self.session_key = token[:token.find('@')]
                 LOGGER.info(f"Found token for connection to"
                             f" {self.server}:{self.port}")
             except ImportError:
                 LOGGER.info("omero_user_token not installed")
+            except AttributeError:
+                LOGGER.warning("Please update omero-user-token to >=0.3.0")
             except Exception:
                 LOGGER.error("Failed to process user token", exc_info=True)
         else:
             LOGGER.info("Server or User details already provided, "
                         "will skip token check.")
 
     def get_gateway(self):
@@ -265,10 +271,24 @@
     # Determine whether we're running in a Jupyter Notebook.
     try:
         from IPython import get_ipython
     except ImportError:
         return False
     shell = get_ipython().__class__.__name__
     if shell == 'ZMQInteractiveShell':
+        if importlib.util.find_spec("ipywidgets") is None:
+            LOGGER.warning(
+                "Detected Jupyter environment but no ipywidgets, "
+                "cannot show interactive login widget.")
+            return False
         LOGGER.debug("Detected Jupyter environment")
         return True
     return False
+
+
+def cleanup_sessions():
+    # Shut down any active sessions when exiting Python
+    for connector in ACTIVE_CONNECTORS:
+        connector.shutdown()
+
+
+atexit.register(cleanup_sessions)
```

### Comparing `omero2pandas-0.1.1/omero2pandas/upload.py` & `omero2pandas-0.1.2/omero2pandas/upload.py`

 * *Files identical despite different names*

### Comparing `omero2pandas-0.1.1/omero2pandas.egg-info/PKG-INFO` & `omero2pandas-0.1.2/omero2pandas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero2pandas
-Version: 0.1.1
+Version: 0.1.2
 Summary: OMERO.tables to pandas bridge
 Home-page: https://github.com/glencoesoftware/omero2pandas
 Author: Glencoe Software, Inc.
 Author-email: info@glencoesoftware.com
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,20 +14,35 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: token
 License-File: LICENSE
 
 # omero2pandas
 
 A convenience package to download data from OMERO.tables into Pandas dataframes.
 
+# Installation
+
+omero2pandas can be installed with pip on Python 3.6+:
+```
+pip install omero2pandas
+```
+omero2pandas also supports authentication using tokens generated by `omero-user-token`. 
+Compatible versions can be installed as follows:
+```
+pip install omero2pandas[token]
+```
+See the [omero-user-token documentation](https://github.com/glencoesoftware/omero-user-token) for more information.
+
+
 # Usage
 
 ```python
 import omero2pandas
 df = omero2pandas.read_table(file_id=402)
 df.head()
 ```
```

### Comparing `omero2pandas-0.1.1/setup.py` & `omero2pandas-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,11 +48,14 @@
     include_package_data=True,
     platforms='any',
     install_requires=[
         'omero-py',
         'pandas',
         'tqdm',
     ],
+    extras_require={
+            "token": ["omero-user-token>=0.3.0"],
+        },
     setup_requires=['pytest-runner', 'flake8'],
     tests_require=['pytest', 'flake8'],
     zip_safe=True,
 )
```

