# Comparing `tmp/learning_pipeline_plugin-0.5.0.tar.gz` & `tmp/learning_pipeline_plugin-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning_pipeline_plugin-0.5.0.tar", max compression
+gzip compressed data, was "learning_pipeline_plugin-0.5.1.tar", max compression
```

## Comparing `learning_pipeline_plugin-0.5.0.tar` & `learning_pipeline_plugin-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2538 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/README.md
--rw-r--r--   0        0        0      164 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/__init__.py
--rw-r--r--   0        0        0     2242 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/actfw_utils.py
--rw-r--r--   0        0        0       90 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/__init__.py
--rw-r--r--   0        0        0     5857 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/stream_al.py
--rw-r--r--   0        0        0    10929 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_diversity.py
--rw-r--r--   0        0        0     2405 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_utils.py
--rw-r--r--   0        0        0      802 2023-05-02 23:32:59.183767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/type_helper.py
--rw-r--r--   0        0        0     2250 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/uncertainty.py
--rw-r--r--   0        0        0     3118 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/collect_pipe.py
--rw-r--r--   0        0        0      881 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/notifier.py
--rw-r--r--   0        0        0     3986 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/select_task.py
--rw-r--r--   0        0        0     7764 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/sender_task.py
--rw-r--r--   0        0        0      707 2023-05-02 23:32:59.187767 learning_pipeline_plugin-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/README.md
+-rw-r--r--   0        0        0      164 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/__init__.py
+-rw-r--r--   0        0        0     2242 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/actfw_utils.py
+-rw-r--r--   0        0        0       90 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/__init__.py
+-rw-r--r--   0        0        0     5857 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/stream_al.py
+-rw-r--r--   0        0        0    10929 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_diversity.py
+-rw-r--r--   0        0        0     2405 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_utils.py
+-rw-r--r--   0        0        0      802 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/type_helper.py
+-rw-r--r--   0        0        0     2250 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/uncertainty.py
+-rw-r--r--   0        0        0     3118 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/collect_pipe.py
+-rw-r--r--   0        0        0      881 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/notifier.py
+-rw-r--r--   0        0        0     3986 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/select_task.py
+-rw-r--r--   0        0        0     9589 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/sender_task.py
+-rw-r--r--   0        0        0      707 2023-05-11 03:27:15.562446 learning_pipeline_plugin-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.5.1/PKG-INFO
```

### Comparing `learning_pipeline_plugin-0.5.0/README.md` & `learning_pipeline_plugin-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/actfw_utils.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/actfw_utils.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/stream_al.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/stream_al.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_diversity.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_diversity.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/submodular_utils.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/submodular_utils.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/type_helper.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/type_helper.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/algorithms/uncertainty.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/algorithms/uncertainty.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/collect_pipe.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/collect_pipe.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/notifier.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/notifier.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/select_task.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/select_task.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.0/learning_pipeline_plugin/sender_task.py` & `learning_pipeline_plugin-0.5.1/learning_pipeline_plugin/sender_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,81 @@
 import io
 import json
 import os
 import random
 import time
-from typing import Dict, Generic, Optional, Tuple, TypeVar, Union
+from typing import Dict, Generic, Optional, Tuple, Type, TypeVar, Union
 
 import requests
 from actfw_core.service_client import ServiceClient
 from PIL.Image import Image
+from typing_extensions import Protocol
 
 from .actfw_utils import IsolatedTask
 from .notifier import AbstractNotifier, NullNotifier
 
 T = TypeVar("T")
 UserMetadata = Dict[str, Union[str, int, float, bool]]
 DatedImage = Tuple[str, Image]
 
 
+class ServiceClientProtocol(Protocol):
+    def rs256(self, payload: bytes) -> str:
+        raise NotImplementedError
+
+
 class AbstractSenderTask(Generic[T], IsolatedTask[T]):
     def set_notifier(self, notifier: AbstractNotifier) -> None:
         raise NotImplementedError
 
     def _proc(self, data: T) -> None:
+        _ = self._sender_call(data)
+
+    def _sender_call(self, data: T) -> bool:
+        """Should return the boolean equal to the success of the operation.
+        Can be used by subclass to perform operations on success or failure
+        """
         raise NotImplementedError
 
 
-class SenderTask(AbstractSenderTask[DatedImage]):
+class AbstractSenderTaskGenericDated(Generic[T], AbstractSenderTask[T]):
+    ServiceClient: Type[ServiceClientProtocol] = ServiceClient
+
     def __init__(self,
                  pipeline_id: str,
                  metadata: Optional[UserMetadata] = None,
                  endpoint_root: str = "https://api.autolearner.actcast.io",
                  max_retries: int = 3,
                  backoff_time_base: float = 60.0,
                  inqueuesize: int = 0):
