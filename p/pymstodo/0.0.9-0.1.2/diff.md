# Comparing `tmp/pymstodo-0.0.9.tar.gz` & `tmp/pymstodo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymstodo-0.0.9.tar", last modified: Mon May  3 10:14:51 2021, max compression
+gzip compressed data, was "pymstodo-0.1.2.tar", last modified: Thu May 11 06:10:25 2023, max compression
```

## Comparing `pymstodo-0.0.9.tar` & `pymstodo-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-03 10:14:51.000000 pymstodo-0.0.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2021-05-03 10:14:34.000000 pymstodo-0.0.9/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2021-05-03 10:14:51.000000 pymstodo-0.0.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1382 2021-05-03 10:14:34.000000 pymstodo-0.0.9/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo/
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-05-03 10:14:34.000000 pymstodo-0.0.9/pymstodo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11016 2021-05-03 10:14:34.000000 pymstodo-0.0.9/pymstodo/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      225 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-05-03 10:14:51.000000 pymstodo-0.0.9/pymstodo.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-05-03 10:14:51.000000 pymstodo-0.0.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1297 2021-05-03 10:14:34.000000 pymstodo-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:10:25.453453 pymstodo-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 06:10:07.000000 pymstodo-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 06:10:25.453453 pymstodo-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-11 06:10:07.000000 pymstodo-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:10:25.449453 pymstodo-0.1.2/pymstodo/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 06:10:07.000000 pymstodo-0.1.2/pymstodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-11 06:10:07.000000 pymstodo-0.1.2/pymstodo/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:10:25.453453 pymstodo-0.1.2/pymstodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 06:10:25.000000 pymstodo-0.1.2/pymstodo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 06:10:25.453453 pymstodo-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-11 06:10:07.000000 pymstodo-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pymstodo-0.0.9/LICENSE` & `pymstodo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymstodo-0.0.9/PKG-INFO` & `pymstodo-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.0.9
+Version: 0.1.2
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
-Description: # pymstodo ✔️
-        [![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.org/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.org/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        
-        ### Python wrapper to deal with [Microsoft To Do](https://to-do.live.com).
-        
-        ## Installation
-        ```
-        pip3 install pymstodo
-        ```
-        
-        ## Requirements
-        * python >= 3.7
-        * requests_oauthlib >= 1.3.0
-        
-        ## Usage
-        1. [Get an API key](https://github.com/inbalboa/pymstodo/blob/master/GET_KEY.md) before using `pymstodo`.
-        2. Use it to initialize client. Here is an example:
-        ```python
-        from pymstodo import ToDoConnection
-        
-        client_id = 'PLACE YOUR CLIENT ID'
-        client_secret = 'PLACE YOUR CLIENT SECRET'
-        
-        auth_url = ToDoConnection.get_auth_url(client_id)
-        redirect_resp = input(f'Go here and authorize:\n{auth_url}\n\nPaste the full redirect URL below:\n')
-        token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)
-        todo_client = ToDoConnection(client_id=client_id, client_secret=client_secret, token=token)
-        
-        lists = todo_client.get_lists()
-        task_list = lists[0]
-        tasks = todo_client.get_tasks(task_list.list_id)
-        
-        print(task_list)
-        print(*tasks, sep='\n')
-        ```
-        3. Full API description see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pymstodo ✔️
+[![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.com/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.com/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+### Python wrapper to deal with [Microsoft To Do](https://to-do.live.com).
+
+## Installation
+```
+pip3 install pymstodo
+```
+
+## Requirements
+* python >= 3.8
+* requests_oauthlib >= 1.3.0
+
+## Usage
+1. [Get an API key](https://github.com/inbalboa/pymstodo/blob/master/GET_KEY.md) before using `pymstodo`.
+2. Use it to initialize client. Here is an example:
+```python
+from pymstodo import ToDoConnection
+
+client_id = 'PLACE YOUR CLIENT ID'
+client_secret = 'PLACE YOUR CLIENT SECRET'
+
+auth_url = ToDoConnection.get_auth_url(client_id)
+redirect_resp = input(f'Go here and authorize:\n{auth_url}\n\nPaste the full redirect URL below:\n')
+token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)
+todo_client = ToDoConnection(client_id=client_id, client_secret=client_secret, token=token)
+
+lists = todo_client.get_lists()
+task_list = lists[0]
+tasks = todo_client.get_tasks(task_list.list_id)
+
+print(task_list)
+print(*tasks, sep='\n')
+```
+3. Full description of library objects and methods: https://raw.githubusercontent.com/inbalboa/pymstodo/master/docs/index.html
+API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
```

### Comparing `pymstodo-0.0.9/README.md` & `pymstodo-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # pymstodo ✔️
-[![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.org/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.org/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.com/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.com/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 ### Python wrapper to deal with [Microsoft To Do](https://to-do.live.com).
 
 ## Installation
 ```
 pip3 install pymstodo
 ```
 
 ## Requirements
-* python >= 3.7
+* python >= 3.8
 * requests_oauthlib >= 1.3.0
 
 ## Usage
 1. [Get an API key](https://github.com/inbalboa/pymstodo/blob/master/GET_KEY.md) before using `pymstodo`.
 2. Use it to initialize client. Here is an example:
 ```python
 from pymstodo import ToDoConnection
@@ -29,9 +29,9 @@
 lists = todo_client.get_lists()
 task_list = lists[0]
 tasks = todo_client.get_tasks(task_list.list_id)
 
 print(task_list)
 print(*tasks, sep='\n')
 ```
-3. Full API description see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
-
+3. Full description of library objects and methods: https://raw.githubusercontent.com/inbalboa/pymstodo/master/docs/index.html
+API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
```

### Comparing `pymstodo-0.0.9/pymstodo.egg-info/PKG-INFO` & `pymstodo-0.1.2/pymstodo.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.0.9
+Version: 0.1.2
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
-Description: # pymstodo ✔️
-        [![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.org/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.org/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        
-        ### Python wrapper to deal with [Microsoft To Do](https://to-do.live.com).
-        
-        ## Installation
-        ```
-        pip3 install pymstodo
-        ```
-        
-        ## Requirements
-        * python >= 3.7
-        * requests_oauthlib >= 1.3.0
-        
-        ## Usage
-        1. [Get an API key](https://github.com/inbalboa/pymstodo/blob/master/GET_KEY.md) before using `pymstodo`.
-        2. Use it to initialize client. Here is an example:
-        ```python
-        from pymstodo import ToDoConnection
-        
-        client_id = 'PLACE YOUR CLIENT ID'
-        client_secret = 'PLACE YOUR CLIENT SECRET'
-        
-        auth_url = ToDoConnection.get_auth_url(client_id)
-        redirect_resp = input(f'Go here and authorize:\n{auth_url}\n\nPaste the full redirect URL below:\n')
-        token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)
-        todo_client = ToDoConnection(client_id=client_id, client_secret=client_secret, token=token)
-        
-        lists = todo_client.get_lists()
-        task_list = lists[0]
-        tasks = todo_client.get_tasks(task_list.list_id)
-        
-        print(task_list)
-        print(*tasks, sep='\n')
-        ```
-        3. Full API description see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pymstodo ✔️
+[![PyPI](https://img.shields.io/pypi/v/pymstodo.svg)](https://pypi.org/project/pymstodo/) [![Build Status](https://travis-ci.com/inbalboa/pymstodo.svg?branch=master)](https://travis-ci.com/inbalboa/pymstodo) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+### Python wrapper to deal with [Microsoft To Do](https://to-do.live.com).
+
+## Installation
+```
+pip3 install pymstodo
+```
+
+## Requirements
+* python >= 3.8
+* requests_oauthlib >= 1.3.0
+
+## Usage
+1. [Get an API key](https://github.com/inbalboa/pymstodo/blob/master/GET_KEY.md) before using `pymstodo`.
+2. Use it to initialize client. Here is an example:
+```python
+from pymstodo import ToDoConnection
+
+client_id = 'PLACE YOUR CLIENT ID'
+client_secret = 'PLACE YOUR CLIENT SECRET'
+
+auth_url = ToDoConnection.get_auth_url(client_id)
+redirect_resp = input(f'Go here and authorize:\n{auth_url}\n\nPaste the full redirect URL below:\n')
+token = ToDoConnection.get_token(client_id, client_secret, redirect_resp)
+todo_client = ToDoConnection(client_id=client_id, client_secret=client_secret, token=token)
+
+lists = todo_client.get_lists()
+task_list = lists[0]
+tasks = todo_client.get_tasks(task_list.list_id)
+
+print(task_list)
+print(*tasks, sep='\n')
+```
+3. Full description of library objects and methods: https://raw.githubusercontent.com/inbalboa/pymstodo/master/docs/index.html
+API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
```

### Comparing `pymstodo-0.0.9/setup.py` & `pymstodo-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,20 +26,19 @@
     author_email='shlyapugin@gmail.com',
     description='Microsoft To Do API client',
     long_description=long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/inbalboa/pymstodo',
     packages=setuptools.find_packages(),
     install_requires=find_requires(),
-    python_requires='>=3.7,<4.0',
+    python_requires='>=3.8,<4.0',
     classifiers=[
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
     license='GPLv3'
 )
-
```

