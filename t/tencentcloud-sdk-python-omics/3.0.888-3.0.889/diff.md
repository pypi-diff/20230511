# Comparing `tmp/tencentcloud-sdk-python-omics-3.0.888.tar.gz` & `tmp/tencentcloud-sdk-python-omics-3.0.889.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.888.tar", last modified: Wed May 10 02:24:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-omics-3.0.889.tar", last modified: Thu May 11 03:07:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-omics-3.0.888.tar` & `tencentcloud-sdk-python-omics-3.0.889.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud_sdk_python_omics.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud_sdk_python_omics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/
--rw-r--r--   0 root         (0) root         (0)     8751 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/omics_client.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45721 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-10 02:24:31.000000 tencentcloud-sdk-python-omics-3.0.888/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/
+-rw-r--r--   0 root         (0) root         (0)     8751 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/omics_client.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46322 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-11 03:07:40.000000 tencentcloud-sdk-python-omics-3.0.889/setup.cfg
```

### Comparing `tencentcloud-sdk-python-omics-3.0.888/README.rst` & `tencentcloud-sdk-python-omics-3.0.889/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.888/tencentcloud_sdk_python_omics.egg-info/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.889/tencentcloud_sdk_python_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/omics_client.py` & `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/omics_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/errorcodes.py` & `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-omics-3.0.888/tencentcloud/omics/v20221128/models.py` & `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/omics/v20221128/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1260,24 +1260,34 @@
 - ContinueWhilePossible
 - NoNewCalls
         :type FailureMode: str
         :param UseCallCache: 是否使用Call-Caching功能。
         :type UseCallCache: bool
         :param UseErrorOnHold: 是否使用错误挂起功能。
         :type UseErrorOnHold: bool
+        :param FinalWorkflowOutputsDir: 输出归档COS路径。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FinalWorkflowOutputsDir: str
+        :param UseRelativeOutputPaths: 是否使用相对目录归档输出。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UseRelativeOutputPaths: bool
         """
         self.FailureMode = None
         self.UseCallCache = None
         self.UseErrorOnHold = None
+        self.FinalWorkflowOutputsDir = None
+        self.UseRelativeOutputPaths = None
 
 
     def _deserialize(self, params):
         self.FailureMode = params.get("FailureMode")
         self.UseCallCache = params.get("UseCallCache")
         self.UseErrorOnHold = params.get("UseErrorOnHold")
+        self.FinalWorkflowOutputsDir = params.get("FinalWorkflowOutputsDir")
+        self.UseRelativeOutputPaths = params.get("UseRelativeOutputPaths")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-omics-3.0.888/tencentcloud/__init__.py` & `tencentcloud-sdk-python-omics-3.0.889/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-omics-3.0.888/PKG-INFO` & `tencentcloud-sdk-python-omics-3.0.889/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-omics
-Version: 3.0.888
+Version: 3.0.889
 Summary: Tencent Cloud Omics SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-omics-3.0.888/setup.py` & `tencentcloud-sdk-python-omics-3.0.889/setup.py`

 * *Files identical despite different names*

