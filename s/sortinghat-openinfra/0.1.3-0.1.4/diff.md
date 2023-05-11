# Comparing `tmp/sortinghat_openinfra-0.1.3.tar.gz` & `tmp/sortinghat_openinfra-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat_openinfra-0.1.3.tar", max compression
+gzip compressed data, was "sortinghat_openinfra-0.1.4.tar", max compression
```

## Comparing `sortinghat_openinfra-0.1.3.tar` & `sortinghat_openinfra-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-09 09:43:46.346635 sortinghat_openinfra-0.1.3/LICENSE
--rw-r--r--   0        0        0     2244 2023-05-09 09:43:46.346635 sortinghat_openinfra-0.1.3/README.md
--rw-r--r--   0        0        0     1268 2023-05-09 09:43:46.346635 sortinghat_openinfra-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       86 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/sortinghat/core/importer/backends/_version.py
--rw-r--r--   0        0        0     7865 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/sortinghat/core/importer/backends/openinfra.py
--rw-r--r--   0        0        0        0 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     6403 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/data/openinfra_page_1.json
--rw-r--r--   0        0        0     5073 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/data/openinfra_page_2.json
--rw-r--r--   0        0        0     2595 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/data/openinfra_private.json
--rw-r--r--   0        0        0    17770 2023-05-09 09:43:46.350635 sortinghat_openinfra-0.1.3/tests/test_openinfra.py
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2244 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/README.md
+-rw-r--r--   0        0        0     1268 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/sortinghat/core/importer/backends/_version.py
+-rw-r--r--   0        0        0     7917 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/sortinghat/core/importer/backends/openinfra.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     6403 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/tests/data/openinfra_page_1.json
+-rw-r--r--   0        0        0     5073 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/tests/data/openinfra_page_2.json
+-rw-r--r--   0        0        0     2595 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/tests/data/openinfra_private.json
+-rw-r--r--   0        0        0      143 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/tests/data/openinfra_token_error.json
+-rw-r--r--   0        0        0    21169 2023-05-11 11:25:27.229476 sortinghat_openinfra-0.1.4/tests/test_openinfra.py
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.4/PKG-INFO
```

### Comparing `sortinghat_openinfra-0.1.3/LICENSE` & `sortinghat_openinfra-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.3/README.md` & `sortinghat_openinfra-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.3/pyproject.toml` & `sortinghat_openinfra-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat-openinfra"
-version = "0.1.3"
+version = "0.1.4"
 description = "SortingHat backend to import identities from OpenInfraID"
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sortinghat_openinfra-0.1.3/sortinghat/core/importer/backends/openinfra.py` & `sortinghat_openinfra-0.1.4/sortinghat/core/importer/backends/openinfra.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,17 +183,18 @@
         """Return items using pagination"""
 
         if not payload:
             payload = {}
 
         page = 1
         while True:
+            logger.info(f"Fetching next members from API {payload}")
             r = requests.get(url, params=payload)
-            if self.private_api and r.status_code == '400' and r.json()['error'] == 'invalid_token':
-                logger.warning(r.json()['description'])
+            if self.private_api and r.status_code == 401 and r.json()['error'] == 'invalid_token':
+                logger.warning(r.json())
                 self.access_token = self._create_access_token()
                 payload[self.PTOKEN] = self.access_token
                 continue
             elif not r.ok:
                 raise LoadError(cause=f"Error fetching items. Status code <{r.status_code}>")
 
             data = r.json()
```

### Comparing `sortinghat_openinfra-0.1.3/tests/data/openinfra_page_1.json` & `sortinghat_openinfra-0.1.4/tests/data/openinfra_page_1.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.3/tests/data/openinfra_page_2.json` & `sortinghat_openinfra-0.1.4/tests/data/openinfra_page_2.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.3/tests/data/openinfra_private.json` & `sortinghat_openinfra-0.1.4/tests/data/openinfra_private.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.3/tests/test_openinfra.py` & `sortinghat_openinfra-0.1.4/tests/test_openinfra.py`

 * *Files 6% similar despite different names*

```diff
@@ -294,14 +294,94 @@
         expected_qs = {
             'grant_type': ['client_credentials'],
             'scope': ['https://openstackid-resources.openstack.org/members/read']
         }
         self.assertEqual(request.querystring, expected_qs)
 
     @httpretty.activate
