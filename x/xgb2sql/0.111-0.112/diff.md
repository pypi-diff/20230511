# Comparing `tmp/xgb2sql-0.111.tar.gz` & `tmp/xgb2sql-0.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xgb2sql-0.111.tar", last modified: Tue Jan 28 15:25:21 2020, max compression
+gzip compressed data, was "xgb2sql-0.112.tar", last modified: Thu May 11 18:42:54 2023, max compression
```

## Comparing `xgb2sql-0.111.tar` & `xgb2sql-0.112.tar`

### file list

```diff
@@ -1,7 +1,18 @@
-drwxr-xr-x   0 benjamin.jiang   (503) staff       (20)        0 2020-01-28 15:25:21.000000 xgb2sql-0.111/
--rw-r--r--   0 benjamin.jiang   (503) staff       (20)      687 2020-01-28 15:25:21.000000 xgb2sql-0.111/PKG-INFO
--rw-r--r--   0 benjamin.jiang   (503) staff       (20)       39 2020-01-25 19:18:00.000000 xgb2sql-0.111/setup.cfg
--rw-r--r--   0 benjamin.jiang   (503) staff       (20)      809 2020-01-28 15:25:18.000000 xgb2sql-0.111/setup.py
-drwxr-xr-x   0 benjamin.jiang   (503) staff       (20)        0 2020-01-28 15:25:21.000000 xgb2sql-0.111/xgb2sql/
--rw-r--r--   0 benjamin.jiang   (503) staff       (20)       26 2020-01-28 15:23:48.000000 xgb2sql-0.111/xgb2sql/__init__.py
--rw-r--r--   0 benjamin.jiang   (503) staff       (20)     7002 2020-01-27 20:07:11.000000 xgb2sql-0.111/xgb2sql/main.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-11 18:42:54.786851 xgb2sql-0.112/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     2348 2023-03-13 17:57:29.000000 xgb2sql-0.112/CONTRIBUTING.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)    11357 2023-03-13 17:09:07.000000 xgb2sql-0.112/LICENSE
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      111 2023-03-13 17:09:07.000000 xgb2sql-0.112/MANIFEST.in
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-11 18:42:54.786634 xgb2sql-0.112/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7514 2023-05-11 17:03:06.000000 xgb2sql-0.112/README.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1752 2023-05-11 18:42:10.000000 xgb2sql-0.112/settings.ini
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       38 2023-05-11 18:42:54.786891 xgb2sql-0.112/setup.cfg
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1911 2023-05-11 18:25:54.000000 xgb2sql-0.112/setup.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-11 18:42:54.785551 xgb2sql-0.112/xgb2sql/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       22 2023-03-13 18:30:03.000000 xgb2sql-0.112/xgb2sql/__init__.py
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7281 2023-05-11 17:38:08.000000 xgb2sql-0.112/xgb2sql/core.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-11 18:42:54.786458 xgb2sql-0.112/xgb2sql.egg-info/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      257 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:39:29.000000 xgb2sql-0.112/xgb2sql.egg-info/not-zip-safe
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        8 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xgb2sql-0.111/xgb2sql/main.py` & `xgb2sql-0.112/xgb2sql/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 import json
+from typing import List
 
 
-def xgb2sql(xgb_booster, table_name, index_list=[], sql_type=None):
+def xgb2sql(xgb_booster, table_name: str, index_list=[], sql_type=None):
     """
-    Takes in an XGB Booster and converts it to a SQL query. 
+    Takes in an XGB Booster and converts it to a SQL query.
     Look, I'm not saying you should use this, but I'm saying it now exists.
-    
+    I imagine any sort of tree based model could be relatively easily converted to a SQL query using this.
+
     Parameters
     ----------
     xgb_booster: xgboost.core.Booster
         https://xgboost.readthedocs.io/en/latest/tutorials/model.html
     table_name: str
-        The name of the SQL table to query from.
+        The name of the SQL table to query from. Obviously this table must be the same as the model inputs or else it won't work.
     index_list : list
-        Anything in the list will be passed through as a column in your final output. 
+        Anything in the list will be passed through as a column in your final output.
     sql_type : str
-        If there's a better way native to the sql_type to generate the code, it will be used. 
-        Otherwise defaults to PostgreSQL compliant code. 
+        If there's a better way native to the sql_type to generate the code, it will be used.
+        Otherwise defaults to PostgreSQL compliant code.
     """
 
