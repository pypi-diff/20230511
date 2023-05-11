# Comparing `tmp/local-dialog-workflow-python-backend-0.0.7.tar.gz` & `tmp/local-dialog-workflow-python-backend-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-dialog-workflow-python-backend-0.0.7.tar", last modified: Thu May 11 19:53:27 2023, max compression
+gzip compressed data, was "local-dialog-workflow-python-backend-0.0.8.tar", last modified: Thu May 11 19:57:54 2023, max compression
```

## Comparing `local-dialog-workflow-python-backend-0.0.7.tar` & `local-dialog-workflow-python-backend-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:53:27.438694 local-dialog-workflow-python-backend-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 19:53:27.438694 local-dialog-workflow-python-backend-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:53:27.434694 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    19827 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:53:27.438694 local-dialog-workflow-python-backend-0.0.7/local_dialog_workflow_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 19:53:27.000000 local-dialog-workflow-python-backend-0.0.7/local_dialog_workflow_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-11 19:53:27.000000 local-dialog-workflow-python-backend-0.0.7/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:53:27.000000 local-dialog-workflow-python-backend-0.0.7/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 19:53:27.000000 local-dialog-workflow-python-backend-0.0.7/local_dialog_workflow_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:53:27.438694 local-dialog-workflow-python-backend-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 19:53:13.000000 local-dialog-workflow-python-backend-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:54.612651 local-dialog-workflow-python-backend-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 19:57:54.608651 local-dialog-workflow-python-backend-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:54.608651 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:57:54.608651 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 19:57:54.000000 local-dialog-workflow-python-backend-0.0.8/local_dialog_workflow_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:57:54.612651 local-dialog-workflow-python-backend-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-11 19:57:43.000000 local-dialog-workflow-python-backend-0.0.8/setup.py
```

### Comparing `local-dialog-workflow-python-backend-0.0.7/dialog_workflow/Act.py` & `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Act.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from utils import *
 import time
 import msvcrt
 import requests
 from AgeDetection import DetectAge
-from TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
+from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
 
 class action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: str, profile_curr_state: int, variables: Variable):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
         self.language = language
         self.variables = variables
```

### Comparing `local-dialog-workflow-python-backend-0.0.7/dialog_workflow/Constants.py` & `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.7/dialog_workflow/DialogWorkflow.py` & `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/DialogWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dialog_workflow.utils import *
-from Act import action
-from TablesAsObjects import DialogWorkflowRecord, Variable
+from dialog_workflow.Act import action
+from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable
 
 
 def get_preferred_language(profile_id: int):
     cursor.execute("""USE profile""")
     cursor.execute("""SELECT preferred_lang_code FROM profile_view WHERE user_id = %s""", [profile_id])
     language = (cursor.fetchone())["preferred_lang_code"]
     cursor.execute("""USE dialog_workflow""")
```

### Comparing `local-dialog-workflow-python-backend-0.0.7/dialog_workflow/TablesAsObjects.py` & `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/TablesAsObjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from Constants import *
-from utils import insert_profile_variable_value, get_curr_state, get_variable_value_by_id
+from dialog_workflow.Constants import *
+from dialog_workflow.utils import insert_profile_variable_value, get_curr_state, get_variable_value_by_id
 
 class Variable(object):
     def __init__(self):
         self.name2id_dict = {}
         self.id2name_dict = {}
         self.next_variable_id = 1
         for variable_id in VARIABLE_NAMES_DICT:
```

### Comparing `local-dialog-workflow-python-backend-0.0.7/dialog_workflow/test.py` & `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `local-dialog-workflow-python-backend-0.0.7/dialog_workflow/utils.py` & `local-dialog-workflow-python-backend-0.0.8/dialog_workflow/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # TODO: Let's talk about Constants and the usage in this file
-from Constants import *
+from dialog_workflow.Constants import *
 import random
 import json
 from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
 
 # TOOD: Please include type to all parameters.
 # TODO: Please include return value.
 # TODO: Please add short documentation per PEP8 standard
```

### Comparing `local-dialog-workflow-python-backend-0.0.7/setup.py` & `local-dialog-workflow-python-backend-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='local-dialog-workflow-python-backend',  
-     version='0.0.7',
+     version='0.0.8',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

