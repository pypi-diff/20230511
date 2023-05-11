# Comparing `tmp/openpay-0.6.tar.gz` & `tmp/openpay-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openpay-0.6.tar", last modified: Thu Jun  7 19:22:56 2018, max compression
+gzip compressed data, was "openpay-1.0.tar", last modified: Wed May 10 20:14:12 2023, max compression
```

## Comparing `openpay-0.6.tar` & `openpay-1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 marcos.alvarado   (502) staff       (20)        0 2018-06-07 19:22:56.000000 openpay-0.6/
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)      222 2018-06-07 19:22:56.000000 openpay-0.6/PKG-INFO
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)     6461 2018-04-28 01:09:47.000000 openpay-0.6/README.md
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)     1312 2018-05-29 16:38:36.000000 openpay-0.6/setup.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)        4 2018-06-07 19:17:08.000000 openpay-0.6/VERSION
-drwxr-xr-x   0 marcos.alvarado   (502) staff       (20)        0 2018-06-07 19:22:56.000000 openpay-0.6/openpay/
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)       16 2018-06-07 19:22:43.000000 openpay-0.6/openpay/version.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)     1347 2018-04-18 21:51:51.000000 openpay-0.6/openpay/error.py
-drwxr-xr-x   0 marcos.alvarado   (502) staff       (20)        0 2018-06-07 19:22:56.000000 openpay-0.6/openpay/test/
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)    11339 2018-04-18 21:51:51.000000 openpay-0.6/openpay/test/test_resources.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)      434 2018-04-18 21:51:51.000000 openpay-0.6/openpay/test/__init__.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)     5398 2018-04-18 21:51:51.000000 openpay-0.6/openpay/test/helper.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)    21990 2018-06-01 18:48:59.000000 openpay-0.6/openpay/test/test_integration.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)     6997 2018-06-07 18:55:09.000000 openpay-0.6/openpay/http_client.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)      237 2018-06-07 19:05:59.000000 openpay-0.6/openpay/util.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)    20295 2018-06-07 18:57:14.000000 openpay-0.6/openpay/resource.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)     1253 2018-05-24 18:42:32.000000 openpay-0.6/openpay/__init__.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)     6187 2018-05-29 15:35:47.000000 openpay-0.6/openpay/api.py
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)       38 2018-06-07 19:22:56.000000 openpay-0.6/setup.cfg
-drwxr-xr-x   0 marcos.alvarado   (502) staff       (20)        0 2018-06-07 19:22:56.000000 openpay-0.6/openpay.egg-info/
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)      222 2018-06-07 19:22:56.000000 openpay-0.6/openpay.egg-info/PKG-INFO
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)      433 2018-06-07 19:22:56.000000 openpay-0.6/openpay.egg-info/SOURCES.txt
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)       31 2018-06-07 19:22:56.000000 openpay-0.6/openpay.egg-info/requires.txt
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)        8 2018-06-07 19:22:56.000000 openpay-0.6/openpay.egg-info/top_level.txt
--rw-r--r--   0 marcos.alvarado   (502) staff       (20)        1 2018-06-07 19:22:56.000000 openpay-0.6/openpay.egg-info/dependency_links.txt
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.265625 openpay-1.0/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      211 2023-05-10 20:14:12.265194 openpay-1.0/PKG-INFO
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    16581 2023-04-28 23:58:01.000000 openpay-1.0/README.md
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)        4 2023-05-10 19:15:34.000000 openpay-1.0/VERSION
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.233664 openpay-1.0/openpay/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     2196 2023-05-10 19:52:12.000000 openpay-1.0/openpay/__init__.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     6187 2023-04-18 15:51:40.000000 openpay-1.0/openpay/api.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     1601 2023-04-18 15:51:40.000000 openpay-1.0/openpay/error.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     6997 2023-04-18 15:51:40.000000 openpay-1.0/openpay/http_client.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    25744 2023-04-18 15:51:40.000000 openpay-1.0/openpay/resource.py
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.264248 openpay-1.0/openpay/test/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      434 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/__init__.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     5434 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/helper.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    21990 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/test_integration.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)    11339 2023-04-18 15:51:40.000000 openpay-1.0/openpay/test/test_resources.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      237 2023-04-18 15:51:40.000000 openpay-1.0/openpay/util.py
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)       16 2023-04-18 15:51:40.000000 openpay-1.0/openpay/version.py
+drwxr-xr-x   0 marcos.vazquez   (502) staff       (20)        0 2023-05-10 20:14:12.253673 openpay-1.0/openpay.egg-info/
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      211 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/PKG-INFO
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)      433 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/SOURCES.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)        1 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/dependency_links.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)       31 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/requires.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)        8 2023-05-10 20:14:12.000000 openpay-1.0/openpay.egg-info/top_level.txt
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)       38 2023-05-10 20:14:12.265682 openpay-1.0/setup.cfg
+-rw-r--r--   0 marcos.vazquez   (502) staff       (20)     1312 2023-04-18 15:51:40.000000 openpay-1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openpay-0.6/setup.py` & `openpay-1.0/setup.py`

 * *Files identical despite different names*

### Comparing `openpay-0.6/openpay/error.py` & `openpay-1.0/openpay/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,7 +44,13 @@
         super(InvalidRequestError, self).__init__(
             message, http_body, http_status, json_body)
         self.param = param
 
 
 class AuthenticationError(OpenpayError):
     pass
