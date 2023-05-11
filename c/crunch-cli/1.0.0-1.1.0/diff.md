# Comparing `tmp/crunch-cli-1.0.0.tar.gz` & `tmp/crunch-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.0.0.tar", last modified: Wed May 10 14:58:46 2023, max compression
+gzip compressed data, was "crunch-cli-1.1.0.tar", last modified: Wed May 10 16:25:35 2023, max compression
```

## Comparing `crunch-cli-1.0.0.tar` & `crunch-cli-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:58:46.155420 crunch-cli-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 14:58:46.155420 crunch-cli-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:58:46.151420 crunch-cli-1.0.0/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:58:46.151420 crunch-cli-1.0.0/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:58:46.155420 crunch-cli-1.0.0/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 14:58:46.000000 crunch-cli-1.0.0/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-10 14:58:46.000000 crunch-cli-1.0.0/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:58:46.000000 crunch-cli-1.0.0/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 14:58:46.000000 crunch-cli-1.0.0/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:58:46.000000 crunch-cli-1.0.0/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 14:58:46.000000 crunch-cli-1.0.0/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 14:58:46.000000 crunch-cli-1.0.0/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:58:46.155420 crunch-cli-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-10 14:58:40.000000 crunch-cli-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:35.083712 crunch-cli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 16:25:35.083712 crunch-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:35.079712 crunch-cli-1.1.0/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:35.083712 crunch-cli-1.1.0/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:35.083712 crunch-cli-1.1.0/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:35.083712 crunch-cli-1.1.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 16:25:35.000000 crunch-cli-1.1.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-10 16:25:35.000000 crunch-cli-1.1.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:25:35.000000 crunch-cli-1.1.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 16:25:35.000000 crunch-cli-1.1.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:25:35.000000 crunch-cli-1.1.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 16:25:35.000000 crunch-cli-1.1.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 16:25:35.000000 crunch-cli-1.1.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:25:35.083712 crunch-cli-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-10 16:25:26.000000 crunch-cli-1.1.0/setup.py
```

### Comparing `crunch-cli-1.0.0/crunch/command/convert.py` & `crunch-cli-1.1.0/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/command/download.py` & `crunch-cli-1.1.0/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/command/push.py` & `crunch-cli-1.1.0/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/command/setup.py` & `crunch-cli-1.1.0/crunch/command/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,59 @@
 import io
+import json
 import os
+import pkgutil
 import shutil
 import tarfile
 
 import click
 import requests
 
-from .. import constants
+from .. import api, constants
 
 
 def _check_if_already_exists(directory: str, force: bool):
     if os.path.exists(directory):
         if force:
             print(f"{directory}: deleting")
             shutil.rmtree(directory)
         else:
             print(f"{directory}: already exists (use --force to override)")
             raise click.Abort()
 
 
+def _setup_demo(directory: str):
+    def read_data(file_name):
+        resource = "/".join(["..", "demo-project", file_name])
+        return pkgutil.get_data(__package__, resource)
+
+    files = json.loads(read_data("files.json").decode("utf-8"))
+    for file in files:
+        print(f"use {file}")
+
+        content = read_data(file)
+
+        path = os.path.join(directory, file)
+        with open(path, "wb") as fd:
+            fd.write(content)
+
+
+def _setup_submission(directory: str, code_tar: io.BytesIO):
+    tar = tarfile.open(fileobj=code_tar)
+    for member in tar.getmembers():
+        path = os.path.join(directory, member.name)
+        print(f"extract {path}")
+
+        os.makedirs(os.path.dirname(path), exist_ok=True)
+
+        fileobj = tar.extractfile(member)
+        with open(path, "wb") as fd:
+            fd.write(fileobj.read())
+
+
 def setup(
     session: requests.Session,
     clone_token: str,
     submission_number: str,
     project_name: str,
     directory: str,
     model_directory: str,
@@ -43,28 +74,22 @@
     with open(project_file_path, "w") as fd:
         fd.write(project_name)
 
     token_file_path = os.path.join(dot_crunchdao_path, constants.TOKEN_FILE)
     with open(token_file_path, "w") as fd:
         fd.write(push_token['plain'])
 
-    code_tar = io.BytesIO(
-        session.get(f"/v1/projects/{project_name}/clone", params={
-            "pushToken": push_token['plain'],
-            "submissionNumber": submission_number,
-            "includeModel": not no_model,
-        }).content
-    )
-
-    tar = tarfile.open(fileobj=code_tar)
-    for member in tar.getmembers():
-        path = os.path.join(directory, member.name)
-        print(f"extract {path}")
-
-        os.makedirs(os.path.dirname(path), exist_ok=True)
-
-        fileobj = tar.extractfile(member)
-        with open(path, "wb") as fd:
-            fd.write(fileobj.read())
+    try:
+        code_tar = io.BytesIO(
+            session.get(f"/v1/projects/{project_name}/clone", params={
+                "pushToken": push_token['plain'],
+                "submissionNumber": submission_number,
+                "includeModel": not no_model,
+            }).content
+        )
+    except api.NeverSubmittedException:
+        _setup_demo(directory)
+    else:
+        _setup_submission(directory, code_tar)
 
     path = os.path.join(directory, model_directory)
     os.makedirs(path, exist_ok=True)
```

### Comparing `crunch-cli-1.0.0/crunch/command/test.py` & `crunch-cli-1.1.0/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/constants.py` & `crunch-cli-1.1.0/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/ensure.py` & `crunch-cli-1.1.0/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/inline.py` & `crunch-cli-1.1.0/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/main.py` & `crunch-cli-1.1.0/crunch/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,10 +156,9 @@
 ):
     command.convert(
         notebook_file_path=notebook_file_path,
         python_file_path=python_file_path,
         override=override,
     )
 