-    def _json_parse(xgb_booster):
+    def _json_parse(xgb_booster) -> str:
 
         ret = xgb_booster.get_dump(dump_format="json")
 
         json_string = "[\n"
         for i, _ in enumerate(ret):
             json_string = json_string + ret[i]
             if i < len(ret) - 1:
                 json_string = json_string + ",\n"
         json_string = json_string + "\n]"
 
         return json.loads(json_string)
 
-    def _psql_eval(index_list, leaf_list):
+    def _psql_eval(index_list: List[str], leaf_list: List) -> str:
 
         column_string = "\n\t+ ".join(columns)
         if len(index_list) > 0:
             query = f"""\nSELECT
-    {index_string},       
+    {index_string},
     1 / ( 1 + EXP ( - (
     {column_string}) ) ) AS score
 FROM booster_output"""
         else:
-            query = f"""\nSELECT 
-    1 / ( 1 + EXP ( - ( 
+            query = f"""\nSELECT
+    1 / ( 1 + EXP ( - (
     {column_string} ) ) ) AS score
 FROM booster_output"""
 
         return query
 
-    def _bq_eval(index_list):
-        def _string_parse(index_list):
+    def _bq_eval(index_list: List[str]) -> str:
+        def _string_parse(index_list: List[str]) -> str:
 
             a = ["'" + i + "'" for i in index_list]
             return ",".join(a)
 
         if len(index_list) > 0:
             query = f""",
 
@@ -71,25 +73,25 @@
         REGEXP_REPLACE(SUBSTR(pairs, 1, STRPOS(pairs, ':') - 1), '^"|"$', '') AS variable_name,
         REGEXP_REPLACE(SUBSTR(pairs, STRPOS(pairs, ':') + 1, LENGTH(pairs)), '^"|"$', '') AS value
     FROM json_collapsed, UNNEST(SPLIT(REGEXP_REPLACE(json_text, '^{{|}}$', ''), ',"')) pairs
 )
 
 SELECT
     {index_string},
-    1 / ( 1 + EXP ( - SUM ( CAST ( value AS FLOAT64 ) ) ) ) AS score
+    1 / ( 1 + EXP ( - SUM ( CAST ( value AS FLOAT64 ) ) ) ) AS score,
 FROM unnested
 WHERE variable_name NOT IN (
     {_string_parse(index_list)}
 )
 GROUP BY {index_string}
 """
 
         else:
             query = f""",
-    
+
 json_collapsed AS (
     SELECT
         TO_JSON_STRING(branching) AS json_text
     FROM booster_output
 ),
 
 unnested AS (
@@ -142,19 +144,19 @@
                 for item in obj:
                     _extract(item, arr, key, prev)
             return key_dict
 
         results = _extract(obj, arr, key)
         return results, info_dict
 
-    def _recurse_backwards(first_node):
+    def _recurse_backwards(first_node) -> str:
 
-        query_list = []
+        query_list: List[str] = []
 
-        def _recurse(x):
+        def _recurse(x) -> None:
 
             prev_node = x
             next_node = splits[prev_node]["parent"]
             try:
                 node = splits[next_node]
                 if (node["if_less_than"] == prev_node) & (
                     node["if_less_than"] == node["if_null"]
@@ -173,15 +175,15 @@
                     query_list.insert(0, text)
                     _recurse(next_node)
                 elif node["if_greater_than"] == prev_node:
                     text = f"({node['split_column']} >= {node['split_number']})"
                     query_list.insert(0, text)
                     _recurse(next_node)
             except:
-                pass
+                query_list.insert(0, "TRUE = TRUE")
 
         _recurse(first_node)
 
         s = "\n\t\t\tAND "
 
         return s.join(query_list)
 
@@ -218,12 +220,11 @@
     else:
         output = _psql_eval(index_list, leaf_list)
 
     query = (
         "WITH booster_output AS (\n\tSELECT\n"
         + ", \n".join((index_list + leaf_list))
         + f"\n\tFROM {table_name}"
-        + f"\n\tWHERE source = 'test'\n)"
         + f"\n{output}"
     )
 
     return query
```

