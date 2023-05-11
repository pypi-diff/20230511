# Comparing `tmp/gradio_client-0.2.3.tar.gz` & `tmp/gradio_client-0.2.4.tar.gz`

## Comparing `gradio_client-0.2.3.tar` & `gradio_client-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.3/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.3/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/__init__.py
--rw-r--r--   0        0        0    46928 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/media_data.py
--rw-r--r--   0        0        0    19006 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/types.json
--rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.3/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.3/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.4/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.4/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/__init__.py
+-rw-r--r--   0        0        0    46928 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19192 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/types.json
+-rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.4/PKG-INFO
```

### Comparing `gradio_client-0.2.3/README.md` & `gradio_client-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/gradio_client/client.py` & `gradio_client-0.2.4/gradio_client/client.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/gradio_client/documentation.py` & `gradio_client-0.2.4/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/gradio_client/media_data.py` & `gradio_client-0.2.4/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/gradio_client/serializing.py` & `gradio_client-0.2.4/gradio_client/serializing.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,11 +537,16 @@
     "highlightedtext": JSONSerializable,
     "json": JSONSerializable,
     "html": StringSerializable,
     "gallery": GallerySerializable,
     "chatbot": JSONSerializable,
     "model3d": FileSerializable,
     "plot": JSONSerializable,
+    "barplot": JSONSerializable,
+    "lineplot": JSONSerializable,
+    "scatterplot": JSONSerializable,
     "markdown": StringSerializable,
     "dataset": StringSerializable,
     "code": StringSerializable,
+    "interpretation": SimpleSerializable,
+    "annotatedimage": JSONSerializable,
 }
```

### Comparing `gradio_client-0.2.3/gradio_client/types.json` & `gradio_client-0.2.4/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/gradio_client/utils.py` & `gradio_client-0.2.4/gradio_client/utils.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/.gitignore` & `gradio_client-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/pyproject.toml` & `gradio_client-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.3/PKG-INFO` & `gradio_client-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

