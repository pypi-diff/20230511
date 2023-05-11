# Comparing `tmp/oaaclient-1.1.2.tar.gz` & `tmp/oaaclient-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaaclient-1.1.2.tar", last modified: Wed Apr 26 18:43:43 2023, max compression
+gzip compressed data, was "oaaclient-1.1.3.tar", last modified: Thu May 11 14:59:15 2023, max compression
```

## Comparing `oaaclient-1.1.2.tar` & `oaaclient-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.981456 oaaclient-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 18:43:20.000000 oaaclient-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-26 18:43:43.977456 oaaclient-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-26 18:43:20.000000 oaaclient-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.977456 oaaclient-1.1.2/oaaclient/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39135 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    90551 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.977456 oaaclient-1.1.2/oaaclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-26 18:43:20.000000 oaaclient-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:43:43.981456 oaaclient-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 18:43:20.000000 oaaclient-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.977456 oaaclient-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36240 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_custom_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_custom_idp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_payload_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_reprs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_template_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.344697 oaaclient-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 14:58:58.000000 oaaclient-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-11 14:59:15.344697 oaaclient-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-11 14:58:58.000000 oaaclient-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.340697 oaaclient-1.1.3/oaaclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39285 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90348 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-05-11 14:58:58.000000 oaaclient-1.1.3/oaaclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.340697 oaaclient-1.1.3/oaaclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 14:59:15.000000 oaaclient-1.1.3/oaaclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-11 14:58:58.000000 oaaclient-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:59:15.344697 oaaclient-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-11 14:58:58.000000 oaaclient-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:59:15.344697 oaaclient-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    34102 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_custom_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_custom_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_payload_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_reprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_template_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-11 14:58:58.000000 oaaclient-1.1.3/tests/test_utils.py
```

### Comparing `oaaclient-1.1.2/LICENSE` & `oaaclient-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/PKG-INFO` & `oaaclient-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaaclient
-Version: 1.1.2
+Version: 1.1.3
 Summary: Veza Open Authorization API (OAA) SDK
 Author-email: "Veza Technologies Inc." <oaa_dev@veza.com>
 License: MIT
 Project-URL: homepage, https://github.com/veza/oaaclient-py
 Project-URL: repository, https://github.com/veza/oaaclient-py
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `oaaclient-1.1.2/README.md` & `oaaclient-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/oaaclient/client.py` & `oaaclient-1.1.3/oaaclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -905,15 +905,17 @@
     to our own value
 
     Args:
         Retry (_type_): _description_
     """
     def __init__(self, backoff_max=30, **kwargs) -> None:
         super(OAARetry, self).__init__(**kwargs)
+        #urllib3 1.x and 2.x have slightly different behavior for BACKOFF_MAX, setting both values covers both
         self.DEFAULT_BACKOFF_MAX = backoff_max
+        self.backoff_max = backoff_max
 
 
 def report_builder_entrypoint() -> None:
     """Entry point for `oaaclient-report-builder` command
 
     Reads a JSON file and passes it to the `oaaclient.utils.build_report` method
     """
```

### Comparing `oaaclient-1.1.2/oaaclient/structures.py` & `oaaclient-1.1.3/oaaclient/structures.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/oaaclient/templates.py` & `oaaclient-1.1.3/oaaclient/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,17 +157,14 @@
                 }
 
         repr['resources'] = [resource.to_dict() for resource in self.resources.values()]
         return repr
 
     def permissions_dict(self) -> dict:
         """ Return the 'permissions' section of the payload as serializable dictionary. """
