# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.888.tar", last modified: Wed May 10 02:01:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.889.tar", last modified: Thu May 11 02:28:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.888.tar` & `tencentcloud-sdk-python-ckafka-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)     3206 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   458707 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    68390 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:01:07.000000 tencentcloud-sdk-python-ckafka-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   460869 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    69267 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:28:49.000000 tencentcloud-sdk-python-ckafka-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5789,14 +5789,61 @@
     def _deserialize(self, params):
         if params.get("Result") is not None:
             self.Result = RouteResponse()
             self.Result._deserialize(params.get("Result"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeTaskStatusRequest(AbstractModel):
+    """DescribeTaskStatus请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 任务唯一标记
+        :type FlowId: int
+        """
+        self.FlowId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeTaskStatusResponse(AbstractModel):
+    """DescribeTaskStatus返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 返回结果
+        :type Result: :class:`tencentcloud.ckafka.v20190819.models.TaskStatusResponse`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Result") is not None:
+            self.Result = TaskStatusResponse()
+            self.Result._deserialize(params.get("Result"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeTopicAttributesRequest(AbstractModel):
     """DescribeTopicAttributes请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11429,14 +11476,46 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class TaskStatusResponse(AbstractModel):
+    """任务状态返回对象
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: 任务状态:
+0 成功
+1 失败
+2 进行中
+        :type Status: int
+        :param Output: 输出信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Output: str
+        """
+        self.Status = None
+        self.Output = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        self.Output = params.get("Output")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class TdwParam(AbstractModel):
     """Tdw类型入参
 
     """
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.889/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1241,14 +1241,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeTaskStatus(self, request):
+        """查询任务状态
+
+        :param request: Request instance for DescribeTaskStatus.
+        :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTaskStatusRequest`
+        :rtype: :class:`tencentcloud.ckafka.v20190819.models.DescribeTaskStatusResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeTaskStatus", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeTaskStatusResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeTopic(self, request):
         """接口请求域名：https://ckafka.tencentcloudapi.com
         本接口（DescribeTopic）用于在用户获取消息队列 CKafka 实例的主题列表
 
         :param request: Request instance for DescribeTopic.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicRequest`
         :rtype: :class:`tencentcloud.ckafka.v20190819.models.DescribeTopicResponse`
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.889/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.888/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.889/setup.py`

 * *Files identical despite different names*

