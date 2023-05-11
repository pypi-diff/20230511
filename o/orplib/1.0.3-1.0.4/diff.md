# Comparing `tmp/orplib-1.0.3.tar.gz` & `tmp/orplib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orplib-1.0.3.tar", last modified: Thu Mar 16 22:44:53 2023, max compression
+gzip compressed data, was "orplib-1.0.4.tar", last modified: Thu May 11 21:09:09 2023, max compression
```

## Comparing `orplib-1.0.3.tar` & `orplib-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-16 22:44:53.519277 orplib-1.0.3/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       23 2022-02-01 16:30:04.000000 orplib-1.0.3/MANIFEST.in
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     9258 2023-03-16 22:44:53.519277 orplib-1.0.3/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8828 2023-03-16 22:41:04.000000 orplib-1.0.3/README.md
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2022-01-31 23:32:47.000000 orplib-1.0.3/pyproject.toml
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-03-16 22:44:53.519277 orplib-1.0.3/setup.cfg
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-16 22:44:53.454276 orplib-1.0.3/src/
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-16 22:44:53.484276 orplib-1.0.3/src/orpl/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      341 2023-03-16 22:41:45.000000 orplib-1.0.3/src/orpl/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-03-15 13:55:52.000000 orplib-1.0.3/src/orpl/__main__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-02-23 13:58:53.000000 orplib-1.0.3/src/orpl/baseline_removal.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-01-12 15:46:31.000000 orplib-1.0.3/src/orpl/bubblegif.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2022-06-16 00:44:35.000000 orplib-1.0.3/src/orpl/calibration.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2022-06-16 00:44:35.000000 orplib-1.0.3/src/orpl/cosmic_ray.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-16 22:44:53.511277 orplib-1.0.3/src/orpl/data/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2022-06-16 00:44:35.000000 orplib-1.0.3/src/orpl/data/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2022-06-16 00:44:35.000000 orplib-1.0.3/src/orpl/data/synthetic_presets.json
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1019 2023-03-14 19:37:33.000000 orplib-1.0.3/src/orpl/datatypes.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6125 2023-03-14 20:45:40.000000 orplib-1.0.3/src/orpl/file_io.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-16 22:44:53.518277 orplib-1.0.3/src/orpl/gui/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-15 16:45:41.000000 orplib-1.0.3/src/orpl/gui/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-02-23 13:58:54.000000 orplib-1.0.3/src/orpl/gui/mplcanvas.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    27768 2023-03-15 17:39:53.000000 orplib-1.0.3/src/orpl/gui/orplGUI.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-16 22:44:53.518277 orplib-1.0.3/src/orpl/gui/uis/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-15 16:48:26.000000 orplib-1.0.3/src/orpl/gui/uis/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30522 2023-03-02 22:27:38.000000 orplib-1.0.3/src/orpl/gui/uis/ui_mainWindow.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2022-11-11 19:47:58.000000 orplib-1.0.3/src/orpl/metrics.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2022-06-16 00:44:35.000000 orplib-1.0.3/src/orpl/normalization.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-03-02 19:51:11.000000 orplib-1.0.3/src/orpl/pipelines.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2022-06-16 00:44:35.000000 orplib-1.0.3/src/orpl/plot.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2022-06-16 00:44:35.000000 orplib-1.0.3/src/orpl/synthetic.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-03-16 22:44:53.519277 orplib-1.0.3/src/orplib.egg-info/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     9258 2023-03-16 22:44:53.000000 orplib-1.0.3/src/orplib.egg-info/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-03-16 22:44:53.000000 orplib-1.0.3/src/orplib.egg-info/SOURCES.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-03-16 22:44:53.000000 orplib-1.0.3/src/orplib.egg-info/dependency_links.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-03-16 22:44:53.000000 orplib-1.0.3/src/orplib.egg-info/requires.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-03-16 22:44:53.000000 orplib-1.0.3/src/orplib.egg-info/top_level.txt
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       45 2023-05-11 21:06:43.000000 orplib-1.0.4/MANIFEST.in
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6973 2023-05-11 21:09:09.195902 orplib-1.0.4/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6543 2023-04-28 16:12:50.000000 orplib-1.0.4/README.md
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2023-04-14 19:45:52.000000 orplib-1.0.4/pyproject.toml
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-05-11 21:09:09.196902 orplib-1.0.4/setup.cfg
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.193902 orplib-1.0.4/src/
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.194902 orplib-1.0.4/src/orpl/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      341 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-05-11 20:49:13.000000 orplib-1.0.4/src/orpl/__main__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/baseline_removal.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/bubblegif.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/calibration.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/cosmic_ray.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.194902 orplib-1.0.4/src/orpl/data/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/data/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/data/synthetic_presets.json
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1019 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/datatypes.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6237 2023-05-11 20:11:54.000000 orplib-1.0.4/src/orpl/file_io.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/src/orpl/gui/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/gui/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/gui/mplcanvas.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    28231 2023-05-11 20:49:15.000000 orplib-1.0.4/src/orpl/gui/orplGUI.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/src/orpl/gui/uis/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/gui/uis/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30696 2023-05-11 19:59:11.000000 orplib-1.0.4/src/orpl/gui/uis/ui_mainWindow.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/metrics.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/normalization.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/pipelines.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/plot.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2023-04-14 19:45:52.000000 orplib-1.0.4/src/orpl/synthetic.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-05-11 21:09:09.195902 orplib-1.0.4/src/orplib.egg-info/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6973 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/SOURCES.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/dependency_links.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/requires.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-05-11 21:09:09.000000 orplib-1.0.4/src/orplib.egg-info/top_level.txt
```

### Comparing `orplib-1.0.3/PKG-INFO` & `orplib-1.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orplib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Open Raman Processing Library
 Home-page: https://github.com/mr-sheg/orpl
 Author: Guillaume Sheehy
 Author-email: guillaume.sheehy@polymtl.ca
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,17 +26,17 @@
 
 ## Table of content
 
 - [ORPL](#orpl)
   - [Table of content](#table-of-content)
   - [ORPL GUI in action](#orpl-gui-in-action)
   - [Installation](#installation)
+    - [Windows Installation Guide](#windows-installation-guide)
     - [Already familiar with python and pip?](#already-familiar-with-python-and-pip)
-    - [I'm new to python and this 'pip' thing](#im-new-to-python-and-this-pip-thing)
-      - [Content of the `orpl GUI.txt` file](#content-of-the-orpl-guitxt-file)
+    - [I'm new to python and this 'pip' thing?](#im-new-to-python-and-this-pip-thing)
     - [Updating ORPL to the latest version](#updating-orpl-to-the-latest-version)
       - [If you have admin rights](#if-you-have-admin-rights)
       - [If you do not have admin rights](#if-you-do-not-have-admin-rights)
     - [Building from source](#building-from-source)
   - [Baseline removal](#baseline-removal)
     - [BubbleFill](#bubblefill)
   - [How to cite this work](#how-to-cite-this-work)
@@ -48,67 +48,31 @@
 
 https://user-images.githubusercontent.com/27356351/225768644-56ebf40a-51d1-44a1-bba3-edb86f8b1fad.mp4
 
 ## Installation
 
 At its core, ORPL is designed to be a processing library to use in your own processing workflow. Nevertheless, I also wrote a GUI to go with it if programming is not your jam. In either case, installation is made through **pip**.
 
+### Windows Installation Guide
+
+I wrote a detailed installation guide for windows complete with screenshots of all the steps, so do not worry if you are a python beginer and have no idea what I'm talking about here. You can access the guide on github ![here](/documentation/Installation%20guide%20-%20Windows.md) or download a ![PDF](/documentation/Installing%20ORPL%20-%20Windows.pdf) version.
+
 ### Already familiar with python and pip?
 
 I recommend you create a virtual environment with [**venv**](https://docs.python.org/3/library/venv.html). Otherwise, just install **orplib** with pip.
 
 ```
 pip install orplib
 ```
 
 Using Anaconda?... dont... Jokes aside, if people ask me about this, I might write a guide for this. Otherwise, use pip.
 
-### I'm new to python and this 'pip' thing
-
-I made a video going through everything on a clean Windows 11 [VM](https://en.wikipedia.org/wiki/Virtual_machine). Here is the video so you can follow step-by-step. PLEASE, make certain you follow the steps EXACTLY for the python installation. Otherwise, you'll get a bunch of error in your terminal and might get lost.
-
-https://user-images.githubusercontent.com/27356351/225757919-e89d59c2-ff3f-4555-bffc-16b11ef3ecde.mp4
-
-The steps for **Windows** are:
+### I'm new to python and this 'pip' thing?
 
-1. Check if python is already installed
-   1. Open a terminal
-   2. run `python`
-      - If you get something like `Python 3.X.X (tag)... Type "help", "copyright", ...`, then you already have a python version installed. Check if it is compatible with ORPL. If so, move to Step 2.7
-      - If a Microsoft Store window opens, or you get a message along the line of `... is not recognized as an internal or external command...`, then python is not installed. Proceed with Step 2.1
-2. Install python (I test with [python 3.8.10](https://www.python.org/downloads/release/python-3810/), but other versions might work perfectly fine)
-   1. **DO NOT!!!** use "Install Now" or default setting, it almost certainly won't work, and you'll have to start over again.
-   2. Make sure you check all boxes on the first page.
-   3. Use "Customize installation".
-   4. Make sure you check EVERYTHING, I mean ALL checkboxes as you keep going through the pages.
-   5. Once the installation is finished, you'll see a last page with "Setup was successful" if it worked. You might see a `Disable path length limit...` option. If so, click it and accept.
-   6. Check if **Python** was correctly installed by running `python` in a terminal (see Step 2.2)
-   7. Check if **pip** was installed and added to your Path by running `pip` in a new terminal.
-      - If you see a long stream of text starting with `Usage: pip <command> [options]`, then you are good!
-      - Otherwise, something went wrong...
-3. Install orplib (https://pypi.org/project/orplib/) with pip
-   1. Run pip command for installation:
-      - If your user has admin rights, run `pip install orplib` in terminal
-      - Otherwise, run `pip install orplib --user` in terminal
-   2. Check that ORPL installed correctly by running `python -m orpl` in terminal.
-      - If you get an error message, something went wrong...
-      - Otherwise, it will take a few seconds the first time you launch it. Please, be patient.
-4. (optional) create a script file to launch ORPL - GUI
-   1. Create a new text file on the Desktop (I suggest calling it `orpl GUI.txt`)
-   2. Open the text file with notepad
-   3. Write the content below inside that file
-   4. Save the file and close it
-   5. Change the extension name of the file to `.bat`
-
-##### Content of the `orpl GUI.txt` file
-
-```
-python -m orpl
-pause
-```
+I am working on a python tutorial repository, you can learn more about it ![here](https://github.com/mr-sheg/Python-Tutorials).
 
 ### Updating ORPL to the latest version
 
 If you want to update to the latest version of ORPL, run the following pip command,
 
 #### If you have admin rights
```

### Comparing `orplib-1.0.3/README.md` & `orplib-1.0.4/src/orplib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: orplib
+Version: 1.0.4
+Summary: Open Raman Processing Library
+Home-page: https://github.com/mr-sheg/orpl
+Author: Guillaume Sheehy
+Author-email: guillaume.sheehy@polymtl.ca
+License: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # ORPL
 
 ORPL (read _orpel_) is the Open Raman Processing Library. It provides tools for the processing of Raman spectrum, including;
 
 1. System calibration (x-axis and system response)
 2. Cosmic Ray removal
 3. Baseline removal (autofluorescence)
@@ -12,17 +26,17 @@
 
 ## Table of content
 
 - [ORPL](#orpl)
   - [Table of content](#table-of-content)
   - [ORPL GUI in action](#orpl-gui-in-action)
   - [Installation](#installation)
+    - [Windows Installation Guide](#windows-installation-guide)
     - [Already familiar with python and pip?](#already-familiar-with-python-and-pip)
-    - [I'm new to python and this 'pip' thing](#im-new-to-python-and-this-pip-thing)
-      - [Content of the `orpl GUI.txt` file](#content-of-the-orpl-guitxt-file)
+    - [I'm new to python and this 'pip' thing?](#im-new-to-python-and-this-pip-thing)
     - [Updating ORPL to the latest version](#updating-orpl-to-the-latest-version)
       - [If you have admin rights](#if-you-have-admin-rights)
       - [If you do not have admin rights](#if-you-do-not-have-admin-rights)
     - [Building from source](#building-from-source)
   - [Baseline removal](#baseline-removal)
     - [BubbleFill](#bubblefill)
   - [How to cite this work](#how-to-cite-this-work)
@@ -34,67 +48,31 @@
 
 https://user-images.githubusercontent.com/27356351/225768644-56ebf40a-51d1-44a1-bba3-edb86f8b1fad.mp4
 
 ## Installation
 
 At its core, ORPL is designed to be a processing library to use in your own processing workflow. Nevertheless, I also wrote a GUI to go with it if programming is not your jam. In either case, installation is made through **pip**.
 
+### Windows Installation Guide
+
+I wrote a detailed installation guide for windows complete with screenshots of all the steps, so do not worry if you are a python beginer and have no idea what I'm talking about here. You can access the guide on github ![here](/documentation/Installation%20guide%20-%20Windows.md) or download a ![PDF](/documentation/Installing%20ORPL%20-%20Windows.pdf) version.
+
 ### Already familiar with python and pip?
 
 I recommend you create a virtual environment with [**venv**](https://docs.python.org/3/library/venv.html). Otherwise, just install **orplib** with pip.
 
 ```
 pip install orplib
 ```
 
 Using Anaconda?... dont... Jokes aside, if people ask me about this, I might write a guide for this. Otherwise, use pip.
 
-### I'm new to python and this 'pip' thing
-
-I made a video going through everything on a clean Windows 11 [VM](https://en.wikipedia.org/wiki/Virtual_machine). Here is the video so you can follow step-by-step. PLEASE, make certain you follow the steps EXACTLY for the python installation. Otherwise, you'll get a bunch of error in your terminal and might get lost.
-
-https://user-images.githubusercontent.com/27356351/225757919-e89d59c2-ff3f-4555-bffc-16b11ef3ecde.mp4
+### I'm new to python and this 'pip' thing?
 
-The steps for **Windows** are:
-
-1. Check if python is already installed
-   1. Open a terminal
-   2. run `python`
-      - If you get something like `Python 3.X.X (tag)... Type "help", "copyright", ...`, then you already have a python version installed. Check if it is compatible with ORPL. If so, move to Step 2.7
-      - If a Microsoft Store window opens, or you get a message along the line of `... is not recognized as an internal or external command...`, then python is not installed. Proceed with Step 2.1
-2. Install python (I test with [python 3.8.10](https://www.python.org/downloads/release/python-3810/), but other versions might work perfectly fine)
-   1. **DO NOT!!!** use "Install Now" or default setting, it almost certainly won't work, and you'll have to start over again.
-   2. Make sure you check all boxes on the first page.
-   3. Use "Customize installation".
-   4. Make sure you check EVERYTHING, I mean ALL checkboxes as you keep going through the pages.
-   5. Once the installation is finished, you'll see a last page with "Setup was successful" if it worked. You might see a `Disable path length limit...` option. If so, click it and accept.
-   6. Check if **Python** was correctly installed by running `python` in a terminal (see Step 2.2)
-   7. Check if **pip** was installed and added to your Path by running `pip` in a new terminal.
-      - If you see a long stream of text starting with `Usage: pip <command> [options]`, then you are good!
-      - Otherwise, something went wrong...
-3. Install orplib (https://pypi.org/project/orplib/) with pip
-   1. Run pip command for installation:
-      - If your user has admin rights, run `pip install orplib` in terminal
-      - Otherwise, run `pip install orplib --user` in terminal
-   2. Check that ORPL installed correctly by running `python -m orpl` in terminal.
-      - If you get an error message, something went wrong...
-      - Otherwise, it will take a few seconds the first time you launch it. Please, be patient.
-4. (optional) create a script file to launch ORPL - GUI
-   1. Create a new text file on the Desktop (I suggest calling it `orpl GUI.txt`)
-   2. Open the text file with notepad
-   3. Write the content below inside that file
-   4. Save the file and close it
-   5. Change the extension name of the file to `.bat`
-
-##### Content of the `orpl GUI.txt` file
-
-```
-python -m orpl
-pause
-```
+I am working on a python tutorial repository, you can learn more about it ![here](https://github.com/mr-sheg/Python-Tutorials).
 
 ### Updating ORPL to the latest version
 
 If you want to update to the latest version of ORPL, run the following pip command,
 
 #### If you have admin rights
```

### Comparing `orplib-1.0.3/setup.cfg` & `orplib-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = orplib
-version = 1.0.3
+version = 1.0.4
 author = Guillaume Sheehy
 author_email = guillaume.sheehy@polymtl.ca
 description = Open Raman Processing Library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/mr-sheg/orpl
```

### Comparing `orplib-1.0.3/src/orpl/baseline_removal.py` & `orplib-1.0.4/src/orpl/baseline_removal.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/bubblegif.py` & `orplib-1.0.4/src/orpl/bubblegif.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/calibration.py` & `orplib-1.0.4/src/orpl/calibration.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/cosmic_ray.py` & `orplib-1.0.4/src/orpl/cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/data/synthetic_presets.json` & `orplib-1.0.4/src/orpl/data/synthetic_presets.json`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/datatypes.py` & `orplib-1.0.4/src/orpl/datatypes.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/file_io.py` & `orplib-1.0.4/src/orpl/file_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,22 @@
     spectrum = load_function[file_path.suffix](file_path)
 
     return spectrum
 
 
 def load_sif(sif_file: Path) -> Spectrum:
     data_array, meta_dict = sif_parser.np_open(sif_file)
-    data_array = np.squeeze(data_array)
+    data_array = np.squeeze(data_array).T
+    if data_array.ndim > 1:
+        data_array = np.flip(data_array, axis=0)
 
     # cleaning up string metadata
     for k, v in meta_dict.items():
         if isinstance(v, bytes):
-            meta_dict[k] = v.decode()
+            meta_dict[k] = v.decode(encoding="utf8", errors="replace")
         if isinstance(v, str):
             meta_dict[k] = v.strip()
 
     metadata = Metadata(
         filepath=sif_file,
         source_power=None,
         exposure_time=meta_dict["CycleTime"],
```

### Comparing `orplib-1.0.3/src/orpl/gui/mplcanvas.py` & `orplib-1.0.4/src/orpl/gui/mplcanvas.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/gui/orplGUI.py` & `orplib-1.0.4/src/orpl/gui/orplGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,26 @@
         self.plot_raw_spectra()
 
         if self.checkBoxAutoUpdate.isChecked():
             self.process_spectra()
 
     def processing_changed(self):
         logger.info("Processing update - %s - changed", self.sender().objectName())
+
+        br_method = self.comboBoxBRAlgorithm.currentText()
+        self.spinBoxPolyOrder.setEnabled(False)
+        self.spinBoxHWS.setEnabled(False)
+        self.spinBoxBubbleWidth.setEnabled(False)
+        if br_method == "IModPoly":
+            self.spinBoxPolyOrder.setEnabled(True)
+        elif br_method == "MorphBR":
+            self.spinBoxHWS.setEnabled(True)
+        elif br_method == "BubbleFill":
+            self.spinBoxBubbleWidth.setEnabled(True)
+
         if self.checkBoxAutoUpdate.isChecked():
             self.process_spectra()
 
     def plot_raw_spectra(self):
         logger.info("Updating Raw Spectra plot")
         # Update Spectra graph (in Processing tab)
         ax = self.rawDataPlot.canvas.axes
```

### Comparing `orplib-1.0.3/src/orpl/gui/uis/ui_mainWindow.py` & `orplib-1.0.4/src/orpl/gui/uis/ui_mainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_mainWindow(object):
     def setupUi(self, mainWindow):
         mainWindow.setObjectName("mainWindow")
-        mainWindow.resize(999, 726)
+        mainWindow.resize(921, 715)
         self.centralwidget = QtWidgets.QWidget(mainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.horizontalLayout = QtWidgets.QHBoxLayout(self.centralwidget)
         self.horizontalLayout.setObjectName("horizontalLayout")
         self.tabWidget = QtWidgets.QTabWidget(self.centralwidget)
         self.tabWidget.setObjectName("tabWidget")
         self.tabFileIO = QtWidgets.QWidget()
@@ -169,15 +169,15 @@
         self.horizontalLayout_16 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_16.setObjectName("horizontalLayout_16")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout()
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.processingToolBox = QtWidgets.QToolBox(self.tabProcessing)
         self.processingToolBox.setObjectName("processingToolBox")
         self.pageCRR = QtWidgets.QWidget()
-        self.pageCRR.setGeometry(QtCore.QRect(0, 0, 133, 353))
+        self.pageCRR.setGeometry(QtCore.QRect(0, 0, 122, 342))
         self.pageCRR.setObjectName("pageCRR")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.pageCRR)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.label_4 = QtWidgets.QLabel(self.pageCRR)
         self.label_4.setObjectName("label_4")
         self.verticalLayout_6.addWidget(self.label_4)
         self.spinBoxLeftCrop = QtWidgets.QSpinBox(self.pageCRR)
@@ -234,15 +234,15 @@
         self.spinBoxSCRRstd.setSingleStep(0.01)
         self.spinBoxSCRRstd.setObjectName("spinBoxSCRRstd")
         self.verticalLayout_10.addWidget(self.spinBoxSCRRstd)
         spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_10.addItem(spacerItem2)
         self.processingToolBox.addItem(self.page_3, "")
         self.page_2 = QtWidgets.QWidget()
-        self.page_2.setGeometry(QtCore.QRect(0, 0, 155, 258))
+        self.page_2.setGeometry(QtCore.QRect(0, 0, 226, 335))
         self.page_2.setObjectName("page_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.page_2)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.comboBoxBRAlgorithm = QtWidgets.QComboBox(self.page_2)
         self.comboBoxBRAlgorithm.setObjectName("comboBoxBRAlgorithm")
         self.comboBoxBRAlgorithm.addItem("")
         self.comboBoxBRAlgorithm.addItem("")
@@ -254,38 +254,41 @@
         self.line_4.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_4.setObjectName("line_4")
         self.verticalLayout_7.addWidget(self.line_4)
         self.label_8 = QtWidgets.QLabel(self.page_2)
         self.label_8.setObjectName("label_8")
         self.verticalLayout_7.addWidget(self.label_8)
         self.spinBoxPolyOrder = QtWidgets.QSpinBox(self.page_2)
+        self.spinBoxPolyOrder.setEnabled(False)
         self.spinBoxPolyOrder.setMaximum(15)
         self.spinBoxPolyOrder.setObjectName("spinBoxPolyOrder")
         self.verticalLayout_7.addWidget(self.spinBoxPolyOrder)
         self.line_3 = QtWidgets.QFrame(self.page_2)
         self.line_3.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_3.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_3.setObjectName("line_3")
         self.verticalLayout_7.addWidget(self.line_3)
         self.label_7 = QtWidgets.QLabel(self.page_2)
         self.label_7.setObjectName("label_7")
         self.verticalLayout_7.addWidget(self.label_7)
         self.spinBoxHWS = QtWidgets.QSpinBox(self.page_2)
+        self.spinBoxHWS.setEnabled(False)
         self.spinBoxHWS.setMinimum(1)
         self.spinBoxHWS.setObjectName("spinBoxHWS")
         self.verticalLayout_7.addWidget(self.spinBoxHWS)
         self.line_2 = QtWidgets.QFrame(self.page_2)
         self.line_2.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_2.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_2.setObjectName("line_2")
         self.verticalLayout_7.addWidget(self.line_2)
         self.label_6 = QtWidgets.QLabel(self.page_2)
         self.label_6.setObjectName("label_6")
         self.verticalLayout_7.addWidget(self.label_6)
         self.spinBoxBubbleWidth = QtWidgets.QSpinBox(self.page_2)
+        self.spinBoxBubbleWidth.setEnabled(False)
         self.spinBoxBubbleWidth.setMinimum(1)
         self.spinBoxBubbleWidth.setObjectName("spinBoxBubbleWidth")
         self.verticalLayout_7.addWidget(self.spinBoxBubbleWidth)
         spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_7.addItem(spacerItem3)
         self.processingToolBox.addItem(self.page_2, "")
         self.page = QtWidgets.QWidget()
@@ -451,20 +454,20 @@
         self.label_10.setText(_translate("mainWindow", "Width"))
         self.label_11.setText(_translate("mainWindow", "Disparity Threshold"))
         self.checkBoxSingleCRR.setText(_translate("mainWindow", "Single-accumulation filter"))
         self.label_12.setText(_translate("mainWindow", "Width"))
         self.label_13.setText(_translate("mainWindow", "STD factor"))
         self.processingToolBox.setItemText(self.processingToolBox.indexOf(self.page_3), _translate("mainWindow", "CRR"))
         self.comboBoxBRAlgorithm.setItemText(0, _translate("mainWindow", "None"))
-        self.comboBoxBRAlgorithm.setItemText(1, _translate("mainWindow", "BubbleFill"))
-        self.comboBoxBRAlgorithm.setItemText(2, _translate("mainWindow", "IModPoly"))
-        self.comboBoxBRAlgorithm.setItemText(3, _translate("mainWindow", "MorphBR"))
-        self.label_8.setText(_translate("mainWindow", "Polynomial Order"))
-        self.label_7.setText(_translate("mainWindow", "half width window size"))
-        self.label_6.setText(_translate("mainWindow", "Minimum Bubble Width"))
+        self.comboBoxBRAlgorithm.setItemText(1, _translate("mainWindow", "IModPoly"))
+        self.comboBoxBRAlgorithm.setItemText(2, _translate("mainWindow", "MorphBR"))
+        self.comboBoxBRAlgorithm.setItemText(3, _translate("mainWindow", "BubbleFill"))
+        self.label_8.setText(_translate("mainWindow", "Polynomial Order (IModPoly)"))
+        self.label_7.setText(_translate("mainWindow", "half width window size (MorphBR)"))
+        self.label_6.setText(_translate("mainWindow", "Minimum Bubble Width (BubbleFill)"))
         self.processingToolBox.setItemText(self.processingToolBox.indexOf(self.page_2), _translate("mainWindow", "Baseline Removal"))
         self.radioButtonNoNorm.setText(_translate("mainWindow", "None"))
         self.radioButtonMinMax.setText(_translate("mainWindow", "MinMax"))
         self.radioButtonAUC.setText(_translate("mainWindow", "AUC"))
         self.radioButtonSNV.setText(_translate("mainWindow", "SNV"))
         self.radioButtonMaxBand.setText(_translate("mainWindow", "Max band"))
         self.label_9.setText(_translate("mainWindow", "Band selection"))
```

### Comparing `orplib-1.0.3/src/orpl/metrics.py` & `orplib-1.0.4/src/orpl/metrics.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/normalization.py` & `orplib-1.0.4/src/orpl/normalization.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/plot.py` & `orplib-1.0.4/src/orpl/plot.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orpl/synthetic.py` & `orplib-1.0.4/src/orpl/synthetic.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.3/src/orplib.egg-info/PKG-INFO` & `orplib-1.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: orplib
-Version: 1.0.3
-Summary: Open Raman Processing Library
-Home-page: https://github.com/mr-sheg/orpl
-Author: Guillaume Sheehy
-Author-email: guillaume.sheehy@polymtl.ca
-License: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # ORPL
 
 ORPL (read _orpel_) is the Open Raman Processing Library. It provides tools for the processing of Raman spectrum, including;
 
 1. System calibration (x-axis and system response)
 2. Cosmic Ray removal
 3. Baseline removal (autofluorescence)
@@ -26,17 +12,17 @@
 
 ## Table of content
 
 - [ORPL](#orpl)
   - [Table of content](#table-of-content)
   - [ORPL GUI in action](#orpl-gui-in-action)
   - [Installation](#installation)
+    - [Windows Installation Guide](#windows-installation-guide)
     - [Already familiar with python and pip?](#already-familiar-with-python-and-pip)
-    - [I'm new to python and this 'pip' thing](#im-new-to-python-and-this-pip-thing)
-      - [Content of the `orpl GUI.txt` file](#content-of-the-orpl-guitxt-file)
+    - [I'm new to python and this 'pip' thing?](#im-new-to-python-and-this-pip-thing)
     - [Updating ORPL to the latest version](#updating-orpl-to-the-latest-version)
       - [If you have admin rights](#if-you-have-admin-rights)
       - [If you do not have admin rights](#if-you-do-not-have-admin-rights)
     - [Building from source](#building-from-source)
   - [Baseline removal](#baseline-removal)
     - [BubbleFill](#bubblefill)
   - [How to cite this work](#how-to-cite-this-work)
@@ -48,67 +34,31 @@
 
 https://user-images.githubusercontent.com/27356351/225768644-56ebf40a-51d1-44a1-bba3-edb86f8b1fad.mp4
 
 ## Installation
 
 At its core, ORPL is designed to be a processing library to use in your own processing workflow. Nevertheless, I also wrote a GUI to go with it if programming is not your jam. In either case, installation is made through **pip**.
 
+### Windows Installation Guide
+
+I wrote a detailed installation guide for windows complete with screenshots of all the steps, so do not worry if you are a python beginer and have no idea what I'm talking about here. You can access the guide on github ![here](/documentation/Installation%20guide%20-%20Windows.md) or download a ![PDF](/documentation/Installing%20ORPL%20-%20Windows.pdf) version.
+
 ### Already familiar with python and pip?
 
 I recommend you create a virtual environment with [**venv**](https://docs.python.org/3/library/venv.html). Otherwise, just install **orplib** with pip.
 
 ```
 pip install orplib
 ```
 
 Using Anaconda?... dont... Jokes aside, if people ask me about this, I might write a guide for this. Otherwise, use pip.
 
-### I'm new to python and this 'pip' thing
-
-I made a video going through everything on a clean Windows 11 [VM](https://en.wikipedia.org/wiki/Virtual_machine). Here is the video so you can follow step-by-step. PLEASE, make certain you follow the steps EXACTLY for the python installation. Otherwise, you'll get a bunch of error in your terminal and might get lost.
-
-https://user-images.githubusercontent.com/27356351/225757919-e89d59c2-ff3f-4555-bffc-16b11ef3ecde.mp4
+### I'm new to python and this 'pip' thing?
 
-The steps for **Windows** are:
-
-1. Check if python is already installed
-   1. Open a terminal
-   2. run `python`
-      - If you get something like `Python 3.X.X (tag)... Type "help", "copyright", ...`, then you already have a python version installed. Check if it is compatible with ORPL. If so, move to Step 2.7
-      - If a Microsoft Store window opens, or you get a message along the line of `... is not recognized as an internal or external command...`, then python is not installed. Proceed with Step 2.1
-2. Install python (I test with [python 3.8.10](https://www.python.org/downloads/release/python-3810/), but other versions might work perfectly fine)
-   1. **DO NOT!!!** use "Install Now" or default setting, it almost certainly won't work, and you'll have to start over again.
-   2. Make sure you check all boxes on the first page.
-   3. Use "Customize installation".
-   4. Make sure you check EVERYTHING, I mean ALL checkboxes as you keep going through the pages.
-   5. Once the installation is finished, you'll see a last page with "Setup was successful" if it worked. You might see a `Disable path length limit...` option. If so, click it and accept.
-   6. Check if **Python** was correctly installed by running `python` in a terminal (see Step 2.2)
-   7. Check if **pip** was installed and added to your Path by running `pip` in a new terminal.
-      - If you see a long stream of text starting with `Usage: pip <command> [options]`, then you are good!
-      - Otherwise, something went wrong...
-3. Install orplib (https://pypi.org/project/orplib/) with pip
-   1. Run pip command for installation:
-      - If your user has admin rights, run `pip install orplib` in terminal
-      - Otherwise, run `pip install orplib --user` in terminal
-   2. Check that ORPL installed correctly by running `python -m orpl` in terminal.
-      - If you get an error message, something went wrong...
-      - Otherwise, it will take a few seconds the first time you launch it. Please, be patient.
-4. (optional) create a script file to launch ORPL - GUI
-   1. Create a new text file on the Desktop (I suggest calling it `orpl GUI.txt`)
-   2. Open the text file with notepad
-   3. Write the content below inside that file
-   4. Save the file and close it
-   5. Change the extension name of the file to `.bat`
-
-##### Content of the `orpl GUI.txt` file
-
-```
-python -m orpl
-pause
-```
+I am working on a python tutorial repository, you can learn more about it ![here](https://github.com/mr-sheg/Python-Tutorials).
 
 ### Updating ORPL to the latest version
 
 If you want to update to the latest version of ORPL, run the following pip command,
 
 #### If you have admin rights
```

### Comparing `orplib-1.0.3/src/orplib.egg-info/SOURCES.txt` & `orplib-1.0.4/src/orplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

