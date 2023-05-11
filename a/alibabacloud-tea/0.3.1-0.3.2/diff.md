# Comparing `tmp/alibabacloud-tea-0.3.1.tar.gz` & `tmp/alibabacloud-tea-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-tea-0.3.1.tar", last modified: Tue Mar 28 02:21:36 2023, max compression
+gzip compressed data, was "dist/alibabacloud-tea-0.3.2.tar", last modified: Thu May 11 02:51:44 2023, max compression
```

## Comparing `alibabacloud-tea-0.3.1.tar` & `alibabacloud-tea-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     2244 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1189 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9895 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/core.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/model.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/request.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/response.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/Tea/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/alibabacloud_tea.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2244 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/alibabacloud_tea.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      321 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/alibabacloud_tea.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/alibabacloud_tea.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/alibabacloud_tea.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/alibabacloud_tea.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2267 2023-03-28 02:21:36.000000 alibabacloud-tea-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9895 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/core.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/model.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/request.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/response.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/setup.py
```

### Comparing `alibabacloud-tea-0.3.1/PKG-INFO` & `alibabacloud-tea-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: alibabacloud-tea
-Version: 0.3.1
+Version: 0.3.2
 Summary: The tea module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/tea-python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud-tea-0.3.1/README.md` & `alibabacloud-tea-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.1/Tea/core.py` & `alibabacloud-tea-0.3.2/Tea/core.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.1/Tea/exceptions.py` & `alibabacloud-tea-0.3.2/Tea/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.1/Tea/model.py` & `alibabacloud-tea-0.3.2/Tea/model.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.1/Tea/request.py` & `alibabacloud-tea-0.3.2/Tea/request.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.1/Tea/stream.py` & `alibabacloud-tea-0.3.2/Tea/stream.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.1/alibabacloud_tea.egg-info/PKG-INFO` & `alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: alibabacloud-tea
-Version: 0.3.1
+Version: 0.3.2
 Summary: The tea module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/tea-python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud-tea-0.3.1/setup.py` & `alibabacloud-tea-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,27 +12,35 @@
  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  KIND, either express or implied.  See the License for the
  specific language governing permissions and limitations
  under the License.
 """
 
 import os
+import ssl
 from setuptools import setup, find_packages
 
 """
 Setup module for tea.
 Created on 3/24/2020
 @author: Alibaba Cloud
 """
 
-
-install_requires = [
-    'requests>=2.21.0, <3.0.0',
-    'aiohttp>=3.7.0, <4.0.0'
-]
+if ssl.OPENSSL_VERSION_INFO is not None and len(ssl.OPENSSL_VERSION_INFO) >= 3 and ssl.OPENSSL_VERSION_INFO[:3] >= (
+        1, 1, 1):
+    install_requires = [
+        'requests>=2.21.0, <3.0.0',
+        'aiohttp>=3.7.0, <4.0.0'
+    ]
+else:
+    install_requires = [
+        'requests>=2.21.0, <3.0.0',
+        'aiohttp>=3.7.0, <4.0.0',
+        'urllib3<2.0.0'
+    ]
 
 PACKAGE = "Tea"
 DESCRIPTION = "The tea module of alibabaCloud Python SDK."
 AUTHOR = "Alibaba Cloud"
 AUTHOR_EMAIL = "alibaba-cloud-sdk-dev-team@list.alibaba-inc.com"
 URL = "https://github.com/aliyun/tea-python"
 VERSION = __import__(PACKAGE).__version__
```

