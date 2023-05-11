# Comparing `tmp/nornir_f5-0.6.0.tar.gz` & `tmp/nornir_f5-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_f5-0.6.0.tar", max compression
+gzip compressed data, was "nornir_f5-0.6.1.tar", max compression
```

## Comparing `nornir_f5-0.6.0.tar` & `nornir_f5-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/LICENSE
--rw-r--r--   0        0        0     3350 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/README.md
--rw-r--r--   0        0        0       40 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/__init__.py
--rw-r--r--   0        0        0       25 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/__init__.py
--rw-r--r--   0        0        0      218 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/connections/__init__.py
--rw-r--r--   0        0        0     4551 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/connections/f5.py
--rw-r--r--   0        0        0     1057 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/__init__.py
--rw-r--r--   0        0        0    11335 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/atc.py
--rw-r--r--   0        0        0       30 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/__init__.py
--rw-r--r--   0        0        0       53 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/cm/__init__.py
--rw-r--r--   0        0        0     3659 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/cm/config_sync.py
--rw-r--r--   0        0        0      695 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/cm/failover_status.py
--rw-r--r--   0        0        0      682 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/cm/sync_status.py
--rw-r--r--   0        0        0       30 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/shared/__init__.py
--rw-r--r--   0        0        0       37 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/shared/file_transfer/__init__.py
--rw-r--r--   0        0        0     2516 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/shared/file_transfer/uploads.py
--rw-r--r--   0        0        0       28 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/shared/iapp/__init__.py
--rw-r--r--   0        0        0     4797 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/shared/iapp/package_management_tasks.py
--rw-r--r--   0        0        0       36 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/sys/__init__.py
--rw-r--r--   0        0        0      610 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/sys/version.py
--rw-r--r--   0        0        0       38 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/util/__init__.py
--rw-r--r--   0        0        0      911 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/util/unix_ls.py
--rw-r--r--   0        0        0      951 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/util/unix_rm.py
--rw-r--r--   0        0        0     2198 2023-02-16 17:10:42.082625 nornir_f5-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4761 2023-02-16 17:11:06.761762 nornir_f5-0.6.0/setup.py
--rw-r--r--   0        0        0     4569 2023-02-16 17:11:06.762503 nornir_f5-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3350 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/README.md
+-rw-r--r--   0        0        0       40 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/__init__.py
+-rw-r--r--   0        0        0      218 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/connections/__init__.py
+-rw-r--r--   0        0        0     4551 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/connections/f5.py
+-rw-r--r--   0        0        0     1057 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/__init__.py
+-rw-r--r--   0        0        0    12048 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/atc.py
+-rw-r--r--   0        0        0       30 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/cm/__init__.py
+-rw-r--r--   0        0        0     3659 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/cm/config_sync.py
+-rw-r--r--   0        0        0      695 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/cm/failover_status.py
+-rw-r--r--   0        0        0      682 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/cm/sync_status.py
+-rw-r--r--   0        0        0       30 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/shared/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/shared/file_transfer/__init__.py
+-rw-r--r--   0        0        0     2516 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/shared/file_transfer/uploads.py
+-rw-r--r--   0        0        0       28 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/shared/iapp/__init__.py
+-rw-r--r--   0        0        0     4797 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/shared/iapp/package_management_tasks.py
+-rw-r--r--   0        0        0       36 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/sys/__init__.py
+-rw-r--r--   0        0        0      610 2023-05-11 15:36:43.009625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/sys/version.py
+-rw-r--r--   0        0        0       38 2023-05-11 15:36:43.013625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/util/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-11 15:36:43.013625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/util/unix_ls.py
+-rw-r--r--   0        0        0      951 2023-05-11 15:36:43.013625 nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/util/unix_rm.py
+-rw-r--r--   0        0        0     2198 2023-05-11 15:36:43.013625 nornir_f5-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 nornir_f5-0.6.1/PKG-INFO
```

### Comparing `nornir_f5-0.6.0/LICENSE` & `nornir_f5-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/README.md` & `nornir_f5-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/connections/f5.py` & `nornir_f5-0.6.1/nornir_f5/plugins/connections/f5.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/__init__.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/atc.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/atc.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,43 +141,58 @@
 
 def _wait_task(
     task: Task,
     atc_task_endpoint: str,
     atc_task_id: str,
     atc_delay: int = 10,
     atc_retries: int = 30,
+    as3_tenant: Optional[str] = None,
 ) -> Result:
     client = f5_rest_client(task)
     host = f"{task.host.hostname}:{task.host.port}"
