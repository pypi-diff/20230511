# Comparing `tmp/juts-2023.4.1.tar.gz` & `tmp/juts-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juts-2023.4.1.tar", last modified: Tue May  9 22:44:35 2023, max compression
+gzip compressed data, was "juts-2023.4.2.tar", last modified: Thu May 11 13:16:18 2023, max compression
```

## Comparing `juts-2023.4.1.tar` & `juts-2023.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-09 22:44:22.000000 juts-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 22:44:35.115958 juts-2023.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/customjobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/customjobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/customplots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/customplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/customplots/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/plotwidgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    27135 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:44:35.115958 juts-2023.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-09 22:44:22.000000 juts-2023.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:18.056861 juts-2023.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-11 13:16:05.000000 juts-2023.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-11 13:16:18.056861 juts-2023.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:18.052861 juts-2023.4.2/juts/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:18.052861 juts-2023.4.2/juts/customjobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/customjobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:18.056861 juts-2023.4.2/juts/customplots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/customplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/customplots/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/plotwidgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:18.056861 juts-2023.4.2/juts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27135 2023-05-11 13:16:05.000000 juts-2023.4.2/juts/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:16:18.052861 juts-2023.4.2/juts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-11 13:16:18.000000 juts-2023.4.2/juts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-11 13:16:18.000000 juts-2023.4.2/juts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:16:18.000000 juts-2023.4.2/juts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 13:16:18.000000 juts-2023.4.2/juts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 13:16:18.000000 juts-2023.4.2/juts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:16:18.056861 juts-2023.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-11 13:16:05.000000 juts-2023.4.2/setup.py
```

### Comparing `juts-2023.4.1/LICENSE` & `juts-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/PKG-INFO` & `juts-2023.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: juts
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Jupyter widgets for scheduling processes and visualizing the resulting (live) data
+Home-page: https://github.com/riemarc/juts
 Author: Marcus Riesmeier
 Author-email: gluehen-sierren-0c@icloud.com
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -58,39 +59,39 @@
     parameter:
         n: 10
         x: 0.3
 ```
 
 or can be defined as python dictionary.
 
-[Screencast min example.webm](https://github.com/riemarc/juts/assets/18379817/0fa83a34-cefd-4f1e-99e9-49642ab31963)
+[Screencast min example.webm](https://github.com/riemarc/juts/assets/18379817/d711701a-4aea-4bd6-9d26-2e476c60b274)
 
 Also live data can be monitored during script execution:
 
-[Screencast min example live.webm](https://github.com/riemarc/juts/assets/18379817/99211beb-424d-4841-bc71-953307306967)
+[Screencast min example live.webm](https://github.com/riemarc/juts/assets/18379817/c5ac1676-ceae-42ea-a652-8128c4e4c466)
 
 
 ## A simulation example
 
 A more practical relevant example is the following simulation of a reaction
 wheel pendulum under state feedback control.
 
-[Screencast pendulum.webm](https://github.com/riemarc/juts/assets/18379817/3e8c9edc-12aa-496f-ba14-4c0adc677900)
+[Screencast pendulum.webm](https://github.com/riemarc/juts/assets/18379817/f4cbbf97-d2cb-410d-a834-11c9422ddc27)
 
 Widgets can be easily connected if required:
 
-[Screencast pendulum link.webm](https://github.com/riemarc/juts/assets/18379817/cb8567b2-4ec8-4d9c-9f09-1cb466accbb7)
+[Screencast pendulum link.webm](https://github.com/riemarc/juts/assets/18379817/e6342830-6258-4ca1-b8ed-0b1654e03444)
 
 Since the simulation runs quite
 fast, a loop was put after it which sends the data with a delay. This shows that
 a job could also record live data from an experiment, so one could compare the
 simulation data with the measurements from a real pendulum.
 
-[Screencast pendulum live.webm](https://github.com/riemarc/juts/assets/18379817/f8759a47-58ba-43f3-8196-8e319ea82b65)
+[Screencast pendulum live.webm](https://github.com/riemarc/juts/assets/18379817/dc0edbe0-8b5a-424a-91bf-eef0b944d14b)
 
 
 ## Visualizing 3D data
 
 An example plot widget to view 3D data is also included.
 This one relies on [ipyvolume](https://github.com/widgetti/ipyvolume).
 
-[Screencast 3d.webm](https://github.com/riemarc/juts/assets/18379817/637269ed-9e42-4dce-8054-e64aafbd48ca)
+[Screencast 3d.webm](https://github.com/riemarc/juts/assets/18379817/762806cf-38b1-4f6d-ba5c-071bcbbcb9e2)
```

