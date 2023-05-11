# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.887.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.887.tar", last modified: Tue May  9 03:11:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.889.tar", last modified: Thu May 11 03:08:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.887.tar` & `tencentcloud-sdk-python-redis-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86832 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   295067 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:11:49.000000 tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86880 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   295489 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:08:47.000000 tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.887/README.rst` & `tencentcloud-sdk-python-redis-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -851,15 +851,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceNodeInfo(self, request):
-        """查询实例节点信息
+        """本接口（DescribeInstanceNodeInfo）用于查询实例节点信息。
 
         :param request: Request instance for DescribeInstanceNodeInfo.
         :type request: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceNodeInfoRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.DescribeInstanceNodeInfoResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2637,19 +2637,19 @@
 class DescribeInstanceNodeInfoRequest(AbstractModel):
     """DescribeInstanceNodeInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param Limit: 列表大小
+        :param Limit: 列表大小。每页输出的节点信息大小。默认为 20，最多输出1000条。该字段已不再使用，请忽略。
         :type Limit: int
-        :param Offset: 偏移量
+        :param Offset: 分页偏移量，取Limit整数倍。计算公式：offset=limit*(页码-1)。该字段已不再使用，请忽略。
         :type Offset: int
         """
         self.InstanceId = None
         self.Limit = None
         self.Offset = None
 
 
@@ -2669,27 +2669,27 @@
 class DescribeInstanceNodeInfoResponse(AbstractModel):
     """DescribeInstanceNodeInfo返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ProxyCount: proxy节点数量
+        :param ProxyCount: Proxy节点数量。
         :type ProxyCount: int
-        :param Proxy: proxy节点信息
+        :param Proxy: Proxy节点信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Proxy: list of ProxyNodes
-        :param RedisCount: redis节点数量
+        :param RedisCount: Redis节点数量。
         :type RedisCount: int
-        :param Redis: redis节点信息
+        :param Redis: Redis节点信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Redis: list of RedisNodes
-        :param TendisCount: tendis节点数量
+        :param TendisCount: 该参数不再使用，请忽略。
         :type TendisCount: int
-        :param Tendis: tendis节点信息
+        :param Tendis: 该参数不再使用，请忽略。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tendis: list of TendisNodes
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.ProxyCount = None
         self.Proxy = None
@@ -7139,21 +7139,21 @@
 class RedisNodes(AbstractModel):
     """Redis节点信息
 
     """
 
     def __init__(self):
         r"""
-        :param NodeId: 节点ID
+        :param NodeId: 节点 ID。
         :type NodeId: str
-        :param NodeRole: 节点角色
+        :param NodeRole: 节点角色。
         :type NodeRole: str
-        :param ClusterId: 分片ID
+        :param ClusterId: 分片 ID。
         :type ClusterId: int
-        :param ZoneId: 可用区ID
+        :param ZoneId: 可用区 ID。
         :type ZoneId: int
         """
         self.NodeId = None
         self.NodeRole = None
         self.ClusterId = None
         self.ZoneId = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.887/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.887/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.889/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.887
+Version: 3.0.889
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.887/setup.py` & `tencentcloud-sdk-python-redis-3.0.889/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.887/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.889/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.887
+Version: 3.0.889
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

