# Comparing `tmp/cheap_pie-0.1.17.tar.gz` & `tmp/cheap_pie-0.9.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-0.1.17.tar", last modified: Fri May  5 18:22:39 2023, max compression
+gzip compressed data, was "cheap_pie-0.9.18.tar", last modified: Thu May 11 06:08:09 2023, max compression
```

## Comparing `cheap_pie-0.1.17.tar` & `cheap_pie-0.9.18.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.770849 cheap_pie-0.1.17/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.1.17/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-05 18:22:39.771406 cheap_pie-0.1.17/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7746 2023-05-05 18:19:03.000000 cheap_pie-0.1.17/README.md
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-05 18:22:39.772809 cheap_pie-0.1.17/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)      808 2023-05-05 18:21:58.000000 cheap_pie-0.1.17/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.672416 cheap_pie-0.1.17/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.683720 cheap_pie-0.1.17/src/cheap_pie/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/__init__.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.715144 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7755 2023-05-04 20:02:54.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2259 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cheap_pie.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2736 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1694 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5636 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     9105 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2235 2022-12-12 23:16:24.000000 cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.737000 cheap_pie-0.1.17/src/cheap_pie/parsers/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1809 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3934 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3518 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      315 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/name_subs.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      910 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4016 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4068 2023-05-04 19:52:33.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.752882 cheap_pie-0.1.17/src/cheap_pie/tools/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       40 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.1.17/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/rdl2verilog.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/reload_module.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2275 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/search.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/tools/test_rdl.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.768229 cheap_pie-0.1.17/src/cheap_pie/transport/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4811 2022-12-12 23:20:40.000000 cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-05 18:22:39.694728 cheap_pie-0.1.17/src/cheap_pie.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      139 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-05 18:22:39.000000 cheap_pie-0.1.17/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.291383 cheap_pie-0.9.18/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.9.18/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 06:08:09.291718 cheap_pie-0.9.18/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7746 2023-05-05 18:19:03.000000 cheap_pie-0.9.18/README.md
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-11 06:08:09.292769 cheap_pie-0.9.18/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1071 2023-05-11 05:59:04.000000 cheap_pie-0.9.18/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.220646 cheap_pie-0.9.18/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.232795 cheap_pie-0.9.18/src/cheap_pie/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/__init__.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.252300 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7394 2023-05-06 21:35:32.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2205 2023-05-05 19:38:54.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cheap_pie.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2873 2023-05-05 19:42:59.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2092 2023-05-05 19:46:51.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     6282 2023-05-07 08:06:02.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8909 2023-05-07 08:47:20.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2534 2023-05-11 05:47:26.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.272649 cheap_pie-0.9.18/src/cheap_pie/parsers/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2088 2023-05-07 09:34:36.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3989 2023-05-07 09:06:44.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3294 2023-05-07 08:41:29.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      430 2023-05-07 09:09:07.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/name_subs.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1026 2023-05-07 09:10:56.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4091 2023-05-07 09:33:12.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4134 2023-05-07 09:35:26.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.282639 cheap_pie-0.9.18/src/cheap_pie/tools/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       40 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.9.18/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/rdl2verilog.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/reload_module.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2275 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/search.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/test_rdl.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.290274 cheap_pie-0.9.18/src/cheap_pie/transport/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5284 2023-05-06 21:31:25.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.241993 cheap_pie-0.9.18/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      101 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-0.1.17/LICENSE` & `cheap_pie-0.9.18/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/README.md` & `cheap_pie-0.9.18/README.md`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/setup.py` & `cheap_pie-0.9.18/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,40 @@
+""" Pypi setup for cheap_pie """
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='0.1.17',
+    version='0.9.18',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
     url='https://github.com/bat52/cheap_pie',
     keywords='python silicon validation',
     install_requires=[
           'untangle',
+          'hickle',
+          # parsers
           'cmsis-svd',
           'ipyxact',
-          'pylink-square',
-          'pyocd',
-          'esptool',
           'python-docx',
           'pyverilator',
           'peakrdl-ipxact',
           'peakrdl-uvm',
           'peakrdl-verilog',
-          'hickle',
-          'packaging'
+          # transport layers
+          #'pylink-square',
+          #'pyocd',
+          #'esptool',
+          #'packaging' # for verilator version check
       ],
-)
+)
+
+project_urls={
+    "Source": "https://github.com/bat52/cheap_pie",
+    "Tracker": "https://github.com/bat52/cheap_pie/issues"
+}
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,135 @@
 #!/usr/bin/python3
+"""
+bitfield register class for cheap-pie.
+"""
 #
-# Autogenerated with SMOP 
+# Autogenerated with SMOP
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 from ast import literal_eval
 
-class cp_bitfield:
+class cp_bitfield():
     """A bitfield register class """
-    #properties    
     # field width
-    width = 1    
+    width = 1
+
     # LSB
     lsb = 1
-    
+
     # mask
     mask = 1
-    
+
     # comments
     comments = ""
-    
+
     # Address (Duplicate information)
     addr = 0
-    
+
     # reg name
     regname = ""
-    
+
     # field name
     fieldname = ""
-    
+
     # host interface handler
     hif = None
-    
+
     # read/write
     rw  = "rw"
 
     # reset value
     reset = 0
 
-    def __init__(self, regfield="",regaddr=0, regname="",width="1", bit_offset="0",comments="",hif=None, rw = "rw", reset=0):
+    def __init__(self, regfield="",regaddr=0, regname="", width="1",
+                 bit_offset="0", comments="",hif=None, rw = "rw", reset=0):
 
         if isinstance(width,str):
             width= literal_eval(width)
         # field width
         self.width = int( width )
-        
+
         if isinstance(bit_offset,str):
             lsb=literal_eval(bit_offset)
         else:
             lsb = bit_offset
         self.lsb = int( lsb )
-        
+
         if lsb is None:
-            print('Bad definition for register field %s @ %s!' % regname,regfield)
+            print(f'Bad definition for register field {regname} @ {regfield}!')
             lsb=0
-            
+
         if isinstance(regaddr,str):
             regaddr=literal_eval(regaddr)
-        
+
         # mask
-        # self.mask=bitshift(bin2dec(repmat('1',cat(1,width))),lsb)        
-        bstr = "0b" + ("1" * self.width) + ("0" * self.lsb)        
-        self.mask=literal_eval( bstr )        
+        bstr = "0b" + ("1" * self.width) + ("0" * self.lsb)
+        self.mask=literal_eval( bstr )
         self.comments = comments
         self.addr = int( regaddr )
         self.regname = regname
         self.fieldname = regfield
         self.hif = hif
         self.rw = rw
         self.reset = reset
 
-    def _strval(self,fieldval,width=25):        
-        
-        bitstr = self.fieldname  + ' [' + str(self.width) + '] = ' + hex(fieldval)        
+    def _strval(self,fieldval,width=25):
+        #
+        bitstr = self.fieldname  + ' [' + str(self.width) + '] = ' + hex(fieldval)
 
         if self.width > 1:
             msb = str( self.lsb + self.width - 1)
             regstr = self.regname + '[' + msb + ':' + str(self.lsb) + ']'
         else:
             regstr = self.regname + '[' + str(self.lsb) + ']'
 
-        fmtstr = '%%%ds @ %%%ds' % (width,width)                
-        return fmtstr % (regstr,bitstr)            
-        
+        fmtstr = '%%%ds @ %%%ds' % (width,width)
+        return fmtstr % (regstr,bitstr)
+
     def __repr__(self,regval=None):
-        """ displays value of a bitfield from a register value         
+        """ displays value of a bitfield from a register value
         input : regval value of the full register either in decimal or
         hexadecimal """
-        
+        #
         if regval is None:
-            if not (self.hif is None):
-                regval=self.hif.hifread(self.addr)    
-            else:
+            if self.hif is None:
                 regval=0
-                
+            else:
+                regval=self.hif.hifread(self.addr)
+        #
         # compute field value from register value
         if isinstance(regval, str):
             regval=literal_eval(regval)
         fieldval = (regval & self.mask ) >> (self.lsb)
-        
+
         outstr= self._strval(fieldval)
         # print(outstr)
         return outstr
-    
+
     def display(self,regval=None):
-        r = self.__repr__(regval=regval)
-        print(r)
-        return r
+        """
+        Display the bitfield
+        """
+        print(self)
+        return self
 
     def getbit(self,regval=None,echo=False,as_signed=False,*args,**kwargs):
-        """ function display(self,regval=None,echo=False,as_signed=False)        
-        # displays value of a bitfield from a register value        
+        """ function display(self,regval=None,echo=False,as_signed=False)
+        # displays value of a bitfield from a register value
         # input : regval value of the full register either in decimal or
-                # hexadecimal"""
-        
+        # hexadecimal"""
+        #
         if regval is None:
-            if not (self.hif is None):
-                regval=self.hif.hifread(self.addr)
+            if self.hif is None:
+                regval=0
             else:
-                regval=0        
-        
+                regval=self.hif.hifread(self.addr)
+
         # compute field value from register value
         if isinstance(regval, str):
             regval=literal_eval(regval)
         fieldval = (regval & self.mask ) >> (self.lsb)
 
         # get bitfield as signed value
         if as_signed:
@@ -132,130 +137,126 @@
             fieldmod = (fieldval & (self.mask>>(self.lsb+1)))
             fieldval = fieldsign + fieldmod
 
         # fieldval=self.value(regval)
         if echo:
             outstr= self._strval(fieldval)
             print(outstr)
-        
+        #
         return fieldval
-        
+
     def setbit(self,fieldval=0,echo=False, writeback=True, regval=None,*args,**kwargs):
-        """ function display(self,regval)        
+        """ function display(self,regval)
         # displays value of a bitfield from a register value
-        
         # input : regval value of the full register either in decimal or
-                # hexadecimal """
-    
+        # hexadecimal """
+
         ## read input register value ###################################################
         if not (self.hif is None) and regval is None:
             hexval=self.hif.hifread(self.addr)
             if isinstance(hexval, str):
                 regval=literal_eval(hexval)
             else:
                 regval = hexval
-        
+        #
         ## handle char input as binary #################################################
         if isinstance(fieldval, str):
             fieldval = literal_eval(fieldval)
 
         ## handle negative values ######################################################
         if fieldval < 0:
             fieldval = (abs(fieldval) ^ (self.mask >> self.lsb)) + 1
 
         ## compute new register value ##################################################
-        
+        #
         shiftval= fieldval << self.lsb
         maskinv= self.mask ^ literal_eval('0xFFFFFFFF')
         regmasked = regval & maskinv
         outregval = regmasked + (shiftval & self.mask)
 
         # check new value in range
         if (shiftval & self.mask) < shiftval:
             raise ValueError(f'Bitifield value f{fieldval} out of range!')
-    
+        #
         ## write back new register value ###############################################
         if writeback:
             self.hif.hifwrite(self.addr,outregval,*args,**kwargs)
-        
+        #
         if echo:
             outstr=self._strval(fieldval)
             print(outstr)
-        
+        #
         return outregval
-        
+
     #@function
     def help(self):
-        """ function ret = help(self)        
-        # displays register comments """    
+        """ function ret = help(self)
+        # displays register comments """
         print(self.comments)
 
     #@function
     def value(self,regval=0):
-        """ function ret = value(self,regval)        
-        # Returns value of a bitfield from a register value        
+        """ function ret = value(self,regval)
+        # Returns value of a bitfield from a register value
         # input : regval value of the full register either in decimal or
-                # hexadecimal """
-        
+        # hexadecimal """
+        #
         if isinstance(regval, str):
             regval=literal_eval(regval)
-        
-        # mask = dec2hex(self.mask)
-                # lsb  = self.lsb
-        
-        # ret=bitshift(bitand(regval,self.mask),- (self.lsb))
-        
+        #
         ret = (regval & self.mask ) >> (self.lsb)
         return ret
 
     def __index__(self):
         return int(self.getbit())
-    
+
 def test_cp_bitfield():
+    """
+    Test function for cp_bitfield class
+    """
     import sys
     import os.path
     sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
     from transport.cp_dummy_transport import cp_dummy
 
-    f = cp_bitfield(
+    field = cp_bitfield(
         regfield = 'fname',
         regaddr = 10,
         regname = 'rname',
         width = '2',
         bit_offset = '2',
         comments = 'comment',
         hif = cp_dummy()
     )
 
     val = 3
-    f.setbit(val)
-    assert( f.getbit() == val )
-    f.value()
-    f.display()
-    f.display(2)
-    f.help()
+    field.setbit(val)
+    assert field.getbit() == val
+    field.value()
+    field.display()
+    field.display(2)
+    field.help()
 
     # signed assignement
     negval = -1
-    f.setbit(negval)
-    retval = f.getbit(as_signed=True)
-    assert(negval==retval)
+    field.setbit(negval)
+    retval = field.getbit(as_signed=True)
+    assert negval==retval
 
     # decimal representation
-    print(hex(f))
+    print(hex(field))
 
     # options
-    f.setbit(val,echo=True)
-    f.setbit(val,writeback=False)
-    rv = f.setbit(1,regval=1)
-    assert(rv==5)
+    field.setbit(val,echo=True)
+    field.setbit(val,writeback=False)
+    rv = field.setbit(1,regval=1)
+    assert rv==5
 
     # test assertion
     try:
-        f.setbit(7)
+        field.setbit(7)
         assert False, 'Assertion was not raised!!!'
     except ValueError as error:
-        print('Assertion raised correctly: <%s>' % error)
+        print(f'Assertion raised correctly: <{error}>')
 
 if __name__ == '__main__':
-    test_cp_bitfield()    
-    pass
+    test_cp_bitfield()
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cheap_pie.py` & `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cheap_pie.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 # %reset
 # %run cheap_pie
 
 import os
 import sys
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
+from parsers.cp_parsers_wrapper import cp_parsers_wrapper
 from cheap_pie_core.cp_banner import cp_banner
 from cheap_pie_core.cp_cli import cp_cli
-from parsers.cp_parsers_wrapper import cp_parsers_wrapper
 from cheap_pie_core.cp_hal import cp_hal
 
 def main(argv=[]):
+    """
+    Main cheap_pie function
+    """
     ## banner #######################################################################
     cp_banner()
-    
+    #
     ## input parameters ###########################################################
     print('Parsing input arguments...')
     p = cp_cli(argv)
 
     ## transport hif interface %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     print('Initialising Host Interface...')
 
@@ -39,31 +42,26 @@
         from transport.cp_dummy_transport import cp_dummy
         hif = cp_dummy()
     elif p.transport == 'ocd':
         from transport.cp_pyocd_transport import cp_pyocd
         hif = cp_pyocd(device = p.device )
     elif p.transport == 'esptool':
         from transport.cp_esptool_transport import cp_esptool
-        hif = cp_esptool(port = p.port )   
+        hif = cp_esptool(port = p.port )
     elif p.transport == 'verilator':
         from transport.cp_pyverilator_transport import cp_pyverilator_transport
         hif = cp_pyverilator_transport( p.top_verilog )
     else:
         hif=None
-        # assert(False,'Invalid transport: %s' % p.transport)
-        assert(False)
+        assert False, f'Invalid transport: {p.transport}'
 
     ## init chip ##################################################################
     print('Initialising Hardware Abstraction Layer...')
     hal = cp_hal( cp_parsers_wrapper( p, hif=hif ) )
 
     ## welcome ####################################################################
     print('Cheap Pie is ready! Type hal.<TAB> to start browsing...')
 
     return hal
 
-if __name__ == '__main__':    
-    # global system_root
-    # system_root = os.getcwd()
-
+if __name__ == '__main__':
     hal = main(sys.argv[1:])
-    pass
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,48 @@
 #!/usr/bin/python3
-#
+"""
+Cheap Pie Command Line Interface
+"""
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 import argparse
 import sys
 
 def cp_cli(args=[]):
+    """
+    Cheap Pie Command Line Interface
+    """
     parser = argparse.ArgumentParser(description='Cheap Pie Configuration')
     # register format options
-    parser.add_argument("-rf", "--regfname", help="register description file name", action='store', type = str, default="QN908XC.svd")
-    parser.add_argument("-dd", "--devicedir", help="register description files folder", action='store', type = str, default="./devices")    
-    parser.add_argument("-fmt","--format", help="device description format", action='store', type = str, default="cmsis-svd", choices=["svd","cmsis-svd","ipxact","ipyxact","rdl"])
-    parser.add_argument("-ve", "--vendor", help="device vendor. if specified parses svd file from github repository.", action='store', type = str, default=None)
+    parser.add_argument("-rf", "--regfname", help="register description file name",
+                        action='store', type = str, default="QN908XC.svd")
+    parser.add_argument("-dd", "--devicedir", help="register description files folder",
+                        action='store', type = str, default="./devices")
+    parser.add_argument("-fmt","--format", help="device description format",
+                        action='store', type = str, default="cmsis-svd",
+                        choices=["svd","cmsis-svd","ipxact","ipyxact","rdl"])
+    parser.add_argument("-ve", "--vendor",
+                        help="device vendor. if specified parses svd file from github repository.",
+                        action='store', type = str, default=None)
     # transport options
-    parser.add_argument("-d", "--device", help="jlink/ocd device name", action='store', type = str, default="CORTEX-M4")
-    parser.add_argument("-t" , "--transport", help="transport", action='store', type = str, default="dummy", choices=["jlink","dummy","ocd","esptool","verilator"])
-    parser.add_argument("-p", "--port", help="esptool serial port", action='store', type = str, default="/dev/ttyUSB0")
-    parser.add_argument("-topv", "--top_verilog", help="top verilog file (when simulating with verilator)", action='store', type = str, default="./devices/rdl/basic/basic_rf.sv")
+    parser.add_argument("-d", "--device", help="jlink/ocd device name", action='store',
+                        type = str, default="CORTEX-M4")
+    parser.add_argument("-t" , "--transport", help="transport", action='store', type = str,
+                        default="dummy", choices=["jlink","dummy","ocd","esptool","verilator"])
+    parser.add_argument("-p", "--port", help="esptool serial port", action='store', type = str,
+                        default="/dev/ttyUSB0")
+    parser.add_argument("-topv", "--top_verilog",
+                        help="top verilog file (when simulating with verilator)",
+                        action='store', type = str, default="./devices/rdl/basic/basic_rf.sv")
 
     return parser.parse_args(args)
 
 def test_cli(argv):
+    """
+    Test function for Cheap Pie Command Line Interface
+    """
     return cp_cli(argv)
-    pass
 
-if __name__ == '__main__':    
+if __name__ == '__main__':
     print(test_cli(sys.argv[1:]))
-    pass
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #!/usr/bin/python3
+"""
+Cheap Pie Hardware Abstraction Layer
+"""
 #
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 import sys
@@ -12,188 +15,203 @@
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from transport.cp_dummy_transport import cp_dummy
 import tools.search
 from tools.hal2doc import hal2doc
 
 class cp_hal:
+    """
+    Cheap Pie Hardware Abstraction Layer
+    """
     regs = []
     hif = None
-    """ Hardware abstraction layer class """
+
     def __init__(self,regs):
         self.regs = regs
-        self.hif = regs[0].hif
-        pass
+        if len(regs) > 0:
+            self.hif = regs[0].hif
+        else:
+            print('# WARNING: no register defined!')
 
     def __len__(self):
         return len(self.regs)
 
     def __iter__(self):
         return self.regs.__iter__()
-    
+
     def __next__(self):
         return self.regs.next()
-    
+
     def __getitem__(self, idx):
         if isinstance(idx,int):
             return self.regs[idx]
         elif isinstance(idx,str):
             return self.regs._asdict()[idx]
-        else:
-            print('Unsupported indexing!')
-            assert(False)
-    
+        assert False,'Unsupported indexing!'
+
     def __setitem__(self, idx, value):
         if isinstance(idx,int):
             return self.regs[idx].setreg(value)
         elif isinstance(idx,str):
             return self.regs._asdict()[idx].setreg(value)
-        else:
-            print('Unsupported indexing!')
-            assert(False)
+        assert False, 'Unsupported indexing!'
 
 ## search methods ###########################################################
 
     def search_bitfield(self,field,case_sensitive=False):
+        """
+        Search bitfields which name contains a specified string
+        """
         return tools.search.bitfield(self.regs,field,case_sensitive=case_sensitive)
-        pass
 
     def search_register(self,reg,case_sensitive=False):
+        """
+        Search registers which name contains a specified string
+        """
         return tools.search.register(self.regs,reg,case_sensitive=case_sensitive)
-    
+
     def search_address(self,address,mask='0xFFFFFFFF'):
-        return tools.search.address(self.regs,address,mask=mask)  
+        """
+        Search register matching a specified address
+        """
+        return tools.search.address(self.regs,address,mask=mask)
 
     def to_docx(self,*args):
+        """
+        Generate a .docx document describing an Hardware Abstraction Layer
+        """
         hal2doc(self.regs,*args)
 
-    pass
-
 ## dump methods #############################################################
     def regs2dict(self):
+        """
+        Converts an hal structure into a dictionary in the form:
+        dictval = {
+            'reg1': val1,
+            'reg2': val2,
+        }
+        """
         outdict = {}
-        for r,v in self.regs._asdict().items():
-            outdict[r] = v.getreg()
+        for reg,val in self.regs._asdict().items():
+            outdict[reg] = val.getreg()
         return outdict
 
     def dump(self,fname='dump.hkl'):
-        rd = self.regs2dict()
-        hkl.dump(rd, fname, compression='gzip')
-        pass
+        """
+        Dump the value of all registers in a .hkl file.
+        """
+        regs_dict = self.regs2dict()
+        hkl.dump(regs_dict, fname, compression='gzip')
 
     def dump_diff(self,f1name='dump.hkl',f2name='dump2.hkl',width = 60):
+        """
+        Perform a diff on two dumped .hkl files.
+        """
         fmtstr = '%%%ds |%%%ds' % (width,width)
 
-        f1 = hkl.load(f1name)        
-        f2 = hkl.load(f2name)
+        field1 = hkl.load(f1name)
+        field2 = hkl.load(f2name)
+
+        # create a header with filenames
+        outstrlist = []
+        for reg,val in field1.items():
+            if not field2[reg] == val:
+                f1regstr = self[reg].__repr__(val).split('\n')
+                f2regstr = self[reg].__repr__(field2[reg]).split('\n')
 
-        # create a header with filenames        
-        outstrlist = []        
-        for r,v in f1.items():
-            if not(f2[r] == v):
-                # print(r)
-                f1regstr = self[r].__repr__(v).split('\n')
-                f2regstr = self[r].__repr__(f2[r]).split('\n')
-                
                 for idx in range(len(f1regstr)):
-                    if not(f1regstr[idx]==f2regstr[idx]):
+                    if not f1regstr[idx]==f2regstr[idx]:
                         linestr = fmtstr % (f1regstr[idx],f2regstr[idx])
                         outstrlist.append(linestr)
-                        # print(linestr)
-                    pass
-                
+
         # print output
         if len(outstrlist) > 0:
             headerstr = fmtstr % (f1name,f2name)
             outstrlist.insert(0,headerstr)
             for line in outstrlist:
                 print(line)
         else:
             print('No differences found!!!')
 
-        pass
-
-    pass
-
 def test_to_docx():
+    """
+    Test Function for Cheap Pie HAL to .docx
+    """
     from parsers.cp_parsers_wrapper import cp_parsers_wrapper
     from cheap_pie_core.cp_cli import cp_cli
-    
-    p = cp_cli(['-t','dummy','-rf','my_subblock.xml','-fmt','ipxact'])
-    hal = cp_hal(cp_parsers_wrapper(p))
+
+    prms = cp_cli(['-t','dummy','-rf','my_subblock.xml','-fmt','ipxact'])
+    hal = cp_hal(cp_parsers_wrapper(prms))
 
     hal.to_docx()
-    pass
 
 def test_cp_hal():
+    """
+    Test Function for Cheap Pie Hardware Abstraction Layer
+    """
     from parsers.cp_parsers_wrapper import cp_parsers_wrapper
     from cheap_pie_core.cp_cli import cp_cli
     from ast import literal_eval
 
-    p = cp_cli(['-t','dummy'])
-    hal = cp_hal(cp_parsers_wrapper(p,cp_dummy()))
+    prms = cp_cli(['-t','dummy'])
+    hal = cp_hal(cp_parsers_wrapper(prms,cp_dummy()))
 
-    print('Test register methods...')     
-    # hex assignement       
+    print('Test register methods...')
+    # hex assignement
     inval = "0xFFFFFFFF"
     hal.regs.ADC_ANA_CTRL.setreg(inval)
     retval = hex(hal.regs.ADC_ANA_CTRL.getreg())
     # print('%s' % retval.encode('hex'))
     print(retval)
-    assert(literal_eval(inval) == literal_eval(retval))
+    assert literal_eval(inval) == literal_eval(retval)
 
-    # decimal assignement        
+    # decimal assignement
     inval = 2
     hal.regs.ADC_ANA_CTRL.setreg(inval)
-    retval = hal.regs.ADC_ANA_CTRL.getreg()        
-    assert(inval == retval)
+    retval = hal.regs.ADC_ANA_CTRL.getreg()
+    assert inval == retval
 
     hal.regs.ADC_ANA_CTRL.display()
-            
     print('Test bitfield methods...')
 
     hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display()
     hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display(2)
     hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.setbit(inval)
     retval = hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.getbit()
-    assert(inval == retval)
+    assert inval == retval
 
     # subscriptable interface
     hal[0]
     hal[0][0]
     hal['ADC_ANA_CTRL']
 
     # test assignement
     hal['ADC_ANA_CTRL'] = 1
     hal['ADC_ANA_CTRL']['ADC_BM'] = 2
     # dict-based assignement in single register write
     hal['ADC_ANA_CTRL'] = {'DITHER_EN': 1, 'CHOP_EN': 1, 'INV_CLK': 1}
 
     # test search
-    r = hal.search_register('ADC_ANA_CTRL')
-    assert(len(r)>0)
-    f = hal.search_bitfield('ADC_BM')
-    assert(len(r)>0)
-    r = hal.search_address('0x4000702c')
-    assert(len(r)>0)
-    r = hal.search_address('0xF000702c',mask='0x0FFFFFFF')
-    assert(len(r)>0)
-    r = hal.search_address('0xF000702c')
-    assert(r is None)
+    reg = hal.search_register('ADC_ANA_CTRL')
+    assert len(reg)>0
+    field = hal.search_bitfield('ADC_BM')
+    assert len(field)>0
+    reg = hal.search_address('0x4000702c')
+    assert len(reg)>0
+    reg = hal.search_address('0xF000702c',mask='0x0FFFFFFF')
+    assert len(reg)>0
+    reg = hal.search_address('0xF000702c')
+    assert reg is None
 
     # test conversion to doc
-    # hal.to_docx()
     test_to_docx()
 
     # test dump
-    d1 = 'dump1.hkl'
-    d2 = 'dump2.hkl'
-    hal.dump(d1)
-    hal['ADC_ANA_CTRL']['ADC_BM'] = 3    
-    hal.dump(d2)
-    hal.dump_diff(d1,d2)
-
-    pass
-        
-if __name__ == '__main__':    
+    dump1 = 'dump1.hkl'
+    dump2 = 'dump2.hkl'
+    hal.dump(dump1)
+    hal['ADC_ANA_CTRL']['ADC_BM'] = 3
+    hal.dump(dump2)
+    hal.dump_diff(dump1,dump2)
+
+if __name__ == '__main__':
     test_cp_hal()
-    pass
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/cp_register.py` & `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_register.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,316 +1,315 @@
 #!/usr/bin/python3
+"""
+Register Class Module for Cheap Pie
+"""
 #
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 import textwrap
 from collections import namedtuple
 from ast import literal_eval
 
 try:
     from cheap_pie_core.cbitfield import cp_bitfield
 except:
-    from cbitfield import cp_bitfield    
+    from cbitfield import cp_bitfield
 
 class cp_register:
-    """ A chip register class """
-    addr = 0    
+    """
+    Register Class for Cheap Pie
+    """
+    addr = 0
     regname = ''
     bitfields = []
-    dictfields = dict()
+    dictfields = {}
     comments = ''
     # host interface handler
     hif = None
     addr_offset = 0
     addr_base   = 0
-    
+    #
     def __init__(self, regname, regaddr, comments, hif, addr_offset=0, addr_base=0):
         # address
-        self.addr = regaddr        
-        
+        self.addr = regaddr
+
         # name
         self.regname = regname
-        
+
         # fields
-        self.dictfields = dict()
-        
+        self.dictfields = {}
+
         # Comments
         self.comments = comments
-        
+
         # host interface handler
-        self.hif = hif    
+        self.hif = hif
 
         # address offset
         self.addr_offset = addr_offset
 
         # address base
-        self.addr_base = addr_base        
+        self.addr_base = addr_base
 
     def getreg(self, asdict=False, as_signed=False):
         """ function getreg(self,regval)
         %
         % Displays value of a register from a register value
         %
         % input : regval value of the full register either in decimal or
         % hexadecimal """
-        
-        # if isinstance(self.hif,cp_jlink):
-        if not (self.hif is None ):
+
+        if not self.hif is None:
             regval = self.hif.hifread(self.addr)
         else :
             regval = 0
 
         if asdict:
             # dictionary
-            retval = dict()
+            retval = {}
             for field in self.bitfields:
                 retval[field.fieldname] = field.getbit(regval)
         elif as_signed:
             # signed integer
             retval = -(regval & literal_eval('0x80000000')) + (regval & literal_eval('0x7FFFFFFF'))
-        else: 
+        else:
             # unsigned integer (default)
             retval = regval
-        
-        return retval    
-        
+
+        return retval
+
     def setreg(self,regval = 0, echo =False, *args,**kwargs):
         """ function setreg(self,regval)
         %
         % Displays value of a register from a register value
         %
         % input : regval value of the full register either in decimal or
-        % hexadecimal """        
-        
+        % hexadecimal """
+
         ## handle string input as binary #################################################
         if isinstance(regval, str):
-            regval = literal_eval(regval)        
+            regval = literal_eval(regval)
 
         ## handle dict values ############################################################
         elif isinstance(regval,dict):
             rval = self.getreg()
-            for f,fval in regval.items():
-                rval = self[f].setbit(fval, regval=rval, writeback=False)
+            for field,fval in regval.items():
+                rval = self[field].setbit(fval, regval=rval, writeback=False)
             regval = rval
 
         ## handle negative values ########################################################
         elif regval < 0:
             regval = (abs(regval) ^ literal_eval('0xFFFFFFFF')) + 1
             # print('regval write: 0x%x' % regval)
 
         #% write %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
-        
-        # if isinstance(self.hif,cp_jlink):   
-        if not (self.hif is None ):                    
+
+        if not self.hif is None:
             ret = self.hif.hifwrite(self.addr, regval, *args,**kwargs)
         else :
             ret = regval
-        
+
         #% only display output if no nargout %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
         if echo:
-            self.display(regval)          
-        
+            self.display(regval)
+
         return ret
 
-    def getbit(self, bit_offset=0, width=1):                
-        b = cp_bitfield(regaddr=self.addr, width=width, bit_offset=bit_offset, hif=self.hif)        
-        return b.getbit()
-
-    def setbit(self, bitval=0, bit_offset=0, width=1):                
-        b = cp_bitfield(regaddr=self.addr, width=width, bit_offset=bit_offset, hif=self.hif)        
-        return b.setbit(bitval)
+    def getbit(self, bit_offset=0, width=1):
+        """ Get a custom bitfield within a register """
+        bitfield = cp_bitfield(regaddr=self.addr, width=width, bit_offset=bit_offset, hif=self.hif)
+        return bitfield.getbit()
+
+    def setbit(self, bitval=0, bit_offset=0, width=1):
+        """ Set a custom bitfield within a register """
+        bitfield = cp_bitfield(regaddr=self.addr, width=width, bit_offset=bit_offset, hif=self.hif)
+        return bitfield.setbit(bitval)
 
     def getbyte(self, byte_offset=0):
-        b = cp_bitfield(regaddr=self.addr, width=8, bit_offset=byte_offset*8, hif=self.hif)        
-        return b.getbit()
+        """ Get a custom byte within a register """
+        byte = cp_bitfield(regaddr=self.addr, width=8, bit_offset=byte_offset*8, hif=self.hif)
+        return byte.getbit()
 
     def setbyte(self, byteval=0, byte_offset=0):
-        b = cp_bitfield(regaddr=self.addr, width=8, bit_offset=byte_offset*8, hif=self.hif)        
-        return b.setbit(byteval)
+        """ Set a custom byte within a register """
+        byte = cp_bitfield(regaddr=self.addr, width=8, bit_offset=byte_offset*8, hif=self.hif)
+        return byte.setbit(byteval)
 
     def help(self,width=25):
-        """ function ret = help(self)        
-        # displays register comments """    
+        """ function ret = help(self)   
+        # displays register comments """
         print(self.comments)
-        
+
         fmtstr = '%%%ds: %%s' % width
         for field in self.bitfields:
             print( fmtstr % (field.fieldname,''))
 
             for line in textwrap.wrap(field.comments):
                 print( fmtstr % ('',line))
-        
+
     def __repr__(self,regval = None ):
         if regval is None:
             # read register value
             regval = self.getreg()
 
         if len(self.bitfields) > 0:
-            r = []        
+            reg = []
             for field in self.bitfields :
                 # field.display(regval)
-                r.append(field.__repr__(regval))        
-            outstr = "\n".join(r)
-        else: 
+                reg.append(field.__repr__(regval))
+            outstr = "\n".join(reg)
+        else:
             outstr = self.regname + ' = ' + hex(regval)
         return outstr
 
     def display(self, regval = None ):
-        r = self.__repr__(regval=regval)
-        print(r)
-        return r    
-        
+        """ Show a register """
+        outstr = self.__repr__(regval)
+        print(outstr)
+        return outstr
+
     def addfield(self, field):
-        # assert isinstance(field,cp_bitfield)
-        # self.bitfields.append(field)
+        """ Add a field to a register """
         self.dictfields[field.fieldname] = field
-        # cmdstr = "self." + field.fieldname + " = field "
-        # eval(cmdstr)
-        
+
     def dictfield2struct(self):
+        """ Convert the list of bitfields into a namedtuple """
         if len(self.dictfields) > 0:
-            self.bitfields = namedtuple(self.regname, self.dictfields.keys())(*self.dictfields.values())
-        
+            self.bitfields = namedtuple(self.regname,
+                                        self.dictfields.keys())(*self.dictfields.values())
+
     def get_bitfields(self, name=None):
         """
         Find a child element by name
         """
         if name:
             return [e for e in self.bitfields if e._name == name]
-        else:
-            return self.bitfields
+
+        return self.bitfields
 
     def __contains__(self, key):
         if self.bitfields is None:
             raise TypeError('not indexable')
         return any(item.fieldname == key for item in self.bitfields)
 
     def __len__(self):
         return len(self.bitfields)
 
     def __iter__(self):
         return self.bitfields.__iter__()
-        # for field in self.bitfields:
-        #    yield (field.fieldname, field.getbit())
-    
+
     def __next__(self):
         return self.bitfields.next()
-    
+
     def __getitem__(self, idx):
         if isinstance(idx,int):
             return self.bitfields[idx]
-        elif isinstance(idx,str):
+        if isinstance(idx,str):
             return self.bitfields._asdict()[idx]
-        else:
-            print('Unsupported indexing!')
-            assert(False)
-        pass    
-    
+        assert False, 'Unsupported indexing!'
+
     def __setitem__(self, idx, value):
         if isinstance(idx,int):
             return self.bitfields[idx].setbit(value)
-        elif isinstance(idx,str):
+        if isinstance(idx,str):
             return self.bitfields._asdict()[idx].setbit(value)
-        else:
-            print('Unsupported indexing!')
-            assert(False)
-        pass
+        assert False, 'Unsupported indexing!'
 
     def __index__(self):
         return int(self.getreg())
 
 def test_cp_register():
+    """ Cheap Pie test for cp_register class """
     import sys
     import os.path
     sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
     from transport.cp_dummy_transport import cp_dummy
     from cheap_pie_core.cbitfield import cp_bitfield
     from random import randint
 
-    r = cp_register( 
+    reg = cp_register(
         regname='regname',
         regaddr=10,
         comments='comments',
         hif = cp_dummy(),
         addr_offset=10,
         addr_base=10
     )
 
     # test value
     val = 15
-    r.setreg(val)
-    assert(val==r.getreg())
-    r.display()
-    r.help()
+    reg.setreg(val)
+    assert val==reg.getreg()
+    reg.display()
+    reg.help()
 
     # negative assignement
     negval = -1
-    r.setreg(negval)
-    retval = r.getreg(as_signed=True)
+    reg.setreg(negval)
+    retval = reg.getreg(as_signed=True)
     print(retval)
-    assert(retval==negval)
+    assert retval==negval
 
     # test bitfield
-    f1 = cp_bitfield(
+    field1 = cp_bitfield(
         regfield = 'fname',
         regaddr = 10,
         regname = 'rname',
         width = '2',
         bit_offset = '2',
         comments = 'comment',
         hif = cp_dummy()
     )
-    f2 = cp_bitfield(
+    field2 = cp_bitfield(
         regfield = 'fname2',
         regaddr = 10,
         regname = 'rname',
         width = '2',
         bit_offset = '4',
         comments = 'comment2',
         hif = cp_dummy()
     )
 
-    r.addfield(f1)
-    r.addfield(f2)
-    r.dictfield2struct()
-    r.get_bitfields()
+    reg.addfield(field1)
+    reg.addfield(field2)
+    reg.dictfield2struct()
+    reg.get_bitfields()
     # display with bitfields
-    r.display()
-    r.help()
+    reg.display()
+    reg.help()
 
     # item access
-    r[0]
-    r['fname']
+    reg[0]
+    reg['fname']
 
     # item assignement
-    r[0] = 1
-    r['fname'] = 2
+    reg[0] = 1
+    reg['fname'] = 2
 
     # bit access
     for offset in range(32):
         for bitval in range(2):
-            r.setbit(bitval, bit_offset=offset)    
-            assert( r.getbit(bit_offset=offset) == bitval ) 
-    
+            reg.setbit(bitval, bit_offset=offset)
+            assert reg.getbit(bit_offset=offset) == bitval
+
     # byte access
     for offset in range(4):
         byteval = randint(0,255)
-        r.setbyte(byteval, byte_offset=offset)    
-        assert( r.getbyte(byte_offset=offset) == byteval ) 
+        reg.setbyte(byteval, byte_offset=offset)
+        assert reg.getbyte(byte_offset=offset) == byteval
 
     # integer representation
-    print(hex(r))
+    print(hex(reg))
 
     # dict-based assignement
-    d = {'fname': 1, 'fname2': 2}
-    r.setreg(d)
+    dreg = {'fname': 1, 'fname2': 2}
+    reg.setreg(dreg)
 
     # dict-based readback
-    dr = r.getreg(asdict=True)
-    assert(d == dr)
+    dregb = reg.getreg(asdict=True)
+    assert dreg == dregb
 
 if __name__ == '__main__':
     test_cp_register()
-    pass
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/cheap_pie_core/test.py` & `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/python3
-
+""" Cheap Pie Test Module """
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 import unittest
 import sys
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 class CheapPieMethods(unittest.TestCase):
+    """ Cheap Pie Test Class """
 
     def test_transport(self):
+        """ Cheap Pie Test Transport Method """
+
         # dummy for mockup
         from transport.cp_dummy_transport import test_cp_dummy
         test_cp_dummy()
 
         # jlink
         from transport.cp_jlink_transport import test_cp_jlink
         test_cp_jlink()
@@ -25,34 +28,35 @@
         from transport.cp_pyocd_transport import test_cp_pyocd
         test_cp_pyocd()
 
         # esptool
         from transport.cp_esptool_transport import test_cp_esptool
         test_cp_esptool()
 
-        # pyverilator 
+        # pyverilator
         from transport.cp_pyverilator_transport import test_cp_pyverilator
         test_cp_pyverilator()
 
-        pass
-   
     def test_bitfield(self):
+        """ Test bitfield class """
         from cheap_pie_core.cbitfield import test_cp_bitfield
         test_cp_bitfield()
-    
+
     def test_register(self):
+        """ Test register class """
         from cheap_pie_core.cp_register import test_cp_register
         test_cp_register()
 
     def test_cp_hal(self):
+        """ Test hal class """
         from cheap_pie_core.cp_hal import test_cp_hal
         test_cp_hal()
-        pass   
 
     def test_parsers(self):
+        """ Test cheap pie parsers """
         from parsers.svd_parse import test_svd_parse
         test_svd_parse()
 
         from parsers.svd_parse_repo import test_svd_parse_repo
         test_svd_parse_repo()
 
         from parsers.ipxact_parse import test_ipxact_parse
@@ -61,25 +65,26 @@
         from parsers.ipyxact_parse import test_ipyxact_parse
         test_ipyxact_parse()
 
         from parsers.rdl_parse import test_rdl_parse
         test_rdl_parse()
 
     def test_parsers_wrapper(self):
+        """ Test parsers wrapper """
         from parsers.cp_parsers_wrapper import test_cp_parsers_wrapper
         test_cp_parsers_wrapper()
-        pass
 
     def test_tools(self):
+        """ Test cheap_pie tools """
         from tools.hal2doc import test_hal2doc
         test_hal2doc()
 
         from tools.search import test_search
         test_search()
-        pass
 
     def test_cheap_pie_main(self):
+        """ Test cheap pie main """
         from cheap_pie_core.cheap_pie import main
         main()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/parsers/ipxact_parse.py` & `cheap_pie-0.9.18/src/cheap_pie/parsers/ipxact_parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,114 +1,109 @@
 #!/usr/bin/python3
-
+""" Cheap Pie native module parser for IP-XACT """
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
-import untangle # for parsing xml
 from ast import literal_eval
-import string as str
 from collections import namedtuple
+import untangle # for parsing xml
 
 import sys
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from cheap_pie_core.cbitfield   import cp_bitfield
 from cheap_pie_core.cp_register import cp_register
 from parsers.name_subs import name_subs
 
 def ipxact_remove_prefix(ipx):
+    """ remove ipxact or spirit prefix"""
     replist = ['ipxact_','spirit_']
-    
+
     if hasattr(ipx,'children'):
-        for e in ipx.children:
+        for elm in ipx.children:
             # remove all suffixes
-            for r in replist:
-                e._name = e._name.replace(r,'')
+            for repl in replist:
+                elm._name = elm._name.replace(repl,'')
             # remove recursively
-            ipxact_remove_prefix(e)
+            ipxact_remove_prefix(elm)
 
     return ipx
     pass
 
 def ipxact_parse(fname,hif=None, base_address_offset = "0x00000000"):
-       
+    """ Cheap Pie native module parser for IP-XACT """
     ## read input file ########################################################
     csv = untangle.parse(fname)
 
     ## remove ipxact/spirit prefixes ##########################################
     csv = ipxact_remove_prefix(csv)
-    
+
     ## loop over lines ########################################################
-    outdict = dict()
+    outdict = {}
 
     periph = csv.component.memoryMaps.memoryMap.addressBlock
-    # print(periph)
-    
     base_addr_str=periph.baseAddress.cdata.replace("'h",'0x')
-    # print(base_addr_str)
     base_address=literal_eval(base_addr_str)
 
     if hasattr(periph,'register'):
-        for reg in periph.register:                
+        for reg in periph.register:
             if hasattr( reg.name, 'cdata'):
                 # close old register, before opening a new one
                 if 'regname' in locals():
                     struct_register.dictfield2struct()
                     outdict[regname]=struct_register
 
                 # new register
                 periph_name=periph.name.cdata
                 rname=reg.name.cdata
-                regname = "%s_%s" % ( periph_name,rname )
+                regname = f'{periph_name}_{rname}'
                 regname=name_subs(regname)
 
                 addr_str=reg.addressOffset.cdata.replace("'h",'0x')
                 regaddr=literal_eval(addr_str) + base_address + literal_eval(base_address_offset)
                 comments=""
                 # print(comments)
                 struct_register=cp_register(regname,regaddr,comments,hif)
 
                 # for field_idx in range(nfields):
                 if hasattr(reg,'field'):
                     for field in reg.field :
                         regfield=field.name.cdata
 
-                        if not(field is None):
+                        if not field is None:
                             # print regfield
                             regfield=name_subs(regfield)
 
-                            csvWidth=field.bitWidth.cdata
+                            csv_width=field.bitWidth.cdata
                             bitoffset=field.bitOffset.cdata
                             comments="" # field.description.cdata
                             # print(comments)
-                            
+
                             # Create new field class
-                            class_regfield=cp_bitfield(regfield,regaddr,regname,csvWidth,bitoffset,comments,hif)
+                            class_regfield=cp_bitfield(
+                                regfield,regaddr,regname,csv_width,bitoffset,comments,hif)
                             struct_register.addfield(class_regfield)
 
         # create last register, if existing
         if 'regname' in locals():
             # outstruct=addreg2struct(outstruct,regname,struct_register)
             struct_register.dictfield2struct()
             outdict[regname]=struct_register
-    
+
     # convert output dictionary into structure
-    # return outdict
-    return namedtuple("HAL", outdict.keys())(*outdict.values()) 
+    return namedtuple("HAL", outdict.keys())(*outdict.values())
 
 def test_ipxact_parse():
+    """ Test function for cheap pie native IP-XACT parser """
     ipxact_parse("./devices/my_subblock.xml")
     ipxact_parse("./devices/leon2_creg.xml")
     ipxact_parse("./devices/generic_example.xml")
-    pass
-    
+
 if __name__ == '__main__':
-    if len(sys.argv) > 1: 
+    if len(sys.argv) > 1:
         fname=sys.argv[1]
     else:
         fname="./devices/my_subblock.xml"
-    print(fname)    
+    print(fname)
     print(ipxact_parse(fname))
-    pass
-
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/parsers/ipyxact_parse.py` & `cheap_pie-0.9.18/src/cheap_pie/parsers/ipyxact_parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,88 @@
 #!/usr/bin/python3
+""" Cheap Pie parser module for IP-XACT structure with ipyxact """   
 
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 from ast import literal_eval
-import string as str
 from collections import namedtuple
-
 from ipyxact.ipyxact import Component
 
 import sys
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from cheap_pie_core.cbitfield   import cp_bitfield
 from cheap_pie_core.cp_register import cp_register
 from parsers.name_subs import name_subs
 
 def ipxact_parse(fname,hif=None, base_address_offset = "0x00000000"):
-       
+    """ Cheap Pie parser for IP-XACT structure with ipyxact """   
     ## read input file ########################################################
     xml = Component()
     xml.load(fname)
-    
+
     ## loop over lines ########################################################
-    outdict = dict()
+    outdict = {}
 
-    for m in xml.memoryMaps.memoryMap:
-        for periph in m.addressBlock:
+    for mem in xml.memoryMaps.memoryMap:
+        for periph in mem.addressBlock:
             # print(periph)
-        
+
             base_address=periph.baseAddress
 
             if hasattr(periph,'register'):
-                for reg in periph.register:                
+                for reg in periph.register:
                     # close old register, before opening a new one
                     if 'regname' in locals():
                         struct_register.dictfield2struct()
                         outdict[regname]=struct_register
 
                     # new register
                     periph_name=periph.name
                     rname=reg.name
-                    regname = "%s_%s" % ( periph_name,rname )
-                    regname=name_subs(regname)
-
+                    regname = name_subs(f'{periph_name}_{rname}')
                     regaddr=reg.addressOffset + base_address + literal_eval(base_address_offset)
                     comments=reg.description
-                    # print(comments)
+
                     struct_register=cp_register(regname,regaddr,comments,hif)
 
-                    # for field_idx in range(nfields):
                     if hasattr(reg,'field'):
                         for field in reg.field :
                             regfield=field.name
 
-                            if not(field is None):
-                                # print regfield
+                            if not field is None:
                                 regfield=name_subs(regfield)
 
-                                csvWidth=field.bitWidth
+                                csv_width=field.bitWidth
                                 bitoffset=field.bitOffset
                                 comments=field.description
-                                # print(comments)
-                                
+
                                 # Create new field class
-                                class_regfield=cp_bitfield(regfield,regaddr,regname,csvWidth,bitoffset,comments,hif)
+                                class_regfield=cp_bitfield(
+                                    regfield,regaddr,regname,csv_width,bitoffset,comments,hif)
                                 struct_register.addfield(class_regfield)
 
             # create last register, if existing
             if 'regname' in locals():
-                # outstruct=addreg2struct(outstruct,regname,struct_register)
                 struct_register.dictfield2struct()
                 outdict[regname]=struct_register
-    
+
     # convert output dictionary into structure
-    # return outdict
-    return namedtuple("HAL", outdict.keys())(*outdict.values()) 
+    return namedtuple("HAL", outdict.keys())(*outdict.values())
 
 def test_ipyxact_parse():
+    """ Test function for IP-XACT parser with ipyxact """   
     ipxact_parse("./devices/my_subblock.xml")
     # ipxact_parse("./devices/leon2_creg.xml") # ValueError: invalid literal for int() with base 10: '4 * (2 ** 10)'
     ipxact_parse("./devices/generic_example.xml")
-    pass
-    
+
 if __name__ == '__main__':
-    if len(sys.argv) > 1: 
+    if len(sys.argv) > 1:
         fname=sys.argv[1]
     else:
         fname="./devices/my_subblock.xml"
-    print(fname)    
+    print(fname)
     hal = ipxact_parse(fname)
     print(hal)
-    pass
-
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse.py` & `cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,99 @@
 #!/usr/bin/python3
-
+""" Cheap Pie module for native .svd files parser """
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 # parser build for CMSIS-SVD xml file format
 # https://www.keil.com/pack/doc/CMSIS/SVD/html/index.html
 #
 # simplified manual initialization
-# 
+#
 # import untangle
 # hal = untangle.parse('QN908XC.xml')
 # from cbitfield import cp_bitfield
 # from cp_register import cp_register
-# ADC_ANA_CTRL = cp_register("ADC_ANA_CTRL","0x4000702C", "ADC core and reference setting regsiter" , hif )
+# ADC_ANA_CTRL = cp_register("ADC_ANA_CTRL","0x4000702C",
+#                            "ADC core and reference setting regsiter" , hif )
 # ADC_BM = cp_bitfield("ADC_BM","0x4000702C","ADC_ANA_CTRL",3,0, "ADC bias current selection." ,hif)
 
-import untangle # for parsing xml
 from ast import literal_eval
-import string as str
 from collections import namedtuple
+import untangle # for parsing xml
 
 import sys
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from cheap_pie_core.cbitfield   import cp_bitfield
 from cheap_pie_core.cp_register import cp_register
 from parsers.name_subs import name_subs
-    
+
 def svd_parse(fname,vendor=None,hif=None, base_address_offset = "0x00000000"):
-        
+    """ Cheap Pie native parser for .svd files """    
     ## read input file ########################################################
     svd = untangle.parse(fname)
-    
+
     ## loop over lines ########################################################
     outdict = dict()
 
     for periph in svd.device.peripherals.peripheral:
         # print(periph.name.cdata)
-        
+
         base_addr_str=periph.baseAddress.cdata
         base_address=literal_eval(base_addr_str)
 
         if hasattr(periph,'registers'):
-            for reg in periph.registers.register:                
+            for reg in periph.registers.register:
                 if hasattr( reg.name, 'cdata'):
                     # close old register, before opening a new one
                     if 'regname' in locals():
                         struct_register.dictfield2struct()
                         outdict[regname]=struct_register
-
+                    #
                     # new register
                     periph_name=periph.name.cdata
                     rname=reg.name.cdata
-                    regname = "%s_%s" % ( periph_name,rname )
-                    regname=name_subs(regname)
-
+                    regname = name_subs(f'{periph_name}_{rname}')
+                    print(regname)
+                    #
                     addr_str=reg.addressOffset.cdata
                     regaddr=literal_eval(addr_str) + base_address + literal_eval(base_address_offset)
                     comments=reg.description.cdata
                     # print(comments)
                     struct_register=cp_register(regname,regaddr,comments,hif)
-
-                    # for field_idx in range(nfields):
+                    #
                     if hasattr(reg,'fields'):
-                        for field in reg.fields.field :
+                        for field in reg.fields.field:
                             regfield=field.name.cdata
-
-                            if not(field is None):
-                                # print regfield
+                            #
+                            if not field is None:
+                                print(regfield)
                                 regfield=name_subs(regfield)
-
-                                csvWidth=field.bitWidth.cdata
+                                width=field.bitWidth.cdata
                                 bitoffset=field.bitOffset.cdata
                                 comments=field.description.cdata
                                 # print(comments)
-                                
                                 # Create new field class
-                                class_regfield=cp_bitfield(regfield,regaddr,regname,csvWidth,bitoffset,comments,hif)
+                                class_regfield=cp_bitfield(
+                                    regfield,regaddr,regname,width,bitoffset,comments,hif)
                                 struct_register.addfield(class_regfield)
-
             # create last register, if existing
             if 'regname' in locals():
                 # outstruct=addreg2struct(outstruct,regname,struct_register)
                 struct_register.dictfield2struct()
                 outdict[regname]=struct_register
-    
     # convert output dictionary into structure
-    # return outdict
-    return namedtuple("HAL", outdict.keys())(*outdict.values()) 
+    return namedtuple("HAL", outdict.keys())(*outdict.values())
 
 def test_svd_parse(argv=[]):
-    if len(argv) > 1: 
+    """ test function for .svd parser """
+    if len(argv) > 1:
         fname=argv[1]
     else:
         fname="./devices/QN908XC.svd"
         # fname="./devices/MIMXRT1011.svd"
     return svd_parse(fname)
-    pass
-        
-if __name__ == '__main__':    
+
+if __name__ == '__main__':
     print(svd_parse(sys.argv))
-    pass
-
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/parsers/svd_parse_repo.py` & `cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 #!/usr/bin/python3
-
+""" Cheap Pie parser module for .svd files using SVDParser module """
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
 # parser build for CMSIS-SVD xml file format
 # https://www.keil.com/pack/doc/CMSIS/SVD/html/index.html
 #
 # simplified manual initialization
-# 
+#
 # import untangle
 # hal = untangle.parse('QN908XC.xml')
 # from cbitfield import cp_bitfield
 # from cp_register import cp_register
-# ADC_ANA_CTRL = cp_register("ADC_ANA_CTRL","0x4000702C", "ADC core and reference setting regsiter" , hif )
-# ADC_BM = cp_bitfield("ADC_BM","0x4000702C","ADC_ANA_CTRL",3,0, "ADC bias current selection." ,hif)
+# ADC_ANA_CTRL = cp_register("ADC_ANA_CTRL","0x4000702C",
+#                            "ADC core and reference setting regsiter" , hif )
+# ADC_BM = cp_bitfield("ADC_BM","0x4000702C",
+#                      "ADC_ANA_CTRL",3,0, "ADC bias current selection." ,hif)
 
-from cmsis_svd.parser import SVDParser
 from ast import literal_eval
-import string as str
 from collections import namedtuple
+from cmsis_svd.parser import SVDParser
 
 import sys
 import os.path
 sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
 
 from cheap_pie_core.cbitfield   import cp_bitfield
 from cheap_pie_core.cp_register import cp_register
 from parsers.name_subs import name_subs
-    
+
 def svd_parse(fname,vendor=None,hif=None, base_address_offset = "0x00000000"):
-        
+    """ Cheap Pie parser function for .svd files using SVDParser module """    
     ## read input file ########################################################
     if vendor is None:
         svd = SVDParser.for_xml_file(fname)
     else:
         svd = SVDParser.for_packaged_svd(vendor,fname)
 
     ## loop over lines ########################################################
-    outdict = dict()
+    outdict = {}
 
     for periph in svd.get_device().peripherals:
         # print(periph.name.cdata)
-        
+
         base_address=periph.base_address
 
         if hasattr(periph,'registers'):
-            for reg in periph.registers:                
+            for reg in periph.registers:
                 if hasattr( reg, 'name'):
                     # close old register, before opening a new one
                     if 'regname' in locals():
                         struct_register.dictfield2struct()
                         outdict[regname]=struct_register
 
                     # new register
                     periph_name=periph.name
                     rname=reg.name
-                    regname = "%s_%s" % ( periph_name,rname )
-                    regname=name_subs(regname)
+                    regname = name_subs(f'{periph_name}_{rname}')
 
                     regaddr=reg.address_offset + base_address + literal_eval(base_address_offset)
                     comments=reg.description
                     # print(comments)
                     struct_register=cp_register(regname,regaddr,comments,hif)
 
                     # for field_idx in range(nfields):
                     if hasattr(reg,'fields'):
                         for field in reg.fields :
                             regfield=field.name
 
-                            if not(field is None):
+                            if not field is None:
                                 # print regfield
                                 regfield=name_subs(regfield)
 
-                                csvWidth=field.bit_width
+                                width=field.bit_width
                                 bitoffset=field.bit_offset
                                 comments=field.description
                                 # print(comments)
-                                
+
                                 # Create new field class
-                                class_regfield=cp_bitfield(regfield,regaddr,regname,csvWidth,bitoffset,comments,hif)
+                                class_regfield=cp_bitfield(regfield,regaddr,regname,
+                                                           width,bitoffset,comments,hif)
                                 struct_register.addfield(class_regfield)
 
             # create last register, if existing
             if 'regname' in locals():
                 # outstruct=addreg2struct(outstruct,regname,struct_register)
                 struct_register.dictfield2struct()
                 outdict[regname]=struct_register
-    
+
     # convert output dictionary into structure
-    # return outdict
     return namedtuple("HAL", outdict.keys())(*outdict.values())
 
 def test_svd_parse_repo():
+    """ Test Function for .svd parser based of SVDParser module """
     print('Testing QN9080 with repo parser...')
 
     from parsers.svd_parse_repo import svd_parse
-    # hal = svd_parse(fname="./devices/MIMXRT1011.svd")
-    hal = svd_parse(fname="./devices/QN908XC.svd")
-        
+    svd_parse(fname="./devices/QN908XC.svd")
+
     print('Testing K20 with repo parser...')
-    hal = svd_parse(fname='MK20D7.svd',vendor='Freescale')
-    
+    svd_parse(fname='MK20D7.svd',vendor='Freescale')
+
 if __name__ == '__main__':
     test_svd_parse_repo()
-    pass
-
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-0.9.18/src/cheap_pie/parsers/xml_xslt.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-0.9.18/src/cheap_pie/tools/hal2doc.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/tools/rdl2any.py` & `cheap_pie-0.9.18/src/cheap_pie/tools/rdl2any.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/tools/rdl2verilog.py` & `cheap_pie-0.9.18/src/cheap_pie/tools/rdl2verilog.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/tools/reload_module.py` & `cheap_pie-0.9.18/src/cheap_pie/tools/reload_module.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/tools/search.py` & `cheap_pie-0.9.18/src/cheap_pie/tools/search.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/tools/test_rdl.py` & `cheap_pie-0.9.18/src/cheap_pie/tools/test_rdl.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-0.9.18/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-0.9.18/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-0.9.18/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyocd_transport.py` & `cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyocd_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.1.17/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 #!/usr/bin/python3
-import pyverilator
+"""
+Cheap Pie module for pyverilator transport
+"""
+import os
 import argparse
 import sys
 from ast import literal_eval
 from shutil import copyfile
-import os
+
+import pyverilator
 
 def cli(args=[]):
+    """ Command Line Interface for pyverilator transport class """
     parser = argparse.ArgumentParser(description='rdl2verilog pyverilator ')
     # register format options
-    parser.add_argument("-f", "--fname", help="register file description .v", action='store', type = str, default="./devices/verilog/basic_rf.v")
+    parser.add_argument("-f", "--fname",
+                        help="register file description .v", action='store',
+                        type = str, default="./devices/verilog/basic_rf.v")
     return parser.parse_args(args)
 
 class cp_pyverilator_transport():
+    """
+    Cheap Pie class for pyverilator transport
+    """
     sim = None
 
     def __init__(self,fname):
 
         # rename to .v, if .sv
         if not os.path.isfile(fname):
-            print('File %s does not exist!' % fname)
-            assert(False)
+            assert False, f'File {fname} does not exist!'
 
         base,ext = os.path.splitext(fname)
         # print(ext)
 
         if ext == '.sv':
             print('renaming input file to .v')
             ofname = base + '.v'
@@ -45,14 +54,15 @@
         # add all the io and internal signals to gtkwave
         self.sim.send_to_gtkwave(self.sim.io)
         self.sim.send_to_gtkwave(self.sim.internals)
 
         self.reset_release()
 
     def reset_release(self):
+        """ Release Reset signal """
         # tick the automatically detected clock
         self.sim.clock.tick()
 
         # set rst back to 0
         # sim.io.rst = 0
         self.sim.io.resetn = 0
         self.sim.clock.tick()
@@ -71,15 +81,15 @@
 
         # check out when en = 1
         # sim.io.en = 1
         # curr_out = sim.io.out
         # print('sim.io.out = ' + str(curr_out))
 
     def hifwrite(self, addr='0x00', val='0xB16B00B5', mask='0xFFFFFFFF'):
-
+        """ Write register """
         if isinstance(addr,str):
             addr = literal_eval(addr)
 
         if isinstance(val,str):
             val = literal_eval(val)
 
         if isinstance(mask,str):
@@ -106,15 +116,15 @@
         # sim.io.basicreg_basicfield_wdata = literal_eval('0xB16B00B5')
         # sim.io.basicreg_basicfield_we = 0
         # sim.clock.tick()
         # sim.io.basicreg_basicfield_we = 1
         # sim.clock.tick()
 
     def hifread(self,addr = '0x00'):
-
+        """ Read register """
         if isinstance(addr,str):
             addr = literal_eval(addr)
 
         # SW read
         self.sim.io.addr = addr
         self.sim.io.read = 1
 
@@ -129,41 +139,42 @@
         self.sim.io.valid = 0
         self.sim.clock.tick()
 
         # print(hex(outval))
         return outval
 
 def verilator_version():
+    """ Return verilator version """
     import subprocess
     result = subprocess.run(['verilator', '--version'], stdout=subprocess.PIPE)
     ver = result.stdout.split()[1]
-    return ver.decode("utf-8") 
+    return ver.decode("utf-8")
 
 def verilator_version_ok():
+    """ True if the installed verilator version works as transport for cheap_pie """
     # check Verilated::flushCall() exist
     # https://github.com/chipsalliance/chisel3/issues/1565
     from packaging import version
     ver = verilator_version()
     # print(ver)
     if ( version.parse(ver) < version.parse("4.036") or
          version.parse(ver) > version.parse("4.102")):
         return True
     else:
         return False
 
 def test_cp_pyverilator(args = []):
-
+    """ Test pyverilator transport """
     if verilator_version_ok():
-        p = cli(args)
-        hif = cp_pyverilator_transport(p.fname)
-        
+        prms = cli(args)
+        hif = cp_pyverilator_transport(prms.fname)
         val = literal_eval('0x5A5A5A5A')
         hif.hifwrite(val = val)
         print( hex(hif.hifread()) )
-        assert( hif.hifread() == val )
-
+        assert hif.hifread() == val
     else:
-        print('Warning: pyverilator not working anymore with verilator versions between 4.036 and 4.102.')
+        print('Warning: pyverilator not working anymore \
+              with verilator versions between 4.036 and 4.102.')
         print('https://github.com/chipsalliance/chisel3/issues/1565')
 
 if __name__ == '__main__':
-    test_cp_pyverilator(sys.argv[1:])
+    test_cp_pyverilator(sys.argv[1:])
```

### Comparing `cheap_pie-0.1.17/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-0.9.18/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

