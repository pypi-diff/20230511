# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.887.tar", last modified: Tue May  9 02:31:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.889.tar", last modified: Thu May 11 02:24:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.887.tar` & `tencentcloud-sdk-python-cdb-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   150803 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   526653 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 02:31:50.000000 tencentcloud-sdk-python-cdb-3.0.887/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   150803 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18943 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   526653 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 02:24:23.000000 tencentcloud-sdk-python-cdb-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:24:24.000000 tencentcloud-sdk-python-cdb-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/README.rst` & `tencentcloud-sdk-python-cdb-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/cdb/v20170320/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.889/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.887'
+__version__ = '3.0.889'
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.889/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.887
+Version: 3.0.889
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.889/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.887
+Version: 3.0.889
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.887/setup.py` & `tencentcloud-sdk-python-cdb-3.0.889/setup.py`

 * *Files identical despite different names*

