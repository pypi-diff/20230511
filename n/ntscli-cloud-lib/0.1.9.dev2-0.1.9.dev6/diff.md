# Comparing `tmp/ntscli_cloud_lib-0.1.9.dev2-py3-none-any.whl.zip` & `tmp/ntscli_cloud_lib-0.1.9.dev6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 22966 bytes, number of entries: 18
--rw-r--r--  2.0 unx     1333 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/__version__.py
--rw-r--r--  2.0 unx    20304 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/automator.py
--rw-r--r--  2.0 unx     4739 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/automator_help.py
--rw-r--r--  2.0 unx     1586 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/device_identifier.py
--rw-r--r--  2.0 unx      118 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/log.py
--rw-r--r--  2.0 unx      103 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/mqtt_retryable_error.py
--rw-r--r--  2.0 unx     1861 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/retry_with_backoff.py
--rw-r--r--  2.0 unx     2160 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/self_responder.py
--rw-r--r--  2.0 unx    19749 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/session.py
--rw-r--r--  2.0 unx     8434 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/stateful_session.py
--rw-r--r--  2.0 unx      736 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/status_watcher_interface.py
--rw-r--r--  2.0 unx      709 b- defN 20-Jul-08 20:20 ntscli_cloud_lib/testplan_checker.py
--rw-r--r--  2.0 unx     1758 b- defN 20-Jul-08 20:23 ntscli_cloud_lib-0.1.9.dev2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Jul-08 20:23 ntscli_cloud_lib-0.1.9.dev2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 20-Jul-08 20:23 ntscli_cloud_lib-0.1.9.dev2.dist-info/dependency_links.txt
--rw-r--r--  2.0 unx       17 b- defN 20-Jul-08 20:23 ntscli_cloud_lib-0.1.9.dev2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1641 b- defN 20-Jul-08 20:23 ntscli_cloud_lib-0.1.9.dev2.dist-info/RECORD
-18 files, 65414 bytes uncompressed, 20218 bytes compressed:  69.1%
+Zip file size: 23055 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     1333 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/__version__.py
+-rw-r--r--  2.0 unx    20500 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/automator.py
+-rw-r--r--  2.0 unx     4739 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/automator_help.py
+-rw-r--r--  2.0 unx     1586 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/device_identifier.py
+-rw-r--r--  2.0 unx      118 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/log.py
+-rw-r--r--  2.0 unx      103 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/mqtt_retryable_error.py
+-rw-r--r--  2.0 unx     1861 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/retry_with_backoff.py
+-rw-r--r--  2.0 unx     2866 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/self_responder.py
+-rw-r--r--  2.0 unx    20009 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/session.py
+-rw-r--r--  2.0 unx     8434 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/stateful_session.py
+-rw-r--r--  2.0 unx      736 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/status_watcher_interface.py
+-rw-r--r--  2.0 unx      709 b- defN 20-Jul-14 22:12 ntscli_cloud_lib/testplan_checker.py
+-rw-r--r--  2.0 unx     1238 b- defN 20-Jul-14 22:13 ntscli_cloud_lib-0.1.9.dev6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 20-Jul-14 22:13 ntscli_cloud_lib-0.1.9.dev6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 20-Jul-14 22:13 ntscli_cloud_lib-0.1.9.dev6.dist-info/dependency_links.txt
+-rw-r--r--  2.0 unx       17 b- defN 20-Jul-14 22:13 ntscli_cloud_lib-0.1.9.dev6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1641 b- defN 20-Jul-14 22:13 ntscli_cloud_lib-0.1.9.dev6.dist-info/RECORD
+18 files, 66056 bytes uncompressed, 20307 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: ntscli_cloud_lib/status_watcher_interface.py
 Comment: 
 
 Filename: ntscli_cloud_lib/testplan_checker.py
 Comment: 
 
-Filename: ntscli_cloud_lib-0.1.9.dev2.dist-info/METADATA
+Filename: ntscli_cloud_lib-0.1.9.dev6.dist-info/METADATA
 Comment: 
 
-Filename: ntscli_cloud_lib-0.1.9.dev2.dist-info/WHEEL
+Filename: ntscli_cloud_lib-0.1.9.dev6.dist-info/WHEEL
 Comment: 
 
