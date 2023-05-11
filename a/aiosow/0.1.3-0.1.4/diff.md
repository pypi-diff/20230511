# Comparing `tmp/aiosow-0.1.3.tar.gz` & `tmp/aiosow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosow-0.1.3.tar", last modified: Wed May 10 14:55:49 2023, max compression
+gzip compressed data, was "aiosow-0.1.4.tar", last modified: Thu May 11 16:22:17 2023, max compression
```

## Comparing `aiosow-0.1.3.tar` & `aiosow-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.790653 aiosow-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-10 14:55:49.790653 aiosow-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-10 14:55:38.000000 aiosow-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.786653 aiosow-0.1.3/aiosow/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.790653 aiosow-0.1.3/aiosow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:55:49.790653 aiosow-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-10 14:55:38.000000 aiosow-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.790653 aiosow-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.574811 aiosow-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-11 16:22:17.574811 aiosow-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-11 16:22:02.000000 aiosow-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.566811 aiosow-0.1.4/aiosow/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.570811 aiosow-0.1.4/aiosow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:22:17.574811 aiosow-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-11 16:22:02.000000 aiosow-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.574811 aiosow-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_setup.py
```

### Comparing `aiosow-0.1.3/PKG-INFO` & `aiosow-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.3
+Version: 0.1.4
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.3/README.md` & `aiosow-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/aiosow/autofill.py` & `aiosow-0.1.4/aiosow/autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/aiosow/bindings.py` & `aiosow-0.1.4/aiosow/bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/aiosow/command.py` & `aiosow-0.1.4/aiosow/command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #! env python3.11
 
 import logging, asyncio, importlib, argparse, sys
-from aiosow.setup import initialize
-from aiosow.options import options
+from aiosow.setup import initialize, TRIGGER_ROUTINES
+from aiosow.options import options, commands
 from aiosow.routines import spawn_routine_consumer
 
 
-def load_composition(composition=None):
+def load_composition(composition=None, **kwargs):
     debug = (
         "-d" in sys.argv
         or "--debug" in sys.argv
         or any(arg.find("-d") != -1 or arg.find("--debug") != -1 for arg in sys.argv)
     )
-    if not "-h" in sys.argv:
+    if "--log" in sys.argv or kwargs.get("log", False):
         logging.basicConfig(
             level=logging.DEBUG if debug else logging.INFO,
             format="[%(asctime)s][%(levelname)s] \t%(message)s",
             datefmt="%H:%M:%S",
         )
     parser = argparse.ArgumentParser()
+
     if not composition:
         parser.add_argument("composition", help="composition to run")
     # parser.add_argument(
     #    "-c", "--config", help="Path to configuration file", default="", type=str
     # )
     parser.add_argument(
         "-d", "--debug", default=False, action="store_true", help="Debug mode"
@@ -36,47 +37,56 @@
     )
     parser.add_argument(
         "--raise",
         default=False,
         action="store_true",
         help="Routines will raise errors and stop the execution",
     )
+    parser.add_argument(
+        "--log", help="Displays logs", action="store_true", default=False
+    )
     try:
         if not composition:
             composition = sys.argv[1]
         composition = (
             f"{composition}.bindings" if not ".bindings" in composition else composition
         )
         importlib.import_module(composition)
     except Exception as e:
         logging.error("An error occured opening the composition")
         raise (e)
     for module_name in sys.modules.keys():
         if "bindings" in module_name and "aiosow" not in module_name:
             logging.info("+ composition %s", module_name)
-    logging.info("--------------------------------")
-    logging.info("-------------START--------------")
-    logging.info("--------------------------------")
     for args, kwargs in options():
         parser.add_argument(*args, **kwargs)
-    return vars(parser.parse_args())
+    for name, function in commands():
+        subparsers = parser.add_subparsers()
+        newcmd_parser = subparsers.add_parser(name)
+        newcmd_parser.set_defaults(
+            func=function
+        )  # set the default function to be called for this subcommand
+    args = parser.parse_args()
+    result = vars(args)
+    if getattr(args, "func", None):
+        args.func(args)
+        result["run_forever"] = False
+    return result
 
 
-def run(composition=None):
-    memory = load_composition(composition=composition)
+def run(composition=None, **kwargs):
+    memory = load_composition(composition=composition, **kwargs)
     logging.debug(memory)
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     tasks = loop.run_until_complete(initialize(memory))
     memory["running"] = True
