# Comparing `tmp/local-dialog-workflow-python-backend-0.0.8.tar.gz` & `tmp/local-dialog-workflow-python-backend-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-dialog-workflow-python-backend-0.0.8.tar", last modified: Thu May 11 19:57:54 2023, max compression
+gzip compressed data, was "local-dialog-workflow-python-backend-0.0.9.tar", last modified: Thu May 11 20:02:56 2023, max compression
```

## Comparing `local-dialog-workflow-python-backend-0.0.8.tar` & `local-dialog-workflow-python-backend-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:54.612651 local-dialog-workflow-python-backend-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 19:57:54.608651 local-dialog-workflow-python-backend-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:54.608651 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:54.608651 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:57:54.612651 local-dialog-workflow-python-backend-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:02:56.637659 local-dialog-workflow-python-backend-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 20:02:56.637659 local-dialog-workflow-python-backend-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:02:56.637659 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:02:56.637659 local-dialog-workflow-python-backend-0.0.9/local_dialog_workflow_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 20:02:56.000000 local-dialog-workflow-python-backend-0.0.9/local_dialog_workflow_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-11 20:02:56.000000 local-dialog-workflow-python-backend-0.0.9/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:02:56.000000 local-dialog-workflow-python-backend-0.0.9/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 20:02:56.000000 local-dialog-workflow-python-backend-0.0.9/local_dialog_workflow_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:02:56.637659 local-dialog-workflow-python-backend-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 20:02:42.000000 local-dialog-workflow-python-backend-0.0.9/setup.py
```

### Comparing `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Act.py` & `local-dialog-workflow-python-backend-0.0.9/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Constants.py` & `local-dialog-workflow-python-backend-0.0.9/dialog_workflow/Constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,10 +29,17 @@
                        5 : "Name Prefix", 6 : "First Name", 7 : "Middle Name" , 
                        8 : "Last Name", 9 : "Name Suffix",  10 : "Full Name", 
                        11 : "Country", 12 : "State" , 13 : "County" , 14 : "City", 
                        15 : "Neighborhood", 16 : "Street", 17 : "House", 18 : "Suite/Apartment", 
                        19 : "Zip Code", 20 : "Post Result", 21 : "Age", 22 : "Result"}
 
 ACTIVE_PROFILE_ID  = 1
-connection = database().connect_to_database()
+# connection = database().connect_to_database()
+import os
+import mysql.connector
+connection = mysql.connector.connect(
+        host=os.getenv("RDS_HOSTNAME"),
+        user=os.getenv("RDS_USERNAME"),
+        password=os.getenv("RDS_PASSWORD")
+        )
 cursor = connection.cursor(dictionary=True, buffered=True)
 cursor.execute("""USE dialog_workflow""")
```

### Comparing `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/DialogWorkflow.py` & `local-dialog-workflow-python-backend-0.0.9/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/TablesAsObjects.py` & `local-dialog-workflow-python-backend-0.0.9/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/test.py` & `local-dialog-workflow-python-backend-0.0.9/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/utils.py` & `local-dialog-workflow-python-backend-0.0.9/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.8/setup.py` & `local-dialog-workflow-python-backend-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='local-dialog-workflow-python-backend',  
-     version='0.0.8',
+     version='0.0.9',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

