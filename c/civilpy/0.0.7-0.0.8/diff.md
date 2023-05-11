# Comparing `tmp/civilpy-0.0.7.tar.gz` & `tmp/civilpy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.7.tar", last modified: Thu Jan  5 18:15:05 2023, max compression
+gzip compressed data, was "civilpy-0.0.8.tar", last modified: Sat Jan 14 06:03:06 2023, max compression
```

## Comparing `civilpy-0.0.7.tar` & `civilpy-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.969891 civilpy-0.0.7/
--rw-rw-r--   0 dane      (1000) dane      (1000)      175 2023-01-04 20:04:45.000000 civilpy-0.0.7/.gitlab-ci.yml
--rw-rw-r--   0 dane      (1000) dane      (1000)     1088 2023-01-04 20:04:45.000000 civilpy-0.0.7/LICENSE
--rw-rw-r--   0 dane      (1000) dane      (1000)      112 2023-01-04 20:04:45.000000 civilpy-0.0.7/MANIFEST.in
--rw-rw-r--   0 dane      (1000) dane      (1000)     4372 2023-01-05 18:15:05.969891 civilpy-0.0.7/PKG-INFO
--rw-rw-r--   0 dane      (1000) dane      (1000)     3908 2023-01-04 20:04:45.000000 civilpy-0.0.7/README.md
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/
--rw-rw-r--   0 dane      (1000) dane      (1000)     1101 2023-01-05 17:27:53.000000 civilpy-0.0.7/civilpy/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/construction/
--rw-rw-r--   0 dane      (1000) dane      (1000)       37 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/construction/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/environmental/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/environmental/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/general/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/cli.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/gis.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/kml_tools.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/math.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/pdf.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/physics.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/plan_development.py
--rw-rw-r--   0 dane      (1000) dane      (1000)      507 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/general/tello_drone.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/geotechnical/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/geotechnical/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/state/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/state/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/state/ohio/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/state/ohio/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)    26116 2023-01-05 18:14:47.000000 civilpy-0.0.7/civilpy/state/ohio/dot.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/structural/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/structural/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/structural/search_tools.py
--rw-rw-r--   0 dane      (1000) dane      (1000)      142 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/structural/steel.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/transportation/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/transportation/__init__.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy/water_resources/
--rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/water_resources/__init__.py
--rw-rw-r--   0 dane      (1000) dane      (1000)      227 2023-01-04 20:04:45.000000 civilpy-0.0.7/civilpy/water_resources/hydraulics.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/civilpy.egg-info/
--rw-rw-r--   0 dane      (1000) dane      (1000)     4372 2023-01-05 18:15:05.000000 civilpy-0.0.7/civilpy.egg-info/PKG-INFO
--rw-rw-r--   0 dane      (1000) dane      (1000)      910 2023-01-05 18:15:05.000000 civilpy-0.0.7/civilpy.egg-info/SOURCES.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)        1 2023-01-05 18:15:05.000000 civilpy-0.0.7/civilpy.egg-info/dependency_links.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)      104 2023-01-05 18:15:05.000000 civilpy-0.0.7/civilpy.egg-info/requires.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)        8 2023-01-05 18:15:05.000000 civilpy-0.0.7/civilpy.egg-info/top_level.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)       24 2023-01-04 20:04:45.000000 civilpy-0.0.7/pytest.ini
--rw-rw-r--   0 dane      (1000) dane      (1000)     2486 2023-01-05 17:27:53.000000 civilpy-0.0.7/requirements.txt
--rw-rw-r--   0 dane      (1000) dane      (1000)       38 2023-01-05 18:15:05.969891 civilpy-0.0.7/setup.cfg
--rw-rw-r--   0 dane      (1000) dane      (1000)     1371 2023-01-05 18:15:01.000000 civilpy-0.0.7/setup.py
-drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-05 18:15:05.965891 civilpy-0.0.7/tests/
--rw-rw-r--   0 dane      (1000) dane      (1000)      229 2023-01-04 20:04:45.000000 civilpy-0.0.7/tests/test_helloworld.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.971480 civilpy-0.0.8/
+-rw-rw-r--   0 dane      (1000) dane      (1000)      175 2023-01-13 22:29:28.000000 civilpy-0.0.8/.gitlab-ci.yml
+-rw-rw-r--   0 dane      (1000) dane      (1000)     1088 2023-01-13 22:29:28.000000 civilpy-0.0.8/LICENSE
+-rw-rw-r--   0 dane      (1000) dane      (1000)      112 2023-01-13 22:29:28.000000 civilpy-0.0.8/MANIFEST.in
+-rw-rw-r--   0 dane      (1000) dane      (1000)     4335 2023-01-14 06:03:06.967480 civilpy-0.0.8/PKG-INFO
+-rw-rw-r--   0 dane      (1000) dane      (1000)     3908 2023-01-13 22:29:28.000000 civilpy-0.0.8/README.md
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy/
+-rw-rw-r--   0 dane      (1000) dane      (1000)     1101 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/__init__.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy/construction/
+-rw-rw-r--   0 dane      (1000) dane      (1000)       37 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/construction/__init__.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy/environmental/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/environmental/__init__.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy/general/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/__init__.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/cli.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)     1091 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/database_tools.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/gis.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/kml_tools.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/math.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/pdf.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/physics.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/plan_development.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)      507 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/general/tello_drone.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy/geotechnical/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/geotechnical/__init__.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy/state/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/state/__init__.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy/state/ohio/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/state/ohio/__init__.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)    26117 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/state/ohio/dot.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.951480 civilpy-0.0.8/civilpy/structural/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/structural/__init__.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/structural/search_tools.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)      142 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/structural/steel.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.951480 civilpy-0.0.8/civilpy/transportation/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/transportation/__init__.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.951480 civilpy-0.0.8/civilpy/water_resources/
+-rw-rw-r--   0 dane      (1000) dane      (1000)        0 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/water_resources/__init__.py
+-rw-rw-r--   0 dane      (1000) dane      (1000)      227 2023-01-13 22:29:28.000000 civilpy-0.0.8/civilpy/water_resources/hydraulics.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.947480 civilpy-0.0.8/civilpy.egg-info/
+-rw-rw-r--   0 dane      (1000) dane      (1000)     4335 2023-01-14 06:03:06.000000 civilpy-0.0.8/civilpy.egg-info/PKG-INFO
+-rw-rw-r--   0 dane      (1000) dane      (1000)      944 2023-01-14 06:03:06.000000 civilpy-0.0.8/civilpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 dane      (1000) dane      (1000)        1 2023-01-14 06:03:06.000000 civilpy-0.0.8/civilpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 dane      (1000) dane      (1000)      236 2023-01-14 06:03:06.000000 civilpy-0.0.8/civilpy.egg-info/requires.txt
+-rw-rw-r--   0 dane      (1000) dane      (1000)        8 2023-01-14 06:03:06.000000 civilpy-0.0.8/civilpy.egg-info/top_level.txt
+-rw-rw-r--   0 dane      (1000) dane      (1000)       24 2023-01-13 22:29:28.000000 civilpy-0.0.8/pytest.ini
+-rw-rw-r--   0 dane      (1000) dane      (1000)     2534 2023-01-14 05:58:05.000000 civilpy-0.0.8/requirements.txt
+-rw-rw-r--   0 dane      (1000) dane      (1000)       38 2023-01-14 06:03:06.971480 civilpy-0.0.8/setup.cfg
+-rw-rw-r--   0 dane      (1000) dane      (1000)     1598 2023-01-14 05:44:42.000000 civilpy-0.0.8/setup.py
+drwxrwxr-x   0 dane      (1000) dane      (1000)        0 2023-01-14 06:03:06.951480 civilpy-0.0.8/tests/
+-rw-rw-r--   0 dane      (1000) dane      (1000)      229 2023-01-13 22:29:28.000000 civilpy-0.0.8/tests/test_helloworld.py
```

### Comparing `civilpy-0.0.7/LICENSE` & `civilpy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.7/PKG-INFO` & `civilpy-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -104,9 +102,7 @@
     K --> |Yes| N("Save under a file for the standard<br>i.e. civilpy.structural.aisc")
     K --> |No| O("save to the relevant __init__.py")
     P("Save under civilpy.general.[relevant_file]")
     N --> |Doesn't make sense to put it there| P
     O --> |Doesn't make sense to put it there|P
 ```
 </div>
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.7 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.8 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
-Parks Author-email: Dane@daneparks.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License Classifier: Environment ::
-Console :: Curses Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE # CivilPy Code snippets for Civil Engineering related
-tasks ## About (Skip to the "Installation" section to start running code)
-Welcome to the CivilPy repository. This program is a simple terminal based
-software package to give users easier access to some of the packages from the
-python repository. The package is focused on civil engineering related tasks
-such as file management, pdf data extraction, image manipulation mapping and
-unit conversions. I did my best to make the user interface obvious to use and
-tried to keep the functionality compatible with tools available to the average
-Civil engineer. ## Intro This repository was created in order for me to gain a
-better understanding of software development work flows and how they can be re-
+Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
+MIT License Classifier: Environment :: Console :: Curses Description-Content-
+Type: text/markdown Provides-Extra: dev License-File: LICENSE # CivilPy Code
+snippets for Civil Engineering related tasks ## About (Skip to the
+"Installation" section to start running code) Welcome to the CivilPy
+repository. This program is a simple terminal based software package to give
+users easier access to some of the packages from the python repository. The
+package is focused on civil engineering related tasks such as file management,
+pdf data extraction, image manipulation mapping and unit conversions. I did my
+best to make the user interface obvious to use and tried to keep the
+functionality compatible with tools available to the average Civil engineer. ##
+Intro This repository was created in order for me to gain a better
+understanding of software development work flows and how they can be re-
 purposed for civil engineering related tasks. This is by no means a
 comprehensive or even functional repository but is more a way for me to track
 my progress while learning more about another industry. There may occasionally
 be how-tos and other code posted here but this repository is not meant as
 tutorial or in depth explanation for how coding works. For those types of
 things I highly suggest you instead check Youtube for general lessons or Stack
 Overflow for specific issues. I highly recommend the Harvard_CS50_Youtube
```

