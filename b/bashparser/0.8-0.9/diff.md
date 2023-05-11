# Comparing `tmp/bashparser-0.8.tar.gz` & `tmp/bashparser-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bashparser-0.8.tar", last modified: Fri Apr 14 20:38:56 2023, max compression
+gzip compressed data, was "bashparser-0.9.tar", last modified: Wed Apr 19 01:47:08 2023, max compression
```

## Comparing `bashparser-0.8.tar` & `bashparser-0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 20:38:43.000000 bashparser-0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 20:38:56.216926 bashparser-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-04-14 20:38:43.000000 bashparser-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/bashparser/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2200 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20757 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/ast.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7410 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/chunk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/complexity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8432 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5761 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/generalize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/bashparser/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_unroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/test/test_variable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1981 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/unroll.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13416 2023-04-14 20:38:43.000000 bashparser-0.8/bashparser/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:38:56.216926 bashparser-0.8/bashparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 20:38:56.000000 bashparser-0.8/bashparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-14 20:38:56.216926 bashparser-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-14 20:38:43.000000 bashparser-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:47:08.478612 bashparser-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 01:46:50.000000 bashparser-0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 01:47:08.478612 bashparser-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23862 2023-04-19 01:46:50.000000 bashparser-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:47:08.474612 bashparser-0.9/bashparser/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2200 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20757 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/ast.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7410 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/chunk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/complexity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8432 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5621 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/generalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3891 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:47:08.478612 bashparser-0.9/bashparser/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/test_unroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/test/test_variable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/unroll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13416 2023-04-19 01:46:50.000000 bashparser-0.9/bashparser/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:47:08.474612 bashparser-0.9/bashparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 01:47:08.000000 bashparser-0.9/bashparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-19 01:47:08.000000 bashparser-0.9/bashparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 01:47:08.000000 bashparser-0.9/bashparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 01:47:08.000000 bashparser-0.9/bashparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 01:47:08.000000 bashparser-0.9/bashparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 01:47:08.000000 bashparser-0.9/bashparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-19 01:47:08.478612 bashparser-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-19 01:46:50.000000 bashparser-0.9/setup.py
```

### Comparing `bashparser-0.8/LICENSE.txt` & `bashparser-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/README.md` & `bashparser-0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
 
 # UNROLL
 
 The file unroll.py can be called from the CLI passing a --file argument to specify the bash script you wish to unroll. Passing the --cmd flag will return the commands executed without any replacement, ie calling strip_cmd, otherwise advanced_unroll is used
 
 **strip_cmd(nodes)** - Strips all the commands executed from a series of bash nodes in order. No replacement occurs, it simply returns the raw commands.
 
-**advanced_unroll(nodes, var_list={}, fn_dict={}, alias_table={})** - This function strips the commands executed by the series of bash nodes after resolving and command aliasing, function calls, and variable substitutions. 
+**advanced_unroll(nodes, var_list={}, fn_dict={}, alias_table={}, strip_cmds=True)** - This function resolves command aliasing, function calls, and variable substitutions in a series of bash nodes, replacing as it progresses. The strip_cmds boolean can be toggeled to return only the commands executed or the replaced nodes. 
 
 
 
 <br/>
 
 # COMPLEXITY
```

### Comparing `bashparser-0.8/bashparser/__init__.py` & `bashparser-0.9/bashparser/__init__.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/ast.py` & `bashparser-0.9/bashparser/ast.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/chunk.py` & `bashparser-0.9/bashparser/chunk.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/commands.py` & `bashparser-0.9/bashparser/commands.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/complexity.py` & `bashparser-0.9/bashparser/complexity.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/functions.py` & `bashparser-0.9/bashparser/functions.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/generalize.py` & `bashparser-0.9/bashparser/generalize.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     amoung the arguments. Start the parameter count at 0 and go up from there 
     referencing a dictionary to maintain internal consistency
     The number shouldn't matter but the pattern of the numbers will """
     if type(generalize_nodes) is not list: generalize_nodes = [ generalize_nodes ]
 
     for node in generalize_nodes:
         if node.kind == 'word':
