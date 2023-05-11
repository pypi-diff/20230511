# Comparing `tmp/shutterstock-cli-1.1.8.tar.gz` & `tmp/shutterstock-cli-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shutterstock-cli-1.1.8.tar", last modified: Mon Oct 11 14:54:22 2021, max compression
+gzip compressed data, was "shutterstock-cli-1.1.9.tar", last modified: Thu Oct 28 17:42:18 2021, max compression
```

## Comparing `shutterstock-cli-1.1.8.tar` & `shutterstock-cli-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 14:54:22.924804 shutterstock-cli-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     8908 2021-10-11 14:54:22.923804 shutterstock-cli-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6409 2021-10-11 14:52:54.000000 shutterstock-cli-1.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-11 14:54:22.924804 shutterstock-cli-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2475 2021-10-11 14:52:54.000000 shutterstock-cli-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 14:54:22.922804 shutterstock-cli-1.1.8/shutterstock/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-11 14:52:54.000000 shutterstock-cli-1.1.8/shutterstock/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2021-10-11 14:54:21.000000 shutterstock-cli-1.1.8/shutterstock/__version__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/ai_audio.py
--rw-r--r--   0 root         (0) root         (0)    11098 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/audio.py
--rw-r--r--   0 root         (0) root         (0)      796 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/cli.py
--rw-r--r--   0 root         (0) root         (0)     2333 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/contributors.py
--rw-r--r--   0 root         (0) root         (0)     2909 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/cv.py
--rw-r--r--   0 root         (0) root         (0)     1873 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/editor.py
--rw-r--r--   0 root         (0) root         (0)    12137 2021-10-11 14:54:11.000000 shutterstock-cli-1.1.8/shutterstock/editorial.py
--rw-r--r--   0 root         (0) root         (0)    19892 2021-10-11 14:54:11.000000 shutterstock-cli-1.1.8/shutterstock/images.py
--rw-r--r--   0 root         (0) root         (0)      685 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/test.py
--rw-r--r--   0 root         (0) root         (0)      745 2021-10-11 14:54:10.000000 shutterstock-cli-1.1.8/shutterstock/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 14:54:22.923804 shutterstock-cli-1.1.8/shutterstock/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2021-10-11 14:52:54.000000 shutterstock-cli-1.1.8/shutterstock/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      476 2021-10-11 14:52:54.000000 shutterstock-cli-1.1.8/shutterstock/utils/prettyprint.py
--rw-r--r--   0 root         (0) root         (0)     2636 2021-10-11 14:52:54.000000 shutterstock-cli-1.1.8/shutterstock/utils/request.py
--rw-r--r--   0 root         (0) root         (0)     1314 2021-10-11 14:52:54.000000 shutterstock-cli-1.1.8/shutterstock/utils/request_helper.py
--rw-r--r--   0 root         (0) root         (0)    16452 2021-10-11 14:54:11.000000 shutterstock-cli-1.1.8/shutterstock/videos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 14:54:22.923804 shutterstock-cli-1.1.8/shutterstock_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8908 2021-10-11 14:54:22.000000 shutterstock-cli-1.1.8/shutterstock_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2021-10-11 14:54:22.000000 shutterstock-cli-1.1.8/shutterstock_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-11 14:54:22.000000 shutterstock-cli-1.1.8/shutterstock_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2021-10-11 14:54:22.000000 shutterstock-cli-1.1.8/shutterstock_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2021-10-11 14:54:22.000000 shutterstock-cli-1.1.8/shutterstock_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-10-11 14:54:22.000000 shutterstock-cli-1.1.8/shutterstock_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 17:42:18.179625 shutterstock-cli-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     8637 2021-10-28 17:42:18.179625 shutterstock-cli-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6202 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-10-28 17:42:18.179625 shutterstock-cli-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2475 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 17:42:18.179625 shutterstock-cli-1.1.9/shutterstock/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2021-10-28 17:42:16.000000 shutterstock-cli-1.1.9/shutterstock/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/ai_audio.py
+-rw-r--r--   0 root         (0) root         (0)    11098 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/audio.py
+-rw-r--r--   0 root         (0) root         (0)      796 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/cli.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/contributors.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/cv.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/editor.py
+-rw-r--r--   0 root         (0) root         (0)    12137 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/editorial.py
+-rw-r--r--   0 root         (0) root         (0)    19892 2021-10-28 17:42:07.000000 shutterstock-cli-1.1.9/shutterstock/images.py
+-rw-r--r--   0 root         (0) root         (0)      685 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/test.py
+-rw-r--r--   0 root         (0) root         (0)      745 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 17:42:18.179625 shutterstock-cli-1.1.9/shutterstock/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      476 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/utils/prettyprint.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/utils/request.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/utils/request_helper.py
+-rw-r--r--   0 root         (0) root         (0)    16452 2021-10-28 17:42:06.000000 shutterstock-cli-1.1.9/shutterstock/videos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-28 17:42:18.179625 shutterstock-cli-1.1.9/shutterstock_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8637 2021-10-28 17:42:18.000000 shutterstock-cli-1.1.9/shutterstock_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2021-10-28 17:42:18.000000 shutterstock-cli-1.1.9/shutterstock_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-28 17:42:18.000000 shutterstock-cli-1.1.9/shutterstock_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2021-10-28 17:42:18.000000 shutterstock-cli-1.1.9/shutterstock_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2021-10-28 17:42:18.000000 shutterstock-cli-1.1.9/shutterstock_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-10-28 17:42:18.000000 shutterstock-cli-1.1.9/shutterstock_cli.egg-info/top_level.txt
```

### Comparing `shutterstock-cli-1.1.8/PKG-INFO` & `shutterstock-cli-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 Metadata-Version: 2.1
 Name: shutterstock-cli
