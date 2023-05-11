# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.888.tar", last modified: Wed May 10 02:58:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.889.tar", last modified: Thu May 11 03:27:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.888.tar` & `tencentcloud-sdk-python-tsf-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49713 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   193599 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   798817 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:58:49.000000 tencentcloud-sdk-python-tsf-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    49713 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   194455 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   800128 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:27:41.000000 tencentcloud-sdk-python-tsf-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:27:42.000000 tencentcloud-sdk-python-tsf-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/README.rst` & `tencentcloud-sdk-python-tsf-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1057,14 +1057,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteGatewayApi(self, request):
+        """批量删除API
+
+        :param request: Request instance for DeleteGatewayApi.
+        :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteGatewayApiRequest`
+        :rtype: :class:`tencentcloud.tsf.v20180326.models.DeleteGatewayApiResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteGatewayApi", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteGatewayApiResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteGroup(self, request):
         """删除容器部署组
 
         :param request: Request instance for DeleteGroup.
         :type request: :class:`tencentcloud.tsf.v20180326.models.DeleteGroupRequest`
         :rtype: :class:`tencentcloud.tsf.v20180326.models.DeleteGroupResponse`
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/tsf/v20180326/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5601,14 +5601,63 @@
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.RequestId = params.get("RequestId")
 
 
+class DeleteGatewayApiRequest(AbstractModel):
+    """DeleteGatewayApi请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GroupId: 分组ID
+        :type GroupId: str
+        :param ApiList: Api ID 数组
+        :type ApiList: list of str
+        """
+        self.GroupId = None
+        self.ApiList = None
+
+
+    def _deserialize(self, params):
+        self.GroupId = params.get("GroupId")
+        self.ApiList = params.get("ApiList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteGatewayApiResponse(AbstractModel):
+    """DeleteGatewayApi返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 是否成功
+        :type Result: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Result = params.get("Result")
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteGroupRequest(AbstractModel):
     """DeleteGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.889/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.889/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.888/setup.py` & `tencentcloud-sdk-python-tsf-3.0.889/setup.py`

 * *Files identical despite different names*

