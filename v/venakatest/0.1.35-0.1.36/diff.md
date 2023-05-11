# Comparing `tmp/venakatest-0.1.35.tar.gz` & `tmp/venakatest-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venakatest-0.1.35.tar", last modified: Tue May  9 04:20:43 2023, max compression
+gzip compressed data, was "venakatest-0.1.36.tar", last modified: Thu May 11 10:41:36 2023, max compression
```

## Comparing `venakatest-0.1.35.tar` & `venakatest-0.1.36.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 04:20:43.236433 venakatest-0.1.35/
--rw-rw-rw-   0        0        0       94 2023-05-09 04:20:43.235433 venakatest-0.1.35/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.35/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 04:20:43.236433 venakatest-0.1.35/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-05-09 04:20:30.000000 venakatest-0.1.35/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 04:20:43.219432 venakatest-0.1.35/venakatest/
--rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.35/venakatest/__init__.py
--rw-rw-rw-   0        0        0     2032 2023-05-09 04:20:26.000000 venakatest-0.1.35/venakatest/test.py
-drwxrwxrwx   0        0        0        0 2023-05-09 04:20:43.234433 venakatest-0.1.35/venakatest.egg-info/
--rw-rw-rw-   0        0        0       94 2023-05-09 04:20:43.000000 venakatest-0.1.35/venakatest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-09 04:20:43.000000 venakatest-0.1.35/venakatest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 04:20:43.000000 venakatest-0.1.35/venakatest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-09 04:20:43.000000 venakatest-0.1.35/venakatest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 04:20:43.000000 venakatest-0.1.35/venakatest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 04:20:43.000000 venakatest-0.1.35/venakatest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 10:41:36.376546 venakatest-0.1.36/
+-rw-rw-rw-   0        0        0       94 2023-05-11 10:41:36.375546 venakatest-0.1.36/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-20 09:43:51.000000 venakatest-0.1.36/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 10:41:36.377546 venakatest-0.1.36/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-05-11 10:39:49.000000 venakatest-0.1.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:41:36.326549 venakatest-0.1.36/venakatest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 03:17:15.000000 venakatest-0.1.36/venakatest/__init__.py
+-rw-rw-rw-   0        0        0     2473 2023-05-11 10:39:33.000000 venakatest-0.1.36/venakatest/test.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:41:36.371548 venakatest-0.1.36/venakatest.egg-info/
+-rw-rw-rw-   0        0        0       94 2023-05-11 10:41:36.000000 venakatest-0.1.36/venakatest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-11 10:41:36.000000 venakatest-0.1.36/venakatest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 10:41:36.000000 venakatest-0.1.36/venakatest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-11 10:41:36.000000 venakatest-0.1.36/venakatest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-11 10:41:36.000000 venakatest-0.1.36/venakatest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-11 10:41:36.000000 venakatest-0.1.36/venakatest.egg-info/top_level.txt
```

### Comparing `venakatest-0.1.35/venakatest/test.py` & `venakatest-0.1.36/venakatest/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,29 +16,40 @@
 batch_executable = 'cmd.exe'
 powershell_executable = 'powershell.exe'
 def testing():
     return "ok"
 def exception_handler(type, value, tb):
     logging.exception("Uncaught exception: {0} {1} - Line : {2} ".format(str(value), str(type),str(tb.tb_lineno)))
 logging.basicConfig(level=logging.DEBUG)
-def check():
+def check1():
     print(os.path.basename(sys.executable))
     print(os.environ.get('COMSPEC', ''))
         # Additional batch-specific code here
     if os.environ.get('COMSPEC', '').endswith('cmd.exe') and not os.path.basename(sys.executable) == 'powershell.exe':
         print("Running from batch")
         logging.exception("Running from a batch file")
         # Additional PowerShell-specific code here
     elif 'MyInvocation' in str(globals().get('Get-Variable')) and os.path.basename(sys.executable) == 'powershell.exe':
         logging.exception("Running from a powershell file")
         print("Running directly from powershell")
     else:
         logging.exception("Running from python file")
 
         print("Running from a python file")
+def check():
+    interpreter = sys.executable.lower()
+    print(interpreter)
+    if 'python.exe' in interpreter:
+        print("Command is being run from Python.")
+    elif 'powershell.exe' in interpreter:
+        print("Command is being run from PowerShell.")
+    elif 'cmd.exe' in interpreter:
+        print("Command is being run from CMD (Batch).")
+    else:
+        print("Command is being run from an unknown interpreter.")
     # Code to handle other cases
 
 # Install exception handler
 sys.excepthook = exception_handler
 
 def tobe():
     logging.info('Started syncing commits to {}'.format("testubg"))
```

