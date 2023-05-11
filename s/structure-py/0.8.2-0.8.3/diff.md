# Comparing `tmp/structure_py-0.8.2.tar.gz` & `tmp/structure_py-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structure_py-0.8.2.tar", last modified: Wed May 10 00:59:00 2023, max compression
+gzip compressed data, was "structure_py-0.8.3.tar", last modified: Thu May 11 00:59:16 2023, max compression
```

## Comparing `structure_py-0.8.2.tar` & `structure_py-0.8.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.641739 structure_py-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 00:58:44.000000 structure_py-0.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-10 00:59:00.641739 structure_py-0.8.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3702 2023-05-10 00:58:44.000000 structure_py-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 00:59:00.641739 structure_py-0.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-05-10 00:58:44.000000 structure_py-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.637739 structure_py-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.637739 structure_py-0.8.2/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4634 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/companies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.637739 structure_py-0.8.2/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.641739 structure_py-0.8.2/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/enrich_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/enrich_person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/list_employees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/list_jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/list_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/login.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/me.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/search_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/operations/search_people.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.641739 structure_py-0.8.2/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2597 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7409 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/shared/person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2705 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/people.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.641739 structure_py-0.8.2/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25963 2023-05-10 00:58:44.000000 structure_py-0.8.2/src/sdk/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:59:00.641739 structure_py-0.8.2/src/structure_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-10 00:59:00.000000 structure_py-0.8.2/src/structure_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-10 00:59:00.000000 structure_py-0.8.2/src/structure_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:59:00.000000 structure_py-0.8.2/src/structure_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-10 00:59:00.000000 structure_py-0.8.2/src/structure_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 00:59:00.000000 structure_py-0.8.2/src/structure_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.539112 structure_py-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 00:59:06.000000 structure_py-0.8.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-11 00:59:16.539112 structure_py-0.8.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3702 2023-05-11 00:59:06.000000 structure_py-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:59:16.539112 structure_py-0.8.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-05-11 00:59:06.000000 structure_py-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.531112 structure_py-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.535112 structure_py-0.8.3/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4634 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/companies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.535112 structure_py-0.8.3/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.535112 structure_py-0.8.3/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/enrich_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/enrich_person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/list_employees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/list_jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/list_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/login.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/me.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/search_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/operations/search_people.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.539112 structure_py-0.8.3/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2597 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7409 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/shared/person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2705 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/people.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.539112 structure_py-0.8.3/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25963 2023-05-11 00:59:06.000000 structure_py-0.8.3/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:59:16.539112 structure_py-0.8.3/src/structure_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-11 00:59:16.000000 structure_py-0.8.3/src/structure_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-11 00:59:16.000000 structure_py-0.8.3/src/structure_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:59:16.000000 structure_py-0.8.3/src/structure_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 00:59:16.000000 structure_py-0.8.3/src/structure_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 00:59:16.000000 structure_py-0.8.3/src/structure_py.egg-info/top_level.txt
```

### Comparing `structure_py-0.8.2/LICENSE.md` & `structure_py-0.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/PKG-INFO` & `structure_py-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure_py
-Version: 0.8.2
+Version: 0.8.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure_py Version: 0.8.2 Summary: Python Client
+Metadata-Version: 2.1 Name: structure_py Version: 0.8.3 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
```

### Comparing `structure_py-0.8.2/README.md` & `structure_py-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/setup.py` & `structure_py-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="structure_py",
-    version="0.8.2",
+    version="0.8.3",
     author="Structure",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `structure_py-0.8.2/src/sdk/accounts.py` & `structure_py-0.8.3/src/sdk/accounts.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/companies.py` & `structure_py-0.8.3/src/sdk/companies.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/__init__.py` & `structure_py-0.8.3/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/enrich_company.py` & `structure_py-0.8.3/src/sdk/models/operations/enrich_company.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/enrich_person.py` & `structure_py-0.8.3/src/sdk/models/operations/enrich_person.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/list_employees.py` & `structure_py-0.8.3/src/sdk/models/operations/list_employees.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/list_jobs.py` & `structure_py-0.8.3/src/sdk/models/operations/list_jobs.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/login.py` & `structure_py-0.8.3/src/sdk/models/operations/login.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/search_companies.py` & `structure_py-0.8.3/src/sdk/models/operations/search_companies.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/operations/search_people.py` & `structure_py-0.8.3/src/sdk/models/operations/search_people.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/shared/account.py` & `structure_py-0.8.3/src/sdk/models/shared/account.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/shared/company.py` & `structure_py-0.8.3/src/sdk/models/shared/company.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/models/shared/person.py` & `structure_py-0.8.3/src/sdk/models/shared/person.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/people.py` & `structure_py-0.8.3/src/sdk/people.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/sdk.py` & `structure_py-0.8.3/src/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     user: User
     r"""User"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.8.2"
-    _gen_version: str = "2.26.2"
+    _sdk_version: str = "0.8.3"
+    _gen_version: str = "2.26.3"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `structure_py-0.8.2/src/sdk/user.py` & `structure_py-0.8.3/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/utils/retries.py` & `structure_py-0.8.3/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/sdk/utils/utils.py` & `structure_py-0.8.3/src/sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.8.2/src/structure_py.egg-info/PKG-INFO` & `structure_py-0.8.3/src/structure_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure-py
-Version: 0.8.2
+Version: 0.8.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure-py Version: 0.8.2 Summary: Python Client
+Metadata-Version: 2.1 Name: structure-py Version: 0.8.3 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
```

### Comparing `structure_py-0.8.2/src/structure_py.egg-info/SOURCES.txt` & `structure_py-0.8.3/src/structure_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

