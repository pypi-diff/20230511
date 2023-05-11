# Comparing `tmp/daskcheck-0.0.5.tar.gz` & `tmp/daskcheck-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daskcheck-0.0.5.tar", last modified: Wed Apr 19 07:18:56 2023, max compression
+gzip compressed data, was "daskcheck-0.0.7.tar", last modified: Wed May 10 12:35:43 2023, max compression
```

## Comparing `daskcheck-0.0.5.tar` & `daskcheck-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.333319 daskcheck-0.0.5/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3799 2023-04-19 07:18:56.333319 daskcheck-0.0.5/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3511 2023-04-19 07:18:53.000000 daskcheck-0.0.5/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.329319 daskcheck-0.0.5/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      853 2023-04-19 07:18:06.000000 daskcheck-0.0.5/bin/daskcheck
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.333319 daskcheck-0.0.5/daskcheck/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6892 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/daskcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-13 14:22:42.000000 daskcheck-0.0.5/daskcheck/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-19 07:18:56.333319 daskcheck-0.0.5/daskcheck.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3799 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      304 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-19 07:18:56.000000 daskcheck-0.0.5/daskcheck.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-19 07:18:56.333319 daskcheck-0.0.5/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1168 2023-04-19 07:18:41.000000 daskcheck-0.0.5/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.134821 daskcheck-0.0.7/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5451 2023-05-10 12:35:43.134821 daskcheck-0.0.7/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5163 2023-05-10 12:35:41.000000 daskcheck-0.0.7/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.130821 daskcheck-0.0.7/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      853 2023-04-19 07:18:06.000000 daskcheck-0.0.7/bin/daskcheck
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.130821 daskcheck-0.0.7/daskcheck/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6892 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/daskcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1486 2023-05-10 10:26:45.000000 daskcheck-0.0.7/daskcheck/singlemod.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1900 2023-05-10 12:22:07.000000 daskcheck-0.0.7/daskcheck/singlexec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-05-10 12:35:42.000000 daskcheck-0.0.7/daskcheck/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.130821 daskcheck-0.0.7/daskcheck.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5451 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      350 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-05-10 12:35:43.134821 daskcheck-0.0.7/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1168 2023-04-19 07:18:41.000000 daskcheck-0.0.7/setup.py
```

### Comparing `daskcheck-0.0.5/PKG-INFO` & `daskcheck-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,62 @@
 Metadata-Version: 2.1
 Name: daskcheck
-Version: 0.0.5
+Version: 0.0.7
 Summary: Automatically created environment for python package
 Home-page: http://gitlab.com/jaromrax/daskcheck
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project daskcheck
 =================
 
-Help with a simple use of the **dask**
+Helping tools for a simple use of the **dask**
+
+Work in progress...
 
 The idea
 --------
 
 1.  define properly the *core function* (*xcorefunc* in the example)
     with **THE return**
 2.  `daskcheck` then will take care about:
     -   sending the parameters
     -   collecting results and saving them to **local json file**
+    -   *in future* take care about sending scripts...
+    -   *in future* take care about making remote folders with data
+        output...
+
+Files
+-----
+
+  ------------------------------------- ------------------------------
+  bin~daskcheck~.py                     will be main script
+  config.py                             module configs
+  daskcheck                             FOLDER
+  daskcheck.py                          module OPERATIONS
+  dask~resultslog20230510142235~.json   log file
+  docextr.py                            attemt to autocreate
+  exo~dask~.py                          work on exogam
+  f.py                                  resulting autogenerate
+  OldLogs                               Previous files
+  README.md                             MD
+  README.org                            this file
+  runme                                 BATCH TEST in remote \~/sand
+  scheduler                             RUN SCHEDULER
+  setup.py                              python
+  singlemod.py                          remote exec MODULE
+  singlexec.py                          remote exec BASH
+  sync~versions~                        keep dasksched sync
+  unitname.py                           module attempt
+  version.py                            version is here
+  worker                                RUN WORKER
+  ------------------------------------- ------------------------------
 
 Instalation of daskcheck
 ------------------------
 
 ``` {.bash org-language="sh"}
 pip install daskcheck
 ```
@@ -99,30 +130,43 @@
 ``` {.bash org-language="sh"}
 dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
 ```
 
 Testing dask
 ------------
 
