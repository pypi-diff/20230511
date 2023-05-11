# Comparing `tmp/tencentcloud-sdk-python-gs-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-gs-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gs-3.0.888.tar", last modified: Wed May 10 02:16:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gs-3.0.889.tar", last modified: Thu May 11 02:51:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gs-3.0.888.tar` & `tencentcloud-sdk-python-gs-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      734 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/
--rw-r--r--   0 root         (0) root         (0)     2065 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7825 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/gs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16447 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud_sdk_python_gs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud_sdk_python_gs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud_sdk_python_gs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud_sdk_python_gs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/tencentcloud_sdk_python_gs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:16:04.000000 tencentcloud-sdk-python-gs-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      734 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7825 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/gs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16482 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud_sdk_python_gs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud_sdk_python_gs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud_sdk_python_gs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud_sdk_python_gs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/tencentcloud_sdk_python_gs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:51:06.000000 tencentcloud-sdk-python-gs-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-gs-3.0.888/README.rst` & `tencentcloud-sdk-python-gs-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/errorcodes.py` & `tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/gs_client.py` & `tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/gs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gs-3.0.888/tencentcloud/gs/v20191118/models.py` & `tencentcloud-sdk-python-gs-3.0.889/tencentcloud/gs/v20191118/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param UserId: 唯一用户身份标识，由业务方自定义，平台不予理解。（可根据业务需要决定使用用户的唯一身份标识或是使用时间戳随机生成；在用户重连时应保持UserId不变）
         :type UserId: str
-        :param GameId: 游戏ID
+        :param GameId: 【已废弃】只在TrylockWorker时生效
         :type GameId: str
         :param GameRegion: 【已废弃】只在TrylockWorker时生效
         :type GameRegion: str
         :param GameParas: 游戏参数
         :type GameParas: str
         :param ClientSession: 客户端session信息，从JSSDK请求中获得。特殊的，当 RunMode 参数为 RunWithoutClient 时，该字段可以为空
         :type ClientSession: str
```

### Comparing `tencentcloud-sdk-python-gs-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gs-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gs-3.0.888/tencentcloud_sdk_python_gs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gs-3.0.889/tencentcloud_sdk_python_gs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gs
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Gs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gs-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-gs-3.0.889/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gs
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Gs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gs-3.0.888/setup.py` & `tencentcloud-sdk-python-gs-3.0.889/setup.py`

 * *Files identical despite different names*