-Filename: ntscli_cloud_lib-0.1.9.dev2.dist-info/dependency_links.txt
+Filename: ntscli_cloud_lib-0.1.9.dev6.dist-info/dependency_links.txt
 Comment: 
 
-Filename: ntscli_cloud_lib-0.1.9.dev2.dist-info/top_level.txt
+Filename: ntscli_cloud_lib-0.1.9.dev6.dist-info/top_level.txt
 Comment: 
 
-Filename: ntscli_cloud_lib-0.1.9.dev2.dist-info/RECORD
+Filename: ntscli_cloud_lib-0.1.9.dev6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ntscli_cloud_lib/automator.py

```diff
@@ -43,14 +43,17 @@
     name: Optional[str] = betterproto.message_field(1, wraps=betterproto.TYPE_STRING)
     # A URL to the test, relative or absolute.
     exec: Optional[str] = betterproto.message_field(2, wraps=betterproto.TYPE_STRING)
     # Text of a CSV field including all the test tags
     tags: Optional[str] = betterproto.message_field(3, wraps=betterproto.TYPE_STRING)
     # The test category.
     category: Optional[str] = betterproto.message_field(4, wraps=betterproto.TYPE_STRING)
+    # The status of the test. Values could be "applicable", "N/A for Plan",
+    # "Maintenance", "exempted"
+    status: Optional[str] = betterproto.message_field(5, wraps=betterproto.TYPE_STRING)
 
 
 @dataclass
 class TestPlan(betterproto.Message):
     """A description of a test plan"""
 
     # A list of TestCase objects.
```

## ntscli_cloud_lib/self_responder.py

```diff
@@ -1,9 +1,10 @@
 #  Copyright (c) 2020 Netflix.
 #  All rights reserved.
+import json
 import uuid
 from threading import Event
 
 from kaiju_mqtt_py import KaijuMqtt
 from kaiju_mqtt_py import MqttPacket
 
 from ntscli_cloud_lib.log import logger
@@ -48,13 +49,26 @@
 
         If the response is not sent back to us, we will typically get a timeout message,
         which will fail these assert checks.
         """
         logger.debug("SelfResponder requesting a response")
         response = self.kaiju.request(self.topic, {"request": "something"})
         logger.debug(f"SelfResponder response: {response}")
-        if "status" not in response or 200 != response["status"] or "body" not in response:
-            raise ValueError("The response did not have the expected format.")
+        try:
+            if 500 == response["status"] and "Timed out." == response["body"]["error"]:
+                logger.error("The connection to the remote broker timed out.")
+                logger.error("If you were already connected, this might be a temporary network or service outage.")
+                logger.error("If you have not been connected yet, you may have ssl configuration directory problems.")
+                raise ValueError("The connection to the remote broker timed out.")
+        except KeyError:
+            # it wasn't our template timed-out error, proceed with other error checks. This is the ideal path.
+            pass
+
+        try:
+            if 200 != response["status"]:
+                raise ValueError(f"The response did not time out, but did return an error: {json.dumps(response)}")
+        except KeyError:
+            pass
 
     def stop(self):
         """Tear down our handler."""
         self.kaiju.close()
```

## ntscli_cloud_lib/session.py

