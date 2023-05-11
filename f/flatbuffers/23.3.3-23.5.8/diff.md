# Comparing `tmp/flatbuffers-23.3.3.tar.gz` & `tmp/flatbuffers-23.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatbuffers-23.3.3.tar", last modified: Fri Mar  3 19:50:20 2023, max compression
+gzip compressed data, was "flatbuffers-23.5.8.tar", last modified: Tue May  9 15:11:11 2023, max compression
```

## Comparing `flatbuffers-23.3.3.tar` & `flatbuffers-23.5.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:50:20.420388 flatbuffers-23.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-03 19:50:20.420388 flatbuffers-23.3.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:50:20.420388 flatbuffers-23.3.3/flatbuffers/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    44275 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/flexbuffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/number_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/flatbuffers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 19:50:20.420388 flatbuffers-23.3.3/flatbuffers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-03 19:50:20.000000 flatbuffers-23.3.3/flatbuffers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-03 19:50:20.000000 flatbuffers-23.3.3/flatbuffers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 19:50:20.000000 flatbuffers-23.3.3/flatbuffers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-03 19:50:20.000000 flatbuffers-23.3.3/flatbuffers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-03 19:50:20.420388 flatbuffers-23.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-03 19:50:11.000000 flatbuffers-23.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:11:11.805129 flatbuffers-23.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-09 15:11:11.805129 flatbuffers-23.5.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:11:11.805129 flatbuffers-23.5.8/flatbuffers/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44275 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/flexbuffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/number_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/flatbuffers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:11:11.805129 flatbuffers-23.5.8/flatbuffers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-09 15:11:11.000000 flatbuffers-23.5.8/flatbuffers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-09 15:11:11.000000 flatbuffers-23.5.8/flatbuffers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:11:11.000000 flatbuffers-23.5.8/flatbuffers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 15:11:11.000000 flatbuffers-23.5.8/flatbuffers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 15:11:11.805129 flatbuffers-23.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-09 15:10:59.000000 flatbuffers-23.5.8/setup.py
```

### Comparing `flatbuffers-23.3.3/PKG-INFO` & `flatbuffers-23.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatbuffers
-Version: 23.3.3
+Version: 23.5.8
 Summary: The FlatBuffers serialization format for Python
 Home-page: https://google.github.io/flatbuffers/
 Author: Derek Bailey
 Author-email: derekbailey@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://google.github.io/flatbuffers/
 Project-URL: Source, https://github.com/google/flatbuffers
```

### Comparing `flatbuffers-23.3.3/flatbuffers/__init__.py` & `flatbuffers-23.5.8/flatbuffers/__init__.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/_version.py` & `flatbuffers-23.5.8/flatbuffers/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Placeholder, to be updated during the release process
 # by the setup.py
-__version__ = u"23.3.3"
+__version__ = u"23.5.8"
```

### Comparing `flatbuffers-23.3.3/flatbuffers/builder.py` & `flatbuffers-23.5.8/flatbuffers/builder.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/compat.py` & `flatbuffers-23.5.8/flatbuffers/compat.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/encode.py` & `flatbuffers-23.5.8/flatbuffers/encode.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/flexbuffers.py` & `flatbuffers-23.5.8/flatbuffers/flexbuffers.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/number_types.py` & `flatbuffers-23.5.8/flatbuffers/number_types.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/packer.py` & `flatbuffers-23.5.8/flatbuffers/packer.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/table.py` & `flatbuffers-23.5.8/flatbuffers/table.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers/util.py` & `flatbuffers-23.5.8/flatbuffers/util.py`

 * *Files identical despite different names*

### Comparing `flatbuffers-23.3.3/flatbuffers.egg-info/PKG-INFO` & `flatbuffers-23.5.8/flatbuffers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatbuffers
-Version: 23.3.3
+Version: 23.5.8
 Summary: The FlatBuffers serialization format for Python
 Home-page: https://google.github.io/flatbuffers/
 Author: Derek Bailey
 Author-email: derekbailey@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://google.github.io/flatbuffers/
 Project-URL: Source, https://github.com/google/flatbuffers
```

### Comparing `flatbuffers-23.3.3/setup.py` & `flatbuffers-23.5.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup
 
 setup(
     name='flatbuffers',
-    version='23.3.3',
+    version='23.5.8',
     license='Apache 2.0',
-    license_files='../LICENSE.txt',
+    license_files='../LICENSE',
     author='Derek Bailey',
     author_email='derekbailey@google.com',
     url='https://google.github.io/flatbuffers/',
     long_description=('Python runtime library for use with the '
                       '`Flatbuffers <https://google.github.io/flatbuffers/>`_ '
                       'serialization format.'),
     packages=['flatbuffers'],
```