+    @override_settings(OPENINFRA_CLIENT_ID='id_test', OPENINFRA_CLIENT_SECRET='secret_test')
+    def test_fetch_items_invalid_token(self):
+        """Test whether fetch items with invalid token generates a new token"""
+
+        # Set up a mock HTTP server
+        body_error = read_file('data/openinfra_token_error.json')
+        body_members = read_file('data/openinfra_private.json')
+
+        responses = [
+            httpretty.Response(body=body_error,
+                               status=401),
+            httpretty.Response(body=body_members),
+        ]
+
+        httpretty.register_uri(httpretty.GET,
+                               OPENINFRA_PRIVATE_MEMBERS_URL,
+                               responses=responses)
+        httpretty.register_uri(
+            httpretty.POST,
+            OpenInfraIDParser.OPENINFRA_TOKEN_URL,
+            body='{"access_token":"test_token","expires_in":7200,"token_type":"Bearer"}',
+            status=200
+        )
+
+        # Run fetch items
+        parser = OpenInfraIDParser(OPENINFRA_URL)
+
+        payload = {
+            OpenInfraIDParser.PPER_PAGE: 100,
+            OpenInfraIDParser.PSORT: 'last_edited',
+            OpenInfraIDParser.PPAGE: 1,
+            OpenInfraIDParser.PTOKEN: 'wrong_token'
+        }
+        raw_items = parser.fetch_items(OPENINFRA_PRIVATE_MEMBERS_URL, payload=payload)
+
+        items = [item for item in raw_items]
+        self.assertEqual(len(items), 1)
+        self.assertDictEqual(items[0], json.loads(body_members))
+
+        # Check requests
+        requests = httpretty.latest_requests()
+
+        expected_requests = [
+            {
+                "body": "",
+                "querystring": {'access_token': ['wrong_token'], 'order': ['last_edited'],
+                            'page': ['1'], 'per_page': ['100']},
+                "method": 'GET',
+                "url": OPENINFRA_PRIVATE_MEMBERS_URL
+            },
+            {
+                "body": {'client_id': ['id_test'], 'client_secret': ['secret_test']},
+                "querystring": {'grant_type': ['client_credentials'],
+                            'scope': ['https://openstackid-resources.openstack.org/members/read']},
+                "method": 'POST',
+                "url": "https://id.openinfra.dev/oauth2/token"
+            },
+            {
+                "body": {'client_id': ['id_test'], 'client_secret': ['secret_test']},
+                "querystring": {'grant_type': ['client_credentials'],
+                            'scope': ['https://openstackid-resources.openstack.org/members/read']},
+                "method": 'POST',
+                "url": "https://id.openinfra.dev/oauth2/token"
+            },
+            {
+                "body": "",
+                "querystring": {'access_token': ['test_token'], 'order': ['last_edited'],
+                                'page': ['1'], 'per_page': ['100']},
+                "method": 'GET',
+                "url": OPENINFRA_PRIVATE_MEMBERS_URL
+            }
+        ]
+        self.assertEqual(len(requests), 4)
+        for i, req in enumerate(requests):
+            self.assertDictEqual(req.querystring, expected_requests[i]["querystring"])
+            self.assertEqual(req.url.split('?')[0], expected_requests[i]["url"])
+            self.assertEqual(req.parsed_body, expected_requests[i]["body"])
+            self.assertEqual(req.method, expected_requests[i]["method"])
+
+    @httpretty.activate
     def test_fetch_individuals(self):
         """Test fetch_individuals returns individuals"""
 
         # Set up a mock HTTP server
         requests, bodies = setup_mock_server(public=True)
 
         # Run fetch individuals
```

### Comparing `sortinghat_openinfra-0.1.3/PKG-INFO` & `sortinghat_openinfra-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat-openinfra
-Version: 0.1.3
+Version: 0.1.4
 Summary: SortingHat backend to import identities from OpenInfraID
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab,sortinghat
 Author: Bitergia Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

