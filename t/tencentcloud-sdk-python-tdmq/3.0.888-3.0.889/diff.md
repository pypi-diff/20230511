# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.888.tar", last modified: Wed May 10 02:53:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.889.tar", last modified: Thu May 11 03:19:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.888.tar` & `tencentcloud-sdk-python-tdmq-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   102882 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   379845 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:53:05.000000 tencentcloud-sdk-python-tdmq-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   102882 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   379845 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:19:16.000000 tencentcloud-sdk-python-tdmq-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/tdmq/v20200217/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6394,55 +6394,55 @@
 
     """
 
     def __init__(self):
         r"""
         :param EnvironmentId: 环境（命名空间）名称。
         :type EnvironmentId: str
+        :param ClusterId: Pulsar 集群的ID
+        :type ClusterId: str
         :param TopicName: 主题名模糊匹配。
         :type TopicName: str
         :param Offset: 起始下标，不填默认为0。
         :type Offset: int
         :param Limit: 返回数量，不填则默认为10，最大值为20。
         :type Limit: int
         :param TopicType: topic类型描述：
 0：非持久非分区主题类型；
 1：非持久分区主题类型；
 2：持久非分区主题类型；
 3：持久分区主题类型；
         :type TopicType: int
-        :param ClusterId: Pulsar 集群的ID
-        :type ClusterId: str
         :param Filters: * TopicName
 按照主题名字查询，精确查询。
 类型：String
 必选：否
         :type Filters: list of Filter
         :param TopicCreator: 创建来源：
 1：用户创建
 2：系统创建
         :type TopicCreator: int
         """
         self.EnvironmentId = None
+        self.ClusterId = None
         self.TopicName = None
         self.Offset = None
         self.Limit = None
         self.TopicType = None
-        self.ClusterId = None
         self.Filters = None
         self.TopicCreator = None
 
 
     def _deserialize(self, params):
         self.EnvironmentId = params.get("EnvironmentId")
+        self.ClusterId = params.get("ClusterId")
         self.TopicName = params.get("TopicName")
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.TopicType = params.get("TopicType")
-        self.ClusterId = params.get("ClusterId")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
         self.TopicCreator = params.get("TopicCreator")
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.889/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.889/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.888/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.889/setup.py`

 * *Files identical despite different names*

