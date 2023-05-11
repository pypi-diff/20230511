# Comparing `tmp/tencentcloud-sdk-python-icr-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-icr-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-icr-3.0.888.tar", last modified: Wed May 10 02:16:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-icr-3.0.889.tar", last modified: Thu May 11 02:51:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-icr-3.0.888.tar` & `tencentcloud-sdk-python-icr-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/
--rw-r--r--   0 root         (0) root         (0)      652 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17883 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/models.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/icr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud_sdk_python_icr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud_sdk_python_icr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud_sdk_python_icr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud_sdk_python_icr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/tencentcloud_sdk_python_icr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:16:59.000000 tencentcloud-sdk-python-icr-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17883 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/models.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/icr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud_sdk_python_icr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud_sdk_python_icr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud_sdk_python_icr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud_sdk_python_icr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/tencentcloud_sdk_python_icr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:51:53.000000 tencentcloud-sdk-python-icr-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-icr-3.0.888/README.rst` & `tencentcloud-sdk-python-icr-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-icr-3.0.889/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.888'
+__version__ = '3.0.889'
```

### Comparing `tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/errorcodes.py` & `tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/models.py` & `tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.888/tencentcloud/icr/v20211014/icr_client.py` & `tencentcloud-sdk-python-icr-3.0.889/tencentcloud/icr/v20211014/icr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-icr-3.0.889/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-icr
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Icr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-icr-3.0.888/tencentcloud_sdk_python_icr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-icr-3.0.889/tencentcloud_sdk_python_icr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-icr
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Icr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-icr-3.0.888/setup.py` & `tencentcloud-sdk-python-icr-3.0.889/setup.py`

 * *Files identical despite different names*