-    logging.info("--------------------------------")
-    logging.info("----------SETUP--DONE-----------")
-    logging.info("--------------------------------")
-    consumer = loop.run_until_complete(spawn_routine_consumer(memory))
-    tasks = tasks + [consumer]
+    if TRIGGER_ROUTINES:
+        consumer = loop.run_until_complete(spawn_routine_consumer(memory))
+        tasks = tasks + [consumer]
     # setups can return a task which is ran here
     # this allows setups to start tasks and still have them complete
     loop.run_until_complete(asyncio.gather(*tasks))
     if memory["run_forever"]:
         loop.run_forever()
```

### Comparing `aiosow-0.1.3/aiosow/options.py` & `aiosow-0.1.4/aiosow/options.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,27 +10,50 @@
 ```
 
 Any option defined is propagated into the memory, in fact the initial memory is
 a copy of the parsed arguments.
 """
 
 OPTIONS = []
+COMMANDS = []
 
 
 def option(*args, **kwargs):  # pragma: no cover
     """
     Register an argparse option to be available using the command-line.
 
     **args**:
     - name: str -> the name of the option (will be used as f'--{name}')
     - kwargs: dict -> the options used by [argparse](https://docs.python.org/3/library/argparse.html)
     """
     global OPTIONS
     OPTIONS.append((args, kwargs))
 
 
+def command(name):
+    """
+    Register an argparse command to be available using the command-line.
+
+    **args**:
+    - name: str -> the name of the option (will be used as f'--{name}')
+    - kwargs: dict -> the options used by [argparse](https://docs.python.org/3/library/argparse.html)
+    """
+    global COMMANDS
+
+    def register(function):
+        COMMANDS.append((name, function))
+        return function
+
+    return register
+
+
 def options():  # pragma: no cover
     global OPTIONS
     return OPTIONS
 
 
-__all__ = ["option"]
+def commands():  # pragma: no cover
+    global COMMANDS
+    return COMMANDS
+
+
+__all__ = ["option", "command"]
```

### Comparing `aiosow-0.1.3/aiosow/perpetuate.py` & `aiosow-0.1.4/aiosow/perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/aiosow/routines.py` & `aiosow-0.1.4/aiosow/routines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Callable
 from functools import wraps
 
 import asyncio, logging
 
 from aiosow.perpetuate import perpetuate, autofill
 from aiosow.bindings import return_true
+from aiosow.setup import trigger_routines
+
+trigger_routines()
 
 
 def infinite_generator(condition: Callable):
     def _generator_consumer(function: Callable):
         """Re-autofill a generator function at end of it's loop"""
 
         iterated = None
@@ -72,16 +75,19 @@
 
     return decorator
 
 
 async def consume_routines(memory):
     routines = get_routines()
     # Find the routine with the smallest remaining timeout or a timeout <= 0
-    smallest_timeout_routine = min(routines, key=lambda x: x["timeout"])
-    smallest_timeout = smallest_timeout_routine["timeout"]
+    if len(routines):
+        smallest_timeout_routine = min(routines, key=lambda x: x["timeout"])
+        smallest_timeout = smallest_timeout_routine["timeout"]
+    else:
+        smallest_timeout = 0
 
     # Wait until the smallest timeout has elapsed
     await asyncio.sleep(smallest_timeout)
 
     # Execute any routines that have timed out
     for routine in routines:
         routine["timeout"] -= smallest_timeout
```

### Comparing `aiosow-0.1.3/aiosow/setup.py` & `aiosow-0.1.4/aiosow/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import logging, asyncio
 from typing import Dict, List, Callable
 from aiosow.perpetuate import perpetuate
 
 SETUP_FUNCTIONS: List = []
+TRIGGER_ROUTINES = False
+
+
+def trigger_routines():
+    global TRIGGER_ROUTINES
+    TRIGGER_ROUTINES = True
 
 
 def clear_setups():  # pragma: no cover
     global SETUP_FUNCTIONS
     SETUP_FUNCTIONS = []
```

### Comparing `aiosow-0.1.3/aiosow.egg-info/PKG-INFO` & `aiosow-0.1.4/aiosow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.3
+Version: 0.1.4
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.3/setup.py` & `aiosow-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="aiosow",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(include=["aiosow"]),
     description="An event-based framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     entry_points={
         "console_scripts": [
```

### Comparing `aiosow-0.1.3/tests/test_autofill.py` & `aiosow-0.1.4/tests/test_autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/tests/test_bindings.py` & `aiosow-0.1.4/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/tests/test_perpetuate.py` & `aiosow-0.1.4/tests/test_perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/tests/test_routines.py` & `aiosow-0.1.4/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.3/tests/test_setup.py` & `aiosow-0.1.4/tests/test_setup.py`

 * *Files identical despite different names*

