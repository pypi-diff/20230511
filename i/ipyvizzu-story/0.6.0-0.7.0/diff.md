# Comparing `tmp/ipyvizzu-story-0.6.0.tar.gz` & `tmp/ipyvizzu-story-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvizzu-story-0.6.0.tar", last modified: Sat Mar 11 17:40:36 2023, max compression
+gzip compressed data, was "ipyvizzu-story-0.7.0.tar", last modified: Thu May 11 05:25:47 2023, max compression
```

## Comparing `ipyvizzu-story-0.6.0.tar` & `ipyvizzu-story-0.7.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-03-11 17:40:32.000000 ipyvizzu-story-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.875416 ipyvizzu-story-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-03-11 17:40:36.000000 ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-11 17:40:36.000000 ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 17:40:36.000000 ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-11 17:40:36.000000 ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-11 17:40:36.000000 ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzustory/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/ipy/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/ipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/ipy/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/pn/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/pn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/pn/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/py/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/py/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/st/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/env/st/story.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:40:36.879416 ipyvizzu-story-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/tests/test_datafilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/tests/test_slide.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/tests/test_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-03-11 17:40:27.000000 ipyvizzu-story-0.6.0/tests/test_storylib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.062588 ipyvizzu-story-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-11 05:25:47.062588 ipyvizzu-story-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-11 05:25:43.000000 ipyvizzu-story-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 05:25:47.062588 ipyvizzu-story-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-11 05:25:47.000000 ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-11 05:25:47.000000 ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:25:47.000000 ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 05:25:47.000000 ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 05:25:47.000000 ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/ipyvizzustory/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/ipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/ipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/ipy/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/pn/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/pn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/pn/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/py/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/py/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.058588 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/st/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/env/st/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.062588 ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:25:47.062588 ipyvizzu-story-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/tests/test_datafilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/tests/test_slide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/tests/test_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19436 2023-05-11 05:25:34.000000 ipyvizzu-story-0.7.0/tests/test_storylib.py
```

### Comparing `ipyvizzu-story-0.6.0/LICENSE` & `ipyvizzu-story-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/PKG-INFO` & `ipyvizzu-story-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,16 @@
-Metadata-Version: 2.1
-Name: ipyvizzu-story
-Version: 0.6.0
-Summary: Build, present and share animated data stories in Jupyter Notebook and similar environments.
-Home-page: https://github.com/vizzuhq/ipyvizzu-story
-License: Apache 2
-Project-URL: Documentation, https://ipyvizzu-story.vizzuhq.com
-Project-URL: Source, https://github.com/vizzuhq/ipyvizzu-story
-Project-URL: Tracker, https://github.com/vizzuhq/ipyvizzu-story/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: jupyter
-Provides-Extra: streamlit
-Provides-Extra: panel
-License-File: LICENSE
-
 <p align="center">
-  <a href="https://ipyvizzu-story.vizzuhq.com/0.6/">
-    <img src="https://ipyvizzu-story.vizzuhq.com/0.6/assets/ipyvizzu-story.gif" alt="ipyvizzu-story" />
+  <a href="https://ipyvizzu-story.vizzuhq.com/0.7/">
+    <img src="https://ipyvizzu-story.vizzuhq.com/0.7/assets/ipyvizzu-story.gif" alt="ipyvizzu-story" />
   </a>
   <p align="center"><b>ipyvizzu-story</b> - Build, present and share animated data stories in Jupyter Notebook and similar environments</p>
   <p align="center">