+
+
+class InvalidCountryError(OpenpayError):
+    def __init__(self, message, param, http_body=None, http_status=None, json_body=None):
+        super(InvalidCountryError, self).__init__(message, http_body, http_status, json_body)
+        self.param = param
```

### Comparing `openpay-0.6/openpay/test/test_resources.py` & `openpay-1.0/openpay/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `openpay-0.6/openpay/test/helper.py` & `openpay-1.0/openpay/test/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
-from future.builtins import super
-from future.builtins import range
-from future.builtins import str
 
-import time
 import datetime
 import os
 import random
 import re
 import string
 import sys
+import time
 import unittest
 
+from future.builtins import range
+from future.builtins import str
+from future.builtins import super
 from mock import patch, Mock
 
 import openpay
 
 
 def generate_order_id():
-
     order_id = 'oid-test-{0}-{1}'.format(
         random.randint(1, 3000), str(time.time())[7:])
     if len(order_id) > 20:
         order_id = order_id[:20]
 
     return order_id
 
+
 NOW = datetime.datetime.now()
 
 DUMMY_CARD = {
     'card_number': '4111111111111111',
     'holder_name': 'Juan Lopez',
     'expiration_month': NOW.month,
     'expiration_year': str(NOW.year + 4)[2:],
@@ -76,36 +76,38 @@
     'amount': 400,
     'customer_id': 'acuqxruyv0hi1wfdwmym',
     'description': 'Dummy Transfer',
     'order_id': 'oid-00099',
 }
 
 
+
 class OpenpayTestCase(unittest.TestCase):
     RESTORE_ATTRIBUTES = ('api_version', 'api_key')
 
     def setUp(self):
         super(OpenpayTestCase, self).setUp()
 
         self._openpay_original_attributes = {}
 
         for attr in self.RESTORE_ATTRIBUTES:
             self._openpay_original_attributes[attr] = getattr(openpay, attr)
 
         api_base = os.environ.get('OPENPAY_API_BASE')
         if api_base:
             openpay.api_base = api_base
-        #Sandbox
+        # Sandbox
         openpay.api_key = os.environ.get(
             'OPENPAY_API_KEY', 'sk_10d37cc4da8e4ffd902cdf62e37abd1b')
         openpay.merchant_id = "mynvbjhtzxdyfewlzmdo"
-        #Dev
-        #openpay.api_key = os.environ.get(
+        openpay.country = "mx"
+        # Dev
+        # openpay.api_key = os.environ.get(
         #    'OPENPAY_API_KEY', '68df281c16184d47bb773d70abd4191b')
-        #openpay.merchant_id = "m4se8bd4fef1mkzk6d1b"
+        # openpay.merchant_id = "m4se8bd4fef1mkzk6d1b"
         openpay.verify_ssl_certs = False
 
     def tearDown(self):
         super(OpenpayTestCase, self).tearDown()
 
         for attr in self.RESTORE_ATTRIBUTES:
             setattr(openpay, attr, self._openpay_original_attributes[attr])
```