-
 if __name__ == '__main__':
     cli()
```

### Comparing `crunch-cli-1.0.0/crunch/tester.py` & `crunch-cli-1.1.0/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.0.0/crunch/utils.py` & `crunch-cli-1.1.0/crunch/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import urllib.parse
 
 import click
 import joblib
 import pandas
 import requests
 
-from . import constants
+from . import constants, api
 
 
 class CustomSession(requests.Session):
     # https://stackoverflow.com/a/51026159/7292958
 
     def __init__(self, web_base_url=None, api_base_url=None, debug=False, notebook=False):
         super().__init__()
@@ -31,26 +31,31 @@
             **kwargs
         )
 
         status_code = response.status_code
         if status_code != 200:
             try:
                 error = response.json()
+            except:
+                print(response.text)
+            else:
+                code = error.get("code", "")
+                message = error.get("message", "")
 
-                if error.get("code") == "INVALID_PROJECT_TOKEN" and error.get("message") == "invalid project token":
+                if code == "INVALID_PROJECT_TOKEN" and message == "invalid project token":
                     print("your token seems to have expired or is invalid")
                     self.print_recopy_command()
-                elif error.get("code") == "ENTITY_NOT_FOUND" and error.get("message", "").startswith("no user found with username"):
+                elif code == "ENTITY_NOT_FOUND" and message.startswith("no user found with username"):
                     print("user not found, did you rename yourself?")
                     self.print_recopy_command()
+                elif code == "NEVER_SUBMITTED":
+                    raise api.NeverSubmittedException(message)
                 else:
                     print(f"{method} {url}: {status_code}")
                     print(json.dumps(error, indent=4))
-            except:
-                print(response.text)
 
             if self.debug:
                 traceback.print_stack()
 
             raise click.Abort()
 
         return response
```

### Comparing `crunch-cli-1.0.0/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.1.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 README.md
 setup.py
 crunch/__init__.py
 crunch/__version__.py
+crunch/api.py
 crunch/constants.py
 crunch/ensure.py
 crunch/inline.py
 crunch/main.py
 crunch/tester.py
 crunch/utils.py
 crunch/command/__init__.py
 crunch/command/convert.py
 crunch/command/download.py
 crunch/command/push.py
 crunch/command/setup.py
 crunch/command/test.py
+crunch/demo-project/.gitignore
+crunch/demo-project/files.json
+crunch/demo-project/main.py
+crunch/demo-project/requirements.txt
 crunch_cli.egg-info/PKG-INFO
 crunch_cli.egg-info/SOURCES.txt
 crunch_cli.egg-info/dependency_links.txt
 crunch_cli.egg-info/entry_points.txt
 crunch_cli.egg-info/not-zip-safe
 crunch_cli.egg-info/requires.txt
 crunch_cli.egg-info/top_level.txt
```

### Comparing `crunch-cli-1.0.0/setup.py` & `crunch-cli-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 
 import os
 from setuptools import setup, find_packages
 
+package = "crunch"
+
 about = {}
 here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, 'crunch', '__version__.py')) as f:
+with open(os.path.join(here, package, '__version__.py')) as f:
     exec(f.read(), about)
 
 with open('requirements.txt') as fd:
     requirements = fd.read().splitlines()
 
 with open('README.md') as fd:
     readme = fd.read()
@@ -20,14 +22,20 @@
     long_description=readme,
     long_description_content_type='text/markdown',
     version=about['__version__'],
     author=about['__author__'],
     author_email=about['__author_email__'],
     url=about['__url__'],
     packages=find_packages(),
+    package_data={
+        package: [
+            "demo-project/*",
+            "demo-project/.*",
+        ]
+    },
     include_package_data=True,
     python_requires=">=3",
     install_requires=requirements,
     zip_safe=False,
     entry_points={
         'console_scripts': ['crunch=crunch.main:cli'],
     },
```

