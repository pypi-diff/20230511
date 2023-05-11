# Comparing `tmp/docker-sand-0.0.7.tar.gz` & `tmp/docker-sand-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-sand-0.0.7.tar", last modified: Sat May  6 17:18:36 2023, max compression
+gzip compressed data, was "docker-sand-0.0.8.tar", last modified: Thu May 11 18:23:36 2023, max compression
```

## Comparing `docker-sand-0.0.7.tar` & `docker-sand-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:18:36.959024 docker-sand-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 17:18:34.000000 docker-sand-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 17:18:34.000000 docker-sand-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-06 17:18:36.959024 docker-sand-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-06 17:18:34.000000 docker-sand-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 17:18:36.000000 docker-sand-0.0.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:18:36.955024 docker-sand-0.0.7/docker_sand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-06 17:18:36.000000 docker-sand-0.0.7/docker_sand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-06 17:18:36.000000 docker-sand-0.0.7/docker_sand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:18:36.000000 docker-sand-0.0.7/docker_sand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 17:18:36.000000 docker-sand-0.0.7/docker_sand.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 17:18:36.000000 docker-sand-0.0.7/docker_sand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 17:18:36.000000 docker-sand-0.0.7/docker_sand.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:18:36.959024 docker-sand-0.0.7/sand/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:18:36.959024 docker-sand-0.0.7/sand/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/internal/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/internal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:18:36.959024 docker-sand-0.0.7/sand/internal/sandfile_executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/internal/sandfile_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/internal/sandfile_executor/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/internal/sandfile_executor/sandfile_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/internal/sandfile_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-06 17:18:34.000000 docker-sand-0.0.7/sand/sand.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:18:36.959024 docker-sand-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-06 17:18:34.000000 docker-sand-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:36.258010 docker-sand-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-11 18:23:34.000000 docker-sand-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 18:23:34.000000 docker-sand-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-11 18:23:36.254010 docker-sand-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-11 18:23:34.000000 docker-sand-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 18:23:35.000000 docker-sand-0.0.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:36.254010 docker-sand-0.0.8/docker_sand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-11 18:23:36.000000 docker-sand-0.0.8/docker_sand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-11 18:23:36.000000 docker-sand-0.0.8/docker_sand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:23:36.000000 docker-sand-0.0.8/docker_sand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 18:23:36.000000 docker-sand-0.0.8/docker_sand.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 18:23:36.000000 docker-sand-0.0.8/docker_sand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 18:23:36.000000 docker-sand-0.0.8/docker_sand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:36.254010 docker-sand-0.0.8/sand/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:36.254010 docker-sand-0.0.8/sand/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/internal/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/internal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:36.254010 docker-sand-0.0.8/sand/internal/sandfile_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/internal/sandfile_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/internal/sandfile_executor/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/internal/sandfile_executor/sandfile_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/internal/sandfile_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-11 18:23:34.000000 docker-sand-0.0.8/sand/sand.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:23:36.258010 docker-sand-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-11 18:23:34.000000 docker-sand-0.0.8/setup.py
```

### Comparing `docker-sand-0.0.7/LICENSE` & `docker-sand-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.7/PKG-INFO` & `docker-sand-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-sand
-Version: 0.0.7
+Version: 0.0.8
 Summary: Sand is a Dockerfile generator based on python that allows you to write your Dockerfile in a more convenient way.
 Home-page: https://github.com/gkpln3/Sand
 Author: Guy Kaplan
 License: MIT
 Description: # Sand 🏝
         [![.github/workflows/ci.yml](https://github.com/gkpln3/Sand/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gkpln3/Sand/actions/workflows/ci.yml)
```

### Comparing `docker-sand-0.0.7/README.md` & `docker-sand-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.7/docker_sand.egg-info/PKG-INFO` & `docker-sand-0.0.8/docker_sand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-sand
-Version: 0.0.7
+Version: 0.0.8
 Summary: Sand is a Dockerfile generator based on python that allows you to write your Dockerfile in a more convenient way.
 Home-page: https://github.com/gkpln3/Sand
 Author: Guy Kaplan
 License: MIT
 Description: # Sand 🏝
         [![.github/workflows/ci.yml](https://github.com/gkpln3/Sand/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gkpln3/Sand/actions/workflows/ci.yml)
```

### Comparing `docker-sand-0.0.7/docker_sand.egg-info/SOURCES.txt` & `docker-sand-0.0.8/docker_sand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.7/sand/internal/docker_image.py` & `docker-sand-0.0.8/sand/internal/docker_image.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.7/sand/internal/main.py` & `docker-sand-0.0.8/sand/internal/main.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.7/sand/internal/sandfile_executor/commands.py` & `docker-sand-0.0.8/sand/internal/sandfile_executor/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,25 @@
         if self.tag is not None:
             ret += f":{self.tag}"
         if self._as is not None:
             ret += f" AS {self._as}"
         return ret
 
 class RunCommand(Command):
-    def __init__(self, Command):
+    def __init__(self, Command, Mounts=None):
         self.command = Command
+        self.mounts = Mounts
 
     def serialize(self):
-        return f"RUN {self.command}"
+        cmd = f"RUN "
+        if self.mounts is not None:
+            for mount in self.mounts:
+                cmd += f"--mount={mount} "
+        cmd += self.command
+        return cmd
 
 class CopyCommand(Command):
     def __init__(self, Src, Dst, From = None):
         self.src = Src
         self.dst = Dst
         self._from = From
 
@@ -40,14 +46,22 @@
 
 class EntrypointCommand(Command):
     def __init__(self, Command):
         self.command = Command
 
     def serialize(self):
         return f"ENTRYPOINT {self.command}"
+    
+class EnvCommand(Command):
+    def __init__(self, Name, Value):
+        self.name = Name
+        self.value = Value
+
+    def serialize(self):
+        return f'ENV {self.name}="{self.value}"'
 
 class ExposeCommand(Command):
     def __init__(self, Ports):
         self.ports = Ports
 
     def serialize(self):
         return f"EXPOSE {self.ports}"
```

### Comparing `docker-sand-0.0.7/sand/internal/sandfile_executor/sandfile_executor.py` & `docker-sand-0.0.8/sand/internal/sandfile_executor/sandfile_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,44 +10,41 @@
 
 class SandfileExecutor:
     def __init__(self, path, env: dict = {}):
         # Create environment for executing Sandfile
         self.env = env
         self.path = path
         
-        # __builtins__.update(self.env)
         self._commands: list[Command] = []
         self._images: list[DockerImage] = []
 
     def execute(self) -> List[DockerImage]:
         global _current_executor
         
         # Read Sandfile from disk
         with open(self.path, "r") as f:
             sandfile_contents = f.read()
         
         # Save the current executor
         prev_executor = _current_executor
         _current_executor = self
 
-        # from ..sand import _commands
-        # self.env.update(_commands)
-
         # Execute Sandfile
         try:
             exec(sandfile_contents, self.env)
         except Exception as e:
             self.print_sandfile_exception(e)
             raise e
 
         # Restore the previous executor
         _current_executor = prev_executor
 
         # Generate Dockerfile
-        dockerfile = f"# Auto-generated by Sand, do not edit!\n"
+        dockerfile = "# syntax = docker/dockerfile:1\n" # Support BuildKit
+        dockerfile += "# Auto-generated by Sand, do not edit!\n"
         for command in self._commands:
             dockerfile += command.serialize() + "\n"
 
         if len(self._commands) > 0 and not isinstance(self._commands[0], FromCommand):
             raise Exception("Sandfile must start with an image command")
         elif len(self._commands) == 0:
             return self._images
```

### Comparing `docker-sand-0.0.7/sand/internal/sandfile_watcher.py` & `docker-sand-0.0.8/sand/internal/sandfile_watcher.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.7/sand/sand.py` & `docker-sand-0.0.8/sand/sand.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,37 +22,54 @@
     subsand = SandfileExecutor(abs_path, e._current_executor.env.copy())
     new_image = subsand.execute()
 
     # Add resulting images to current executor
     e._current_executor._images.extend(new_image)
 
 @_SandAPI
-def Run(command: str | list[str]):
+def Run(Command: str | list[str], Mount: str | list[str] = None):
+    if isinstance(Mount, str):
+        Mount = [Mount]
+
     # If command is a list, add each command to the list of commands
-    if isinstance(command, list):
-        for cmd in command:
-            e._current_executor._commands.append(RunCommand(cmd))
+    if isinstance(Command, list):
+        for cmd in Command:
+            e._current_executor._commands.append(RunCommand(cmd, Mounts=Mount))
     # If command is a string, add it to the list of commands
-    elif isinstance(command, str):
-        e._current_executor._commands.append(RunCommand(command))
+    elif isinstance(Command, str):
+        e._current_executor._commands.append(RunCommand(Command, Mounts=Mount))
     else:
         raise Exception("Invalid type in run command")
 
 @_SandAPI
 def Copy(Src, Dst, From = None):
     e._current_executor._commands.append(CopyCommand(Src, Dst, From=From))
 
 @_SandAPI
 def Entrypoint(Command):
     e._current_executor._commands.append(EntrypointCommand(Command))
 
 @_SandAPI
 def From(Image, Tag=None, As=None):
+    if ":" in Image:
+        if Tag is not None:
+            raise Exception("Cannot specify tag twice")
+        Image, Tag = Image.split(":")
     e._current_executor._commands.append(FromCommand(Image, Tag=Tag, As=As))
 
+@_SandAPI
+def Env(Name, Value=None):
+    if "=" in Name:
+        if Value is not None:
+            raise Exception("Cannot specify value twice")
+        Name, Value = Name.split("=")
+    elif Value is None:
+        raise Exception("Must specify value")
+    e._current_executor._commands.append(EnvCommand(Name, Value))
+
 
 class AttributeDict(dict):
     def __getattr__(self, attr):
         if attr in self:
             return self[attr]
         return None
```

### Comparing `docker-sand-0.0.7/setup.py` & `docker-sand-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
```

