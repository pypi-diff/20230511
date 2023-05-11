# Comparing `tmp/xguard-1.0.0.tar.gz` & `tmp/xguard-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xguard-1.0.0.tar", last modified: Fri Mar 31 19:05:34 2023, max compression
+gzip compressed data, was "xguard-1.0.4.tar", last modified: Thu May 11 13:25:16 2023, max compression
```

## Comparing `xguard-1.0.0.tar` & `xguard-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 gitahi    (1000) gitahi    (1000)        0 2023-03-31 19:05:34.748094 xguard-1.0.0/
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)     1069 2023-03-31 18:06:12.000000 xguard-1.0.0/LICENSE
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)     3185 2023-03-31 19:05:34.748094 xguard-1.0.0/PKG-INFO
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)     2695 2023-03-31 18:38:26.000000 xguard-1.0.0/README.md
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)       38 2023-03-31 19:05:34.748094 xguard-1.0.0/setup.cfg
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)      703 2023-03-31 19:05:14.000000 xguard-1.0.0/setup.py
-drwxrwxr-x   0 gitahi    (1000) gitahi    (1000)        0 2023-03-31 19:05:34.748094 xguard-1.0.0/xguard.egg-info/
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)     3185 2023-03-31 19:05:34.000000 xguard-1.0.0/xguard.egg-info/PKG-INFO
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)      146 2023-03-31 19:05:34.000000 xguard-1.0.0/xguard.egg-info/SOURCES.txt
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)        1 2023-03-31 19:05:34.000000 xguard-1.0.0/xguard.egg-info/dependency_links.txt
--rw-rw-r--   0 gitahi    (1000) gitahi    (1000)        1 2023-03-31 19:05:34.000000 xguard-1.0.0/xguard.egg-info/top_level.txt
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:25:16.944650 xguard-1.0.4/
+-rw-r--r--   0 gus       (1000) gus       (1000)     3560 2023-05-11 13:25:16.944650 xguard-1.0.4/PKG-INFO
+-rw-r--r--   0 gus       (1000) gus       (1000)     3120 2023-05-11 13:25:07.000000 xguard-1.0.4/README.txt
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:25:16.941316 xguard-1.0.4/core/
+-rw-r--r--   0 gus       (1000) gus       (1000)     1005 2023-05-11 12:22:04.000000 xguard-1.0.4/core/__init__.py
+-rw-r--r--   0 gus       (1000) gus       (1000)       38 2023-05-11 13:25:16.944650 xguard-1.0.4/setup.cfg
+-rw-r--r--   0 gus       (1000) gus       (1000)      696 2023-05-11 13:14:02.000000 xguard-1.0.4/setup.py
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:25:16.941316 xguard-1.0.4/tests/
+-rw-r--r--   0 gus       (1000) gus       (1000)       90 2023-05-11 12:57:45.000000 xguard-1.0.4/tests/test_is_gt.py
+drwxr-xr-x   0 gus       (1000) gus       (1000)        0 2023-05-11 13:25:16.941316 xguard-1.0.4/xguard.egg-info/
+-rw-r--r--   0 gus       (1000) gus       (1000)     3560 2023-05-11 13:25:16.000000 xguard-1.0.4/xguard.egg-info/PKG-INFO
+-rw-r--r--   0 gus       (1000) gus       (1000)      176 2023-05-11 13:25:16.000000 xguard-1.0.4/xguard.egg-info/SOURCES.txt
+-rw-r--r--   0 gus       (1000) gus       (1000)        1 2023-05-11 13:25:16.000000 xguard-1.0.4/xguard.egg-info/dependency_links.txt
+-rw-r--r--   0 gus       (1000) gus       (1000)        5 2023-05-11 13:25:16.000000 xguard-1.0.4/xguard.egg-info/top_level.txt
```

### Comparing `xguard-1.0.0/PKG-INFO` & `xguard-1.0.4/README.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-Metadata-Version: 2.1
-Name: xguard
-Version: 1.0.0
-Summary: xguard, yet another guard clauses libary
-Home-page: https://github.com/johngitahi/xguard
-Author: John Gitahi
-Author-email: gitahi109@gmail.com
-License: MIT
-Keywords: guard clause
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# xguard
 
