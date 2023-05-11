# Comparing `tmp/grai_source_dbt_cloud-0.0.2.tar.gz` & `tmp/grai_source_dbt_cloud-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt_cloud-0.0.2.tar", max compression
+gzip compressed data, was "grai_source_dbt_cloud-0.0.3a1.tar", max compression
```

## Comparing `grai_source_dbt_cloud-0.0.2.tar` & `grai_source_dbt_cloud-0.0.3a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.0.2/README.md
--rw-r--r--   0        0        0      926 2023-05-04 09:38:52.431220 grai_source_dbt_cloud-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-03 16:29:40.851280 grai_source_dbt_cloud-0.0.2/src/grai_source_dbt_cloud/__init__.py
--rw-r--r--   0        0        0      753 2023-05-03 16:29:40.851647 grai_source_dbt_cloud-0.0.2/src/grai_source_dbt_cloud/base.py
--rw-r--r--   0        0        0      745 2023-05-04 09:38:52.431926 grai_source_dbt_cloud-0.0.2/src/grai_source_dbt_cloud/loader.py
--rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.0.2/src/grai_source_dbt_cloud/py.typed
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.0.3a1/README.md
+-rw-r--r--   0        0        0      933 2023-05-10 10:17:45.968170 grai_source_dbt_cloud-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-03 16:29:40.851280 grai_source_dbt_cloud-0.0.3a1/src/grai_source_dbt_cloud/__init__.py
+-rw-r--r--   0        0        0      877 2023-05-10 10:03:30.937728 grai_source_dbt_cloud-0.0.3a1/src/grai_source_dbt_cloud/base.py
+-rw-r--r--   0        0        0     1489 2023-05-10 12:32:57.840093 grai_source_dbt_cloud-0.0.3a1/src/grai_source_dbt_cloud/loader.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.0.3a1/src/grai_source_dbt_cloud/py.typed
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.0.3a1/PKG-INFO
```

### Comparing `grai_source_dbt_cloud-0.0.2/pyproject.toml` & `grai_source_dbt_cloud-0.0.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt_cloud"
-version = "0.0.2"
+version = "0.0.3-alpha1"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt_cloud", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_dbt_cloud-0.0.2/src/grai_source_dbt_cloud/base.py` & `grai_source_dbt_cloud-0.0.3a1/src/grai_source_dbt_cloud/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from grai_client.update import update
 from grai_schemas.base import Edge, Node
 from grai_source_dbt_cloud.loader import DbtCloudConnector
 
 from grai_source_dbt.adapters import adapt_to_client
 
 
+def get_events(connector: DbtCloudConnector, version: str = "v1"):
+    events = connector.get_events()
+
+    return events
+
+
 def get_nodes_and_edges(connector: DbtCloudConnector, version: str = "v1") -> Tuple[List[Node], List[Edge]]:
     nodes, edges = connector.get_nodes_and_edges()
 
     return nodes, edges
 
 
 def update_server(client: BaseClient, api_key: str, namespace: str = "default") -> None:
```

### Comparing `grai_source_dbt_cloud-0.0.2/src/grai_source_dbt_cloud/loader.py` & `grai_source_dbt_cloud-0.0.3a1/src/grai_source_dbt_cloud/loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,17 +11,51 @@
         api_key: str,
         namespace: Optional[str] = "default",
     ):
         self.api_key = api_key
         self.namespace = namespace
 
     def get_nodes_and_edges(self):
-        client = dbtCloudClient(api_key=self.api_key)
+        self.load_client()
 
-        accounts = client.cloud.list_accounts()
-        account = accounts["data"][0]
+        account = self.get_default_acount()
 
-        manifest_obj = client.cloud.get_most_recent_run_artifact(account_id=account["id"], path="manifest.json")
+        manifest_obj = self.client.cloud.get_most_recent_run_artifact(account_id=account["id"], path="manifest.json")
 
         manifest = ManifestProcessor.load(manifest_obj, self.namespace)
 
         return manifest.adapted_nodes, manifest.adapted_edges
+
+    def get_events(self):
+        self.load_client()
+
+        account = self.get_default_acount()
+
+        runs = self.get_runs(account_id=account["id"])
+
+        return runs
+
+    def load_client(self):
+        self.client = dbtCloudClient(api_key=self.api_key)
+
+    def get_default_acount(self):
+        accounts = self.client.cloud.list_accounts()
+
+        return accounts["data"][0]
+
+    def get_runs(self, account_id: str):
+        runs = []
+
+        offset = 0
+        limit = 100
+
+        while True:
+            result = self.client.cloud.list_runs(account_id=account_id, order_by="id", limit=limit, offset=offset)
+
+            runs.extend(result["data"])
+
+            if result["extra"]["pagination"]["total_count"] <= len(runs):
+                break
+
+            offset += 100
+
+        return runs
```

### Comparing `grai_source_dbt_cloud-0.0.2/PKG-INFO` & `grai_source_dbt_cloud-0.0.3a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt-cloud
-Version: 0.0.2
+Version: 0.0.3a1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

