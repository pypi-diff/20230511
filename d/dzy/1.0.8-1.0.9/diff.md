# Comparing `tmp/dzy-1.0.8.tar.gz` & `tmp/dzy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dzy-1.0.8.tar", last modified: Tue Aug 31 18:53:51 2021, max compression
+gzip compressed data, was "dist/dzy-1.0.9.tar", last modified: Tue Aug 31 21:35:15 2021, max compression
```

## Comparing `dzy-1.0.8.tar` & `dzy-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 18:53:51.000000 dzy-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      185 2021-08-31 18:53:51.000000 dzy-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1641 2021-08-31 18:53:32.000000 dzy-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 18:53:51.000000 dzy-1.0.8/dzy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 18:53:32.000000 dzy-1.0.8/dzy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14208 2021-08-31 18:53:32.000000 dzy-1.0.8/dzy/dw.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2021-08-31 18:53:32.000000 dzy-1.0.8/dzy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 18:53:51.000000 dzy-1.0.8/dzy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      185 2021-08-31 18:53:51.000000 dzy-1.0.8/dzy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      229 2021-08-31 18:53:51.000000 dzy-1.0.8/dzy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-31 18:53:51.000000 dzy-1.0.8/dzy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2021-08-31 18:53:51.000000 dzy-1.0.8/dzy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-08-31 18:53:51.000000 dzy-1.0.8/dzy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-31 18:53:51.000000 dzy-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      441 2021-08-31 18:53:32.000000 dzy-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 18:53:51.000000 dzy-1.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 18:53:32.000000 dzy-1.0.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2021-08-31 18:53:32.000000 dzy-1.0.8/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 21:35:15.000000 dzy-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      185 2021-08-31 21:35:15.000000 dzy-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2021-08-31 21:34:50.000000 dzy-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 21:35:15.000000 dzy-1.0.9/dzy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 21:34:50.000000 dzy-1.0.9/dzy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14625 2021-08-31 21:34:50.000000 dzy-1.0.9/dzy/dw.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2021-08-31 21:34:50.000000 dzy-1.0.9/dzy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 21:35:15.000000 dzy-1.0.9/dzy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      185 2021-08-31 21:35:14.000000 dzy-1.0.9/dzy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      229 2021-08-31 21:35:14.000000 dzy-1.0.9/dzy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-31 21:35:14.000000 dzy-1.0.9/dzy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2021-08-31 21:35:14.000000 dzy-1.0.9/dzy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-08-31 21:35:14.000000 dzy-1.0.9/dzy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-31 21:35:15.000000 dzy-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      441 2021-08-31 21:34:50.000000 dzy-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-31 21:35:15.000000 dzy-1.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-31 21:34:50.000000 dzy-1.0.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2021-08-31 21:34:50.000000 dzy-1.0.9/tests/test_utils.py
```

### Comparing `dzy-1.0.8/README.md` & `dzy-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dzy-1.0.8/dzy/dw.py` & `dzy-1.0.9/dzy/dw.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,21 +404,25 @@
         self,
         dataset_name: str,
         table_name: str
     ):
         """
         Empty the table but preserve structure.
         """
-        sql = f"""
-            DELETE FROM `{dataset_name}.{table_name}` WHERE TRUE
-        """
-        job_config = bigquery.QueryJobConfig()
-        load_job = self.client.query(sql, job_config=job_config)
-        load_job.result()
-        print(f"Emptied table '{dataset_name}.{table_name}'")
+        table_id = f"{self.project}.{dataset_name}.{table_name}"
+        if self.client.get_table(table_id):
+            sql = f"""
+                DELETE FROM `{dataset_name}.{table_name}` WHERE TRUE
+            """
+            job_config = bigquery.QueryJobConfig()
+            load_job = self.client.query(sql, job_config=job_config)
+            load_job.result()
+            print(f"Emptied table '{dataset_name}.{table_name}'")
+        else:
+            print(f"Table '{dataset_name}.{table_name}' is empty")
 
     # gcs to bq ingestion
     def load_gcs_json_to_bq(
             self,
             uri: str,
             dataset_name: str,
             table_name: str,
@@ -428,23 +432,28 @@
         """
         Load a CSV file from Cloud Storage using an explicit schema.
         """
         table_id = f"{self.project}.{dataset_name}.{table_name}"
         if self.check_table_exists(dataset_name, table_name, returns=True):
             uri = f"gs://{uri}"
             job_config = bigquery.LoadJobConfig(
-                source_format=bigquery.SourceFormat.NEWLINE_DELIMITED_JSON
+                source_format=bigquery.SourceFormat.NEWLINE_DELIMITED_JSON,
+                schema_update_options=[
+                    "ALLOW_FIELD_ADDITION",
+                    "ALLOW_FIELD_RELAXATION"
+                ],
+                write_disposition="WRITE_TRUNCATE"
             )
             if schema:
                 job_config.schema = schema
             else:
                 job_config.autodetect = True
 
-            if not append:
-                self.empty_table(dataset_name, table_name)
+            if append:
+                job_config.write_disposition = "WRITE_APPEND"
 
             load_job = self.client.load_table_from_uri(
                 uri,
                 table_id,
                 location=self.location,
                 job_config=job_config
             )
```

