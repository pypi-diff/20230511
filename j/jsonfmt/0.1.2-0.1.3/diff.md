# Comparing `tmp/jsonfmt-0.1.2.tar.gz` & `tmp/jsonfmt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.1.2.tar", last modified: Wed May 10 03:03:14 2023, max compression
+gzip compressed data, was "jsonfmt-0.1.3.tar", last modified: Thu May 11 16:15:58 2023, max compression
```

## Comparing `jsonfmt-0.1.2.tar` & `jsonfmt-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4472 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 16:15:58.000000 jsonfmt-0.1.3/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4964 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 16:15:42.000000 jsonfmt-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:15:58.444173 jsonfmt-0.1.3/setup.cfg
```

### Comparing `jsonfmt-0.1.2/LICENSE` & `jsonfmt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.1.2/PKG-INFO` & `jsonfmt-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.1.2
-Summary: A JSON object formatting tool.
-Home-page: https://github.com/seamile/jsonfmt
-Author: Seamile
-Author-email: lanhuermao@gmail.com
+Version: 0.1.3
+Summary: A simple tool for formatting JSON object.
+Author-email: Seamile <lanhuermao@gmail.com>
+License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formator
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/jsonfmt?label=Install&color=green)
 ![PyPI](https://img.shields.io/pypi/v/jsonfmt?color=9cf)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?branch=main&label=build&logo=python)
 
 
-**jsonfmt** is a json object formatting tool.
+**jsonfmt** is a JSON object formatting tool.
 
-## Features
+It has the following features:
 
-1. Print the json object in pretty format from files or stdin.
-2. Compress the json object into a single line without spaces.
-3. Output part of a large json object via jsonpath.
+1. Print the JSON object with **hightlight** and **pretty format** from files or stdin.
+2. Compress the JSON object into a single line without spaces.
+3. Output part of a large JSON object via jsonpath.
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
 
@@ -45,127 +44,148 @@
 - positional arguments:
 
      - `json_files`   the json files that will be processed
 
 - options:
 
      - `-h, --help`: show this help message and exit.
-     - `-c`: compression the json object in the files or stdin.
+     - `-c`: compression the JSON object in the files or stdin.
+     - `-e`: escape non-ASCII characters.
+     - `-i INDENT`: number of spaces to use for indentation. (default: 4)
      - `-O`: overwrite to the json file.
-     - `-p JSONPATH`: output part of json object via jsonpath.
+     - `-p JSONPATH`: output part of JSON object via jsonpath.
      - `-v`: show the version.
 
 
 ## Example
 
-In the file example.json there is a compressed json object.
+In the file example.json there is a compressed JSON object.
 
 1. Pretty print from json file.
 
      ```shell
      $ jsonfmt example.json
      ```
 
-     ouput:
+     Output:
      ```json
      {
           "age": 23,
-          "gender": "male",
+          "gender": "纯爷们",
           "history": [
                {
                     "action": "eat",
                     "date": "2021-03-02",
                     "items": [
                          {
-                              "bar": 222,
-                              "foo": 111
+                              "calorie": 294.9,
+                              "name": "hamburger"
                          },
                          {
-                              "bar": -222,
-                              "foo": -111
+                              "calorie": 266,
+                              "name": "pizza"
                          }
                     ]
                },
                {
                     "action": "drink",
                     "date": "2022-11-01",
                     "items": [
                          {
-                              "bar": 444,
-                              "foo": 333
+                              "calorie": 37.5,
+                              "name": "Coca Cola"
                          },
                          {
-                              "bar": -444,
-                              "foo": -333
+                              "calorie": 54.5,
+                              "name": "juice"
                          }
                     ]
                },
                {
-                    "action": "walk",
+                    "action": "sport",
                     "date": "2023-04-27",
                     "items": [
                          {
-                              "bar": 666,
-                              "foo": 555
+                              "calorie": -375,
+                              "name": "running"
                          },
                          {
-                              "bar": -666,
-                              "foo": -555
+                              "calorie": -350,
+                              "name": "swimming"
                          }
                     ]
                }
           ],
-          "name": "bob"
+          "name": "Bob"
      }
     ```
 
      Of course, you can use the `-O` parameter to overwrite the file with the result:
 
      ```shell
      $ jsonfmt -O example.json
      ```
 
-2. Compress the json string from stdin.
+
+2. Format a JSON object from stdin via pipeline.
+
+     ```shell
+     $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
+     ```
+
+     Output: Ditto.
+
+
+3. Compress the JSON object.
 
      ```shell
      $ echo '{
           "name": "alex",
           "age": 21,
           "items": ["pen", "ruler", "phone"]
      }' | jsonfmt -c
      ```
 
-     ouput:
+     Output:
      ```json
      {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
      ```
 
-3. Use jsonpath to match part of a json object.
+4. Use jsonpath to match part of a JSON object.
 
      **jsonfmt** uses a simplified jsonpath syntax.
 
-     - It matches json objects starting from the root node.
+     - It matches JSON objects starting from the root node.
      - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
 
           ```shell
           $ jsonfmt -p 'history/0/date' example.json
           ```
 
-          ouput:
+          Output:
           ```json
           "2021-03-02"
           ```
 
      - If you want to match all items in a list, just use `*` to match.
 
           ```shell
-          $ jsonfmt -p 'history/*/action' example.json
+          $ jsonfmt -p 'history/*/items/*/name' example.json
           ```
 
-          ouput:
+          Output:
           ```json
           [
-               "eat",
-               "drink",
-               "walk"
+               [
+                    "hamburger",
+                    "pizza"
+               ],
+               [
+                    "Coca Cola",
+                    "juice"
+               ],
+               [
+                    "running",
+                    "swimming"
+               ]
           ]
           ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jsonfmt-0.1.2/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.1.3/jsonfmt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.1.2
-Summary: A JSON object formatting tool.
-Home-page: https://github.com/seamile/jsonfmt
-Author: Seamile
-Author-email: lanhuermao@gmail.com
+Version: 0.1.3
+Summary: A simple tool for formatting JSON object.
+Author-email: Seamile <lanhuermao@gmail.com>
+License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formator
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/jsonfmt?label=Install&color=green)
 ![PyPI](https://img.shields.io/pypi/v/jsonfmt?color=9cf)
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?branch=main&label=build&logo=python)
 
 
-**jsonfmt** is a json object formatting tool.
+**jsonfmt** is a JSON object formatting tool.
 
-## Features
+It has the following features:
 
-1. Print the json object in pretty format from files or stdin.
-2. Compress the json object into a single line without spaces.
-3. Output part of a large json object via jsonpath.
+1. Print the JSON object with **hightlight** and **pretty format** from files or stdin.
+2. Compress the JSON object into a single line without spaces.
+3. Output part of a large JSON object via jsonpath.
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
 
@@ -45,127 +44,148 @@
 - positional arguments:
 
      - `json_files`   the json files that will be processed
 
 - options:
 
      - `-h, --help`: show this help message and exit.
-     - `-c`: compression the json object in the files or stdin.
+     - `-c`: compression the JSON object in the files or stdin.
+     - `-e`: escape non-ASCII characters.
+     - `-i INDENT`: number of spaces to use for indentation. (default: 4)
      - `-O`: overwrite to the json file.
-     - `-p JSONPATH`: output part of json object via jsonpath.
+     - `-p JSONPATH`: output part of JSON object via jsonpath.
      - `-v`: show the version.
 
 
 ## Example
 
-In the file example.json there is a compressed json object.
+In the file example.json there is a compressed JSON object.
 
 1. Pretty print from json file.
 
      ```shell
      $ jsonfmt example.json
      ```
 
-     ouput:
+     Output:
      ```json
      {
           "age": 23,
-          "gender": "male",
+          "gender": "纯爷们",
           "history": [
                {
                     "action": "eat",
                     "date": "2021-03-02",
                     "items": [
                          {
-                              "bar": 222,
-                              "foo": 111
+                              "calorie": 294.9,
+                              "name": "hamburger"
                          },
                          {
-                              "bar": -222,
-                              "foo": -111
+                              "calorie": 266,
+                              "name": "pizza"
                          }
                     ]
                },
                {
                     "action": "drink",
                     "date": "2022-11-01",
                     "items": [
                          {
-                              "bar": 444,
-                              "foo": 333
+                              "calorie": 37.5,
+                              "name": "Coca Cola"
                          },
                          {
-                              "bar": -444,
-                              "foo": -333
+                              "calorie": 54.5,
+                              "name": "juice"
                          }
                     ]
                },
                {
-                    "action": "walk",
+                    "action": "sport",
                     "date": "2023-04-27",
                     "items": [
                          {
-                              "bar": 666,
-                              "foo": 555
+                              "calorie": -375,
+                              "name": "running"
                          },
                          {
-                              "bar": -666,
-                              "foo": -555
+                              "calorie": -350,
+                              "name": "swimming"
                          }
                     ]
                }
           ],
-          "name": "bob"
+          "name": "Bob"
      }
     ```
 
      Of course, you can use the `-O` parameter to overwrite the file with the result:
 
      ```shell
      $ jsonfmt -O example.json
      ```
 
-2. Compress the json string from stdin.
+
+2. Format a JSON object from stdin via pipeline.
+
+     ```shell
+     $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
+     ```
+
+     Output: Ditto.
+
+
+3. Compress the JSON object.
 
      ```shell
      $ echo '{
           "name": "alex",
           "age": 21,
           "items": ["pen", "ruler", "phone"]
      }' | jsonfmt -c
      ```
 
-     ouput:
+     Output:
      ```json
      {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
      ```
 
-3. Use jsonpath to match part of a json object.
+4. Use jsonpath to match part of a JSON object.
 
      **jsonfmt** uses a simplified jsonpath syntax.
 
-     - It matches json objects starting from the root node.
+     - It matches JSON objects starting from the root node.
      - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
 
           ```shell
           $ jsonfmt -p 'history/0/date' example.json
           ```
 
-          ouput:
+          Output:
           ```json
           "2021-03-02"
           ```
 
      - If you want to match all items in a list, just use `*` to match.
 
           ```shell
-          $ jsonfmt -p 'history/*/action' example.json
+          $ jsonfmt -p 'history/*/items/*/name' example.json
           ```
 
-          ouput:
+          Output:
           ```json
           [
-               "eat",
-               "drink",
-               "walk"
+               [
+                    "hamburger",
+                    "pizza"
+               ],
+               [
+                    "Coca Cola",
+                    "juice"
+               ],
+               [
+                    "running",
+                    "swimming"
+               ]
           ]
           ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jsonfmt-0.1.2/jsonfmt.py` & `jsonfmt-0.1.3/jsonfmt.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 '''JSON Format Tool'''
 
 import json
 from sys import stdin, stdout, stderr
 from argparse import ArgumentParser
 from typing import Any, List, IO, Union
 
-__version__ = '0.1.2'
+from pygments import highlight
+from pygments.lexers import JsonLexer
+from pygments.formatters import TerminalFormatter
+
+__version__ = '0.1.3'
 
 
 def print_err(msg: str):
     print(f'\033[0;31m{msg}\033[0m', file=stderr)
 
 
 class JSONPathError(Exception):
@@ -23,34 +27,40 @@
     if output_fp.fileno() > 2:
         output_fp.seek(0)
         output_fp.truncate()
     if compression:
         json.dump(json_obj, output_fp, ensure_ascii=escape,
                   sort_keys=True, separators=(',', ':'))
     else:
-        json.dump(json_obj, output_fp, ensure_ascii=escape,
-                  sort_keys=True, indent=indent)
+        json_text = json.dumps(json_obj, ensure_ascii=escape,
+                               sort_keys=True, indent=indent)
+        # highlight the json code when outputint to TTY divice
+        if output_fp.isatty():
+            json_text = highlight(json_text, JsonLexer(), TerminalFormatter())
+        output_fp.write(json_text)
 
     # append a blank line at the end of `fp``
     output_fp.write('\n')
 
 
 def parse_jsonpath(jsonpath: str) -> List[Union[str, int]]:
+    '''parse the jsonpath into a list of pathname components'''
     jsonpath = jsonpath.strip().strip('/')
     if not jsonpath:
         return []
     else:
         components = jsonpath.split('/')
         for i, c in enumerate(components):
             if c.isdecimal():
                 components[i] = int(c)  # type: ignore
         return components  # type: ignore
 
 
-def get_element_by_components(json_obj: Any, jpath_components: List[Union[str, int]]) -> Any:
+def get_element_by_components(json_obj: Any,
+                              jpath_components: List[Union[str, int]]) -> Any:
     for i, c in enumerate(jpath_components):
         if c == '*' and isinstance(json_obj, list):
             return [get_element_by_components(sub_obj, jpath_components[i + 1:])
                     for sub_obj in json_obj]
         else:
             try:
                 json_obj = json_obj[c]
@@ -64,31 +74,35 @@
     jpath_components = parse_jsonpath(jsonpath)
     if not jpath_components:
         return json_obj
     else:
         return get_element_by_components(json_obj, jpath_components)
 
 
-def main():
+def parse_cmdline_args():
     parser = ArgumentParser('jsonfmt')
     parser.add_argument('-c', dest='compression', action='store_true',
-                        help='compression the json object in the files or stdin.')
+                        help='compression the json object in the files or stdin')
     parser.add_argument('-e', dest='escape', action='store_true',
                         help='escape non-ASCII characters')
     parser.add_argument('-i', dest='indent', type=int, default=4,
-                        help='number of spaces to use for indentation. (default: %(default)s)')
+                        help='number of spaces to use for indentation (default: %(default)s)')
     parser.add_argument('-O', dest='overwrite', action='store_true',
-                        help='overwrite the formated json object into the json file.')
+                        help='overwrite the formated json object into the json file')
     parser.add_argument('-p', dest='jsonpath', type=str, default='',
-                        help='output part of json object via jsonpath.')
+                        help='output part of json object via jsonpath')
     parser.add_argument(dest='json_files', nargs='*',
                         help='the json files that will be processed')
     parser.add_argument('-v', dest='version', action='version', version=__version__,
-                        help="show the version.")
-    args = parser.parse_args()
+                        help="show the version")
+    return parser.parse_args()
+
+
+def main():
+    args = parse_cmdline_args()
 
     if args.json_files:
         # get json from files
         for j_file in args.json_files:
             try:
                 with open(j_file, 'r+') as fp:
                     try:
```

