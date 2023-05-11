# Comparing `tmp/log10_io-0.0.6.tar.gz` & `tmp/log10_io-0.0.7.tar.gz`

## Comparing `log10_io-0.0.6.tar` & `log10_io-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.6/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.0.6/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/completion.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/completion_ada.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_babyagi.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_multiple_tools.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_qa.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/        __init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/bigquery.py
--rw-r--r--   0        0        0    10361 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.6/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.6/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.0.6/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.0.7/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/completion.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/completion_ada.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/get_url.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_babyagi.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_multiple_tools.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_qa.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/        __init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/bigquery.py
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.0.7/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.0.7/PKG-INFO
```

### Comparing `log10_io-0.0.6/.github/workflows/release.yml` & `log10_io-0.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/examples/chatcompletion_async_vs_sync.py` & `log10_io-0.0.7/examples/chatcompletion_async_vs_sync.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/examples/langchain_babyagi.py` & `log10_io-0.0.7/examples/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/examples/langchain_multiple_tools.py` & `log10_io-0.0.7/examples/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/examples/langchain_qa.py` & `log10_io-0.0.7/examples/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/examples/langchain_simple_sequential.py` & `log10_io-0.0.7/examples/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/examples/langchain_sqlagent.py` & `log10_io-0.0.7/examples/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/examples/multiple_sessions.py` & `log10_io-0.0.7/examples/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/log10/bigquery.py` & `log10_io-0.0.7/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/log10/load.py` & `log10_io-0.0.7/log10/load.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,20 +47,30 @@
     except Exception as e:
         raise Exception("Failed to create LOG10 session: " + str(e) + "\nLikely cause: LOG10 env vars missing or not picked up correctly!" +
                         "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details")
 
 
 # Global variable to store the current sessionID.
 sessionID = get_session_id()
-
+last_completion_response = None
 
 class log10_session:
     def __enter__(self):
         global sessionID
+        global last_completion_response
         sessionID = get_session_id()
+        last_completion_response = None
+        return self
+
+    def last_completion_url(self):
+        if last_completion_response is None:
+            return None
+
+        return url + '/app/' +  last_completion_response['organizationSlug'] + '/completions/' + last_completion_response['completionID']
+
 
     def __exit__(self, exc_type, exc_value, traceback):
         return
 
 
 @contextmanager
 def timed_block(block_name):
@@ -81,20 +91,24 @@
     organizationSlug = output['organizationSlug']
     full_url = url + '/app/' + organizationSlug + '/completions/' + completionID
     logging.debug(f"LOG10: Completion URL: {full_url}")
 
 
 async def log_async(completion_url, func, **kwargs):
     async with ClientSession() as session:
+        global last_completion_response
+
         res = requests.request("POST",
                                completion_url, headers={"x-log10-token": token, "Content-Type": "application/json"}, json={
                                    "organization_id": org_id
                                })
         # todo: handle session id for bigquery scenario
+        last_completion_response = res.json()
         completionID = res.json()['completionID']
+
         if DEBUG:
             log_url(res, completionID)
         log_row = {
             # do we want to also store args?
             "status": "started",
             "orig_module": func.__module__,
             "orig_qualname": func.__qualname__,
@@ -118,18 +132,21 @@
 def run_async_in_thread(completion_url, func, result_queue, **kwargs):
     result = asyncio.run(
         log_async(completion_url=completion_url, func=func, **kwargs))
     result_queue.put(result)
 
 
 def log_sync(completion_url, func, **kwargs):
+    global last_completion_response
     res = requests.request("POST",
                            completion_url, headers={"x-log10-token": token, "Content-Type": "application/json"}, json={
                                "organization_id": org_id
                            })
+
+    last_completion_response = res.json()
     completionID = res.json()['completionID']
     if DEBUG:
         log_url(res, completionID)
     res = requests.request("POST",
                            completion_url + "/" + completionID,
                            headers={"x-log10-token": token,
                                     "Content-Type": "application/json"},
```

### Comparing `log10_io-0.0.6/log10/schemas/bigquery.json` & `log10_io-0.0.7/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/LICENSE` & `log10_io-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/README.md` & `log10_io-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.6/pyproject.toml` & `log10_io-0.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.0.6"
+version = "0.0.7"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.0.6/PKG-INFO` & `log10_io-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