### Comparing `civilpy-0.0.7/README.md` & `civilpy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.7/civilpy/__init__.py` & `civilpy-0.0.8/civilpy/__init__.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.7/civilpy/state/ohio/dot.py` & `civilpy-0.0.8/civilpy/state/ohio/dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
                 pass
             else:
                 print(f"\nWriting tiff file to W:\\CivilPy_Output\\pulled_plans\\{self.SFN}\\{file_set_name}.tiff...\n")
                 try:
                     tifftools.write_tiff(tiff_objects_list[0], f"W:\\CivilPy_Output\\pulled_plans\\{self.SFN}\\{file_set_name}.tiff")
                 except(AttributeError):
                     print(f"There is a problem with the tiff file at \nW:\\CivilPy_Output\\"
-                          f"pulled_plans\\{self.SFN}\\{file_set_name}.tiff\nYou might want to check there"
+                          f"pulled_plans\\{self.SFN}\\{file_set_name}.tiff\nYou might want to check there "
                           f"to resolve the issue\n\n")
 
             # Convert multipage tiff file to pdf
             try:
                 self.tiff_to_pdf(f"W:\\CivilPy_Output\\pulled_plans\\{self.SFN}\\{file_set_name}.tiff")
             except:
                 print(f"There was an error during conversion of the file: W:\\CivilPy_Output\\pulled_plans\\{self.SFN}"
```

### Comparing `civilpy-0.0.7/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.8/civilpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -104,9 +102,7 @@
     K --> |Yes| N("Save under a file for the standard<br>i.e. civilpy.structural.aisc")
     K --> |No| O("save to the relevant __init__.py")
     P("Save under civilpy.general.[relevant_file]")
     N --> |Doesn't make sense to put it there| P
     O --> |Doesn't make sense to put it there|P
 ```
 </div>
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.7 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.8 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
-Parks Author-email: Dane@daneparks.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License Classifier: Environment ::
-Console :: Curses Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE # CivilPy Code snippets for Civil Engineering related
-tasks ## About (Skip to the "Installation" section to start running code)
-Welcome to the CivilPy repository. This program is a simple terminal based
-software package to give users easier access to some of the packages from the
-python repository. The package is focused on civil engineering related tasks
-such as file management, pdf data extraction, image manipulation mapping and
-unit conversions. I did my best to make the user interface obvious to use and
-tried to keep the functionality compatible with tools available to the average
-Civil engineer. ## Intro This repository was created in order for me to gain a
-better understanding of software development work flows and how they can be re-
+Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
+MIT License Classifier: Environment :: Console :: Curses Description-Content-
+Type: text/markdown Provides-Extra: dev License-File: LICENSE # CivilPy Code
+snippets for Civil Engineering related tasks ## About (Skip to the
+"Installation" section to start running code) Welcome to the CivilPy
+repository. This program is a simple terminal based software package to give
+users easier access to some of the packages from the python repository. The
+package is focused on civil engineering related tasks such as file management,
+pdf data extraction, image manipulation mapping and unit conversions. I did my
+best to make the user interface obvious to use and tried to keep the
+functionality compatible with tools available to the average Civil engineer. ##
+Intro This repository was created in order for me to gain a better
+understanding of software development work flows and how they can be re-
 purposed for civil engineering related tasks. This is by no means a
 comprehensive or even functional repository but is more a way for me to track
 my progress while learning more about another industry. There may occasionally
 be how-tos and other code posted here but this repository is not meant as
 tutorial or in depth explanation for how coding works. For those types of
 things I highly suggest you instead check Youtube for general lessons or Stack
 Overflow for specific issues. I highly recommend the Harvard_CS50_Youtube
```

### Comparing `civilpy-0.0.7/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.8/civilpy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 civilpy.egg-info/dependency_links.txt
 civilpy.egg-info/requires.txt
 civilpy.egg-info/top_level.txt
 civilpy/construction/__init__.py
 civilpy/environmental/__init__.py
 civilpy/general/__init__.py
 civilpy/general/cli.py
+civilpy/general/database_tools.py
 civilpy/general/gis.py
 civilpy/general/kml_tools.py
 civilpy/general/math.py
 civilpy/general/pdf.py
 civilpy/general/physics.py
 civilpy/general/plan_development.py
 civilpy/general/tello_drone.py
```

### Comparing `civilpy-0.0.7/setup.py` & `civilpy-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.7',
+    version='0.0.8',
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     py_modules=['civilpy', 'civilpy.state.ohio'],
     package_dir={'civilpy': 'civilpy'},
     packages=[
@@ -32,17 +32,26 @@
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "numpy>=1.22.3",
         "folium>=0.12.1",
         "pandas>=1.4.2",
-        "Pillow>=9.1.0",
+        "Pillow>=9.4.0",
         "Pint>=0.19.2",
+        "jupyter>=1.0.0",
+        "Flask>=2.2.2",
+        "PyPDF2>=3.0.1",
+        "simplekml>=1.3.6",
+        "beautifulsoup4>=4.11.1",
+        "psycopg2>=2.9.5",
+        "sshtunnel>=0.4.0",
+        "icalendar>=4.0.7"
     ],
-    extras_require = {
+
+    extras_require={
         "dev": [
             "pytest>=3.7",
             "jupyter>=1.0.0",
         ]
     }
 )
```