-*IN DEVELOPMENT...*
+*IN DEVELOPMENT... NEW*
 
 This runs (sched and workers are ON) 40x get~cpuinfo~
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py test
 ```
 
-**In progress ... this worked only inside git project folder with actual
-files...**
+Just local run of get~cpuinfo~
+
+``` {.bash org-language="sh"}
+./daskcheck.py loc
+```
+
+Run single-file module or batch
+-------------------------------
+
+**In progress**
+
+I use importlib to get the module to memory, chdir to \~/dask~sendbox~
+and run main:
 
-This is solved .... possible to load (unload first). See `tesmod.py`
+-   singlemod.py - writes a file
+-   singlexec.py - launches ./runme - if not present in (remote)
+    \~/dask~sendbox~, crashes
 
 ``` {.bash org-language="sh"}
-./daskcheck.py dask py_file_with_main  1,3
-./daskcheck.py dask py_file_with_main  11..33
+./daskcheck.py dask singlexec.py  1,3
+./daskcheck.py dask singlemod.py  11..33
 ```
 
 Monitoring dask
 ---------------
 
     xdg-open http://localhost:8787
```

### Comparing `daskcheck-0.0.5/bin/daskcheck` & `daskcheck-0.0.7/bin/daskcheck`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.5/daskcheck/config.py` & `daskcheck-0.0.7/daskcheck/config.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.5/daskcheck/daskcheck.py` & `daskcheck-0.0.7/daskcheck/daskcheck.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.5/daskcheck/unitname.py` & `daskcheck-0.0.7/daskcheck/unitname.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.5/daskcheck.egg-info/PKG-INFO` & `daskcheck-0.0.7/daskcheck.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,62 @@
 Metadata-Version: 2.1
 Name: daskcheck
-Version: 0.0.5
+Version: 0.0.7
 Summary: Automatically created environment for python package
 Home-page: http://gitlab.com/jaromrax/daskcheck
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project daskcheck
 =================
 
-Help with a simple use of the **dask**
+Helping tools for a simple use of the **dask**
+
+Work in progress...
 
 The idea
 --------
 
 1.  define properly the *core function* (*xcorefunc* in the example)
     with **THE return**
 2.  `daskcheck` then will take care about:
     -   sending the parameters
     -   collecting results and saving them to **local json file**
+    -   *in future* take care about sending scripts...
+    -   *in future* take care about making remote folders with data
+        output...
+
+Files
+-----
+
+  ------------------------------------- ------------------------------
+  bin~daskcheck~.py                     will be main script
+  config.py                             module configs
+  daskcheck                             FOLDER
+  daskcheck.py                          module OPERATIONS
+  dask~resultslog20230510142235~.json   log file
+  docextr.py                            attemt to autocreate
+  exo~dask~.py                          work on exogam
+  f.py                                  resulting autogenerate
+  OldLogs                               Previous files
+  README.md                             MD
+  README.org                            this file
+  runme                                 BATCH TEST in remote \~/sand
+  scheduler                             RUN SCHEDULER
+  setup.py                              python
+  singlemod.py                          remote exec MODULE
+  singlexec.py                          remote exec BASH
+  sync~versions~                        keep dasksched sync
+  unitname.py                           module attempt
+  version.py                            version is here
+  worker                                RUN WORKER
+  ------------------------------------- ------------------------------
 
 Instalation of daskcheck
 ------------------------
 
 ``` {.bash org-language="sh"}
 pip install daskcheck
 ```
@@ -99,30 +130,43 @@
 ``` {.bash org-language="sh"}
 dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
 ```
 
 Testing dask
 ------------
 
-*IN DEVELOPMENT...*
+*IN DEVELOPMENT... NEW*
 
 This runs (sched and workers are ON) 40x get~cpuinfo~
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py test
 ```
 
-**In progress ... this worked only inside git project folder with actual
-files...**
+Just local run of get~cpuinfo~
+
+``` {.bash org-language="sh"}
+./daskcheck.py loc
+```
+
+Run single-file module or batch
+-------------------------------
+
+**In progress**
+
+I use importlib to get the module to memory, chdir to \~/dask~sendbox~
+and run main:
 
-This is solved .... possible to load (unload first). See `tesmod.py`
+-   singlemod.py - writes a file
+-   singlexec.py - launches ./runme - if not present in (remote)
+    \~/dask~sendbox~, crashes
 
 ``` {.bash org-language="sh"}
-./daskcheck.py dask py_file_with_main  1,3
-./daskcheck.py dask py_file_with_main  11..33
+./daskcheck.py dask singlexec.py  1,3
+./daskcheck.py dask singlemod.py  11..33
 ```
 
 Monitoring dask
 ---------------
 
     xdg-open http://localhost:8787
```

### Comparing `daskcheck-0.0.5/setup.py` & `daskcheck-0.0.7/setup.py`

 * *Files identical despite different names*