-        # TODO: error handling for empty list or non-permissions
-        if not self.custom_permissions:
-            raise Exception("No custom permissions defined, must define at least one permission")
 
         return [permission.to_dict() for permission in self.custom_permissions.values()]
 
     def define_custom_permission(self, custom_permission: CustomPermission) -> CustomPermission:
         """Add a custom permission to the application.
 
         .. deprecated::
```

### Comparing `oaaclient-1.1.2/oaaclient/utils.py` & `oaaclient-1.1.3/oaaclient/utils.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/oaaclient.egg-info/PKG-INFO` & `oaaclient-1.1.3/oaaclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaaclient
-Version: 1.1.2
+Version: 1.1.3
 Summary: Veza Open Authorization API (OAA) SDK
 Author-email: "Veza Technologies Inc." <oaa_dev@veza.com>
 License: MIT
 Project-URL: homepage, https://github.com/veza/oaaclient-py
 Project-URL: repository, https://github.com/veza/oaaclient-py
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `oaaclient-1.1.2/oaaclient.egg-info/SOURCES.txt` & `oaaclient-1.1.3/oaaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/pyproject.toml` & `oaaclient-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_client.py` & `oaaclient-1.1.3/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 """
 
 import base64
 import logging
 import os
 import time
 import uuid
+import urllib3
+import io
 from http.client import HTTPMessage, HTTPResponse
 from unittest.mock import MagicMock, PropertyMock, patch
 
 import pytest
 import requests
 from oaaclient.client import OAAClient, OAAClientError, OAAConnectionError, OAAResponseError
 from requests.models import Response
@@ -180,115 +182,59 @@
     # test that the error is populated property
     assert e.value.error == "Internal"
     assert e.value.message == "Internal Server Error, please retry and if the error persists contact support at support@veza.com"
     assert e.value.status_code == 400
     assert len(e.value.details) == 1
     assert "Internal server error." in str(e.value.details)
 
-@patch("urllib3.connectionpool.HTTPConnectionPool._get_conn")
+@patch("urllib3.connectionpool.HTTPConnectionPool._make_request")
 @patch("time.sleep", return_value=None)
-def test_api_get_retry(mock_sleep, mock_get_conn):
-    # Test that the correct OAAClient exception is raised on properly populated
-
-    # set total retry count lower to speed up tests
-    os.environ.setdefault("OAA_API_RETRIES", "3")
-
+def test_api_get_retry(mock_sleep, mock_make_request):
+    # test that the retry logic behaves correctly, that it retries the right number of times and that total time is within our expected
     test_api_key = "1234"
     # patch _test_connection to instantiate a connection object
     with patch.object(OAAClient, "_test_connection", return_value=None):
         veza_con = OAAClient(url="https://noreply.vezacloud.com", token=test_api_key)
 
     url = "/api/should/fail"
 
-    bad = MagicMock(status=500, msg=HTTPMessage(), response=Response())
-    bad.create_autospec(HTTPResponse)
-    # assert five bad raises exception
-
-
-    # the mock_get_conn is patched urllib3.connectionpool.HTTPConnectionPool._get_conn
-    # _get_conn returns a urllib3.HTTPConection
-    # ensure that the side effect is bad for the total number of retries
-    mock_get_conn.return_value.getresponse.side_effect = [bad] * (OAAClient.DEFAULT_RETRY_COUNT + 1)
-
-    timeout_start = time.time()
+    bad = urllib3.response.HTTPResponse(status=500, reason="Failure", request_url=url)
+    mock_make_request.return_value = bad
 
     with pytest.raises(OAAConnectionError) as e:
         response = veza_con.api_get(url)
 
-    # three tries would require two sleep backoff calls
-    assert mock_sleep.call_count == 2
+    # ten retries (default) would require nine sleep back off calls
+    assert mock_sleep.call_count == 9
+    sleep_times = [c.args[0] for c in mock_sleep.call_args_list]
+    assert sum(sleep_times) == 157.2
 
     # test that the error is populated property
     assert e.value.error == "ERROR"
     assert "Max retries exceeded" in e.value.message
 
-    # test that retry to good works
+    # test that retry to good works correct, two bad responses and a good
     url = "/api/should/work"
 
-    mock_get_conn.reset_mock()
+    mock_make_request.reset_mock()
 
