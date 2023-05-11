# Comparing `tmp/tencentcloud-sdk-python-es-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-es-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.888.tar", last modified: Wed May 10 02:13:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.889.tar", last modified: Thu May 11 02:49:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-es-3.0.888.tar` & `tencentcloud-sdk-python-es-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      734 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/
--rw-r--r--   0 root         (0) root         (0)    35037 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/es_client.py
--rw-r--r--   0 root         (0) root         (0)     3332 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177567 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud_sdk_python_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud_sdk_python_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/tencentcloud_sdk_python_es.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:13:17.000000 tencentcloud-sdk-python-es-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      734 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    35037 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/es_client.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   177851 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud_sdk_python_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud_sdk_python_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/tencentcloud_sdk_python_es.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-11 02:49:39.000000 tencentcloud-sdk-python-es-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:49:40.000000 tencentcloud-sdk-python-es-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-es-3.0.888/README.rst` & `tencentcloud-sdk-python-es-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/es_client.py` & `tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/es_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/errorcodes.py` & `tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.888/tencentcloud/es/v20180416/models.py` & `tencentcloud-sdk-python-es-3.0.889/tencentcloud/es/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2528,26 +2528,30 @@
         :type Time: str
         :param Level: 日志级别
         :type Level: str
         :param Ip: 集群节点ip
         :type Ip: str
         :param Message: 日志内容
         :type Message: str
+        :param NodeID: 集群节点ID
+        :type NodeID: str
         """
         self.Time = None
         self.Level = None
         self.Ip = None
         self.Message = None
+        self.NodeID = None
 
 
     def _deserialize(self, params):
         self.Time = params.get("Time")
         self.Level = params.get("Level")
         self.Ip = params.get("Ip")
         self.Message = params.get("Message")
+        self.NodeID = params.get("NodeID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2644,34 +2648,38 @@
         :type MemUsage: float
         :param CpuNum: 节点cpu个数
         :type CpuNum: int
         :param CpuUsage: cpu使用率
         :type CpuUsage: float
         :param Zone: 可用区
         :type Zone: str
+        :param NodeId: ts-0noqayxu-az6-hot-03222010-0
+        :type NodeId: str
         """
         self.Ip = None
         self.DiskSize = None
         self.DiskUsage = None
         self.MemSize = None
         self.MemUsage = None
         self.CpuNum = None
         self.CpuUsage = None
         self.Zone = None
+        self.NodeId = None
 
 
     def _deserialize(self, params):
         self.Ip = params.get("Ip")
         self.DiskSize = params.get("DiskSize")
         self.DiskUsage = params.get("DiskUsage")
         self.MemSize = params.get("MemSize")
         self.MemUsage = params.get("MemUsage")
         self.CpuNum = params.get("CpuNum")
         self.CpuUsage = params.get("CpuUsage")
         self.Zone = params.get("Zone")
+        self.NodeId = params.get("NodeId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-es-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-es-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-es-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.889/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.888/tencentcloud_sdk_python_es.egg-info/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.889/tencentcloud_sdk_python_es.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.888/setup.py` & `tencentcloud-sdk-python-es-3.0.889/setup.py`

 * *Files identical despite different names*

