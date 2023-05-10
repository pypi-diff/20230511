# Comparing `tmp/armada_airflow-0.3.0-py3-none-any.whl.zip` & `tmp/armada_airflow-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 18490 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 00:07 armada/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 00:10 armada/jobservice/__init__.py
--rw-r--r--  2.0 unx     2728 b- defN 23-Apr-25 00:10 armada/jobservice/jobservice_pb2.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Apr-25 00:10 armada/jobservice/jobservice_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 00:07 armada/operators/__init__.py
--rw-r--r--  2.0 unx     4579 b- defN 23-Apr-25 00:07 armada/operators/armada.py
--rw-r--r--  2.0 unx    11285 b- defN 23-Apr-25 00:07 armada/operators/armada_deferrable.py
--rw-r--r--  2.0 unx     1384 b- defN 23-Apr-25 00:07 armada/operators/jobservice.py
--rw-r--r--  2.0 unx     1542 b- defN 23-Apr-25 00:07 armada/operators/jobservice_asyncio.py
--rw-r--r--  2.0 unx     9976 b- defN 23-Apr-25 00:07 armada/operators/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3769 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1289 b- defN 23-Apr-25 00:14 armada_airflow-0.3.0.dist-info/RECORD
-15 files, 52130 bytes uncompressed, 16328 bytes compressed:  68.7%
+Zip file size: 18725 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-May-10 23:13 armada/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-10 23:18 armada/jobservice/__init__.py
+-rw-r--r--  2.0 unx     2728 b- defN 23-May-10 23:18 armada/jobservice/jobservice_pb2.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-May-10 23:18 armada/jobservice/jobservice_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-10 23:13 armada/operators/__init__.py
+-rw-r--r--  2.0 unx     4869 b- defN 23-May-10 23:13 armada/operators/armada.py
+-rw-r--r--  2.0 unx    11756 b- defN 23-May-10 23:13 armada/operators/armada_deferrable.py
+-rw-r--r--  2.0 unx     1384 b- defN 23-May-10 23:13 armada/operators/jobservice.py
+-rw-r--r--  2.0 unx     1542 b- defN 23-May-10 23:13 armada/operators/jobservice_asyncio.py
+-rw-r--r--  2.0 unx    10090 b- defN 23-May-10 23:13 armada/operators/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3769 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1290 b- defN 23-May-10 23:24 armada_airflow-0.4.0.dist-info/RECORD
+15 files, 53006 bytes uncompressed, 16563 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: armada/operators/jobservice_asyncio.py
 Comment: 
 
 Filename: armada/operators/utils.py
 Comment: 
 
-Filename: armada_airflow-0.3.0.dist-info/LICENSE
+Filename: armada_airflow-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: armada_airflow-0.3.0.dist-info/METADATA
+Filename: armada_airflow-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: armada_airflow-0.3.0.dist-info/WHEEL
+Filename: armada_airflow-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: armada_airflow-0.3.0.dist-info/top_level.txt
+Filename: armada_airflow-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: armada_airflow-0.3.0.dist-info/RECORD
+Filename: armada_airflow-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armada/operators/armada.py

```diff
@@ -13,22 +13,23 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import logging
-from typing import Optional
+from typing import Optional, List
 
 from airflow.models import BaseOperator
 from airflow.exceptions import AirflowException
 
+from armada_client.armada.submit_pb2 import JobSubmitRequestItem
 from armada_client.client import ArmadaClient
-from armada.operators.jobservice import JobServiceClient
 
+from armada.operators.jobservice import JobServiceClient
 from armada.operators.utils import (
     airflow_error,
     search_for_job_complete,
     annotate_job_request_items,
 )
 from armada.jobservice import jobservice_pb2
 
@@ -49,35 +50,37 @@
     :param armada_queue: The queue name for Armada.
     :param job_request_items: A PodSpec that is used by Armada for submitting a job
     :param lookout_url_template: A URL template to be used to provide users
         a valid link to the related lookout job in this operator's log.
         The format should be:
         "https://lookout.armada.domain/jobs?job_id=<job_id>" where <job_id> will
         be replaced with the actual job ID.
-
+    :param poll_interval: How often to poll jobservice to get status.
     :return: an armada operator instance
     """
 
     def __init__(
         self,
         name: str,
         armada_client: ArmadaClient,
         job_service_client: JobServiceClient,
         armada_queue: str,
-        job_request_items,
+        job_request_items: List[JobSubmitRequestItem],
         lookout_url_template: Optional[str] = None,
+        poll_interval: int = 30,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.name = name
         self.armada_client = armada_client
         self.job_service = job_service_client
         self.armada_queue = armada_queue
         self.job_request_items = job_request_items
         self.lookout_url_template = lookout_url_template
+        self.poll_interval = poll_interval
 
     def execute(self, context) -> None:
         """
         Executes the Armada Operator.
 
         Runs an Armada job and calls the job_service_client for polling.
 
@@ -113,14 +116,15 @@
 
         job_state, job_message = search_for_job_complete(
             job_service_client=self.job_service,
             armada_queue=self.armada_queue,
             job_set_id=job_set_id,
             airflow_task_name=self.name,
             job_id=job_id,
+            poll_interval=self.poll_interval,
         )
         armada_logger.info(
             "Armada Job finished with %s and message: %s", job_state, job_message
         )
         airflow_error(job_state, self.name, job_id)
 
     def _get_lookout_url(self, job_id: str) -> str:
```