### Comparing `juts-2023.4.1/juts/container.py` & `juts-2023.4.2/juts/container.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts/customplots/matplotlib.py` & `juts-2023.4.2/juts/customplots/matplotlib.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts/interface.py` & `juts-2023.4.2/juts/interface.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts/plotwidgets.py` & `juts-2023.4.2/juts/plotwidgets.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts/tests/test_container.py` & `juts-2023.4.2/juts/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts/tests/test_interface.py` & `juts-2023.4.2/juts/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts/tests/test_widgets.py` & `juts-2023.4.2/juts/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts/widgets.py` & `juts-2023.4.2/juts/widgets.py`

 * *Files identical despite different names*

### Comparing `juts-2023.4.1/juts.egg-info/PKG-INFO` & `juts-2023.4.2/juts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: juts
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Jupyter widgets for scheduling processes and visualizing the resulting (live) data
+Home-page: https://github.com/riemarc/juts
 Author: Marcus Riesmeier
 Author-email: gluehen-sierren-0c@icloud.com
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -58,39 +59,39 @@
     parameter:
         n: 10
         x: 0.3
 ```
 
 or can be defined as python dictionary.
 
-[Screencast min example.webm](https://github.com/riemarc/juts/assets/18379817/0fa83a34-cefd-4f1e-99e9-49642ab31963)
+[Screencast min example.webm](https://github.com/riemarc/juts/assets/18379817/d711701a-4aea-4bd6-9d26-2e476c60b274)
 
 Also live data can be monitored during script execution:
 
-[Screencast min example live.webm](https://github.com/riemarc/juts/assets/18379817/99211beb-424d-4841-bc71-953307306967)
+[Screencast min example live.webm](https://github.com/riemarc/juts/assets/18379817/c5ac1676-ceae-42ea-a652-8128c4e4c466)
 
 
 ## A simulation example
 
 A more practical relevant example is the following simulation of a reaction
 wheel pendulum under state feedback control.
 
-[Screencast pendulum.webm](https://github.com/riemarc/juts/assets/18379817/3e8c9edc-12aa-496f-ba14-4c0adc677900)
+[Screencast pendulum.webm](https://github.com/riemarc/juts/assets/18379817/f4cbbf97-d2cb-410d-a834-11c9422ddc27)
 
 Widgets can be easily connected if required:
 
-[Screencast pendulum link.webm](https://github.com/riemarc/juts/assets/18379817/cb8567b2-4ec8-4d9c-9f09-1cb466accbb7)
+[Screencast pendulum link.webm](https://github.com/riemarc/juts/assets/18379817/e6342830-6258-4ca1-b8ed-0b1654e03444)
 
 Since the simulation runs quite
 fast, a loop was put after it which sends the data with a delay. This shows that
 a job could also record live data from an experiment, so one could compare the
 simulation data with the measurements from a real pendulum.
 
-[Screencast pendulum live.webm](https://github.com/riemarc/juts/assets/18379817/f8759a47-58ba-43f3-8196-8e319ea82b65)
+[Screencast pendulum live.webm](https://github.com/riemarc/juts/assets/18379817/dc0edbe0-8b5a-424a-91bf-eef0b944d14b)
 
 
 ## Visualizing 3D data
 
 An example plot widget to view 3D data is also included.
 This one relies on [ipyvolume](https://github.com/widgetti/ipyvolume).
 
-[Screencast 3d.webm](https://github.com/riemarc/juts/assets/18379817/637269ed-9e42-4dce-8054-e64aafbd48ca)
+[Screencast 3d.webm](https://github.com/riemarc/juts/assets/18379817/762806cf-38b1-4f6d-ba5c-071bcbbcb9e2)
```

