# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.888.tar", last modified: Wed May 10 02:03:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.889.tar", last modified: Thu May 11 02:37:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.888.tar` & `tencentcloud-sdk-python-cynosdb-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)    75124 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   276142 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:03:17.000000 tencentcloud-sdk-python-cynosdb-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)    77019 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)     9935 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   284224 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:37:52.000000 tencentcloud-sdk-python-cynosdb-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -781,14 +781,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeInstanceErrorLogs(self, request):
+        """查询实例错误日志列表
+
+        :param request: Request instance for DescribeInstanceErrorLogs.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceErrorLogsRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceErrorLogsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeInstanceErrorLogs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeInstanceErrorLogsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeInstanceSlowQueries(self, request):
         """此接口（DescribeInstanceSlowQueries）用于查询实例慢查询日志。
 
         :param request: Request instance for DescribeInstanceSlowQueries.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceSlowQueriesRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeInstanceSlowQueriesResponse`
 
@@ -1032,14 +1055,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ExportInstanceErrorLogs(self, request):
+        """此接口（ExportInstanceErrorLogs）用于导出实例错误日志。
+
+        :param request: Request instance for ExportInstanceErrorLogs.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.ExportInstanceErrorLogsRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ExportInstanceErrorLogsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ExportInstanceErrorLogs", params, headers=headers)
+            response = json.loads(body)
+            model = models.ExportInstanceErrorLogsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ExportInstanceSlowQueries(self, request):
         """此接口（ExportInstanceSlowQueries）用于导出实例慢日志。
 
         :param request: Request instance for ExportInstanceSlowQueries.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ExportInstanceSlowQueriesRequest`
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,17 @@
 
 # 未找到相关存储pool。
 INVALIDPARAMETERVALUE_STORAGEPOOLNOTFOUND = 'InvalidParameterValue.StoragePoolNotFound'
 
 # 找不到所选子网。
 INVALIDPARAMETERVALUE_SUBNETNOTFOUND = 'InvalidParameterValue.SubnetNotFound'
 
+# 未找到该数据。
+INVALIDPARAMETERVALUE_VALUENOTFOUND = 'InvalidParameterValue.ValueNotFound'
+
 # 找不到所选VPC网络。
 INVALIDPARAMETERVALUE_VPCNOTFOUND = 'InvalidParameterValue.VpcNotFound'
 
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
 # 集群中节点数超过最大限制。
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2000,14 +2000,49 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CynosdbErrorLogItem(AbstractModel):
+    """实例错误日志返回类型
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Timestamp: 日志时间戳
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Timestamp: int
+        :param Level: 日志等级
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Level: str
+        :param Content: 日志内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Content: str
+        """
+        self.Timestamp = None
+        self.Level = None
+        self.Content = None
+
+
+    def _deserialize(self, params):
+        self.Timestamp = params.get("Timestamp")
+        self.Level = params.get("Level")
+        self.Content = params.get("Content")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CynosdbInstance(AbstractModel):
     """实例信息
 
     """
 
     def __init__(self):
         r"""
@@ -4013,14 +4048,102 @@
     def _deserialize(self, params):
         if params.get("Detail") is not None:
             self.Detail = CynosdbInstanceDetail()
             self.Detail._deserialize(params.get("Detail"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeInstanceErrorLogsRequest(AbstractModel):
+    """DescribeInstanceErrorLogs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例Id
+        :type InstanceId: str
+        :param Limit: 日志条数限制
+        :type Limit: int
+        :param Offset: 日志条数偏移量
+        :type Offset: int
+        :param StartTime: 开始时间
+        :type StartTime: str
+        :param EndTime: 结束时间
+        :type EndTime: str
+        :param OrderBy: 排序字段，有Timestamp枚举值
+        :type OrderBy: str
+        :param OrderByType: 排序类型，有ASC,DESC枚举值
+        :type OrderByType: str
+        :param LogLevels: 日志等级，有error、warning、note三种，支持多个等级同时搜索
+        :type LogLevels: list of str
+        :param KeyWords: 关键字，支持模糊搜索
+        :type KeyWords: list of str
+        """
+        self.InstanceId = None
+        self.Limit = None
+        self.Offset = None
+        self.StartTime = None
+        self.EndTime = None
+        self.OrderBy = None
+        self.OrderByType = None
+        self.LogLevels = None
+        self.KeyWords = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.OrderBy = params.get("OrderBy")
+        self.OrderByType = params.get("OrderByType")
+        self.LogLevels = params.get("LogLevels")
+        self.KeyWords = params.get("KeyWords")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeInstanceErrorLogsResponse(AbstractModel):
+    """DescribeInstanceErrorLogs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 日志条数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param ErrorLogs: 错误日志列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ErrorLogs: list of CynosdbErrorLogItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.ErrorLogs = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("ErrorLogs") is not None:
+            self.ErrorLogs = []
+            for item in params.get("ErrorLogs"):
+                obj = CynosdbErrorLogItem()
+                obj._deserialize(item)
+                self.ErrorLogs.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeInstanceSlowQueriesRequest(AbstractModel):
     """DescribeInstanceSlowQueries请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4751,14 +4874,136 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ErrorLogItemExport(AbstractModel):
+    """错误日志导出格式
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Timestamp: 时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Timestamp: str
+        :param Level: 日志等级，可选值note, warning，error
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Level: str
+        :param Content: 日志内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Content: str
+        """
+        self.Timestamp = None
+        self.Level = None
+        self.Content = None
+
+
+    def _deserialize(self, params):
+        self.Timestamp = params.get("Timestamp")
+        self.Level = params.get("Level")
+        self.Content = params.get("Content")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ExportInstanceErrorLogsRequest(AbstractModel):
+    """ExportInstanceErrorLogs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param StartTime: 日志最早时间
+        :type StartTime: str
+        :param EndTime: 日志最晚时间
+        :type EndTime: str
+        :param Limit: 限制条数
+        :type Limit: int
+        :param Offset: 偏移量
+        :type Offset: int
+        :param LogLevels: 日志等级
+        :type LogLevels: list of str
+        :param KeyWords: 关键字
+        :type KeyWords: list of str
+        :param FileType: 文件类型，可选值：csv, original
+        :type FileType: str
+        :param OrderBy: 可选值Timestamp
+        :type OrderBy: str
+        :param OrderByType: ASC或DESC
+        :type OrderByType: str
+        """
+        self.InstanceId = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Limit = None
+        self.Offset = None
+        self.LogLevels = None
+        self.KeyWords = None
+        self.FileType = None
+        self.OrderBy = None
+        self.OrderByType = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.LogLevels = params.get("LogLevels")
+        self.KeyWords = params.get("KeyWords")
+        self.FileType = params.get("FileType")
+        self.OrderBy = params.get("OrderBy")
+        self.OrderByType = params.get("OrderByType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ExportInstanceErrorLogsResponse(AbstractModel):
+    """ExportInstanceErrorLogs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ErrorLogItems: 错误日志导出内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ErrorLogItems: list of ErrorLogItemExport
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ErrorLogItems = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("ErrorLogItems") is not None:
+            self.ErrorLogItems = []
+            for item in params.get("ErrorLogItems"):
+                obj = ErrorLogItemExport()
+                obj._deserialize(item)
+                self.ErrorLogItems.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class ExportInstanceSlowQueriesRequest(AbstractModel):
     """ExportInstanceSlowQueries请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.889/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.889/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.888/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.889/setup.py`

 * *Files identical despite different names*

