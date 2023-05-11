# Comparing `tmp/robotcode_robot-0.36.0.tar.gz` & `tmp/robotcode_robot-0.37.0.tar.gz`

## Comparing `robotcode_robot-0.36.0.tar` & `robotcode_robot-0.37.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    77317 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/pyproject.toml
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.36.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    78357 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/README.md
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/pyproject.toml
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 robotcode_robot-0.37.0/PKG-INFO
```

### Comparing `robotcode_robot-0.36.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.37.0/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.36.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.37.0/src/robotcode/robot/config/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,15 @@
                         else:
                             result.append(str(item))
                 elif isinstance(value, dict):
                     for key, item in value.items():
                         append_name(field)
                         if isinstance(item, list):
                             separator = ";" if any(True for s in item if ":" in s) else ":"
-                            result.append(f"{key}{separator}{separator.join(item)}")
+                            result.append(f"{key}{separator if item else ''}{separator.join(item)}")
                         else:
                             result.append(f"{key}:{item}")
                 else:
                     append_name(field)
                     result.append(str(value))
             except EvaluationError as e:
                 raise ValueError(f"Evaluation of '{field.name}' failed: {str(e)}") from e
@@ -533,17 +533,18 @@
         robot_name="outputdir",
         robot_priority=500,
         robot_short_name="d",
     )
     pre_rebot_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Class to programmatically modify the result
-            model before creating reports and logs.
+            model before creating reports and logs. Accepts
+            arguments the same way as with --listener.
 
-            corresponds to the `--prerebotmodifier class *` option of _robot_
+            corresponds to the `--prerebotmodifier modifier *` option of _robot_
             """,
         robot_name="prerebotmodifier",
         robot_priority=500,
     )
     python_path: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Additional locations (directories, ZIPs) where to
@@ -938,17 +939,18 @@
             """,
     )
     extra_pre_rebot_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Appends entries to the --prerebotmodifier option.
 
             Class to programmatically modify the result
-            model before creating reports and logs.
+            model before creating reports and logs. Accepts
+            arguments the same way as with --listener.
 
-            corresponds to the `--prerebotmodifier class *` option of _robot_
+            corresponds to the `--prerebotmodifier modifier *` option of _robot_
             """,
     )
     extra_python_path: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --pythonpath option.
 
             Additional locations (directories, ZIPs) where to
@@ -1273,27 +1275,27 @@
             corresponds to the `--language lang *` option of _robot_
             """,
         robot_name="language",
         robot_priority=500,
     )
     listeners: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
-            A class for monitoring test execution. Gets
-            notifications e.g. when tests start and end.
+            Class or module for monitoring test execution.
+            Gets notifications e.g. when tests start and end.
             Arguments to the listener class can be given after
             the name using a colon or a semicolon as a separator.
 
             Examples:
 
             ```
-            --listener MyListenerClass
+            --listener MyListener
             --listener path/to/Listener.py:arg1:arg2
             ```
 
-            corresponds to the `--listener class *` option of _robot_
+            corresponds to the `--listener listener *` option of _robot_
             """,
         robot_name="listener",
         robot_priority=500,
     )
     log_level: Optional[Union[str, StringExpression]] = field(
         description="""\
             Threshold level for logging. Available levels: TRACE,
@@ -1350,20 +1352,31 @@
 
             corresponds to the `-o --output file` option of _robot_
             """,
         robot_name="output",
         robot_priority=500,
         robot_short_name="o",
     )
+    parsers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
+        description="""\
+            Custom parser class or module. Parser classes accept
+            arguments the same way as with --listener.
+
+            corresponds to the `--parser parser *` option of _robot_
+            """,
+        robot_name="parser",
+        robot_priority=500,
+    )
     pre_run_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Class to programmatically modify the suite
-            structure before execution.
+            structure before execution. Accepts arguments the
+            same way as with --listener.
 
-            corresponds to the `--prerunmodifier class *` option of _robot_
+            corresponds to the `--prerunmodifier modifier *` option of _robot_
             """,
         robot_name="prerunmodifier",
         robot_priority=500,
     )
     quiet: Union[bool, Flag, None] = field(
         description="""\
             Shortcut for `--console quiet`.
@@ -1519,37 +1532,48 @@
             corresponds to the `--language lang *` option of _rebot_
             """,
     )
     extra_listeners: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Appends entries to the --listener option.
 
-            A class for monitoring test execution. Gets
-            notifications e.g. when tests start and end.
+            Class or module for monitoring test execution.
+            Gets notifications e.g. when tests start and end.
             Arguments to the listener class can be given after
             the name using a colon or a semicolon as a separator.
 
             Examples:
 
             ```
-            --listener MyListenerClass
+            --listener MyListener
             --listener path/to/Listener.py:arg1:arg2
             ```
 
-            corresponds to the `--listener class *` option of _rebot_
+            corresponds to the `--listener listener *` option of _rebot_
+            """,
+    )
+    extra_parsers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
+        description="""\
+            Appends entries to the --parser option.
+
+            Custom parser class or module. Parser classes accept
+            arguments the same way as with --listener.
+
+            corresponds to the `--parser parser *` option of _rebot_
             """,
     )
     extra_pre_run_modifiers: Optional[Dict[str, List[Union[str, StringExpression]]]] = field(
         description="""\
             Appends entries to the --prerunmodifier option.
 
             Class to programmatically modify the suite
-            structure before execution.
+            structure before execution. Accepts arguments the
+            same way as with --listener.
 
-            corresponds to the `--prerunmodifier class *` option of _rebot_
+            corresponds to the `--prerunmodifier modifier *` option of _rebot_
             """,
     )
     extra_skip: Optional[List[Union[str, StringExpression]]] = field(
         description="""\
             Appends entries to the --skip option.
 
             Tests having given tag will be skipped. Tag can be
```

### Comparing `robotcode_robot-0.36.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.37.0/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.36.0/.gitignore` & `robotcode_robot-0.37.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.36.0/LICENSE.txt` & `robotcode_robot-0.37.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.36.0/README.md` & `robotcode_robot-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.36.0/pyproject.toml` & `robotcode_robot-0.37.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
-  "robotcode-core==0.36.0",
+  "robotcode-core==0.37.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.36.0/PKG-INFO` & `robotcode_robot-0.37.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.36.0
+Version: 0.37.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.36.0
+Requires-Dist: robotcode-core==0.37.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