-Version: 1.1.8
+Version: 1.1.9
 Summary: A command-line utility that allows you to interact with the Shutterstock public API.
 Home-page: https://github.com/shutterstock/shutterstock-cli
 Author: Shutterstock
 Author-email: tech.api.team@shutterstock.com
 License: UNKNOWN
 Description: # shutterstock-cli
         
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         A command-line utility that allows you to interact with the Shutterstock public API. For more information about the CLI and the API, see the [Shutterstock API reference](https://api-reference.shutterstock.com/).
         
-        ## Installation
-        
-        The Shutterstock CLI is available on the [Python Package Index (PyPI)](https://pypi.org/project/shutterstock-cli/). You can install it using pip.
-        
-        ``` bash
-        pip install shutterstock-cli
-        ```
-        
         ## Authentication
         
         ### Basic authentication
         
         All endpoints in the Shutterstock API require authentication.
         The API accepts HTTP basic authentication for some endpoints and OAuth authentication for all endpoints.
```

### Comparing `shutterstock-cli-1.1.8/README.md` & `shutterstock-cli-1.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 # shutterstock-cli
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A command-line utility that allows you to interact with the Shutterstock public API. For more information about the CLI and the API, see the [Shutterstock API reference](https://api-reference.shutterstock.com/).
 
-## Installation
-
-The Shutterstock CLI is available on the [Python Package Index (PyPI)](https://pypi.org/project/shutterstock-cli/). You can install it using pip.
-
-``` bash
-pip install shutterstock-cli
-```
-
 ## Authentication
 
 ### Basic authentication
 
 All endpoints in the Shutterstock API require authentication.
 The API accepts HTTP basic authentication for some endpoints and OAuth authentication for all endpoints.
```

### Comparing `shutterstock-cli-1.1.8/setup.py` & `shutterstock-cli-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/ai_audio.py` & `shutterstock-cli-1.1.9/shutterstock/ai_audio.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/audio.py` & `shutterstock-cli-1.1.9/shutterstock/audio.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/cli.py` & `shutterstock-cli-1.1.9/shutterstock/cli.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/contributors.py` & `shutterstock-cli-1.1.9/shutterstock/contributors.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/cv.py` & `shutterstock-cli-1.1.9/shutterstock/cv.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/editor.py` & `shutterstock-cli-1.1.9/shutterstock/editor.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/editorial.py` & `shutterstock-cli-1.1.9/shutterstock/editorial.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/images.py` & `shutterstock-cli-1.1.9/shutterstock/images.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/test.py` & `shutterstock-cli-1.1.9/shutterstock/test.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/user.py` & `shutterstock-cli-1.1.9/shutterstock/user.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/utils/request.py` & `shutterstock-cli-1.1.9/shutterstock/utils/request.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/utils/request_helper.py` & `shutterstock-cli-1.1.9/shutterstock/utils/request_helper.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock/videos.py` & `shutterstock-cli-1.1.9/shutterstock/videos.py`

 * *Files identical despite different names*

### Comparing `shutterstock-cli-1.1.8/shutterstock_cli.egg-info/PKG-INFO` & `shutterstock-cli-1.1.9/shutterstock_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 Metadata-Version: 2.1
 Name: shutterstock-cli
-Version: 1.1.8
+Version: 1.1.9
 Summary: A command-line utility that allows you to interact with the Shutterstock public API.
 Home-page: https://github.com/shutterstock/shutterstock-cli
 Author: Shutterstock
 Author-email: tech.api.team@shutterstock.com
 License: UNKNOWN
 Description: # shutterstock-cli
         
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         A command-line utility that allows you to interact with the Shutterstock public API. For more information about the CLI and the API, see the [Shutterstock API reference](https://api-reference.shutterstock.com/).
         
-        ## Installation
-        
-        The Shutterstock CLI is available on the [Python Package Index (PyPI)](https://pypi.org/project/shutterstock-cli/). You can install it using pip.
-        
-        ``` bash
-        pip install shutterstock-cli
-        ```
-        
         ## Authentication
         
         ### Basic authentication
         
         All endpoints in the Shutterstock API require authentication.
         The API accepts HTTP basic authentication for some endpoints and OAuth authentication for all endpoints.
```

### Comparing `shutterstock-cli-1.1.8/shutterstock_cli.egg-info/SOURCES.txt` & `shutterstock-cli-1.1.9/shutterstock_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

