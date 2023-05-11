# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.888.tar", last modified: Wed May 10 02:59:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.889.tar", last modified: Thu May 11 03:28:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.888.tar` & `tencentcloud-sdk-python-vpc-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   328827 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41072 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   839291 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:59:40.000000 tencentcloud-sdk-python-vpc-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   328827 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41072 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   839372 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:28:44.000000 tencentcloud-sdk-python-vpc-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/README.rst` & `tencentcloud-sdk-python-vpc-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -21088,14 +21088,15 @@
 HAVIP：高可用虚拟IP；
 NAT：NAT网关; 
 NORMAL_CVM：普通云服务器；
 EIP：云服务器的公网IP；
 LOCAL_GATEWAY：本地网关。
         :type GatewayType: str
         :param GatewayId: 下一跳地址，这里只需要指定不同下一跳类型的网关ID，系统会自动匹配到下一跳地址。
+特殊说明：GatewayType为NORMAL_CVM时，GatewayId填写实例的内网IP。
         :type GatewayId: str
         :param RouteId: 路由策略ID。IPv4路由策略ID是有意义的值，IPv6路由策略是无意义的值0。后续建议完全使用字符串唯一ID `RouteItemId`操作路由策略。
 该字段在删除时必填，其他字段无需填写。
         :type RouteId: int
         :param RouteDescription: 路由策略描述。
         :type RouteDescription: str
         :param Enabled: 是否启用
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.889/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.888/setup.py` & `tencentcloud-sdk-python-vpc-3.0.889/setup.py`

 * *Files identical despite different names*