-            print('here1')
             if node.word not in params_used: 
-                print('here2')
                 params_used[node.word] = str(param_num) 
                 param_num += 1
             node.word = '%' + params_used[node.word]
         if hasattr(node, 'parts'):
             if node.kind == 'command':
                 if node.parts[0].kind == 'assignment':
                     # Should the variable assignments always be different? I think yes
@@ -54,17 +52,15 @@
                     value_assigned = node.parts[0].word.split('=', 1)[1]
                     if value_assigned not in params_used:
                         params_used[value_assigned] = param_num 
                         param_num += 1
                     node.parts[0].word = "%d=%" + str(params_used[value_assigned])
                 for i in range(1, len(node.parts)):
                     if hasattr(node.parts[i], 'word'):
-                        print('here3')
                         if node.parts[i].word not in params_used: 
-                            print('here4')
                             params_used[node.parts[i].word] = str(param_num) 
                             param_num += 1
                         node.parts[i].word = '%' + str(params_used[node.parts[i].word])
             else:
                 for part in node.parts:
                     param_num = parameter_tracking_generalization(part, params_used, param_num)
```

### Comparing `bashparser-0.8/bashparser/template.py` & `bashparser-0.9/bashparser/template.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/test/test_ast.py` & `bashparser-0.9/bashparser/test/test_ast.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/test/test_command.py` & `bashparser-0.9/bashparser/test/test_command.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/test/test_features.py` & `bashparser-0.9/bashparser/test/test_features.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/test/test_functions.py` & `bashparser-0.9/bashparser/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/test/test_unroll.py` & `bashparser-0.9/bashparser/test/test_unroll.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/test/test_variable.py` & `bashparser-0.9/bashparser/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser/unroll.py` & `bashparser-0.9/bashparser/unroll.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,26 +28,30 @@
 		vstr = NodeVisitor(node)
 		vstr.nodes = []
 		vstr.apply(apply_fn, vstr)
 		unrolled_commands += vstr.nodes
 	return unrolled_commands
 
 
-def advanced_unroll(nodes, var_list={}, fn_dict={}, alias_table={}):
+def advanced_unroll(nodes, var_list={}, fn_dict={}, alias_table={}, strip_cmds=True):
 	# The ordering of this function is important. Tread lightly
 
 	nodes = bashparser.build_and_resolve_aliasing(nodes, alias_table)
 
 	nodes = bashparser.build_and_resolve_fns(nodes, fn_dict)
 
 	nodes = bashparser.substitute_variables(nodes, var_list)
 
-	commands = strip_cmd(nodes)
+	if strip_cmds:
+		ret_val = strip_cmd(nodes)
+	else:
+		ret_val = nodes
+
+	return ret_val
 
-	return commands
 
 def main():
 	import argparse
 
 	parser = argparse.ArgumentParser()
 	parser.add_argument("--cmds", help='Strip the commands from the bash file', action='store_true')
 	parser.add_argument("--file", help="The filename of the bash script you'd like to unroll", type=str)
```

### Comparing `bashparser-0.8/bashparser/variables.py` & `bashparser-0.9/bashparser/variables.py`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/bashparser.egg-info/SOURCES.txt` & `bashparser-0.9/bashparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bashparser-0.8/setup.cfg` & `bashparser-0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bashparser
-version = 0.8
+version = 0.9
 author = Spencer Stingley
 description = A framework for manipulating and analysing bash scripts
 long_description = A framework for manipulating and analysing bash scripts
 url = https://github.com/BlankCanvasStudio/bashparse
 keywords = bash, parsing, analysis
 python_requires = >=3.6
 classifiers =
```

### Comparing `bashparser-0.8/setup.py` & `bashparser-0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bashparser",
-    version="0.8",
+    version="0.9",
     author="Spencer Stingley",
     author_email="sstingle@usc.edu",
     description="A framework for manipulating and analysing bash scripts",
     long_description="A framework for manipulating and analysing bash scripts",
     long_description_content_type="text/markdown",
     url="https://github.com/BlankCanvasStudio/bashparse",
     packages=setuptools.find_packages(),
```

