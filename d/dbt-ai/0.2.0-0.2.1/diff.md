# Comparing `tmp/dbt-ai-0.2.0.tar.gz` & `tmp/dbt-ai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.2.0.tar", last modified: Wed May 10 03:46:17 2023, max compression
+gzip compressed data, was "dbt-ai-0.2.1.tar", last modified: Thu May 11 13:24:42 2023, max compression
```

## Comparing `dbt-ai-0.2.0.tar` & `dbt-ai-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.900000 dbt-ai-0.2.0/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1069 2023-05-07 00:28:17.000000 dbt-ai-0.2.0/LICENSE
--rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.2.0/MANIFEST.in
--rw-r--r--   0 armalite  (1000) armalite  (1000)     4212 2023-05-10 03:46:17.900000 dbt-ai-0.2.0/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)     4012 2023-05-10 03:46:06.000000 dbt-ai-0.2.0/README.md
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.850000 dbt-ai-0.2.0/dbt_ai/
--rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.2.0/dbt_ai/__init__.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     7603 2023-05-10 03:43:35.000000 dbt-ai-0.2.0/dbt_ai/ai.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     9524 2023-05-10 03:43:35.000000 dbt-ai-0.2.0/dbt_ai/dbt.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)      565 2023-05-07 06:43:19.000000 dbt-ai-0.2.0/dbt_ai/helper.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2247 2023-05-10 03:43:35.000000 dbt-ai-0.2.0/dbt_ai/main.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.2.0/dbt_ai/py.typed
--rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.2.0/dbt_ai/report.py
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.860000 dbt-ai-0.2.0/dbt_ai/templates/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3094 2023-05-06 13:45:28.000000 dbt-ai-0.2.0/dbt_ai/templates/report_template.html
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.860000 dbt-ai-0.2.0/dbt_ai.egg-info/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     4212 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)      384 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/entry_points.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)      193 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1619 2023-05-10 03:45:40.000000 dbt-ai-0.2.0/pyproject.toml
--rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-10 03:46:17.900000 dbt-ai-0.2.0/setup.cfg
--rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:24:42.565673 dbt-ai-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4217 2023-05-11 13:24:42.565673 dbt-ai-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:24:42.565673 dbt-ai-0.2.1/dbt_ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7603 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/ai.py
+-rw-r--r--   0 root         (0) root         (0)     9524 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/dbt.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/helper.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/main.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/py.typed
+-rw-r--r--   0 root         (0) root         (0)      811 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:24:42.565673 dbt-ai-0.2.1/dbt_ai/templates/
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/dbt_ai/templates/report_template.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 13:24:42.565673 dbt-ai-0.2.1/dbt_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4217 2023-05-11 13:24:42.000000 dbt-ai-0.2.1/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-11 13:24:42.000000 dbt-ai-0.2.1/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 13:24:42.000000 dbt-ai-0.2.1/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-11 13:24:42.000000 dbt-ai-0.2.1/dbt_ai.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-11 13:24:42.000000 dbt-ai-0.2.1/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 13:24:42.000000 dbt-ai-0.2.1/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-05-11 13:24:34.000000 dbt-ai-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 13:24:42.565673 dbt-ai-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-11 13:23:40.000000 dbt-ai-0.2.1/setup.py
```

### Comparing `dbt-ai-0.2.0/LICENSE` & `dbt-ai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.0/PKG-INFO` & `dbt-ai-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.2.0
+Version: 0.2.1
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DBT AI
@@ -56,22 +56,22 @@
 For example, if you are already inside your dbt project directory, you can run:
 ```bash
 dbt-ai -f .
 ```
 
 #### Available Settings
 
-   - Database: specify which database system your dbt models are written for. Default: `snowflake`
+   - *Database:* specify which database system your dbt models are written for. Default: `snowflake`
       - `-d` / `--database`
       - Available values: `snowflake`, `postgres`, `redshift`, `bigquery`
       - Usage example: 
       ```bash
       dbt ai -f . -d snowflake
       ```
-   - Advanced Recommendation: Request for advanced recommendations. Default: No setting defaults to basic recommendations
+   - *Advanced Recommendations:* Request for advanced recommendations. Default: No setting defaults to basic recommendations
       - `-a` / `--advanced-rec`
       - Available values: Only flag required
       - Usage example: 
       ```bash
       dbt ai -f . -a 
       ```
       Or
```

### Comparing `dbt-ai-0.2.0/README.md` & `dbt-ai-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,22 @@
 For example, if you are already inside your dbt project directory, you can run:
 ```bash
 dbt-ai -f .
 ```
 
 #### Available Settings
 
-   - Database: specify which database system your dbt models are written for. Default: `snowflake`
+   - *Database:* specify which database system your dbt models are written for. Default: `snowflake`
       - `-d` / `--database`
       - Available values: `snowflake`, `postgres`, `redshift`, `bigquery`
       - Usage example: 
       ```bash
       dbt ai -f . -d snowflake
       ```
-   - Advanced Recommendation: Request for advanced recommendations. Default: No setting defaults to basic recommendations
+   - *Advanced Recommendations:* Request for advanced recommendations. Default: No setting defaults to basic recommendations
       - `-a` / `--advanced-rec`
       - Available values: Only flag required
       - Usage example: 
       ```bash
       dbt ai -f . -a 
       ```
       Or
```

### Comparing `dbt-ai-0.2.0/dbt_ai/ai.py` & `dbt-ai-0.2.1/dbt_ai/ai.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.0/dbt_ai/dbt.py` & `dbt-ai-0.2.1/dbt_ai/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.0/dbt_ai/helper.py` & `dbt-ai-0.2.1/dbt_ai/helper.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.0/dbt_ai/main.py` & `dbt-ai-0.2.1/dbt_ai/main.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.0/dbt_ai/report.py` & `dbt-ai-0.2.1/dbt_ai/report.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.0/dbt_ai/templates/report_template.html` & `dbt-ai-0.2.1/dbt_ai/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.0/dbt_ai.egg-info/PKG-INFO` & `dbt-ai-0.2.1/dbt_ai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.2.0
+Version: 0.2.1
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DBT AI
@@ -56,22 +56,22 @@
 For example, if you are already inside your dbt project directory, you can run:
 ```bash
 dbt-ai -f .
 ```
 
 #### Available Settings
 
-   - Database: specify which database system your dbt models are written for. Default: `snowflake`
+   - *Database:* specify which database system your dbt models are written for. Default: `snowflake`
       - `-d` / `--database`
       - Available values: `snowflake`, `postgres`, `redshift`, `bigquery`
       - Usage example: 
       ```bash
       dbt ai -f . -d snowflake
       ```
-   - Advanced Recommendation: Request for advanced recommendations. Default: No setting defaults to basic recommendations
+   - *Advanced Recommendations:* Request for advanced recommendations. Default: No setting defaults to basic recommendations
       - `-a` / `--advanced-rec`
       - Available values: Only flag required
       - Usage example: 
       ```bash
       dbt ai -f . -a 
       ```
       Or
```

### Comparing `dbt-ai-0.2.0/pyproject.toml` & `dbt-ai-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
@@ -15,15 +15,14 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "black~=23.1",
     "build~=0.10",
     "pre-commit~=3.0",
-    "pytest~=7.2",
     "ruff~=0.0.254",
     "twine~=4.0",
     "pytest~=7.3",
 ]
 
 [build-system]
 requires = ["setuptools~=66.1", "wheel~=0.37"]
```

