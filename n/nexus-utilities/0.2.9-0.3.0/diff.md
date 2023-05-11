# Comparing `tmp/nexus-utilities-0.2.9.tar.gz` & `tmp/nexus-utilities-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.2.9.tar", last modified: Wed May 10 16:25:55 2023, max compression
+gzip compressed data, was "nexus-utilities-0.3.0.tar", last modified: Thu May 11 20:59:28 2023, max compression
```

## Comparing `nexus-utilities-0.2.9.tar` & `nexus-utilities-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:55.483606 nexus-utilities-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 16:25:55.483606 nexus-utilities-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:55.479606 nexus-utilities-0.2.9/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:55.479606 nexus-utilities-0.2.9/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:25:55.483606 nexus-utilities-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:59:28.044417 nexus-utilities-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-11 20:59:28.044417 nexus-utilities-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:59:28.044417 nexus-utilities-0.3.0/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-11 20:59:27.000000 nexus-utilities-0.3.0/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-11 20:59:28.000000 nexus-utilities-0.3.0/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:59:27.000000 nexus-utilities-0.3.0/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 20:59:27.000000 nexus-utilities-0.3.0/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 20:59:27.000000 nexus-utilities-0.3.0/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:59:28.044417 nexus-utilities-0.3.0/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:59:28.044417 nexus-utilities-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-11 20:59:14.000000 nexus-utilities-0.3.0/setup.py
```

### Comparing `nexus-utilities-0.2.9/LICENSE.txt` & `nexus-utilities-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.9/PKG-INFO` & `nexus-utilities-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.9
+Version: 0.3.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.9/README.md` & `nexus-utilities-0.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -13,14 +13,16 @@
   - [**get\_current\_timestamp()**](#get_current_timestamp)
   - [**getDuration(then, now=datetime.datetime.now())**](#getdurationthen-nowdatetimedatetimenow)
 - [package\_utils.py](#package_utilspy)
   - [**add\_package\_to\_path()**](#add_package_to_path)
   - [**import\_relative(package\_root\_name, module\_path, import\_name, alias=None)**](#import_relativepackage_root_name-module_path-import_name-aliasnone)
 - [password\_utils.py](#password_utilspy)
   - [**get\_password(password\_method, password\_key, account\_name=None, access\_key=None, secret\_key=None, endpoint\_url=None, region\_name=None, password\_path=None, encoding='utf-8')**](#get_passwordpassword_method-password_key-account_namenone-access_keynone-secret_keynone-endpoint_urlnone-region_namenone-password_pathnone-encodingutf-8)
+- [string\_utils.py](#string_utilspy)
+  - [**cleanse\_string(string, remove\_symbols=True, title\_to\_snake\_case=False, hyphen\_to\_underscore=True, period\_to\_underscore=True, to\_upper=False, to\_lower=True)**](#cleanse_stringstring-remove_symbolstrue-title_to_snake_casefalse-hyphen_to_underscoretrue-period_to_underscoretrue-to_upperfalse-to_lowertrue)
 - [About the Author](#about-the-author)
 
 ---
 
 ## Installation
 
 ```python
@@ -193,12 +195,42 @@
 endpoint_url = 'AWS_SM_ENDPOINT_URL'
 region_name = 'AWS_SM_REGION_NAME'
 password_key = 'AWS_SM_PASSWORD_KEY'
 ```
 
 ---
 
+## string_utils.py
+
+This module contains functions for working with strings.
+
+### **cleanse_string(string, remove_symbols=True, title_to_snake_case=False, hyphen_to_underscore=True, period_to_underscore=True, to_upper=False, to_lower=True)**
+
+Arguments:
+ * ***string (str):*** String to be cleansed
+ * ***remove_symbols (bool):*** Remove some symbols, and replace others with "_"
+ * ***title_to_snake_case (bool):*** Convert TitleCase to Snake_Case
+ * ***hyphen_to_underscore (bool):*** Change hypehens to underscores
+ * ***period_to_underscore (bool):*** Change periods to underscores
+ * ***to_upper (bool):*** Change string to uppercase
+ * ***to_lower (bool):*** Change string to lowercase
+
+Returns:
+ * ***string (str):*** Transformed string value
+
+Below is additional details about what each transformation does:
+ * ***remove_symbols*** - Removes or converts to "_" based on the below rules.  Will also attempt to preserve multiple underscores in the original field without adding to them (using the '†' symbol).  Eg. "Field__(Name)" will become "Field__Name", not "Field___Name"
+     * characters_to_replace_with_underscore  
+' ', ':', ';', '&', '@', '^', '+', '=', '~', '/', '\\', '|', '(', '{', '[', '<'
+     * characters_to_remove  
+',', '`', '#', '$', '%', '*', ''', '"', '?', '!', ')', '}', ']', '>'
+ * ***title_to_snake_case*** - Convert TitleCase to SnakeCase.  Attempts to account for clusters of uppercase letters.  For example, "SalesForNBCUniversal" will return "sales_for_nbc_universal"
+ * ***hyphen_to_underscore*** - Converts "-" to "_", otherwise leaves them alone
+ * ***period_to_underscore*** - Converts "." to "_", otherwise leaves them alone
+ * ***to_upper*** - Converts string to UPPERCASE
+ * ***to_lower*** - Converts string to lowercase, takes precedence over "to_upper"
+
 ## About the Author
 
 My name is James Larsen, and I have been working professionally as a Business Analyst, Database Architect and Data Engineer since 2007.  While I specialize in Data Modeling and SQL, I am working to improve my knowledge in different data engineering technologies, particularly Python.
 
 [https://www.linkedin.com/in/jameslarsen42/](https://www.linkedin.com/in/jameslarsen42/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nexus-utilities-0.2.9/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.3.0/nexus_utilities.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.9
+Version: 0.3.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.9/nexus_utils/config_utils.py` & `nexus-utilities-0.3.0/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.9/nexus_utils/database_utils.py` & `nexus-utilities-0.3.0/nexus_utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.9/nexus_utils/datetime_utils.py` & `nexus-utilities-0.3.0/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.9/nexus_utils/package_utils.py` & `nexus-utilities-0.3.0/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.9/nexus_utils/password_utils.py` & `nexus-utilities-0.3.0/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.9/setup.py` & `nexus-utilities-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.2.9',
+    version='0.3.0',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