```diff
@@ -30,29 +30,38 @@
 from ntscli_cloud_lib.automator import TestPlanRunRequest
 from ntscli_cloud_lib.log import logger
 from ntscli_cloud_lib.mqtt_retryable_error import MqttRetryableError
 
 CLOUD_BROKER: str = "cloud"
 NTSCLI: str = "ntscli"
 RESPONSE: str = "response"
-BUSY_DEVICE: str = "The automator reports that the device is busy and could not accept your request. You may "
-"choose to wait, or cancel the current test plan before this request can succeed."
-MISSING_DEVICE: str = "The device was not found in the device list. "
-"See if you can start and stop Netflix on your device from the Network Agent UI on the RAE."
+BUSY_DEVICE: str = (
+    "\nThe automator reports that the device is busy and could not accept your request. You may "
+    "choose to wait, or cancel the current test plan before this request can succeed."
+)
+MISSING_DEVICE: str = (
+    "\nThe device was not found in the device list. "
+    "You were looking for:\n{}\n"
+    "See if you can start and stop Netflix on your device from the Network Agent UI on the RAE."
+)
 BROKER_UP_REQUEST_TIMEOUT: str = "The broker is responding, but the automator request failed without talking to the automator."
 RUN_REJECTED: str = "The automator rejected the request to run tests"
 DEVICE_NOT_RECOGNIZED: str = "The RAE does not recognize the device identifier:\n{}"
 IOT_BASE_PATTERN: str = "client/partner/{}"
-TOPIC_REQUIRES_CONNECTION: str = "The connection has not been made yet, so we can't form the topic string. "
-"Please call connect() before issuing other calls."
-SSL_CONFIG_MISSING: str = "The SSL configuration for the named broker is missing. "
-"Check the ~/.config/netflix/ directory for configurations."
-SSL_CONFIG_INCOMPLETE: str = "The SSL configuration for the named broker is incomplete. "
-"Check the ~/.config/netflix/ directory for configurations. "
-"Please download it again from the Netflix partner portal."
+TOPIC_REQUIRES_CONNECTION: str = (
+    "The connection has not been made yet, so we can't form the topic string. Please call connect() before issuing other calls."
+)
+SSL_CONFIG_MISSING: str = (
+    "The SSL configuration for the named broker is missing. Check the ~/.config/netflix/ directory for configuration directories."
+)
+SSL_CONFIG_INCOMPLETE: str = (
+    "\nThe SSL configuration for the named broker is incomplete. Check the ~/.config/netflix/ directory for configuration directories.\n"
+    "Each subdirectory should include .crt, .pem, and other files to create the connection with. Contact Netflix to create one of these "
+    "configurations for you."
+)
 QOS: str = "qos"
 TIMEOUT: str = "timeoutMs"
 TARGET: str = "target"
 BROKER_KEY: str = "broker"
 CERTIFICATE_ID: str = "certificate_id"
 PERIPHERAL_LIST_MISSING = "The peripheral list API did not include a list of peripherals."
 DEFLATE_BYTE_LIMIT: int = 120 * 1024  # originally these were set differently, but it's nice to have them separate even now
@@ -275,27 +284,27 @@
             # this could mean we are having broker issues -- check it ourselves
             self._check_broker()
             # if you get past _check_broker, the broker works, now it's one circle farther away
             raise ConnectionError(BROKER_UP_REQUEST_TIMEOUT)
         if error.body.error is not None:
             # explicit error from the automator
             if AutomatorStrings.MISSING_DEVICE in error.body.error:
-                raise MqttRetryableError(MISSING_DEVICE)
+                raise MqttRetryableError(MISSING_DEVICE.format(target.to_json()))
             else:
                 raise ValueError(f"Error included in response while {action_description}\n{error.body.error}")
         if error.body.message is not None:
             if AutomatorStrings.BUSY_DEVICE in error.body.message:
                 # busy message looks similar to this:
                 # {'status': 200,
                 # 'body': {'status': 'running', 'message':
                 #          'Device is currently busy running tests, request test cancellation or try again later'}}
                 logger.info(BUSY_DEVICE)
                 raise MqttRetryableError(BUSY_DEVICE)
             elif AutomatorStrings.MISSING_DEVICE in error.body.message:
-                raise MqttRetryableError(MISSING_DEVICE)
+                raise MqttRetryableError(MISSING_DEVICE.format(target.to_json()))
 
     def cancel_plan_for_device(self, device: DeviceIdentifier) -> HttpLikeCancelResponse:
         """
         Request that we cancel the tests for this device.
 
         :param device: Which device to cancel for.
         :return: dict with keys status and body. Status will be a typical HTTP error code.
```

## Comparing `ntscli_cloud_lib-0.1.9.dev2.dist-info/RECORD` & `ntscli_cloud_lib-0.1.9.dev6.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ntscli_cloud_lib/__init__.py,sha256=mYQUoguCdRASobC7wct3wbsJ3eDRjpNMjF7bdPU1s1Y,1333
 ntscli_cloud_lib/__version__.py,sha256=C69ADlbQREQlR15trneyA2sk8x0-oH4rDAX5fsv19_U,22
