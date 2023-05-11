# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.888.tar", last modified: Wed May 10 02:58:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.889.tar", last modified: Thu May 11 03:27:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.888.tar` & `tencentcloud-sdk-python-trtc-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   199052 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58535 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-10 02:58:31.000000 tencentcloud-sdk-python-trtc-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:58:32.000000 tencentcloud-sdk-python-trtc-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198994 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58535 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:27:17.000000 tencentcloud-sdk-python-trtc-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/README.rst` & `tencentcloud-sdk-python-trtc-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         :type RoomIdType: int
         :param MixTranscodeParams: 混流的转码参数，录制模式为混流的时候可以设置。
         :type MixTranscodeParams: :class:`tencentcloud.trtc.v20190722.models.MixTranscodeParams`
         :param MixLayoutParams: 混流的布局参数，录制模式为混流的时候可以设置。
         :type MixLayoutParams: :class:`tencentcloud.trtc.v20190722.models.MixLayoutParams`
         :param ResourceExpiredHour: 接口可以调用的时效性，从成功开启录制并获得任务ID后开始计算，超时后无法调用查询、更新和停止等接口，但是录制任务不会停止。 参数的单位是小时，默认72小时（3天），最大可设置720小时（30天），最小设置6小时。举例说明：如果不设置该参数，那么开始录制成功后，查询、更新和停止录制的调用时效为72个小时。
         :type ResourceExpiredHour: int
-        :param PrivateMapKey: TRTC房间权限加密串，只有在TRTC控制台启用了高级权限控制的时候需要携带，在TRTC控制台如果开启高级权限控制后，TRTC 的后台服务系统会校验一个叫做 [PrivateMapKey]（https://cloud.tencent.com/document/product/647/32240） 的“权限票据”，权限票据中包含了一个加密后的 RoomId 和一个加密后的“权限位列表”。由于 PrivateMapKey 中包含 RoomId，所以只提供了 UserSig 没有提供 PrivateMapKey 时，并不能进入指定的房间。
+        :param PrivateMapKey: TRTC房间权限加密串，只有在TRTC控制台启用了高级权限控制的时候需要携带，在TRTC控制台如果开启高级权限控制后，TRTC 的后台服务系统会校验一个叫做 [PrivateMapKey] 的“权限票据”，权限票据中包含了一个加密后的 RoomId 和一个加密后的“权限位列表”。由于 PrivateMapKey 中包含 RoomId，所以只提供了 UserSig 没有提供 PrivateMapKey 时，并不能进入指定的房间。
         :type PrivateMapKey: str
         """
         self.SdkAppId = None
         self.RoomId = None
         self.UserId = None
         self.UserSig = None
         self.RecordParams = None
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.889/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.889/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.888/setup.py` & `tencentcloud-sdk-python-trtc-3.0.889/setup.py`

 * *Files identical despite different names*

