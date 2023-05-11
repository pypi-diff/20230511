# Comparing `tmp/daskcheck-0.0.7.tar.gz` & `tmp/daskcheck-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daskcheck-0.0.7.tar", last modified: Wed May 10 12:35:43 2023, max compression
+gzip compressed data, was "daskcheck-0.0.8.tar", last modified: Thu May 11 11:40:56 2023, max compression
```

## Comparing `daskcheck-0.0.7.tar` & `daskcheck-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.134821 daskcheck-0.0.7/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5451 2023-05-10 12:35:43.134821 daskcheck-0.0.7/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5163 2023-05-10 12:35:41.000000 daskcheck-0.0.7/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.130821 daskcheck-0.0.7/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      853 2023-04-19 07:18:06.000000 daskcheck-0.0.7/bin/daskcheck
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.130821 daskcheck-0.0.7/daskcheck/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6892 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/daskcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1486 2023-05-10 10:26:45.000000 daskcheck-0.0.7/daskcheck/singlemod.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1900 2023-05-10 12:22:07.000000 daskcheck-0.0.7/daskcheck/singlexec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-13 14:22:42.000000 daskcheck-0.0.7/daskcheck/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-05-10 12:35:42.000000 daskcheck-0.0.7/daskcheck/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-10 12:35:43.130821 daskcheck-0.0.7/daskcheck.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5451 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      350 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-05-10 12:35:43.000000 daskcheck-0.0.7/daskcheck.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-05-10 12:35:43.134821 daskcheck-0.0.7/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1168 2023-04-19 07:18:41.000000 daskcheck-0.0.7/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-11 11:40:56.568581 daskcheck-0.0.8/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     6825 2023-05-11 11:40:56.568581 daskcheck-0.0.8/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     6537 2023-05-11 11:40:54.000000 daskcheck-0.0.8/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-11 11:40:56.564581 daskcheck-0.0.8/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      853 2023-04-19 07:18:06.000000 daskcheck-0.0.8/bin/daskcheck
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-11 11:40:56.568581 daskcheck-0.0.8/daskcheck/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-13 14:22:42.000000 daskcheck-0.0.8/daskcheck/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-13 14:22:42.000000 daskcheck-0.0.8/daskcheck/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6892 2023-01-13 14:22:42.000000 daskcheck-0.0.8/daskcheck/daskcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1486 2023-05-10 10:26:45.000000 daskcheck-0.0.8/daskcheck/singlemod.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3348 2023-05-11 11:35:55.000000 daskcheck-0.0.8/daskcheck/singlexec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-13 14:22:42.000000 daskcheck-0.0.8/daskcheck/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-05-11 11:40:56.000000 daskcheck-0.0.8/daskcheck/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-05-11 11:40:56.568581 daskcheck-0.0.8/daskcheck.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     6825 2023-05-11 11:40:56.000000 daskcheck-0.0.8/daskcheck.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      350 2023-05-11 11:40:56.000000 daskcheck-0.0.8/daskcheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-05-11 11:40:56.000000 daskcheck-0.0.8/daskcheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-05-11 11:40:56.000000 daskcheck-0.0.8/daskcheck.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-05-11 11:40:56.000000 daskcheck-0.0.8/daskcheck.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-05-11 11:40:56.568581 daskcheck-0.0.8/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1168 2023-04-19 07:18:41.000000 daskcheck-0.0.8/setup.py
```

### Comparing `daskcheck-0.0.7/PKG-INFO` & `daskcheck-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 2.1
-Name: daskcheck
-Version: 0.0.7
-Summary: Automatically created environment for python package
-Home-page: http://gitlab.com/jaromrax/daskcheck
-Author: jaromrax
-Author-email: jaromrax@gmail.com
-License: GPL2
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 Project daskcheck
 =================
 
-Helping tools for a simple use of the **dask**
+Tools for a more simple use of the **dask**. Dask scheduler is defined
+in `~/.dask_ server` file.
 
-Work in progress...
+*Work is in progress...*
 
 The idea
 --------
 
 1.  define properly the *core function* (*xcorefunc* in the example)
-    with **THE return**
+    with **THE proper return**
 2.  `daskcheck` then will take care about:
+    -   sending the task to the scheduler (but this is natural)
+    -   uploads (python) single-file module to workers (via .upload)
     -   sending the parameters
     -   collecting results and saving them to **local json file**
