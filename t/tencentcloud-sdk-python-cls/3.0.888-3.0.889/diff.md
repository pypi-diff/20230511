# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.888.tar", last modified: Wed May 10 02:01:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.889.tar", last modified: Thu May 11 02:29:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.888.tar` & `tencentcloud-sdk-python-cls-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   253451 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67925 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:01:46.000000 tencentcloud-sdk-python-cls-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   253720 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67925 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-11 02:29:27.000000 tencentcloud-sdk-python-cls-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 02:29:28.000000 tencentcloud-sdk-python-cls-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.888/README.rst` & `tencentcloud-sdk-python-cls-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4794,22 +4794,27 @@
     def __init__(self):
         r"""
         :param EnableTag: 启用标志
         :type EnableTag: bool
         :param MetaFields: 元数据信息列表, 可选值为 __SOURCE__、__FILENAME__、__TIMESTAMP__、__HOSTNAME__。
 注意：此字段可能返回 null，表示取不到有效值。
         :type MetaFields: list of str
+        :param JsonType: 投递Json格式，0：字符串方式投递；1:以结构化方式投递
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JsonType: int
         """
         self.EnableTag = None
         self.MetaFields = None
+        self.JsonType = None
 
 
     def _deserialize(self, params):
         self.EnableTag = params.get("EnableTag")
         self.MetaFields = params.get("MetaFields")
+        self.JsonType = params.get("JsonType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.889/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.888/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.889/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.889/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.888/setup.py` & `tencentcloud-sdk-python-cls-3.0.889/setup.py`

 * *Files identical despite different names*

