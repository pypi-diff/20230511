# Comparing `tmp/tencentcloud-sdk-python-cbs-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-cbs-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.888.tar", last modified: Wed May 10 01:53:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.889.tar", last modified: Thu May 11 02:24:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cbs-3.0.888.tar` & `tencentcloud-sdk-python-cbs-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud_sdk_python_cbs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)     7755 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53378 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   159212 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 01:53:19.000000 tencentcloud-sdk-python-cbs-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud_sdk_python_cbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53328 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   159290 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:24:10.000000 tencentcloud-sdk-python-cbs-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.889/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/README.rst` & `tencentcloud-sdk-python-cbs-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -902,19 +902,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyDisksChargeType(self, request):
-        """接口请求域名： cbs.tencentcloudapi.com 。
+        """本接口 (ModifyDisksChargeType) 用于切换云硬盘的计费模式。
 
-        本接口 (ModifyDisksChargeType) 用于切换云盘的计费模式。
-
-        非弹性云盘不支持此接口，请通过修改实例计费模式接口将实例连同非弹性云盘一起转换。
+        非弹性云硬盘不支持此接口，请通过修改实例计费模式接口将实例连同非弹性云硬盘一起转换。
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for ModifyDisksChargeType.
         :type request: :class:`tencentcloud.cbs.v20170312.models.ModifyDisksChargeTypeRequest`
         :rtype: :class:`tencentcloud.cbs.v20170312.models.ModifyDisksChargeTypeResponse`
 
         """
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-cbs-3.0.889/tencentcloud/cbs/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,14 +803,15 @@
     """CreateDisks返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param DiskIdSet: 创建的云硬盘ID列表。
+注意：此字段可能返回 null，表示取不到有效值。
         :type DiskIdSet: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DiskIdSet = None
         self.RequestId = None
 
@@ -2981,15 +2982,15 @@
 class ModifyDisksChargeTypeRequest(AbstractModel):
     """ModifyDisksChargeType请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DiskIds: 一个或多个待操作的云硬盘ID。每次请求批量云盘上限为100。
+        :param DiskIds: 一个或多个待操作的云硬盘ID。每次请求批量云硬盘上限为100。
         :type DiskIds: list of str
         :param DiskChargePrepaid: 设置为预付费模式，即包年包月相关参数设置。通过该参数可以指定包年包月实例的购买时长、是否设置自动续费等属性。
         :type DiskChargePrepaid: :class:`tencentcloud.cbs.v20170312.models.DiskChargePrepaid`
         :param DiskChargePostpaid: 设置为后付费模式
         :type DiskChargePostpaid: bool
         """
         self.DiskIds = None
@@ -3130,30 +3131,30 @@
 class ModifySnapshotsSharePermissionRequest(AbstractModel):
     """ModifySnapshotsSharePermission请求参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param SnapshotIds: 快照ID, 可通过[DescribeSnapshots](https://cloud.tencent.com/document/api/362/15647)查询获取。
+        :type SnapshotIds: list of str
         :param AccountIds: 接收分享快照的账号Id列表，array型参数的格式可以参考[API简介](https://cloud.tencent.com/document/api/213/568)。帐号ID不同于QQ号，查询用户帐号ID请查看[帐号信息](https://console.cloud.tencent.com/developer)中的帐号ID栏。
         :type AccountIds: list of str
         :param Permission: 操作，包括 SHARE，CANCEL。其中SHARE代表分享操作，CANCEL代表取消分享操作。
         :type Permission: str
-        :param SnapshotIds: 快照ID, 可通过[DescribeSnapshots](https://cloud.tencent.com/document/api/362/15647)查询获取。
-        :type SnapshotIds: list of str
         """
+        self.SnapshotIds = None
         self.AccountIds = None
         self.Permission = None
-        self.SnapshotIds = None
 
 
     def _deserialize(self, params):
+        self.SnapshotIds = params.get("SnapshotIds")
         self.AccountIds = params.get("AccountIds")
         self.Permission = params.get("Permission")
-        self.SnapshotIds = params.get("SnapshotIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3407,15 +3408,15 @@
 class RenewDiskRequest(AbstractModel):
     """RenewDisk请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DiskChargePrepaid: 预付费模式，即包年包月相关参数设置。通过该参数可以指定包年包月云盘的续费时长。<br>在云盘与挂载的实例一起续费的场景下，可以指定参数CurInstanceDeadline，此时云盘会按对齐到实例续费后的到期时间来续费。
+        :param DiskChargePrepaid: 预付费模式，即包年包月相关参数设置。通过该参数可以指定包年包月云硬盘的续费时长。<br>在云硬盘与挂载的实例一起续费的场景下，可以指定参数CurInstanceDeadline，此时云硬盘会按对齐到实例续费后的到期时间来续费。
         :type DiskChargePrepaid: :class:`tencentcloud.cbs.v20170312.models.DiskChargePrepaid`
         :param DiskId: 云硬盘ID， 通过[DescribeDisks](/document/product/362/16315)接口查询。
         :type DiskId: str
         """
         self.DiskChargePrepaid = None
         self.DiskId = None
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.889/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.888/setup.py` & `tencentcloud-sdk-python-cbs-3.0.889/setup.py`

 * *Files identical despite different names*