-    good = MagicMock(name="HttpResponse200")
-    good.status = 200
-    # in order to get urlib3 to populate the response content before returning it to requests you have to do a few things
-    # set msg contains the headers, need to tell it that there is a response coming that is a chunked response
-    good.msg = HTTPMessage()
-    good.msg.add_header('Transfer-Encoding', 'chunked')
-    good.msg.add_header('Content-Type', 'application/json')
-    # in order to get urllib3 to read the content we need to pass it a size of chunks, this is from fp.readline
-    good.fp.readline.side_effect = [b'1dc1\r\n', b'0\r\n', b'\r\n']
-    # after it works out the sizes it makes "_safe_read" calls to get the actual content, we can just pass the value we want here
-    good._safe_read.return_value = b'{"message": "ok"}'
+    response_body = io.BytesIO(b'{"message": "ok"}')
+    headers={"Content-Type": "application/json", "Content-Length": "17"}
+    good = urllib3.response.HTTPResponse(response_body, status=200, request_url=url, headers=headers, preload_content=False)
 
-    bad.reset_mock()
-    mock_get_conn.return_value.getresponse.side_effect = [bad, bad, good]
+    # two bad responses then a good should result in no exceptions raised to caller
+    mock_make_request.side_effect = [bad, bad, good]
 
     # test that the api get will retry to get to the good response
     response = veza_con.api_get(url)
     log.debug(response)
     assert response.get("message") == "ok"
 
-
-@patch("time.sleep", return_value=None)
-@patch("urllib3.connectionpool.HTTPConnectionPool._get_conn")
-def test_api_get_retry_timeout(mock_get_conn, mock_sleep):
-    # Test to ensure full retry timeout exceeds 60 second target
-
-    # ensure that the default isn't being overridden
-    del os.environ["OAA_API_RETRIES"]
-
-    test_api_key = "1234"
-    # patch _test_connection to instantiate a connection object
-    with patch.object(OAAClient, "_test_connection", return_value=None):
-        veza_con = OAAClient(url="https://noreply.vezacloud.com", token=test_api_key)
-
-    url = "/api/should/fail"
-
-    bad = MagicMock(status=500, msg=HTTPMessage(), response=Response())
-    bad.create_autospec(HTTPResponse)
-
-    # the mock_get_conn is patched urllib3.connectionpool.HTTPConnectionPool._get_conn
-    # _get_conn returns a urllib3.HTTPConection
-    # ensure that the side effect is bad for the total number of retries
-    mock_get_conn.return_value.getresponse.side_effect = [bad] * (OAAClient.DEFAULT_RETRY_COUNT + 1)
-
-
-    with pytest.raises(OAAConnectionError) as e:
-        response = veza_con.api_get(url)
-
-    assert mock_sleep.call_count == 9
-    sleep_times = [c.args[0] for c in mock_sleep.call_args_list]
-    assert 150 < sum(sleep_times) < 200
-
-    # test that the error is populated property
-    assert e.value.error == "ERROR"
-    assert "Max retries exceeded" in e.value.message
-
     return
 
-
 @patch.object(requests.Session, "request")
 def test_api_get_nonjson_error(mock_session_get):
     # Test that the OAAClient correctly handles a non-JSON respponse if error isn't coming from Veza stack
 
     test_api_key = "1234"
     url = "https://noreply.vezacloud.com"
     # patch _test_connection to instantiate a connection object
```

### Comparing `oaaclient-1.1.2/tests/test_commands.py` & `oaaclient-1.1.3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_custom_application.py` & `oaaclient-1.1.3/tests/test_custom_application.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_custom_idp.py` & `oaaclient-1.1.3/tests/test_custom_idp.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_payload_push.py` & `oaaclient-1.1.3/tests/test_payload_push.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_reprs.py` & `oaaclient-1.1.3/tests/test_reprs.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_structures.py` & `oaaclient-1.1.3/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_tags.py` & `oaaclient-1.1.3/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.2/tests/test_utils.py` & `oaaclient-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