### Comparing `openpay-0.6/openpay/test/test_integration.py` & `openpay-1.0/openpay/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `openpay-0.6/openpay/http_client.py` & `openpay-1.0/openpay/http_client.py`

 * *Files identical despite different names*

### Comparing `openpay-0.6/openpay/resource.py` & `openpay-1.0/openpay/resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from openpay.util import utf8, logger
 
 
 def convert_to_openpay_object(resp, api_key, item_type=None):
     types = {'charge': Charge, 'customer': Customer,
              'plan': Plan, 'transfer': Transfer, 'list': ListObject,
              'card': Card, 'payout': Payout, 'subscription': Subscription,
-             'bank_account': BankAccount, 'fee': Fee}
+             'bank_account': BankAccount, 'fee': Fee, 'pse': Pse, 'checkout': Checkout,
+             'webhook': Webhook, 'token': Token}
 
     if isinstance(resp, list):
         return [convert_to_openpay_object(i, api_key, item_type) for i in resp]
     elif isinstance(resp, dict) and not isinstance(resp, BaseObject):
         resp = resp.copy()
         klass_name = resp.get('object')
         if klass_name:
@@ -326,15 +327,15 @@
 
     def serialize_metadata(self):
         if 'metadata' in self._unsaved_values:
             # the metadata object has been reassigned
             # i.e. as object.metadata = {key: val}
             metadata_update = self.metadata
             keys_to_unset = set(self._previous_metadata.keys()) - \
-                set(self.metadata.keys())
+                            set(self.metadata.keys())
             for key in keys_to_unset:
                 metadata_update[key] = ""
 
             return metadata_update
         else:
             return self.serialize(self.metadata)
 
@@ -351,14 +352,15 @@
 
 class DeletableAPIResource(APIResource):
 
     def delete(self, **params):
         self.refresh_from(self.request('delete', self.instance_url(), params))
         return self
 
+
 # API objects
 
 
 class Card(ListableAPIResource, UpdateableAPIResource,
            DeletableAPIResource, CreateableAPIResource):
 
     @classmethod
@@ -564,14 +566,38 @@
         }
 
         if not hasattr(self, '_subscriptions'):
             self._subscriptions = convert_to_openpay_object(data, self.api_key)
 
         return self._subscriptions
 