-ntscli_cloud_lib/automator.py,sha256=g2W4x8TSc-2e3K3rh3FIg7mckNEhvelIHgX9UkKyiHo,20304
+ntscli_cloud_lib/automator.py,sha256=yw1fN_sq60WkSJ113ZfGMF4jcZXy29oPbCBd-pd4hJY,20500
 ntscli_cloud_lib/automator_help.py,sha256=f41wDQ1rEDchqJFHigtolMsaQZlrBazDVdFcC4OjJpk,4739
 ntscli_cloud_lib/device_identifier.py,sha256=XpIbi8aYqgL4QNsy6wBhTel1SJE-HjNVIS94FOJ7-_o,1586
 ntscli_cloud_lib/log.py,sha256=uEB4qELUduNT3zI4CTfFVaPNF2UNyVqvR13cZcsQctY,118
 ntscli_cloud_lib/mqtt_retryable_error.py,sha256=GemCLwK9X2oEGShnHy5ZRd9smdL17AIXeECtLowkxoU,103
 ntscli_cloud_lib/retry_with_backoff.py,sha256=eGf0oxrSZT7KH5-o5vcWmTKHfT7HKBR_zAvTd8UxOsk,1861
-ntscli_cloud_lib/self_responder.py,sha256=2WVWyZ2m14NjCa5e4FDr03tQc8Kr7cSpAPejmSQe880,2160
-ntscli_cloud_lib/session.py,sha256=I9yFkxZzRlnJ35sxH_2XH572KUY_vzSNKG7IuSHvO_Y,19749
+ntscli_cloud_lib/self_responder.py,sha256=vFcwiAlB1qlrTP4eg41O5EM_uSvWdqaLMAXaZ68vPOA,2866
+ntscli_cloud_lib/session.py,sha256=vtXKd1BO0HujlHJEUb152QzF9mtgM-wlBhiOpx_mcFM,20009
 ntscli_cloud_lib/stateful_session.py,sha256=zMkS3fyh2fyeoWBbV5LLHBY_LpPk_AxP1fzX3hhRPyc,8434
 ntscli_cloud_lib/status_watcher_interface.py,sha256=RzMY_p2lfA-h4waOacVebeTBpP8GGBcMXswY-ulQTHs,736
 ntscli_cloud_lib/testplan_checker.py,sha256=kU_FLqk6fkZd730cJtQ1S-m1Xz4prYjITBkMVBY480M,709
-ntscli_cloud_lib-0.1.9.dev2.dist-info/METADATA,sha256=0I456wnwiEPeGBP3IEdrPuXLlHwhBoAp1zMCNVPgkYk,1758
-ntscli_cloud_lib-0.1.9.dev2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-ntscli_cloud_lib-0.1.9.dev2.dist-info/dependency_links.txt,sha256=jVpY3e-WY1t52NkCNt7qf1qQ6EI80gDiIATho9Sg-aY,52
-ntscli_cloud_lib-0.1.9.dev2.dist-info/top_level.txt,sha256=pz09Eu-CO4GJaLV7uSJDsQSKzGrav1lXN74KrWGs4RM,17
-ntscli_cloud_lib-0.1.9.dev2.dist-info/RECORD,,
+ntscli_cloud_lib-0.1.9.dev6.dist-info/METADATA,sha256=m50UTQ8xkGXU9LBw_Ihs86CxYPHQ7hcLcNlrJCP9tmw,1238
+ntscli_cloud_lib-0.1.9.dev6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+ntscli_cloud_lib-0.1.9.dev6.dist-info/dependency_links.txt,sha256=jVpY3e-WY1t52NkCNt7qf1qQ6EI80gDiIATho9Sg-aY,52
+ntscli_cloud_lib-0.1.9.dev6.dist-info/top_level.txt,sha256=pz09Eu-CO4GJaLV7uSJDsQSKzGrav1lXN74KrWGs4RM,17
+ntscli_cloud_lib-0.1.9.dev6.dist-info/RECORD,,
```

