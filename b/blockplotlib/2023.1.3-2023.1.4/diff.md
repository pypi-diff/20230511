# Comparing `tmp/blockplotlib-2023.1.3.tar.gz` & `tmp/blockplotlib-2023.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockplotlib-2023.1.3.tar", last modified: Wed May 10 21:27:08 2023, max compression
+gzip compressed data, was "blockplotlib-2023.1.4.tar", last modified: Thu May 11 13:17:18 2023, max compression
```

## Comparing `blockplotlib-2023.1.3.tar` & `blockplotlib-2023.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:27:08.077532 blockplotlib-2023.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-10 21:26:54.000000 blockplotlib-2023.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-10 21:27:08.077532 blockplotlib-2023.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:27:08.073532 blockplotlib-2023.1.3/blockplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 21:26:54.000000 blockplotlib-2023.1.3/blockplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-10 21:26:54.000000 blockplotlib-2023.1.3/blockplotlib/blockplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:27:08.077532 blockplotlib-2023.1.3/blockplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-10 21:27:08.000000 blockplotlib-2023.1.3/blockplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-10 21:27:08.000000 blockplotlib-2023.1.3/blockplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:27:08.000000 blockplotlib-2023.1.3/blockplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 21:27:08.000000 blockplotlib-2023.1.3/blockplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 21:27:08.000000 blockplotlib-2023.1.3/blockplotlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:27:08.077532 blockplotlib-2023.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-10 21:26:54.000000 blockplotlib-2023.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:17:18.062939 blockplotlib-2023.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-11 13:17:05.000000 blockplotlib-2023.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-11 13:17:18.062939 blockplotlib-2023.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:17:18.058939 blockplotlib-2023.1.4/blockplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 13:17:05.000000 blockplotlib-2023.1.4/blockplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-11 13:17:05.000000 blockplotlib-2023.1.4/blockplotlib/blockplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:17:18.062939 blockplotlib-2023.1.4/blockplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-11 13:17:18.000000 blockplotlib-2023.1.4/blockplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 13:17:18.000000 blockplotlib-2023.1.4/blockplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:17:18.000000 blockplotlib-2023.1.4/blockplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 13:17:18.000000 blockplotlib-2023.1.4/blockplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 13:17:18.000000 blockplotlib-2023.1.4/blockplotlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:17:18.062939 blockplotlib-2023.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-11 13:17:05.000000 blockplotlib-2023.1.4/setup.py
```

### Comparing `blockplotlib-2023.1.3/LICENSE` & `blockplotlib-2023.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blockplotlib-2023.1.3/PKG-INFO` & `blockplotlib-2023.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: blockplotlib
-Version: 2023.1.3
+Version: 2023.1.4
 Summary: Matplotlib-based library for the creation of block diagrams
+Home-page: https://github.com/riemarc/blockplotlib
 Author: Marcus Riesmeier
 Author-email: gluehen-sierren-0c@icloud.com
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -27,22 +28,24 @@
 demonstrated in the examples but can be extended quite easily.
 
 ## Examples
 
 How to draw a simple control loop is illustrated with the
 example `blockplotlib/examples/control_loop_one_dof.py`.
 
-![control_loop_one_dof](https://github.com/riemarc/blockplotlib/assets/18379817/7be3ba47-7e22-4965-98a3-467b6b47969b)
+<img src="https://github.com/riemarc/blockplotlib/assets/18379817/7be3ba47-7e22-4965-98a3-467b6b47969b" width="60%">
+
 [control_loop_one_dof.pdf](https://github.com/riemarc/blockplotlib/files/11445397/control_loop_one_dof.pdf)
 
 A more complex example is the block diagram of the
 so-called hyperbolic observer canonical form:
 `blockplotlib/examples/hyperbolic_ocf.py`
 
-![hyperbolic_ocf](https://github.com/riemarc/blockplotlib/assets/18379817/5148f97a-12b8-4c1f-af6f-6d4b741f22c1)
+<img src="https://github.com/riemarc/blockplotlib/assets/18379817/5148f97a-12b8-4c1f-af6f-6d4b741f22c1" width="80%">
+
 [hyperbolic_ocf.pdf](https://github.com/riemarc/blockplotlib/files/11445461/hyperbolic_ocf.pdf)
 
 The inclusion of matplotlib figures with the correct
 font size into a latex document can be adapted
 from the example under `blockplotlib/examples/tex_article`.
 It basically relies on two measurements of the height of a string.
 One measurement is performed in the latex preamble and the
```

### Comparing `blockplotlib-2023.1.3/blockplotlib/blockplotlib.py` & `blockplotlib-2023.1.4/blockplotlib/blockplotlib.py`

 * *Files identical despite different names*

### Comparing `blockplotlib-2023.1.3/blockplotlib.egg-info/PKG-INFO` & `blockplotlib-2023.1.4/blockplotlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: blockplotlib
-Version: 2023.1.3
+Version: 2023.1.4
 Summary: Matplotlib-based library for the creation of block diagrams
+Home-page: https://github.com/riemarc/blockplotlib
 Author: Marcus Riesmeier
 Author-email: gluehen-sierren-0c@icloud.com
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -27,22 +28,24 @@
 demonstrated in the examples but can be extended quite easily.
 
 ## Examples
 
 How to draw a simple control loop is illustrated with the
 example `blockplotlib/examples/control_loop_one_dof.py`.
 
-![control_loop_one_dof](https://github.com/riemarc/blockplotlib/assets/18379817/7be3ba47-7e22-4965-98a3-467b6b47969b)
+<img src="https://github.com/riemarc/blockplotlib/assets/18379817/7be3ba47-7e22-4965-98a3-467b6b47969b" width="60%">
+
 [control_loop_one_dof.pdf](https://github.com/riemarc/blockplotlib/files/11445397/control_loop_one_dof.pdf)
 
 A more complex example is the block diagram of the
 so-called hyperbolic observer canonical form:
 `blockplotlib/examples/hyperbolic_ocf.py`
 
-![hyperbolic_ocf](https://github.com/riemarc/blockplotlib/assets/18379817/5148f97a-12b8-4c1f-af6f-6d4b741f22c1)
+<img src="https://github.com/riemarc/blockplotlib/assets/18379817/5148f97a-12b8-4c1f-af6f-6d4b741f22c1" width="80%">
+
 [hyperbolic_ocf.pdf](https://github.com/riemarc/blockplotlib/files/11445461/hyperbolic_ocf.pdf)
 
 The inclusion of matplotlib figures with the correct
 font size into a latex document can be adapted
 from the example under `blockplotlib/examples/tex_article`.
 It basically relies on two measurements of the height of a string.
 One measurement is performed in the latex preamble and the
```

### Comparing `blockplotlib-2023.1.3/setup.py` & `blockplotlib-2023.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
         return file.read()
 
 long_description = read_file("readme.md")
 requirements = read_file("requirements.txt").splitlines()
 
 setuptools.setup(
     name="blockplotlib",
-    version="2023.1.3",
+    version="2023.1.4",
+    url="https://github.com/riemarc/blockplotlib",
     author="Marcus Riesmeier",
     author_email="gluehen-sierren-0c@icloud.com",
     license="BSD 3-Clause License",
     description=description,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=setuptools.find_packages(),
```