-        """Isolated task used to send data to the Learning pipeline servers.
+        """Abstract isolated task used to send data to the Learning pipeline servers.
+        A concrete subclass should implement the two static methods: `timestamp_from_data` and
+        `bytes_from_data`.
+
         - pipeline_id (str): ID of the pipeline to send data to (obtained after created a pipeline)
         - metadata (UserMetadata): JSON-like data that will be stored with the image
                                     (e.g. user may include here some act settings)
         - endpoint_root (str): endpoint root of the lp API server (https://....)
         - max_retries (int): Max number of retry attempts.
         - backoff_time_base (float): The delay time between retry attempts
           is defined by random(backoff_time_base * (2 ** i)) seconds.
         - inqueuesize (int): size of the sending queue (default: 0 (no limit))
 
         Use example:
         ```
-        st = SenderTask(pipeline_id)
+        st = MySenderTask(pipeline_id)
         app.register_task(st)
         st.set_notifier(my_notifier)
 
         ...
-        st.enqueue((time_stamp, image))
+        st.enqueue(my_data)
         ```
         """
         super().__init__(inqueuesize)
-        self.service_client = ServiceClient()
+        self.service_client = self.ServiceClient()
         self.endpoint_root = endpoint_root
         self.pipeline_id = pipeline_id
         self.notifier: AbstractNotifier = NullNotifier()
         self.user_metadata = {} if metadata is None else metadata
         self.device_token = None
         self.device_token_endpoint = os.path.join(endpoint_root, "device", "token")
         self.collect_requests_endpoint = os.path.join(endpoint_root, "collect", "requests")
@@ -66,14 +83,27 @@
         self.max_retries = max_retries
         assert backoff_time_base > 0
         self.backoff_time_base = backoff_time_base
 
     def set_notifier(self, notifier: AbstractNotifier) -> None:
         self.notifier = notifier
 
+    @staticmethod
+    def timestamp_from_data(data: T) -> str:
+        """Returns a ISO formated timestamp of the data.
+        """
+        raise NotImplementedError
+
+    @staticmethod
+    def bytes_from_data(data: T) -> bytes:
+        """Returns a bytes object corresponding to the data to be sent.
+        e.g. converts the image inside data to PNG format and returns its bytes.
+        """
+        raise NotImplementedError
+
     def backoff(self, attempt: int) -> None:
         assert attempt >= 0
         max_period = self.backoff_time_base * (2 ** attempt)
         t = random.random() * max_period
         time.sleep(t)
 
     def proxies_common(self) -> dict:
@@ -129,16 +159,17 @@
             self.device_token = device_token
             self.device_token_expires = time.time() + expires_in
         else:
             self.device_token = None
             failure_status = {"status_code": response.status_code, "text": response.text}
             self.notifier.notify(f"Failed to update Device Token. {failure_status}")
 
-    def send_image(self, data: DatedImage) -> bool:
-        def get_upload_url(timestamp: str) -> Optional[str]:
+    def send_image(self, data: T) -> bool:
+        def get_upload_url(data: T) -> Optional[str]:
+            timestamp = self.timestamp_from_data(data)
             response = requests.post(
                 self.collect_requests_endpoint,
                 json={
                     "timestamp": timestamp,
                     "act_id": os.environ.get("ACTCAST_ACT_ID"),
                     "user_data": json.dumps(self.user_metadata)
                 },
@@ -157,39 +188,38 @@
                     self.notifier.notify(f"Invalid API response. (endpoint: {self.collect_requests_endpoint})")
                     return None
             else:
                 failure_status = {"status_code": response.status_code, "text": response.text}
                 self.notifier.notify(f"Failed to get an upload url. {failure_status}")
                 return None
 
-        def upload_image(upload_url: str, image: Image) -> bool:
-            image_bytes = io.BytesIO()
-            image.save(image_bytes, format="PNG")
+        def upload_image(upload_url: str, data: T) -> bool:
+            image_bytes = self.bytes_from_data(data)
 
-            response = requests.put(upload_url, data=image_bytes.getvalue(), proxies=self.proxies_common())
+            response = requests.put(upload_url, data=image_bytes, proxies=self.proxies_common())
 
             if response.status_code == 200:
                 return True
             else:
                 failure_status = {"status_code": response.status_code, "text": response.text}
                 self.notifier.notify(f"Failed to upload an image to {upload_url} . {failure_status}")
                 return False
 
-        timestamp, image = data
-        upload_url = get_upload_url(timestamp)
+        upload_url = get_upload_url(data)
 
         if upload_url is None:
             return False
 
-        return upload_image(upload_url, image)
+        return upload_image(upload_url, data)
 
-    def _proc(self, data: DatedImage) -> None:
+    def _sender_call(self, data: T) -> bool:
         if not self.has_valid_params():
-            return
+            return False
 
+        success = False
         for i in range(self.max_retries):
             if not self.has_valid_token():
                 self.update_token()
 
                 if not self.has_valid_token():
                     self.backoff(i)
                     continue
@@ -199,7 +229,35 @@
             if success:
                 break
 
             self.backoff(i)
 
         result = "Success" if success else "Failure"
         self.notifier.notify(f"SenderTask Result: {result}")
+        return success
+
+
+class SenderTask(AbstractSenderTaskGenericDated[DatedImage]):
+    """Isolated task to send data in format (timestamp, image),
+    where timestamp is a ISO formatted string, and image a pillow image.
+    See super class docstring for more informations.
+
+    Use example:
+    ```
+    st = SenderTask(pipeline_id)
+    app.register_task(st)
+    st.set_notifier(my_notifier)
+
+    ...
+    st.enqueue((time_stamp, image))
+    """
+    @staticmethod
+    def bytes_from_data(data: DatedImage) -> bytes:
+        _, image = data
+        image_bytes_io = io.BytesIO()
+        image.save(image_bytes_io, format="PNG")
+        return image_bytes_io.getvalue()
+
+    @staticmethod
+    def timestamp_from_data(data: DatedImage) -> str:
+        timestamp, _ = data
+        return timestamp
```

### Comparing `learning_pipeline_plugin-0.5.0/pyproject.toml` & `learning_pipeline_plugin-0.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "learning-pipeline-plugin"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Idein Inc."]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "learning_pipeline_plugin"}]
 repository = "https://github.com/Idein/learning-pipeline-plugin"
```

### Comparing `learning_pipeline_plugin-0.5.0/PKG-INFO` & `learning_pipeline_plugin-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning-pipeline-plugin
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Home-page: https://github.com/Idein/learning-pipeline-plugin
 License: MIT
 Author: Idein Inc.
 Requires-Python: >=3.7.0,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