-    <a href="https://ipyvizzu-story.vizzuhq.com/0.6/">Documentation</a>
-    · <a href="https://ipyvizzu-story.vizzuhq.com/0.6/examples/">Examples</a>
-    · <a href="https://ipyvizzu-story.vizzuhq.com/0.6/reference/ipyvizzustory/">Code reference</a>
+    <a href="https://ipyvizzu-story.vizzuhq.com/0.7/">Documentation</a>
+    · <a href="https://ipyvizzu-story.vizzuhq.com/0.7/examples/">Examples</a>
+    · <a href="https://ipyvizzu-story.vizzuhq.com/0.7/reference/ipyvizzustory/">Code reference</a>
     · <a href="https://github.com/vizzuhq/ipyvizzu-story">Repository</a>
   </p>
 </p>
 
 [![PyPI version](https://badge.fury.io/py/ipyvizzu-story.svg)](https://badge.fury.io/py/ipyvizzu-story)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ipyvizzu-story.svg)](https://anaconda.org/conda-forge/ipyvizzu-story)
 [![CI-CD](https://github.com/vizzuhq/ipyvizzu-story/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/vizzuhq/ipyvizzu-story/actions/workflows/cicd.yml)
@@ -51,27 +31,27 @@
 ## Installation
 
 ```sh
 pip install ipyvizzu-story
 ```
 
 Visit
-[Installation chapter](https://ipyvizzu-story.vizzuhq.com/0.6/installation)
+[Installation chapter](https://ipyvizzu-story.vizzuhq.com/0.7/installation)
 for more options and details.
 
 ## Usage
 
 You can check and download the code behind the animation on the top of the page
 in our
-[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/usbudget/).
+[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/usbudget/).
 
 You can create the story below with the following code snippet.
 
 <p align="center">
-  <img src="https://ipyvizzu-story.vizzuhq.com/0.6/assets/readme-example.gif" alt="ipyvizzu-story" />
+  <img src="https://ipyvizzu-story.vizzuhq.com/0.7/assets/readme-example.gif" alt="ipyvizzu-story" />
 </p>
 
 ```python
 from ipyvizzu import Data, Config
 from ipyvizzustory import Story, Slide, Step
 
 data = Data()
@@ -96,59 +76,59 @@
 story.add_slide(slide2)
 
 story.play()
 ```
 
 ## Documentation
 
-Visit our [Documentation site](https://ipyvizzu-story.vizzuhq.com/0.6/) for
+Visit our [Documentation site](https://ipyvizzu-story.vizzuhq.com/0.7/) for
 more details and a step-by-step tutorial into `ipyvizzu-story` or check out our
-[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/).
+[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/).
 
 ## Environments
 
 `ipyvizzu-story` can be used in a wide variety of environments, visit
-[Environments chapter](https://ipyvizzu-story.vizzuhq.com/0.6/environments/)
+[Environments chapter](https://ipyvizzu-story.vizzuhq.com/0.7/environments/)
 for more details.
 
 - Notebooks
-  - [Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyternotebook/)
-  - [Colab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/colab/)
-  - [Databricks](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/databricks/)
-  - [DataCamp](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/datacamp/)
-  - [Deepnote](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/deepnote/)
-  - [JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyterlab/)
-  - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyterlite/)
-  - [Kaggle](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/kaggle/)
-  - [Noteable](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/noteable/)
+  - [Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyternotebook/)
+  - [Colab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/colab/)
+  - [Databricks](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/databricks/)
+  - [DataCamp](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/datacamp/)
+  - [Deepnote](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/deepnote/)
+  - [JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyterlab/)
+  - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyterlite/)
+  - [Kaggle](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/kaggle/)
+  - [Noteable](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/noteable/)
 - App platforms
-  - [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/streamlit/)
-  - [Flask](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/flask/)
-  - [Panel](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/panel/)
-  - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/mercury/)
-  - [Voilà](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/voila/)
+  - [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/streamlit/)
+  - [Flask](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/flask/)
+  - [Panel](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/panel/)
+  - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/mercury/)
+  - [Voilà](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/voila/)
 - BI tools
-  - [Mode](https://ipyvizzu-story.vizzuhq.com/0.6/environments/bi/mode/)
+  - [Mode](https://ipyvizzu-story.vizzuhq.com/0.7/environments/bi/mode/)
 - IDEs
-  - [PyCharm](https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/pycharm/)
-  - [VSCode Python](https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/vscode/)
-- [Python](https://ipyvizzu-story.vizzuhq.com/0.6/environments/python/)
+  - [PyCharm](https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/pycharm/)
+  - [VSCode Python](https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/vscode/)
+- [Python](https://ipyvizzu-story.vizzuhq.com/0.7/environments/python/)
 
 ## Contributing
 
 We welcome contributions to the project, visit our
-[Contributing guide](https://ipyvizzu-story.vizzuhq.com/0.6/CONTRIBUTING) for
+[Contributing guide](https://ipyvizzu-story.vizzuhq.com/0.7/CONTRIBUTING) for
 further info.
 
 ## Contact
 
 - Join our Slack if you have any questions or comments:
   [vizzu-community.slack.com](https://join.slack.com/t/vizzu-community/shared_invite/zt-w2nqhq44-2CCWL4o7qn2Ns1EFSf9kEg)
 - Drop us a line at hello@vizzuhq.com
 - Follow us on Twitter: [VizzuHQ](https://twitter.com/VizzuHQ)
 
 ## License
 
 Copyright © 2022-2023 [Vizzu Inc](https://vizzuhq.com).
 
 Released under the
-[Apache 2.0 License](https://ipyvizzu-story.vizzuhq.com/0.6/LICENSE).
+[Apache 2.0 License](https://ipyvizzu-story.vizzuhq.com/0.7/LICENSE).
```

#### html2text {}

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1 Name: ipyvizzu-story Version: 0.6.0 Summary: Build,
-present and share animated data stories in Jupyter Notebook and similar
-environments. Home-page: https://github.com/vizzuhq/ipyvizzu-story License:
-Apache 2 Project-URL: Documentation, https://ipyvizzu-story.vizzuhq.com
-Project-URL: Source, https://github.com/vizzuhq/ipyvizzu-story Project-URL:
-Tracker, https://github.com/vizzuhq/ipyvizzu-story/issues Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console Requires-Python: >=3.6 Description-Content-
-Type: text/markdown Provides-Extra: jupyter Provides-Extra: streamlit Provides-
-Extra: panel License-File: LICENSE
                                [ipyvizzu-story]
   ipyvizzu-story - Build, present and share animated data stories in Jupyter
                        Notebook and similar environments
            Documentation Â· Examples Â· Code_reference Â· Repository
 [![PyPI version](https://badge.fury.io/py/ipyvizzu-story.svg)](https://
 badge.fury.io/py/ipyvizzu-story) [![Conda Version](https://img.shields.io/
 conda/vn/conda-forge/ipyvizzu-story.svg)](https://anaconda.org/conda-forge/
@@ -24,53 +13,53 @@
 interactive data presentations within the data science notebook of their choice
 and to share them as an `HTML` file. The extension provides a widget that
 contains the presentation and adds controls for navigating between slides -
 predefined stages within the story being presented. Navigation also works with
 keyboard shortcuts - arrow keys, `PgUp`, `PgDn`, `Home`, `End` - and you can
 also use a clicker to switch between the slides. ## Installation ```sh pip
 install ipyvizzu-story ``` Visit [Installation chapter](https://ipyvizzu-
-story.vizzuhq.com/0.6/installation) for more options and details. ## Usage You
+story.vizzuhq.com/0.7/installation) for more options and details. ## Usage You
 can check and download the code behind the animation on the top of the page in
-our [Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/usbudget/
+our [Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/usbudget/
 ). You can create the story below with the following code snippet.
                                [ipyvizzu-story]
 ```python from ipyvizzu import Data, Config from ipyvizzustory import Story,
 Slide, Step data = Data() data.add_series("Foo", ["Alice", "Bob", "Ted"])
 data.add_series("Bar", [15, 32, 12]) data.add_series("Baz", [5, 3, 2]) story =
 Story(data=data) slide1 = Slide( Step( Config({"x": "Foo", "y": "Bar"}), ) )
 story.add_slide(slide1) slide2 = Slide( Step( Config({"color": "Foo", "x":
 "Baz", "geometry": "circle"}), ) ) story.add_slide(slide2) story.play() ``` ##
 Documentation Visit our [Documentation site](https://ipyvizzu-
-story.vizzuhq.com/0.6/) for more details and a step-by-step tutorial into
+story.vizzuhq.com/0.7/) for more details and a step-by-step tutorial into
 `ipyvizzu-story` or check out our [Example gallery](https://ipyvizzu-
-story.vizzuhq.com/0.6/examples/). ## Environments `ipyvizzu-story` can be used
+story.vizzuhq.com/0.7/examples/). ## Environments `ipyvizzu-story` can be used
 in a wide variety of environments, visit [Environments chapter](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/) for more details. - Notebooks -
-[Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-notebook/jupyternotebook/) - [Colab](https://ipyvizzu-story.vizzuhq.com/0.6/
+ipyvizzu-story.vizzuhq.com/0.7/environments/) for more details. - Notebooks -
+[Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+notebook/jupyternotebook/) - [Colab](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/notebook/colab/) - [Databricks](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/notebook/databricks/) - [DataCamp](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/datacamp/) - [Deepnote]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/deepnote/) -
-[JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/
-jupyterlab/) - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.6/
+story.vizzuhq.com/0.7/environments/notebook/databricks/) - [DataCamp](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/datacamp/) - [Deepnote]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/deepnote/) -
+[JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/
+jupyterlab/) - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/notebook/jupyterlite/) - [Kaggle](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/notebook/kaggle/) - [Noteable](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/noteable/) - App platforms
-- [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/
-streamlit/) - [Flask](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-platform/flask/) - [Panel](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-platform/panel/) - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.6/
+story.vizzuhq.com/0.7/environments/notebook/kaggle/) - [Noteable](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/noteable/) - App platforms
+- [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/
+streamlit/) - [Flask](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+platform/flask/) - [Panel](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+platform/panel/) - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/platform/mercury/) - [VoilÃ ](https://ipyvizzu-story.vizzuhq.com/
-0.6/environments/platform/voila/) - BI tools - [Mode](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/bi/mode/) - IDEs - [PyCharm](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/ide/pycharm/) - [VSCode Python]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/vscode/) - [Python]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/python/) ## Contributing
+0.7/environments/platform/voila/) - BI tools - [Mode](https://ipyvizzu-
+story.vizzuhq.com/0.7/environments/bi/mode/) - IDEs - [PyCharm](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/ide/pycharm/) - [VSCode Python]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/vscode/) - [Python]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/python/) ## Contributing
 We welcome contributions to the project, visit our [Contributing guide](https:/
-/ipyvizzu-story.vizzuhq.com/0.6/CONTRIBUTING) for further info. ## Contact -
+/ipyvizzu-story.vizzuhq.com/0.7/CONTRIBUTING) for further info. ## Contact -
 Join our Slack if you have any questions or comments: [vizzu-
 community.slack.com](https://join.slack.com/t/vizzu-community/shared_invite/zt-
 w2nqhq44-2CCWL4o7qn2Ns1EFSf9kEg) - Drop us a line at hello@vizzuhq.com - Follow
 us on Twitter: [VizzuHQ](https://twitter.com/VizzuHQ) ## License Copyright Â©
 2022-2023 [Vizzu Inc](https://vizzuhq.com). Released under the [Apache 2.0
-License](https://ipyvizzu-story.vizzuhq.com/0.6/LICENSE).
+License](https://ipyvizzu-story.vizzuhq.com/0.7/LICENSE).
```

### Comparing `ipyvizzu-story-0.6.0/README.md` & `ipyvizzu-story-0.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,36 @@
+Metadata-Version: 2.1
+Name: ipyvizzu-story
+Version: 0.7.0
+Summary: Build, present and share animated data stories in Jupyter Notebook and similar environments.
+Home-page: https://github.com/vizzuhq/ipyvizzu-story
+License: Apache 2
+Project-URL: Documentation, https://ipyvizzu-story.vizzuhq.com
+Project-URL: Source, https://github.com/vizzuhq/ipyvizzu-story
+Project-URL: Tracker, https://github.com/vizzuhq/ipyvizzu-story/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: jupyter
+Provides-Extra: streamlit
+Provides-Extra: panel
+License-File: LICENSE
+
 <p align="center">
-  <a href="https://ipyvizzu-story.vizzuhq.com/0.6/">
-    <img src="https://ipyvizzu-story.vizzuhq.com/0.6/assets/ipyvizzu-story.gif" alt="ipyvizzu-story" />
+  <a href="https://ipyvizzu-story.vizzuhq.com/0.7/">
+    <img src="https://ipyvizzu-story.vizzuhq.com/0.7/assets/ipyvizzu-story.gif" alt="ipyvizzu-story" />
   </a>
   <p align="center"><b>ipyvizzu-story</b> - Build, present and share animated data stories in Jupyter Notebook and similar environments</p>
   <p align="center">
-    <a href="https://ipyvizzu-story.vizzuhq.com/0.6/">Documentation</a>
-    · <a href="https://ipyvizzu-story.vizzuhq.com/0.6/examples/">Examples</a>
-    · <a href="https://ipyvizzu-story.vizzuhq.com/0.6/reference/ipyvizzustory/">Code reference</a>
+    <a href="https://ipyvizzu-story.vizzuhq.com/0.7/">Documentation</a>
+    · <a href="https://ipyvizzu-story.vizzuhq.com/0.7/examples/">Examples</a>
+    · <a href="https://ipyvizzu-story.vizzuhq.com/0.7/reference/ipyvizzustory/">Code reference</a>
     · <a href="https://github.com/vizzuhq/ipyvizzu-story">Repository</a>
   </p>
 </p>
 
 [![PyPI version](https://badge.fury.io/py/ipyvizzu-story.svg)](https://badge.fury.io/py/ipyvizzu-story)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ipyvizzu-story.svg)](https://anaconda.org/conda-forge/ipyvizzu-story)
 [![CI-CD](https://github.com/vizzuhq/ipyvizzu-story/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/vizzuhq/ipyvizzu-story/actions/workflows/cicd.yml)
@@ -31,27 +51,27 @@
 ## Installation
 
 ```sh
 pip install ipyvizzu-story
 ```
 
 Visit
-[Installation chapter](https://ipyvizzu-story.vizzuhq.com/0.6/installation)
+[Installation chapter](https://ipyvizzu-story.vizzuhq.com/0.7/installation)
 for more options and details.
 
 ## Usage
 
 You can check and download the code behind the animation on the top of the page
 in our
-[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/usbudget/).
+[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/usbudget/).
 
 You can create the story below with the following code snippet.
 
 <p align="center">
-  <img src="https://ipyvizzu-story.vizzuhq.com/0.6/assets/readme-example.gif" alt="ipyvizzu-story" />
+  <img src="https://ipyvizzu-story.vizzuhq.com/0.7/assets/readme-example.gif" alt="ipyvizzu-story" />
 </p>
 
 ```python
 from ipyvizzu import Data, Config
 from ipyvizzustory import Story, Slide, Step
 
 data = Data()
@@ -76,59 +96,59 @@
 story.add_slide(slide2)
 
 story.play()
 ```
 
 ## Documentation
 
-Visit our [Documentation site](https://ipyvizzu-story.vizzuhq.com/0.6/) for
+Visit our [Documentation site](https://ipyvizzu-story.vizzuhq.com/0.7/) for
 more details and a step-by-step tutorial into `ipyvizzu-story` or check out our
-[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/).
+[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/).
 
 ## Environments
 
 `ipyvizzu-story` can be used in a wide variety of environments, visit
-[Environments chapter](https://ipyvizzu-story.vizzuhq.com/0.6/environments/)
+[Environments chapter](https://ipyvizzu-story.vizzuhq.com/0.7/environments/)
 for more details.
 
 - Notebooks
-  - [Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyternotebook/)
-  - [Colab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/colab/)
-  - [Databricks](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/databricks/)
-  - [DataCamp](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/datacamp/)
-  - [Deepnote](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/deepnote/)
-  - [JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyterlab/)
-  - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyterlite/)
-  - [Kaggle](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/kaggle/)
-  - [Noteable](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/noteable/)
+  - [Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyternotebook/)
+  - [Colab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/colab/)
+  - [Databricks](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/databricks/)
+  - [DataCamp](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/datacamp/)
+  - [Deepnote](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/deepnote/)
+  - [JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyterlab/)
+  - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyterlite/)
+  - [Kaggle](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/kaggle/)
+  - [Noteable](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/noteable/)
 - App platforms
-  - [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/streamlit/)
-  - [Flask](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/flask/)
-  - [Panel](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/panel/)
-  - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/mercury/)
-  - [Voilà](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/voila/)
+  - [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/streamlit/)
+  - [Flask](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/flask/)
+  - [Panel](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/panel/)
+  - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/mercury/)
+  - [Voilà](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/voila/)
 - BI tools
-  - [Mode](https://ipyvizzu-story.vizzuhq.com/0.6/environments/bi/mode/)
+  - [Mode](https://ipyvizzu-story.vizzuhq.com/0.7/environments/bi/mode/)
 - IDEs
-  - [PyCharm](https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/pycharm/)
-  - [VSCode Python](https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/vscode/)
-- [Python](https://ipyvizzu-story.vizzuhq.com/0.6/environments/python/)
+  - [PyCharm](https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/pycharm/)
+  - [VSCode Python](https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/vscode/)
+- [Python](https://ipyvizzu-story.vizzuhq.com/0.7/environments/python/)
 
 ## Contributing
 
 We welcome contributions to the project, visit our
-[Contributing guide](https://ipyvizzu-story.vizzuhq.com/0.6/CONTRIBUTING) for
+[Contributing guide](https://ipyvizzu-story.vizzuhq.com/0.7/CONTRIBUTING) for
 further info.
 
 ## Contact
 
 - Join our Slack if you have any questions or comments:
   [vizzu-community.slack.com](https://join.slack.com/t/vizzu-community/shared_invite/zt-w2nqhq44-2CCWL4o7qn2Ns1EFSf9kEg)
 - Drop us a line at hello@vizzuhq.com
 - Follow us on Twitter: [VizzuHQ](https://twitter.com/VizzuHQ)
 
 ## License
 
 Copyright © 2022-2023 [Vizzu Inc](https://vizzuhq.com).
 
 Released under the
-[Apache 2.0 License](https://ipyvizzu-story.vizzuhq.com/0.6/LICENSE).
+[Apache 2.0 License](https://ipyvizzu-story.vizzuhq.com/0.7/LICENSE).
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: ipyvizzu-story Version: 0.7.0 Summary: Build,
+present and share animated data stories in Jupyter Notebook and similar
+environments. Home-page: https://github.com/vizzuhq/ipyvizzu-story License:
+Apache 2 Project-URL: Documentation, https://ipyvizzu-story.vizzuhq.com
+Project-URL: Source, https://github.com/vizzuhq/ipyvizzu-story Project-URL:
+Tracker, https://github.com/vizzuhq/ipyvizzu-story/issues Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console Requires-Python: >=3.6 Description-Content-
+Type: text/markdown Provides-Extra: jupyter Provides-Extra: streamlit Provides-
+Extra: panel License-File: LICENSE
                                [ipyvizzu-story]
   ipyvizzu-story - Build, present and share animated data stories in Jupyter
                        Notebook and similar environments
            Documentation Â· Examples Â· Code_reference Â· Repository
 [![PyPI version](https://badge.fury.io/py/ipyvizzu-story.svg)](https://
 badge.fury.io/py/ipyvizzu-story) [![Conda Version](https://img.shields.io/
 conda/vn/conda-forge/ipyvizzu-story.svg)](https://anaconda.org/conda-forge/
@@ -13,53 +24,53 @@
 interactive data presentations within the data science notebook of their choice
 and to share them as an `HTML` file. The extension provides a widget that
 contains the presentation and adds controls for navigating between slides -
 predefined stages within the story being presented. Navigation also works with
 keyboard shortcuts - arrow keys, `PgUp`, `PgDn`, `Home`, `End` - and you can
 also use a clicker to switch between the slides. ## Installation ```sh pip
 install ipyvizzu-story ``` Visit [Installation chapter](https://ipyvizzu-
-story.vizzuhq.com/0.6/installation) for more options and details. ## Usage You
+story.vizzuhq.com/0.7/installation) for more options and details. ## Usage You
 can check and download the code behind the animation on the top of the page in
-our [Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/usbudget/
+our [Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/usbudget/
 ). You can create the story below with the following code snippet.
                                [ipyvizzu-story]
 ```python from ipyvizzu import Data, Config from ipyvizzustory import Story,
 Slide, Step data = Data() data.add_series("Foo", ["Alice", "Bob", "Ted"])
 data.add_series("Bar", [15, 32, 12]) data.add_series("Baz", [5, 3, 2]) story =
 Story(data=data) slide1 = Slide( Step( Config({"x": "Foo", "y": "Bar"}), ) )
 story.add_slide(slide1) slide2 = Slide( Step( Config({"color": "Foo", "x":
 "Baz", "geometry": "circle"}), ) ) story.add_slide(slide2) story.play() ``` ##
 Documentation Visit our [Documentation site](https://ipyvizzu-
-story.vizzuhq.com/0.6/) for more details and a step-by-step tutorial into
+story.vizzuhq.com/0.7/) for more details and a step-by-step tutorial into
 `ipyvizzu-story` or check out our [Example gallery](https://ipyvizzu-
-story.vizzuhq.com/0.6/examples/). ## Environments `ipyvizzu-story` can be used
+story.vizzuhq.com/0.7/examples/). ## Environments `ipyvizzu-story` can be used
 in a wide variety of environments, visit [Environments chapter](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/) for more details. - Notebooks -
-[Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-notebook/jupyternotebook/) - [Colab](https://ipyvizzu-story.vizzuhq.com/0.6/
+ipyvizzu-story.vizzuhq.com/0.7/environments/) for more details. - Notebooks -
+[Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+notebook/jupyternotebook/) - [Colab](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/notebook/colab/) - [Databricks](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/notebook/databricks/) - [DataCamp](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/datacamp/) - [Deepnote]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/deepnote/) -
-[JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/
-jupyterlab/) - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.6/
+story.vizzuhq.com/0.7/environments/notebook/databricks/) - [DataCamp](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/datacamp/) - [Deepnote]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/deepnote/) -
+[JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/
+jupyterlab/) - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/notebook/jupyterlite/) - [Kaggle](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/notebook/kaggle/) - [Noteable](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/noteable/) - App platforms
-- [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/
-streamlit/) - [Flask](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-platform/flask/) - [Panel](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-platform/panel/) - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.6/
+story.vizzuhq.com/0.7/environments/notebook/kaggle/) - [Noteable](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/noteable/) - App platforms
+- [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/
+streamlit/) - [Flask](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+platform/flask/) - [Panel](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+platform/panel/) - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/platform/mercury/) - [VoilÃ ](https://ipyvizzu-story.vizzuhq.com/
-0.6/environments/platform/voila/) - BI tools - [Mode](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/bi/mode/) - IDEs - [PyCharm](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/ide/pycharm/) - [VSCode Python]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/vscode/) - [Python]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/python/) ## Contributing
+0.7/environments/platform/voila/) - BI tools - [Mode](https://ipyvizzu-
+story.vizzuhq.com/0.7/environments/bi/mode/) - IDEs - [PyCharm](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/ide/pycharm/) - [VSCode Python]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/vscode/) - [Python]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/python/) ## Contributing
 We welcome contributions to the project, visit our [Contributing guide](https:/
-/ipyvizzu-story.vizzuhq.com/0.6/CONTRIBUTING) for further info. ## Contact -
+/ipyvizzu-story.vizzuhq.com/0.7/CONTRIBUTING) for further info. ## Contact -
 Join our Slack if you have any questions or comments: [vizzu-
 community.slack.com](https://join.slack.com/t/vizzu-community/shared_invite/zt-
 w2nqhq44-2CCWL4o7qn2Ns1EFSf9kEg) - Drop us a line at hello@vizzuhq.com - Follow
 us on Twitter: [VizzuHQ](https://twitter.com/VizzuHQ) ## License Copyright Â©
 2022-2023 [Vizzu Inc](https://vizzuhq.com). Released under the [Apache 2.0
-License](https://ipyvizzu-story.vizzuhq.com/0.6/LICENSE).
+License](https://ipyvizzu-story.vizzuhq.com/0.7/LICENSE).
```

### Comparing `ipyvizzu-story-0.6.0/setup.py` & `ipyvizzu-story-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 with open("README.md", encoding="utf8") as fp:
     long_description = fp.read()
 
 packages = find_packages(where="src", exclude=["__pycache__"])
 
 setup(
     name="ipyvizzu-story",
-    version="0.6.0",
+    version="0.7.0",
     description=(
         "Build, present and share animated data stories in Jupyter Notebook and similar environments."  # pylint: disable=line-too-long
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=packages,
```

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/PKG-INFO` & `ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvizzu-story
-Version: 0.6.0
+Version: 0.7.0
 Summary: Build, present and share animated data stories in Jupyter Notebook and similar environments.
 Home-page: https://github.com/vizzuhq/ipyvizzu-story
 License: Apache 2
 Project-URL: Documentation, https://ipyvizzu-story.vizzuhq.com
 Project-URL: Source, https://github.com/vizzuhq/ipyvizzu-story
 Project-URL: Tracker, https://github.com/vizzuhq/ipyvizzu-story/issues
 Classifier: Programming Language :: Python :: 3
@@ -15,22 +15,22 @@
 Description-Content-Type: text/markdown
 Provides-Extra: jupyter
 Provides-Extra: streamlit
 Provides-Extra: panel
 License-File: LICENSE
 
 <p align="center">
-  <a href="https://ipyvizzu-story.vizzuhq.com/0.6/">
-    <img src="https://ipyvizzu-story.vizzuhq.com/0.6/assets/ipyvizzu-story.gif" alt="ipyvizzu-story" />
+  <a href="https://ipyvizzu-story.vizzuhq.com/0.7/">
+    <img src="https://ipyvizzu-story.vizzuhq.com/0.7/assets/ipyvizzu-story.gif" alt="ipyvizzu-story" />
   </a>
   <p align="center"><b>ipyvizzu-story</b> - Build, present and share animated data stories in Jupyter Notebook and similar environments</p>
   <p align="center">
-    <a href="https://ipyvizzu-story.vizzuhq.com/0.6/">Documentation</a>
-    · <a href="https://ipyvizzu-story.vizzuhq.com/0.6/examples/">Examples</a>
-    · <a href="https://ipyvizzu-story.vizzuhq.com/0.6/reference/ipyvizzustory/">Code reference</a>
+    <a href="https://ipyvizzu-story.vizzuhq.com/0.7/">Documentation</a>
+    · <a href="https://ipyvizzu-story.vizzuhq.com/0.7/examples/">Examples</a>
+    · <a href="https://ipyvizzu-story.vizzuhq.com/0.7/reference/ipyvizzustory/">Code reference</a>
     · <a href="https://github.com/vizzuhq/ipyvizzu-story">Repository</a>
   </p>
 </p>
 
 [![PyPI version](https://badge.fury.io/py/ipyvizzu-story.svg)](https://badge.fury.io/py/ipyvizzu-story)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ipyvizzu-story.svg)](https://anaconda.org/conda-forge/ipyvizzu-story)
 [![CI-CD](https://github.com/vizzuhq/ipyvizzu-story/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/vizzuhq/ipyvizzu-story/actions/workflows/cicd.yml)
@@ -51,27 +51,27 @@
 ## Installation
 
 ```sh
 pip install ipyvizzu-story
 ```
 
 Visit
-[Installation chapter](https://ipyvizzu-story.vizzuhq.com/0.6/installation)
+[Installation chapter](https://ipyvizzu-story.vizzuhq.com/0.7/installation)
 for more options and details.
 
 ## Usage
 
 You can check and download the code behind the animation on the top of the page
 in our
-[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/usbudget/).
+[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/usbudget/).
 
 You can create the story below with the following code snippet.
 
 <p align="center">
-  <img src="https://ipyvizzu-story.vizzuhq.com/0.6/assets/readme-example.gif" alt="ipyvizzu-story" />
+  <img src="https://ipyvizzu-story.vizzuhq.com/0.7/assets/readme-example.gif" alt="ipyvizzu-story" />
 </p>
 
 ```python
 from ipyvizzu import Data, Config
 from ipyvizzustory import Story, Slide, Step
 
 data = Data()
@@ -96,59 +96,59 @@
 story.add_slide(slide2)
 
 story.play()
 ```
 
 ## Documentation
 
-Visit our [Documentation site](https://ipyvizzu-story.vizzuhq.com/0.6/) for
+Visit our [Documentation site](https://ipyvizzu-story.vizzuhq.com/0.7/) for
 more details and a step-by-step tutorial into `ipyvizzu-story` or check out our
-[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/).
+[Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/).
 
 ## Environments
 
 `ipyvizzu-story` can be used in a wide variety of environments, visit
-[Environments chapter](https://ipyvizzu-story.vizzuhq.com/0.6/environments/)
+[Environments chapter](https://ipyvizzu-story.vizzuhq.com/0.7/environments/)
 for more details.
 
 - Notebooks
-  - [Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyternotebook/)
-  - [Colab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/colab/)
-  - [Databricks](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/databricks/)
-  - [DataCamp](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/datacamp/)
-  - [Deepnote](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/deepnote/)
-  - [JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyterlab/)
-  - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/jupyterlite/)
-  - [Kaggle](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/kaggle/)
-  - [Noteable](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/noteable/)
+  - [Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyternotebook/)
+  - [Colab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/colab/)
+  - [Databricks](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/databricks/)
+  - [DataCamp](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/datacamp/)
+  - [Deepnote](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/deepnote/)
+  - [JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyterlab/)
+  - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/jupyterlite/)
+  - [Kaggle](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/kaggle/)
+  - [Noteable](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/noteable/)
 - App platforms
-  - [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/streamlit/)
-  - [Flask](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/flask/)
-  - [Panel](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/panel/)
-  - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/mercury/)
-  - [Voilà](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/voila/)
+  - [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/streamlit/)
+  - [Flask](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/flask/)
+  - [Panel](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/panel/)
+  - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/mercury/)
+  - [Voilà](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/voila/)
 - BI tools
-  - [Mode](https://ipyvizzu-story.vizzuhq.com/0.6/environments/bi/mode/)
+  - [Mode](https://ipyvizzu-story.vizzuhq.com/0.7/environments/bi/mode/)
 - IDEs
-  - [PyCharm](https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/pycharm/)
-  - [VSCode Python](https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/vscode/)
-- [Python](https://ipyvizzu-story.vizzuhq.com/0.6/environments/python/)
+  - [PyCharm](https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/pycharm/)
+  - [VSCode Python](https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/vscode/)
+- [Python](https://ipyvizzu-story.vizzuhq.com/0.7/environments/python/)
 
 ## Contributing
 
 We welcome contributions to the project, visit our
-[Contributing guide](https://ipyvizzu-story.vizzuhq.com/0.6/CONTRIBUTING) for
+[Contributing guide](https://ipyvizzu-story.vizzuhq.com/0.7/CONTRIBUTING) for
 further info.
 
 ## Contact
 
 - Join our Slack if you have any questions or comments:
   [vizzu-community.slack.com](https://join.slack.com/t/vizzu-community/shared_invite/zt-w2nqhq44-2CCWL4o7qn2Ns1EFSf9kEg)
 - Drop us a line at hello@vizzuhq.com
 - Follow us on Twitter: [VizzuHQ](https://twitter.com/VizzuHQ)
 
 ## License
 
 Copyright © 2022-2023 [Vizzu Inc](https://vizzuhq.com).
 
 Released under the
-[Apache 2.0 License](https://ipyvizzu-story.vizzuhq.com/0.6/LICENSE).
+[Apache 2.0 License](https://ipyvizzu-story.vizzuhq.com/0.7/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ipyvizzu-story Version: 0.6.0 Summary: Build,
+Metadata-Version: 2.1 Name: ipyvizzu-story Version: 0.7.0 Summary: Build,
 present and share animated data stories in Jupyter Notebook and similar
 environments. Home-page: https://github.com/vizzuhq/ipyvizzu-story License:
 Apache 2 Project-URL: Documentation, https://ipyvizzu-story.vizzuhq.com
 Project-URL: Source, https://github.com/vizzuhq/ipyvizzu-story Project-URL:
 Tracker, https://github.com/vizzuhq/ipyvizzu-story/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
@@ -24,53 +24,53 @@
 interactive data presentations within the data science notebook of their choice
 and to share them as an `HTML` file. The extension provides a widget that
 contains the presentation and adds controls for navigating between slides -
 predefined stages within the story being presented. Navigation also works with
 keyboard shortcuts - arrow keys, `PgUp`, `PgDn`, `Home`, `End` - and you can
 also use a clicker to switch between the slides. ## Installation ```sh pip
 install ipyvizzu-story ``` Visit [Installation chapter](https://ipyvizzu-
-story.vizzuhq.com/0.6/installation) for more options and details. ## Usage You
+story.vizzuhq.com/0.7/installation) for more options and details. ## Usage You
 can check and download the code behind the animation on the top of the page in
-our [Example gallery](https://ipyvizzu-story.vizzuhq.com/0.6/examples/usbudget/
+our [Example gallery](https://ipyvizzu-story.vizzuhq.com/0.7/examples/usbudget/
 ). You can create the story below with the following code snippet.
                                [ipyvizzu-story]
 ```python from ipyvizzu import Data, Config from ipyvizzustory import Story,
 Slide, Step data = Data() data.add_series("Foo", ["Alice", "Bob", "Ted"])
 data.add_series("Bar", [15, 32, 12]) data.add_series("Baz", [5, 3, 2]) story =
 Story(data=data) slide1 = Slide( Step( Config({"x": "Foo", "y": "Bar"}), ) )
 story.add_slide(slide1) slide2 = Slide( Step( Config({"color": "Foo", "x":
 "Baz", "geometry": "circle"}), ) ) story.add_slide(slide2) story.play() ``` ##
 Documentation Visit our [Documentation site](https://ipyvizzu-
-story.vizzuhq.com/0.6/) for more details and a step-by-step tutorial into
+story.vizzuhq.com/0.7/) for more details and a step-by-step tutorial into
 `ipyvizzu-story` or check out our [Example gallery](https://ipyvizzu-
-story.vizzuhq.com/0.6/examples/). ## Environments `ipyvizzu-story` can be used
+story.vizzuhq.com/0.7/examples/). ## Environments `ipyvizzu-story` can be used
 in a wide variety of environments, visit [Environments chapter](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/) for more details. - Notebooks -
-[Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-notebook/jupyternotebook/) - [Colab](https://ipyvizzu-story.vizzuhq.com/0.6/
+ipyvizzu-story.vizzuhq.com/0.7/environments/) for more details. - Notebooks -
+[Jupyter Notebook](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+notebook/jupyternotebook/) - [Colab](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/notebook/colab/) - [Databricks](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/notebook/databricks/) - [DataCamp](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/datacamp/) - [Deepnote]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/deepnote/) -
-[JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/
-jupyterlab/) - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.6/
+story.vizzuhq.com/0.7/environments/notebook/databricks/) - [DataCamp](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/datacamp/) - [Deepnote]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/deepnote/) -
+[JupyterLab](https://ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/
+jupyterlab/) - [JupyterLite](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/notebook/jupyterlite/) - [Kaggle](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/notebook/kaggle/) - [Noteable](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/notebook/noteable/) - App platforms
-- [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.6/environments/platform/
-streamlit/) - [Flask](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-platform/flask/) - [Panel](https://ipyvizzu-story.vizzuhq.com/0.6/environments/
-platform/panel/) - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.6/
+story.vizzuhq.com/0.7/environments/notebook/kaggle/) - [Noteable](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/notebook/noteable/) - App platforms
+- [Streamlit](https://ipyvizzu-story.vizzuhq.com/0.7/environments/platform/
+streamlit/) - [Flask](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+platform/flask/) - [Panel](https://ipyvizzu-story.vizzuhq.com/0.7/environments/
+platform/panel/) - [Mercury/mljar](https://ipyvizzu-story.vizzuhq.com/0.7/
 environments/platform/mercury/) - [VoilÃ ](https://ipyvizzu-story.vizzuhq.com/
-0.6/environments/platform/voila/) - BI tools - [Mode](https://ipyvizzu-
-story.vizzuhq.com/0.6/environments/bi/mode/) - IDEs - [PyCharm](https://
-ipyvizzu-story.vizzuhq.com/0.6/environments/ide/pycharm/) - [VSCode Python]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/ide/vscode/) - [Python]
-(https://ipyvizzu-story.vizzuhq.com/0.6/environments/python/) ## Contributing
+0.7/environments/platform/voila/) - BI tools - [Mode](https://ipyvizzu-
+story.vizzuhq.com/0.7/environments/bi/mode/) - IDEs - [PyCharm](https://
+ipyvizzu-story.vizzuhq.com/0.7/environments/ide/pycharm/) - [VSCode Python]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/ide/vscode/) - [Python]
+(https://ipyvizzu-story.vizzuhq.com/0.7/environments/python/) ## Contributing
 We welcome contributions to the project, visit our [Contributing guide](https:/
-/ipyvizzu-story.vizzuhq.com/0.6/CONTRIBUTING) for further info. ## Contact -
+/ipyvizzu-story.vizzuhq.com/0.7/CONTRIBUTING) for further info. ## Contact -
 Join our Slack if you have any questions or comments: [vizzu-
 community.slack.com](https://join.slack.com/t/vizzu-community/shared_invite/zt-
 w2nqhq44-2CCWL4o7qn2Ns1EFSf9kEg) - Drop us a line at hello@vizzuhq.com - Follow
 us on Twitter: [VizzuHQ](https://twitter.com/VizzuHQ) ## License Copyright Â©
 2022-2023 [Vizzu Inc](https://vizzuhq.com). Released under the [Apache 2.0
-License](https://ipyvizzu-story.vizzuhq.com/0.6/LICENSE).
+License](https://ipyvizzu-story.vizzuhq.com/0.7/LICENSE).
```

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzu_story.egg-info/SOURCES.txt` & `ipyvizzu-story-0.7.0/src/ipyvizzu_story.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/__init__.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Build, present and share animated data stories in `Jupyter Notebook` and similar environments.
 
 `ipyvizzu-story` package consists of two main parts:
 
-* [Env][ipyvizzustory.env]: environment dependent modules
 * [Storylib][ipyvizzustory.storylib]: environment independent modules
+* [Env][ipyvizzustory.env]: environment dependent modules
 
 `ipyvizzu-story` package tries to figure out the environment and import the correct type of `Story`,
 however `Story` could be imported with full path.
 
 `ipyvizzu-story` package imports the following objects in `__init__.py`:
 
-* [Step][ipyvizzustory.storylib.story.Step] and
-  [Slide][ipyvizzustory.storylib.story.Slide]
+
 * `Story` from [Env.py.story][ipyvizzustory.env.py.story] or
     [Env.ipy.story][ipyvizzustory.env.ipy.story] or
     [Env.st.story][ipyvizzustory.env.st.story]
+* [Step][ipyvizzustory.storylib.story.Step]
+* [Slide][ipyvizzustory.storylib.story.Slide]
 """
 
 
 from .storylib.story import Step, Slide
 
 from .env.py.story import Story as PythonStory
 
@@ -56,9 +57,17 @@
             The appropriate `Story` for the environment.
     """  # pylint: disable=line-too-long
 
     return JupyterStory or StreamlitStory or PythonStory  # type: ignore
 
 
 Story = get_story()
+"""
+Available types:
+
+* [Jupyter/IPython Story][ipyvizzustory.env.ipy.story.Story]
+* [Streamlit Story][ipyvizzustory.env.st.story.Story]
+* [Panel Story][ipyvizzustory.env.pn.story.Story]
+* [Python Story][ipyvizzustory.env.py.story.Story]
+"""
 
-__all__ = ["Story", "Slide", "Step"]
+__all__ = ["get_story", "Story", "Slide", "Step"]
```

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/env/ipy/story.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/env/ipy/story.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/env/pn/story.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/env/pn/story.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/env/py/story.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/env/py/story.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/env/st/story.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/env/st/story.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/animation.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/animation.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/story.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/story.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,26 +22,22 @@
         self,
         *animations: Union[Data, Style, Config],
         **anim_options: Optional[Union[str, int, float, dict]],
     ):
         """
         Step constructor.
 
-        Note:
-            Do not set `anim_options` argument, it will raise `NotImplementedError` error.
-
         Args:
             *animations: List of [Data][ipyvizzu.Data],
                 [Config][ipyvizzu.Config] and [Style][ipyvizzu.Style] objects.
                 A `Step` can contain each of the above once.
             **anim_options: Animation options such as duration.
 
         Raises:
             ValueError: If `animations` are not set.
-            NotImplementedError: If `anim_options` are set.
 
         Example:
             Initialize a step with a [Config][ipyvizzu.Config] object:
 
                 step = Step(
                     Config({"x": "Foo", "y": "Bar"})
                 )
@@ -49,16 +45,15 @@
 
         super().__init__()
         if not animations:
             raise ValueError("No animation was set.")
         self._update(*animations)
 
         if anim_options:
-            # self["animOptions"] = PlainAnimation(**anim_options).build()
-            raise NotImplementedError("Anim options are not supported.")
+            self["animOptions"] = anim_options
 
     def _update(self, *animations: Union[Data, Style, Config]) -> None:
         for animation in animations:
             if not animation or type(animation) not in [
                 Data,
                 Style,
                 Config,
@@ -208,14 +203,16 @@
                 value_is_pixel = value[:-2].isnumeric()
         return value_is_pixel
 
 
 class Story(dict):
     """A class for representing a presentation story."""
 
+    # pylint: disable=too-many-instance-attributes
+
     def __init__(self, data: Data, style: Optional[Style] = None):
         """
         Presentation Story constructor.
 
         Args:
             data: Data set for the whole presentation story.
                 After initialization `data` can not be modified,
@@ -238,14 +235,15 @@
                 story = Story(data=data)
         """
 
         super().__init__()
 
         self._vizzu: Optional[str] = None
         self._vizzu_story: str = VIZZU_STORY
+        self._start_slide: Optional[int] = None
 
         self._size: StorySize = StorySize()
 
         self._features: List[str] = []
         self._events: List[str] = []
 
         if not data or type(data) != Data:  # pylint: disable=unidiomatic-typecheck
@@ -288,14 +286,29 @@
 
         return self._vizzu_story
 
     @vizzu_story.setter
     def vizzu_story(self, url: str) -> None:
         self._vizzu_story = url
 
+    @property
+    def start_slide(self) -> Optional[int]:
+        """
+        A property for setting the starter slide.
+
+        Returns:
+            Number of the starter slide.
+        """
+
+        return self._start_slide
+
+    @start_slide.setter
+    def start_slide(self, number: int) -> None:
+        self._start_slide = number
+
     def add_slide(self, slide: Slide) -> None:
         """
         A method for adding a slide for the story.
 
         Args:
             slide: The next slide of the story.
 
@@ -382,14 +395,17 @@
             The assembled `HTML` code as string.
         """
 
         vizzu_player_data = f"{json.dumps(self, cls=RawJavaScriptEncoder)}"
         return DISPLAY_TEMPLATE.format(
             id=uuid.uuid4().hex[:7],
             vizzu_attribute=f'vizzu-url="{self._vizzu}"' if self._vizzu else "",
+            start_slide=f'start-slide="{self._start_slide}"'
+            if self._start_slide
+            else "",
             vizzu_story=self._vizzu_story,
             vizzu_player_data=vizzu_player_data,
             chart_size=self._size.style,
             chart_features=f"\n{DISPLAY_INDENT * 3}".join(self._features),
             chart_events=f"\n{DISPLAY_INDENT * 3}".join(self._events),
         )
```

### Comparing `ipyvizzu-story-0.6.0/src/ipyvizzustory/storylib/template.py` & `ipyvizzu-story-0.7.0/src/ipyvizzustory/storylib/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """A module for storing the `HTML` templates."""
 
 
 VIZZU_STORY: str = (
-    "https://cdn.jsdelivr.net/npm/vizzu-story@0.3/dist/vizzu-story.min.js"
+    "https://cdn.jsdelivr.net/npm/vizzu-story@0.4/dist/vizzu-story.min.js"
 )
 """A variable for storing the default url of the `vizzu-story` package."""
 
 DISPLAY_INDENT: str = "    "
 """A variable for storing the default indent in the `HTML` template."""
 
 DISPLAY_TEMPLATE: str = """
 <div>
-    <vizzu-player id="{id}" {vizzu_attribute} controller></vizzu-player>
+    <vizzu-player id="{id}" {vizzu_attribute} {start_slide} controller></vizzu-player>
     <script type="module">
         import VizzuPlayer from "{vizzu_story}";
 
         const vp = document.getElementById("{id}");
         import(vp.vizzuUrl).then(vizzuLoaded => {{
             const lib = vizzuLoaded.default;
             const vizzuPlayerData = {vizzu_player_data};
```

### Comparing `ipyvizzu-story-0.6.0/tests/test_datafilter.py` & `ipyvizzu-story-0.7.0/tests/test_datafilter.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/tests/test_slide.py` & `ipyvizzu-story-0.7.0/tests/test_slide.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/tests/test_step.py` & `ipyvizzu-story-0.7.0/tests/test_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
             Step()
 
     def test_init_if_anim_option_was_set(self) -> None:
         """
         A method for testing Step.__init__ method if anim option was set.
 
         Raises:
-            AssertionError: If NotImplementedError is not occurred.
+            AssertionError: If the step dict is not correct.
         """
 
-        with self.assertRaises(NotImplementedError):
-            Step(Data.filter(None), duration=1)
+        self.assertEqual(
+            Step(Data.filter(None), duration=1),
+            {"filter": None, "animOptions": {"duration": 1}},
+        )
 
     def test_init_if_animation_was_data(self) -> None:
         """
         A method for testing Step.__init__ method if animation was data.
 
         Raises:
             AssertionError: If the step dict is not correct.
```

### Comparing `ipyvizzu-story-0.6.0/tests/test_story.py` & `ipyvizzu-story-0.7.0/tests/test_story.py`

 * *Files identical despite different names*

### Comparing `ipyvizzu-story-0.6.0/tests/test_storylib.py` & `ipyvizzu-story-0.7.0/tests/test_storylib.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         Returns:
             A test html output.
         """
 
         return DISPLAY_TEMPLATE.format(
             id="1234567",
             vizzu_attribute="",
+            start_slide="",
             vizzu_story=VIZZU_STORY,
             vizzu_player_data=self.get_vpd(),
             chart_size="",
             chart_features="",
             chart_events="",
         )
 
@@ -81,14 +82,15 @@
         Returns:
             A test html output.
         """
 
         return DISPLAY_TEMPLATE.format(
             id="1234567",
             vizzu_attribute="",
+            start_slide="",
             vizzu_story=VIZZU_STORY,
             vizzu_player_data=self.get_vpd(),
             chart_size="vp.style.cssText = 'width: 800px;height: 480px;'",
             chart_features="",
             chart_events="",
         )
 
@@ -269,14 +271,15 @@
             story = self.get_story()
             story.vizzu = vizzu
             self.assertEqual(
                 story.to_html(),
                 DISPLAY_TEMPLATE.format(
                     id="1234567",
                     vizzu_attribute=f'vizzu-url="{vizzu}"',
+                    start_slide="",
                     vizzu_story=VIZZU_STORY,
                     vizzu_player_data=self.get_vpd(),
                     chart_size="",
                     chart_features="",
                     chart_events="",
                 ),
             )
@@ -307,22 +310,62 @@
             story = self.get_story()
             story.vizzu_story = vizzu_story
             self.assertEqual(
                 story.to_html(),
                 DISPLAY_TEMPLATE.format(
                     id="1234567",
                     vizzu_attribute="",
+                    start_slide="",
                     vizzu_story=vizzu_story,
                     vizzu_player_data=self.get_vpd(),
                     chart_size="",
                     chart_features="",
                     chart_events="",
                 ),
             )
 
+    def test_start_slide_default(self) -> None:
+        """
+        A method for testing default Story.start_slide property.
+
+        Raises:
+            AssertionError: If the property value is not correct.
+        """
+
+        story = self.get_story()
+        self.assertEqual(story.start_slide, None)
+
+    def test_start_slide(self) -> None:
+        """
+        A method for testing Story.start_slide property.
+
+        Raises:
+            AssertionError: If the story html is not correct.
+        """
+
+        start_slide = 3
+        with unittest.mock.patch(
+            "ipyvizzustory.storylib.story.uuid.uuid4", return_value=self
+        ):
+            story = self.get_story()
+            story.start_slide = start_slide
+            self.assertEqual(
+                story.to_html(),
+                DISPLAY_TEMPLATE.format(
+                    id="1234567",
+                    vizzu_attribute="",
+                    start_slide=f'start-slide="{start_slide}"',
+                    vizzu_story=VIZZU_STORY,
+                    vizzu_player_data=self.get_vpd(),
+                    chart_size="",
+                    chart_features="",
+                    chart_events="",
+                ),
+            )
+
 
 class TestStoryHtml(TestHtml, unittest.TestCase):
     """A class for testing story html releated methods."""
 
     def setUp(self):
         self.test_dir = os.path.dirname(os.path.realpath(__file__))
 
@@ -412,14 +455,15 @@
             story = self.get_story()
             story.set_size(width=None, height=None)
             self.assertEqual(
                 story.to_html(),
                 DISPLAY_TEMPLATE.format(
                     id="1234567",
                     vizzu_attribute="",
+                    start_slide="",
                     vizzu_story=VIZZU_STORY,
                     vizzu_player_data=self.get_vpd(),
                     chart_size="",
                     chart_features="",
                     chart_events="",
                 ),
             )
@@ -438,14 +482,15 @@
             story = self.get_story()
             story.set_size(width="800px", height=None)
             self.assertEqual(
                 story.to_html(),
                 DISPLAY_TEMPLATE.format(
                     id="1234567",
                     vizzu_attribute="",
+                    start_slide="",
                     vizzu_story=VIZZU_STORY,
                     vizzu_player_data=self.get_vpd(),
                     chart_size="vp.style.cssText = 'width: 800px;'",
                     chart_features="",
                     chart_events="",
                 ),
             )
@@ -464,14 +509,15 @@
             story = self.get_story()
             story.set_size(width=None, height="480px")
             self.assertEqual(
                 story.to_html(),
                 DISPLAY_TEMPLATE.format(
                     id="1234567",
                     vizzu_attribute="",
+                    start_slide="",
                     vizzu_story=VIZZU_STORY,
                     vizzu_player_data=self.get_vpd(),
                     chart_size="vp.style.cssText = 'height: 480px;'",
                     chart_features="",
                     chart_events="",
                 ),
             )
@@ -509,14 +555,15 @@
             story.set_feature("tooltip", True)
             story.set_feature("tooltip", True)
             self.assertEqual(
                 story.to_html(),
                 DISPLAY_TEMPLATE.format(
                     id="1234567",
                     vizzu_attribute="",
+                    start_slide="",
                     vizzu_story=VIZZU_STORY,
                     vizzu_player_data=self.get_vpd(),
                     chart_size="",
                     chart_features=(
                         "chart.feature('tooltip', true);"
                         + f"\n{DISPLAY_INDENT * 3}"
                         + "chart.feature('tooltip', true);"
@@ -546,14 +593,15 @@
             story.add_event("plot-axis-label-draw", handler)
             story.add_event("plot-axis-label-draw", handler)
             self.assertEqual(
                 story.to_html(),
                 DISPLAY_TEMPLATE.format(
                     id="1234567",
                     vizzu_attribute="",
+                    start_slide="",
                     vizzu_story=VIZZU_STORY,
                     vizzu_player_data=self.get_vpd(),
                     chart_size="",
                     chart_features="",
                     chart_events=(
                         "chart.on('plot-axis-label-draw', "
                         + f"event => {{{' '.join(handler.split())}}});"
```