## armada/operators/armada_deferrable.py

```diff
@@ -13,37 +13,49 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import logging
-from typing import Optional, Sequence, Tuple, Any
+from typing import Optional, Sequence, Tuple, Any, TypedDict, List
 
 import grpc
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
+from armada_client.armada.submit_pb2 import JobSubmitRequestItem
 from armada_client.client import ArmadaClient
+
 from armada.operators.jobservice import JobServiceClient
 from armada.operators.jobservice_asyncio import JobServiceAsyncIOClient
-
 from armada.operators.utils import (
     airflow_error,
     search_for_job_complete_async,
     annotate_job_request_items,
 )
 from armada.jobservice import jobservice_pb2
 
 
 armada_logger = logging.getLogger("airflow.task")
 
 
+class GrpcChannelArgsDict(TypedDict):
+    """
+    Helper class to provide stronger type checking on Grpc channel arugments.
+    """
+
+    target: str
+    credentials: Optional[grpc.ChannelCredentials] = None
+    options: Optional[Sequence[Tuple[str, Any]]] = None
+    compression: Optional[grpc.Compression] = None
+
+
 class ArmadaDeferrableOperator(BaseOperator):
     """
     Implementation of a deferrable armada operator for airflow.
 
     Distinguished from ArmadaOperator by its ability to defer itself after
     submitting its job_request_items.
 
@@ -67,18 +79,18 @@
 
     :return: A deferrable armada operator instance.
     """  # noqa
 
     def __init__(
         self,
         name: str,
-        armada_channel_args: dict,
-        job_service_channel_args: dict,
+        armada_channel_args: GrpcChannelArgsDict,
+        job_service_channel_args: GrpcChannelArgsDict,
         armada_queue: str,
-        job_request_items,
+        job_request_items: List[JobSubmitRequestItem],
         lookout_url_template: Optional[str] = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.name = name
         self.armada_channel_args = GrpcChannelArguments(**armada_channel_args)
         self.job_service_channel_args = GrpcChannelArguments(**job_service_channel_args)
@@ -189,15 +201,15 @@
 
     :returns: An armada job complete trigger instance.
     """
 
     def __init__(
         self,
         job_id: str,
-        job_service_channel_args: dict,
+        job_service_channel_args: GrpcChannelArgsDict,
         armada_queue: str,
         job_set_id: str,
         airflow_task_name: str,
     ) -> None:
         super().__init__()
         self.job_id = job_id
         self.job_service_channel_args = GrpcChannelArguments(**job_service_channel_args)
```

## armada/operators/utils.py

```diff
@@ -79,27 +79,29 @@
 
 
 def search_for_job_complete(
     armada_queue: str,
     job_set_id: str,
     airflow_task_name: str,
     job_id: str,
+    poll_interval: int = 30,
     job_service_client: Optional[JobServiceClient] = None,
     job_status_callable=default_job_status_callable,
     time_out_for_failure: int = 7200,
 ) -> Tuple[JobState, str]:
     """
 
     Poll JobService cache until you get a terminated event.
 
     A terminated event is SUCCEEDED, FAILED or CANCELLED
 
     :param armada_queue: The queue for armada
     :param job_set_id: Your job_set_id
     :param airflow_task_name: The name of your armada job
+    :param poll_interval: Polling interval for jobservice to get status.
     :param job_id: The name of the job id that armada assigns to it
     :param job_service_client: A JobServiceClient that is used for polling.
                                 It is optional only for testing
     :param job_status_callable: A callable object for test injection.
     :param time_out_for_failure: The amount of time a job
                                     can be in job_id_not_found
                                     before we decide it was a invalid job
@@ -124,15 +126,15 @@
             job_status_return = job_status_callable(
                 armada_queue=armada_queue, job_id=job_id, job_set_id=job_set_id
             )
 
         job_state = job_state_from_pb(job_status_return.state)
         armada_logger.debug(f"Got job state '{job_state.name}' for job {job_id}")
 
-        time.sleep(3)
+        time.sleep(poll_interval)
         if job_state == JobState.SUCCEEDED:
             job_message = f"Armada {airflow_task_name}:{job_id} succeeded"
             break
         if job_state == JobState.FAILED:
             job_message = (
                 f"Armada {airflow_task_name}:{job_id} failed\n"
                 f"failed with reason {job_status_return.error}"
```

