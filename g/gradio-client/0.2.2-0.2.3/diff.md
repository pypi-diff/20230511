# Comparing `tmp/gradio_client-0.2.2.tar.gz` & `tmp/gradio_client-0.2.3.tar.gz`

## Comparing `gradio_client-0.2.2.tar` & `gradio_client-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.2/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.2/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/__init__.py
--rw-r--r--   0        0        0    46928 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/media_data.py
--rw-r--r--   0        0        0    18591 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/types.json
--rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.2/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.2/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.3/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.3/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/__init__.py
+-rw-r--r--   0        0        0    46928 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19006 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/types.json
+-rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.3/PKG-INFO
```

### Comparing `gradio_client-0.2.2/README.md` & `gradio_client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.2/gradio_client/client.py` & `gradio_client-0.2.3/gradio_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,17 +399,17 @@
 
         """
         if self.serialize:
             api_info_url = urllib.parse.urljoin(self.src, utils.API_INFO_URL)
         else:
             api_info_url = urllib.parse.urljoin(self.src, utils.RAW_API_INFO_URL)
 
-        # Versions of Gradio older than 3.28.3 returned format of the API info
+        # Versions of Gradio older than 3.29.0 returned format of the API info
         # from the /info endpoint
-        if version.parse(self.config.get("version", "2.0")) > version.Version("3.28.3"):
+        if version.parse(self.config.get("version", "2.0")) > version.Version("3.29.0"):
             r = requests.get(api_info_url, headers=self.headers)
             if r.ok:
                 info = r.json()
             else:
                 raise ValueError(f"Could not fetch api info for {self.src}")
         else:
             fetch = requests.post(
```

### Comparing `gradio_client-0.2.2/gradio_client/documentation.py` & `gradio_client-0.2.3/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.2/gradio_client/media_data.py` & `gradio_client-0.2.3/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.2/gradio_client/serializing.py` & `gradio_client-0.2.3/gradio_client/serializing.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,19 +227,30 @@
             "serialized_info": True,
         }
 
     def api_info(self) -> dict[str, dict | bool]:
         return self._single_file_api_info()
 
     def example_inputs(self) -> dict[str, Any]:
+        return self._single_file_example_inputs()
+
+    def _single_file_example_inputs(self) -> dict[str, Any]:
         return {
             "raw": {"is_file": False, "data": media_data.BASE64_FILE},
             "serialized": "https://github.com/gradio-app/gradio/raw/main/test/test_files/sample_file.pdf",
         }
 
+    def _multiple_file_example_inputs(self) -> dict[str, Any]:
+        return {
+            "raw": [{"is_file": False, "data": media_data.BASE64_FILE}],
+            "serialized": [
+                "https://github.com/gradio-app/gradio/raw/main/test/test_files/sample_file.pdf"
+            ],
+        }
+
     def _serialize_single(
         self, x: str | FileData | None, load_dir: str | Path = ""
     ) -> FileData | None:
         if x is None or isinstance(x, dict):
             return x
         if utils.is_valid_url(x):
             filename = x
```

### Comparing `gradio_client-0.2.2/gradio_client/types.json` & `gradio_client-0.2.3/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.2/gradio_client/utils.py` & `gradio_client-0.2.3/gradio_client/utils.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.2/.gitignore` & `gradio_client-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.2/pyproject.toml` & `gradio_client-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.2/PKG-INFO` & `gradio_client-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