+    @property
+    def pse(self):
+        data = {
+            'object': 'list',
+            'count': 0,
+            'url':Pse.build_url(self.id),
+            'item_type': 'pse'
+        }
+        if not hasattr(self, '_pse'):
+            self._pse = convert_to_openpay_object(data, self.api_key)
+        return self._pse
+
+    @property
+    def checkouts(self):
+        data = {
+            'object': 'list',
+            'count': 0,
+            'url':Checkout.build_url(self.id),
+            'item_type': 'checkout'
+        }
+        if not hasattr(self, '_checkouts'):
+            self._checkouts = convert_to_openpay_object(data, self.api_key)
+        return self._checkouts
+
 
 class Plan(CreateableAPIResource, DeletableAPIResource,
            UpdateableAPIResource, ListableAPIResource):
     pass
 
 
 class Transfer(CreateableAPIResource, UpdateableAPIResource,
@@ -611,14 +637,15 @@
         api_key = getattr(cls, 'api_key', openpay.api_key)
 
         requestor = api.APIClient(api_key)
         url = "{0}/{1}".format(cls.class_url(), payout_id)
         response, api_key = requestor.request('get', url, params)
         return convert_to_openpay_object(response, api_key, 'payout')
 
+
 class Fee(CreateableAPIResource, ListableAPIResource):
 
     @classmethod
     def refund(cls, fee_id, **params):
         if hasattr(cls, 'api_key'):
             api_key = cls.api_key
         else:
@@ -636,7 +663,133 @@
     def instance_url(self):
         self.id = utf8(self.id)
         self.customer = utf8(getattr(self, 'customer', self.customer_id))
         extn = quote_plus(self.id)
 
         return "%s/%s/subscriptions/%s" % (Customer.class_url(),
                                            self.customer, extn)
+
+
+class Pse(CreateableAPIResource):
+
+    @classmethod
+    def create(cls, customer_id=None, **params):
+        if hasattr(cls, 'api_key'):
+            api_key = cls.api_key
+        else:
+            api_key = openpay.api_key
+        requestor = api.APIClient(api_key)
+        url = cls.build_url(customer_id)
+        response, api_key = requestor.request('post', url, params)
+        openpay_object = convert_to_openpay_object(response, api_key)
+        return openpay_object
+
+    @classmethod
+    def build_url(cls, customer_id=None):
+        merchant_id = openpay.merchant_id
+        if customer_id == None:
+            return "/v1/{0}/charges".format(merchant_id, customer_id)
+        else:
+            return "/v1/{0}/customers/{1}/charges".format(merchant_id, customer_id)
+
+
+class Webhook(CreateableAPIResource, ListableAPIResource, DeletableAPIResource):
+    @classmethod
+    def retrieve(cls, webhook_id=None, api_key=None, **params):
+        api_key = getattr(cls, 'api_key', openpay.api_key)
+        requestor = api.APIClient(api_key)
+        url = cls.build_url(webhook_id)
+        response, api_key = requestor.request('get', url, params)
+        return convert_to_openpay_object(response, api_key, 'checkout')
+
+    @classmethod
+    def build_url(cls, webhook_id):
+        merchant_id = openpay.merchant_id
+        if webhook_id is None:
+            return "/v1/{0}/webhooks".format(merchant_id)
+        if webhook_id is not None:
+            return "/v1/{0}/webhooks/{1}".format(merchant_id, webhook_id)
+
+class Checkout(CreateableAPIResource,
+               UpdateableAPIResource, ListableAPIResource):
+
+    @classmethod
+    def create(cls, customer_id=None, **params):
+        if hasattr(cls, 'api_key'):
+            api_key = cls.api_key
+        else:
+            api_key = openpay.api_key
+        requestor = api.APIClient(api_key)
+        url = cls.build_url(customer=customer_id)
+        response, api_key = requestor.request('post', url, params)
+        openpay_object = convert_to_openpay_object(response, api_key)
+        return openpay_object
+
+    @classmethod
+    def retrieve(cls, api_key=None, checkout_id=None, **params):
+        api_key = getattr(cls, 'api_key', openpay.api_key)
+        requestor = api.APIClient(api_key)
+        url = cls.build_url(checkout_id)
+        response, api_key = requestor.request('get', url, params)
+        return convert_to_openpay_object(response, api_key, 'checkout')
+
+    @classmethod
+    def build_url(cls, checkout_id=None, customer=None):
+        merchant_id = openpay.merchant_id
+        if checkout_id is None and customer is None:
+            return "/v1/{0}/checkouts".format(merchant_id)
+        if customer is not None:
+            return "/v1/{0}/customers/{1}/checkouts".format(merchant_id, customer)
+        if checkout_id is not None:
+            return "/v1/{0}/checkouts/{1}".format(merchant_id, checkout_id)
+
+    def save(self):
+        updated_params = self.serialize(self)
+
+        if getattr(self, 'metadata', None):
+            updated_params['metadata'] = self.serialize_metadata()
+
+        if updated_params:
+            self.refresh_from(self.request('put', self.instance_url(),
+                                           updated_params))
+        else:
+            logger.debug("Trying to save already saved object %r", self)
+        return self
+
+    def serialize_metadata(self):
+        if 'metadata' in self._unsaved_values:
+            # the metadata object has been reassigned
+            # i.e. as object.metadata = {key: val}
+            metadata_update = self.metadata
+            keys_to_unset = set(self._previous_metadata.keys()) - \
+                            set(self.metadata.keys())
+            for key in keys_to_unset:
+                metadata_update[key] = ""
+
+            return metadata_update
+        else:
+            return self.serialize(self.metadata)
+
+    def serialize(self, obj):
+        params = {}
+        if obj._unsaved_values:
+            for k in obj._unsaved_values:
+                if k == 'id' or k == '_previous_metadata':
+                    continue
+                v = getattr(obj, k)
+                params[k] = v if v is not None else ""
+        return params
+
+    def instance_url(self):
+        id = self.get('id')
+        status = self.get('status')
+        if not id:
+            raise error.InvalidRequestError(
+                'Could not determine which URL to request: %s instance '
+                'has invalid ID: %r' % (type(self).__name__, id), 'id')
+        id = utf8(id)
+        base = self.class_url()
+        extn = quote_plus(id)
+        return "%s/%s?status=%s" % (base, extn, status)
+
+class Token(CreateableAPIResource):
+    pass
```

### Comparing `openpay-0.6/openpay/__init__.py` & `openpay-1.0/openpay/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import unicode_literals
 from future.builtins import str
-
+from openpay.util import logger
 api_key = None
 merchant_id = None
-
 production = False
-
 api_version = None
 verify_ssl_certs = True
-
+country = "mx"
 # Resource
+
 from openpay.resource import (  # noqa
     Card, Charge, Customer, Plan, Transfer,
-    Fee, BankAccount, Payout, Subscription)
+    Fee, BankAccount, Payout, Subscription, Pse, Token, Checkout, Webhook)
 
 # Error imports.  Note that we may want to move these out of the root
 # namespace in the future and you should prefer to access them via
 # the fully qualified `openpay.error` module.
 
 from openpay.error import (  # noqa
     OpenpayError, APIError, APIConnectionError, AuthenticationError, CardError,
@@ -39,13 +38,31 @@
     'verify_ssl_certs',
     'TEST_MODE',
 )
 _original_module = _sys.modules[__name__]
 
 
 def get_api_base():
-    if not production:
-        api_base = str("https://sandbox-api.openpay.mx")
-    else:
-        api_base = str("https://api.openpay.mx")
-
+    api_base = None
+    if country is None or (country != "mx" and country != "co" and country != "pe"):
+        errorMessage = "Country is " + country + ", you can set country with value 'mx', 'co' or 'pe', Mexico, Colombia or Peru respectively"
+        logger.error(errorMessage)
+        raise error.InvalidCountryError(errorMessage, None, None, 400, None)
+    if country == "mx":
+        logger.info("Country Mexico")
+        if not production:
+            api_base = str("https://sandbox-api.openpay.mx")
+        else:
+            api_base = str("https://api.openpay.mx")
+    if country == "co":
+        logger.info("Country Mexico")
+        if not production:
+            api_base = str("https://sandbox-api.openpay.co")
+        else:
+            api_base = str("https://api.openpay.co")
+    if country == "pe":
+        logger.info("Country Peru")
+        if not production:
+            api_base = str("https://sandbox-api.openpay.pe")
+        else:
+            api_base = str("https://api.openpay.pe")
     return api_base
```

### Comparing `openpay-0.6/openpay/api.py` & `openpay-1.0/openpay/api.py`

 * *Files identical despite different names*