-    -   *in future* take care about sending scripts...
-    -   *in future* take care about making remote folders with data
-        output...
+    -   *in future* about parsing the local **json** file
+    -   *in future* about sending local (bash) scripts to workers... (?)
+    -   *in future* about managing (worker\'s) folders with data output
+        (if output is too large)...
+
+Files in the repo
+-----------------
 
-Files
------
+It is becoming a bit messy, so for the reference:
 
-  ------------------------------------- ------------------------------
+  ------------------------------------- ----------------------------------------
+  batch~forworker~                      BATCH TEST in remote \~/sand
   bin~daskcheck~.py                     will be main script
   config.py                             module configs
+  conv~json2spectra~.py                 exo~dask~ output conversion to spectra
   daskcheck                             FOLDER
   daskcheck.py                          module OPERATIONS
   dask~resultslog20230510142235~.json   log file
   docextr.py                            attemt to autocreate
   exo~dask~.py                          work on exogam
   f.py                                  resulting autogenerate
   OldLogs                               Previous files
   README.md                             MD
   README.org                            this file
-  runme                                 BATCH TEST in remote \~/sand
-  scheduler                             RUN SCHEDULER
+  run~scheduler~                        RUN SCHEDULER
+  run~syncversions~                     KEEP dasksched-workers in sync
+  run~worker~                           RUN WORKER
   setup.py                              python
   singlemod.py                          remote exec MODULE
   singlexec.py                          remote exec BASH
-  sync~versions~                        keep dasksched sync
   unitname.py                           module attempt
   version.py                            version is here
-  worker                                RUN WORKER
-  ------------------------------------- ------------------------------
+                                        
+  ------------------------------------- ----------------------------------------
 
 Instalation of daskcheck
 ------------------------
 
 ``` {.bash org-language="sh"}
 pip install daskcheck
 ```
 
-Installation of dask
---------------------
+Installation of dask 2023
+-------------------------
 
 See <https://docs.dask.org/en/stable/install.html>
 
 ``` {.bash org-language="sh"}
 pip install "dask[complete]"
 ```
 
 Launching dask scheduler/workers
 --------------------------------
 
 *Pay attention to correct/compatible libraries on different workers*
 
+-   use `run_scheduler`
+-   `run_worker`
+
 ### Environment needed
 
     export PATH=$PATH:$HOME/.local/bin
 
     export PYTHONPATH=$HOME/root/lib/
     export ROOTSYS=$HOME/root
     export PATH=$ROOTSYS/bin:~/bin:$PATH
@@ -130,90 +130,107 @@
 ``` {.bash org-language="sh"}
 dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
 ```
 
 Testing dask
 ------------
 
-*IN DEVELOPMENT... NEW*
-
-This runs (sched and workers are ON) 40x get~cpuinfo~
+Just local run of get~cpuinfo~
 
 ``` {.bash org-language="sh"}
-./daskcheck.py test
+./daskcheck.py loc
 ```
 
-Just local run of get~cpuinfo~
+This runs (scheduler and workers should be running) 40x get~cpuinfo~
 
 ``` {.bash org-language="sh"}
-./daskcheck.py loc
+./daskcheck.py test
 ```
 
-Run single-file module or batch
--------------------------------
+Run single-file - (python) module OR (bash) batch
+-------------------------------------------------
 
 **In progress**
 
-I use importlib to get the module to memory, chdir to \~/dask~sendbox~
-and run main:
-
--   singlemod.py - writes a file
--   singlexec.py - launches ./runme - if not present in (remote)
-    \~/dask~sendbox~, crashes
+I use importlib to get the module to the memory, and sneak it to the
+scheduler, chdir to `/dask_sendbox and run main()` function of the
+single-file-module:
+
+-   singlemod.py - writes a file to (worker\'s) `~/dask_sendbox`
+-   singlexec.py - launches `./runme` - if not present in (worker\'s)
+    `~/dask_sendbox`, it crashes
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py dask singlexec.py  1,3
 ./daskcheck.py dask singlemod.py  11..33
 ```
 
-Monitoring dask
----------------
+Run a (python) function from python code
+----------------------------------------
 
-    xdg-open http://localhost:8787
+*This must be updated...*
 
-Recollection the data from json
--------------------------------
+`exo_dask.py` Contains a working (in the past) example, using `root`.
 
-Usage
------
+This is (or should be) a python code that uses `daskcheck` for sending a
+function.
+
+It is evidently crippled for the moment...
 
 ``` {.python}
 from daskcheck import daskcheck
 
 from fire import Fire
 import time
 import platform
 import datetime as dt
 import json
 
 def main( parlist ):
+    """
+    Initiated by Fire. If one parameter, runs locally with local xcorefunc
+    """
     parameters = daskcheck.prepare_params( parlist )
 
     if type(parameters)==list:
         print("i... viable for DASK ....")
         daskcheck.submit( daskcheck.get_cpu_info , parameters)
+    elif type(parameters)==tuple:
+        print("i... viable for DASK ....")
+        daskcheck.submit( daskcheck.get_cpu_info , parameters)
     else:
         print("i... running only locally")
-        my_results = xcorefunc( 1 , parameters )
+        my_results = xcorefunc( 1 , parameters ) # order = 1, just arbitrary number
         # Write LOG file.
         now = dt.datetime.now()
         stamp = now.strftime("%Y%m%d_%H%M%S")
         with open(f"dask_results_log_{stamp}.json", "w") as fp:
             json.dump( my_results , fp, sort_keys=True, indent='\t', separators=(',', ': '))
     return
 
 def xcorefunc( order, param):
     """
-    Function to be sent to dask server with order# + parameter
+    CORE function to be sent to dask schedule.
+
+    :param order: order number of the call
+    :param param: parameter to be sent
     """
-    import ROOT # I need to avoid breaking pickle
+    import ROOT # *TRICK* I need to import here to avoid breaking pickle
     start_time = time.perf_counter()
 
-    return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" , ni]
+    return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" ]
 
 
 if __name__=="__main__":
     Fire(main)
 
 ```
 
+Monitoring dask
+---------------
+
+    xdg-open http://localhost:8787
+
+Recollection the data from json
+-------------------------------
 
+*to recover...*
```

### Comparing `daskcheck-0.0.7/README.md` & `daskcheck-0.0.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,95 @@
+Metadata-Version: 2.1
+Name: daskcheck
+Version: 0.0.8
+Summary: Automatically created environment for python package
+Home-page: http://gitlab.com/jaromrax/daskcheck
+Author: jaromrax
+Author-email: jaromrax@gmail.com
+License: GPL2
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 Project daskcheck
 =================
 
-Helping tools for a simple use of the **dask**
+Tools for a more simple use of the **dask**. Dask scheduler is defined
+in `~/.dask_ server` file.
 
-Work in progress...
+*Work is in progress...*
 
 The idea
 --------
 
 1.  define properly the *core function* (*xcorefunc* in the example)
-    with **THE return**
+    with **THE proper return**
 2.  `daskcheck` then will take care about:
+    -   sending the task to the scheduler (but this is natural)
+    -   uploads (python) single-file module to workers (via .upload)
     -   sending the parameters
     -   collecting results and saving them to **local json file**
-    -   *in future* take care about sending scripts...
-    -   *in future* take care about making remote folders with data
-        output...
+    -   *in future* about parsing the local **json** file
+    -   *in future* about sending local (bash) scripts to workers... (?)
+    -   *in future* about managing (worker\'s) folders with data output
+        (if output is too large)...
+
+Files in the repo
+-----------------
 
-Files
------
+It is becoming a bit messy, so for the reference:
 
-  ------------------------------------- ------------------------------
+  ------------------------------------- ----------------------------------------
+  batch~forworker~                      BATCH TEST in remote \~/sand
   bin~daskcheck~.py                     will be main script
   config.py                             module configs
+  conv~json2spectra~.py                 exo~dask~ output conversion to spectra
   daskcheck                             FOLDER
   daskcheck.py                          module OPERATIONS
   dask~resultslog20230510142235~.json   log file
   docextr.py                            attemt to autocreate
   exo~dask~.py                          work on exogam
   f.py                                  resulting autogenerate
   OldLogs                               Previous files
   README.md                             MD
   README.org                            this file
-  runme                                 BATCH TEST in remote \~/sand
-  scheduler                             RUN SCHEDULER
+  run~scheduler~                        RUN SCHEDULER
+  run~syncversions~                     KEEP dasksched-workers in sync
+  run~worker~                           RUN WORKER
   setup.py                              python
   singlemod.py                          remote exec MODULE
   singlexec.py                          remote exec BASH
-  sync~versions~                        keep dasksched sync
   unitname.py                           module attempt
   version.py                            version is here
-  worker                                RUN WORKER
-  ------------------------------------- ------------------------------
+                                        
+  ------------------------------------- ----------------------------------------
 
 Instalation of daskcheck
 ------------------------
 
 ``` {.bash org-language="sh"}
 pip install daskcheck
 ```
 
-Installation of dask
---------------------
+Installation of dask 2023
+-------------------------
 
 See <https://docs.dask.org/en/stable/install.html>
 
 ``` {.bash org-language="sh"}
 pip install "dask[complete]"
 ```
 
 Launching dask scheduler/workers
 --------------------------------
 
 *Pay attention to correct/compatible libraries on different workers*
 
+-   use `run_scheduler`
+-   `run_worker`
+
 ### Environment needed
 
     export PATH=$PATH:$HOME/.local/bin
 
     export PYTHONPATH=$HOME/root/lib/
     export ROOTSYS=$HOME/root
     export PATH=$ROOTSYS/bin:~/bin:$PATH
@@ -119,88 +141,109 @@
 ``` {.bash org-language="sh"}
 dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
 ```
 
 Testing dask
 ------------
 
-*IN DEVELOPMENT... NEW*
-
-This runs (sched and workers are ON) 40x get~cpuinfo~
+Just local run of get~cpuinfo~
 
 ``` {.bash org-language="sh"}
-./daskcheck.py test
+./daskcheck.py loc
 ```
 
-Just local run of get~cpuinfo~
+This runs (scheduler and workers should be running) 40x get~cpuinfo~
 
 ``` {.bash org-language="sh"}
-./daskcheck.py loc
+./daskcheck.py test
 ```
 
-Run single-file module or batch
--------------------------------
+Run single-file - (python) module OR (bash) batch
+-------------------------------------------------
 
 **In progress**
 
-I use importlib to get the module to memory, chdir to \~/dask~sendbox~
-and run main:
-
--   singlemod.py - writes a file
--   singlexec.py - launches ./runme - if not present in (remote)
-    \~/dask~sendbox~, crashes
+I use importlib to get the module to the memory, and sneak it to the
+scheduler, chdir to `/dask_sendbox and run main()` function of the
+single-file-module:
+
+-   singlemod.py - writes a file to (worker\'s) `~/dask_sendbox`
+-   singlexec.py - launches `./runme` - if not present in (worker\'s)
+    `~/dask_sendbox`, it crashes
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py dask singlexec.py  1,3
 ./daskcheck.py dask singlemod.py  11..33
 ```
 
-Monitoring dask
----------------
+Run a (python) function from python code
+----------------------------------------
 
-    xdg-open http://localhost:8787
+*This must be updated...*
 
-Recollection the data from json
--------------------------------
+`exo_dask.py` Contains a working (in the past) example, using `root`.
 
-Usage
------
+This is (or should be) a python code that uses `daskcheck` for sending a
+function.
+
+It is evidently crippled for the moment...
 
 ``` {.python}
 from daskcheck import daskcheck
 
 from fire import Fire
 import time
 import platform
 import datetime as dt
 import json
 
 def main( parlist ):
+    """
+    Initiated by Fire. If one parameter, runs locally with local xcorefunc
+    """
     parameters = daskcheck.prepare_params( parlist )
 
     if type(parameters)==list:
         print("i... viable for DASK ....")
         daskcheck.submit( daskcheck.get_cpu_info , parameters)
+    elif type(parameters)==tuple:
+        print("i... viable for DASK ....")
+        daskcheck.submit( daskcheck.get_cpu_info , parameters)
     else:
         print("i... running only locally")
-        my_results = xcorefunc( 1 , parameters )
+        my_results = xcorefunc( 1 , parameters ) # order = 1, just arbitrary number
         # Write LOG file.
         now = dt.datetime.now()
         stamp = now.strftime("%Y%m%d_%H%M%S")
         with open(f"dask_results_log_{stamp}.json", "w") as fp:
             json.dump( my_results , fp, sort_keys=True, indent='\t', separators=(',', ': '))
     return
 
 def xcorefunc( order, param):
     """
-    Function to be sent to dask server with order# + parameter
+    CORE function to be sent to dask schedule.
+
+    :param order: order number of the call
+    :param param: parameter to be sent
     """
-    import ROOT # I need to avoid breaking pickle
+    import ROOT # *TRICK* I need to import here to avoid breaking pickle
     start_time = time.perf_counter()
 
-    return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" , ni]
+    return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" ]
 
 
 if __name__=="__main__":
     Fire(main)
 
 ```
+
+Monitoring dask
+---------------
+
+    xdg-open http://localhost:8787
+
+Recollection the data from json
+-------------------------------
+
+*to recover...*
+
+
```

### Comparing `daskcheck-0.0.7/bin/daskcheck` & `daskcheck-0.0.8/bin/daskcheck`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.7/daskcheck/config.py` & `daskcheck-0.0.8/daskcheck/config.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.7/daskcheck/daskcheck.py` & `daskcheck-0.0.8/daskcheck/daskcheck.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.7/daskcheck/singlemod.py` & `daskcheck-0.0.8/daskcheck/singlemod.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.7/daskcheck/unitname.py` & `daskcheck-0.0.8/daskcheck/unitname.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.7/daskcheck.egg-info/PKG-INFO` & `daskcheck-0.0.8/daskcheck.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,95 @@
 Metadata-Version: 2.1
 Name: daskcheck
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automatically created environment for python package
 Home-page: http://gitlab.com/jaromrax/daskcheck
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project daskcheck
 =================
 
-Helping tools for a simple use of the **dask**
+Tools for a more simple use of the **dask**. Dask scheduler is defined
+in `~/.dask_ server` file.
 
-Work in progress...
+*Work is in progress...*
 
 The idea
 --------
 
 1.  define properly the *core function* (*xcorefunc* in the example)
-    with **THE return**
+    with **THE proper return**
 2.  `daskcheck` then will take care about:
+    -   sending the task to the scheduler (but this is natural)
+    -   uploads (python) single-file module to workers (via .upload)
     -   sending the parameters
     -   collecting results and saving them to **local json file**
-    -   *in future* take care about sending scripts...
-    -   *in future* take care about making remote folders with data
-        output...
+    -   *in future* about parsing the local **json** file
+    -   *in future* about sending local (bash) scripts to workers... (?)
+    -   *in future* about managing (worker\'s) folders with data output
+        (if output is too large)...
 
-Files
------
+Files in the repo
+-----------------
 
-  ------------------------------------- ------------------------------
+It is becoming a bit messy, so for the reference:
+
+  ------------------------------------- ----------------------------------------
+  batch~forworker~                      BATCH TEST in remote \~/sand
   bin~daskcheck~.py                     will be main script
   config.py                             module configs
+  conv~json2spectra~.py                 exo~dask~ output conversion to spectra
   daskcheck                             FOLDER
   daskcheck.py                          module OPERATIONS
   dask~resultslog20230510142235~.json   log file
   docextr.py                            attemt to autocreate
   exo~dask~.py                          work on exogam
   f.py                                  resulting autogenerate
   OldLogs                               Previous files
   README.md                             MD
   README.org                            this file
-  runme                                 BATCH TEST in remote \~/sand
-  scheduler                             RUN SCHEDULER
+  run~scheduler~                        RUN SCHEDULER
+  run~syncversions~                     KEEP dasksched-workers in sync
+  run~worker~                           RUN WORKER
   setup.py                              python
   singlemod.py                          remote exec MODULE
   singlexec.py                          remote exec BASH
-  sync~versions~                        keep dasksched sync
   unitname.py                           module attempt
   version.py                            version is here
-  worker                                RUN WORKER
-  ------------------------------------- ------------------------------
+                                        
+  ------------------------------------- ----------------------------------------
 
 Instalation of daskcheck
 ------------------------
 
 ``` {.bash org-language="sh"}
 pip install daskcheck
 ```
 
-Installation of dask
---------------------
+Installation of dask 2023
+-------------------------
 
 See <https://docs.dask.org/en/stable/install.html>
 
 ``` {.bash org-language="sh"}
 pip install "dask[complete]"
 ```
 
 Launching dask scheduler/workers
 --------------------------------
 
 *Pay attention to correct/compatible libraries on different workers*
 
+-   use `run_scheduler`
+-   `run_worker`
+
 ### Environment needed
 
     export PATH=$PATH:$HOME/.local/bin
 
     export PYTHONPATH=$HOME/root/lib/
     export ROOTSYS=$HOME/root
     export PATH=$ROOTSYS/bin:~/bin:$PATH
@@ -130,90 +141,109 @@
 ``` {.bash org-language="sh"}
 dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
 ```
 
 Testing dask
 ------------
 
-*IN DEVELOPMENT... NEW*
-
-This runs (sched and workers are ON) 40x get~cpuinfo~
+Just local run of get~cpuinfo~
 
 ``` {.bash org-language="sh"}
-./daskcheck.py test
+./daskcheck.py loc
 ```
 
-Just local run of get~cpuinfo~
+This runs (scheduler and workers should be running) 40x get~cpuinfo~
 
 ``` {.bash org-language="sh"}
-./daskcheck.py loc
+./daskcheck.py test
 ```
 
-Run single-file module or batch
--------------------------------
+Run single-file - (python) module OR (bash) batch
+-------------------------------------------------
 
 **In progress**
 
-I use importlib to get the module to memory, chdir to \~/dask~sendbox~
-and run main:
-
--   singlemod.py - writes a file
--   singlexec.py - launches ./runme - if not present in (remote)
-    \~/dask~sendbox~, crashes
+I use importlib to get the module to the memory, and sneak it to the
+scheduler, chdir to `/dask_sendbox and run main()` function of the
+single-file-module:
+
+-   singlemod.py - writes a file to (worker\'s) `~/dask_sendbox`
+-   singlexec.py - launches `./runme` - if not present in (worker\'s)
+    `~/dask_sendbox`, it crashes
 
 ``` {.bash org-language="sh"}
 ./daskcheck.py dask singlexec.py  1,3
 ./daskcheck.py dask singlemod.py  11..33
 ```
 
-Monitoring dask
----------------
+Run a (python) function from python code
+----------------------------------------
 
-    xdg-open http://localhost:8787
+*This must be updated...*
 
-Recollection the data from json
--------------------------------
+`exo_dask.py` Contains a working (in the past) example, using `root`.
 
-Usage
------
+This is (or should be) a python code that uses `daskcheck` for sending a
+function.
+
+It is evidently crippled for the moment...
 
 ``` {.python}
 from daskcheck import daskcheck
 
 from fire import Fire
 import time
 import platform
 import datetime as dt
 import json
 
 def main( parlist ):
+    """
+    Initiated by Fire. If one parameter, runs locally with local xcorefunc
+    """
     parameters = daskcheck.prepare_params( parlist )
 
     if type(parameters)==list:
         print("i... viable for DASK ....")
         daskcheck.submit( daskcheck.get_cpu_info , parameters)
+    elif type(parameters)==tuple:
+        print("i... viable for DASK ....")
+        daskcheck.submit( daskcheck.get_cpu_info , parameters)
     else:
         print("i... running only locally")
-        my_results = xcorefunc( 1 , parameters )
+        my_results = xcorefunc( 1 , parameters ) # order = 1, just arbitrary number
         # Write LOG file.
         now = dt.datetime.now()
         stamp = now.strftime("%Y%m%d_%H%M%S")
         with open(f"dask_results_log_{stamp}.json", "w") as fp:
             json.dump( my_results , fp, sort_keys=True, indent='\t', separators=(',', ': '))
     return
 
 def xcorefunc( order, param):
     """
-    Function to be sent to dask server with order# + parameter
+    CORE function to be sent to dask schedule.
+
+    :param order: order number of the call
+    :param param: parameter to be sent
     """
-    import ROOT # I need to avoid breaking pickle
+    import ROOT # *TRICK* I need to import here to avoid breaking pickle
     start_time = time.perf_counter()
 
-    return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" , ni]
+    return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" ]
 
 
 if __name__=="__main__":
     Fire(main)
 
 ```
 
+Monitoring dask
+---------------
+
+    xdg-open http://localhost:8787
+
+Recollection the data from json
+-------------------------------
+
+*to recover...*
+
```

### Comparing `daskcheck-0.0.7/setup.py` & `daskcheck-0.0.8/setup.py`

 * *Files identical despite different names*