## Comparing `armada_airflow-0.3.0.dist-info/LICENSE` & `armada_airflow-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `armada_airflow-0.3.0.dist-info/METADATA` & `armada_airflow-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armada-airflow
-Version: 0.3.0
+Version: 0.4.0
 Summary: Armada Airflow Operator
 Author-email: Armada-GROSS <armada@armadaproject.io>
 License: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: armada-client
@@ -14,17 +14,17 @@
 Requires-Dist: types-protobuf (>=3.19.22)
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: sphinx-jekyll-builder ; extra == 'docs'
 Provides-Extra: format
 Requires-Dist: black (==23.3.0) ; extra == 'format'
 Requires-Dist: flake8 (==6.0.0) ; extra == 'format'
-Requires-Dist: pylint (==2.17.2) ; extra == 'format'
+Requires-Dist: pylint (==2.17.3) ; extra == 'format'
 Provides-Extra: test
-Requires-Dist: pytest (==7.2.2) ; extra == 'test'
+Requires-Dist: pytest (==7.3.1) ; extra == 'test'
 Requires-Dist: coverage (>=6.5.0) ; extra == 'test'
 Requires-Dist: pytest-asyncio (==0.21.0) ; extra == 'test'
 
 # armada-airflow-operator
 
 An Airflow operator for interfacing with the armada client
```

## Comparing `armada_airflow-0.3.0.dist-info/RECORD` & `armada_airflow-0.4.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 armada/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/jobservice_pb2.py,sha256=qqr5DOfjMVk0nImQPBPoN9tSBVz9oRt2o90VNAxWARI,2728
 armada/jobservice/jobservice_pb2_grpc.py,sha256=ApiwP6_oYV8oHFlRC7oFum3I0aeEFQ9RE-7cNuaUmOk,4122
 armada/operators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-armada/operators/armada.py,sha256=7scMwIWLDUFaIZEJ6FHkHgul-YnMUSuIaPOBRW0f5IE,4579
-armada/operators/armada_deferrable.py,sha256=TmqP0-Rau7q5C6AgCEtRpWzIBfMkN8iwyWYHfercA9E,11285
+armada/operators/armada.py,sha256=5bKXOjXEG1KeUc-M2BBt3NjS34xJzX9BEHVxMHxtsa8,4869
+armada/operators/armada_deferrable.py,sha256=2WPDKYPsc-B6fNO9mEBEXqHpcoqMHTSw75rkW9l8RF0,11756
 armada/operators/jobservice.py,sha256=3K7aIsu-VU42gwLHPMYLqItV4CEJ6ovwn46hSXQGRgU,1384
 armada/operators/jobservice_asyncio.py,sha256=9dJwTuV0OslVavBJVcf1tzb7uU3tuimou8o35lLEdn0,1542
-armada/operators/utils.py,sha256=WuboRUqCHw-SAaA6NegiudvcC7zGyOXkiY0aa7E4eWQ,9976
-armada_airflow-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-armada_airflow-0.3.0.dist-info/METADATA,sha256=7A6W_hqA1zh8ZNDSaNUPQReCd6DZUCqYeSBwV9KBip8,3769
-armada_airflow-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-armada_airflow-0.3.0.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
-armada_airflow-0.3.0.dist-info/RECORD,,
+armada/operators/utils.py,sha256=ZKgFazRLXNp__htb-ZqLkWW95rm6Z5VNvtNmxCzkyQw,10090
+armada_airflow-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+armada_airflow-0.4.0.dist-info/METADATA,sha256=H05SqyRWx-HOWVFiKOyjprVVsRyfxgUkbQeQPxi-0YQ,3769
+armada_airflow-0.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+armada_airflow-0.4.0.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
+armada_airflow-0.4.0.dist-info/RECORD,,
```