+    _return = {
+        "declaration failed": {"retry": True, "result": "response", "raise": True},
+        "declaration is invalid": {"retry": True, "result": "errors", "raise": True},
+        "in progress": {"retry": True, "result": "message", "raise": False},
+        "no change": {"retry": False, "result": "message", "raise": False},
+        "processing": {"retry": True, "result": "message", "raise": False},
+        "success": {"retry": False, "result": "message", "raise": False},
+    }
 
     for _i in range(0, atc_retries):
         atc_task_resp = client.get(
             f"https://{host}{atc_task_endpoint}/{atc_task_id}"
         ).json()
 
-        result = (
-            atc_task_resp["results"][0]
+        results = (
+            atc_task_resp["results"]
             if "results" in atc_task_resp
-            else atc_task_resp["result"]
+            else [atc_task_resp["result"]]
         )
-        message = result["message"]
 
-        if message in ["in progress", "processing"]:
-            pass
-        elif message == "success":
-            return Result(host=task.host, changed=True, result=message)
-        elif message == "no change":
-            return Result(host=task.host, result=message)
-        elif message == "declaration is invalid":
-            raise Exception(result["errors"])
-        elif message == "declaration failed":
-            raise Exception(result["response"])
+        retry = False
+        for result in results:
+            message = result["message"]
+            if message in _return:
+                if _return[message]["raise"]:
+                    raise Exception(result[_return[message]["result"]])
+                elif _return[message]["retry"]:
+                    retry = True
+            else:
+                raise Exception("The task failed.")
+
+        if retry:
+            time.sleep(atc_delay)
         else:
-            raise Exception("The task failed.")
-        time.sleep(atc_delay)
+            message = results[0]["message"]
+            if as3_tenant:
+                for result in results:
+                    if result["tenant"] == as3_tenant:
+                        message = result["message"]
+            return Result(host=task.host, result=message)
 
     raise Exception("The task has reached maximum retries.")
 
 
 def atc_info(task: Task, atc_method: str, atc_service: str) -> Result:
     """Task to verify if ATC service is available and collect service info.
 
@@ -316,14 +331,15 @@
     if atc_service == "Telemetry" or atc_method == "GET":
         return Result(host=task.host, result=atc_send_result)
 
     # Wait for task to complete
     task_result = task.run(
         name="Wait for task to complete",
         task=_wait_task,
+        as3_tenant=as3_tenant,
         atc_delay=atc_delay,
         atc_retries=atc_retries,
         atc_task_endpoint=ATC_COMPONENTS[atc_service]["endpoints"]["task"]["uri"],
         atc_task_id=atc_send_result["id"],
     ).result
 
     if task_result == "no change":
```

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/cm/config_sync.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/cm/config_sync.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/cm/failover_status.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/cm/failover_status.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/cm/sync_status.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/cm/sync_status.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/shared/file_transfer/uploads.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/shared/file_transfer/uploads.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/shared/iapp/package_management_tasks.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/shared/iapp/package_management_tasks.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/sys/version.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/sys/version.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/util/unix_ls.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/util/unix_ls.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/nornir_f5/plugins/tasks/bigip/util/unix_rm.py` & `nornir_f5-0.6.1/nornir_f5/plugins/tasks/bigip/util/unix_rm.py`

 * *Files identical despite different names*

### Comparing `nornir_f5-0.6.0/pyproject.toml` & `nornir_f5-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 documentation = "https://github.com/erjac77/nornir_f5"
 homepage = "https://github.com/erjac77/nornir_f5"
 keywords = ["nornir", "f5", "bigip", "automation", "as3"]
 license = "Apache-2.0"
 name = "nornir_f5"
 readme = "README.md"
 repository = "https://github.com/erjac77/nornir_f5"
-version = "0.6.0"
+version = "0.6.1"
 
 [tool.poetry.urls]
 Issues = "https://github.com/erjac77/nornir_f5/issues"
 "Pull Requests" = "https://github.com/erjac77/nornir_f5/pulls"
 Releases = "https://github.com/erjac77/nornir_f5/releases"
 
 [tool.poetry.dependencies]
```

### Comparing `nornir_f5-0.6.0/PKG-INFO` & `nornir_f5-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: nornir-f5
-Version: 0.6.0
+Version: 0.6.1
 Summary: F5 plugins for Nornir
 Home-page: https://github.com/erjac77/nornir_f5
 License: Apache-2.0
 Keywords: nornir,f5,bigip,automation,as3
 Author: Eric Jacob
 Author-email: erjac77@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Networking
 Requires-Dist: nornir (>=3.3.0,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

