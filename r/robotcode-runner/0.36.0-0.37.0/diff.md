# Comparing `tmp/robotcode_runner-0.36.0.tar.gz` & `tmp/robotcode_runner-0.37.0.tar.gz`

## Comparing `robotcode_runner-0.36.0.tar` & `robotcode_runner-0.37.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0     8441 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.36.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    18803 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.37.0/PKG-INFO
```

### Comparing `robotcode_runner-0.36.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.37.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.36.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.37.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.36.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.37.0/src/robotcode/runner/cli/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.app = app
         self.paths = paths
         self.dry = dry
         self.root_folder = root_folder
         self._orig_cwd = Path.cwd()
 
     def parse_arguments(self, cli_args: Any) -> Any:
-        if self.root_folder is not None:
+        if self.root_folder is not None and Path.cwd() != self.root_folder:
             self.app.verbose(f"Changing working directory from {self._orig_cwd} to {self.root_folder}")
             os.chdir(self.root_folder)
 
         try:
             options, arguments = super().parse_arguments(cli_args)
             if self.root_folder is not None:
                 for i, arg in enumerate(arguments.copy()):
@@ -117,15 +117,15 @@
 
     if profile.env:
         for k, v in profile.env.items():
             os.environ[k] = v
             app.verbose(lambda: f"Set environment variable {k} to {v}")
 
     app.verbose(
-        lambda: "Executing robot with the following options:\n    "
+        lambda: "Executing robot with following options:\n    "
         + " ".join(f'"{o}"' for o in (cmd_options + list(robot_options_and_args)))
     )
 
     return root_folder, profile, cmd_options
 
 
 @click.command(
@@ -161,15 +161,19 @@
     )
 
     app.exit(
         cast(
             int,
             RobotFrameworkEx(
                 app,
-                [] if profile.paths is None else profile.paths if isinstance(profile.paths, list) else [profile.paths],
+                [*(app.config.default_paths if app.config.default_paths else ())]
+                if profile.paths is None
+                else profile.paths
+                if isinstance(profile.paths, list)
+                else [profile.paths],
                 app.config.dry,
                 root_folder,
             ).execute_cli(
                 (*cmd_options, *robot_options_and_args),
                 exit=False,
             ),
         )
```

### Comparing `robotcode_runner-0.36.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.37.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.36.0/.gitignore` & `robotcode_runner-0.37.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.36.0/LICENSE.txt` & `robotcode_runner-0.37.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.36.0/README.md` & `robotcode_runner-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.36.0/pyproject.toml` & `robotcode_runner-0.37.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.36.0",
-  "robotcode-modifiers==0.36.0",
-  "robotcode==0.36.0",
+  "robotcode-robot==0.37.0",
+  "robotcode-modifiers==0.37.0",
+  "robotcode==0.37.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.36.0/PKG-INFO` & `robotcode_runner-0.37.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.36.0
+Version: 0.37.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.36.0
-Requires-Dist: robotcode-robot==0.36.0
-Requires-Dist: robotcode==0.36.0
+Requires-Dist: robotcode-modifiers==0.37.0
+Requires-Dist: robotcode-robot==0.37.0
+Requires-Dist: robotcode==0.37.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