-# Pyguards
-Xguard is just another guard clause library.
+[![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
+![License: GPLv3](https://img.shields.io/github/license/johngitahi/xguard?style=flat)
+
+Xguard is yet another guard clause library.
 
 ## What are Guard Clauses
-A guard clause is simply a check that immediately exits the function, either with a return statement or an exception. If you're used to writing functions that check to ensure everything is valid for the function to run, then you write the main function code, and then you write else statements to deal with error cases, this involves inverting your current workflow. The benefit is that your code will tend to be shorter and simpler, and less deeply indented. (Credit)['deviq.com/design-patterns/guard-clause']
+A guard clause is simply a check that immediately exits the function, either with a return statement or an exception. If you're used to writing functions that check to ensure everything is valid for the function to run, then you write the main function code, and then you write else statements to deal with error cases, this involves inverting your current workflow. The benefit is that your code will tend to be shorter and simpler, and less deeply indented. [Credit](https://deviq.com/design-patterns/guard-clause)
 
 ## How to use this library
-Using this library is easy. Just import the library, create an instance of the Pyguard class, and start chaining your guard clauses together.
+Using this library is easy. Just import the library, create an instance of the Xguard class, and start chaining your guard clauses together.
+
+In dev mode, if you still encounter a lot of import errors, and you think you know what you are doing, try to add the xguard dir to the python path.
+```
+export PYTHONPATH=/path/to/parent/directory:$PYTHONPATH
+```
 
 Here's an example:
 ```python
 import xguard
 
 def add_ten(number: int):
     guard = xguard.Xguard()
@@ -41,24 +33,22 @@
 print(res)
 
 # Good Issue: Try to use the guard clauses in a factorial function
 ```
 See? Easy!
 
 ## Why I wrote the library
-I wrote Guard Clauses because I wanted to create something useful for other developers like myself. As someone who has written a lot of code, I know how frustrating it can be to spend time tracking down errors caused by bad inputs. I wanted to make it easier for developers to catch these issues early on and write more robust code.
+I wrote xguard because I wanted to create something useful for other developers like myself. As someone who has written a lot of code, I know how frustrating it can be to spend time tracking down errors caused by bad inputs. I wanted to make it easier for developers to catch these issues early on and write more robust code.
 
-It was also an opporuinty for me to improve on a similar project by Adrian without wrecking his original idea. I added some extra features like custom error messages to make it more powerful and flexible. With custom error messages, developers can quickly understand what went wrong when a guard clause fails.
+It was also an opporuinty for me to improve on a similar project by Adrian without wrecking his original idea. I am adding some extra features like custom error messages to make it more powerful and flexible. With custom error messages, developers can quickly understand what went wrong when a guard clause fails.
 
-Overall, my main motivation for creating Guard Clauses was to write something that I found useful and that I hope other developers will find useful as well. I believe in the power of open source software and I would love for others to contribute to the project. If you have any feedback or suggestions, please feel free to share them or even open a pull request on GitHub. Together, we can make pyguards even better.
+Overall, my main motivation for creating xguard was to write something that I found useful and that I hope other developers will find useful as well. I believe in the power of open source software and I would love for others to contribute to the project. If you have any feedback or suggestions, please feel free to share them or even open a pull request on GitHub. Together, we can make xguard even better.
 
 ## Documentation
 Each guard method is documented with a docstring that explains its purpose and usage, following the reST style. You can access the documentation for each method using Python's built-in `help` function
 
 ## License
-This library is released under the MIT License. See the LICENSE file for details.
+This library is released under the GNU GPLv3 License. See the LICENSE file for details.
 
 ## Acknowledgements
-This library is based on the ideas and code of Adrian's similar project. Thank you, Adrian!
-
-
+This library is based on the ideas and code of Adrian's [similar project](https://github.com/veldfolds/NGuard). Thank you, Adrian!
```

### Comparing `xguard-1.0.0/setup.py` & `xguard-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as fh:
+with open("README.txt", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="xguard",
-    version="1.0.0",
+    version="1.0.4",
     author="John Gitahi",
     author_email="gitahi109@gmail.com",
-    description="xguard, yet another guard clauses libary",
+    description="yet another guard clauses libary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     url="https://github.com/johngitahi/xguard",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `xguard-1.0.0/xguard.egg-info/PKG-INFO` & `xguard-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 2.1
 Name: xguard
-Version: 1.0.0
-Summary: xguard, yet another guard clauses libary
+Version: 1.0.4
+Summary: yet another guard clauses libary
 Home-page: https://github.com/johngitahi/xguard
 Author: John Gitahi
 Author-email: gitahi109@gmail.com
 License: MIT
 Keywords: guard clause
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
-# Pyguards
-Xguard is just another guard clause library.
+# xguard
+
+[![PyPI version](https://badge.fury.io/py/xguard.svg)](https://badge.fury.io/py/xguard)
+![License: GPLv3](https://img.shields.io/github/license/johngitahi/xguard?style=flat)
+
+Xguard is yet another guard clause library.
 
 ## What are Guard Clauses
-A guard clause is simply a check that immediately exits the function, either with a return statement or an exception. If you're used to writing functions that check to ensure everything is valid for the function to run, then you write the main function code, and then you write else statements to deal with error cases, this involves inverting your current workflow. The benefit is that your code will tend to be shorter and simpler, and less deeply indented. (Credit)['deviq.com/design-patterns/guard-clause']
+A guard clause is simply a check that immediately exits the function, either with a return statement or an exception. If you're used to writing functions that check to ensure everything is valid for the function to run, then you write the main function code, and then you write else statements to deal with error cases, this involves inverting your current workflow. The benefit is that your code will tend to be shorter and simpler, and less deeply indented. [Credit](https://deviq.com/design-patterns/guard-clause)
 
 ## How to use this library
-Using this library is easy. Just import the library, create an instance of the Pyguard class, and start chaining your guard clauses together.
+Using this library is easy. Just import the library, create an instance of the Xguard class, and start chaining your guard clauses together.
+
+In dev mode, if you still encounter a lot of import errors, and you think you know what you are doing, try to add the xguard dir to the python path.
+```
+export PYTHONPATH=/path/to/parent/directory:$PYTHONPATH
+```
 
 Here's an example:
 ```python
 import xguard
 
 def add_ten(number: int):
     guard = xguard.Xguard()
@@ -41,24 +48,22 @@
 print(res)
 
 # Good Issue: Try to use the guard clauses in a factorial function
 ```
 See? Easy!
 
 ## Why I wrote the library
-I wrote Guard Clauses because I wanted to create something useful for other developers like myself. As someone who has written a lot of code, I know how frustrating it can be to spend time tracking down errors caused by bad inputs. I wanted to make it easier for developers to catch these issues early on and write more robust code.
+I wrote xguard because I wanted to create something useful for other developers like myself. As someone who has written a lot of code, I know how frustrating it can be to spend time tracking down errors caused by bad inputs. I wanted to make it easier for developers to catch these issues early on and write more robust code.
 
-It was also an opporuinty for me to improve on a similar project by Adrian without wrecking his original idea. I added some extra features like custom error messages to make it more powerful and flexible. With custom error messages, developers can quickly understand what went wrong when a guard clause fails.
+It was also an opporuinty for me to improve on a similar project by Adrian without wrecking his original idea. I am adding some extra features like custom error messages to make it more powerful and flexible. With custom error messages, developers can quickly understand what went wrong when a guard clause fails.
 
-Overall, my main motivation for creating Guard Clauses was to write something that I found useful and that I hope other developers will find useful as well. I believe in the power of open source software and I would love for others to contribute to the project. If you have any feedback or suggestions, please feel free to share them or even open a pull request on GitHub. Together, we can make pyguards even better.
+Overall, my main motivation for creating xguard was to write something that I found useful and that I hope other developers will find useful as well. I believe in the power of open source software and I would love for others to contribute to the project. If you have any feedback or suggestions, please feel free to share them or even open a pull request on GitHub. Together, we can make xguard even better.
 
 ## Documentation
 Each guard method is documented with a docstring that explains its purpose and usage, following the reST style. You can access the documentation for each method using Python's built-in `help` function
 
 ## License
-This library is released under the MIT License. See the LICENSE file for details.
+This library is released under the GNU GPLv3 License. See the LICENSE file for details.
 
 ## Acknowledgements
-This library is based on the ideas and code of Adrian's similar project. Thank you, Adrian!
-
-
+This library is based on the ideas and code of Adrian's [similar project](https://github.com/veldfolds/NGuard). Thank you, Adrian!
```

