# Comparing `tmp/databricks_sql_cli-0.3.1.tar.gz` & `tmp/databricks_sql_cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_cli-0.3.1.tar", max compression
+gzip compressed data, was "databricks_sql_cli-0.3.2.tar", max compression
```

## Comparing `databricks_sql_cli-0.3.1.tar` & `databricks_sql_cli-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     3466 2023-04-24 20:44:11.649621 databricks_sql_cli-0.3.1/LICENSE
--rw-r--r--   0        0        0     3512 2023-04-24 20:44:11.649621 databricks_sql_cli-0.3.1/README.md
--rw-r--r--   0        0        0       22 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/clibuffer.py
--rw-r--r--   0        0        0     4681 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/clistyle.py
--rw-r--r--   0        0        0     1504 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/clitoolbar.py
--rw-r--r--   0        0        0      137 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/compat.py
--rw-r--r--   0        0        0    15034 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/completer.py
--rw-r--r--   0        0        0     4332 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/completion_refresher.py
--rw-r--r--   0        0        0     2085 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/config.py
--rw-r--r--   0        0        0     3298 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/dbsqlclirc
--rw-r--r--   0        0        0     2254 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/key_bindings.py
--rw-r--r--   0        0        0      288 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/lexer.py
--rw-r--r--   0        0        0    26041 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/main.py
--rw-r--r--   0        0        0        0 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/__init__.py
--rw-r--r--   0        0        0    12595 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/completion_engine.py
--rw-r--r--   0        0        0     1713 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/filepaths.py
--rw-r--r--   0        0        0      892 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/format_utils.py
--rw-r--r--   0        0        0        0 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/literals/__init__.py
--rw-r--r--   0        0        0    10151 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/literals/main.py
--rw-r--r--   0        0        0     7976 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/parseutils.py
--rw-r--r--   0        0        0     1065 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/prompt_utils.py
--rw-r--r--   0        0        0      247 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/dbcommands.py
--rw-r--r--   0        0        0     2093 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/favoritequeries.py
--rw-r--r--   0        0        0    14399 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/iocommands.py
--rw-r--r--   0        0        0     4228 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/main.py
--rw-r--r--   0        0        0     1440 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/tabular_output/__init__.py
--rw-r--r--   0        0        0     1935 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/tabular_output/sql_format.py
--rw-r--r--   0        0        0     6734 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/sqlexecute.py
--rw-r--r--   0        0        0      867 2023-04-24 20:44:37.525833 databricks_sql_cli-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4585 1970-01-01 00:00:00.000000 databricks_sql_cli-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3466 2023-05-11 16:02:31.955474 databricks_sql_cli-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3512 2023-05-11 16:02:31.955474 databricks_sql_cli-0.3.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/__init__.py
+-rw-r--r--   0        0        0     1256 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/clibuffer.py
+-rw-r--r--   0        0        0     4681 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/clistyle.py
+-rw-r--r--   0        0        0     1504 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/clitoolbar.py
+-rw-r--r--   0        0        0      137 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/compat.py
+-rw-r--r--   0        0        0    15034 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/completer.py
+-rw-r--r--   0        0        0     4332 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/completion_refresher.py
+-rw-r--r--   0        0        0     2085 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/config.py
+-rw-r--r--   0        0        0     3298 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/dbsqlclirc
+-rw-r--r--   0        0        0     2254 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/key_bindings.py
+-rw-r--r--   0        0        0      288 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/lexer.py
+-rw-r--r--   0        0        0    26052 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/main.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/__init__.py
+-rw-r--r--   0        0        0    12595 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/completion_engine.py
+-rw-r--r--   0        0        0     1713 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/filepaths.py
+-rw-r--r--   0        0        0      892 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/format_utils.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/literals/__init__.py
+-rw-r--r--   0        0        0    10151 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/literals/main.py
+-rw-r--r--   0        0        0     7976 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/parseutils.py
+-rw-r--r--   0        0        0     1065 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/prompt_utils.py
+-rw-r--r--   0        0        0      247 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/special/__init__.py
+-rw-r--r--   0        0        0     1198 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/special/dbcommands.py
+-rw-r--r--   0        0        0     2093 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/special/favoritequeries.py
+-rw-r--r--   0        0        0    14399 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/special/iocommands.py
+-rw-r--r--   0        0        0     4228 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/special/main.py
+-rw-r--r--   0        0        0     1440 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/special/utils.py
+-rw-r--r--   0        0        0        0 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/tabular_output/__init__.py
+-rw-r--r--   0        0        0     1935 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/packages/tabular_output/sql_format.py
+-rw-r--r--   0        0        0     6734 2023-05-11 16:02:31.971475 databricks_sql_cli-0.3.2/dbsqlcli/sqlexecute.py
+-rw-r--r--   0        0        0      867 2023-05-11 16:02:57.539830 databricks_sql_cli-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4585 1970-01-01 00:00:00.000000 databricks_sql_cli-0.3.2/PKG-INFO
```

### Comparing `databricks_sql_cli-0.3.1/LICENSE` & `databricks_sql_cli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/README.md` & `databricks_sql_cli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/clibuffer.py` & `databricks_sql_cli-0.3.2/dbsqlcli/clibuffer.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/clistyle.py` & `databricks_sql_cli-0.3.2/dbsqlcli/clistyle.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/clitoolbar.py` & `databricks_sql_cli-0.3.2/dbsqlcli/clitoolbar.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/completer.py` & `databricks_sql_cli-0.3.2/dbsqlcli/completer.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/completion_refresher.py` & `databricks_sql_cli-0.3.2/dbsqlcli/completion_refresher.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/config.py` & `databricks_sql_cli-0.3.2/dbsqlcli/config.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/dbsqlclirc` & `databricks_sql_cli-0.3.2/dbsqlcli/dbsqlclirc`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/key_bindings.py` & `databricks_sql_cli-0.3.2/dbsqlcli/key_bindings.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/main.py` & `databricks_sql_cli-0.3.2/dbsqlcli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 def apply_credentials_from_cfg(hostname, http_path, access_token, auth_type, cfg):
     """
     Returns http_path, hostname, access_token and auth_type from the passed configuration or from clirc file.
     """
 
     if not cfg.get("credentials"):
-        return hostname, http_path, access_token
+        return hostname, http_path, access_token, auth_type
 
     hostname = hostname or cfg.get("credentials", {}).get("host_name")
     http_path = http_path or cfg.get("credentials", {}).get("http_path")
     access_token = access_token or cfg.get("credentials", {}).get("access_token")
     auth_type = auth_type or cfg.get("credentials", {}).get("auth_type")
 
     return hostname, http_path, access_token, auth_type
```

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/completion_engine.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/completion_engine.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/filepaths.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/filepaths.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/format_utils.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/format_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/literals/main.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/literals/main.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/parseutils.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/parseutils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/prompt_utils.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/dbcommands.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/special/dbcommands.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/favoritequeries.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/special/favoritequeries.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/iocommands.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/special/iocommands.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/main.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/special/main.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/utils.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/special/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/packages/tabular_output/sql_format.py` & `databricks_sql_cli-0.3.2/dbsqlcli/packages/tabular_output/sql_format.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/dbsqlcli/sqlexecute.py` & `databricks_sql_cli-0.3.2/dbsqlcli/sqlexecute.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.1/pyproject.toml` & `databricks_sql_cli-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-cli"
-version = "0.3.1"
+version = "0.3.2"
 description = "A DBCLI client for Databricks SQL"
 authors = ["Databricks SQL CLI Maintainers <dbsqlcli-maintainers@databricks.com>"]
 packages = [{include = "dbsqlcli"}]
 readme = "README.md"
 license = "proprietary"
 
 [tool.poetry.dependencies]
```

### Comparing `databricks_sql_cli-0.3.1/PKG-INFO` & `databricks_sql_cli-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-cli
-Version: 0.3.1
+Version: 0.3.2
 Summary: A DBCLI client for Databricks SQL
 License: Proprietary
 Author: Databricks SQL CLI Maintainers
 Author-email: dbsqlcli-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

