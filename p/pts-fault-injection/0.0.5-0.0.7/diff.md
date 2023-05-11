# Comparing `tmp/pts_fault_injection-0.0.5.tar.gz` & `tmp/pts_fault_injection-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_fault_injection-0.0.5.tar", last modified: Tue Apr 25 13:18:11 2023, max compression
+gzip compressed data, was "dist/pts_fault_injection-0.0.7.tar", last modified: Thu May 11 10:39:50 2023, max compression
```

## Comparing `pts_fault_injection-0.0.5.tar` & `pts_fault_injection-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3470 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3083 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/fault_injection_box.py
--rw-rw-rw-   0 root         (0) root         (0)     8385 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/signal_card_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7764 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/CANFWupdate.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/pts_fault_injection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/pts_fault_injection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/pts_fault_injection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/pts_fault_injection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/pts_fault_injection.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/pts_fault_injection.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/pts_fault_injection/
+-rw-rw-rw-   0 root         (0) root         (0)    23696 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/pts_fault_injection/fib_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     6146 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/pts_fault_injection/cmb_box.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/pts_fault_injection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6176 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/pts_fault_injection/load_box.py
+-rw-rw-rw-   0 root         (0) root         (0)     7764 2023-05-11 10:39:39.000000 pts_fault_injection-0.0.7/pts_fault_injection/CANFWupdate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 10:39:50.000000 pts_fault_injection-0.0.7/setup.cfg
```

### Comparing `pts_fault_injection-0.0.5/PKG-INFO` & `pts_fault_injection-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_fault_injection
-Version: 0.0.5
+Version: 0.0.7
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.5/setup.py` & `pts_fault_injection-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_fault_injection",
-    version="0.0.5",
+    version="0.0.7",
     author="Pass testing Solutions GmbH",
     description="Fault Injection box Diagnostics package Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/pts-fault-injection-box",
     license="MIT",
```

### Comparing `pts_fault_injection-0.0.5/pts_fault_injection.egg-info/PKG-INFO` & `pts_fault_injection-0.0.7/pts_fault_injection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-fault-injection
-Version: 0.0.5
+Version: 0.0.7
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.5/LICENSE.txt` & `pts_fault_injection-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.5/README.md` & `pts_fault_injection-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.5/pts_fault_injection/CANFWupdate.py` & `pts_fault_injection-0.0.7/pts_fault_injection/CANFWupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 ####### Setup Script#######
 ###########################
 # Set to True if you want to create a logfile
 create_log_file = False
 
 # Configure PEAK CAN interface PCAN Mac library has to be installed
 can.rc['interface'] = 'pcan'
-can.rc['channel'] = 'PCAN_USBBUS2'
+can.rc['channel'] = 'PCAN_USBBUS1'
 can.rc['bitrate'] = 500000
 bus = can.interface.Bus()
 
 # Setup Can filters for safe interaction and flush buffer
 bus.flush_tx_buffer()
 filters = [{'can_mask': 0x700, 'can_id': 0x600}]
 bus.set_filters(filters)
```

