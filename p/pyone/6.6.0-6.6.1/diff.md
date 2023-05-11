# Comparing `tmp/pyone-6.6.0.tar.gz` & `tmp/pyone-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyone-6.6.0.tar", last modified: Wed Dec 21 12:18:13 2022, max compression
+gzip compressed data, was "pyone-6.6.1.tar", last modified: Tue Mar  7 10:35:46 2023, max compression
```

## Comparing `pyone-6.6.0.tar` & `pyone-6.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2022-12-21 12:18:13.118041 pyone-6.6.0/
--rw-rw-r--   0 one       (1001) one       (1001)      889 2022-12-21 12:18:13.118041 pyone-6.6.0/PKG-INFO
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2022-12-21 12:18:13.110041 pyone-6.6.0/pyone/
--rw-r--r--   0 one       (1001) one       (1001)    11256 2022-12-21 12:05:41.000000 pyone-6.6.0/pyone/__init__.py
--rw-r--r--   0 one       (1001) one       (1001)     5898 2022-12-21 12:05:41.000000 pyone-6.6.0/pyone/acl.py
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2022-12-21 12:18:13.114041 pyone-6.6.0/pyone/bindings/
--rw-rw-r--   0 one       (1001) one       (1001)   114234 2022-12-21 12:18:12.000000 pyone-6.6.0/pyone/bindings/__init__.py
--rw-rw-r--   0 one       (1001) one       (1001)  2609185 2022-12-21 12:18:12.000000 pyone-6.6.0/pyone/bindings/supbind.py
--rw-r--r--   0 one       (1001) one       (1001)     3278 2022-12-21 12:05:41.000000 pyone-6.6.0/pyone/helpers.py
--rw-r--r--   0 one       (1001) one       (1001)      929 2022-12-21 12:05:41.000000 pyone-6.6.0/pyone/server.py
--rw-r--r--   0 one       (1001) one       (1001)     7039 2022-12-21 12:05:41.000000 pyone-6.6.0/pyone/tester.py
--rw-r--r--   0 one       (1001) one       (1001)     5023 2022-12-21 12:05:41.000000 pyone-6.6.0/pyone/util.py
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2022-12-21 12:18:13.110041 pyone-6.6.0/pyone.egg-info/
--rw-rw-r--   0 one       (1001) one       (1001)      889 2022-12-21 12:18:12.000000 pyone-6.6.0/pyone.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1001) one       (1001)      299 2022-12-21 12:18:13.000000 pyone-6.6.0/pyone.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1001) one       (1001)        1 2022-12-21 12:18:12.000000 pyone-6.6.0/pyone.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1001) one       (1001)       89 2022-12-21 12:18:12.000000 pyone-6.6.0/pyone.egg-info/requires.txt
--rw-rw-r--   0 one       (1001) one       (1001)        6 2022-12-21 12:18:12.000000 pyone-6.6.0/pyone.egg-info/top_level.txt
--rw-rw-r--   0 one       (1001) one       (1001)       38 2022-12-21 12:18:13.118041 pyone-6.6.0/setup.cfg
--rw-r--r--   0 one       (1001) one       (1001)     2495 2022-12-21 12:05:41.000000 pyone-6.6.0/setup.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.078187 pyone-6.6.1/
+-rw-rw-r--   0 one       (1001) one       (1001)      889 2023-03-07 10:35:46.078187 pyone-6.6.1/PKG-INFO
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.070187 pyone-6.6.1/pyone/
+-rw-r--r--   0 one       (1001) one       (1001)    11256 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/__init__.py
+-rw-r--r--   0 one       (1001) one       (1001)     5898 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/acl.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.070187 pyone-6.6.1/pyone/bindings/
+-rw-rw-r--   0 one       (1001) one       (1001)   115076 2023-03-07 10:35:44.000000 pyone-6.6.1/pyone/bindings/__init__.py
+-rw-rw-r--   0 one       (1001) one       (1001)  2624697 2023-03-07 10:35:44.000000 pyone-6.6.1/pyone/bindings/supbind.py
+-rw-r--r--   0 one       (1001) one       (1001)     3278 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/helpers.py
+-rw-r--r--   0 one       (1001) one       (1001)      929 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/server.py
+-rw-r--r--   0 one       (1001) one       (1001)     7039 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/tester.py
+-rw-r--r--   0 one       (1001) one       (1001)     5023 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/util.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.070187 pyone-6.6.1/pyone.egg-info/
+-rw-rw-r--   0 one       (1001) one       (1001)      889 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1001) one       (1001)      299 2023-03-07 10:35:46.000000 pyone-6.6.1/pyone.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1001) one       (1001)        1 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1001) one       (1001)       89 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/requires.txt
+-rw-rw-r--   0 one       (1001) one       (1001)        6 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/top_level.txt
+-rw-rw-r--   0 one       (1001) one       (1001)       38 2023-03-07 10:35:46.078187 pyone-6.6.1/setup.cfg
+-rw-r--r--   0 one       (1001) one       (1001)     2495 2023-03-07 10:22:11.000000 pyone-6.6.1/setup.py
```

### Comparing `pyone-6.6.0/PKG-INFO` & `pyone-6.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyone
-Version: 6.6.0
+Version: 6.6.1
 Summary: Python Bindings for OpenNebula XML-RPC API
 Home-page: http://opennebula.io
 Author: Rafael del Valle
 Author-email: rvalle@privaz.io
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: PyOne is an implementation of OpenNebula XML-RPC
                 bindings in Python. It works as a proxy over the XML-RPC api and
```

### Comparing `pyone-6.6.0/pyone/__init__.py` & `pyone-6.6.1/pyone/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018 www.privaz.io Valletech AB
-# Copyright 2002-2022, OpenNebula Project, OpenNebula Systems
+# Copyright 2002-2023, OpenNebula Project, OpenNebula Systems
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pyone-6.6.0/pyone/acl.py` & `pyone-6.6.1/pyone/acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2020 FELDSAM s.r.o. (www.feldhost.net)
-# Copyright 2002-2022, OpenNebula Project, OpenNebula Systems
+# Copyright 2002-2023, OpenNebula Project, OpenNebula Systems
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pyone-6.6.0/pyone/bindings/__init__.py` & `pyone-6.6.1/pyone/bindings/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 #
-# Generated Wed Dec 21 12:18:12 2022 by generateDS.py version 2.41.1.
+# Generated Tue Mar  7 10:35:44 2023 by generateDS.py version 2.41.3.
 # Python 3.8.10 (default, Nov 14 2022, 12:59:47)  [GCC 9.4.0]
 #
 # Command line options:
 #   ('-q', '')
 #   ('-f', '')
 #   ('-o', 'pyone/bindings/supbind.py')
 #   ('-s', 'pyone/bindings/__init__.py')
@@ -13,15 +13,15 @@
 #   ('--external-encoding', 'utf-8')
 #   ('--silence', '')
 #
 # Command line arguments:
 #   ../../../share/doc/xsd/index.xsd
 #
 # Command line:
-#   /home/one/init-build-jenkins.MUCv2w/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
+#   /home/one/init-build-jenkins.T9TFrJ/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
 #
 # Current working directory (os.getcwd()):
 #   python
 #
 
 import os
 import sys
@@ -890,23 +890,23 @@
     def __init__(self, CPUS=None, DEDICATED=None, FREE=None, ID=None, **kwargs_):
         super(CORETypeSub, self).__init__(CPUS, DEDICATED, FREE, ID,  **kwargs_)
 supermod.COREType.subclass = CORETypeSub
 # end class CORETypeSub
 
 
 class HUGEPAGETypeSub(TemplatedType, supermod.HUGEPAGEType):
-    def __init__(self, FREE=None, PAGES=None, SIZE=None, USAGE=None, **kwargs_):
-        super(HUGEPAGETypeSub, self).__init__(FREE, PAGES, SIZE, USAGE,  **kwargs_)
+    def __init__(self, PAGES=None, SIZE=None, USAGE=None, **kwargs_):
+        super(HUGEPAGETypeSub, self).__init__(PAGES, SIZE, USAGE,  **kwargs_)
 supermod.HUGEPAGEType.subclass = HUGEPAGETypeSub
 # end class HUGEPAGETypeSub
 
 
 class MEMORYTypeSub(TemplatedType, supermod.MEMORYType):
-    def __init__(self, DISTANCE=None, FREE=None, TOTAL=None, USAGE=None, USED=None, **kwargs_):
-        super(MEMORYTypeSub, self).__init__(DISTANCE, FREE, TOTAL, USAGE, USED,  **kwargs_)
+    def __init__(self, DISTANCE=None, TOTAL=None, USAGE=None, **kwargs_):
+        super(MEMORYTypeSub, self).__init__(DISTANCE, TOTAL, USAGE,  **kwargs_)
 supermod.MEMORYType.subclass = MEMORYTypeSub
 # end class MEMORYTypeSub
 
 
 class VMSTypeSub(TemplatedType, supermod.VMSType):
     def __init__(self, ID=None, **kwargs_):
         super(VMSTypeSub, self).__init__(ID,  **kwargs_)
@@ -918,16 +918,16 @@
     def __init__(self, VCENTER_CCR_REF=None, VCENTER_DS_REF=None, VCENTER_HOST=None, VCENTER_INSTANCE_ID=None, VCENTER_NAME=None, VCENTER_PASSWORD=None, VCENTER_RESOURCE_POOL_INFO=None, VCENTER_USER=None, VCENTER_VERSION=None, anytypeobjs_=None, **kwargs_):
         super(TEMPLATEType33Sub, self).__init__(VCENTER_CCR_REF, VCENTER_DS_REF, VCENTER_HOST, VCENTER_INSTANCE_ID, VCENTER_NAME, VCENTER_PASSWORD, VCENTER_RESOURCE_POOL_INFO, VCENTER_USER, VCENTER_VERSION, anytypeobjs_,  **kwargs_)
 supermod.TEMPLATEType33.subclass = TEMPLATEType33Sub
 # end class TEMPLATEType33Sub
 
 
 class MONITORINGTypeSub(TemplatedType, supermod.MONITORINGType):
-    def __init__(self, TIMESTAMP=None, ID=None, CAPACITY=None, SYSTEM=None, **kwargs_):
-        super(MONITORINGTypeSub, self).__init__(TIMESTAMP, ID, CAPACITY, SYSTEM,  **kwargs_)
+    def __init__(self, TIMESTAMP=None, ID=None, CAPACITY=None, SYSTEM=None, NUMA_NODE=None, **kwargs_):
+        super(MONITORINGTypeSub, self).__init__(TIMESTAMP, ID, CAPACITY, SYSTEM, NUMA_NODE,  **kwargs_)
 supermod.MONITORINGType.subclass = MONITORINGTypeSub
 # end class MONITORINGTypeSub
 
 
 class CAPACITYTypeSub(TemplatedType, supermod.CAPACITYType):
     def __init__(self, FREE_CPU=None, FREE_MEMORY=None, USED_CPU=None, USED_MEMORY=None, **kwargs_):
         super(CAPACITYTypeSub, self).__init__(FREE_CPU, FREE_MEMORY, USED_CPU, USED_MEMORY,  **kwargs_)
@@ -938,33 +938,54 @@
 class SYSTEMTypeSub(TemplatedType, supermod.SYSTEMType):
     def __init__(self, NETRX=None, NETTX=None, **kwargs_):
         super(SYSTEMTypeSub, self).__init__(NETRX, NETTX,  **kwargs_)
 supermod.SYSTEMType.subclass = SYSTEMTypeSub
 # end class SYSTEMTypeSub
 
 
-class LOCKType34Sub(TemplatedType, supermod.LOCKType34):
+class NUMA_NODETypeSub(TemplatedType, supermod.NUMA_NODEType):
+    def __init__(self, HUGEPAGE=None, MEMORY=None, NODE_ID=None, **kwargs_):
+        super(NUMA_NODETypeSub, self).__init__(HUGEPAGE, MEMORY, NODE_ID,  **kwargs_)
+supermod.NUMA_NODEType.subclass = NUMA_NODETypeSub
+# end class NUMA_NODETypeSub
+
+
+class HUGEPAGEType34Sub(TemplatedType, supermod.HUGEPAGEType34):
+    def __init__(self, FREE=None, SIZE=None, **kwargs_):
+        super(HUGEPAGEType34Sub, self).__init__(FREE, SIZE,  **kwargs_)
+supermod.HUGEPAGEType34.subclass = HUGEPAGEType34Sub
+# end class HUGEPAGEType34Sub
+
+
+class MEMORYType35Sub(TemplatedType, supermod.MEMORYType35):
+    def __init__(self, FREE=None, USED=None, **kwargs_):
+        super(MEMORYType35Sub, self).__init__(FREE, USED,  **kwargs_)
+supermod.MEMORYType35.subclass = MEMORYType35Sub
+# end class MEMORYType35Sub
+
+
+class LOCKType36Sub(TemplatedType, supermod.LOCKType36):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType34Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType34.subclass = LOCKType34Sub
-# end class LOCKType34Sub
+        super(LOCKType36Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType36.subclass = LOCKType36Sub
+# end class LOCKType36Sub
 
 
-class PERMISSIONSType35Sub(TemplatedType, supermod.PERMISSIONSType35):
+class PERMISSIONSType37Sub(TemplatedType, supermod.PERMISSIONSType37):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType35Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType35.subclass = PERMISSIONSType35Sub
-# end class PERMISSIONSType35Sub
+        super(PERMISSIONSType37Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType37.subclass = PERMISSIONSType37Sub
+# end class PERMISSIONSType37Sub
 
 
-class VMSType36Sub(TemplatedType, supermod.VMSType36):
+class VMSType38Sub(TemplatedType, supermod.VMSType38):
     def __init__(self, ID=None, **kwargs_):
-        super(VMSType36Sub, self).__init__(ID,  **kwargs_)
-supermod.VMSType36.subclass = VMSType36Sub
-# end class VMSType36Sub
+        super(VMSType38Sub, self).__init__(ID,  **kwargs_)
+supermod.VMSType38.subclass = VMSType38Sub
+# end class VMSType38Sub
 
 
 class CLONESTypeSub(TemplatedType, supermod.CLONESType):
     def __init__(self, ID=None, **kwargs_):
         super(CLONESTypeSub, self).__init__(ID,  **kwargs_)
 supermod.CLONESType.subclass = CLONESTypeSub
 # end class CLONESTypeSub
@@ -973,33 +994,33 @@
 class APP_CLONESTypeSub(TemplatedType, supermod.APP_CLONESType):
     def __init__(self, ID=None, **kwargs_):
         super(APP_CLONESTypeSub, self).__init__(ID,  **kwargs_)
 supermod.APP_CLONESType.subclass = APP_CLONESTypeSub
 # end class APP_CLONESTypeSub
 
 
-class TEMPLATEType37Sub(TemplatedType, supermod.TEMPLATEType37):
+class TEMPLATEType39Sub(TemplatedType, supermod.TEMPLATEType39):
     def __init__(self, VCENTER_IMPORTED=None, anytypeobjs_=None, **kwargs_):
-        super(TEMPLATEType37Sub, self).__init__(VCENTER_IMPORTED, anytypeobjs_,  **kwargs_)
-supermod.TEMPLATEType37.subclass = TEMPLATEType37Sub
-# end class TEMPLATEType37Sub
+        super(TEMPLATEType39Sub, self).__init__(VCENTER_IMPORTED, anytypeobjs_,  **kwargs_)
+supermod.TEMPLATEType39.subclass = TEMPLATEType39Sub
+# end class TEMPLATEType39Sub
 
 
-class SNAPSHOTSType38Sub(TemplatedType, supermod.SNAPSHOTSType38):
+class SNAPSHOTSType40Sub(TemplatedType, supermod.SNAPSHOTSType40):
     def __init__(self, ALLOW_ORPHANS=None, CURRENT_BASE=None, NEXT_SNAPSHOT=None, SNAPSHOT=None, **kwargs_):
-        super(SNAPSHOTSType38Sub, self).__init__(ALLOW_ORPHANS, CURRENT_BASE, NEXT_SNAPSHOT, SNAPSHOT,  **kwargs_)
-supermod.SNAPSHOTSType38.subclass = SNAPSHOTSType38Sub
-# end class SNAPSHOTSType38Sub
+        super(SNAPSHOTSType40Sub, self).__init__(ALLOW_ORPHANS, CURRENT_BASE, NEXT_SNAPSHOT, SNAPSHOT,  **kwargs_)
+supermod.SNAPSHOTSType40.subclass = SNAPSHOTSType40Sub
+# end class SNAPSHOTSType40Sub
 
 
-class SNAPSHOTType39Sub(TemplatedType, supermod.SNAPSHOTType39):
+class SNAPSHOTType41Sub(TemplatedType, supermod.SNAPSHOTType41):
     def __init__(self, CHILDREN=None, ACTIVE=None, DATE=None, ID=None, NAME=None, PARENT=None, SIZE=None, **kwargs_):
-        super(SNAPSHOTType39Sub, self).__init__(CHILDREN, ACTIVE, DATE, ID, NAME, PARENT, SIZE,  **kwargs_)
-supermod.SNAPSHOTType39.subclass = SNAPSHOTType39Sub
-# end class SNAPSHOTType39Sub
+        super(SNAPSHOTType41Sub, self).__init__(CHILDREN, ACTIVE, DATE, ID, NAME, PARENT, SIZE,  **kwargs_)
+supermod.SNAPSHOTType41.subclass = SNAPSHOTType41Sub
+# end class SNAPSHOTType41Sub
 
 
 class BACKUP_INCREMENTSTypeSub(TemplatedType, supermod.BACKUP_INCREMENTSType):
     def __init__(self, INCREMENT=None, **kwargs_):
         super(BACKUP_INCREMENTSTypeSub, self).__init__(INCREMENT,  **kwargs_)
 supermod.BACKUP_INCREMENTSType.subclass = BACKUP_INCREMENTSTypeSub
 # end class BACKUP_INCREMENTSTypeSub
@@ -1008,47 +1029,47 @@
 class INCREMENTTypeSub(TemplatedType, supermod.INCREMENTType):
     def __init__(self, DATE=None, ID=None, PARENT_ID=None, SIZE=None, SOURCE=None, TYPE=None, **kwargs_):
         super(INCREMENTTypeSub, self).__init__(DATE, ID, PARENT_ID, SIZE, SOURCE, TYPE,  **kwargs_)
 supermod.INCREMENTType.subclass = INCREMENTTypeSub
 # end class INCREMENTTypeSub
 
 
-class LOCKType40Sub(TemplatedType, supermod.LOCKType40):
+class LOCKType42Sub(TemplatedType, supermod.LOCKType42):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType40Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType40.subclass = LOCKType40Sub
-# end class LOCKType40Sub
+        super(LOCKType42Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType42.subclass = LOCKType42Sub
+# end class LOCKType42Sub
 
 
-class PERMISSIONSType41Sub(TemplatedType, supermod.PERMISSIONSType41):
+class PERMISSIONSType43Sub(TemplatedType, supermod.PERMISSIONSType43):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType41Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType41.subclass = PERMISSIONSType41Sub
-# end class PERMISSIONSType41Sub
+        super(PERMISSIONSType43Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType43.subclass = PERMISSIONSType43Sub
+# end class PERMISSIONSType43Sub
 
 
 class MARKETPLACEAPPSTypeSub(TemplatedType, supermod.MARKETPLACEAPPSType):
     def __init__(self, ID=None, **kwargs_):
         super(MARKETPLACEAPPSTypeSub, self).__init__(ID,  **kwargs_)
 supermod.MARKETPLACEAPPSType.subclass = MARKETPLACEAPPSTypeSub
 # end class MARKETPLACEAPPSTypeSub
 
 
-class PERMISSIONSType42Sub(TemplatedType, supermod.PERMISSIONSType42):
+class PERMISSIONSType44Sub(TemplatedType, supermod.PERMISSIONSType44):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType42Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType42.subclass = PERMISSIONSType42Sub
-# end class PERMISSIONSType42Sub
+        super(PERMISSIONSType44Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType44.subclass = PERMISSIONSType44Sub
+# end class PERMISSIONSType44Sub
 
 
-class MONITORINGType43Sub(TemplatedType, supermod.MONITORINGType43):
+class MONITORINGType45Sub(TemplatedType, supermod.MONITORINGType45):
     def __init__(self, CPU=None, DISKRDBYTES=None, DISKRDIOPS=None, DISKWRBYTES=None, DISKWRIOPS=None, DISK_SIZE=None, ID=None, MEMORY=None, NETRX=None, NETTX=None, TIMESTAMP=None, VCENTER_ESX_HOST=None, VCENTER_GUEST_STATE=None, VCENTER_RP_NAME=None, VCENTER_VMWARETOOLS_RUNNING_STATUS=None, VCENTER_VMWARETOOLS_VERSION=None, VCENTER_VMWARETOOLS_VERSION_STATUS=None, VCENTER_VM_NAME=None, **kwargs_):
-        super(MONITORINGType43Sub, self).__init__(CPU, DISKRDBYTES, DISKRDIOPS, DISKWRBYTES, DISKWRIOPS, DISK_SIZE, ID, MEMORY, NETRX, NETTX, TIMESTAMP, VCENTER_ESX_HOST, VCENTER_GUEST_STATE, VCENTER_RP_NAME, VCENTER_VMWARETOOLS_RUNNING_STATUS, VCENTER_VMWARETOOLS_VERSION, VCENTER_VMWARETOOLS_VERSION_STATUS, VCENTER_VM_NAME,  **kwargs_)
-supermod.MONITORINGType43.subclass = MONITORINGType43Sub
-# end class MONITORINGType43Sub
+        super(MONITORINGType45Sub, self).__init__(CPU, DISKRDBYTES, DISKRDIOPS, DISKWRBYTES, DISKWRIOPS, DISK_SIZE, ID, MEMORY, NETRX, NETTX, TIMESTAMP, VCENTER_ESX_HOST, VCENTER_GUEST_STATE, VCENTER_RP_NAME, VCENTER_VMWARETOOLS_RUNNING_STATUS, VCENTER_VMWARETOOLS_VERSION, VCENTER_VMWARETOOLS_VERSION_STATUS, VCENTER_VM_NAME,  **kwargs_)
+supermod.MONITORINGType45.subclass = MONITORINGType45Sub
+# end class MONITORINGType45Sub
 
 
 class DISK_SIZETypeSub(TemplatedType, supermod.DISK_SIZEType):
     def __init__(self, ID=None, SIZE=None, **kwargs_):
         super(DISK_SIZETypeSub, self).__init__(ID, SIZE,  **kwargs_)
 supermod.DISK_SIZEType.subclass = DISK_SIZETypeSub
 # end class DISK_SIZETypeSub
@@ -1204,19 +1225,19 @@
 class VXLAN_IDSTypeSub(TemplatedType, supermod.VXLAN_IDSType):
     def __init__(self, START=None, **kwargs_):
         super(VXLAN_IDSTypeSub, self).__init__(START,  **kwargs_)
 supermod.VXLAN_IDSType.subclass = VXLAN_IDSTypeSub
 # end class VXLAN_IDSTypeSub
 
 
-class PERMISSIONSType44Sub(TemplatedType, supermod.PERMISSIONSType44):
+class PERMISSIONSType46Sub(TemplatedType, supermod.PERMISSIONSType46):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType44Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType44.subclass = PERMISSIONSType44Sub
-# end class PERMISSIONSType44Sub
+        super(PERMISSIONSType46Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType46.subclass = PERMISSIONSType46Sub
+# end class PERMISSIONSType46Sub
 
 
 class UPDATED_VMSTypeSub(TemplatedType, supermod.UPDATED_VMSType):
     def __init__(self, ID=None, **kwargs_):
         super(UPDATED_VMSTypeSub, self).__init__(ID,  **kwargs_)
 supermod.UPDATED_VMSType.subclass = UPDATED_VMSTypeSub
 # end class UPDATED_VMSTypeSub
@@ -1239,19 +1260,19 @@
 class ERROR_VMSTypeSub(TemplatedType, supermod.ERROR_VMSType):
     def __init__(self, ID=None, **kwargs_):
         super(ERROR_VMSTypeSub, self).__init__(ID,  **kwargs_)
 supermod.ERROR_VMSType.subclass = ERROR_VMSTypeSub
 # end class ERROR_VMSTypeSub
 
 
-class TEMPLATEType45Sub(TemplatedType, supermod.TEMPLATEType45):
+class TEMPLATEType47Sub(TemplatedType, supermod.TEMPLATEType47):
     def __init__(self, DESCRIPTION=None, RULE=None, anytypeobjs_=None, **kwargs_):
-        super(TEMPLATEType45Sub, self).__init__(DESCRIPTION, RULE, anytypeobjs_,  **kwargs_)
-supermod.TEMPLATEType45.subclass = TEMPLATEType45Sub
-# end class TEMPLATEType45Sub
+        super(TEMPLATEType47Sub, self).__init__(DESCRIPTION, RULE, anytypeobjs_,  **kwargs_)
+supermod.TEMPLATEType47.subclass = TEMPLATEType47Sub
+# end class TEMPLATEType47Sub
 
 
 class RULETypeSub(TemplatedType, supermod.RULEType):
     def __init__(self, PROTOCOL=None, RULE_TYPE=None, **kwargs_):
         super(RULETypeSub, self).__init__(PROTOCOL, RULE_TYPE,  **kwargs_)
 supermod.RULEType.subclass = RULETypeSub
 # end class RULETypeSub
@@ -1281,348 +1302,348 @@
 class LOGIN_TOKENTypeSub(TemplatedType, supermod.LOGIN_TOKENType):
     def __init__(self, TOKEN=None, EXPIRATION_TIME=None, EGID=None, **kwargs_):
         super(LOGIN_TOKENTypeSub, self).__init__(TOKEN, EXPIRATION_TIME, EGID,  **kwargs_)
 supermod.LOGIN_TOKENType.subclass = LOGIN_TOKENTypeSub
 # end class LOGIN_TOKENTypeSub
 
 
-class QUOTASType46Sub(TemplatedType, supermod.QUOTASType46):
+class QUOTASType48Sub(TemplatedType, supermod.QUOTASType48):
     def __init__(self, ID=None, DATASTORE_QUOTA=None, NETWORK_QUOTA=None, VM_QUOTA=None, IMAGE_QUOTA=None, **kwargs_):
-        super(QUOTASType46Sub, self).__init__(ID, DATASTORE_QUOTA, NETWORK_QUOTA, VM_QUOTA, IMAGE_QUOTA,  **kwargs_)
-supermod.QUOTASType46.subclass = QUOTASType46Sub
-# end class QUOTASType46Sub
+        super(QUOTASType48Sub, self).__init__(ID, DATASTORE_QUOTA, NETWORK_QUOTA, VM_QUOTA, IMAGE_QUOTA,  **kwargs_)
+supermod.QUOTASType48.subclass = QUOTASType48Sub
+# end class QUOTASType48Sub
 
 
-class DATASTORE_QUOTAType47Sub(TemplatedType, supermod.DATASTORE_QUOTAType47):
+class DATASTORE_QUOTAType49Sub(TemplatedType, supermod.DATASTORE_QUOTAType49):
     def __init__(self, DATASTORE=None, **kwargs_):
-        super(DATASTORE_QUOTAType47Sub, self).__init__(DATASTORE,  **kwargs_)
-supermod.DATASTORE_QUOTAType47.subclass = DATASTORE_QUOTAType47Sub
-# end class DATASTORE_QUOTAType47Sub
+        super(DATASTORE_QUOTAType49Sub, self).__init__(DATASTORE,  **kwargs_)
+supermod.DATASTORE_QUOTAType49.subclass = DATASTORE_QUOTAType49Sub
+# end class DATASTORE_QUOTAType49Sub
 
 
-class DATASTOREType48Sub(TemplatedType, supermod.DATASTOREType48):
+class DATASTOREType50Sub(TemplatedType, supermod.DATASTOREType50):
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, **kwargs_):
-        super(DATASTOREType48Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
-supermod.DATASTOREType48.subclass = DATASTOREType48Sub
-# end class DATASTOREType48Sub
+        super(DATASTOREType50Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
+supermod.DATASTOREType50.subclass = DATASTOREType50Sub
+# end class DATASTOREType50Sub
 
 
-class NETWORK_QUOTAType49Sub(TemplatedType, supermod.NETWORK_QUOTAType49):
+class NETWORK_QUOTAType51Sub(TemplatedType, supermod.NETWORK_QUOTAType51):
     def __init__(self, NETWORK=None, **kwargs_):
-        super(NETWORK_QUOTAType49Sub, self).__init__(NETWORK,  **kwargs_)
-supermod.NETWORK_QUOTAType49.subclass = NETWORK_QUOTAType49Sub
-# end class NETWORK_QUOTAType49Sub
+        super(NETWORK_QUOTAType51Sub, self).__init__(NETWORK,  **kwargs_)
+supermod.NETWORK_QUOTAType51.subclass = NETWORK_QUOTAType51Sub
+# end class NETWORK_QUOTAType51Sub
 
 
-class NETWORKType50Sub(TemplatedType, supermod.NETWORKType50):
+class NETWORKType52Sub(TemplatedType, supermod.NETWORKType52):
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, **kwargs_):
-        super(NETWORKType50Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
-supermod.NETWORKType50.subclass = NETWORKType50Sub
-# end class NETWORKType50Sub
+        super(NETWORKType52Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
+supermod.NETWORKType52.subclass = NETWORKType52Sub
+# end class NETWORKType52Sub
 
 
-class VM_QUOTAType51Sub(TemplatedType, supermod.VM_QUOTAType51):
+class VM_QUOTAType53Sub(TemplatedType, supermod.VM_QUOTAType53):
     def __init__(self, VM=None, **kwargs_):
-        super(VM_QUOTAType51Sub, self).__init__(VM,  **kwargs_)
-supermod.VM_QUOTAType51.subclass = VM_QUOTAType51Sub
-# end class VM_QUOTAType51Sub
+        super(VM_QUOTAType53Sub, self).__init__(VM,  **kwargs_)
+supermod.VM_QUOTAType53.subclass = VM_QUOTAType53Sub
+# end class VM_QUOTAType53Sub
 
 
-class VMType52Sub(TemplatedType, supermod.VMType52):
+class VMType54Sub(TemplatedType, supermod.VMType54):
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, **kwargs_):
-        super(VMType52Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
-supermod.VMType52.subclass = VMType52Sub
-# end class VMType52Sub
+        super(VMType54Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
+supermod.VMType54.subclass = VMType54Sub
+# end class VMType54Sub
 
 
-class IMAGE_QUOTAType53Sub(TemplatedType, supermod.IMAGE_QUOTAType53):
+class IMAGE_QUOTAType55Sub(TemplatedType, supermod.IMAGE_QUOTAType55):
     def __init__(self, IMAGE=None, **kwargs_):
-        super(IMAGE_QUOTAType53Sub, self).__init__(IMAGE,  **kwargs_)
-supermod.IMAGE_QUOTAType53.subclass = IMAGE_QUOTAType53Sub
-# end class IMAGE_QUOTAType53Sub
+        super(IMAGE_QUOTAType55Sub, self).__init__(IMAGE,  **kwargs_)
+supermod.IMAGE_QUOTAType55.subclass = IMAGE_QUOTAType55Sub
+# end class IMAGE_QUOTAType55Sub
 
 
-class IMAGEType54Sub(TemplatedType, supermod.IMAGEType54):
+class IMAGEType56Sub(TemplatedType, supermod.IMAGEType56):
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, **kwargs_):
-        super(IMAGEType54Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
-supermod.IMAGEType54.subclass = IMAGEType54Sub
-# end class IMAGEType54Sub
+        super(IMAGEType56Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
+supermod.IMAGEType56.subclass = IMAGEType56Sub
+# end class IMAGEType56Sub
 
 
 class DEFAULT_USER_QUOTASTypeSub(TemplatedType, supermod.DEFAULT_USER_QUOTASType):
     def __init__(self, DATASTORE_QUOTA=None, NETWORK_QUOTA=None, VM_QUOTA=None, IMAGE_QUOTA=None, **kwargs_):
         super(DEFAULT_USER_QUOTASTypeSub, self).__init__(DATASTORE_QUOTA, NETWORK_QUOTA, VM_QUOTA, IMAGE_QUOTA,  **kwargs_)
 supermod.DEFAULT_USER_QUOTASType.subclass = DEFAULT_USER_QUOTASTypeSub
 # end class DEFAULT_USER_QUOTASTypeSub
 
 
-class DATASTORE_QUOTAType55Sub(TemplatedType, supermod.DATASTORE_QUOTAType55):
+class DATASTORE_QUOTAType57Sub(TemplatedType, supermod.DATASTORE_QUOTAType57):
     def __init__(self, DATASTORE=None, **kwargs_):
-        super(DATASTORE_QUOTAType55Sub, self).__init__(DATASTORE,  **kwargs_)
-supermod.DATASTORE_QUOTAType55.subclass = DATASTORE_QUOTAType55Sub
-# end class DATASTORE_QUOTAType55Sub
+        super(DATASTORE_QUOTAType57Sub, self).__init__(DATASTORE,  **kwargs_)
+supermod.DATASTORE_QUOTAType57.subclass = DATASTORE_QUOTAType57Sub
+# end class DATASTORE_QUOTAType57Sub
 
 
-class DATASTOREType56Sub(TemplatedType, supermod.DATASTOREType56):
+class DATASTOREType58Sub(TemplatedType, supermod.DATASTOREType58):
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, **kwargs_):
-        super(DATASTOREType56Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
-supermod.DATASTOREType56.subclass = DATASTOREType56Sub
-# end class DATASTOREType56Sub
+        super(DATASTOREType58Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
+supermod.DATASTOREType58.subclass = DATASTOREType58Sub
+# end class DATASTOREType58Sub
 
 
-class NETWORK_QUOTAType57Sub(TemplatedType, supermod.NETWORK_QUOTAType57):
+class NETWORK_QUOTAType59Sub(TemplatedType, supermod.NETWORK_QUOTAType59):
     def __init__(self, NETWORK=None, **kwargs_):
-        super(NETWORK_QUOTAType57Sub, self).__init__(NETWORK,  **kwargs_)
-supermod.NETWORK_QUOTAType57.subclass = NETWORK_QUOTAType57Sub
-# end class NETWORK_QUOTAType57Sub
+        super(NETWORK_QUOTAType59Sub, self).__init__(NETWORK,  **kwargs_)
+supermod.NETWORK_QUOTAType59.subclass = NETWORK_QUOTAType59Sub
+# end class NETWORK_QUOTAType59Sub
 
 
-class NETWORKType58Sub(TemplatedType, supermod.NETWORKType58):
+class NETWORKType60Sub(TemplatedType, supermod.NETWORKType60):
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, **kwargs_):
-        super(NETWORKType58Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
-supermod.NETWORKType58.subclass = NETWORKType58Sub
-# end class NETWORKType58Sub
+        super(NETWORKType60Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
+supermod.NETWORKType60.subclass = NETWORKType60Sub
+# end class NETWORKType60Sub
 
 
-class VM_QUOTAType59Sub(TemplatedType, supermod.VM_QUOTAType59):
+class VM_QUOTAType61Sub(TemplatedType, supermod.VM_QUOTAType61):
     def __init__(self, VM=None, **kwargs_):
-        super(VM_QUOTAType59Sub, self).__init__(VM,  **kwargs_)
-supermod.VM_QUOTAType59.subclass = VM_QUOTAType59Sub
-# end class VM_QUOTAType59Sub
+        super(VM_QUOTAType61Sub, self).__init__(VM,  **kwargs_)
+supermod.VM_QUOTAType61.subclass = VM_QUOTAType61Sub
+# end class VM_QUOTAType61Sub
 
 
-class VMType60Sub(TemplatedType, supermod.VMType60):
+class VMType62Sub(TemplatedType, supermod.VMType62):
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, **kwargs_):
-        super(VMType60Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
-supermod.VMType60.subclass = VMType60Sub
-# end class VMType60Sub
+        super(VMType62Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
+supermod.VMType62.subclass = VMType62Sub
+# end class VMType62Sub
 
 
-class IMAGE_QUOTAType61Sub(TemplatedType, supermod.IMAGE_QUOTAType61):
+class IMAGE_QUOTAType63Sub(TemplatedType, supermod.IMAGE_QUOTAType63):
     def __init__(self, IMAGE=None, **kwargs_):
-        super(IMAGE_QUOTAType61Sub, self).__init__(IMAGE,  **kwargs_)
-supermod.IMAGE_QUOTAType61.subclass = IMAGE_QUOTAType61Sub
-# end class IMAGE_QUOTAType61Sub
+        super(IMAGE_QUOTAType63Sub, self).__init__(IMAGE,  **kwargs_)
+supermod.IMAGE_QUOTAType63.subclass = IMAGE_QUOTAType63Sub
+# end class IMAGE_QUOTAType63Sub
 
 
-class IMAGEType62Sub(TemplatedType, supermod.IMAGEType62):
+class IMAGEType64Sub(TemplatedType, supermod.IMAGEType64):
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, **kwargs_):
-        super(IMAGEType62Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
-supermod.IMAGEType62.subclass = IMAGEType62Sub
-# end class IMAGEType62Sub
+        super(IMAGEType64Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
+supermod.IMAGEType64.subclass = IMAGEType64Sub
+# end class IMAGEType64Sub
 
 
-class GROUPSType63Sub(TemplatedType, supermod.GROUPSType63):
+class GROUPSType65Sub(TemplatedType, supermod.GROUPSType65):
     def __init__(self, ID=None, **kwargs_):
-        super(GROUPSType63Sub, self).__init__(ID,  **kwargs_)
-supermod.GROUPSType63.subclass = GROUPSType63Sub
-# end class GROUPSType63Sub
+        super(GROUPSType65Sub, self).__init__(ID,  **kwargs_)
+supermod.GROUPSType65.subclass = GROUPSType65Sub
+# end class GROUPSType65Sub
 
 
-class LOGIN_TOKENType64Sub(TemplatedType, supermod.LOGIN_TOKENType64):
+class LOGIN_TOKENType66Sub(TemplatedType, supermod.LOGIN_TOKENType66):
     def __init__(self, TOKEN=None, EXPIRATION_TIME=None, EGID=None, **kwargs_):
-        super(LOGIN_TOKENType64Sub, self).__init__(TOKEN, EXPIRATION_TIME, EGID,  **kwargs_)
-supermod.LOGIN_TOKENType64.subclass = LOGIN_TOKENType64Sub
-# end class LOGIN_TOKENType64Sub
+        super(LOGIN_TOKENType66Sub, self).__init__(TOKEN, EXPIRATION_TIME, EGID,  **kwargs_)
+supermod.LOGIN_TOKENType66.subclass = LOGIN_TOKENType66Sub
+# end class LOGIN_TOKENType66Sub
 
 
-class DATASTORE_QUOTAType65Sub(TemplatedType, supermod.DATASTORE_QUOTAType65):
+class DATASTORE_QUOTAType67Sub(TemplatedType, supermod.DATASTORE_QUOTAType67):
     def __init__(self, DATASTORE=None, **kwargs_):
-        super(DATASTORE_QUOTAType65Sub, self).__init__(DATASTORE,  **kwargs_)
-supermod.DATASTORE_QUOTAType65.subclass = DATASTORE_QUOTAType65Sub
-# end class DATASTORE_QUOTAType65Sub
+        super(DATASTORE_QUOTAType67Sub, self).__init__(DATASTORE,  **kwargs_)
+supermod.DATASTORE_QUOTAType67.subclass = DATASTORE_QUOTAType67Sub
+# end class DATASTORE_QUOTAType67Sub
 
 
-class DATASTOREType66Sub(TemplatedType, supermod.DATASTOREType66):
+class DATASTOREType68Sub(TemplatedType, supermod.DATASTOREType68):
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, **kwargs_):
-        super(DATASTOREType66Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
-supermod.DATASTOREType66.subclass = DATASTOREType66Sub
-# end class DATASTOREType66Sub
+        super(DATASTOREType68Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
+supermod.DATASTOREType68.subclass = DATASTOREType68Sub
+# end class DATASTOREType68Sub
 
 
-class NETWORK_QUOTAType67Sub(TemplatedType, supermod.NETWORK_QUOTAType67):
+class NETWORK_QUOTAType69Sub(TemplatedType, supermod.NETWORK_QUOTAType69):
     def __init__(self, NETWORK=None, **kwargs_):
-        super(NETWORK_QUOTAType67Sub, self).__init__(NETWORK,  **kwargs_)
-supermod.NETWORK_QUOTAType67.subclass = NETWORK_QUOTAType67Sub
-# end class NETWORK_QUOTAType67Sub
+        super(NETWORK_QUOTAType69Sub, self).__init__(NETWORK,  **kwargs_)
+supermod.NETWORK_QUOTAType69.subclass = NETWORK_QUOTAType69Sub
+# end class NETWORK_QUOTAType69Sub
 
 
-class NETWORKType68Sub(TemplatedType, supermod.NETWORKType68):
+class NETWORKType70Sub(TemplatedType, supermod.NETWORKType70):
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, **kwargs_):
-        super(NETWORKType68Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
-supermod.NETWORKType68.subclass = NETWORKType68Sub
-# end class NETWORKType68Sub
+        super(NETWORKType70Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
+supermod.NETWORKType70.subclass = NETWORKType70Sub
+# end class NETWORKType70Sub
 
 
-class VM_QUOTAType69Sub(TemplatedType, supermod.VM_QUOTAType69):
+class VM_QUOTAType71Sub(TemplatedType, supermod.VM_QUOTAType71):
     def __init__(self, VM=None, **kwargs_):
-        super(VM_QUOTAType69Sub, self).__init__(VM,  **kwargs_)
-supermod.VM_QUOTAType69.subclass = VM_QUOTAType69Sub
-# end class VM_QUOTAType69Sub
+        super(VM_QUOTAType71Sub, self).__init__(VM,  **kwargs_)
+supermod.VM_QUOTAType71.subclass = VM_QUOTAType71Sub
+# end class VM_QUOTAType71Sub
 
 
-class VMType70Sub(TemplatedType, supermod.VMType70):
+class VMType72Sub(TemplatedType, supermod.VMType72):
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, **kwargs_):
-        super(VMType70Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
-supermod.VMType70.subclass = VMType70Sub
-# end class VMType70Sub
+        super(VMType72Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
+supermod.VMType72.subclass = VMType72Sub
+# end class VMType72Sub
 
 
-class IMAGE_QUOTAType71Sub(TemplatedType, supermod.IMAGE_QUOTAType71):
+class IMAGE_QUOTAType73Sub(TemplatedType, supermod.IMAGE_QUOTAType73):
     def __init__(self, IMAGE=None, **kwargs_):
-        super(IMAGE_QUOTAType71Sub, self).__init__(IMAGE,  **kwargs_)
-supermod.IMAGE_QUOTAType71.subclass = IMAGE_QUOTAType71Sub
-# end class IMAGE_QUOTAType71Sub
+        super(IMAGE_QUOTAType73Sub, self).__init__(IMAGE,  **kwargs_)
+supermod.IMAGE_QUOTAType73.subclass = IMAGE_QUOTAType73Sub
+# end class IMAGE_QUOTAType73Sub
 
 
-class IMAGEType72Sub(TemplatedType, supermod.IMAGEType72):
+class IMAGEType74Sub(TemplatedType, supermod.IMAGEType74):
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, **kwargs_):
-        super(IMAGEType72Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
-supermod.IMAGEType72.subclass = IMAGEType72Sub
-# end class IMAGEType72Sub
+        super(IMAGEType74Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
+supermod.IMAGEType74.subclass = IMAGEType74Sub
+# end class IMAGEType74Sub
 
 
-class DEFAULT_USER_QUOTASType73Sub(TemplatedType, supermod.DEFAULT_USER_QUOTASType73):
+class DEFAULT_USER_QUOTASType75Sub(TemplatedType, supermod.DEFAULT_USER_QUOTASType75):
     def __init__(self, DATASTORE_QUOTA=None, NETWORK_QUOTA=None, VM_QUOTA=None, IMAGE_QUOTA=None, **kwargs_):
-        super(DEFAULT_USER_QUOTASType73Sub, self).__init__(DATASTORE_QUOTA, NETWORK_QUOTA, VM_QUOTA, IMAGE_QUOTA,  **kwargs_)
-supermod.DEFAULT_USER_QUOTASType73.subclass = DEFAULT_USER_QUOTASType73Sub
-# end class DEFAULT_USER_QUOTASType73Sub
+        super(DEFAULT_USER_QUOTASType75Sub, self).__init__(DATASTORE_QUOTA, NETWORK_QUOTA, VM_QUOTA, IMAGE_QUOTA,  **kwargs_)
+supermod.DEFAULT_USER_QUOTASType75.subclass = DEFAULT_USER_QUOTASType75Sub
+# end class DEFAULT_USER_QUOTASType75Sub
 
 
-class DATASTORE_QUOTAType74Sub(TemplatedType, supermod.DATASTORE_QUOTAType74):
+class DATASTORE_QUOTAType76Sub(TemplatedType, supermod.DATASTORE_QUOTAType76):
     def __init__(self, DATASTORE=None, **kwargs_):
-        super(DATASTORE_QUOTAType74Sub, self).__init__(DATASTORE,  **kwargs_)
-supermod.DATASTORE_QUOTAType74.subclass = DATASTORE_QUOTAType74Sub
-# end class DATASTORE_QUOTAType74Sub
+        super(DATASTORE_QUOTAType76Sub, self).__init__(DATASTORE,  **kwargs_)
+supermod.DATASTORE_QUOTAType76.subclass = DATASTORE_QUOTAType76Sub
+# end class DATASTORE_QUOTAType76Sub
 
 
-class DATASTOREType75Sub(TemplatedType, supermod.DATASTOREType75):
+class DATASTOREType77Sub(TemplatedType, supermod.DATASTOREType77):
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, **kwargs_):
-        super(DATASTOREType75Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
-supermod.DATASTOREType75.subclass = DATASTOREType75Sub
-# end class DATASTOREType75Sub
+        super(DATASTOREType77Sub, self).__init__(ID, IMAGES, IMAGES_USED, SIZE, SIZE_USED,  **kwargs_)
+supermod.DATASTOREType77.subclass = DATASTOREType77Sub
+# end class DATASTOREType77Sub
 
 
-class NETWORK_QUOTAType76Sub(TemplatedType, supermod.NETWORK_QUOTAType76):
+class NETWORK_QUOTAType78Sub(TemplatedType, supermod.NETWORK_QUOTAType78):
     def __init__(self, NETWORK=None, **kwargs_):
-        super(NETWORK_QUOTAType76Sub, self).__init__(NETWORK,  **kwargs_)
-supermod.NETWORK_QUOTAType76.subclass = NETWORK_QUOTAType76Sub
-# end class NETWORK_QUOTAType76Sub
+        super(NETWORK_QUOTAType78Sub, self).__init__(NETWORK,  **kwargs_)
+supermod.NETWORK_QUOTAType78.subclass = NETWORK_QUOTAType78Sub
+# end class NETWORK_QUOTAType78Sub
 
 
-class NETWORKType77Sub(TemplatedType, supermod.NETWORKType77):
+class NETWORKType79Sub(TemplatedType, supermod.NETWORKType79):
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, **kwargs_):
-        super(NETWORKType77Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
-supermod.NETWORKType77.subclass = NETWORKType77Sub
-# end class NETWORKType77Sub
+        super(NETWORKType79Sub, self).__init__(ID, LEASES, LEASES_USED,  **kwargs_)
+supermod.NETWORKType79.subclass = NETWORKType79Sub
+# end class NETWORKType79Sub
 
 
-class VM_QUOTAType78Sub(TemplatedType, supermod.VM_QUOTAType78):
+class VM_QUOTAType80Sub(TemplatedType, supermod.VM_QUOTAType80):
     def __init__(self, VM=None, **kwargs_):
-        super(VM_QUOTAType78Sub, self).__init__(VM,  **kwargs_)
-supermod.VM_QUOTAType78.subclass = VM_QUOTAType78Sub
-# end class VM_QUOTAType78Sub
+        super(VM_QUOTAType80Sub, self).__init__(VM,  **kwargs_)
+supermod.VM_QUOTAType80.subclass = VM_QUOTAType80Sub
+# end class VM_QUOTAType80Sub
 
 
-class VMType79Sub(TemplatedType, supermod.VMType79):
+class VMType81Sub(TemplatedType, supermod.VMType81):
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, **kwargs_):
-        super(VMType79Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
-supermod.VMType79.subclass = VMType79Sub
-# end class VMType79Sub
+        super(VMType81Sub, self).__init__(CPU, CPU_USED, MEMORY, MEMORY_USED, RUNNING_CPU, RUNNING_CPU_USED, RUNNING_MEMORY, RUNNING_MEMORY_USED, RUNNING_VMS, RUNNING_VMS_USED, SYSTEM_DISK_SIZE, SYSTEM_DISK_SIZE_USED, VMS, VMS_USED,  **kwargs_)
+supermod.VMType81.subclass = VMType81Sub
+# end class VMType81Sub
 
 
-class IMAGE_QUOTAType80Sub(TemplatedType, supermod.IMAGE_QUOTAType80):
+class IMAGE_QUOTAType82Sub(TemplatedType, supermod.IMAGE_QUOTAType82):
     def __init__(self, IMAGE=None, **kwargs_):
-        super(IMAGE_QUOTAType80Sub, self).__init__(IMAGE,  **kwargs_)
-supermod.IMAGE_QUOTAType80.subclass = IMAGE_QUOTAType80Sub
-# end class IMAGE_QUOTAType80Sub
+        super(IMAGE_QUOTAType82Sub, self).__init__(IMAGE,  **kwargs_)
+supermod.IMAGE_QUOTAType82.subclass = IMAGE_QUOTAType82Sub
+# end class IMAGE_QUOTAType82Sub
 
 
-class IMAGEType81Sub(TemplatedType, supermod.IMAGEType81):
+class IMAGEType83Sub(TemplatedType, supermod.IMAGEType83):
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, **kwargs_):
-        super(IMAGEType81Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
-supermod.IMAGEType81.subclass = IMAGEType81Sub
-# end class IMAGEType81Sub
+        super(IMAGEType83Sub, self).__init__(ID, RVMS, RVMS_USED,  **kwargs_)
+supermod.IMAGEType83.subclass = IMAGEType83Sub
+# end class IMAGEType83Sub
 
 
-class GROUPSType82Sub(TemplatedType, supermod.GROUPSType82):
+class GROUPSType84Sub(TemplatedType, supermod.GROUPSType84):
     def __init__(self, ID=None, **kwargs_):
-        super(GROUPSType82Sub, self).__init__(ID,  **kwargs_)
-supermod.GROUPSType82.subclass = GROUPSType82Sub
-# end class GROUPSType82Sub
+        super(GROUPSType84Sub, self).__init__(ID,  **kwargs_)
+supermod.GROUPSType84.subclass = GROUPSType84Sub
+# end class GROUPSType84Sub
 
 
-class CLUSTERSType83Sub(TemplatedType, supermod.CLUSTERSType83):
+class CLUSTERSType85Sub(TemplatedType, supermod.CLUSTERSType85):
     def __init__(self, CLUSTER=None, **kwargs_):
-        super(CLUSTERSType83Sub, self).__init__(CLUSTER,  **kwargs_)
-supermod.CLUSTERSType83.subclass = CLUSTERSType83Sub
-# end class CLUSTERSType83Sub
+        super(CLUSTERSType85Sub, self).__init__(CLUSTER,  **kwargs_)
+supermod.CLUSTERSType85.subclass = CLUSTERSType85Sub
+# end class CLUSTERSType85Sub
 
 
 class CLUSTERTypeSub(TemplatedType, supermod.CLUSTERType):
     def __init__(self, ZONE_ID=None, CLUSTER_ID=None, **kwargs_):
         super(CLUSTERTypeSub, self).__init__(ZONE_ID, CLUSTER_ID,  **kwargs_)
 supermod.CLUSTERType.subclass = CLUSTERTypeSub
 # end class CLUSTERTypeSub
 
 
-class HOSTSType84Sub(TemplatedType, supermod.HOSTSType84):
+class HOSTSType86Sub(TemplatedType, supermod.HOSTSType86):
     def __init__(self, HOST=None, **kwargs_):
-        super(HOSTSType84Sub, self).__init__(HOST,  **kwargs_)
-supermod.HOSTSType84.subclass = HOSTSType84Sub
-# end class HOSTSType84Sub
+        super(HOSTSType86Sub, self).__init__(HOST,  **kwargs_)
+supermod.HOSTSType86.subclass = HOSTSType86Sub
+# end class HOSTSType86Sub
 
 
 class HOSTTypeSub(TemplatedType, supermod.HOSTType):
     def __init__(self, ZONE_ID=None, HOST_ID=None, **kwargs_):
         super(HOSTTypeSub, self).__init__(ZONE_ID, HOST_ID,  **kwargs_)
 supermod.HOSTType.subclass = HOSTTypeSub
 # end class HOSTTypeSub
 
 
-class DATASTORESType85Sub(TemplatedType, supermod.DATASTORESType85):
+class DATASTORESType87Sub(TemplatedType, supermod.DATASTORESType87):
     def __init__(self, DATASTORE=None, **kwargs_):
-        super(DATASTORESType85Sub, self).__init__(DATASTORE,  **kwargs_)
-supermod.DATASTORESType85.subclass = DATASTORESType85Sub
-# end class DATASTORESType85Sub
+        super(DATASTORESType87Sub, self).__init__(DATASTORE,  **kwargs_)
+supermod.DATASTORESType87.subclass = DATASTORESType87Sub
+# end class DATASTORESType87Sub
 
 
-class DATASTOREType86Sub(TemplatedType, supermod.DATASTOREType86):
+class DATASTOREType88Sub(TemplatedType, supermod.DATASTOREType88):
     def __init__(self, ZONE_ID=None, DATASTORE_ID=None, **kwargs_):
-        super(DATASTOREType86Sub, self).__init__(ZONE_ID, DATASTORE_ID,  **kwargs_)
-supermod.DATASTOREType86.subclass = DATASTOREType86Sub
-# end class DATASTOREType86Sub
+        super(DATASTOREType88Sub, self).__init__(ZONE_ID, DATASTORE_ID,  **kwargs_)
+supermod.DATASTOREType88.subclass = DATASTOREType88Sub
+# end class DATASTOREType88Sub
 
 
-class VNETSType87Sub(TemplatedType, supermod.VNETSType87):
+class VNETSType89Sub(TemplatedType, supermod.VNETSType89):
     def __init__(self, VNET=None, **kwargs_):
-        super(VNETSType87Sub, self).__init__(VNET,  **kwargs_)
-supermod.VNETSType87.subclass = VNETSType87Sub
-# end class VNETSType87Sub
+        super(VNETSType89Sub, self).__init__(VNET,  **kwargs_)
+supermod.VNETSType89.subclass = VNETSType89Sub
+# end class VNETSType89Sub
 
 
 class VNETTypeSub(TemplatedType, supermod.VNETType):
     def __init__(self, ZONE_ID=None, VNET_ID=None, **kwargs_):
         super(VNETTypeSub, self).__init__(ZONE_ID, VNET_ID,  **kwargs_)
 supermod.VNETType.subclass = VNETTypeSub
 # end class VNETTypeSub
 
 
-class PERMISSIONSType88Sub(TemplatedType, supermod.PERMISSIONSType88):
+class PERMISSIONSType90Sub(TemplatedType, supermod.PERMISSIONSType90):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType88Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType88.subclass = PERMISSIONSType88Sub
-# end class PERMISSIONSType88Sub
+        super(PERMISSIONSType90Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType90.subclass = PERMISSIONSType90Sub
+# end class PERMISSIONSType90Sub
 
 
-class LOCKType89Sub(TemplatedType, supermod.LOCKType89):
+class LOCKType91Sub(TemplatedType, supermod.LOCKType91):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType89Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType89.subclass = LOCKType89Sub
-# end class LOCKType89Sub
+        super(LOCKType91Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType91.subclass = LOCKType91Sub
+# end class LOCKType91Sub
 
 
 class ROLESTypeSub(TemplatedType, supermod.ROLESType):
     def __init__(self, ROLE=None, **kwargs_):
         super(ROLESTypeSub, self).__init__(ROLE,  **kwargs_)
 supermod.ROLESType.subclass = ROLESTypeSub
 # end class ROLESTypeSub
@@ -1631,26 +1652,26 @@
 class ROLETypeSub(TemplatedType, supermod.ROLEType):
     def __init__(self, HOST_AFFINED=None, HOST_ANTI_AFFINED=None, ID=None, NAME=None, POLICY=None, **kwargs_):
         super(ROLETypeSub, self).__init__(HOST_AFFINED, HOST_ANTI_AFFINED, ID, NAME, POLICY,  **kwargs_)
 supermod.ROLEType.subclass = ROLETypeSub
 # end class ROLETypeSub
 
 
-class VMType90Sub(TemplatedType, supermod.VMType90):
+class VMType92Sub(TemplatedType, supermod.VMType92):
     def __init__(self, ID=None, UID=None, GID=None, UNAME=None, GNAME=None, NAME=None, LAST_POLL=None, STATE=None, LCM_STATE=None, RESCHED=None, STIME=None, ETIME=None, DEPLOY_ID=None, TEMPLATE=None, MONITORING=None, USER_TEMPLATE=None, HISTORY_RECORDS=None, **kwargs_):
-        super(VMType90Sub, self).__init__(ID, UID, GID, UNAME, GNAME, NAME, LAST_POLL, STATE, LCM_STATE, RESCHED, STIME, ETIME, DEPLOY_ID, TEMPLATE, MONITORING, USER_TEMPLATE, HISTORY_RECORDS,  **kwargs_)
-supermod.VMType90.subclass = VMType90Sub
-# end class VMType90Sub
+        super(VMType92Sub, self).__init__(ID, UID, GID, UNAME, GNAME, NAME, LAST_POLL, STATE, LCM_STATE, RESCHED, STIME, ETIME, DEPLOY_ID, TEMPLATE, MONITORING, USER_TEMPLATE, HISTORY_RECORDS,  **kwargs_)
+supermod.VMType92.subclass = VMType92Sub
+# end class VMType92Sub
 
 
-class TEMPLATEType91Sub(TemplatedType, supermod.TEMPLATEType91):
+class TEMPLATEType93Sub(TemplatedType, supermod.TEMPLATEType93):
     def __init__(self, CPU=None, MEMORY=None, DISK=None, NIC=None, GRAPHICS=None, **kwargs_):
-        super(TEMPLATEType91Sub, self).__init__(CPU, MEMORY, DISK, NIC, GRAPHICS,  **kwargs_)
-supermod.TEMPLATEType91.subclass = TEMPLATEType91Sub
-# end class TEMPLATEType91Sub
+        super(TEMPLATEType93Sub, self).__init__(CPU, MEMORY, DISK, NIC, GRAPHICS,  **kwargs_)
+supermod.TEMPLATEType93.subclass = TEMPLATEType93Sub
+# end class TEMPLATEType93Sub
 
 
 class DISKTypeSub(TemplatedType, supermod.DISKType):
     def __init__(self, VCENTER_DS_REF=None, VCENTER_INSTANCE_ID=None, anytypeobjs_=None, **kwargs_):
         super(DISKTypeSub, self).__init__(VCENTER_DS_REF, VCENTER_INSTANCE_ID, anytypeobjs_,  **kwargs_)
 supermod.DISKType.subclass = DISKTypeSub
 # end class DISKTypeSub
@@ -1659,19 +1680,19 @@
 class NICTypeSub(TemplatedType, supermod.NICType):
     def __init__(self, anytypeobjs_=None, VCENTER_INSTANCE_ID=None, VCENTER_NET_REF=None, VCENTER_PORTGROUP_TYPE=None, **kwargs_):
         super(NICTypeSub, self).__init__(anytypeobjs_, VCENTER_INSTANCE_ID, VCENTER_NET_REF, VCENTER_PORTGROUP_TYPE,  **kwargs_)
 supermod.NICType.subclass = NICTypeSub
 # end class NICTypeSub
 
 
-class MONITORINGType92Sub(TemplatedType, supermod.MONITORINGType92):
+class MONITORINGType94Sub(TemplatedType, supermod.MONITORINGType94):
     def __init__(self, anytypeobjs_=None, **kwargs_):
-        super(MONITORINGType92Sub, self).__init__(anytypeobjs_,  **kwargs_)
-supermod.MONITORINGType92.subclass = MONITORINGType92Sub
-# end class MONITORINGType92Sub
+        super(MONITORINGType94Sub, self).__init__(anytypeobjs_,  **kwargs_)
+supermod.MONITORINGType94.subclass = MONITORINGType94Sub
+# end class MONITORINGType94Sub
 
 
 class USER_TEMPLATETypeSub(TemplatedType, supermod.USER_TEMPLATEType):
     def __init__(self, anytypeobjs_=None, **kwargs_):
         super(USER_TEMPLATETypeSub, self).__init__(anytypeobjs_,  **kwargs_)
 supermod.USER_TEMPLATEType.subclass = USER_TEMPLATETypeSub
 # end class USER_TEMPLATETypeSub
@@ -1687,82 +1708,82 @@
 class HISTORYTypeSub(TemplatedType, supermod.HISTORYType):
     def __init__(self, OID=None, SEQ=None, HOSTNAME=None, HID=None, CID=None, DS_ID=None, VM_MAD=None, TM_MAD=None, ACTION=None, **kwargs_):
         super(HISTORYTypeSub, self).__init__(OID, SEQ, HOSTNAME, HID, CID, DS_ID, VM_MAD, TM_MAD, ACTION,  **kwargs_)
 supermod.HISTORYType.subclass = HISTORYTypeSub
 # end class HISTORYTypeSub
 
 
-class LOCKType93Sub(TemplatedType, supermod.LOCKType93):
+class LOCKType95Sub(TemplatedType, supermod.LOCKType95):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType93Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType93.subclass = LOCKType93Sub
-# end class LOCKType93Sub
+        super(LOCKType95Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType95.subclass = LOCKType95Sub
+# end class LOCKType95Sub
 
 
-class PERMISSIONSType94Sub(TemplatedType, supermod.PERMISSIONSType94):
+class PERMISSIONSType96Sub(TemplatedType, supermod.PERMISSIONSType96):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType94Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType94.subclass = PERMISSIONSType94Sub
-# end class PERMISSIONSType94Sub
+        super(PERMISSIONSType96Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType96.subclass = PERMISSIONSType96Sub
+# end class PERMISSIONSType96Sub
 
 
-class TEMPLATEType95Sub(TemplatedType, supermod.TEMPLATEType95):
+class TEMPLATEType97Sub(TemplatedType, supermod.TEMPLATEType97):
     def __init__(self, VCENTER_CCR_REF=None, VCENTER_INSTANCE_ID=None, VCENTER_TEMPLATE_REF=None, anytypeobjs_=None, **kwargs_):
-        super(TEMPLATEType95Sub, self).__init__(VCENTER_CCR_REF, VCENTER_INSTANCE_ID, VCENTER_TEMPLATE_REF, anytypeobjs_,  **kwargs_)
-supermod.TEMPLATEType95.subclass = TEMPLATEType95Sub
-# end class TEMPLATEType95Sub
+        super(TEMPLATEType97Sub, self).__init__(VCENTER_CCR_REF, VCENTER_INSTANCE_ID, VCENTER_TEMPLATE_REF, anytypeobjs_,  **kwargs_)
+supermod.TEMPLATEType97.subclass = TEMPLATEType97Sub
+# end class TEMPLATEType97Sub
 
 
-class PERMISSIONSType96Sub(TemplatedType, supermod.PERMISSIONSType96):
+class PERMISSIONSType98Sub(TemplatedType, supermod.PERMISSIONSType98):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType96Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType96.subclass = PERMISSIONSType96Sub
-# end class PERMISSIONSType96Sub
+        super(PERMISSIONSType98Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType98.subclass = PERMISSIONSType98Sub
+# end class PERMISSIONSType98Sub
 
 
-class LOCKType97Sub(TemplatedType, supermod.LOCKType97):
+class LOCKType99Sub(TemplatedType, supermod.LOCKType99):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType97Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType97.subclass = LOCKType97Sub
-# end class LOCKType97Sub
+        super(LOCKType99Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType99.subclass = LOCKType99Sub
+# end class LOCKType99Sub
 
 
-class MONITORINGType98Sub(TemplatedType, supermod.MONITORINGType98):
+class MONITORINGType100Sub(TemplatedType, supermod.MONITORINGType100):
     def __init__(self, CPU=None, DISKRDBYTES=None, DISKRDIOPS=None, DISKWRBYTES=None, DISKWRIOPS=None, DISK_SIZE=None, ID=None, MEMORY=None, NETRX=None, NETTX=None, TIMESTAMP=None, VCENTER_ESX_HOST=None, VCENTER_GUEST_STATE=None, VCENTER_RP_NAME=None, VCENTER_VMWARETOOLS_RUNNING_STATUS=None, VCENTER_VMWARETOOLS_VERSION=None, VCENTER_VMWARETOOLS_VERSION_STATUS=None, VCENTER_VM_NAME=None, **kwargs_):
-        super(MONITORINGType98Sub, self).__init__(CPU, DISKRDBYTES, DISKRDIOPS, DISKWRBYTES, DISKWRIOPS, DISK_SIZE, ID, MEMORY, NETRX, NETTX, TIMESTAMP, VCENTER_ESX_HOST, VCENTER_GUEST_STATE, VCENTER_RP_NAME, VCENTER_VMWARETOOLS_RUNNING_STATUS, VCENTER_VMWARETOOLS_VERSION, VCENTER_VMWARETOOLS_VERSION_STATUS, VCENTER_VM_NAME,  **kwargs_)
-supermod.MONITORINGType98.subclass = MONITORINGType98Sub
-# end class MONITORINGType98Sub
+        super(MONITORINGType100Sub, self).__init__(CPU, DISKRDBYTES, DISKRDIOPS, DISKWRBYTES, DISKWRIOPS, DISK_SIZE, ID, MEMORY, NETRX, NETTX, TIMESTAMP, VCENTER_ESX_HOST, VCENTER_GUEST_STATE, VCENTER_RP_NAME, VCENTER_VMWARETOOLS_RUNNING_STATUS, VCENTER_VMWARETOOLS_VERSION, VCENTER_VMWARETOOLS_VERSION_STATUS, VCENTER_VM_NAME,  **kwargs_)
+supermod.MONITORINGType100.subclass = MONITORINGType100Sub
+# end class MONITORINGType100Sub
 
 
-class DISK_SIZEType99Sub(TemplatedType, supermod.DISK_SIZEType99):
+class DISK_SIZEType101Sub(TemplatedType, supermod.DISK_SIZEType101):
     def __init__(self, ID=None, SIZE=None, **kwargs_):
-        super(DISK_SIZEType99Sub, self).__init__(ID, SIZE,  **kwargs_)
-supermod.DISK_SIZEType99.subclass = DISK_SIZEType99Sub
-# end class DISK_SIZEType99Sub
+        super(DISK_SIZEType101Sub, self).__init__(ID, SIZE,  **kwargs_)
+supermod.DISK_SIZEType101.subclass = DISK_SIZEType101Sub
+# end class DISK_SIZEType101Sub
 
 
-class TEMPLATEType100Sub(TemplatedType, supermod.TEMPLATEType100):
+class TEMPLATEType102Sub(TemplatedType, supermod.TEMPLATEType102):
     def __init__(self, AUTOMATIC_DS_REQUIREMENTS=None, AUTOMATIC_NIC_REQUIREMENTS=None, AUTOMATIC_REQUIREMENTS=None, CLONING_TEMPLATE_ID=None, CONTEXT=None, CPU=None, CPU_COST=None, DISK=None, DISK_COST=None, EMULATOR=None, FEATURES=None, HYPERV_OPTIONS=None, GRAPHICS=None, IMPORTED=None, INPUT=None, MEMORY=None, MEMORY_COST=None, MEMORY_MAX=None, MEMORY_SLOTS=None, MEMORY_RESIZE_MODE=None, NIC=None, NIC_ALIAS=None, NIC_DEFAULT=None, NUMA_NODE=None, OS=None, PCI=None, RAW=None, SCHED_ACTION=None, SECURITY_GROUP_RULE=None, SNAPSHOT=None, SPICE_OPTIONS=None, SUBMIT_ON_HOLD=None, TEMPLATE_ID=None, TM_MAD_SYSTEM=None, TOPOLOGY=None, VCPU=None, VCPU_MAX=None, VMGROUP=None, VMID=None, VROUTER_ID=None, VROUTER_KEEPALIVED_ID=None, VROUTER_KEEPALIVED_PASSWORD=None, **kwargs_):
-        super(TEMPLATEType100Sub, self).__init__(AUTOMATIC_DS_REQUIREMENTS, AUTOMATIC_NIC_REQUIREMENTS, AUTOMATIC_REQUIREMENTS, CLONING_TEMPLATE_ID, CONTEXT, CPU, CPU_COST, DISK, DISK_COST, EMULATOR, FEATURES, HYPERV_OPTIONS, GRAPHICS, IMPORTED, INPUT, MEMORY, MEMORY_COST, MEMORY_MAX, MEMORY_SLOTS, MEMORY_RESIZE_MODE, NIC, NIC_ALIAS, NIC_DEFAULT, NUMA_NODE, OS, PCI, RAW, SCHED_ACTION, SECURITY_GROUP_RULE, SNAPSHOT, SPICE_OPTIONS, SUBMIT_ON_HOLD, TEMPLATE_ID, TM_MAD_SYSTEM, TOPOLOGY, VCPU, VCPU_MAX, VMGROUP, VMID, VROUTER_ID, VROUTER_KEEPALIVED_ID, VROUTER_KEEPALIVED_PASSWORD,  **kwargs_)
-supermod.TEMPLATEType100.subclass = TEMPLATEType100Sub
-# end class TEMPLATEType100Sub
+        super(TEMPLATEType102Sub, self).__init__(AUTOMATIC_DS_REQUIREMENTS, AUTOMATIC_NIC_REQUIREMENTS, AUTOMATIC_REQUIREMENTS, CLONING_TEMPLATE_ID, CONTEXT, CPU, CPU_COST, DISK, DISK_COST, EMULATOR, FEATURES, HYPERV_OPTIONS, GRAPHICS, IMPORTED, INPUT, MEMORY, MEMORY_COST, MEMORY_MAX, MEMORY_SLOTS, MEMORY_RESIZE_MODE, NIC, NIC_ALIAS, NIC_DEFAULT, NUMA_NODE, OS, PCI, RAW, SCHED_ACTION, SECURITY_GROUP_RULE, SNAPSHOT, SPICE_OPTIONS, SUBMIT_ON_HOLD, TEMPLATE_ID, TM_MAD_SYSTEM, TOPOLOGY, VCPU, VCPU_MAX, VMGROUP, VMID, VROUTER_ID, VROUTER_KEEPALIVED_ID, VROUTER_KEEPALIVED_PASSWORD,  **kwargs_)
+supermod.TEMPLATEType102.subclass = TEMPLATEType102Sub
+# end class TEMPLATEType102Sub
 
 
-class DISKType101Sub(TemplatedType, supermod.DISKType101):
+class DISKType103Sub(TemplatedType, supermod.DISKType103):
     def __init__(self, VCENTER_DS_REF=None, VCENTER_INSTANCE_ID=None, anytypeobjs_=None, **kwargs_):
-        super(DISKType101Sub, self).__init__(VCENTER_DS_REF, VCENTER_INSTANCE_ID, anytypeobjs_,  **kwargs_)
-supermod.DISKType101.subclass = DISKType101Sub
-# end class DISKType101Sub
+        super(DISKType103Sub, self).__init__(VCENTER_DS_REF, VCENTER_INSTANCE_ID, anytypeobjs_,  **kwargs_)
+supermod.DISKType103.subclass = DISKType103Sub
+# end class DISKType103Sub
 
 
-class NICType102Sub(TemplatedType, supermod.NICType102):
+class NICType104Sub(TemplatedType, supermod.NICType104):
     def __init__(self, anytypeobjs_=None, VCENTER_INSTANCE_ID=None, VCENTER_NET_REF=None, VCENTER_PORTGROUP_TYPE=None, **kwargs_):
-        super(NICType102Sub, self).__init__(anytypeobjs_, VCENTER_INSTANCE_ID, VCENTER_NET_REF, VCENTER_PORTGROUP_TYPE,  **kwargs_)
-supermod.NICType102.subclass = NICType102Sub
-# end class NICType102Sub
+        super(NICType104Sub, self).__init__(anytypeobjs_, VCENTER_INSTANCE_ID, VCENTER_NET_REF, VCENTER_PORTGROUP_TYPE,  **kwargs_)
+supermod.NICType104.subclass = NICType104Sub
+# end class NICType104Sub
 
 
 class NIC_ALIASTypeSub(TemplatedType, supermod.NIC_ALIASType):
     def __init__(self, ALIAS_ID=None, PARENT=None, PARENT_ID=None, anytypeobjs_=None, VCENTER_INSTANCE_ID=None, VCENTER_NET_REF=None, VCENTER_PORTGROUP_TYPE=None, **kwargs_):
         super(NIC_ALIASTypeSub, self).__init__(ALIAS_ID, PARENT, PARENT_ID, anytypeobjs_, VCENTER_INSTANCE_ID, VCENTER_NET_REF, VCENTER_PORTGROUP_TYPE,  **kwargs_)
 supermod.NIC_ALIASType.subclass = NIC_ALIASTypeSub
 # end class NIC_ALIASTypeSub
@@ -1771,131 +1792,131 @@
 class SCHED_ACTIONTypeSub(TemplatedType, supermod.SCHED_ACTIONType):
     def __init__(self, ACTION=None, ARGS=None, DAYS=None, END_TYPE=None, END_VALUE=None, ID=None, REPEAT=None, TIME=None, WARNING=None, **kwargs_):
         super(SCHED_ACTIONTypeSub, self).__init__(ACTION, ARGS, DAYS, END_TYPE, END_VALUE, ID, REPEAT, TIME, WARNING,  **kwargs_)
 supermod.SCHED_ACTIONType.subclass = SCHED_ACTIONTypeSub
 # end class SCHED_ACTIONTypeSub
 
 
-class SNAPSHOTType103Sub(TemplatedType, supermod.SNAPSHOTType103):
+class SNAPSHOTType105Sub(TemplatedType, supermod.SNAPSHOTType105):
     def __init__(self, ACTION=None, ACTIVE=None, HYPERVISOR_ID=None, NAME=None, SNAPSHOT_ID=None, SYSTEM_DISK_SIZE=None, TIME=None, **kwargs_):
-        super(SNAPSHOTType103Sub, self).__init__(ACTION, ACTIVE, HYPERVISOR_ID, NAME, SNAPSHOT_ID, SYSTEM_DISK_SIZE, TIME,  **kwargs_)
-supermod.SNAPSHOTType103.subclass = SNAPSHOTType103Sub
-# end class SNAPSHOTType103Sub
+        super(SNAPSHOTType105Sub, self).__init__(ACTION, ACTIVE, HYPERVISOR_ID, NAME, SNAPSHOT_ID, SYSTEM_DISK_SIZE, TIME,  **kwargs_)
+supermod.SNAPSHOTType105.subclass = SNAPSHOTType105Sub
+# end class SNAPSHOTType105Sub
 
 
-class USER_TEMPLATEType104Sub(TemplatedType, supermod.USER_TEMPLATEType104):
+class USER_TEMPLATEType106Sub(TemplatedType, supermod.USER_TEMPLATEType106):
     def __init__(self, VCENTER_CCR_REF=None, VCENTER_DS_REF=None, VCENTER_INSTANCE_ID=None, anytypeobjs_=None, **kwargs_):
-        super(USER_TEMPLATEType104Sub, self).__init__(VCENTER_CCR_REF, VCENTER_DS_REF, VCENTER_INSTANCE_ID, anytypeobjs_,  **kwargs_)
-supermod.USER_TEMPLATEType104.subclass = USER_TEMPLATEType104Sub
-# end class USER_TEMPLATEType104Sub
+        super(USER_TEMPLATEType106Sub, self).__init__(VCENTER_CCR_REF, VCENTER_DS_REF, VCENTER_INSTANCE_ID, anytypeobjs_,  **kwargs_)
+supermod.USER_TEMPLATEType106.subclass = USER_TEMPLATEType106Sub
+# end class USER_TEMPLATEType106Sub
 
 
-class HISTORY_RECORDSType105Sub(TemplatedType, supermod.HISTORY_RECORDSType105):
+class HISTORY_RECORDSType107Sub(TemplatedType, supermod.HISTORY_RECORDSType107):
     def __init__(self, HISTORY=None, **kwargs_):
-        super(HISTORY_RECORDSType105Sub, self).__init__(HISTORY,  **kwargs_)
-supermod.HISTORY_RECORDSType105.subclass = HISTORY_RECORDSType105Sub
-# end class HISTORY_RECORDSType105Sub
+        super(HISTORY_RECORDSType107Sub, self).__init__(HISTORY,  **kwargs_)
+supermod.HISTORY_RECORDSType107.subclass = HISTORY_RECORDSType107Sub
+# end class HISTORY_RECORDSType107Sub
 
 
-class HISTORYType106Sub(TemplatedType, supermod.HISTORYType106):
+class HISTORYType108Sub(TemplatedType, supermod.HISTORYType108):
     def __init__(self, OID=None, SEQ=None, HOSTNAME=None, HID=None, CID=None, STIME=None, ETIME=None, VM_MAD=None, TM_MAD=None, DS_ID=None, PSTIME=None, PETIME=None, RSTIME=None, RETIME=None, ESTIME=None, EETIME=None, ACTION=None, UID=None, GID=None, REQUEST_ID=None, **kwargs_):
-        super(HISTORYType106Sub, self).__init__(OID, SEQ, HOSTNAME, HID, CID, STIME, ETIME, VM_MAD, TM_MAD, DS_ID, PSTIME, PETIME, RSTIME, RETIME, ESTIME, EETIME, ACTION, UID, GID, REQUEST_ID,  **kwargs_)
-supermod.HISTORYType106.subclass = HISTORYType106Sub
-# end class HISTORYType106Sub
+        super(HISTORYType108Sub, self).__init__(OID, SEQ, HOSTNAME, HID, CID, STIME, ETIME, VM_MAD, TM_MAD, DS_ID, PSTIME, PETIME, RSTIME, RETIME, ESTIME, EETIME, ACTION, UID, GID, REQUEST_ID,  **kwargs_)
+supermod.HISTORYType108.subclass = HISTORYType108Sub
+# end class HISTORYType108Sub
 
 
-class SNAPSHOTSType107Sub(TemplatedType, supermod.SNAPSHOTSType107):
+class SNAPSHOTSType109Sub(TemplatedType, supermod.SNAPSHOTSType109):
     def __init__(self, ALLOW_ORPHANS=None, CURRENT_BASE=None, DISK_ID=None, NEXT_SNAPSHOT=None, SNAPSHOT=None, **kwargs_):
-        super(SNAPSHOTSType107Sub, self).__init__(ALLOW_ORPHANS, CURRENT_BASE, DISK_ID, NEXT_SNAPSHOT, SNAPSHOT,  **kwargs_)
-supermod.SNAPSHOTSType107.subclass = SNAPSHOTSType107Sub
-# end class SNAPSHOTSType107Sub
+        super(SNAPSHOTSType109Sub, self).__init__(ALLOW_ORPHANS, CURRENT_BASE, DISK_ID, NEXT_SNAPSHOT, SNAPSHOT,  **kwargs_)
+supermod.SNAPSHOTSType109.subclass = SNAPSHOTSType109Sub
+# end class SNAPSHOTSType109Sub
 
 
-class SNAPSHOTType108Sub(TemplatedType, supermod.SNAPSHOTType108):
+class SNAPSHOTType110Sub(TemplatedType, supermod.SNAPSHOTType110):
     def __init__(self, ACTIVE=None, CHILDREN=None, DATE=None, ID=None, NAME=None, PARENT=None, SIZE=None, **kwargs_):
-        super(SNAPSHOTType108Sub, self).__init__(ACTIVE, CHILDREN, DATE, ID, NAME, PARENT, SIZE,  **kwargs_)
-supermod.SNAPSHOTType108.subclass = SNAPSHOTType108Sub
-# end class SNAPSHOTType108Sub
+        super(SNAPSHOTType110Sub, self).__init__(ACTIVE, CHILDREN, DATE, ID, NAME, PARENT, SIZE,  **kwargs_)
+supermod.SNAPSHOTType110.subclass = SNAPSHOTType110Sub
+# end class SNAPSHOTType110Sub
 
 
-class BACKUPSType109Sub(TemplatedType, supermod.BACKUPSType109):
+class BACKUPSType111Sub(TemplatedType, supermod.BACKUPSType111):
     def __init__(self, BACKUP_CONFIG=None, BACKUP_IDS=None, **kwargs_):
-        super(BACKUPSType109Sub, self).__init__(BACKUP_CONFIG, BACKUP_IDS,  **kwargs_)
-supermod.BACKUPSType109.subclass = BACKUPSType109Sub
-# end class BACKUPSType109Sub
+        super(BACKUPSType111Sub, self).__init__(BACKUP_CONFIG, BACKUP_IDS,  **kwargs_)
+supermod.BACKUPSType111.subclass = BACKUPSType111Sub
+# end class BACKUPSType111Sub
 
 
-class BACKUP_CONFIGType110Sub(TemplatedType, supermod.BACKUP_CONFIGType110):
+class BACKUP_CONFIGType112Sub(TemplatedType, supermod.BACKUP_CONFIGType112):
     def __init__(self, BACKUP_VOLATILE=None, FS_FREEZE=None, INCREMENTAL_BACKUP_ID=None, KEEP_LAST=None, LAST_BACKUP_ID=None, LAST_BACKUP_SIZE=None, LAST_DATASTORE_ID=None, LAST_INCREMENT_ID=None, MODE=None, **kwargs_):
-        super(BACKUP_CONFIGType110Sub, self).__init__(BACKUP_VOLATILE, FS_FREEZE, INCREMENTAL_BACKUP_ID, KEEP_LAST, LAST_BACKUP_ID, LAST_BACKUP_SIZE, LAST_DATASTORE_ID, LAST_INCREMENT_ID, MODE,  **kwargs_)
-supermod.BACKUP_CONFIGType110.subclass = BACKUP_CONFIGType110Sub
-# end class BACKUP_CONFIGType110Sub
+        super(BACKUP_CONFIGType112Sub, self).__init__(BACKUP_VOLATILE, FS_FREEZE, INCREMENTAL_BACKUP_ID, KEEP_LAST, LAST_BACKUP_ID, LAST_BACKUP_SIZE, LAST_DATASTORE_ID, LAST_INCREMENT_ID, MODE,  **kwargs_)
+supermod.BACKUP_CONFIGType112.subclass = BACKUP_CONFIGType112Sub
+# end class BACKUP_CONFIGType112Sub
 
 
-class BACKUP_IDSType111Sub(TemplatedType, supermod.BACKUP_IDSType111):
+class BACKUP_IDSType113Sub(TemplatedType, supermod.BACKUP_IDSType113):
     def __init__(self, ID=None, **kwargs_):
-        super(BACKUP_IDSType111Sub, self).__init__(ID,  **kwargs_)
-supermod.BACKUP_IDSType111.subclass = BACKUP_IDSType111Sub
-# end class BACKUP_IDSType111Sub
+        super(BACKUP_IDSType113Sub, self).__init__(ID,  **kwargs_)
+supermod.BACKUP_IDSType113.subclass = BACKUP_IDSType113Sub
+# end class BACKUP_IDSType113Sub
 
 
-class VNETType112Sub(TemplatedType, supermod.VNETType112):
+class VNETType114Sub(TemplatedType, supermod.VNETType114):
     def __init__(self, ID=None, UID=None, GID=None, UNAME=None, GNAME=None, NAME=None, PERMISSIONS=None, CLUSTERS=None, BRIDGE=None, BRIDGE_TYPE=None, STATE=None, PREV_STATE=None, PARENT_NETWORK_ID=None, VN_MAD=None, PHYDEV=None, VLAN_ID=None, OUTER_VLAN_ID=None, VLAN_ID_AUTOMATIC=None, OUTER_VLAN_ID_AUTOMATIC=None, USED_LEASES=None, VROUTERS=None, UPDATED_VMS=None, OUTDATED_VMS=None, UPDATING_VMS=None, ERROR_VMS=None, TEMPLATE=None, AR_POOL=None, **kwargs_):
-        super(VNETType112Sub, self).__init__(ID, UID, GID, UNAME, GNAME, NAME, PERMISSIONS, CLUSTERS, BRIDGE, BRIDGE_TYPE, STATE, PREV_STATE, PARENT_NETWORK_ID, VN_MAD, PHYDEV, VLAN_ID, OUTER_VLAN_ID, VLAN_ID_AUTOMATIC, OUTER_VLAN_ID_AUTOMATIC, USED_LEASES, VROUTERS, UPDATED_VMS, OUTDATED_VMS, UPDATING_VMS, ERROR_VMS, TEMPLATE, AR_POOL,  **kwargs_)
-supermod.VNETType112.subclass = VNETType112Sub
-# end class VNETType112Sub
+        super(VNETType114Sub, self).__init__(ID, UID, GID, UNAME, GNAME, NAME, PERMISSIONS, CLUSTERS, BRIDGE, BRIDGE_TYPE, STATE, PREV_STATE, PARENT_NETWORK_ID, VN_MAD, PHYDEV, VLAN_ID, OUTER_VLAN_ID, VLAN_ID_AUTOMATIC, OUTER_VLAN_ID_AUTOMATIC, USED_LEASES, VROUTERS, UPDATED_VMS, OUTDATED_VMS, UPDATING_VMS, ERROR_VMS, TEMPLATE, AR_POOL,  **kwargs_)
+supermod.VNETType114.subclass = VNETType114Sub
+# end class VNETType114Sub
 
 
-class PERMISSIONSType113Sub(TemplatedType, supermod.PERMISSIONSType113):
+class PERMISSIONSType115Sub(TemplatedType, supermod.PERMISSIONSType115):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType113Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType113.subclass = PERMISSIONSType113Sub
-# end class PERMISSIONSType113Sub
+        super(PERMISSIONSType115Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType115.subclass = PERMISSIONSType115Sub
+# end class PERMISSIONSType115Sub
 
 
-class CLUSTERSType114Sub(TemplatedType, supermod.CLUSTERSType114):
+class CLUSTERSType116Sub(TemplatedType, supermod.CLUSTERSType116):
     def __init__(self, ID=None, **kwargs_):
-        super(CLUSTERSType114Sub, self).__init__(ID,  **kwargs_)
-supermod.CLUSTERSType114.subclass = CLUSTERSType114Sub
-# end class CLUSTERSType114Sub
+        super(CLUSTERSType116Sub, self).__init__(ID,  **kwargs_)
+supermod.CLUSTERSType116.subclass = CLUSTERSType116Sub
+# end class CLUSTERSType116Sub
 
 
 class VROUTERSTypeSub(TemplatedType, supermod.VROUTERSType):
     def __init__(self, ID=None, **kwargs_):
         super(VROUTERSTypeSub, self).__init__(ID,  **kwargs_)
 supermod.VROUTERSType.subclass = VROUTERSTypeSub
 # end class VROUTERSTypeSub
 
 
-class UPDATED_VMSType115Sub(TemplatedType, supermod.UPDATED_VMSType115):
+class UPDATED_VMSType117Sub(TemplatedType, supermod.UPDATED_VMSType117):
     def __init__(self, ID=None, **kwargs_):
-        super(UPDATED_VMSType115Sub, self).__init__(ID,  **kwargs_)
-supermod.UPDATED_VMSType115.subclass = UPDATED_VMSType115Sub
-# end class UPDATED_VMSType115Sub
+        super(UPDATED_VMSType117Sub, self).__init__(ID,  **kwargs_)
+supermod.UPDATED_VMSType117.subclass = UPDATED_VMSType117Sub
+# end class UPDATED_VMSType117Sub
 
 
-class OUTDATED_VMSType116Sub(TemplatedType, supermod.OUTDATED_VMSType116):
+class OUTDATED_VMSType118Sub(TemplatedType, supermod.OUTDATED_VMSType118):
     def __init__(self, ID=None, **kwargs_):
-        super(OUTDATED_VMSType116Sub, self).__init__(ID,  **kwargs_)
-supermod.OUTDATED_VMSType116.subclass = OUTDATED_VMSType116Sub
-# end class OUTDATED_VMSType116Sub
+        super(OUTDATED_VMSType118Sub, self).__init__(ID,  **kwargs_)
+supermod.OUTDATED_VMSType118.subclass = OUTDATED_VMSType118Sub
+# end class OUTDATED_VMSType118Sub
 
 
-class UPDATING_VMSType117Sub(TemplatedType, supermod.UPDATING_VMSType117):
+class UPDATING_VMSType119Sub(TemplatedType, supermod.UPDATING_VMSType119):
     def __init__(self, ID=None, **kwargs_):
-        super(UPDATING_VMSType117Sub, self).__init__(ID,  **kwargs_)
-supermod.UPDATING_VMSType117.subclass = UPDATING_VMSType117Sub
-# end class UPDATING_VMSType117Sub
+        super(UPDATING_VMSType119Sub, self).__init__(ID,  **kwargs_)
+supermod.UPDATING_VMSType119.subclass = UPDATING_VMSType119Sub
+# end class UPDATING_VMSType119Sub
 
 
-class ERROR_VMSType118Sub(TemplatedType, supermod.ERROR_VMSType118):
+class ERROR_VMSType120Sub(TemplatedType, supermod.ERROR_VMSType120):
     def __init__(self, ID=None, **kwargs_):
-        super(ERROR_VMSType118Sub, self).__init__(ID,  **kwargs_)
-supermod.ERROR_VMSType118.subclass = ERROR_VMSType118Sub
-# end class ERROR_VMSType118Sub
+        super(ERROR_VMSType120Sub, self).__init__(ID,  **kwargs_)
+supermod.ERROR_VMSType120.subclass = ERROR_VMSType120Sub
+# end class ERROR_VMSType120Sub
 
 
 class AR_POOLTypeSub(TemplatedType, supermod.AR_POOLType):
     def __init__(self, AR=None, **kwargs_):
         super(AR_POOLTypeSub, self).__init__(AR,  **kwargs_)
 supermod.AR_POOLType.subclass = AR_POOLTypeSub
 # end class AR_POOLTypeSub
@@ -1904,89 +1925,89 @@
 class ARTypeSub(TemplatedType, supermod.ARType):
     def __init__(self, ALLOCATED=None, AR_ID=None, GLOBAL_PREFIX=None, IP=None, MAC=None, PARENT_NETWORK_AR_ID=None, SIZE=None, TYPE=None, ULA_PREFIX=None, VN_MAD=None, **kwargs_):
         super(ARTypeSub, self).__init__(ALLOCATED, AR_ID, GLOBAL_PREFIX, IP, MAC, PARENT_NETWORK_AR_ID, SIZE, TYPE, ULA_PREFIX, VN_MAD,  **kwargs_)
 supermod.ARType.subclass = ARTypeSub
 # end class ARTypeSub
 
 
-class LOCKType119Sub(TemplatedType, supermod.LOCKType119):
+class LOCKType121Sub(TemplatedType, supermod.LOCKType121):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType119Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType119.subclass = LOCKType119Sub
-# end class LOCKType119Sub
+        super(LOCKType121Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType121.subclass = LOCKType121Sub
+# end class LOCKType121Sub
 
 
-class PERMISSIONSType120Sub(TemplatedType, supermod.PERMISSIONSType120):
+class PERMISSIONSType122Sub(TemplatedType, supermod.PERMISSIONSType122):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType120Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType120.subclass = PERMISSIONSType120Sub
-# end class PERMISSIONSType120Sub
+        super(PERMISSIONSType122Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType122.subclass = PERMISSIONSType122Sub
+# end class PERMISSIONSType122Sub
 
 
-class CLUSTERSType121Sub(TemplatedType, supermod.CLUSTERSType121):
+class CLUSTERSType123Sub(TemplatedType, supermod.CLUSTERSType123):
     def __init__(self, ID=None, **kwargs_):
-        super(CLUSTERSType121Sub, self).__init__(ID,  **kwargs_)
-supermod.CLUSTERSType121.subclass = CLUSTERSType121Sub
-# end class CLUSTERSType121Sub
+        super(CLUSTERSType123Sub, self).__init__(ID,  **kwargs_)
+supermod.CLUSTERSType123.subclass = CLUSTERSType123Sub
+# end class CLUSTERSType123Sub
 
 
-class VROUTERSType122Sub(TemplatedType, supermod.VROUTERSType122):
+class VROUTERSType124Sub(TemplatedType, supermod.VROUTERSType124):
     def __init__(self, ID=None, **kwargs_):
-        super(VROUTERSType122Sub, self).__init__(ID,  **kwargs_)
-supermod.VROUTERSType122.subclass = VROUTERSType122Sub
-# end class VROUTERSType122Sub
+        super(VROUTERSType124Sub, self).__init__(ID,  **kwargs_)
+supermod.VROUTERSType124.subclass = VROUTERSType124Sub
+# end class VROUTERSType124Sub
 
 
-class UPDATED_VMSType123Sub(TemplatedType, supermod.UPDATED_VMSType123):
+class UPDATED_VMSType125Sub(TemplatedType, supermod.UPDATED_VMSType125):
     def __init__(self, ID=None, **kwargs_):
-        super(UPDATED_VMSType123Sub, self).__init__(ID,  **kwargs_)
-supermod.UPDATED_VMSType123.subclass = UPDATED_VMSType123Sub
-# end class UPDATED_VMSType123Sub
+        super(UPDATED_VMSType125Sub, self).__init__(ID,  **kwargs_)
+supermod.UPDATED_VMSType125.subclass = UPDATED_VMSType125Sub
+# end class UPDATED_VMSType125Sub
 
 
-class OUTDATED_VMSType124Sub(TemplatedType, supermod.OUTDATED_VMSType124):
+class OUTDATED_VMSType126Sub(TemplatedType, supermod.OUTDATED_VMSType126):
     def __init__(self, ID=None, **kwargs_):
-        super(OUTDATED_VMSType124Sub, self).__init__(ID,  **kwargs_)
-supermod.OUTDATED_VMSType124.subclass = OUTDATED_VMSType124Sub
-# end class OUTDATED_VMSType124Sub
+        super(OUTDATED_VMSType126Sub, self).__init__(ID,  **kwargs_)
+supermod.OUTDATED_VMSType126.subclass = OUTDATED_VMSType126Sub
+# end class OUTDATED_VMSType126Sub
 
 
-class UPDATING_VMSType125Sub(TemplatedType, supermod.UPDATING_VMSType125):
+class UPDATING_VMSType127Sub(TemplatedType, supermod.UPDATING_VMSType127):
     def __init__(self, ID=None, **kwargs_):
-        super(UPDATING_VMSType125Sub, self).__init__(ID,  **kwargs_)
-supermod.UPDATING_VMSType125.subclass = UPDATING_VMSType125Sub
-# end class UPDATING_VMSType125Sub
+        super(UPDATING_VMSType127Sub, self).__init__(ID,  **kwargs_)
+supermod.UPDATING_VMSType127.subclass = UPDATING_VMSType127Sub
+# end class UPDATING_VMSType127Sub
 
 
-class ERROR_VMSType126Sub(TemplatedType, supermod.ERROR_VMSType126):
+class ERROR_VMSType128Sub(TemplatedType, supermod.ERROR_VMSType128):
     def __init__(self, ID=None, **kwargs_):
-        super(ERROR_VMSType126Sub, self).__init__(ID,  **kwargs_)
-supermod.ERROR_VMSType126.subclass = ERROR_VMSType126Sub
-# end class ERROR_VMSType126Sub
+        super(ERROR_VMSType128Sub, self).__init__(ID,  **kwargs_)
+supermod.ERROR_VMSType128.subclass = ERROR_VMSType128Sub
+# end class ERROR_VMSType128Sub
 
 
-class TEMPLATEType127Sub(TemplatedType, supermod.TEMPLATEType127):
+class TEMPLATEType129Sub(TemplatedType, supermod.TEMPLATEType129):
     def __init__(self, DNS=None, GATEWAY=None, GATEWAY6=None, GUEST_MTU=None, IP6_METHOD=None, IP6_METRIC=None, METHOD=None, METRIC=None, NETWORK_ADDRESS=None, NETWORK_MASK=None, SEARCH_DOMAIN=None, VCENTER_FROM_WILD=None, VCENTER_INSTANCE_ID=None, VCENTER_NET_REF=None, VCENTER_PORTGROUP_TYPE=None, VCENTER_TEMPLATE_REF=None, anytypeobjs_=None, **kwargs_):
-        super(TEMPLATEType127Sub, self).__init__(DNS, GATEWAY, GATEWAY6, GUEST_MTU, IP6_METHOD, IP6_METRIC, METHOD, METRIC, NETWORK_ADDRESS, NETWORK_MASK, SEARCH_DOMAIN, VCENTER_FROM_WILD, VCENTER_INSTANCE_ID, VCENTER_NET_REF, VCENTER_PORTGROUP_TYPE, VCENTER_TEMPLATE_REF, anytypeobjs_,  **kwargs_)
-supermod.TEMPLATEType127.subclass = TEMPLATEType127Sub
-# end class TEMPLATEType127Sub
+        super(TEMPLATEType129Sub, self).__init__(DNS, GATEWAY, GATEWAY6, GUEST_MTU, IP6_METHOD, IP6_METRIC, METHOD, METRIC, NETWORK_ADDRESS, NETWORK_MASK, SEARCH_DOMAIN, VCENTER_FROM_WILD, VCENTER_INSTANCE_ID, VCENTER_NET_REF, VCENTER_PORTGROUP_TYPE, VCENTER_TEMPLATE_REF, anytypeobjs_,  **kwargs_)
+supermod.TEMPLATEType129.subclass = TEMPLATEType129Sub
+# end class TEMPLATEType129Sub
 
 
-class AR_POOLType128Sub(TemplatedType, supermod.AR_POOLType128):
+class AR_POOLType130Sub(TemplatedType, supermod.AR_POOLType130):
     def __init__(self, AR=None, **kwargs_):
-        super(AR_POOLType128Sub, self).__init__(AR,  **kwargs_)
-supermod.AR_POOLType128.subclass = AR_POOLType128Sub
-# end class AR_POOLType128Sub
+        super(AR_POOLType130Sub, self).__init__(AR,  **kwargs_)
+supermod.AR_POOLType130.subclass = AR_POOLType130Sub
+# end class AR_POOLType130Sub
 
 
-class ARType129Sub(TemplatedType, supermod.ARType129):
+class ARType131Sub(TemplatedType, supermod.ARType131):
     def __init__(self, AR_ID=None, GLOBAL_PREFIX=None, IP=None, MAC=None, PARENT_NETWORK_AR_ID=None, SIZE=None, TYPE=None, ULA_PREFIX=None, VN_MAD=None, MAC_END=None, IP_END=None, IP6_ULA=None, IP6_ULA_END=None, IP6_GLOBAL=None, IP6_GLOBAL_END=None, IP6=None, IP6_END=None, PORT_START=None, PORT_SIZE=None, USED_LEASES=None, LEASES=None, **kwargs_):
-        super(ARType129Sub, self).__init__(AR_ID, GLOBAL_PREFIX, IP, MAC, PARENT_NETWORK_AR_ID, SIZE, TYPE, ULA_PREFIX, VN_MAD, MAC_END, IP_END, IP6_ULA, IP6_ULA_END, IP6_GLOBAL, IP6_GLOBAL_END, IP6, IP6_END, PORT_START, PORT_SIZE, USED_LEASES, LEASES,  **kwargs_)
-supermod.ARType129.subclass = ARType129Sub
-# end class ARType129Sub
+        super(ARType131Sub, self).__init__(AR_ID, GLOBAL_PREFIX, IP, MAC, PARENT_NETWORK_AR_ID, SIZE, TYPE, ULA_PREFIX, VN_MAD, MAC_END, IP_END, IP6_ULA, IP6_ULA_END, IP6_GLOBAL, IP6_GLOBAL_END, IP6, IP6_END, PORT_START, PORT_SIZE, USED_LEASES, LEASES,  **kwargs_)
+supermod.ARType131.subclass = ARType131Sub
+# end class ARType131Sub
 
 
 class LEASESTypeSub(TemplatedType, supermod.LEASESType):
     def __init__(self, LEASE=None, **kwargs_):
         super(LEASESTypeSub, self).__init__(LEASE,  **kwargs_)
 supermod.LEASESType.subclass = LEASESTypeSub
 # end class LEASESTypeSub
@@ -1995,68 +2016,68 @@
 class LEASETypeSub(TemplatedType, supermod.LEASEType):
     def __init__(self, IP=None, IP6=None, IP6_GLOBAL=None, IP6_LINK=None, IP6_ULA=None, MAC=None, VM=None, VNET=None, VROUTER=None, **kwargs_):
         super(LEASETypeSub, self).__init__(IP, IP6, IP6_GLOBAL, IP6_LINK, IP6_ULA, MAC, VM, VNET, VROUTER,  **kwargs_)
 supermod.LEASEType.subclass = LEASETypeSub
 # end class LEASETypeSub
 
 
-class LOCKType130Sub(TemplatedType, supermod.LOCKType130):
+class LOCKType132Sub(TemplatedType, supermod.LOCKType132):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType130Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType130.subclass = LOCKType130Sub
-# end class LOCKType130Sub
+        super(LOCKType132Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType132.subclass = LOCKType132Sub
+# end class LOCKType132Sub
 
 
-class PERMISSIONSType131Sub(TemplatedType, supermod.PERMISSIONSType131):
+class PERMISSIONSType133Sub(TemplatedType, supermod.PERMISSIONSType133):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType131Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType131.subclass = PERMISSIONSType131Sub
-# end class PERMISSIONSType131Sub
+        super(PERMISSIONSType133Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType133.subclass = PERMISSIONSType133Sub
+# end class PERMISSIONSType133Sub
 
 
-class TEMPLATEType132Sub(TemplatedType, supermod.TEMPLATEType132):
+class TEMPLATEType134Sub(TemplatedType, supermod.TEMPLATEType134):
     def __init__(self, VN_MAD=None, anytypeobjs_=None, **kwargs_):
-        super(TEMPLATEType132Sub, self).__init__(VN_MAD, anytypeobjs_,  **kwargs_)
-supermod.TEMPLATEType132.subclass = TEMPLATEType132Sub
-# end class TEMPLATEType132Sub
+        super(TEMPLATEType134Sub, self).__init__(VN_MAD, anytypeobjs_,  **kwargs_)
+supermod.TEMPLATEType134.subclass = TEMPLATEType134Sub
+# end class TEMPLATEType134Sub
 
 
-class PERMISSIONSType133Sub(TemplatedType, supermod.PERMISSIONSType133):
+class PERMISSIONSType135Sub(TemplatedType, supermod.PERMISSIONSType135):
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, **kwargs_):
-        super(PERMISSIONSType133Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
-supermod.PERMISSIONSType133.subclass = PERMISSIONSType133Sub
-# end class PERMISSIONSType133Sub
+        super(PERMISSIONSType135Sub, self).__init__(OWNER_U, OWNER_M, OWNER_A, GROUP_U, GROUP_M, GROUP_A, OTHER_U, OTHER_M, OTHER_A,  **kwargs_)
+supermod.PERMISSIONSType135.subclass = PERMISSIONSType135Sub
+# end class PERMISSIONSType135Sub
 
 
-class LOCKType134Sub(TemplatedType, supermod.LOCKType134):
+class LOCKType136Sub(TemplatedType, supermod.LOCKType136):
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, **kwargs_):
-        super(LOCKType134Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
-supermod.LOCKType134.subclass = LOCKType134Sub
-# end class LOCKType134Sub
+        super(LOCKType136Sub, self).__init__(LOCKED, OWNER, TIME, REQ_ID,  **kwargs_)
+supermod.LOCKType136.subclass = LOCKType136Sub
+# end class LOCKType136Sub
 
 
-class VMSType135Sub(TemplatedType, supermod.VMSType135):
+class VMSType137Sub(TemplatedType, supermod.VMSType137):
     def __init__(self, ID=None, **kwargs_):
-        super(VMSType135Sub, self).__init__(ID,  **kwargs_)
-supermod.VMSType135.subclass = VMSType135Sub
-# end class VMSType135Sub
+        super(VMSType137Sub, self).__init__(ID,  **kwargs_)
+supermod.VMSType137.subclass = VMSType137Sub
+# end class VMSType137Sub
 
 
 class ZONETypeSub(TemplatedType, supermod.ZONEType):
     def __init__(self, ID=None, NAME=None, STATE=None, TEMPLATE=None, SERVER_POOL=None, **kwargs_):
         super(ZONETypeSub, self).__init__(ID, NAME, STATE, TEMPLATE, SERVER_POOL,  **kwargs_)
 supermod.ZONEType.subclass = ZONETypeSub
 # end class ZONETypeSub
 
 
-class TEMPLATEType136Sub(TemplatedType, supermod.TEMPLATEType136):
+class TEMPLATEType138Sub(TemplatedType, supermod.TEMPLATEType138):
     def __init__(self, ENDPOINT=None, **kwargs_):
-        super(TEMPLATEType136Sub, self).__init__(ENDPOINT,  **kwargs_)
-supermod.TEMPLATEType136.subclass = TEMPLATEType136Sub
-# end class TEMPLATEType136Sub
+        super(TEMPLATEType138Sub, self).__init__(ENDPOINT,  **kwargs_)
+supermod.TEMPLATEType138.subclass = TEMPLATEType138Sub
+# end class TEMPLATEType138Sub
 
 
 class SERVER_POOLTypeSub(TemplatedType, supermod.SERVER_POOLType):
     def __init__(self, SERVER=None, **kwargs_):
         super(SERVER_POOLTypeSub, self).__init__(SERVER,  **kwargs_)
 supermod.SERVER_POOLType.subclass = SERVER_POOLTypeSub
 # end class SERVER_POOLTypeSub
@@ -2065,33 +2086,33 @@
 class SERVERTypeSub(TemplatedType, supermod.SERVERType):
     def __init__(self, ENDPOINT=None, ID=None, NAME=None, **kwargs_):
         super(SERVERTypeSub, self).__init__(ENDPOINT, ID, NAME,  **kwargs_)
 supermod.SERVERType.subclass = SERVERTypeSub
 # end class SERVERTypeSub
 
 
-class TEMPLATEType137Sub(TemplatedType, supermod.TEMPLATEType137):
+class TEMPLATEType139Sub(TemplatedType, supermod.TEMPLATEType139):
     def __init__(self, ENDPOINT=None, **kwargs_):
-        super(TEMPLATEType137Sub, self).__init__(ENDPOINT,  **kwargs_)
-supermod.TEMPLATEType137.subclass = TEMPLATEType137Sub
-# end class TEMPLATEType137Sub
+        super(TEMPLATEType139Sub, self).__init__(ENDPOINT,  **kwargs_)
+supermod.TEMPLATEType139.subclass = TEMPLATEType139Sub
+# end class TEMPLATEType139Sub
 
 
-class SERVER_POOLType138Sub(TemplatedType, supermod.SERVER_POOLType138):
+class SERVER_POOLType140Sub(TemplatedType, supermod.SERVER_POOLType140):
     def __init__(self, SERVER=None, **kwargs_):
-        super(SERVER_POOLType138Sub, self).__init__(SERVER,  **kwargs_)
-supermod.SERVER_POOLType138.subclass = SERVER_POOLType138Sub
-# end class SERVER_POOLType138Sub
+        super(SERVER_POOLType140Sub, self).__init__(SERVER,  **kwargs_)
+supermod.SERVER_POOLType140.subclass = SERVER_POOLType140Sub
+# end class SERVER_POOLType140Sub
 
 
-class SERVERType139Sub(TemplatedType, supermod.SERVERType139):
+class SERVERType141Sub(TemplatedType, supermod.SERVERType141):
     def __init__(self, ENDPOINT=None, ID=None, NAME=None, STATE=None, TERM=None, VOTEDFOR=None, COMMIT=None, LOG_INDEX=None, FEDLOG_INDEX=None, **kwargs_):
-        super(SERVERType139Sub, self).__init__(ENDPOINT, ID, NAME, STATE, TERM, VOTEDFOR, COMMIT, LOG_INDEX, FEDLOG_INDEX,  **kwargs_)
-supermod.SERVERType139.subclass = SERVERType139Sub
-# end class SERVERType139Sub
+        super(SERVERType141Sub, self).__init__(ENDPOINT, ID, NAME, STATE, TERM, VOTEDFOR, COMMIT, LOG_INDEX, FEDLOG_INDEX,  **kwargs_)
+supermod.SERVERType141.subclass = SERVERType141Sub
+# end class SERVERType141Sub
 
 
 def get_root_tag(node):
     tag = supermod.Tag_pattern_.match(node.tag).groups()[-1]
     rootClass = None
     rootClass = supermod.GDSClassesMapping.get(tag)
     if rootClass is None and hasattr(supermod, tag):
```

### Comparing `pyone-6.6.0/pyone/bindings/supbind.py` & `pyone-6.6.1/pyone/bindings/supbind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Wed Dec 21 12:18:12 2022 by generateDS.py version 2.41.1.
+# Generated Tue Mar  7 10:35:44 2023 by generateDS.py version 2.41.3.
 # Python 3.8.10 (default, Nov 14 2022, 12:59:47)  [GCC 9.4.0]
 #
 # Command line options:
 #   ('-q', '')
 #   ('-f', '')
 #   ('-o', 'pyone/bindings/supbind.py')
 #   ('-s', 'pyone/bindings/__init__.py')
@@ -14,15 +14,15 @@
 #   ('--external-encoding', 'utf-8')
 #   ('--silence', '')
 #
 # Command line arguments:
 #   ../../../share/doc/xsd/index.xsd
 #
 # Command line:
-#   /home/one/init-build-jenkins.MUCv2w/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
+#   /home/one/init-build-jenkins.T9TFrJ/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
 #
 # Current working directory (os.getcwd()):
 #   python
 #
 
 import sys
 try:
@@ -4593,20 +4593,20 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType34.factory(parent_object_=self)
+            obj_ = LOCKType36.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType35.factory(parent_object_=self)
+            obj_ = PERMISSIONSType37.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'TYPE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'TYPE')
             ival_ = self.gds_validate_integer(ival_, node, 'TYPE')
@@ -4705,35 +4705,35 @@
         elif nodeName_ == 'DATASTORE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'DATASTORE')
             value_ = self.gds_validate_string(value_, node, 'DATASTORE')
             self.DATASTORE = value_
             self.DATASTORE_nsprefix_ = child_.prefix
         elif nodeName_ == 'VMS':
-            obj_ = VMSType36.factory(parent_object_=self)
+            obj_ = VMSType38.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VMS = obj_
             obj_.original_tagname_ = 'VMS'
         elif nodeName_ == 'CLONES':
             obj_ = CLONESType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.CLONES = obj_
             obj_.original_tagname_ = 'CLONES'
         elif nodeName_ == 'APP_CLONES':
             obj_ = APP_CLONESType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.APP_CLONES = obj_
             obj_.original_tagname_ = 'APP_CLONES'
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType37.factory(parent_object_=self)
+            obj_ = TEMPLATEType39.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
         elif nodeName_ == 'SNAPSHOTS':
-            obj_ = SNAPSHOTSType38.factory(parent_object_=self)
+            obj_ = SNAPSHOTSType40.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SNAPSHOTS = obj_
             obj_.original_tagname_ = 'SNAPSHOTS'
         elif nodeName_ == 'BACKUP_INCREMENTS':
             obj_ = BACKUP_INCREMENTSType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.BACKUP_INCREMENTS = obj_
@@ -5196,15 +5196,15 @@
         elif nodeName_ == 'GNAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'GNAME')
             value_ = self.gds_validate_string(value_, node, 'GNAME')
             self.GNAME = value_
             self.GNAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType40.factory(parent_object_=self)
+            obj_ = LOCKType42.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'REGTIME' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REGTIME')
             ival_ = self.gds_validate_integer(ival_, node, 'REGTIME')
@@ -5291,15 +5291,15 @@
         elif nodeName_ == 'TYPE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'TYPE')
             ival_ = self.gds_validate_integer(ival_, node, 'TYPE')
             self.TYPE = ival_
             self.TYPE_nsprefix_ = child_.prefix
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType41.factory(parent_object_=self)
+            obj_ = PERMISSIONSType43.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'TEMPLATE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'TEMPLATE')
             value_ = self.gds_validate_string(value_, node, 'TEMPLATE')
@@ -5722,15 +5722,15 @@
             self.USED_MB_nsprefix_ = child_.prefix
         elif nodeName_ == 'MARKETPLACEAPPS':
             obj_ = MARKETPLACEAPPSType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.MARKETPLACEAPPS = obj_
             obj_.original_tagname_ = 'MARKETPLACEAPPS'
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType42.factory(parent_object_=self)
+            obj_ = PERMISSIONSType44.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'TEMPLATE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'TEMPLATE')
             value_ = self.gds_validate_string(value_, node, 'TEMPLATE')
@@ -5830,15 +5830,15 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'MONITORING':
-            obj_ = MONITORINGType43.factory(parent_object_=self)
+            obj_ = MONITORINGType45.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.MONITORING.append(obj_)
             obj_.original_tagname_ = 'MONITORING'
 # end class MONITORING_DATA
 
 
 class OPENNEBULA_CONFIGURATION(GeneratedsSuper):
@@ -8433,15 +8433,15 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType44.factory(parent_object_=self)
+            obj_ = PERMISSIONSType46.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'UPDATED_VMS':
             obj_ = UPDATED_VMSType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.UPDATED_VMS = obj_
@@ -8458,15 +8458,15 @@
             obj_.original_tagname_ = 'UPDATING_VMS'
         elif nodeName_ == 'ERROR_VMS':
             obj_ = ERROR_VMSType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.ERROR_VMS = obj_
             obj_.original_tagname_ = 'ERROR_VMS'
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType45.factory(parent_object_=self)
+            obj_ = TEMPLATEType47.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
 # end class SECURITY_GROUP
 
 
 class SHOWBACK_RECORDS(GeneratedsSuper):
@@ -8696,15 +8696,15 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'USER':
             obj_ = USERType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.USER.append(obj_)
             obj_.original_tagname_ = 'USER'
         elif nodeName_ == 'QUOTAS':
-            obj_ = QUOTASType46.factory(parent_object_=self)
+            obj_ = QUOTASType48.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.QUOTAS.append(obj_)
             obj_.original_tagname_ = 'QUOTAS'
         elif nodeName_ == 'DEFAULT_USER_QUOTAS':
             obj_ = DEFAULT_USER_QUOTASType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DEFAULT_USER_QUOTAS = obj_
@@ -8963,15 +8963,15 @@
         elif nodeName_ == 'GID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'GID')
             ival_ = self.gds_validate_integer(ival_, node, 'GID')
             self.GID = ival_
             self.GID_nsprefix_ = child_.prefix
         elif nodeName_ == 'GROUPS':
-            obj_ = GROUPSType63.factory(parent_object_=self)
+            obj_ = GROUPSType65.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.GROUPS = obj_
             obj_.original_tagname_ = 'GROUPS'
         elif nodeName_ == 'GNAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'GNAME')
             value_ = self.gds_validate_string(value_, node, 'GNAME')
@@ -8998,46 +8998,46 @@
         elif nodeName_ == 'ENABLED' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ENABLED')
             ival_ = self.gds_validate_integer(ival_, node, 'ENABLED')
             self.ENABLED = ival_
             self.ENABLED_nsprefix_ = child_.prefix
         elif nodeName_ == 'LOGIN_TOKEN':
-            obj_ = LOGIN_TOKENType64.factory(parent_object_=self)
+            obj_ = LOGIN_TOKENType66.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOGIN_TOKEN.append(obj_)
             obj_.original_tagname_ = 'LOGIN_TOKEN'
         elif nodeName_ == 'TEMPLATE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'TEMPLATE')
             value_ = self.gds_validate_string(value_, node, 'TEMPLATE')
             self.TEMPLATE = value_
             self.TEMPLATE_nsprefix_ = child_.prefix
         elif nodeName_ == 'DATASTORE_QUOTA':
-            obj_ = DATASTORE_QUOTAType65.factory(parent_object_=self)
+            obj_ = DATASTORE_QUOTAType67.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE_QUOTA = obj_
             obj_.original_tagname_ = 'DATASTORE_QUOTA'
         elif nodeName_ == 'NETWORK_QUOTA':
-            obj_ = NETWORK_QUOTAType67.factory(parent_object_=self)
+            obj_ = NETWORK_QUOTAType69.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK_QUOTA = obj_
             obj_.original_tagname_ = 'NETWORK_QUOTA'
         elif nodeName_ == 'VM_QUOTA':
-            obj_ = VM_QUOTAType69.factory(parent_object_=self)
+            obj_ = VM_QUOTAType71.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM_QUOTA = obj_
             obj_.original_tagname_ = 'VM_QUOTA'
         elif nodeName_ == 'IMAGE_QUOTA':
-            obj_ = IMAGE_QUOTAType71.factory(parent_object_=self)
+            obj_ = IMAGE_QUOTAType73.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE_QUOTA = obj_
             obj_.original_tagname_ = 'IMAGE_QUOTA'
         elif nodeName_ == 'DEFAULT_USER_QUOTAS':
-            obj_ = DEFAULT_USER_QUOTASType73.factory(parent_object_=self)
+            obj_ = DEFAULT_USER_QUOTASType75.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DEFAULT_USER_QUOTAS = obj_
             obj_.original_tagname_ = 'DEFAULT_USER_QUOTAS'
 # end class USER
 
 
 class VDC_POOL(GeneratedsSuper):
@@ -9309,35 +9309,35 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'GROUPS':
-            obj_ = GROUPSType82.factory(parent_object_=self)
+            obj_ = GROUPSType84.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.GROUPS = obj_
             obj_.original_tagname_ = 'GROUPS'
         elif nodeName_ == 'CLUSTERS':
-            obj_ = CLUSTERSType83.factory(parent_object_=self)
+            obj_ = CLUSTERSType85.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.CLUSTERS = obj_
             obj_.original_tagname_ = 'CLUSTERS'
         elif nodeName_ == 'HOSTS':
-            obj_ = HOSTSType84.factory(parent_object_=self)
+            obj_ = HOSTSType86.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.HOSTS = obj_
             obj_.original_tagname_ = 'HOSTS'
         elif nodeName_ == 'DATASTORES':
-            obj_ = DATASTORESType85.factory(parent_object_=self)
+            obj_ = DATASTORESType87.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORES = obj_
             obj_.original_tagname_ = 'DATASTORES'
         elif nodeName_ == 'VNETS':
-            obj_ = VNETSType87.factory(parent_object_=self)
+            obj_ = VNETSType89.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VNETS = obj_
             obj_.original_tagname_ = 'VNETS'
         elif nodeName_ == 'TEMPLATE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'TEMPLATE')
             value_ = self.gds_validate_string(value_, node, 'TEMPLATE')
@@ -9663,20 +9663,20 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType88.factory(parent_object_=self)
+            obj_ = PERMISSIONSType90.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType89.factory(parent_object_=self)
+            obj_ = LOCKType91.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'ROLES':
             obj_ = ROLESType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.ROLES = obj_
@@ -9781,15 +9781,15 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'VM':
-            obj_ = VMType90.factory(parent_object_=self)
+            obj_ = VMType92.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM.append(obj_)
             obj_.original_tagname_ = 'VM'
 # end class VM_POOL
 
 
 class VMTEMPLATE_POOL(GeneratedsSuper):
@@ -10109,31 +10109,31 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType93.factory(parent_object_=self)
+            obj_ = LOCKType95.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType94.factory(parent_object_=self)
+            obj_ = PERMISSIONSType96.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'REGTIME' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REGTIME')
             ival_ = self.gds_validate_integer(ival_, node, 'REGTIME')
             self.REGTIME = ival_
             self.REGTIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType95.factory(parent_object_=self)
+            obj_ = TEMPLATEType97.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
 # end class VMTEMPLATE
 
 
 class VM(GeneratedsSuper):
@@ -10498,15 +10498,15 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType96.factory(parent_object_=self)
+            obj_ = PERMISSIONSType98.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'LAST_POLL' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'LAST_POLL')
             ival_ = self.gds_validate_integer(ival_, node, 'LAST_POLL')
@@ -10557,45 +10557,45 @@
         elif nodeName_ == 'DEPLOY_ID':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'DEPLOY_ID')
             value_ = self.gds_validate_string(value_, node, 'DEPLOY_ID')
             self.DEPLOY_ID = value_
             self.DEPLOY_ID_nsprefix_ = child_.prefix
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType97.factory(parent_object_=self)
+            obj_ = LOCKType99.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'MONITORING':
-            obj_ = MONITORINGType98.factory(parent_object_=self)
+            obj_ = MONITORINGType100.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.MONITORING = obj_
             obj_.original_tagname_ = 'MONITORING'
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType100.factory(parent_object_=self)
+            obj_ = TEMPLATEType102.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
         elif nodeName_ == 'USER_TEMPLATE':
-            obj_ = USER_TEMPLATEType104.factory(parent_object_=self)
+            obj_ = USER_TEMPLATEType106.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.USER_TEMPLATE = obj_
             obj_.original_tagname_ = 'USER_TEMPLATE'
         elif nodeName_ == 'HISTORY_RECORDS':
-            obj_ = HISTORY_RECORDSType105.factory(parent_object_=self)
+            obj_ = HISTORY_RECORDSType107.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.HISTORY_RECORDS = obj_
             obj_.original_tagname_ = 'HISTORY_RECORDS'
         elif nodeName_ == 'SNAPSHOTS':
-            obj_ = SNAPSHOTSType107.factory(parent_object_=self)
+            obj_ = SNAPSHOTSType109.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SNAPSHOTS.append(obj_)
             obj_.original_tagname_ = 'SNAPSHOTS'
         elif nodeName_ == 'BACKUPS':
-            obj_ = BACKUPSType109.factory(parent_object_=self)
+            obj_ = BACKUPSType111.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.BACKUPS = obj_
             obj_.original_tagname_ = 'BACKUPS'
 # end class VM
 
 
 class VNET_POOL(GeneratedsSuper):
@@ -10689,15 +10689,15 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'VNET':
-            obj_ = VNETType112.factory(parent_object_=self)
+            obj_ = VNETType114.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VNET.append(obj_)
             obj_.original_tagname_ = 'VNET'
 # end class VNET_POOL
 
 
 class VNET(GeneratedsSuper):
@@ -11106,25 +11106,25 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType119.factory(parent_object_=self)
+            obj_ = LOCKType121.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType120.factory(parent_object_=self)
+            obj_ = PERMISSIONSType122.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'CLUSTERS':
-            obj_ = CLUSTERSType121.factory(parent_object_=self)
+            obj_ = CLUSTERSType123.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.CLUSTERS = obj_
             obj_.original_tagname_ = 'CLUSTERS'
         elif nodeName_ == 'BRIDGE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'BRIDGE')
             value_ = self.gds_validate_string(value_, node, 'BRIDGE')
@@ -11193,45 +11193,45 @@
         elif nodeName_ == 'USED_LEASES' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'USED_LEASES')
             ival_ = self.gds_validate_integer(ival_, node, 'USED_LEASES')
             self.USED_LEASES = ival_
             self.USED_LEASES_nsprefix_ = child_.prefix
         elif nodeName_ == 'VROUTERS':
-            obj_ = VROUTERSType122.factory(parent_object_=self)
+            obj_ = VROUTERSType124.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VROUTERS = obj_
             obj_.original_tagname_ = 'VROUTERS'
         elif nodeName_ == 'UPDATED_VMS':
-            obj_ = UPDATED_VMSType123.factory(parent_object_=self)
+            obj_ = UPDATED_VMSType125.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.UPDATED_VMS = obj_
             obj_.original_tagname_ = 'UPDATED_VMS'
         elif nodeName_ == 'OUTDATED_VMS':
-            obj_ = OUTDATED_VMSType124.factory(parent_object_=self)
+            obj_ = OUTDATED_VMSType126.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.OUTDATED_VMS = obj_
             obj_.original_tagname_ = 'OUTDATED_VMS'
         elif nodeName_ == 'UPDATING_VMS':
-            obj_ = UPDATING_VMSType125.factory(parent_object_=self)
+            obj_ = UPDATING_VMSType127.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.UPDATING_VMS = obj_
             obj_.original_tagname_ = 'UPDATING_VMS'
         elif nodeName_ == 'ERROR_VMS':
-            obj_ = ERROR_VMSType126.factory(parent_object_=self)
+            obj_ = ERROR_VMSType128.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.ERROR_VMS = obj_
             obj_.original_tagname_ = 'ERROR_VMS'
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType127.factory(parent_object_=self)
+            obj_ = TEMPLATEType129.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
         elif nodeName_ == 'AR_POOL':
-            obj_ = AR_POOLType128.factory(parent_object_=self)
+            obj_ = AR_POOLType130.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.AR_POOL = obj_
             obj_.original_tagname_ = 'AR_POOL'
 # end class VNET
 
 
 class VNTEMPLATE_POOL(GeneratedsSuper):
@@ -11551,31 +11551,31 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType130.factory(parent_object_=self)
+            obj_ = LOCKType132.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType131.factory(parent_object_=self)
+            obj_ = PERMISSIONSType133.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'REGTIME' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REGTIME')
             ival_ = self.gds_validate_integer(ival_, node, 'REGTIME')
             self.REGTIME = ival_
             self.REGTIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType132.factory(parent_object_=self)
+            obj_ = TEMPLATEType134.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
 # end class VNTEMPLATE
 
 
 class VROUTER_POOL(GeneratedsSuper):
@@ -11895,25 +11895,25 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType133.factory(parent_object_=self)
+            obj_ = PERMISSIONSType135.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'LOCK':
-            obj_ = LOCKType134.factory(parent_object_=self)
+            obj_ = LOCKType136.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LOCK = obj_
             obj_.original_tagname_ = 'LOCK'
         elif nodeName_ == 'VMS':
-            obj_ = VMSType135.factory(parent_object_=self)
+            obj_ = VMSType137.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VMS = obj_
             obj_.original_tagname_ = 'VMS'
         elif nodeName_ == 'TEMPLATE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'TEMPLATE')
             value_ = self.gds_validate_string(value_, node, 'TEMPLATE')
@@ -12167,20 +12167,20 @@
         elif nodeName_ == 'STATE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'STATE')
             ival_ = self.gds_validate_integer(ival_, node, 'STATE')
             self.STATE = ival_
             self.STATE_nsprefix_ = child_.prefix
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType137.factory(parent_object_=self)
+            obj_ = TEMPLATEType139.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
         elif nodeName_ == 'SERVER_POOL':
-            obj_ = SERVER_POOLType138.factory(parent_object_=self)
+            obj_ = SERVER_POOLType140.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SERVER_POOL = obj_
             obj_.original_tagname_ = 'SERVER_POOL'
 # end class ZONE
 
 
 class VMType(GeneratedsSuper):
@@ -23122,22 +23122,20 @@
 # end class COREType
 
 
 class HUGEPAGEType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, FREE=None, PAGES=None, SIZE=None, USAGE=None, gds_collector_=None, **kwargs_):
+    def __init__(self, PAGES=None, SIZE=None, USAGE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
-        self.FREE = FREE
-        self.FREE_nsprefix_ = None
         self.PAGES = PAGES
         self.PAGES_nsprefix_ = None
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
         self.USAGE = USAGE
         self.USAGE_nsprefix_ = None
     def factory(*args_, **kwargs_):
@@ -23151,33 +23149,28 @@
         else:
             return HUGEPAGEType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def get_FREE(self):
-        return self.FREE
-    def set_FREE(self, FREE):
-        self.FREE = FREE
     def get_PAGES(self):
         return self.PAGES
     def set_PAGES(self, PAGES):
         self.PAGES = PAGES
     def get_SIZE(self):
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_USAGE(self):
         return self.USAGE
     def set_USAGE(self, USAGE):
         self.USAGE = USAGE
     def _hasContent(self):
         if (
-            self.FREE is not None or
             self.PAGES is not None or
             self.SIZE is not None or
             self.USAGE is not None
         ):
             return True
         else:
             return False
@@ -23207,18 +23200,14 @@
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HUGEPAGEType'):
         pass
     def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HUGEPAGEType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.FREE is not None:
-            namespaceprefix_ = self.FREE_nsprefix_ + ':' if (UseCapturedNS_ and self.FREE_nsprefix_) else ''
-            showIndent(outfile, level, pretty_print)
-            outfile.write('<%sFREE>%s</%sFREE>%s' % (namespaceprefix_ , self.gds_format_integer(self.FREE, input_name='FREE'), namespaceprefix_ , eol_))
         if self.PAGES is not None:
             namespaceprefix_ = self.PAGES_nsprefix_ + ':' if (UseCapturedNS_ and self.PAGES_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sPAGES>%s</%sPAGES>%s' % (namespaceprefix_ , self.gds_format_integer(self.PAGES, input_name='PAGES'), namespaceprefix_ , eol_))
         if self.SIZE is not None:
             namespaceprefix_ = self.SIZE_nsprefix_ + ':' if (UseCapturedNS_ and self.SIZE_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -23237,21 +23226,15 @@
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        if nodeName_ == 'FREE' and child_.text:
-            sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'FREE')
-            ival_ = self.gds_validate_integer(ival_, node, 'FREE')
-            self.FREE = ival_
-            self.FREE_nsprefix_ = child_.prefix
-        elif nodeName_ == 'PAGES' and child_.text:
+        if nodeName_ == 'PAGES' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'PAGES')
             ival_ = self.gds_validate_integer(ival_, node, 'PAGES')
             self.PAGES = ival_
             self.PAGES_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE' and child_.text:
             sval_ = child_.text
@@ -23268,30 +23251,26 @@
 # end class HUGEPAGEType
 
 
 class MEMORYType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, DISTANCE=None, FREE=None, TOTAL=None, USAGE=None, USED=None, gds_collector_=None, **kwargs_):
+    def __init__(self, DISTANCE=None, TOTAL=None, USAGE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.DISTANCE = DISTANCE
         self.DISTANCE_nsprefix_ = None
-        self.FREE = FREE
-        self.FREE_nsprefix_ = None
         self.TOTAL = TOTAL
         self.TOTAL_nsprefix_ = None
         self.USAGE = USAGE
         self.USAGE_nsprefix_ = None
-        self.USED = USED
-        self.USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, MEMORYType)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if MEMORYType.subclass:
@@ -23303,37 +23282,27 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DISTANCE(self):
         return self.DISTANCE
     def set_DISTANCE(self, DISTANCE):
         self.DISTANCE = DISTANCE
-    def get_FREE(self):
-        return self.FREE
-    def set_FREE(self, FREE):
-        self.FREE = FREE
     def get_TOTAL(self):
         return self.TOTAL
     def set_TOTAL(self, TOTAL):
         self.TOTAL = TOTAL
     def get_USAGE(self):
         return self.USAGE
     def set_USAGE(self, USAGE):
         self.USAGE = USAGE
-    def get_USED(self):
-        return self.USED
-    def set_USED(self, USED):
-        self.USED = USED
     def _hasContent(self):
         if (
             self.DISTANCE is not None or
-            self.FREE is not None or
             self.TOTAL is not None or
-            self.USAGE is not None or
-            self.USED is not None
+            self.USAGE is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MEMORYType', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('MEMORYType')
         if imported_ns_def_ is not None:
@@ -23364,30 +23333,22 @@
             eol_ = '\n'
         else:
             eol_ = ''
         if self.DISTANCE is not None:
             namespaceprefix_ = self.DISTANCE_nsprefix_ + ':' if (UseCapturedNS_ and self.DISTANCE_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sDISTANCE>%s</%sDISTANCE>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.DISTANCE), input_name='DISTANCE')), namespaceprefix_ , eol_))
-        if self.FREE is not None:
-            namespaceprefix_ = self.FREE_nsprefix_ + ':' if (UseCapturedNS_ and self.FREE_nsprefix_) else ''
-            showIndent(outfile, level, pretty_print)
-            outfile.write('<%sFREE>%s</%sFREE>%s' % (namespaceprefix_ , self.gds_format_integer(self.FREE, input_name='FREE'), namespaceprefix_ , eol_))
         if self.TOTAL is not None:
             namespaceprefix_ = self.TOTAL_nsprefix_ + ':' if (UseCapturedNS_ and self.TOTAL_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sTOTAL>%s</%sTOTAL>%s' % (namespaceprefix_ , self.gds_format_integer(self.TOTAL, input_name='TOTAL'), namespaceprefix_ , eol_))
         if self.USAGE is not None:
             namespaceprefix_ = self.USAGE_nsprefix_ + ':' if (UseCapturedNS_ and self.USAGE_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sUSAGE>%s</%sUSAGE>%s' % (namespaceprefix_ , self.gds_format_integer(self.USAGE, input_name='USAGE'), namespaceprefix_ , eol_))
-        if self.USED is not None:
-            namespaceprefix_ = self.USED_nsprefix_ + ':' if (UseCapturedNS_ and self.USED_nsprefix_) else ''
-            showIndent(outfile, level, pretty_print)
-            outfile.write('<%sUSED>%s</%sUSED>%s' % (namespaceprefix_ , self.gds_format_integer(self.USED, input_name='USED'), namespaceprefix_ , eol_))
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
         self._buildAttributes(node, node.attrib, already_processed)
@@ -23400,38 +23361,26 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DISTANCE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'DISTANCE')
             value_ = self.gds_validate_string(value_, node, 'DISTANCE')
             self.DISTANCE = value_
             self.DISTANCE_nsprefix_ = child_.prefix
-        elif nodeName_ == 'FREE' and child_.text:
-            sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'FREE')
-            ival_ = self.gds_validate_integer(ival_, node, 'FREE')
-            self.FREE = ival_
-            self.FREE_nsprefix_ = child_.prefix
         elif nodeName_ == 'TOTAL' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'TOTAL')
             ival_ = self.gds_validate_integer(ival_, node, 'TOTAL')
             self.TOTAL = ival_
             self.TOTAL_nsprefix_ = child_.prefix
         elif nodeName_ == 'USAGE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'USAGE')
             ival_ = self.gds_validate_integer(ival_, node, 'USAGE')
             self.USAGE = ival_
             self.USAGE_nsprefix_ = child_.prefix
-        elif nodeName_ == 'USED' and child_.text:
-            sval_ = child_.text
-            ival_ = self.gds_parse_integer(sval_, node, 'USED')
-            ival_ = self.gds_validate_integer(ival_, node, 'USED')
-            self.USED = ival_
-            self.USED_nsprefix_ = child_.prefix
 # end class MEMORYType
 
 
 class VMSType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
@@ -23877,28 +23826,33 @@
 # end class VCENTER_RESOURCE_POOL_INFO
 
 
 class MONITORINGType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, TIMESTAMP=None, ID=None, CAPACITY=None, SYSTEM=None, gds_collector_=None, **kwargs_):
+    def __init__(self, TIMESTAMP=None, ID=None, CAPACITY=None, SYSTEM=None, NUMA_NODE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.TIMESTAMP = TIMESTAMP
         self.TIMESTAMP_nsprefix_ = None
         self.ID = ID
         self.ID_nsprefix_ = None
         self.CAPACITY = CAPACITY
         self.CAPACITY_nsprefix_ = None
         self.SYSTEM = SYSTEM
         self.SYSTEM_nsprefix_ = None
+        if NUMA_NODE is None:
+            self.NUMA_NODE = []
+        else:
+            self.NUMA_NODE = NUMA_NODE
+        self.NUMA_NODE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, MONITORINGType)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if MONITORINGType.subclass:
@@ -23922,20 +23876,31 @@
         return self.CAPACITY
     def set_CAPACITY(self, CAPACITY):
         self.CAPACITY = CAPACITY
     def get_SYSTEM(self):
         return self.SYSTEM
     def set_SYSTEM(self, SYSTEM):
         self.SYSTEM = SYSTEM
+    def get_NUMA_NODE(self):
+        return self.NUMA_NODE
+    def set_NUMA_NODE(self, NUMA_NODE):
+        self.NUMA_NODE = NUMA_NODE
+    def add_NUMA_NODE(self, value):
+        self.NUMA_NODE.append(value)
+    def insert_NUMA_NODE_at(self, index, value):
+        self.NUMA_NODE.insert(index, value)
+    def replace_NUMA_NODE_at(self, index, value):
+        self.NUMA_NODE[index] = value
     def _hasContent(self):
         if (
             self.TIMESTAMP is not None or
             self.ID is not None or
             self.CAPACITY is not None or
-            self.SYSTEM is not None
+            self.SYSTEM is not None or
+            self.NUMA_NODE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('MONITORINGType')
         if imported_ns_def_ is not None:
@@ -23976,14 +23941,17 @@
             outfile.write('<%sID>%s</%sID>%s' % (namespaceprefix_ , self.gds_format_integer(self.ID, input_name='ID'), namespaceprefix_ , eol_))
         if self.CAPACITY is not None:
             namespaceprefix_ = self.CAPACITY_nsprefix_ + ':' if (UseCapturedNS_ and self.CAPACITY_nsprefix_) else ''
             self.CAPACITY.export(outfile, level, namespaceprefix_, namespacedef_='', name_='CAPACITY', pretty_print=pretty_print)
         if self.SYSTEM is not None:
             namespaceprefix_ = self.SYSTEM_nsprefix_ + ':' if (UseCapturedNS_ and self.SYSTEM_nsprefix_) else ''
             self.SYSTEM.export(outfile, level, namespaceprefix_, namespacedef_='', name_='SYSTEM', pretty_print=pretty_print)
+        for NUMA_NODE_ in self.NUMA_NODE:
+            namespaceprefix_ = self.NUMA_NODE_nsprefix_ + ':' if (UseCapturedNS_ and self.NUMA_NODE_nsprefix_) else ''
+            NUMA_NODE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='NUMA_NODE', pretty_print=pretty_print)
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
         self._buildAttributes(node, node.attrib, already_processed)
@@ -24012,14 +23980,19 @@
             self.CAPACITY = obj_
             obj_.original_tagname_ = 'CAPACITY'
         elif nodeName_ == 'SYSTEM':
             obj_ = SYSTEMType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SYSTEM = obj_
             obj_.original_tagname_ = 'SYSTEM'
+        elif nodeName_ == 'NUMA_NODE':
+            obj_ = NUMA_NODEType.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.NUMA_NODE.append(obj_)
+            obj_.original_tagname_ = 'NUMA_NODE'
 # end class MONITORINGType
 
 
 class CAPACITYType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
@@ -24273,15 +24246,373 @@
             ival_ = self.gds_parse_integer(sval_, node, 'NETTX')
             ival_ = self.gds_validate_integer(ival_, node, 'NETTX')
             self.NETTX = ival_
             self.NETTX_nsprefix_ = child_.prefix
 # end class SYSTEMType
 
 
-class LOCKType34(GeneratedsSuper):
+class NUMA_NODEType(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, HUGEPAGE=None, MEMORY=None, NODE_ID=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        if HUGEPAGE is None:
+            self.HUGEPAGE = []
+        else:
+            self.HUGEPAGE = HUGEPAGE
+        self.HUGEPAGE_nsprefix_ = None
+        self.MEMORY = MEMORY
+        self.MEMORY_nsprefix_ = None
+        self.NODE_ID = NODE_ID
+        self.NODE_ID_nsprefix_ = None
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, NUMA_NODEType)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if NUMA_NODEType.subclass:
+            return NUMA_NODEType.subclass(*args_, **kwargs_)
+        else:
+            return NUMA_NODEType(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_HUGEPAGE(self):
+        return self.HUGEPAGE
+    def set_HUGEPAGE(self, HUGEPAGE):
+        self.HUGEPAGE = HUGEPAGE
+    def add_HUGEPAGE(self, value):
+        self.HUGEPAGE.append(value)
+    def insert_HUGEPAGE_at(self, index, value):
+        self.HUGEPAGE.insert(index, value)
+    def replace_HUGEPAGE_at(self, index, value):
+        self.HUGEPAGE[index] = value
+    def get_MEMORY(self):
+        return self.MEMORY
+    def set_MEMORY(self, MEMORY):
+        self.MEMORY = MEMORY
+    def get_NODE_ID(self):
+        return self.NODE_ID
+    def set_NODE_ID(self, NODE_ID):
+        self.NODE_ID = NODE_ID
+    def _hasContent(self):
+        if (
+            self.HUGEPAGE or
+            self.MEMORY is not None or
+            self.NODE_ID is not None
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NUMA_NODEType', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NUMA_NODEType')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'NUMA_NODEType':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NUMA_NODEType')
+        if self._hasContent():
+            outfile.write('>%s' % (eol_, ))
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NUMA_NODEType', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NUMA_NODEType'):
+        pass
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NUMA_NODEType', fromsubclass_=False, pretty_print=True):
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        for HUGEPAGE_ in self.HUGEPAGE:
+            namespaceprefix_ = self.HUGEPAGE_nsprefix_ + ':' if (UseCapturedNS_ and self.HUGEPAGE_nsprefix_) else ''
+            HUGEPAGE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='HUGEPAGE', pretty_print=pretty_print)
+        if self.MEMORY is not None:
+            namespaceprefix_ = self.MEMORY_nsprefix_ + ':' if (UseCapturedNS_ and self.MEMORY_nsprefix_) else ''
+            self.MEMORY.export(outfile, level, namespaceprefix_, namespacedef_='', name_='MEMORY', pretty_print=pretty_print)
+        if self.NODE_ID is not None:
+            namespaceprefix_ = self.NODE_ID_nsprefix_ + ':' if (UseCapturedNS_ and self.NODE_ID_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sNODE_ID>%s</%sNODE_ID>%s' % (namespaceprefix_ , self.gds_format_integer(self.NODE_ID, input_name='NODE_ID'), namespaceprefix_ , eol_))
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+    def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'HUGEPAGE':
+            obj_ = HUGEPAGEType34.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.HUGEPAGE.append(obj_)
+            obj_.original_tagname_ = 'HUGEPAGE'
+        elif nodeName_ == 'MEMORY':
+            obj_ = MEMORYType35.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.MEMORY = obj_
+            obj_.original_tagname_ = 'MEMORY'
+        elif nodeName_ == 'NODE_ID' and child_.text:
+            sval_ = child_.text
+            ival_ = self.gds_parse_integer(sval_, node, 'NODE_ID')
+            ival_ = self.gds_validate_integer(ival_, node, 'NODE_ID')
+            self.NODE_ID = ival_
+            self.NODE_ID_nsprefix_ = child_.prefix
+# end class NUMA_NODEType
+
+
+class HUGEPAGEType34(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, FREE=None, SIZE=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        self.FREE = FREE
+        self.FREE_nsprefix_ = None
+        self.SIZE = SIZE
+        self.SIZE_nsprefix_ = None
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, HUGEPAGEType34)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if HUGEPAGEType34.subclass:
+            return HUGEPAGEType34.subclass(*args_, **kwargs_)
+        else:
+            return HUGEPAGEType34(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_FREE(self):
+        return self.FREE
+    def set_FREE(self, FREE):
+        self.FREE = FREE
+    def get_SIZE(self):
+        return self.SIZE
+    def set_SIZE(self, SIZE):
+        self.SIZE = SIZE
+    def _hasContent(self):
+        if (
+            self.FREE is not None or
+            self.SIZE is not None
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HUGEPAGEType34', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('HUGEPAGEType34')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'HUGEPAGEType34':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HUGEPAGEType34')
+        if self._hasContent():
+            outfile.write('>%s' % (eol_, ))
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HUGEPAGEType34', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HUGEPAGEType34'):
+        pass
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HUGEPAGEType34', fromsubclass_=False, pretty_print=True):
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.FREE is not None:
+            namespaceprefix_ = self.FREE_nsprefix_ + ':' if (UseCapturedNS_ and self.FREE_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sFREE>%s</%sFREE>%s' % (namespaceprefix_ , self.gds_format_integer(self.FREE, input_name='FREE'), namespaceprefix_ , eol_))
+        if self.SIZE is not None:
+            namespaceprefix_ = self.SIZE_nsprefix_ + ':' if (UseCapturedNS_ and self.SIZE_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sSIZE>%s</%sSIZE>%s' % (namespaceprefix_ , self.gds_format_integer(self.SIZE, input_name='SIZE'), namespaceprefix_ , eol_))
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+    def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'FREE' and child_.text:
+            sval_ = child_.text
+            ival_ = self.gds_parse_integer(sval_, node, 'FREE')
+            ival_ = self.gds_validate_integer(ival_, node, 'FREE')
+            self.FREE = ival_
+            self.FREE_nsprefix_ = child_.prefix
+        elif nodeName_ == 'SIZE' and child_.text:
+            sval_ = child_.text
+            ival_ = self.gds_parse_integer(sval_, node, 'SIZE')
+            ival_ = self.gds_validate_integer(ival_, node, 'SIZE')
+            self.SIZE = ival_
+            self.SIZE_nsprefix_ = child_.prefix
+# end class HUGEPAGEType34
+
+
+class MEMORYType35(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    subclass = None
+    superclass = None
+    def __init__(self, FREE=None, USED=None, gds_collector_=None, **kwargs_):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get('parent_object_')
+        self.ns_prefix_ = None
+        self.FREE = FREE
+        self.FREE_nsprefix_ = None
+        self.USED = USED
+        self.USED_nsprefix_ = None
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(
+                CurrentSubclassModule_, MEMORYType35)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if MEMORYType35.subclass:
+            return MEMORYType35.subclass(*args_, **kwargs_)
+        else:
+            return MEMORYType35(*args_, **kwargs_)
+    factory = staticmethod(factory)
+    def get_ns_prefix_(self):
+        return self.ns_prefix_
+    def set_ns_prefix_(self, ns_prefix):
+        self.ns_prefix_ = ns_prefix
+    def get_FREE(self):
+        return self.FREE
+    def set_FREE(self, FREE):
+        self.FREE = FREE
+    def get_USED(self):
+        return self.USED
+    def set_USED(self, USED):
+        self.USED = USED
+    def _hasContent(self):
+        if (
+            self.FREE is not None or
+            self.USED is not None
+        ):
+            return True
+        else:
+            return False
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MEMORYType35', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('MEMORYType35')
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.original_tagname_ is not None and name_ == 'MEMORYType35':
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ':'
+        showIndent(outfile, level, pretty_print)
+        outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
+        already_processed = set()
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MEMORYType35')
+        if self._hasContent():
+            outfile.write('>%s' % (eol_, ))
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MEMORYType35', pretty_print=pretty_print)
+            showIndent(outfile, level, pretty_print)
+            outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write('/>%s' % (eol_, ))
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MEMORYType35'):
+        pass
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MEMORYType35', fromsubclass_=False, pretty_print=True):
+        if pretty_print:
+            eol_ = '\n'
+        else:
+            eol_ = ''
+        if self.FREE is not None:
+            namespaceprefix_ = self.FREE_nsprefix_ + ':' if (UseCapturedNS_ and self.FREE_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sFREE>%s</%sFREE>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.FREE), input_name='FREE')), namespaceprefix_ , eol_))
+        if self.USED is not None:
+            namespaceprefix_ = self.USED_nsprefix_ + ':' if (UseCapturedNS_ and self.USED_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sUSED>%s</%sUSED>%s' % (namespaceprefix_ , self.gds_format_integer(self.USED, input_name='USED'), namespaceprefix_ , eol_))
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+    def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
+        if nodeName_ == 'FREE':
+            value_ = child_.text
+            value_ = self.gds_parse_string(value_, node, 'FREE')
+            value_ = self.gds_validate_string(value_, node, 'FREE')
+            self.FREE = value_
+            self.FREE_nsprefix_ = child_.prefix
+        elif nodeName_ == 'USED' and child_.text:
+            sval_ = child_.text
+            ival_ = self.gds_parse_integer(sval_, node, 'USED')
+            ival_ = self.gds_validate_integer(ival_, node, 'USED')
+            self.USED = ival_
+            self.USED_nsprefix_ = child_.prefix
+# end class MEMORYType35
+
+
+class LOCKType36(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -24294,21 +24625,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType34)
+                CurrentSubclassModule_, LOCKType36)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType34.subclass:
-            return LOCKType34.subclass(*args_, **kwargs_)
+        if LOCKType36.subclass:
+            return LOCKType36.subclass(*args_, **kwargs_)
         else:
-            return LOCKType34(*args_, **kwargs_)
+            return LOCKType36(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -24332,40 +24663,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType34', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType34')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType36', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType36')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType34':
+        if self.original_tagname_ is not None and name_ == 'LOCKType36':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType34')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType36')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType34', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType36', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType34'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType36'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType34', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType36', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -24416,18 +24747,18 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType34
+# end class LOCKType36
 
 
-class PERMISSIONSType35(GeneratedsSuper):
+class PERMISSIONSType37(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -24450,21 +24781,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType35)
+                CurrentSubclassModule_, PERMISSIONSType37)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType35.subclass:
-            return PERMISSIONSType35.subclass(*args_, **kwargs_)
+        if PERMISSIONSType37.subclass:
+            return PERMISSIONSType37.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType35(*args_, **kwargs_)
+            return PERMISSIONSType37(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -24513,40 +24844,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType35', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType35')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType37', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType37')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType35':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType37':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType35')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType37')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType35', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType37', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType35'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType37'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType35', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType37', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -24647,18 +24978,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType35
+# end class PERMISSIONSType37
 
 
-class VMSType36(GeneratedsSuper):
+class VMSType38(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -24668,21 +24999,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VMSType36)
+                CurrentSubclassModule_, VMSType38)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VMSType36.subclass:
-            return VMSType36.subclass(*args_, **kwargs_)
+        if VMSType38.subclass:
+            return VMSType38.subclass(*args_, **kwargs_)
         else:
-            return VMSType36(*args_, **kwargs_)
+            return VMSType38(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -24697,40 +25028,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType36', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMSType36')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType38', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMSType38')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VMSType36':
+        if self.original_tagname_ is not None and name_ == 'VMSType38':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMSType36')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMSType38')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMSType36', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMSType38', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMSType36'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMSType38'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType36', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType38', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -24751,15 +25082,15 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class VMSType36
+# end class VMSType38
 
 
 class CLONESType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
@@ -24962,15 +25293,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
 # end class APP_CLONESType
 
 
-class TEMPLATEType37(GeneratedsSuper):
+class TEMPLATEType39(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VCENTER_IMPORTED=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -24981,21 +25312,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType37)
+                CurrentSubclassModule_, TEMPLATEType39)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType37.subclass:
-            return TEMPLATEType37.subclass(*args_, **kwargs_)
+        if TEMPLATEType39.subclass:
+            return TEMPLATEType39.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType37(*args_, **kwargs_)
+            return TEMPLATEType39(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VCENTER_IMPORTED(self):
         return self.VCENTER_IMPORTED
@@ -25009,40 +25340,40 @@
         if (
             self.VCENTER_IMPORTED is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType37', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType37')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType39', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType39')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType37':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType39':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType37')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType39')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType37', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType39', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType37'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType39'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType37', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType39', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VCENTER_IMPORTED is not None:
             namespaceprefix_ = self.VCENTER_IMPORTED_nsprefix_ + ':' if (UseCapturedNS_ and self.VCENTER_IMPORTED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -25069,20 +25400,20 @@
         if nodeName_ == 'VCENTER_IMPORTED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_IMPORTED')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_IMPORTED')
             self.VCENTER_IMPORTED = value_
             self.VCENTER_IMPORTED_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'TEMPLATEType37')
+            content_ = self.gds_build_any(child_, 'TEMPLATEType39')
             self.anytypeobjs_.append(content_)
-# end class TEMPLATEType37
+# end class TEMPLATEType39
 
 
-class SNAPSHOTSType38(GeneratedsSuper):
+class SNAPSHOTSType40(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ALLOW_ORPHANS=None, CURRENT_BASE=None, NEXT_SNAPSHOT=None, SNAPSHOT=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -25098,21 +25429,21 @@
             self.SNAPSHOT = []
         else:
             self.SNAPSHOT = SNAPSHOT
         self.SNAPSHOT_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SNAPSHOTSType38)
+                CurrentSubclassModule_, SNAPSHOTSType40)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if SNAPSHOTSType38.subclass:
-            return SNAPSHOTSType38.subclass(*args_, **kwargs_)
+        if SNAPSHOTSType40.subclass:
+            return SNAPSHOTSType40.subclass(*args_, **kwargs_)
         else:
-            return SNAPSHOTSType38(*args_, **kwargs_)
+            return SNAPSHOTSType40(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ALLOW_ORPHANS(self):
         return self.ALLOW_ORPHANS
@@ -25142,40 +25473,40 @@
             self.CURRENT_BASE is not None or
             self.NEXT_SNAPSHOT is not None or
             self.SNAPSHOT
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType38', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTSType38')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType40', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTSType40')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SNAPSHOTSType38':
+        if self.original_tagname_ is not None and name_ == 'SNAPSHOTSType40':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTSType38')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTSType40')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTSType38', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTSType40', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTSType38'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTSType40'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType38', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType40', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ALLOW_ORPHANS is not None:
             namespaceprefix_ = self.ALLOW_ORPHANS_nsprefix_ + ':' if (UseCapturedNS_ and self.ALLOW_ORPHANS_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -25220,22 +25551,22 @@
         elif nodeName_ == 'NEXT_SNAPSHOT':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NEXT_SNAPSHOT')
             value_ = self.gds_validate_string(value_, node, 'NEXT_SNAPSHOT')
             self.NEXT_SNAPSHOT = value_
             self.NEXT_SNAPSHOT_nsprefix_ = child_.prefix
         elif nodeName_ == 'SNAPSHOT':
-            obj_ = SNAPSHOTType39.factory(parent_object_=self)
+            obj_ = SNAPSHOTType41.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SNAPSHOT.append(obj_)
             obj_.original_tagname_ = 'SNAPSHOT'
-# end class SNAPSHOTSType38
+# end class SNAPSHOTSType40
 
 
-class SNAPSHOTType39(GeneratedsSuper):
+class SNAPSHOTType41(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CHILDREN=None, ACTIVE=None, DATE=None, ID=None, NAME=None, PARENT=None, SIZE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -25254,21 +25585,21 @@
         self.PARENT = PARENT
         self.PARENT_nsprefix_ = None
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SNAPSHOTType39)
+                CurrentSubclassModule_, SNAPSHOTType41)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if SNAPSHOTType39.subclass:
-            return SNAPSHOTType39.subclass(*args_, **kwargs_)
+        if SNAPSHOTType41.subclass:
+            return SNAPSHOTType41.subclass(*args_, **kwargs_)
         else:
-            return SNAPSHOTType39(*args_, **kwargs_)
+            return SNAPSHOTType41(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CHILDREN(self):
         return self.CHILDREN
@@ -25307,40 +25638,40 @@
             self.NAME is not None or
             self.PARENT is not None or
             self.SIZE is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType39', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTType39')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType41', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTType41')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SNAPSHOTType39':
+        if self.original_tagname_ is not None and name_ == 'SNAPSHOTType41':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType39')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType41')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType39', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType41', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType39'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType41'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType39', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType41', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CHILDREN is not None:
             namespaceprefix_ = self.CHILDREN_nsprefix_ + ':' if (UseCapturedNS_ and self.CHILDREN_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -25421,15 +25752,15 @@
             self.PARENT_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'SIZE')
             ival_ = self.gds_validate_integer(ival_, node, 'SIZE')
             self.SIZE = ival_
             self.SIZE_nsprefix_ = child_.prefix
-# end class SNAPSHOTType39
+# end class SNAPSHOTType41
 
 
 class BACKUP_INCREMENTSType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, INCREMENT=None, gds_collector_=None, **kwargs_):
@@ -25706,15 +26037,15 @@
             value_ = self.gds_parse_string(value_, node, 'TYPE')
             value_ = self.gds_validate_string(value_, node, 'TYPE')
             self.TYPE = value_
             self.TYPE_nsprefix_ = child_.prefix
 # end class INCREMENTType
 
 
-class LOCKType40(GeneratedsSuper):
+class LOCKType42(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -25727,21 +26058,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType40)
+                CurrentSubclassModule_, LOCKType42)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType40.subclass:
-            return LOCKType40.subclass(*args_, **kwargs_)
+        if LOCKType42.subclass:
+            return LOCKType42.subclass(*args_, **kwargs_)
         else:
-            return LOCKType40(*args_, **kwargs_)
+            return LOCKType42(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -25765,40 +26096,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType40', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType40')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType42', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType42')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType40':
+        if self.original_tagname_ is not None and name_ == 'LOCKType42':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType40')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType42')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType40', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType42', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType40'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType42'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType40', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType42', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -25849,18 +26180,18 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType40
+# end class LOCKType42
 
 
-class PERMISSIONSType41(GeneratedsSuper):
+class PERMISSIONSType43(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -25883,21 +26214,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType41)
+                CurrentSubclassModule_, PERMISSIONSType43)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType41.subclass:
-            return PERMISSIONSType41.subclass(*args_, **kwargs_)
+        if PERMISSIONSType43.subclass:
+            return PERMISSIONSType43.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType41(*args_, **kwargs_)
+            return PERMISSIONSType43(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -25946,40 +26277,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType41', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType41')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType43', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType43')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType41':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType43':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType41')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType43')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType41', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType43', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType41'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType43'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType41', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType43', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -26080,15 +26411,15 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType41
+# end class PERMISSIONSType43
 
 
 class MARKETPLACEAPPSType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
@@ -26187,15 +26518,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
 # end class MARKETPLACEAPPSType
 
 
-class PERMISSIONSType42(GeneratedsSuper):
+class PERMISSIONSType44(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -26218,21 +26549,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType42)
+                CurrentSubclassModule_, PERMISSIONSType44)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType42.subclass:
-            return PERMISSIONSType42.subclass(*args_, **kwargs_)
+        if PERMISSIONSType44.subclass:
+            return PERMISSIONSType44.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType42(*args_, **kwargs_)
+            return PERMISSIONSType44(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -26281,40 +26612,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType42', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType42')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType44', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType44')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType42':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType44':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType42')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType44')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType42', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType44', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType42'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType44'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType42', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType44', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -26415,18 +26746,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType42
+# end class PERMISSIONSType44
 
 
-class MONITORINGType43(GeneratedsSuper):
+class MONITORINGType45(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CPU=None, DISKRDBYTES=None, DISKRDIOPS=None, DISKWRBYTES=None, DISKWRIOPS=None, DISK_SIZE=None, ID=None, MEMORY=None, NETRX=None, NETTX=None, TIMESTAMP=None, VCENTER_ESX_HOST=None, VCENTER_GUEST_STATE=None, VCENTER_RP_NAME=None, VCENTER_VMWARETOOLS_RUNNING_STATUS=None, VCENTER_VMWARETOOLS_VERSION=None, VCENTER_VMWARETOOLS_VERSION_STATUS=None, VCENTER_VM_NAME=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -26470,21 +26801,21 @@
         self.VCENTER_VMWARETOOLS_VERSION_STATUS = VCENTER_VMWARETOOLS_VERSION_STATUS
         self.VCENTER_VMWARETOOLS_VERSION_STATUS_nsprefix_ = None
         self.VCENTER_VM_NAME = VCENTER_VM_NAME
         self.VCENTER_VM_NAME_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, MONITORINGType43)
+                CurrentSubclassModule_, MONITORINGType45)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if MONITORINGType43.subclass:
-            return MONITORINGType43.subclass(*args_, **kwargs_)
+        if MONITORINGType45.subclass:
+            return MONITORINGType45.subclass(*args_, **kwargs_)
         else:
-            return MONITORINGType43(*args_, **kwargs_)
+            return MONITORINGType45(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CPU(self):
         return self.CPU
@@ -26584,40 +26915,40 @@
             self.VCENTER_VMWARETOOLS_VERSION is not None or
             self.VCENTER_VMWARETOOLS_VERSION_STATUS is not None or
             self.VCENTER_VM_NAME is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType43', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('MONITORINGType43')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType45', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('MONITORINGType45')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'MONITORINGType43':
+        if self.original_tagname_ is not None and name_ == 'MONITORINGType45':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType43')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType45')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType43', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType45', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType43'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType45'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType43', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType45', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CPU is not None:
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -26806,15 +27137,15 @@
             self.VCENTER_VMWARETOOLS_VERSION_STATUS_nsprefix_ = child_.prefix
         elif nodeName_ == 'VCENTER_VM_NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_VM_NAME')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_VM_NAME')
             self.VCENTER_VM_NAME = value_
             self.VCENTER_VM_NAME_nsprefix_ = child_.prefix
-# end class MONITORINGType43
+# end class MONITORINGType45
 
 
 class DISK_SIZEType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, SIZE=None, gds_collector_=None, **kwargs_):
@@ -30305,15 +30636,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'START')
             ival_ = self.gds_validate_integer(ival_, node, 'START')
             self.START = ival_
             self.START_nsprefix_ = child_.prefix
 # end class VXLAN_IDSType
 
 
-class PERMISSIONSType44(GeneratedsSuper):
+class PERMISSIONSType46(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -30336,21 +30667,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType44)
+                CurrentSubclassModule_, PERMISSIONSType46)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType44.subclass:
-            return PERMISSIONSType44.subclass(*args_, **kwargs_)
+        if PERMISSIONSType46.subclass:
+            return PERMISSIONSType46.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType44(*args_, **kwargs_)
+            return PERMISSIONSType46(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -30399,40 +30730,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType44', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType44')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType46', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType46')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType44':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType46':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType44')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType46')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType44', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType46', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType44'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType46'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType44', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType46', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -30533,15 +30864,15 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType44
+# end class PERMISSIONSType46
 
 
 class UPDATED_VMSType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
@@ -30952,15 +31283,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
 # end class ERROR_VMSType
 
 
-class TEMPLATEType45(GeneratedsSuper):
+class TEMPLATEType47(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DESCRIPTION=None, RULE=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -30976,21 +31307,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType45)
+                CurrentSubclassModule_, TEMPLATEType47)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType45.subclass:
-            return TEMPLATEType45.subclass(*args_, **kwargs_)
+        if TEMPLATEType47.subclass:
+            return TEMPLATEType47.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType45(*args_, **kwargs_)
+            return TEMPLATEType47(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DESCRIPTION(self):
         return self.DESCRIPTION
@@ -31015,40 +31346,40 @@
             self.DESCRIPTION is not None or
             self.RULE or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType45', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType45')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType47', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType47')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType45':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType47':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType45')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType47')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType45', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType47', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType45'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType47'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType45', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType47', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.DESCRIPTION is not None:
             namespaceprefix_ = self.DESCRIPTION_nsprefix_ + ':' if (UseCapturedNS_ and self.DESCRIPTION_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -31083,17 +31414,17 @@
             self.DESCRIPTION_nsprefix_ = child_.prefix
         elif nodeName_ == 'RULE':
             obj_ = RULEType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.RULE.append(obj_)
             obj_.original_tagname_ = 'RULE'
         else:
-            content_ = self.gds_build_any(child_, 'TEMPLATEType45')
+            content_ = self.gds_build_any(child_, 'TEMPLATEType47')
             self.anytypeobjs_.append(content_)
-# end class TEMPLATEType45
+# end class TEMPLATEType47
 
 
 class RULEType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, PROTOCOL=None, RULE_TYPE=None, gds_collector_=None, **kwargs_):
@@ -32002,15 +32333,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'EGID')
             ival_ = self.gds_validate_integer(ival_, node, 'EGID')
             self.EGID = ival_
             self.EGID_nsprefix_ = child_.prefix
 # end class LOGIN_TOKENType
 
 
-class QUOTASType46(GeneratedsSuper):
+class QUOTASType48(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, DATASTORE_QUOTA=None, NETWORK_QUOTA=None, VM_QUOTA=None, IMAGE_QUOTA=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -32025,21 +32356,21 @@
         self.VM_QUOTA = VM_QUOTA
         self.VM_QUOTA_nsprefix_ = None
         self.IMAGE_QUOTA = IMAGE_QUOTA
         self.IMAGE_QUOTA_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, QUOTASType46)
+                CurrentSubclassModule_, QUOTASType48)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if QUOTASType46.subclass:
-            return QUOTASType46.subclass(*args_, **kwargs_)
+        if QUOTASType48.subclass:
+            return QUOTASType48.subclass(*args_, **kwargs_)
         else:
-            return QUOTASType46(*args_, **kwargs_)
+            return QUOTASType48(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -32068,40 +32399,40 @@
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='QUOTASType46', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('QUOTASType46')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='QUOTASType48', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('QUOTASType48')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'QUOTASType46':
+        if self.original_tagname_ is not None and name_ == 'QUOTASType48':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='QUOTASType46')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='QUOTASType48')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='QUOTASType46', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='QUOTASType48', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='QUOTASType46'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='QUOTASType48'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='QUOTASType46', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='QUOTASType48', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -32135,37 +32466,37 @@
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID = ival_
             self.ID_nsprefix_ = child_.prefix
         elif nodeName_ == 'DATASTORE_QUOTA':
-            obj_ = DATASTORE_QUOTAType47.factory(parent_object_=self)
+            obj_ = DATASTORE_QUOTAType49.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE_QUOTA = obj_
             obj_.original_tagname_ = 'DATASTORE_QUOTA'
         elif nodeName_ == 'NETWORK_QUOTA':
-            obj_ = NETWORK_QUOTAType49.factory(parent_object_=self)
+            obj_ = NETWORK_QUOTAType51.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK_QUOTA = obj_
             obj_.original_tagname_ = 'NETWORK_QUOTA'
         elif nodeName_ == 'VM_QUOTA':
-            obj_ = VM_QUOTAType51.factory(parent_object_=self)
+            obj_ = VM_QUOTAType53.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM_QUOTA = obj_
             obj_.original_tagname_ = 'VM_QUOTA'
         elif nodeName_ == 'IMAGE_QUOTA':
-            obj_ = IMAGE_QUOTAType53.factory(parent_object_=self)
+            obj_ = IMAGE_QUOTAType55.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE_QUOTA = obj_
             obj_.original_tagname_ = 'IMAGE_QUOTA'
-# end class QUOTASType46
+# end class QUOTASType48
 
 
-class DATASTORE_QUOTAType47(GeneratedsSuper):
+class DATASTORE_QUOTAType49(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DATASTORE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -32175,21 +32506,21 @@
             self.DATASTORE = []
         else:
             self.DATASTORE = DATASTORE
         self.DATASTORE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTORE_QUOTAType47)
+                CurrentSubclassModule_, DATASTORE_QUOTAType49)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTORE_QUOTAType47.subclass:
-            return DATASTORE_QUOTAType47.subclass(*args_, **kwargs_)
+        if DATASTORE_QUOTAType49.subclass:
+            return DATASTORE_QUOTAType49.subclass(*args_, **kwargs_)
         else:
-            return DATASTORE_QUOTAType47(*args_, **kwargs_)
+            return DATASTORE_QUOTAType49(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DATASTORE(self):
         return self.DATASTORE
@@ -32204,40 +32535,40 @@
     def _hasContent(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType47', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType47')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType49', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType49')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType47':
+        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType49':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType47')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType49')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType47', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType49', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType47'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType49'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType47', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType49', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for DATASTORE_ in self.DATASTORE:
             namespaceprefix_ = self.DATASTORE_nsprefix_ + ':' if (UseCapturedNS_ and self.DATASTORE_nsprefix_) else ''
             DATASTORE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='DATASTORE', pretty_print=pretty_print)
@@ -32252,22 +32583,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DATASTORE':
-            obj_ = DATASTOREType48.factory(parent_object_=self)
+            obj_ = DATASTOREType50.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE.append(obj_)
             obj_.original_tagname_ = 'DATASTORE'
-# end class DATASTORE_QUOTAType47
+# end class DATASTORE_QUOTAType49
 
 
-class DATASTOREType48(GeneratedsSuper):
+class DATASTOREType50(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -32282,21 +32613,21 @@
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
         self.SIZE_USED = SIZE_USED
         self.SIZE_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTOREType48)
+                CurrentSubclassModule_, DATASTOREType50)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTOREType48.subclass:
-            return DATASTOREType48.subclass(*args_, **kwargs_)
+        if DATASTOREType50.subclass:
+            return DATASTOREType50.subclass(*args_, **kwargs_)
         else:
-            return DATASTOREType48(*args_, **kwargs_)
+            return DATASTOREType50(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -32325,40 +32656,40 @@
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType48', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType48')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType50', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType50')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTOREType48':
+        if self.original_tagname_ is not None and name_ == 'DATASTOREType50':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType48')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType50')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType48', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType50', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType48'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType50'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType48', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType50', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -32419,18 +32750,18 @@
             self.SIZE_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'SIZE_USED')
             value_ = self.gds_validate_string(value_, node, 'SIZE_USED')
             self.SIZE_USED = value_
             self.SIZE_USED_nsprefix_ = child_.prefix
-# end class DATASTOREType48
+# end class DATASTOREType50
 
 
-class NETWORK_QUOTAType49(GeneratedsSuper):
+class NETWORK_QUOTAType51(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, NETWORK=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -32440,21 +32771,21 @@
             self.NETWORK = []
         else:
             self.NETWORK = NETWORK
         self.NETWORK_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORK_QUOTAType49)
+                CurrentSubclassModule_, NETWORK_QUOTAType51)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORK_QUOTAType49.subclass:
-            return NETWORK_QUOTAType49.subclass(*args_, **kwargs_)
+        if NETWORK_QUOTAType51.subclass:
+            return NETWORK_QUOTAType51.subclass(*args_, **kwargs_)
         else:
-            return NETWORK_QUOTAType49(*args_, **kwargs_)
+            return NETWORK_QUOTAType51(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_NETWORK(self):
         return self.NETWORK
@@ -32469,40 +32800,40 @@
     def _hasContent(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType49', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType49')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType51', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType51')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType49':
+        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType51':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType49')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType51')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType49', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType51', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType49'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType51'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType49', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType51', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for NETWORK_ in self.NETWORK:
             namespaceprefix_ = self.NETWORK_nsprefix_ + ':' if (UseCapturedNS_ and self.NETWORK_nsprefix_) else ''
             NETWORK_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='NETWORK', pretty_print=pretty_print)
@@ -32517,22 +32848,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'NETWORK':
-            obj_ = NETWORKType50.factory(parent_object_=self)
+            obj_ = NETWORKType52.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK.append(obj_)
             obj_.original_tagname_ = 'NETWORK'
-# end class NETWORK_QUOTAType49
+# end class NETWORK_QUOTAType51
 
 
-class NETWORKType50(GeneratedsSuper):
+class NETWORKType52(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -32543,21 +32874,21 @@
         self.LEASES = LEASES
         self.LEASES_nsprefix_ = None
         self.LEASES_USED = LEASES_USED
         self.LEASES_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORKType50)
+                CurrentSubclassModule_, NETWORKType52)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORKType50.subclass:
-            return NETWORKType50.subclass(*args_, **kwargs_)
+        if NETWORKType52.subclass:
+            return NETWORKType52.subclass(*args_, **kwargs_)
         else:
-            return NETWORKType50(*args_, **kwargs_)
+            return NETWORKType52(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -32576,40 +32907,40 @@
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType50', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType50')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType52', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType52')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORKType50':
+        if self.original_tagname_ is not None and name_ == 'NETWORKType52':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType50')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType52')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType50', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType52', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType50'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType52'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType50', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType52', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -32650,39 +32981,39 @@
             self.LEASES_nsprefix_ = child_.prefix
         elif nodeName_ == 'LEASES_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'LEASES_USED')
             value_ = self.gds_validate_string(value_, node, 'LEASES_USED')
             self.LEASES_USED = value_
             self.LEASES_USED_nsprefix_ = child_.prefix
-# end class NETWORKType50
+# end class NETWORKType52
 
 
-class VM_QUOTAType51(GeneratedsSuper):
+class VM_QUOTAType53(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VM=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.VM = VM
         self.VM_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VM_QUOTAType51)
+                CurrentSubclassModule_, VM_QUOTAType53)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VM_QUOTAType51.subclass:
-            return VM_QUOTAType51.subclass(*args_, **kwargs_)
+        if VM_QUOTAType53.subclass:
+            return VM_QUOTAType53.subclass(*args_, **kwargs_)
         else:
-            return VM_QUOTAType51(*args_, **kwargs_)
+            return VM_QUOTAType53(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
@@ -32691,40 +33022,40 @@
     def _hasContent(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType51', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType51')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType53', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType53')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType51':
+        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType53':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType51')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType53')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType51', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType53', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType51'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType53'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType51', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType53', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VM is not None:
             namespaceprefix_ = self.VM_nsprefix_ + ':' if (UseCapturedNS_ and self.VM_nsprefix_) else ''
             self.VM.export(outfile, level, namespaceprefix_, namespacedef_='', name_='VM', pretty_print=pretty_print)
@@ -32739,22 +33070,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'VM':
-            obj_ = VMType52.factory(parent_object_=self)
+            obj_ = VMType54.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM = obj_
             obj_.original_tagname_ = 'VM'
-# end class VM_QUOTAType51
+# end class VM_QUOTAType53
 
 
-class VMType52(GeneratedsSuper):
+class VMType54(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -32787,21 +33118,21 @@
         self.VMS = VMS
         self.VMS_nsprefix_ = None
         self.VMS_USED = VMS_USED
         self.VMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VMType52)
+                CurrentSubclassModule_, VMType54)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VMType52.subclass:
-            return VMType52.subclass(*args_, **kwargs_)
+        if VMType54.subclass:
+            return VMType54.subclass(*args_, **kwargs_)
         else:
-            return VMType52(*args_, **kwargs_)
+            return VMType54(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CPU(self):
         return self.CPU
@@ -32875,40 +33206,40 @@
             self.SYSTEM_DISK_SIZE_USED is not None or
             self.VMS is not None or
             self.VMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType52', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType52')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType54', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType54')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VMType52':
+        if self.original_tagname_ is not None and name_ == 'VMType54':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType52')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType54')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType52', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType54', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType52'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType54'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType52', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType54', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CPU is not None:
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -33059,18 +33390,18 @@
             self.VMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'VMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VMS_USED')
             value_ = self.gds_validate_string(value_, node, 'VMS_USED')
             self.VMS_USED = value_
             self.VMS_USED_nsprefix_ = child_.prefix
-# end class VMType52
+# end class VMType54
 
 
-class IMAGE_QUOTAType53(GeneratedsSuper):
+class IMAGE_QUOTAType55(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, IMAGE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -33080,21 +33411,21 @@
             self.IMAGE = []
         else:
             self.IMAGE = IMAGE
         self.IMAGE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGE_QUOTAType53)
+                CurrentSubclassModule_, IMAGE_QUOTAType55)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGE_QUOTAType53.subclass:
-            return IMAGE_QUOTAType53.subclass(*args_, **kwargs_)
+        if IMAGE_QUOTAType55.subclass:
+            return IMAGE_QUOTAType55.subclass(*args_, **kwargs_)
         else:
-            return IMAGE_QUOTAType53(*args_, **kwargs_)
+            return IMAGE_QUOTAType55(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_IMAGE(self):
         return self.IMAGE
@@ -33109,40 +33440,40 @@
     def _hasContent(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType53', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType53')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType55', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType55')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType53':
+        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType55':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType53')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType55')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType53', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType55', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType53'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType55'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType53', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType55', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for IMAGE_ in self.IMAGE:
             namespaceprefix_ = self.IMAGE_nsprefix_ + ':' if (UseCapturedNS_ and self.IMAGE_nsprefix_) else ''
             IMAGE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='IMAGE', pretty_print=pretty_print)
@@ -33157,22 +33488,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'IMAGE':
-            obj_ = IMAGEType54.factory(parent_object_=self)
+            obj_ = IMAGEType56.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE.append(obj_)
             obj_.original_tagname_ = 'IMAGE'
-# end class IMAGE_QUOTAType53
+# end class IMAGE_QUOTAType55
 
 
-class IMAGEType54(GeneratedsSuper):
+class IMAGEType56(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -33183,21 +33514,21 @@
         self.RVMS = RVMS
         self.RVMS_nsprefix_ = None
         self.RVMS_USED = RVMS_USED
         self.RVMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGEType54)
+                CurrentSubclassModule_, IMAGEType56)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGEType54.subclass:
-            return IMAGEType54.subclass(*args_, **kwargs_)
+        if IMAGEType56.subclass:
+            return IMAGEType56.subclass(*args_, **kwargs_)
         else:
-            return IMAGEType54(*args_, **kwargs_)
+            return IMAGEType56(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -33216,40 +33547,40 @@
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType54', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType54')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType56', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType56')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGEType54':
+        if self.original_tagname_ is not None and name_ == 'IMAGEType56':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType54')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType56')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType54', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType56', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType54'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType56'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType54', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType56', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -33290,15 +33621,15 @@
             self.RVMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'RVMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'RVMS_USED')
             value_ = self.gds_validate_string(value_, node, 'RVMS_USED')
             self.RVMS_USED = value_
             self.RVMS_USED_nsprefix_ = child_.prefix
-# end class IMAGEType54
+# end class IMAGEType56
 
 
 class DEFAULT_USER_QUOTASType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DATASTORE_QUOTA=None, NETWORK_QUOTA=None, VM_QUOTA=None, IMAGE_QUOTA=None, gds_collector_=None, **kwargs_):
@@ -33409,37 +33740,37 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DATASTORE_QUOTA':
-            obj_ = DATASTORE_QUOTAType55.factory(parent_object_=self)
+            obj_ = DATASTORE_QUOTAType57.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE_QUOTA = obj_
             obj_.original_tagname_ = 'DATASTORE_QUOTA'
         elif nodeName_ == 'NETWORK_QUOTA':
-            obj_ = NETWORK_QUOTAType57.factory(parent_object_=self)
+            obj_ = NETWORK_QUOTAType59.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK_QUOTA = obj_
             obj_.original_tagname_ = 'NETWORK_QUOTA'
         elif nodeName_ == 'VM_QUOTA':
-            obj_ = VM_QUOTAType59.factory(parent_object_=self)
+            obj_ = VM_QUOTAType61.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM_QUOTA = obj_
             obj_.original_tagname_ = 'VM_QUOTA'
         elif nodeName_ == 'IMAGE_QUOTA':
-            obj_ = IMAGE_QUOTAType61.factory(parent_object_=self)
+            obj_ = IMAGE_QUOTAType63.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE_QUOTA = obj_
             obj_.original_tagname_ = 'IMAGE_QUOTA'
 # end class DEFAULT_USER_QUOTASType
 
 
-class DATASTORE_QUOTAType55(GeneratedsSuper):
+class DATASTORE_QUOTAType57(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DATASTORE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -33449,21 +33780,21 @@
             self.DATASTORE = []
         else:
             self.DATASTORE = DATASTORE
         self.DATASTORE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTORE_QUOTAType55)
+                CurrentSubclassModule_, DATASTORE_QUOTAType57)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTORE_QUOTAType55.subclass:
-            return DATASTORE_QUOTAType55.subclass(*args_, **kwargs_)
+        if DATASTORE_QUOTAType57.subclass:
+            return DATASTORE_QUOTAType57.subclass(*args_, **kwargs_)
         else:
-            return DATASTORE_QUOTAType55(*args_, **kwargs_)
+            return DATASTORE_QUOTAType57(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DATASTORE(self):
         return self.DATASTORE
@@ -33478,40 +33809,40 @@
     def _hasContent(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType55', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType55')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType57', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType57')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType55':
+        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType57':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType55')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType57')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType55', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType57', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType55'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType57'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType55', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType57', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for DATASTORE_ in self.DATASTORE:
             namespaceprefix_ = self.DATASTORE_nsprefix_ + ':' if (UseCapturedNS_ and self.DATASTORE_nsprefix_) else ''
             DATASTORE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='DATASTORE', pretty_print=pretty_print)
@@ -33526,22 +33857,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DATASTORE':
-            obj_ = DATASTOREType56.factory(parent_object_=self)
+            obj_ = DATASTOREType58.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE.append(obj_)
             obj_.original_tagname_ = 'DATASTORE'
-# end class DATASTORE_QUOTAType55
+# end class DATASTORE_QUOTAType57
 
 
-class DATASTOREType56(GeneratedsSuper):
+class DATASTOREType58(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -33556,21 +33887,21 @@
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
         self.SIZE_USED = SIZE_USED
         self.SIZE_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTOREType56)
+                CurrentSubclassModule_, DATASTOREType58)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTOREType56.subclass:
-            return DATASTOREType56.subclass(*args_, **kwargs_)
+        if DATASTOREType58.subclass:
+            return DATASTOREType58.subclass(*args_, **kwargs_)
         else:
-            return DATASTOREType56(*args_, **kwargs_)
+            return DATASTOREType58(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -33599,40 +33930,40 @@
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType56', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType56')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType58', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType58')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTOREType56':
+        if self.original_tagname_ is not None and name_ == 'DATASTOREType58':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType56')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType58')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType56', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType58', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType56'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType58'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType56', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType58', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -33693,18 +34024,18 @@
             self.SIZE_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'SIZE_USED')
             value_ = self.gds_validate_string(value_, node, 'SIZE_USED')
             self.SIZE_USED = value_
             self.SIZE_USED_nsprefix_ = child_.prefix
-# end class DATASTOREType56
+# end class DATASTOREType58
 
 
-class NETWORK_QUOTAType57(GeneratedsSuper):
+class NETWORK_QUOTAType59(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, NETWORK=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -33714,21 +34045,21 @@
             self.NETWORK = []
         else:
             self.NETWORK = NETWORK
         self.NETWORK_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORK_QUOTAType57)
+                CurrentSubclassModule_, NETWORK_QUOTAType59)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORK_QUOTAType57.subclass:
-            return NETWORK_QUOTAType57.subclass(*args_, **kwargs_)
+        if NETWORK_QUOTAType59.subclass:
+            return NETWORK_QUOTAType59.subclass(*args_, **kwargs_)
         else:
-            return NETWORK_QUOTAType57(*args_, **kwargs_)
+            return NETWORK_QUOTAType59(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_NETWORK(self):
         return self.NETWORK
@@ -33743,40 +34074,40 @@
     def _hasContent(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType57', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType57')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType59', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType59')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType57':
+        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType59':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType57')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType59')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType57', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType59', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType57'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType59'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType57', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType59', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for NETWORK_ in self.NETWORK:
             namespaceprefix_ = self.NETWORK_nsprefix_ + ':' if (UseCapturedNS_ and self.NETWORK_nsprefix_) else ''
             NETWORK_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='NETWORK', pretty_print=pretty_print)
@@ -33791,22 +34122,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'NETWORK':
-            obj_ = NETWORKType58.factory(parent_object_=self)
+            obj_ = NETWORKType60.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK.append(obj_)
             obj_.original_tagname_ = 'NETWORK'
-# end class NETWORK_QUOTAType57
+# end class NETWORK_QUOTAType59
 
 
-class NETWORKType58(GeneratedsSuper):
+class NETWORKType60(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -33817,21 +34148,21 @@
         self.LEASES = LEASES
         self.LEASES_nsprefix_ = None
         self.LEASES_USED = LEASES_USED
         self.LEASES_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORKType58)
+                CurrentSubclassModule_, NETWORKType60)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORKType58.subclass:
-            return NETWORKType58.subclass(*args_, **kwargs_)
+        if NETWORKType60.subclass:
+            return NETWORKType60.subclass(*args_, **kwargs_)
         else:
-            return NETWORKType58(*args_, **kwargs_)
+            return NETWORKType60(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -33850,40 +34181,40 @@
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType58', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType58')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType60', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType60')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORKType58':
+        if self.original_tagname_ is not None and name_ == 'NETWORKType60':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType58')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType60')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType58', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType60', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType58'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType60'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType58', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType60', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -33924,39 +34255,39 @@
             self.LEASES_nsprefix_ = child_.prefix
         elif nodeName_ == 'LEASES_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'LEASES_USED')
             value_ = self.gds_validate_string(value_, node, 'LEASES_USED')
             self.LEASES_USED = value_
             self.LEASES_USED_nsprefix_ = child_.prefix
-# end class NETWORKType58
+# end class NETWORKType60
 
 
-class VM_QUOTAType59(GeneratedsSuper):
+class VM_QUOTAType61(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VM=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.VM = VM
         self.VM_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VM_QUOTAType59)
+                CurrentSubclassModule_, VM_QUOTAType61)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VM_QUOTAType59.subclass:
-            return VM_QUOTAType59.subclass(*args_, **kwargs_)
+        if VM_QUOTAType61.subclass:
+            return VM_QUOTAType61.subclass(*args_, **kwargs_)
         else:
-            return VM_QUOTAType59(*args_, **kwargs_)
+            return VM_QUOTAType61(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
@@ -33965,40 +34296,40 @@
     def _hasContent(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType59', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType59')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType61', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType61')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType59':
+        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType61':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType59')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType61')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType59', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType61', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType59'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType61'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType59', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType61', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VM is not None:
             namespaceprefix_ = self.VM_nsprefix_ + ':' if (UseCapturedNS_ and self.VM_nsprefix_) else ''
             self.VM.export(outfile, level, namespaceprefix_, namespacedef_='', name_='VM', pretty_print=pretty_print)
@@ -34013,22 +34344,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'VM':
-            obj_ = VMType60.factory(parent_object_=self)
+            obj_ = VMType62.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM = obj_
             obj_.original_tagname_ = 'VM'
-# end class VM_QUOTAType59
+# end class VM_QUOTAType61
 
 
-class VMType60(GeneratedsSuper):
+class VMType62(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -34061,21 +34392,21 @@
         self.VMS = VMS
         self.VMS_nsprefix_ = None
         self.VMS_USED = VMS_USED
         self.VMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VMType60)
+                CurrentSubclassModule_, VMType62)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VMType60.subclass:
-            return VMType60.subclass(*args_, **kwargs_)
+        if VMType62.subclass:
+            return VMType62.subclass(*args_, **kwargs_)
         else:
-            return VMType60(*args_, **kwargs_)
+            return VMType62(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CPU(self):
         return self.CPU
@@ -34149,40 +34480,40 @@
             self.SYSTEM_DISK_SIZE_USED is not None or
             self.VMS is not None or
             self.VMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType60', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType60')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType62', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType62')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VMType60':
+        if self.original_tagname_ is not None and name_ == 'VMType62':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType60')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType62')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType60', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType62', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType60'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType62'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType60', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType62', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CPU is not None:
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -34333,18 +34664,18 @@
             self.VMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'VMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VMS_USED')
             value_ = self.gds_validate_string(value_, node, 'VMS_USED')
             self.VMS_USED = value_
             self.VMS_USED_nsprefix_ = child_.prefix
-# end class VMType60
+# end class VMType62
 
 
-class IMAGE_QUOTAType61(GeneratedsSuper):
+class IMAGE_QUOTAType63(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, IMAGE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -34354,21 +34685,21 @@
             self.IMAGE = []
         else:
             self.IMAGE = IMAGE
         self.IMAGE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGE_QUOTAType61)
+                CurrentSubclassModule_, IMAGE_QUOTAType63)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGE_QUOTAType61.subclass:
-            return IMAGE_QUOTAType61.subclass(*args_, **kwargs_)
+        if IMAGE_QUOTAType63.subclass:
+            return IMAGE_QUOTAType63.subclass(*args_, **kwargs_)
         else:
-            return IMAGE_QUOTAType61(*args_, **kwargs_)
+            return IMAGE_QUOTAType63(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_IMAGE(self):
         return self.IMAGE
@@ -34383,40 +34714,40 @@
     def _hasContent(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType61', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType61')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType63', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType63')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType61':
+        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType63':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType61')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType63')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType61', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType63', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType61'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType63'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType61', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType63', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for IMAGE_ in self.IMAGE:
             namespaceprefix_ = self.IMAGE_nsprefix_ + ':' if (UseCapturedNS_ and self.IMAGE_nsprefix_) else ''
             IMAGE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='IMAGE', pretty_print=pretty_print)
@@ -34431,22 +34762,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'IMAGE':
-            obj_ = IMAGEType62.factory(parent_object_=self)
+            obj_ = IMAGEType64.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE.append(obj_)
             obj_.original_tagname_ = 'IMAGE'
-# end class IMAGE_QUOTAType61
+# end class IMAGE_QUOTAType63
 
 
-class IMAGEType62(GeneratedsSuper):
+class IMAGEType64(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -34457,21 +34788,21 @@
         self.RVMS = RVMS
         self.RVMS_nsprefix_ = None
         self.RVMS_USED = RVMS_USED
         self.RVMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGEType62)
+                CurrentSubclassModule_, IMAGEType64)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGEType62.subclass:
-            return IMAGEType62.subclass(*args_, **kwargs_)
+        if IMAGEType64.subclass:
+            return IMAGEType64.subclass(*args_, **kwargs_)
         else:
-            return IMAGEType62(*args_, **kwargs_)
+            return IMAGEType64(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -34490,40 +34821,40 @@
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType62', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType62')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType64', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType64')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGEType62':
+        if self.original_tagname_ is not None and name_ == 'IMAGEType64':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType62')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType64')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType62', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType64', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType62'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType64'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType62', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType64', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -34564,18 +34895,18 @@
             self.RVMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'RVMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'RVMS_USED')
             value_ = self.gds_validate_string(value_, node, 'RVMS_USED')
             self.RVMS_USED = value_
             self.RVMS_USED_nsprefix_ = child_.prefix
-# end class IMAGEType62
+# end class IMAGEType64
 
 
-class GROUPSType63(GeneratedsSuper):
+class GROUPSType65(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -34585,21 +34916,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, GROUPSType63)
+                CurrentSubclassModule_, GROUPSType65)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if GROUPSType63.subclass:
-            return GROUPSType63.subclass(*args_, **kwargs_)
+        if GROUPSType65.subclass:
+            return GROUPSType65.subclass(*args_, **kwargs_)
         else:
-            return GROUPSType63(*args_, **kwargs_)
+            return GROUPSType65(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -34614,40 +34945,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType63', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('GROUPSType63')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType65', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('GROUPSType65')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'GROUPSType63':
+        if self.original_tagname_ is not None and name_ == 'GROUPSType65':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPSType63')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPSType65')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPSType63', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPSType65', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPSType63'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPSType65'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType63', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType65', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -34668,18 +34999,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class GROUPSType63
+# end class GROUPSType65
 
 
-class LOGIN_TOKENType64(GeneratedsSuper):
+class LOGIN_TOKENType66(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, TOKEN=None, EXPIRATION_TIME=None, EGID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -34690,21 +35021,21 @@
         self.EXPIRATION_TIME = EXPIRATION_TIME
         self.EXPIRATION_TIME_nsprefix_ = None
         self.EGID = EGID
         self.EGID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOGIN_TOKENType64)
+                CurrentSubclassModule_, LOGIN_TOKENType66)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOGIN_TOKENType64.subclass:
-            return LOGIN_TOKENType64.subclass(*args_, **kwargs_)
+        if LOGIN_TOKENType66.subclass:
+            return LOGIN_TOKENType66.subclass(*args_, **kwargs_)
         else:
-            return LOGIN_TOKENType64(*args_, **kwargs_)
+            return LOGIN_TOKENType66(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_TOKEN(self):
         return self.TOKEN
@@ -34723,40 +35054,40 @@
             self.TOKEN is not None or
             self.EXPIRATION_TIME is not None or
             self.EGID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOGIN_TOKENType64', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOGIN_TOKENType64')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOGIN_TOKENType66', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOGIN_TOKENType66')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOGIN_TOKENType64':
+        if self.original_tagname_ is not None and name_ == 'LOGIN_TOKENType66':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOGIN_TOKENType64')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOGIN_TOKENType66')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOGIN_TOKENType64', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOGIN_TOKENType66', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOGIN_TOKENType64'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOGIN_TOKENType66'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOGIN_TOKENType64', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOGIN_TOKENType66', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.TOKEN is not None:
             namespaceprefix_ = self.TOKEN_nsprefix_ + ':' if (UseCapturedNS_ and self.TOKEN_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -34797,18 +35128,18 @@
             self.EXPIRATION_TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'EGID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'EGID')
             ival_ = self.gds_validate_integer(ival_, node, 'EGID')
             self.EGID = ival_
             self.EGID_nsprefix_ = child_.prefix
-# end class LOGIN_TOKENType64
+# end class LOGIN_TOKENType66
 
 
-class DATASTORE_QUOTAType65(GeneratedsSuper):
+class DATASTORE_QUOTAType67(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DATASTORE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -34818,21 +35149,21 @@
             self.DATASTORE = []
         else:
             self.DATASTORE = DATASTORE
         self.DATASTORE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTORE_QUOTAType65)
+                CurrentSubclassModule_, DATASTORE_QUOTAType67)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTORE_QUOTAType65.subclass:
-            return DATASTORE_QUOTAType65.subclass(*args_, **kwargs_)
+        if DATASTORE_QUOTAType67.subclass:
+            return DATASTORE_QUOTAType67.subclass(*args_, **kwargs_)
         else:
-            return DATASTORE_QUOTAType65(*args_, **kwargs_)
+            return DATASTORE_QUOTAType67(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DATASTORE(self):
         return self.DATASTORE
@@ -34847,40 +35178,40 @@
     def _hasContent(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType65', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType65')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType67', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType67')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType65':
+        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType67':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType65')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType67')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType65', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType67', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType65'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType67'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType65', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType67', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for DATASTORE_ in self.DATASTORE:
             namespaceprefix_ = self.DATASTORE_nsprefix_ + ':' if (UseCapturedNS_ and self.DATASTORE_nsprefix_) else ''
             DATASTORE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='DATASTORE', pretty_print=pretty_print)
@@ -34895,22 +35226,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DATASTORE':
-            obj_ = DATASTOREType66.factory(parent_object_=self)
+            obj_ = DATASTOREType68.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE.append(obj_)
             obj_.original_tagname_ = 'DATASTORE'
-# end class DATASTORE_QUOTAType65
+# end class DATASTORE_QUOTAType67
 
 
-class DATASTOREType66(GeneratedsSuper):
+class DATASTOREType68(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -34925,21 +35256,21 @@
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
         self.SIZE_USED = SIZE_USED
         self.SIZE_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTOREType66)
+                CurrentSubclassModule_, DATASTOREType68)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTOREType66.subclass:
-            return DATASTOREType66.subclass(*args_, **kwargs_)
+        if DATASTOREType68.subclass:
+            return DATASTOREType68.subclass(*args_, **kwargs_)
         else:
-            return DATASTOREType66(*args_, **kwargs_)
+            return DATASTOREType68(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -34968,40 +35299,40 @@
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType66', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType66')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType68', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType68')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTOREType66':
+        if self.original_tagname_ is not None and name_ == 'DATASTOREType68':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType66')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType68')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType66', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType68', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType66'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType68'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType66', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType68', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -35062,18 +35393,18 @@
             self.SIZE_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'SIZE_USED')
             value_ = self.gds_validate_string(value_, node, 'SIZE_USED')
             self.SIZE_USED = value_
             self.SIZE_USED_nsprefix_ = child_.prefix
-# end class DATASTOREType66
+# end class DATASTOREType68
 
 
-class NETWORK_QUOTAType67(GeneratedsSuper):
+class NETWORK_QUOTAType69(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, NETWORK=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -35083,21 +35414,21 @@
             self.NETWORK = []
         else:
             self.NETWORK = NETWORK
         self.NETWORK_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORK_QUOTAType67)
+                CurrentSubclassModule_, NETWORK_QUOTAType69)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORK_QUOTAType67.subclass:
-            return NETWORK_QUOTAType67.subclass(*args_, **kwargs_)
+        if NETWORK_QUOTAType69.subclass:
+            return NETWORK_QUOTAType69.subclass(*args_, **kwargs_)
         else:
-            return NETWORK_QUOTAType67(*args_, **kwargs_)
+            return NETWORK_QUOTAType69(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_NETWORK(self):
         return self.NETWORK
@@ -35112,40 +35443,40 @@
     def _hasContent(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType67', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType67')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType69', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType69')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType67':
+        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType69':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType67')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType69')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType67', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType69', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType67'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType69'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType67', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType69', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for NETWORK_ in self.NETWORK:
             namespaceprefix_ = self.NETWORK_nsprefix_ + ':' if (UseCapturedNS_ and self.NETWORK_nsprefix_) else ''
             NETWORK_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='NETWORK', pretty_print=pretty_print)
@@ -35160,22 +35491,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'NETWORK':
-            obj_ = NETWORKType68.factory(parent_object_=self)
+            obj_ = NETWORKType70.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK.append(obj_)
             obj_.original_tagname_ = 'NETWORK'
-# end class NETWORK_QUOTAType67
+# end class NETWORK_QUOTAType69
 
 
-class NETWORKType68(GeneratedsSuper):
+class NETWORKType70(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -35186,21 +35517,21 @@
         self.LEASES = LEASES
         self.LEASES_nsprefix_ = None
         self.LEASES_USED = LEASES_USED
         self.LEASES_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORKType68)
+                CurrentSubclassModule_, NETWORKType70)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORKType68.subclass:
-            return NETWORKType68.subclass(*args_, **kwargs_)
+        if NETWORKType70.subclass:
+            return NETWORKType70.subclass(*args_, **kwargs_)
         else:
-            return NETWORKType68(*args_, **kwargs_)
+            return NETWORKType70(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -35219,40 +35550,40 @@
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType68', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType68')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType70', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType70')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORKType68':
+        if self.original_tagname_ is not None and name_ == 'NETWORKType70':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType68')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType70')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType68', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType70', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType68'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType70'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType68', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType70', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -35293,39 +35624,39 @@
             self.LEASES_nsprefix_ = child_.prefix
         elif nodeName_ == 'LEASES_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'LEASES_USED')
             value_ = self.gds_validate_string(value_, node, 'LEASES_USED')
             self.LEASES_USED = value_
             self.LEASES_USED_nsprefix_ = child_.prefix
-# end class NETWORKType68
+# end class NETWORKType70
 
 
-class VM_QUOTAType69(GeneratedsSuper):
+class VM_QUOTAType71(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VM=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.VM = VM
         self.VM_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VM_QUOTAType69)
+                CurrentSubclassModule_, VM_QUOTAType71)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VM_QUOTAType69.subclass:
-            return VM_QUOTAType69.subclass(*args_, **kwargs_)
+        if VM_QUOTAType71.subclass:
+            return VM_QUOTAType71.subclass(*args_, **kwargs_)
         else:
-            return VM_QUOTAType69(*args_, **kwargs_)
+            return VM_QUOTAType71(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
@@ -35334,40 +35665,40 @@
     def _hasContent(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType69', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType69')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType71', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType71')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType69':
+        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType71':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType69')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType71')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType69', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType71', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType69'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType71'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType69', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType71', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VM is not None:
             namespaceprefix_ = self.VM_nsprefix_ + ':' if (UseCapturedNS_ and self.VM_nsprefix_) else ''
             self.VM.export(outfile, level, namespaceprefix_, namespacedef_='', name_='VM', pretty_print=pretty_print)
@@ -35382,22 +35713,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'VM':
-            obj_ = VMType70.factory(parent_object_=self)
+            obj_ = VMType72.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM = obj_
             obj_.original_tagname_ = 'VM'
-# end class VM_QUOTAType69
+# end class VM_QUOTAType71
 
 
-class VMType70(GeneratedsSuper):
+class VMType72(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -35430,21 +35761,21 @@
         self.VMS = VMS
         self.VMS_nsprefix_ = None
         self.VMS_USED = VMS_USED
         self.VMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VMType70)
+                CurrentSubclassModule_, VMType72)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VMType70.subclass:
-            return VMType70.subclass(*args_, **kwargs_)
+        if VMType72.subclass:
+            return VMType72.subclass(*args_, **kwargs_)
         else:
-            return VMType70(*args_, **kwargs_)
+            return VMType72(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CPU(self):
         return self.CPU
@@ -35518,40 +35849,40 @@
             self.SYSTEM_DISK_SIZE_USED is not None or
             self.VMS is not None or
             self.VMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType70', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType70')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType72', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType72')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VMType70':
+        if self.original_tagname_ is not None and name_ == 'VMType72':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType70')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType72')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType70', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType72', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType70'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType72'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType70', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType72', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CPU is not None:
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -35702,18 +36033,18 @@
             self.VMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'VMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VMS_USED')
             value_ = self.gds_validate_string(value_, node, 'VMS_USED')
             self.VMS_USED = value_
             self.VMS_USED_nsprefix_ = child_.prefix
-# end class VMType70
+# end class VMType72
 
 
-class IMAGE_QUOTAType71(GeneratedsSuper):
+class IMAGE_QUOTAType73(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, IMAGE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -35723,21 +36054,21 @@
             self.IMAGE = []
         else:
             self.IMAGE = IMAGE
         self.IMAGE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGE_QUOTAType71)
+                CurrentSubclassModule_, IMAGE_QUOTAType73)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGE_QUOTAType71.subclass:
-            return IMAGE_QUOTAType71.subclass(*args_, **kwargs_)
+        if IMAGE_QUOTAType73.subclass:
+            return IMAGE_QUOTAType73.subclass(*args_, **kwargs_)
         else:
-            return IMAGE_QUOTAType71(*args_, **kwargs_)
+            return IMAGE_QUOTAType73(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_IMAGE(self):
         return self.IMAGE
@@ -35752,40 +36083,40 @@
     def _hasContent(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType71', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType71')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType73', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType73')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType71':
+        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType73':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType71')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType73')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType71', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType73', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType71'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType73'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType71', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType73', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for IMAGE_ in self.IMAGE:
             namespaceprefix_ = self.IMAGE_nsprefix_ + ':' if (UseCapturedNS_ and self.IMAGE_nsprefix_) else ''
             IMAGE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='IMAGE', pretty_print=pretty_print)
@@ -35800,22 +36131,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'IMAGE':
-            obj_ = IMAGEType72.factory(parent_object_=self)
+            obj_ = IMAGEType74.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE.append(obj_)
             obj_.original_tagname_ = 'IMAGE'
-# end class IMAGE_QUOTAType71
+# end class IMAGE_QUOTAType73
 
 
-class IMAGEType72(GeneratedsSuper):
+class IMAGEType74(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -35826,21 +36157,21 @@
         self.RVMS = RVMS
         self.RVMS_nsprefix_ = None
         self.RVMS_USED = RVMS_USED
         self.RVMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGEType72)
+                CurrentSubclassModule_, IMAGEType74)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGEType72.subclass:
-            return IMAGEType72.subclass(*args_, **kwargs_)
+        if IMAGEType74.subclass:
+            return IMAGEType74.subclass(*args_, **kwargs_)
         else:
-            return IMAGEType72(*args_, **kwargs_)
+            return IMAGEType74(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -35859,40 +36190,40 @@
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType72', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType72')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType74', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType74')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGEType72':
+        if self.original_tagname_ is not None and name_ == 'IMAGEType74':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType72')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType74')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType72', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType74', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType72'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType74'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType72', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType74', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -35933,18 +36264,18 @@
             self.RVMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'RVMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'RVMS_USED')
             value_ = self.gds_validate_string(value_, node, 'RVMS_USED')
             self.RVMS_USED = value_
             self.RVMS_USED_nsprefix_ = child_.prefix
-# end class IMAGEType72
+# end class IMAGEType74
 
 
-class DEFAULT_USER_QUOTASType73(GeneratedsSuper):
+class DEFAULT_USER_QUOTASType75(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DATASTORE_QUOTA=None, NETWORK_QUOTA=None, VM_QUOTA=None, IMAGE_QUOTA=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -35957,21 +36288,21 @@
         self.VM_QUOTA = VM_QUOTA
         self.VM_QUOTA_nsprefix_ = None
         self.IMAGE_QUOTA = IMAGE_QUOTA
         self.IMAGE_QUOTA_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DEFAULT_USER_QUOTASType73)
+                CurrentSubclassModule_, DEFAULT_USER_QUOTASType75)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DEFAULT_USER_QUOTASType73.subclass:
-            return DEFAULT_USER_QUOTASType73.subclass(*args_, **kwargs_)
+        if DEFAULT_USER_QUOTASType75.subclass:
+            return DEFAULT_USER_QUOTASType75.subclass(*args_, **kwargs_)
         else:
-            return DEFAULT_USER_QUOTASType73(*args_, **kwargs_)
+            return DEFAULT_USER_QUOTASType75(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DATASTORE_QUOTA(self):
         return self.DATASTORE_QUOTA
@@ -35995,40 +36326,40 @@
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DEFAULT_USER_QUOTASType73', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DEFAULT_USER_QUOTASType73')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DEFAULT_USER_QUOTASType75', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DEFAULT_USER_QUOTASType75')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DEFAULT_USER_QUOTASType73':
+        if self.original_tagname_ is not None and name_ == 'DEFAULT_USER_QUOTASType75':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DEFAULT_USER_QUOTASType73')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DEFAULT_USER_QUOTASType75')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DEFAULT_USER_QUOTASType73', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DEFAULT_USER_QUOTASType75', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DEFAULT_USER_QUOTASType73'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DEFAULT_USER_QUOTASType75'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DEFAULT_USER_QUOTASType73', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DEFAULT_USER_QUOTASType75', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.DATASTORE_QUOTA is not None:
             namespaceprefix_ = self.DATASTORE_QUOTA_nsprefix_ + ':' if (UseCapturedNS_ and self.DATASTORE_QUOTA_nsprefix_) else ''
             self.DATASTORE_QUOTA.export(outfile, level, namespaceprefix_, namespacedef_='', name_='DATASTORE_QUOTA', pretty_print=pretty_print)
@@ -36052,37 +36383,37 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DATASTORE_QUOTA':
-            obj_ = DATASTORE_QUOTAType74.factory(parent_object_=self)
+            obj_ = DATASTORE_QUOTAType76.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE_QUOTA = obj_
             obj_.original_tagname_ = 'DATASTORE_QUOTA'
         elif nodeName_ == 'NETWORK_QUOTA':
-            obj_ = NETWORK_QUOTAType76.factory(parent_object_=self)
+            obj_ = NETWORK_QUOTAType78.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK_QUOTA = obj_
             obj_.original_tagname_ = 'NETWORK_QUOTA'
         elif nodeName_ == 'VM_QUOTA':
-            obj_ = VM_QUOTAType78.factory(parent_object_=self)
+            obj_ = VM_QUOTAType80.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM_QUOTA = obj_
             obj_.original_tagname_ = 'VM_QUOTA'
         elif nodeName_ == 'IMAGE_QUOTA':
-            obj_ = IMAGE_QUOTAType80.factory(parent_object_=self)
+            obj_ = IMAGE_QUOTAType82.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE_QUOTA = obj_
             obj_.original_tagname_ = 'IMAGE_QUOTA'
-# end class DEFAULT_USER_QUOTASType73
+# end class DEFAULT_USER_QUOTASType75
 
 
-class DATASTORE_QUOTAType74(GeneratedsSuper):
+class DATASTORE_QUOTAType76(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DATASTORE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36092,21 +36423,21 @@
             self.DATASTORE = []
         else:
             self.DATASTORE = DATASTORE
         self.DATASTORE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTORE_QUOTAType74)
+                CurrentSubclassModule_, DATASTORE_QUOTAType76)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTORE_QUOTAType74.subclass:
-            return DATASTORE_QUOTAType74.subclass(*args_, **kwargs_)
+        if DATASTORE_QUOTAType76.subclass:
+            return DATASTORE_QUOTAType76.subclass(*args_, **kwargs_)
         else:
-            return DATASTORE_QUOTAType74(*args_, **kwargs_)
+            return DATASTORE_QUOTAType76(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DATASTORE(self):
         return self.DATASTORE
@@ -36121,40 +36452,40 @@
     def _hasContent(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType74', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType74')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType76', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORE_QUOTAType76')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType74':
+        if self.original_tagname_ is not None and name_ == 'DATASTORE_QUOTAType76':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType74')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType76')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType74', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType76', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType74'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType76'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType74', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType76', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for DATASTORE_ in self.DATASTORE:
             namespaceprefix_ = self.DATASTORE_nsprefix_ + ':' if (UseCapturedNS_ and self.DATASTORE_nsprefix_) else ''
             DATASTORE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='DATASTORE', pretty_print=pretty_print)
@@ -36169,22 +36500,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DATASTORE':
-            obj_ = DATASTOREType75.factory(parent_object_=self)
+            obj_ = DATASTOREType77.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE.append(obj_)
             obj_.original_tagname_ = 'DATASTORE'
-# end class DATASTORE_QUOTAType74
+# end class DATASTORE_QUOTAType76
 
 
-class DATASTOREType75(GeneratedsSuper):
+class DATASTOREType77(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, IMAGES=None, IMAGES_USED=None, SIZE=None, SIZE_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36199,21 +36530,21 @@
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
         self.SIZE_USED = SIZE_USED
         self.SIZE_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTOREType75)
+                CurrentSubclassModule_, DATASTOREType77)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTOREType75.subclass:
-            return DATASTOREType75.subclass(*args_, **kwargs_)
+        if DATASTOREType77.subclass:
+            return DATASTOREType77.subclass(*args_, **kwargs_)
         else:
-            return DATASTOREType75(*args_, **kwargs_)
+            return DATASTOREType77(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -36242,40 +36573,40 @@
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType75', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType75')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType77', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType77')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTOREType75':
+        if self.original_tagname_ is not None and name_ == 'DATASTOREType77':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType75')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType77')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType75', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType77', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType75'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType77'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType75', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType77', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -36336,18 +36667,18 @@
             self.SIZE_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'SIZE_USED')
             value_ = self.gds_validate_string(value_, node, 'SIZE_USED')
             self.SIZE_USED = value_
             self.SIZE_USED_nsprefix_ = child_.prefix
-# end class DATASTOREType75
+# end class DATASTOREType77
 
 
-class NETWORK_QUOTAType76(GeneratedsSuper):
+class NETWORK_QUOTAType78(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, NETWORK=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36357,21 +36688,21 @@
             self.NETWORK = []
         else:
             self.NETWORK = NETWORK
         self.NETWORK_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORK_QUOTAType76)
+                CurrentSubclassModule_, NETWORK_QUOTAType78)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORK_QUOTAType76.subclass:
-            return NETWORK_QUOTAType76.subclass(*args_, **kwargs_)
+        if NETWORK_QUOTAType78.subclass:
+            return NETWORK_QUOTAType78.subclass(*args_, **kwargs_)
         else:
-            return NETWORK_QUOTAType76(*args_, **kwargs_)
+            return NETWORK_QUOTAType78(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_NETWORK(self):
         return self.NETWORK
@@ -36386,40 +36717,40 @@
     def _hasContent(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType76', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType76')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType78', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORK_QUOTAType78')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType76':
+        if self.original_tagname_ is not None and name_ == 'NETWORK_QUOTAType78':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType76')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType78')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType76', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType78', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType76'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType78'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType76', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType78', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for NETWORK_ in self.NETWORK:
             namespaceprefix_ = self.NETWORK_nsprefix_ + ':' if (UseCapturedNS_ and self.NETWORK_nsprefix_) else ''
             NETWORK_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='NETWORK', pretty_print=pretty_print)
@@ -36434,22 +36765,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'NETWORK':
-            obj_ = NETWORKType77.factory(parent_object_=self)
+            obj_ = NETWORKType79.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NETWORK.append(obj_)
             obj_.original_tagname_ = 'NETWORK'
-# end class NETWORK_QUOTAType76
+# end class NETWORK_QUOTAType78
 
 
-class NETWORKType77(GeneratedsSuper):
+class NETWORKType79(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, LEASES=None, LEASES_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36460,21 +36791,21 @@
         self.LEASES = LEASES
         self.LEASES_nsprefix_ = None
         self.LEASES_USED = LEASES_USED
         self.LEASES_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NETWORKType77)
+                CurrentSubclassModule_, NETWORKType79)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NETWORKType77.subclass:
-            return NETWORKType77.subclass(*args_, **kwargs_)
+        if NETWORKType79.subclass:
+            return NETWORKType79.subclass(*args_, **kwargs_)
         else:
-            return NETWORKType77(*args_, **kwargs_)
+            return NETWORKType79(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -36493,40 +36824,40 @@
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType77', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType77')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType79', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NETWORKType79')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NETWORKType77':
+        if self.original_tagname_ is not None and name_ == 'NETWORKType79':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType77')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType79')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType77', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType79', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType77'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType79'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType77', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORKType79', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -36567,39 +36898,39 @@
             self.LEASES_nsprefix_ = child_.prefix
         elif nodeName_ == 'LEASES_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'LEASES_USED')
             value_ = self.gds_validate_string(value_, node, 'LEASES_USED')
             self.LEASES_USED = value_
             self.LEASES_USED_nsprefix_ = child_.prefix
-# end class NETWORKType77
+# end class NETWORKType79
 
 
-class VM_QUOTAType78(GeneratedsSuper):
+class VM_QUOTAType80(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VM=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.VM = VM
         self.VM_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VM_QUOTAType78)
+                CurrentSubclassModule_, VM_QUOTAType80)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VM_QUOTAType78.subclass:
-            return VM_QUOTAType78.subclass(*args_, **kwargs_)
+        if VM_QUOTAType80.subclass:
+            return VM_QUOTAType80.subclass(*args_, **kwargs_)
         else:
-            return VM_QUOTAType78(*args_, **kwargs_)
+            return VM_QUOTAType80(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
@@ -36608,40 +36939,40 @@
     def _hasContent(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType78', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType78')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType80', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VM_QUOTAType80')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType78':
+        if self.original_tagname_ is not None and name_ == 'VM_QUOTAType80':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType78')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType80')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType78', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType80', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType78'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType80'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType78', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType80', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VM is not None:
             namespaceprefix_ = self.VM_nsprefix_ + ':' if (UseCapturedNS_ and self.VM_nsprefix_) else ''
             self.VM.export(outfile, level, namespaceprefix_, namespacedef_='', name_='VM', pretty_print=pretty_print)
@@ -36656,22 +36987,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'VM':
-            obj_ = VMType79.factory(parent_object_=self)
+            obj_ = VMType81.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VM = obj_
             obj_.original_tagname_ = 'VM'
-# end class VM_QUOTAType78
+# end class VM_QUOTAType80
 
 
-class VMType79(GeneratedsSuper):
+class VMType81(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CPU=None, CPU_USED=None, MEMORY=None, MEMORY_USED=None, RUNNING_CPU=None, RUNNING_CPU_USED=None, RUNNING_MEMORY=None, RUNNING_MEMORY_USED=None, RUNNING_VMS=None, RUNNING_VMS_USED=None, SYSTEM_DISK_SIZE=None, SYSTEM_DISK_SIZE_USED=None, VMS=None, VMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36704,21 +37035,21 @@
         self.VMS = VMS
         self.VMS_nsprefix_ = None
         self.VMS_USED = VMS_USED
         self.VMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VMType79)
+                CurrentSubclassModule_, VMType81)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VMType79.subclass:
-            return VMType79.subclass(*args_, **kwargs_)
+        if VMType81.subclass:
+            return VMType81.subclass(*args_, **kwargs_)
         else:
-            return VMType79(*args_, **kwargs_)
+            return VMType81(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CPU(self):
         return self.CPU
@@ -36792,40 +37123,40 @@
             self.SYSTEM_DISK_SIZE_USED is not None or
             self.VMS is not None or
             self.VMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType79', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType79')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType81', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType81')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VMType79':
+        if self.original_tagname_ is not None and name_ == 'VMType81':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType79')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType81')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType79', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType81', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType79'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType81'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType79', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType81', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CPU is not None:
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -36976,18 +37307,18 @@
             self.VMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'VMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VMS_USED')
             value_ = self.gds_validate_string(value_, node, 'VMS_USED')
             self.VMS_USED = value_
             self.VMS_USED_nsprefix_ = child_.prefix
-# end class VMType79
+# end class VMType81
 
 
-class IMAGE_QUOTAType80(GeneratedsSuper):
+class IMAGE_QUOTAType82(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, IMAGE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36997,21 +37328,21 @@
             self.IMAGE = []
         else:
             self.IMAGE = IMAGE
         self.IMAGE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGE_QUOTAType80)
+                CurrentSubclassModule_, IMAGE_QUOTAType82)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGE_QUOTAType80.subclass:
-            return IMAGE_QUOTAType80.subclass(*args_, **kwargs_)
+        if IMAGE_QUOTAType82.subclass:
+            return IMAGE_QUOTAType82.subclass(*args_, **kwargs_)
         else:
-            return IMAGE_QUOTAType80(*args_, **kwargs_)
+            return IMAGE_QUOTAType82(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_IMAGE(self):
         return self.IMAGE
@@ -37026,40 +37357,40 @@
     def _hasContent(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType80', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType80')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType82', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGE_QUOTAType82')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType80':
+        if self.original_tagname_ is not None and name_ == 'IMAGE_QUOTAType82':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType80')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType82')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType80', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType82', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType80'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType82'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType80', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType82', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for IMAGE_ in self.IMAGE:
             namespaceprefix_ = self.IMAGE_nsprefix_ + ':' if (UseCapturedNS_ and self.IMAGE_nsprefix_) else ''
             IMAGE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='IMAGE', pretty_print=pretty_print)
@@ -37074,22 +37405,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'IMAGE':
-            obj_ = IMAGEType81.factory(parent_object_=self)
+            obj_ = IMAGEType83.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.IMAGE.append(obj_)
             obj_.original_tagname_ = 'IMAGE'
-# end class IMAGE_QUOTAType80
+# end class IMAGE_QUOTAType82
 
 
-class IMAGEType81(GeneratedsSuper):
+class IMAGEType83(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, RVMS=None, RVMS_USED=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -37100,21 +37431,21 @@
         self.RVMS = RVMS
         self.RVMS_nsprefix_ = None
         self.RVMS_USED = RVMS_USED
         self.RVMS_USED_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, IMAGEType81)
+                CurrentSubclassModule_, IMAGEType83)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if IMAGEType81.subclass:
-            return IMAGEType81.subclass(*args_, **kwargs_)
+        if IMAGEType83.subclass:
+            return IMAGEType83.subclass(*args_, **kwargs_)
         else:
-            return IMAGEType81(*args_, **kwargs_)
+            return IMAGEType83(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -37133,40 +37464,40 @@
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType81', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType81')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType83', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('IMAGEType83')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'IMAGEType81':
+        if self.original_tagname_ is not None and name_ == 'IMAGEType83':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType81')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType83')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType81', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType83', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType81'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType83'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType81', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGEType83', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -37207,18 +37538,18 @@
             self.RVMS_nsprefix_ = child_.prefix
         elif nodeName_ == 'RVMS_USED':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'RVMS_USED')
             value_ = self.gds_validate_string(value_, node, 'RVMS_USED')
             self.RVMS_USED = value_
             self.RVMS_USED_nsprefix_ = child_.prefix
-# end class IMAGEType81
+# end class IMAGEType83
 
 
-class GROUPSType82(GeneratedsSuper):
+class GROUPSType84(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -37228,21 +37559,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, GROUPSType82)
+                CurrentSubclassModule_, GROUPSType84)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if GROUPSType82.subclass:
-            return GROUPSType82.subclass(*args_, **kwargs_)
+        if GROUPSType84.subclass:
+            return GROUPSType84.subclass(*args_, **kwargs_)
         else:
-            return GROUPSType82(*args_, **kwargs_)
+            return GROUPSType84(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -37257,40 +37588,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType82', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('GROUPSType82')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType84', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('GROUPSType84')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'GROUPSType82':
+        if self.original_tagname_ is not None and name_ == 'GROUPSType84':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPSType82')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPSType84')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPSType82', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPSType84', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPSType82'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPSType84'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType82', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType84', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -37311,18 +37642,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class GROUPSType82
+# end class GROUPSType84
 
 
-class CLUSTERSType83(GeneratedsSuper):
+class CLUSTERSType85(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CLUSTER=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -37332,21 +37663,21 @@
             self.CLUSTER = []
         else:
             self.CLUSTER = CLUSTER
         self.CLUSTER_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, CLUSTERSType83)
+                CurrentSubclassModule_, CLUSTERSType85)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if CLUSTERSType83.subclass:
-            return CLUSTERSType83.subclass(*args_, **kwargs_)
+        if CLUSTERSType85.subclass:
+            return CLUSTERSType85.subclass(*args_, **kwargs_)
         else:
-            return CLUSTERSType83(*args_, **kwargs_)
+            return CLUSTERSType85(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CLUSTER(self):
         return self.CLUSTER
@@ -37361,40 +37692,40 @@
     def _hasContent(self):
         if (
             self.CLUSTER
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType83', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('CLUSTERSType83')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType85', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('CLUSTERSType85')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'CLUSTERSType83':
+        if self.original_tagname_ is not None and name_ == 'CLUSTERSType85':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType83')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType85')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType83', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType85', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType83'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType85'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType83', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType85', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for CLUSTER_ in self.CLUSTER:
             namespaceprefix_ = self.CLUSTER_nsprefix_ + ':' if (UseCapturedNS_ and self.CLUSTER_nsprefix_) else ''
             CLUSTER_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='CLUSTER', pretty_print=pretty_print)
@@ -37413,15 +37744,15 @@
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'CLUSTER':
             obj_ = CLUSTERType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.CLUSTER.append(obj_)
             obj_.original_tagname_ = 'CLUSTER'
-# end class CLUSTERSType83
+# end class CLUSTERSType85
 
 
 class CLUSTERType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ZONE_ID=None, CLUSTER_ID=None, gds_collector_=None, **kwargs_):
@@ -37528,15 +37859,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'CLUSTER_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'CLUSTER_ID')
             self.CLUSTER_ID = ival_
             self.CLUSTER_ID_nsprefix_ = child_.prefix
 # end class CLUSTERType
 
 
-class HOSTSType84(GeneratedsSuper):
+class HOSTSType86(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, HOST=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -37546,21 +37877,21 @@
             self.HOST = []
         else:
             self.HOST = HOST
         self.HOST_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, HOSTSType84)
+                CurrentSubclassModule_, HOSTSType86)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if HOSTSType84.subclass:
-            return HOSTSType84.subclass(*args_, **kwargs_)
+        if HOSTSType86.subclass:
+            return HOSTSType86.subclass(*args_, **kwargs_)
         else:
-            return HOSTSType84(*args_, **kwargs_)
+            return HOSTSType86(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_HOST(self):
         return self.HOST
@@ -37575,40 +37906,40 @@
     def _hasContent(self):
         if (
             self.HOST
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOSTSType84', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('HOSTSType84')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOSTSType86', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('HOSTSType86')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'HOSTSType84':
+        if self.original_tagname_ is not None and name_ == 'HOSTSType86':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOSTSType84')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOSTSType86')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOSTSType84', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOSTSType86', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOSTSType84'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOSTSType86'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOSTSType84', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOSTSType86', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for HOST_ in self.HOST:
             namespaceprefix_ = self.HOST_nsprefix_ + ':' if (UseCapturedNS_ and self.HOST_nsprefix_) else ''
             HOST_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='HOST', pretty_print=pretty_print)
@@ -37627,15 +37958,15 @@
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'HOST':
             obj_ = HOSTType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.HOST.append(obj_)
             obj_.original_tagname_ = 'HOST'
-# end class HOSTSType84
+# end class HOSTSType86
 
 
 class HOSTType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ZONE_ID=None, HOST_ID=None, gds_collector_=None, **kwargs_):
@@ -37742,15 +38073,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'HOST_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'HOST_ID')
             self.HOST_ID = ival_
             self.HOST_ID_nsprefix_ = child_.prefix
 # end class HOSTType
 
 
-class DATASTORESType85(GeneratedsSuper):
+class DATASTORESType87(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DATASTORE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -37760,21 +38091,21 @@
             self.DATASTORE = []
         else:
             self.DATASTORE = DATASTORE
         self.DATASTORE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTORESType85)
+                CurrentSubclassModule_, DATASTORESType87)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTORESType85.subclass:
-            return DATASTORESType85.subclass(*args_, **kwargs_)
+        if DATASTORESType87.subclass:
+            return DATASTORESType87.subclass(*args_, **kwargs_)
         else:
-            return DATASTORESType85(*args_, **kwargs_)
+            return DATASTORESType87(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DATASTORE(self):
         return self.DATASTORE
@@ -37789,40 +38120,40 @@
     def _hasContent(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORESType85', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORESType85')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORESType87', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTORESType87')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTORESType85':
+        if self.original_tagname_ is not None and name_ == 'DATASTORESType87':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORESType85')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORESType87')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORESType85', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORESType87', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORESType85'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORESType87'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORESType85', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORESType87', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for DATASTORE_ in self.DATASTORE:
             namespaceprefix_ = self.DATASTORE_nsprefix_ + ':' if (UseCapturedNS_ and self.DATASTORE_nsprefix_) else ''
             DATASTORE_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='DATASTORE', pretty_print=pretty_print)
@@ -37837,22 +38168,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'DATASTORE':
-            obj_ = DATASTOREType86.factory(parent_object_=self)
+            obj_ = DATASTOREType88.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DATASTORE.append(obj_)
             obj_.original_tagname_ = 'DATASTORE'
-# end class DATASTORESType85
+# end class DATASTORESType87
 
 
-class DATASTOREType86(GeneratedsSuper):
+class DATASTOREType88(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ZONE_ID=None, DATASTORE_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -37861,21 +38192,21 @@
         self.ZONE_ID = ZONE_ID
         self.ZONE_ID_nsprefix_ = None
         self.DATASTORE_ID = DATASTORE_ID
         self.DATASTORE_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DATASTOREType86)
+                CurrentSubclassModule_, DATASTOREType88)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DATASTOREType86.subclass:
-            return DATASTOREType86.subclass(*args_, **kwargs_)
+        if DATASTOREType88.subclass:
+            return DATASTOREType88.subclass(*args_, **kwargs_)
         else:
-            return DATASTOREType86(*args_, **kwargs_)
+            return DATASTOREType88(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ZONE_ID(self):
         return self.ZONE_ID
@@ -37889,40 +38220,40 @@
         if (
             self.ZONE_ID is not None or
             self.DATASTORE_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType86', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType86')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType88', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DATASTOREType88')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DATASTOREType86':
+        if self.original_tagname_ is not None and name_ == 'DATASTOREType88':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType86')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType88')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType86', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType88', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType86'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType88'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType86', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTOREType88', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ZONE_ID is not None:
             namespaceprefix_ = self.ZONE_ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ZONE_ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -37953,18 +38284,18 @@
             self.ZONE_ID_nsprefix_ = child_.prefix
         elif nodeName_ == 'DATASTORE_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'DATASTORE_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'DATASTORE_ID')
             self.DATASTORE_ID = ival_
             self.DATASTORE_ID_nsprefix_ = child_.prefix
-# end class DATASTOREType86
+# end class DATASTOREType88
 
 
-class VNETSType87(GeneratedsSuper):
+class VNETSType89(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VNET=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -37974,21 +38305,21 @@
             self.VNET = []
         else:
             self.VNET = VNET
         self.VNET_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VNETSType87)
+                CurrentSubclassModule_, VNETSType89)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VNETSType87.subclass:
-            return VNETSType87.subclass(*args_, **kwargs_)
+        if VNETSType89.subclass:
+            return VNETSType89.subclass(*args_, **kwargs_)
         else:
-            return VNETSType87(*args_, **kwargs_)
+            return VNETSType89(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VNET(self):
         return self.VNET
@@ -38003,40 +38334,40 @@
     def _hasContent(self):
         if (
             self.VNET
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETSType87', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VNETSType87')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETSType89', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VNETSType89')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VNETSType87':
+        if self.original_tagname_ is not None and name_ == 'VNETSType89':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETSType87')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETSType89')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETSType87', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETSType89', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETSType87'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETSType89'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETSType87', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETSType89', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for VNET_ in self.VNET:
             namespaceprefix_ = self.VNET_nsprefix_ + ':' if (UseCapturedNS_ and self.VNET_nsprefix_) else ''
             VNET_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='VNET', pretty_print=pretty_print)
@@ -38055,15 +38386,15 @@
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'VNET':
             obj_ = VNETType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VNET.append(obj_)
             obj_.original_tagname_ = 'VNET'
-# end class VNETSType87
+# end class VNETSType89
 
 
 class VNETType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ZONE_ID=None, VNET_ID=None, gds_collector_=None, **kwargs_):
@@ -38170,15 +38501,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'VNET_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'VNET_ID')
             self.VNET_ID = ival_
             self.VNET_ID_nsprefix_ = child_.prefix
 # end class VNETType
 
 
-class PERMISSIONSType88(GeneratedsSuper):
+class PERMISSIONSType90(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38201,21 +38532,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType88)
+                CurrentSubclassModule_, PERMISSIONSType90)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType88.subclass:
-            return PERMISSIONSType88.subclass(*args_, **kwargs_)
+        if PERMISSIONSType90.subclass:
+            return PERMISSIONSType90.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType88(*args_, **kwargs_)
+            return PERMISSIONSType90(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -38264,40 +38595,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType88', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType88')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType90', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType90')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType88':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType90':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType88')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType90')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType88', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType90', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType88'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType90'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType88', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType90', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -38398,18 +38729,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType88
+# end class PERMISSIONSType90
 
 
-class LOCKType89(GeneratedsSuper):
+class LOCKType91(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38422,21 +38753,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType89)
+                CurrentSubclassModule_, LOCKType91)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType89.subclass:
-            return LOCKType89.subclass(*args_, **kwargs_)
+        if LOCKType91.subclass:
+            return LOCKType91.subclass(*args_, **kwargs_)
         else:
-            return LOCKType89(*args_, **kwargs_)
+            return LOCKType91(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -38460,40 +38791,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType89', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType89')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType91', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType91')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType89':
+        if self.original_tagname_ is not None and name_ == 'LOCKType91':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType89')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType91')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType89', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType91', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType89'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType91'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType89', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType91', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -38544,15 +38875,15 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType89
+# end class LOCKType91
 
 
 class ROLESType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ROLE=None, gds_collector_=None, **kwargs_):
@@ -38812,15 +39143,15 @@
             value_ = self.gds_parse_string(value_, node, 'POLICY')
             value_ = self.gds_validate_string(value_, node, 'POLICY')
             self.POLICY = value_
             self.POLICY_nsprefix_ = child_.prefix
 # end class ROLEType
 
 
-class VMType90(GeneratedsSuper):
+class VMType92(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, UID=None, GID=None, UNAME=None, GNAME=None, NAME=None, LAST_POLL=None, STATE=None, LCM_STATE=None, RESCHED=None, STIME=None, ETIME=None, DEPLOY_ID=None, TEMPLATE=None, MONITORING=None, USER_TEMPLATE=None, HISTORY_RECORDS=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38859,21 +39190,21 @@
         self.USER_TEMPLATE = USER_TEMPLATE
         self.USER_TEMPLATE_nsprefix_ = None
         self.HISTORY_RECORDS = HISTORY_RECORDS
         self.HISTORY_RECORDS_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VMType90)
+                CurrentSubclassModule_, VMType92)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VMType90.subclass:
-            return VMType90.subclass(*args_, **kwargs_)
+        if VMType92.subclass:
+            return VMType92.subclass(*args_, **kwargs_)
         else:
-            return VMType90(*args_, **kwargs_)
+            return VMType92(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -38962,40 +39293,40 @@
             self.MONITORING is not None or
             self.USER_TEMPLATE is not None or
             self.HISTORY_RECORDS is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType90', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType90')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType92', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMType92')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VMType90':
+        if self.original_tagname_ is not None and name_ == 'VMType92':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType90')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType92')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType90', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType92', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType90'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType92'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType90', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMType92', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -39149,37 +39480,37 @@
         elif nodeName_ == 'DEPLOY_ID':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'DEPLOY_ID')
             value_ = self.gds_validate_string(value_, node, 'DEPLOY_ID')
             self.DEPLOY_ID = value_
             self.DEPLOY_ID_nsprefix_ = child_.prefix
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType91.factory(parent_object_=self)
+            obj_ = TEMPLATEType93.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
         elif nodeName_ == 'MONITORING':
-            obj_ = MONITORINGType92.factory(parent_object_=self)
+            obj_ = MONITORINGType94.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.MONITORING = obj_
             obj_.original_tagname_ = 'MONITORING'
         elif nodeName_ == 'USER_TEMPLATE':
             obj_ = USER_TEMPLATEType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.USER_TEMPLATE = obj_
             obj_.original_tagname_ = 'USER_TEMPLATE'
         elif nodeName_ == 'HISTORY_RECORDS':
             obj_ = HISTORY_RECORDSType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.HISTORY_RECORDS = obj_
             obj_.original_tagname_ = 'HISTORY_RECORDS'
-# end class VMType90
+# end class VMType92
 
 
-class TEMPLATEType91(GeneratedsSuper):
+class TEMPLATEType93(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CPU=None, MEMORY=None, DISK=None, NIC=None, GRAPHICS=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -39200,21 +39531,21 @@
             self.NIC = NIC
         self.NIC_nsprefix_ = None
         self.GRAPHICS = GRAPHICS
         self.GRAPHICS_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType91)
+                CurrentSubclassModule_, TEMPLATEType93)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType91.subclass:
-            return TEMPLATEType91.subclass(*args_, **kwargs_)
+        if TEMPLATEType93.subclass:
+            return TEMPLATEType93.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType91(*args_, **kwargs_)
+            return TEMPLATEType93(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CPU(self):
         return self.CPU
@@ -39255,40 +39586,40 @@
             self.DISK or
             self.NIC or
             self.GRAPHICS is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType91', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType91')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType93', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType93')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType91':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType93':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType91')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType93')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType91', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType93', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType91'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType93'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType91', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType93', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CPU is not None:
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -39345,15 +39676,15 @@
             obj_.original_tagname_ = 'NIC'
         elif nodeName_ == 'GRAPHICS':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'GRAPHICS')
             value_ = self.gds_validate_string(value_, node, 'GRAPHICS')
             self.GRAPHICS = value_
             self.GRAPHICS_nsprefix_ = child_.prefix
-# end class TEMPLATEType91
+# end class TEMPLATEType93
 
 
 class GRAPHICS(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, gds_collector_=None, **kwargs_):
@@ -39699,15 +40030,15 @@
             self.VCENTER_PORTGROUP_TYPE_nsprefix_ = child_.prefix
         else:
             content_ = self.gds_build_any(child_, 'NICType')
             self.anytypeobjs_.append(content_)
 # end class NICType
 
 
-class MONITORINGType92(GeneratedsSuper):
+class MONITORINGType94(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -39716,21 +40047,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, MONITORINGType92)
+                CurrentSubclassModule_, MONITORINGType94)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if MONITORINGType92.subclass:
-            return MONITORINGType92.subclass(*args_, **kwargs_)
+        if MONITORINGType94.subclass:
+            return MONITORINGType94.subclass(*args_, **kwargs_)
         else:
-            return MONITORINGType92(*args_, **kwargs_)
+            return MONITORINGType94(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
@@ -39739,40 +40070,40 @@
     def _hasContent(self):
         if (
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType92', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('MONITORINGType92')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType94', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('MONITORINGType94')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'MONITORINGType92':
+        if self.original_tagname_ is not None and name_ == 'MONITORINGType94':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType92')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType94')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType92', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType94', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType92'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType94'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType92', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType94', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if not fromsubclass_:
             for obj_ in self.anytypeobjs_:
                 showIndent(outfile, level, pretty_print)
@@ -39788,17 +40119,17 @@
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
-        content_ = self.gds_build_any(child_, 'MONITORINGType92')
+        content_ = self.gds_build_any(child_, 'MONITORINGType94')
         self.anytypeobjs_.append(content_)
-# end class MONITORINGType92
+# end class MONITORINGType94
 
 
 class USER_TEMPLATEType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, anytypeobjs_=None, gds_collector_=None, **kwargs_):
@@ -40220,15 +40551,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'ACTION')
             ival_ = self.gds_validate_integer(ival_, node, 'ACTION')
             self.ACTION = ival_
             self.ACTION_nsprefix_ = child_.prefix
 # end class HISTORYType
 
 
-class LOCKType93(GeneratedsSuper):
+class LOCKType95(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40241,21 +40572,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType93)
+                CurrentSubclassModule_, LOCKType95)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType93.subclass:
-            return LOCKType93.subclass(*args_, **kwargs_)
+        if LOCKType95.subclass:
+            return LOCKType95.subclass(*args_, **kwargs_)
         else:
-            return LOCKType93(*args_, **kwargs_)
+            return LOCKType95(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -40279,40 +40610,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType93', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType93')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType95', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType95')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType93':
+        if self.original_tagname_ is not None and name_ == 'LOCKType95':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType93')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType95')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType93', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType95', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType93'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType95'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType93', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType95', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40363,18 +40694,18 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType93
+# end class LOCKType95
 
 
-class PERMISSIONSType94(GeneratedsSuper):
+class PERMISSIONSType96(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40397,21 +40728,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType94)
+                CurrentSubclassModule_, PERMISSIONSType96)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType94.subclass:
-            return PERMISSIONSType94.subclass(*args_, **kwargs_)
+        if PERMISSIONSType96.subclass:
+            return PERMISSIONSType96.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType94(*args_, **kwargs_)
+            return PERMISSIONSType96(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -40460,40 +40791,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType94', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType94')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType96', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType96')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType94':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType96':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType94')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType96')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType94', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType96', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType94'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType96'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType94', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType96', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40594,18 +40925,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType94
+# end class PERMISSIONSType96
 
 
-class TEMPLATEType95(GeneratedsSuper):
+class TEMPLATEType97(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VCENTER_CCR_REF=None, VCENTER_INSTANCE_ID=None, VCENTER_TEMPLATE_REF=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40620,21 +40951,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType95)
+                CurrentSubclassModule_, TEMPLATEType97)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType95.subclass:
-            return TEMPLATEType95.subclass(*args_, **kwargs_)
+        if TEMPLATEType97.subclass:
+            return TEMPLATEType97.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType95(*args_, **kwargs_)
+            return TEMPLATEType97(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VCENTER_CCR_REF(self):
         return self.VCENTER_CCR_REF
@@ -40658,40 +40989,40 @@
             self.VCENTER_INSTANCE_ID is not None or
             self.VCENTER_TEMPLATE_REF is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType95', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType95')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType97', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType97')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType95':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType97':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType95')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType97')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType95', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType97', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType95'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType97'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType95', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType97', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VCENTER_CCR_REF is not None:
             namespaceprefix_ = self.VCENTER_CCR_REF_nsprefix_ + ':' if (UseCapturedNS_ and self.VCENTER_CCR_REF_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40738,20 +41069,20 @@
         elif nodeName_ == 'VCENTER_TEMPLATE_REF':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_TEMPLATE_REF')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_TEMPLATE_REF')
             self.VCENTER_TEMPLATE_REF = value_
             self.VCENTER_TEMPLATE_REF_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'TEMPLATEType95')
+            content_ = self.gds_build_any(child_, 'TEMPLATEType97')
             self.anytypeobjs_.append(content_)
-# end class TEMPLATEType95
+# end class TEMPLATEType97
 
 
-class PERMISSIONSType96(GeneratedsSuper):
+class PERMISSIONSType98(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40774,21 +41105,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType96)
+                CurrentSubclassModule_, PERMISSIONSType98)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType96.subclass:
-            return PERMISSIONSType96.subclass(*args_, **kwargs_)
+        if PERMISSIONSType98.subclass:
+            return PERMISSIONSType98.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType96(*args_, **kwargs_)
+            return PERMISSIONSType98(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -40837,40 +41168,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType96', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType96')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType98', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType98')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType96':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType98':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType96')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType98')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType96', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType98', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType96'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType98'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType96', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType98', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40971,18 +41302,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType96
+# end class PERMISSIONSType98
 
 
-class LOCKType97(GeneratedsSuper):
+class LOCKType99(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40995,21 +41326,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType97)
+                CurrentSubclassModule_, LOCKType99)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType97.subclass:
-            return LOCKType97.subclass(*args_, **kwargs_)
+        if LOCKType99.subclass:
+            return LOCKType99.subclass(*args_, **kwargs_)
         else:
-            return LOCKType97(*args_, **kwargs_)
+            return LOCKType99(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -41033,40 +41364,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType97', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType97')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType99', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType99')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType97':
+        if self.original_tagname_ is not None and name_ == 'LOCKType99':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType97')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType99')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType97', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType99', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType97'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType99'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType97', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType99', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -41117,18 +41448,18 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType97
+# end class LOCKType99
 
 
-class MONITORINGType98(GeneratedsSuper):
+class MONITORINGType100(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, CPU=None, DISKRDBYTES=None, DISKRDIOPS=None, DISKWRBYTES=None, DISKWRIOPS=None, DISK_SIZE=None, ID=None, MEMORY=None, NETRX=None, NETTX=None, TIMESTAMP=None, VCENTER_ESX_HOST=None, VCENTER_GUEST_STATE=None, VCENTER_RP_NAME=None, VCENTER_VMWARETOOLS_RUNNING_STATUS=None, VCENTER_VMWARETOOLS_VERSION=None, VCENTER_VMWARETOOLS_VERSION_STATUS=None, VCENTER_VM_NAME=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -41172,21 +41503,21 @@
         self.VCENTER_VMWARETOOLS_VERSION_STATUS = VCENTER_VMWARETOOLS_VERSION_STATUS
         self.VCENTER_VMWARETOOLS_VERSION_STATUS_nsprefix_ = None
         self.VCENTER_VM_NAME = VCENTER_VM_NAME
         self.VCENTER_VM_NAME_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, MONITORINGType98)
+                CurrentSubclassModule_, MONITORINGType100)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if MONITORINGType98.subclass:
-            return MONITORINGType98.subclass(*args_, **kwargs_)
+        if MONITORINGType100.subclass:
+            return MONITORINGType100.subclass(*args_, **kwargs_)
         else:
-            return MONITORINGType98(*args_, **kwargs_)
+            return MONITORINGType100(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_CPU(self):
         return self.CPU
@@ -41286,40 +41617,40 @@
             self.VCENTER_VMWARETOOLS_VERSION is not None or
             self.VCENTER_VMWARETOOLS_VERSION_STATUS is not None or
             self.VCENTER_VM_NAME is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType98', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('MONITORINGType98')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType100', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('MONITORINGType100')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'MONITORINGType98':
+        if self.original_tagname_ is not None and name_ == 'MONITORINGType100':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType98')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType100')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType98', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType100', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType98'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType100'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType98', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType100', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.CPU is not None:
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -41432,15 +41763,15 @@
         elif nodeName_ == 'DISKWRIOPS' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'DISKWRIOPS')
             ival_ = self.gds_validate_integer(ival_, node, 'DISKWRIOPS')
             self.DISKWRIOPS = ival_
             self.DISKWRIOPS_nsprefix_ = child_.prefix
         elif nodeName_ == 'DISK_SIZE':
-            obj_ = DISK_SIZEType99.factory(parent_object_=self)
+            obj_ = DISK_SIZEType101.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DISK_SIZE.append(obj_)
             obj_.original_tagname_ = 'DISK_SIZE'
         elif nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
@@ -41508,18 +41839,18 @@
             self.VCENTER_VMWARETOOLS_VERSION_STATUS_nsprefix_ = child_.prefix
         elif nodeName_ == 'VCENTER_VM_NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_VM_NAME')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_VM_NAME')
             self.VCENTER_VM_NAME = value_
             self.VCENTER_VM_NAME_nsprefix_ = child_.prefix
-# end class MONITORINGType98
+# end class MONITORINGType100
 
 
-class DISK_SIZEType99(GeneratedsSuper):
+class DISK_SIZEType101(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, SIZE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -41528,21 +41859,21 @@
         self.ID = ID
         self.ID_nsprefix_ = None
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DISK_SIZEType99)
+                CurrentSubclassModule_, DISK_SIZEType101)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DISK_SIZEType99.subclass:
-            return DISK_SIZEType99.subclass(*args_, **kwargs_)
+        if DISK_SIZEType101.subclass:
+            return DISK_SIZEType101.subclass(*args_, **kwargs_)
         else:
-            return DISK_SIZEType99(*args_, **kwargs_)
+            return DISK_SIZEType101(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -41556,40 +41887,40 @@
         if (
             self.ID is not None or
             self.SIZE is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISK_SIZEType99', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DISK_SIZEType99')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISK_SIZEType101', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DISK_SIZEType101')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DISK_SIZEType99':
+        if self.original_tagname_ is not None and name_ == 'DISK_SIZEType101':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISK_SIZEType99')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISK_SIZEType101')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISK_SIZEType99', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISK_SIZEType101', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISK_SIZEType99'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISK_SIZEType101'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISK_SIZEType99', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISK_SIZEType101', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -41620,18 +41951,18 @@
             self.ID_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'SIZE')
             ival_ = self.gds_validate_integer(ival_, node, 'SIZE')
             self.SIZE = ival_
             self.SIZE_nsprefix_ = child_.prefix
-# end class DISK_SIZEType99
+# end class DISK_SIZEType101
 
 
-class TEMPLATEType100(GeneratedsSuper):
+class TEMPLATEType102(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, AUTOMATIC_DS_REQUIREMENTS=None, AUTOMATIC_NIC_REQUIREMENTS=None, AUTOMATIC_REQUIREMENTS=None, CLONING_TEMPLATE_ID=None, CONTEXT=None, CPU=None, CPU_COST=None, DISK=None, DISK_COST=None, EMULATOR=None, FEATURES=None, HYPERV_OPTIONS=None, GRAPHICS=None, IMPORTED=None, INPUT=None, MEMORY=None, MEMORY_COST=None, MEMORY_MAX=None, MEMORY_SLOTS=None, MEMORY_RESIZE_MODE=None, NIC=None, NIC_ALIAS=None, NIC_DEFAULT=None, NUMA_NODE=None, OS=None, PCI=None, RAW=None, SCHED_ACTION=None, SECURITY_GROUP_RULE=None, SNAPSHOT=None, SPICE_OPTIONS=None, SUBMIT_ON_HOLD=None, TEMPLATE_ID=None, TM_MAD_SYSTEM=None, TOPOLOGY=None, VCPU=None, VCPU_MAX=None, VMGROUP=None, VMID=None, VROUTER_ID=None, VROUTER_KEEPALIVED_ID=None, VROUTER_KEEPALIVED_PASSWORD=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -41741,21 +42072,21 @@
         self.VROUTER_KEEPALIVED_ID = VROUTER_KEEPALIVED_ID
         self.VROUTER_KEEPALIVED_ID_nsprefix_ = None
         self.VROUTER_KEEPALIVED_PASSWORD = VROUTER_KEEPALIVED_PASSWORD
         self.VROUTER_KEEPALIVED_PASSWORD_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType100)
+                CurrentSubclassModule_, TEMPLATEType102)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType100.subclass:
-            return TEMPLATEType100.subclass(*args_, **kwargs_)
+        if TEMPLATEType102.subclass:
+            return TEMPLATEType102.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType100(*args_, **kwargs_)
+            return TEMPLATEType102(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_AUTOMATIC_DS_REQUIREMENTS(self):
         return self.AUTOMATIC_DS_REQUIREMENTS
@@ -42011,40 +42342,40 @@
             self.VROUTER_ID is not None or
             self.VROUTER_KEEPALIVED_ID is not None or
             self.VROUTER_KEEPALIVED_PASSWORD is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType100', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType100')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType102', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType102')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType100':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType102':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType100')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType102')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType100', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType102', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType100'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType102'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType100', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType102', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.AUTOMATIC_DS_REQUIREMENTS is not None:
             namespaceprefix_ = self.AUTOMATIC_DS_REQUIREMENTS_nsprefix_ + ':' if (UseCapturedNS_ and self.AUTOMATIC_DS_REQUIREMENTS_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -42261,15 +42592,15 @@
         elif nodeName_ == 'CPU_COST':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'CPU_COST')
             value_ = self.gds_validate_string(value_, node, 'CPU_COST')
             self.CPU_COST = value_
             self.CPU_COST_nsprefix_ = child_.prefix
         elif nodeName_ == 'DISK':
-            obj_ = DISKType101.factory(parent_object_=self)
+            obj_ = DISKType103.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DISK.append(obj_)
             obj_.original_tagname_ = 'DISK'
         elif nodeName_ == 'DISK_COST':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'DISK_COST')
             value_ = self.gds_validate_string(value_, node, 'DISK_COST')
@@ -42338,15 +42669,15 @@
         elif nodeName_ == 'MEMORY_RESIZE_MODE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'MEMORY_RESIZE_MODE')
             value_ = self.gds_validate_string(value_, node, 'MEMORY_RESIZE_MODE')
             self.MEMORY_RESIZE_MODE = value_
             self.MEMORY_RESIZE_MODE_nsprefix_ = child_.prefix
         elif nodeName_ == 'NIC':
-            obj_ = NICType102.factory(parent_object_=self)
+            obj_ = NICType104.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NIC.append(obj_)
             obj_.original_tagname_ = 'NIC'
         elif nodeName_ == 'NIC_ALIAS':
             obj_ = NIC_ALIASType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.NIC_ALIAS.append(obj_)
@@ -42389,15 +42720,15 @@
         elif nodeName_ == 'SECURITY_GROUP_RULE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'SECURITY_GROUP_RULE')
             value_ = self.gds_validate_string(value_, node, 'SECURITY_GROUP_RULE')
             self.SECURITY_GROUP_RULE.append(value_)
             self.SECURITY_GROUP_RULE_nsprefix_ = child_.prefix
         elif nodeName_ == 'SNAPSHOT':
-            obj_ = SNAPSHOTType103.factory(parent_object_=self)
+            obj_ = SNAPSHOTType105.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SNAPSHOT.append(obj_)
             obj_.original_tagname_ = 'SNAPSHOT'
         elif nodeName_ == 'SPICE_OPTIONS':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'SPICE_OPTIONS')
             value_ = self.gds_validate_string(value_, node, 'SPICE_OPTIONS')
@@ -42465,15 +42796,15 @@
             self.VROUTER_KEEPALIVED_ID_nsprefix_ = child_.prefix
         elif nodeName_ == 'VROUTER_KEEPALIVED_PASSWORD':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VROUTER_KEEPALIVED_PASSWORD')
             value_ = self.gds_validate_string(value_, node, 'VROUTER_KEEPALIVED_PASSWORD')
             self.VROUTER_KEEPALIVED_PASSWORD = value_
             self.VROUTER_KEEPALIVED_PASSWORD_nsprefix_ = child_.prefix
-# end class TEMPLATEType100
+# end class TEMPLATEType102
 
 
 class CONTEXT(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, gds_collector_=None, **kwargs_):
@@ -43456,15 +43787,15 @@
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class VMGROUP
 
 
-class DISKType101(GeneratedsSuper):
+class DISKType103(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VCENTER_DS_REF=None, VCENTER_INSTANCE_ID=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -43477,21 +43808,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, DISKType101)
+                CurrentSubclassModule_, DISKType103)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if DISKType101.subclass:
-            return DISKType101.subclass(*args_, **kwargs_)
+        if DISKType103.subclass:
+            return DISKType103.subclass(*args_, **kwargs_)
         else:
-            return DISKType101(*args_, **kwargs_)
+            return DISKType103(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VCENTER_DS_REF(self):
         return self.VCENTER_DS_REF
@@ -43510,40 +43841,40 @@
             self.VCENTER_DS_REF is not None or
             self.VCENTER_INSTANCE_ID is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISKType101', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DISKType101')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISKType103', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('DISKType103')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'DISKType101':
+        if self.original_tagname_ is not None and name_ == 'DISKType103':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISKType101')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISKType103')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISKType101', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISKType103', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISKType101'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISKType103'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISKType101', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DISKType103', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VCENTER_DS_REF is not None:
             namespaceprefix_ = self.VCENTER_DS_REF_nsprefix_ + ':' if (UseCapturedNS_ and self.VCENTER_DS_REF_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -43580,20 +43911,20 @@
         elif nodeName_ == 'VCENTER_INSTANCE_ID':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_INSTANCE_ID')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_INSTANCE_ID')
             self.VCENTER_INSTANCE_ID = value_
             self.VCENTER_INSTANCE_ID_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'DISKType101')
+            content_ = self.gds_build_any(child_, 'DISKType103')
             self.anytypeobjs_.append(content_)
-# end class DISKType101
+# end class DISKType103
 
 
-class NICType102(GeneratedsSuper):
+class NICType104(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, anytypeobjs_=None, VCENTER_INSTANCE_ID=None, VCENTER_NET_REF=None, VCENTER_PORTGROUP_TYPE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -43608,21 +43939,21 @@
         self.VCENTER_NET_REF = VCENTER_NET_REF
         self.VCENTER_NET_REF_nsprefix_ = None
         self.VCENTER_PORTGROUP_TYPE = VCENTER_PORTGROUP_TYPE
         self.VCENTER_PORTGROUP_TYPE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, NICType102)
+                CurrentSubclassModule_, NICType104)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if NICType102.subclass:
-            return NICType102.subclass(*args_, **kwargs_)
+        if NICType104.subclass:
+            return NICType104.subclass(*args_, **kwargs_)
         else:
-            return NICType102(*args_, **kwargs_)
+            return NICType104(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
@@ -43646,40 +43977,40 @@
             self.VCENTER_INSTANCE_ID is not None or
             self.VCENTER_NET_REF is not None or
             self.VCENTER_PORTGROUP_TYPE is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NICType102', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NICType102')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NICType104', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('NICType104')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'NICType102':
+        if self.original_tagname_ is not None and name_ == 'NICType104':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NICType102')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NICType104')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NICType102', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NICType104', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NICType102'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NICType104'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NICType102', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NICType104', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VCENTER_INSTANCE_ID is not None:
             namespaceprefix_ = self.VCENTER_INSTANCE_ID_nsprefix_ + ':' if (UseCapturedNS_ and self.VCENTER_INSTANCE_ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -43726,17 +44057,17 @@
         elif nodeName_ == 'VCENTER_PORTGROUP_TYPE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_PORTGROUP_TYPE')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_PORTGROUP_TYPE')
             self.VCENTER_PORTGROUP_TYPE = value_
             self.VCENTER_PORTGROUP_TYPE_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'NICType102')
+            content_ = self.gds_build_any(child_, 'NICType104')
             self.anytypeobjs_.append(content_)
-# end class NICType102
+# end class NICType104
 
 
 class NIC_ALIASType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ALIAS_ID=None, PARENT=None, PARENT_ID=None, anytypeobjs_=None, VCENTER_INSTANCE_ID=None, VCENTER_NET_REF=None, VCENTER_PORTGROUP_TYPE=None, gds_collector_=None, **kwargs_):
@@ -44159,15 +44490,15 @@
             value_ = self.gds_parse_string(value_, node, 'WARNING')
             value_ = self.gds_validate_string(value_, node, 'WARNING')
             self.WARNING = value_
             self.WARNING_nsprefix_ = child_.prefix
 # end class SCHED_ACTIONType
 
 
-class SNAPSHOTType103(GeneratedsSuper):
+class SNAPSHOTType105(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ACTION=None, ACTIVE=None, HYPERVISOR_ID=None, NAME=None, SNAPSHOT_ID=None, SYSTEM_DISK_SIZE=None, TIME=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -44186,21 +44517,21 @@
         self.SYSTEM_DISK_SIZE = SYSTEM_DISK_SIZE
         self.SYSTEM_DISK_SIZE_nsprefix_ = None
         self.TIME = TIME
         self.TIME_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SNAPSHOTType103)
+                CurrentSubclassModule_, SNAPSHOTType105)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if SNAPSHOTType103.subclass:
-            return SNAPSHOTType103.subclass(*args_, **kwargs_)
+        if SNAPSHOTType105.subclass:
+            return SNAPSHOTType105.subclass(*args_, **kwargs_)
         else:
-            return SNAPSHOTType103(*args_, **kwargs_)
+            return SNAPSHOTType105(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ACTION(self):
         return self.ACTION
@@ -44239,40 +44570,40 @@
             self.SNAPSHOT_ID is not None or
             self.SYSTEM_DISK_SIZE is not None or
             self.TIME is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType103', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTType103')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType105', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTType105')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SNAPSHOTType103':
+        if self.original_tagname_ is not None and name_ == 'SNAPSHOTType105':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType103')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType105')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType103', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType105', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType103'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType105'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType103', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType105', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ACTION is not None:
             namespaceprefix_ = self.ACTION_nsprefix_ + ':' if (UseCapturedNS_ and self.ACTION_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -44353,18 +44684,18 @@
             self.SYSTEM_DISK_SIZE_nsprefix_ = child_.prefix
         elif nodeName_ == 'TIME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'TIME')
             value_ = self.gds_validate_string(value_, node, 'TIME')
             self.TIME = value_
             self.TIME_nsprefix_ = child_.prefix
-# end class SNAPSHOTType103
+# end class SNAPSHOTType105
 
 
-class USER_TEMPLATEType104(GeneratedsSuper):
+class USER_TEMPLATEType106(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VCENTER_CCR_REF=None, VCENTER_DS_REF=None, VCENTER_INSTANCE_ID=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -44379,21 +44710,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, USER_TEMPLATEType104)
+                CurrentSubclassModule_, USER_TEMPLATEType106)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if USER_TEMPLATEType104.subclass:
-            return USER_TEMPLATEType104.subclass(*args_, **kwargs_)
+        if USER_TEMPLATEType106.subclass:
+            return USER_TEMPLATEType106.subclass(*args_, **kwargs_)
         else:
-            return USER_TEMPLATEType104(*args_, **kwargs_)
+            return USER_TEMPLATEType106(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VCENTER_CCR_REF(self):
         return self.VCENTER_CCR_REF
@@ -44417,40 +44748,40 @@
             self.VCENTER_DS_REF is not None or
             self.VCENTER_INSTANCE_ID is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='USER_TEMPLATEType104', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('USER_TEMPLATEType104')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='USER_TEMPLATEType106', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('USER_TEMPLATEType106')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'USER_TEMPLATEType104':
+        if self.original_tagname_ is not None and name_ == 'USER_TEMPLATEType106':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USER_TEMPLATEType104')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USER_TEMPLATEType106')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USER_TEMPLATEType104', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USER_TEMPLATEType106', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USER_TEMPLATEType104'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USER_TEMPLATEType106'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='USER_TEMPLATEType104', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='USER_TEMPLATEType106', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VCENTER_CCR_REF is not None:
             namespaceprefix_ = self.VCENTER_CCR_REF_nsprefix_ + ':' if (UseCapturedNS_ and self.VCENTER_CCR_REF_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -44497,20 +44828,20 @@
         elif nodeName_ == 'VCENTER_INSTANCE_ID':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_INSTANCE_ID')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_INSTANCE_ID')
             self.VCENTER_INSTANCE_ID = value_
             self.VCENTER_INSTANCE_ID_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'USER_TEMPLATEType104')
+            content_ = self.gds_build_any(child_, 'USER_TEMPLATEType106')
             self.anytypeobjs_.append(content_)
-# end class USER_TEMPLATEType104
+# end class USER_TEMPLATEType106
 
 
-class HISTORY_RECORDSType105(GeneratedsSuper):
+class HISTORY_RECORDSType107(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, HISTORY=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -44520,21 +44851,21 @@
             self.HISTORY = []
         else:
             self.HISTORY = HISTORY
         self.HISTORY_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, HISTORY_RECORDSType105)
+                CurrentSubclassModule_, HISTORY_RECORDSType107)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if HISTORY_RECORDSType105.subclass:
-            return HISTORY_RECORDSType105.subclass(*args_, **kwargs_)
+        if HISTORY_RECORDSType107.subclass:
+            return HISTORY_RECORDSType107.subclass(*args_, **kwargs_)
         else:
-            return HISTORY_RECORDSType105(*args_, **kwargs_)
+            return HISTORY_RECORDSType107(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_HISTORY(self):
         return self.HISTORY
@@ -44549,40 +44880,40 @@
     def _hasContent(self):
         if (
             self.HISTORY
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORY_RECORDSType105', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('HISTORY_RECORDSType105')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORY_RECORDSType107', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('HISTORY_RECORDSType107')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'HISTORY_RECORDSType105':
+        if self.original_tagname_ is not None and name_ == 'HISTORY_RECORDSType107':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORY_RECORDSType105')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORY_RECORDSType107')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORY_RECORDSType105', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORY_RECORDSType107', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORY_RECORDSType105'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORY_RECORDSType107'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORY_RECORDSType105', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORY_RECORDSType107', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for HISTORY_ in self.HISTORY:
             namespaceprefix_ = self.HISTORY_nsprefix_ + ':' if (UseCapturedNS_ and self.HISTORY_nsprefix_) else ''
             HISTORY_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='HISTORY', pretty_print=pretty_print)
@@ -44597,22 +44928,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'HISTORY':
-            obj_ = HISTORYType106.factory(parent_object_=self)
+            obj_ = HISTORYType108.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.HISTORY.append(obj_)
             obj_.original_tagname_ = 'HISTORY'
-# end class HISTORY_RECORDSType105
+# end class HISTORY_RECORDSType107
 
 
-class HISTORYType106(GeneratedsSuper):
+class HISTORYType108(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OID=None, SEQ=None, HOSTNAME=None, HID=None, CID=None, STIME=None, ETIME=None, VM_MAD=None, TM_MAD=None, DS_ID=None, PSTIME=None, PETIME=None, RSTIME=None, RETIME=None, ESTIME=None, EETIME=None, ACTION=None, UID=None, GID=None, REQUEST_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -44657,21 +44988,21 @@
         self.GID = GID
         self.GID_nsprefix_ = None
         self.REQUEST_ID = REQUEST_ID
         self.REQUEST_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, HISTORYType106)
+                CurrentSubclassModule_, HISTORYType108)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if HISTORYType106.subclass:
-            return HISTORYType106.subclass(*args_, **kwargs_)
+        if HISTORYType108.subclass:
+            return HISTORYType108.subclass(*args_, **kwargs_)
         else:
-            return HISTORYType106(*args_, **kwargs_)
+            return HISTORYType108(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OID(self):
         return self.OID
@@ -44775,40 +45106,40 @@
             self.UID is not None or
             self.GID is not None or
             self.REQUEST_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORYType106', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('HISTORYType106')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORYType108', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('HISTORYType108')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'HISTORYType106':
+        if self.original_tagname_ is not None and name_ == 'HISTORYType108':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORYType106')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORYType108')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORYType106', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORYType108', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORYType106'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORYType108'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORYType106', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORYType108', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OID is not None:
             namespaceprefix_ = self.OID_nsprefix_ + ':' if (UseCapturedNS_ and self.OID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -45019,18 +45350,18 @@
             self.GID_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQUEST_ID':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'REQUEST_ID')
             value_ = self.gds_validate_string(value_, node, 'REQUEST_ID')
             self.REQUEST_ID = value_
             self.REQUEST_ID_nsprefix_ = child_.prefix
-# end class HISTORYType106
+# end class HISTORYType108
 
 
-class SNAPSHOTSType107(GeneratedsSuper):
+class SNAPSHOTSType109(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ALLOW_ORPHANS=None, CURRENT_BASE=None, DISK_ID=None, NEXT_SNAPSHOT=None, SNAPSHOT=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -45048,21 +45379,21 @@
             self.SNAPSHOT = []
         else:
             self.SNAPSHOT = SNAPSHOT
         self.SNAPSHOT_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SNAPSHOTSType107)
+                CurrentSubclassModule_, SNAPSHOTSType109)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if SNAPSHOTSType107.subclass:
-            return SNAPSHOTSType107.subclass(*args_, **kwargs_)
+        if SNAPSHOTSType109.subclass:
+            return SNAPSHOTSType109.subclass(*args_, **kwargs_)
         else:
-            return SNAPSHOTSType107(*args_, **kwargs_)
+            return SNAPSHOTSType109(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ALLOW_ORPHANS(self):
         return self.ALLOW_ORPHANS
@@ -45097,40 +45428,40 @@
             self.DISK_ID is not None or
             self.NEXT_SNAPSHOT is not None or
             self.SNAPSHOT
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType107', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTSType107')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType109', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTSType109')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SNAPSHOTSType107':
+        if self.original_tagname_ is not None and name_ == 'SNAPSHOTSType109':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTSType107')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTSType109')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTSType107', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTSType109', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTSType107'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTSType109'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType107', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTSType109', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ALLOW_ORPHANS is not None:
             namespaceprefix_ = self.ALLOW_ORPHANS_nsprefix_ + ':' if (UseCapturedNS_ and self.ALLOW_ORPHANS_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -45185,22 +45516,22 @@
         elif nodeName_ == 'NEXT_SNAPSHOT' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'NEXT_SNAPSHOT')
             ival_ = self.gds_validate_integer(ival_, node, 'NEXT_SNAPSHOT')
             self.NEXT_SNAPSHOT = ival_
             self.NEXT_SNAPSHOT_nsprefix_ = child_.prefix
         elif nodeName_ == 'SNAPSHOT':
-            obj_ = SNAPSHOTType108.factory(parent_object_=self)
+            obj_ = SNAPSHOTType110.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SNAPSHOT.append(obj_)
             obj_.original_tagname_ = 'SNAPSHOT'
-# end class SNAPSHOTSType107
+# end class SNAPSHOTSType109
 
 
-class SNAPSHOTType108(GeneratedsSuper):
+class SNAPSHOTType110(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ACTIVE=None, CHILDREN=None, DATE=None, ID=None, NAME=None, PARENT=None, SIZE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -45219,21 +45550,21 @@
         self.PARENT = PARENT
         self.PARENT_nsprefix_ = None
         self.SIZE = SIZE
         self.SIZE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SNAPSHOTType108)
+                CurrentSubclassModule_, SNAPSHOTType110)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if SNAPSHOTType108.subclass:
-            return SNAPSHOTType108.subclass(*args_, **kwargs_)
+        if SNAPSHOTType110.subclass:
+            return SNAPSHOTType110.subclass(*args_, **kwargs_)
         else:
-            return SNAPSHOTType108(*args_, **kwargs_)
+            return SNAPSHOTType110(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ACTIVE(self):
         return self.ACTIVE
@@ -45272,40 +45603,40 @@
             self.NAME is not None or
             self.PARENT is not None or
             self.SIZE is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType108', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTType108')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType110', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SNAPSHOTType110')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SNAPSHOTType108':
+        if self.original_tagname_ is not None and name_ == 'SNAPSHOTType110':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType108')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType110')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType108', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType110', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType108'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType110'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType108', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SNAPSHOTType110', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ACTIVE is not None:
             namespaceprefix_ = self.ACTIVE_nsprefix_ + ':' if (UseCapturedNS_ and self.ACTIVE_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -45386,18 +45717,18 @@
             self.PARENT_nsprefix_ = child_.prefix
         elif nodeName_ == 'SIZE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'SIZE')
             ival_ = self.gds_validate_integer(ival_, node, 'SIZE')
             self.SIZE = ival_
             self.SIZE_nsprefix_ = child_.prefix
-# end class SNAPSHOTType108
+# end class SNAPSHOTType110
 
 
-class BACKUPSType109(GeneratedsSuper):
+class BACKUPSType111(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, BACKUP_CONFIG=None, BACKUP_IDS=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -45406,21 +45737,21 @@
         self.BACKUP_CONFIG = BACKUP_CONFIG
         self.BACKUP_CONFIG_nsprefix_ = None
         self.BACKUP_IDS = BACKUP_IDS
         self.BACKUP_IDS_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, BACKUPSType109)
+                CurrentSubclassModule_, BACKUPSType111)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if BACKUPSType109.subclass:
-            return BACKUPSType109.subclass(*args_, **kwargs_)
+        if BACKUPSType111.subclass:
+            return BACKUPSType111.subclass(*args_, **kwargs_)
         else:
-            return BACKUPSType109(*args_, **kwargs_)
+            return BACKUPSType111(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_BACKUP_CONFIG(self):
         return self.BACKUP_CONFIG
@@ -45434,40 +45765,40 @@
         if (
             self.BACKUP_CONFIG is not None or
             self.BACKUP_IDS is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUPSType109', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('BACKUPSType109')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUPSType111', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('BACKUPSType111')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'BACKUPSType109':
+        if self.original_tagname_ is not None and name_ == 'BACKUPSType111':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUPSType109')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUPSType111')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUPSType109', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUPSType111', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUPSType109'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUPSType111'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUPSType109', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUPSType111', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.BACKUP_CONFIG is not None:
             namespaceprefix_ = self.BACKUP_CONFIG_nsprefix_ + ':' if (UseCapturedNS_ and self.BACKUP_CONFIG_nsprefix_) else ''
             self.BACKUP_CONFIG.export(outfile, level, namespaceprefix_, namespacedef_='', name_='BACKUP_CONFIG', pretty_print=pretty_print)
@@ -45485,27 +45816,27 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'BACKUP_CONFIG':
-            obj_ = BACKUP_CONFIGType110.factory(parent_object_=self)
+            obj_ = BACKUP_CONFIGType112.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.BACKUP_CONFIG = obj_
             obj_.original_tagname_ = 'BACKUP_CONFIG'
         elif nodeName_ == 'BACKUP_IDS':
-            obj_ = BACKUP_IDSType111.factory(parent_object_=self)
+            obj_ = BACKUP_IDSType113.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.BACKUP_IDS = obj_
             obj_.original_tagname_ = 'BACKUP_IDS'
-# end class BACKUPSType109
+# end class BACKUPSType111
 
 
-class BACKUP_CONFIGType110(GeneratedsSuper):
+class BACKUP_CONFIGType112(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, BACKUP_VOLATILE=None, FS_FREEZE=None, INCREMENTAL_BACKUP_ID=None, KEEP_LAST=None, LAST_BACKUP_ID=None, LAST_BACKUP_SIZE=None, LAST_DATASTORE_ID=None, LAST_INCREMENT_ID=None, MODE=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -45528,21 +45859,21 @@
         self.LAST_INCREMENT_ID = LAST_INCREMENT_ID
         self.LAST_INCREMENT_ID_nsprefix_ = None
         self.MODE = MODE
         self.MODE_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, BACKUP_CONFIGType110)
+                CurrentSubclassModule_, BACKUP_CONFIGType112)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if BACKUP_CONFIGType110.subclass:
-            return BACKUP_CONFIGType110.subclass(*args_, **kwargs_)
+        if BACKUP_CONFIGType112.subclass:
+            return BACKUP_CONFIGType112.subclass(*args_, **kwargs_)
         else:
-            return BACKUP_CONFIGType110(*args_, **kwargs_)
+            return BACKUP_CONFIGType112(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_BACKUP_VOLATILE(self):
         return self.BACKUP_VOLATILE
@@ -45591,40 +45922,40 @@
             self.LAST_DATASTORE_ID is not None or
             self.LAST_INCREMENT_ID is not None or
             self.MODE is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_CONFIGType110', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('BACKUP_CONFIGType110')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_CONFIGType112', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('BACKUP_CONFIGType112')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'BACKUP_CONFIGType110':
+        if self.original_tagname_ is not None and name_ == 'BACKUP_CONFIGType112':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_CONFIGType110')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_CONFIGType112')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_CONFIGType110', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_CONFIGType112', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_CONFIGType110'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_CONFIGType112'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_CONFIGType110', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_CONFIGType112', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.BACKUP_VOLATILE is not None:
             namespaceprefix_ = self.BACKUP_VOLATILE_nsprefix_ + ':' if (UseCapturedNS_ and self.BACKUP_VOLATILE_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -45725,18 +46056,18 @@
             self.LAST_INCREMENT_ID_nsprefix_ = child_.prefix
         elif nodeName_ == 'MODE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'MODE')
             value_ = self.gds_validate_string(value_, node, 'MODE')
             self.MODE = value_
             self.MODE_nsprefix_ = child_.prefix
-# end class BACKUP_CONFIGType110
+# end class BACKUP_CONFIGType112
 
 
-class BACKUP_IDSType111(GeneratedsSuper):
+class BACKUP_IDSType113(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -45746,21 +46077,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, BACKUP_IDSType111)
+                CurrentSubclassModule_, BACKUP_IDSType113)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if BACKUP_IDSType111.subclass:
-            return BACKUP_IDSType111.subclass(*args_, **kwargs_)
+        if BACKUP_IDSType113.subclass:
+            return BACKUP_IDSType113.subclass(*args_, **kwargs_)
         else:
-            return BACKUP_IDSType111(*args_, **kwargs_)
+            return BACKUP_IDSType113(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -45775,40 +46106,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_IDSType111', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('BACKUP_IDSType111')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_IDSType113', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('BACKUP_IDSType113')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'BACKUP_IDSType111':
+        if self.original_tagname_ is not None and name_ == 'BACKUP_IDSType113':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_IDSType111')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_IDSType113')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_IDSType111', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_IDSType113', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_IDSType111'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_IDSType113'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_IDSType111', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_IDSType113', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -45829,18 +46160,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'ID')
             value_ = self.gds_validate_string(value_, node, 'ID')
             self.ID.append(value_)
             self.ID_nsprefix_ = child_.prefix
-# end class BACKUP_IDSType111
+# end class BACKUP_IDSType113
 
 
-class VNETType112(GeneratedsSuper):
+class VNETType114(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, UID=None, GID=None, UNAME=None, GNAME=None, NAME=None, PERMISSIONS=None, CLUSTERS=None, BRIDGE=None, BRIDGE_TYPE=None, STATE=None, PREV_STATE=None, PARENT_NETWORK_ID=None, VN_MAD=None, PHYDEV=None, VLAN_ID=None, OUTER_VLAN_ID=None, VLAN_ID_AUTOMATIC=None, OUTER_VLAN_ID_AUTOMATIC=None, USED_LEASES=None, VROUTERS=None, UPDATED_VMS=None, OUTDATED_VMS=None, UPDATING_VMS=None, ERROR_VMS=None, TEMPLATE=None, AR_POOL=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -45899,21 +46230,21 @@
         self.TEMPLATE = TEMPLATE
         self.TEMPLATE_nsprefix_ = None
         self.AR_POOL = AR_POOL
         self.AR_POOL_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VNETType112)
+                CurrentSubclassModule_, VNETType114)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VNETType112.subclass:
-            return VNETType112.subclass(*args_, **kwargs_)
+        if VNETType114.subclass:
+            return VNETType114.subclass(*args_, **kwargs_)
         else:
-            return VNETType112(*args_, **kwargs_)
+            return VNETType114(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -46052,40 +46383,40 @@
             self.ERROR_VMS is not None or
             self.TEMPLATE is not None or
             self.AR_POOL is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETType112', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VNETType112')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETType114', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VNETType114')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VNETType112':
+        if self.original_tagname_ is not None and name_ == 'VNETType114':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETType112')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETType114')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETType112', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETType114', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETType112'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETType114'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETType112', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETType114', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ID is not None:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -46233,20 +46564,20 @@
         elif nodeName_ == 'NAME':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
         elif nodeName_ == 'PERMISSIONS':
-            obj_ = PERMISSIONSType113.factory(parent_object_=self)
+            obj_ = PERMISSIONSType115.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.PERMISSIONS = obj_
             obj_.original_tagname_ = 'PERMISSIONS'
         elif nodeName_ == 'CLUSTERS':
-            obj_ = CLUSTERSType114.factory(parent_object_=self)
+            obj_ = CLUSTERSType116.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.CLUSTERS = obj_
             obj_.original_tagname_ = 'CLUSTERS'
         elif nodeName_ == 'BRIDGE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'BRIDGE')
             value_ = self.gds_validate_string(value_, node, 'BRIDGE')
@@ -46320,48 +46651,48 @@
             self.USED_LEASES_nsprefix_ = child_.prefix
         elif nodeName_ == 'VROUTERS':
             obj_ = VROUTERSType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.VROUTERS = obj_
             obj_.original_tagname_ = 'VROUTERS'
         elif nodeName_ == 'UPDATED_VMS':
-            obj_ = UPDATED_VMSType115.factory(parent_object_=self)
+            obj_ = UPDATED_VMSType117.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.UPDATED_VMS = obj_
             obj_.original_tagname_ = 'UPDATED_VMS'
         elif nodeName_ == 'OUTDATED_VMS':
-            obj_ = OUTDATED_VMSType116.factory(parent_object_=self)
+            obj_ = OUTDATED_VMSType118.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.OUTDATED_VMS = obj_
             obj_.original_tagname_ = 'OUTDATED_VMS'
         elif nodeName_ == 'UPDATING_VMS':
-            obj_ = UPDATING_VMSType117.factory(parent_object_=self)
+            obj_ = UPDATING_VMSType119.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.UPDATING_VMS = obj_
             obj_.original_tagname_ = 'UPDATING_VMS'
         elif nodeName_ == 'ERROR_VMS':
-            obj_ = ERROR_VMSType118.factory(parent_object_=self)
+            obj_ = ERROR_VMSType120.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.ERROR_VMS = obj_
             obj_.original_tagname_ = 'ERROR_VMS'
         elif nodeName_ == 'TEMPLATE':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'TEMPLATE')
             value_ = self.gds_validate_string(value_, node, 'TEMPLATE')
             self.TEMPLATE = value_
             self.TEMPLATE_nsprefix_ = child_.prefix
         elif nodeName_ == 'AR_POOL':
             obj_ = AR_POOLType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.AR_POOL = obj_
             obj_.original_tagname_ = 'AR_POOL'
-# end class VNETType112
+# end class VNETType114
 
 
-class PERMISSIONSType113(GeneratedsSuper):
+class PERMISSIONSType115(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -46384,21 +46715,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType113)
+                CurrentSubclassModule_, PERMISSIONSType115)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType113.subclass:
-            return PERMISSIONSType113.subclass(*args_, **kwargs_)
+        if PERMISSIONSType115.subclass:
+            return PERMISSIONSType115.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType113(*args_, **kwargs_)
+            return PERMISSIONSType115(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -46447,40 +46778,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType113', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType113')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType115', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType115')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType113':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType115':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType113')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType115')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType113', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType115', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType113'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType115'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType113', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType115', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -46581,18 +46912,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType113
+# end class PERMISSIONSType115
 
 
-class CLUSTERSType114(GeneratedsSuper):
+class CLUSTERSType116(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -46602,21 +46933,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, CLUSTERSType114)
+                CurrentSubclassModule_, CLUSTERSType116)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if CLUSTERSType114.subclass:
-            return CLUSTERSType114.subclass(*args_, **kwargs_)
+        if CLUSTERSType116.subclass:
+            return CLUSTERSType116.subclass(*args_, **kwargs_)
         else:
-            return CLUSTERSType114(*args_, **kwargs_)
+            return CLUSTERSType116(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -46631,40 +46962,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType114', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('CLUSTERSType114')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType116', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('CLUSTERSType116')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'CLUSTERSType114':
+        if self.original_tagname_ is not None and name_ == 'CLUSTERSType116':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType114')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType116')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType114', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType116', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType114'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType116'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType114', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType116', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -46685,15 +47016,15 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class CLUSTERSType114
+# end class CLUSTERSType116
 
 
 class VROUTERSType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
@@ -46792,15 +47123,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
 # end class VROUTERSType
 
 
-class UPDATED_VMSType115(GeneratedsSuper):
+class UPDATED_VMSType117(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -46810,21 +47141,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, UPDATED_VMSType115)
+                CurrentSubclassModule_, UPDATED_VMSType117)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if UPDATED_VMSType115.subclass:
-            return UPDATED_VMSType115.subclass(*args_, **kwargs_)
+        if UPDATED_VMSType117.subclass:
+            return UPDATED_VMSType117.subclass(*args_, **kwargs_)
         else:
-            return UPDATED_VMSType115(*args_, **kwargs_)
+            return UPDATED_VMSType117(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -46839,40 +47170,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType115', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATED_VMSType115')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType117', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATED_VMSType117')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'UPDATED_VMSType115':
+        if self.original_tagname_ is not None and name_ == 'UPDATED_VMSType117':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATED_VMSType115')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATED_VMSType117')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATED_VMSType115', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATED_VMSType117', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATED_VMSType115'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATED_VMSType117'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType115', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType117', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -46893,18 +47224,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class UPDATED_VMSType115
+# end class UPDATED_VMSType117
 
 
-class OUTDATED_VMSType116(GeneratedsSuper):
+class OUTDATED_VMSType118(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -46914,21 +47245,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, OUTDATED_VMSType116)
+                CurrentSubclassModule_, OUTDATED_VMSType118)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if OUTDATED_VMSType116.subclass:
-            return OUTDATED_VMSType116.subclass(*args_, **kwargs_)
+        if OUTDATED_VMSType118.subclass:
+            return OUTDATED_VMSType118.subclass(*args_, **kwargs_)
         else:
-            return OUTDATED_VMSType116(*args_, **kwargs_)
+            return OUTDATED_VMSType118(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -46943,40 +47274,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType116', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('OUTDATED_VMSType116')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType118', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('OUTDATED_VMSType118')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'OUTDATED_VMSType116':
+        if self.original_tagname_ is not None and name_ == 'OUTDATED_VMSType118':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OUTDATED_VMSType116')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OUTDATED_VMSType118')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OUTDATED_VMSType116', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OUTDATED_VMSType118', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OUTDATED_VMSType116'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OUTDATED_VMSType118'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType116', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType118', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -46997,18 +47328,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class OUTDATED_VMSType116
+# end class OUTDATED_VMSType118
 
 
-class UPDATING_VMSType117(GeneratedsSuper):
+class UPDATING_VMSType119(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -47018,21 +47349,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, UPDATING_VMSType117)
+                CurrentSubclassModule_, UPDATING_VMSType119)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if UPDATING_VMSType117.subclass:
-            return UPDATING_VMSType117.subclass(*args_, **kwargs_)
+        if UPDATING_VMSType119.subclass:
+            return UPDATING_VMSType119.subclass(*args_, **kwargs_)
         else:
-            return UPDATING_VMSType117(*args_, **kwargs_)
+            return UPDATING_VMSType119(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -47047,40 +47378,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType117', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATING_VMSType117')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType119', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATING_VMSType119')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'UPDATING_VMSType117':
+        if self.original_tagname_ is not None and name_ == 'UPDATING_VMSType119':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATING_VMSType117')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATING_VMSType119')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATING_VMSType117', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATING_VMSType119', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATING_VMSType117'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATING_VMSType119'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType117', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType119', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -47101,18 +47432,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class UPDATING_VMSType117
+# end class UPDATING_VMSType119
 
 
-class ERROR_VMSType118(GeneratedsSuper):
+class ERROR_VMSType120(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -47122,21 +47453,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ERROR_VMSType118)
+                CurrentSubclassModule_, ERROR_VMSType120)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if ERROR_VMSType118.subclass:
-            return ERROR_VMSType118.subclass(*args_, **kwargs_)
+        if ERROR_VMSType120.subclass:
+            return ERROR_VMSType120.subclass(*args_, **kwargs_)
         else:
-            return ERROR_VMSType118(*args_, **kwargs_)
+            return ERROR_VMSType120(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -47151,40 +47482,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType118', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ERROR_VMSType118')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType120', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ERROR_VMSType120')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ERROR_VMSType118':
+        if self.original_tagname_ is not None and name_ == 'ERROR_VMSType120':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ERROR_VMSType118')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ERROR_VMSType120')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ERROR_VMSType118', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ERROR_VMSType120', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ERROR_VMSType118'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ERROR_VMSType120'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType118', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType120', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -47205,15 +47536,15 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class ERROR_VMSType118
+# end class ERROR_VMSType120
 
 
 class AR_POOLType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, AR=None, gds_collector_=None, **kwargs_):
@@ -47558,15 +47889,15 @@
             value_ = self.gds_parse_string(value_, node, 'VN_MAD')
             value_ = self.gds_validate_string(value_, node, 'VN_MAD')
             self.VN_MAD = value_
             self.VN_MAD_nsprefix_ = child_.prefix
 # end class ARType
 
 
-class LOCKType119(GeneratedsSuper):
+class LOCKType121(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -47579,21 +47910,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType119)
+                CurrentSubclassModule_, LOCKType121)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType119.subclass:
-            return LOCKType119.subclass(*args_, **kwargs_)
+        if LOCKType121.subclass:
+            return LOCKType121.subclass(*args_, **kwargs_)
         else:
-            return LOCKType119(*args_, **kwargs_)
+            return LOCKType121(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -47617,40 +47948,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType119', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType119')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType121', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType121')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType119':
+        if self.original_tagname_ is not None and name_ == 'LOCKType121':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType119')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType121')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType119', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType121', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType119'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType121'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType119', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType121', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -47701,18 +48032,18 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType119
+# end class LOCKType121
 
 
-class PERMISSIONSType120(GeneratedsSuper):
+class PERMISSIONSType122(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -47735,21 +48066,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType120)
+                CurrentSubclassModule_, PERMISSIONSType122)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType120.subclass:
-            return PERMISSIONSType120.subclass(*args_, **kwargs_)
+        if PERMISSIONSType122.subclass:
+            return PERMISSIONSType122.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType120(*args_, **kwargs_)
+            return PERMISSIONSType122(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -47798,40 +48129,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType120', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType120')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType122', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType122')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType120':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType122':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType120')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType122')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType120', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType122', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType120'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType122'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType120', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType122', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -47932,18 +48263,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType120
+# end class PERMISSIONSType122
 
 
-class CLUSTERSType121(GeneratedsSuper):
+class CLUSTERSType123(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -47953,21 +48284,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, CLUSTERSType121)
+                CurrentSubclassModule_, CLUSTERSType123)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if CLUSTERSType121.subclass:
-            return CLUSTERSType121.subclass(*args_, **kwargs_)
+        if CLUSTERSType123.subclass:
+            return CLUSTERSType123.subclass(*args_, **kwargs_)
         else:
-            return CLUSTERSType121(*args_, **kwargs_)
+            return CLUSTERSType123(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -47982,40 +48313,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType121', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('CLUSTERSType121')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType123', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('CLUSTERSType123')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'CLUSTERSType121':
+        if self.original_tagname_ is not None and name_ == 'CLUSTERSType123':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType121')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType123')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType121', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType123', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType121'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType123'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType121', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType123', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -48036,18 +48367,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class CLUSTERSType121
+# end class CLUSTERSType123
 
 
-class VROUTERSType122(GeneratedsSuper):
+class VROUTERSType124(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -48057,21 +48388,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VROUTERSType122)
+                CurrentSubclassModule_, VROUTERSType124)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VROUTERSType122.subclass:
-            return VROUTERSType122.subclass(*args_, **kwargs_)
+        if VROUTERSType124.subclass:
+            return VROUTERSType124.subclass(*args_, **kwargs_)
         else:
-            return VROUTERSType122(*args_, **kwargs_)
+            return VROUTERSType124(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -48086,40 +48417,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VROUTERSType122', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VROUTERSType122')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VROUTERSType124', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VROUTERSType124')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VROUTERSType122':
+        if self.original_tagname_ is not None and name_ == 'VROUTERSType124':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VROUTERSType122')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VROUTERSType124')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VROUTERSType122', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VROUTERSType124', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VROUTERSType122'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VROUTERSType124'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VROUTERSType122', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VROUTERSType124', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -48140,18 +48471,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class VROUTERSType122
+# end class VROUTERSType124
 
 
-class UPDATED_VMSType123(GeneratedsSuper):
+class UPDATED_VMSType125(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -48161,21 +48492,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, UPDATED_VMSType123)
+                CurrentSubclassModule_, UPDATED_VMSType125)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if UPDATED_VMSType123.subclass:
-            return UPDATED_VMSType123.subclass(*args_, **kwargs_)
+        if UPDATED_VMSType125.subclass:
+            return UPDATED_VMSType125.subclass(*args_, **kwargs_)
         else:
-            return UPDATED_VMSType123(*args_, **kwargs_)
+            return UPDATED_VMSType125(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -48190,40 +48521,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType123', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATED_VMSType123')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType125', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATED_VMSType125')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'UPDATED_VMSType123':
+        if self.original_tagname_ is not None and name_ == 'UPDATED_VMSType125':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATED_VMSType123')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATED_VMSType125')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATED_VMSType123', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATED_VMSType125', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATED_VMSType123'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATED_VMSType125'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType123', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType125', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -48244,18 +48575,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class UPDATED_VMSType123
+# end class UPDATED_VMSType125
 
 
-class OUTDATED_VMSType124(GeneratedsSuper):
+class OUTDATED_VMSType126(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -48265,21 +48596,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, OUTDATED_VMSType124)
+                CurrentSubclassModule_, OUTDATED_VMSType126)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if OUTDATED_VMSType124.subclass:
-            return OUTDATED_VMSType124.subclass(*args_, **kwargs_)
+        if OUTDATED_VMSType126.subclass:
+            return OUTDATED_VMSType126.subclass(*args_, **kwargs_)
         else:
-            return OUTDATED_VMSType124(*args_, **kwargs_)
+            return OUTDATED_VMSType126(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -48294,40 +48625,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType124', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('OUTDATED_VMSType124')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType126', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('OUTDATED_VMSType126')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'OUTDATED_VMSType124':
+        if self.original_tagname_ is not None and name_ == 'OUTDATED_VMSType126':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OUTDATED_VMSType124')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OUTDATED_VMSType126')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OUTDATED_VMSType124', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OUTDATED_VMSType126', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OUTDATED_VMSType124'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OUTDATED_VMSType126'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType124', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType126', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -48348,18 +48679,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class OUTDATED_VMSType124
+# end class OUTDATED_VMSType126
 
 
-class UPDATING_VMSType125(GeneratedsSuper):
+class UPDATING_VMSType127(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -48369,21 +48700,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, UPDATING_VMSType125)
+                CurrentSubclassModule_, UPDATING_VMSType127)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if UPDATING_VMSType125.subclass:
-            return UPDATING_VMSType125.subclass(*args_, **kwargs_)
+        if UPDATING_VMSType127.subclass:
+            return UPDATING_VMSType127.subclass(*args_, **kwargs_)
         else:
-            return UPDATING_VMSType125(*args_, **kwargs_)
+            return UPDATING_VMSType127(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -48398,40 +48729,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType125', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATING_VMSType125')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType127', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('UPDATING_VMSType127')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'UPDATING_VMSType125':
+        if self.original_tagname_ is not None and name_ == 'UPDATING_VMSType127':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATING_VMSType125')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATING_VMSType127')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATING_VMSType125', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATING_VMSType127', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATING_VMSType125'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATING_VMSType127'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType125', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType127', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -48452,18 +48783,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class UPDATING_VMSType125
+# end class UPDATING_VMSType127
 
 
-class ERROR_VMSType126(GeneratedsSuper):
+class ERROR_VMSType128(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -48473,21 +48804,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ERROR_VMSType126)
+                CurrentSubclassModule_, ERROR_VMSType128)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if ERROR_VMSType126.subclass:
-            return ERROR_VMSType126.subclass(*args_, **kwargs_)
+        if ERROR_VMSType128.subclass:
+            return ERROR_VMSType128.subclass(*args_, **kwargs_)
         else:
-            return ERROR_VMSType126(*args_, **kwargs_)
+            return ERROR_VMSType128(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -48502,40 +48833,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType126', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ERROR_VMSType126')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType128', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ERROR_VMSType128')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ERROR_VMSType126':
+        if self.original_tagname_ is not None and name_ == 'ERROR_VMSType128':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ERROR_VMSType126')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ERROR_VMSType128')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ERROR_VMSType126', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ERROR_VMSType128', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ERROR_VMSType126'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ERROR_VMSType128'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType126', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType128', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -48556,18 +48887,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class ERROR_VMSType126
+# end class ERROR_VMSType128
 
 
-class TEMPLATEType127(GeneratedsSuper):
+class TEMPLATEType129(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, DNS=None, GATEWAY=None, GATEWAY6=None, GUEST_MTU=None, IP6_METHOD=None, IP6_METRIC=None, METHOD=None, METRIC=None, NETWORK_ADDRESS=None, NETWORK_MASK=None, SEARCH_DOMAIN=None, VCENTER_FROM_WILD=None, VCENTER_INSTANCE_ID=None, VCENTER_NET_REF=None, VCENTER_PORTGROUP_TYPE=None, VCENTER_TEMPLATE_REF=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -48608,21 +48939,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType127)
+                CurrentSubclassModule_, TEMPLATEType129)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType127.subclass:
-            return TEMPLATEType127.subclass(*args_, **kwargs_)
+        if TEMPLATEType129.subclass:
+            return TEMPLATEType129.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType127(*args_, **kwargs_)
+            return TEMPLATEType129(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_DNS(self):
         return self.DNS
@@ -48711,40 +49042,40 @@
             self.VCENTER_PORTGROUP_TYPE is not None or
             self.VCENTER_TEMPLATE_REF is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType127', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType127')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType129', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType129')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType127':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType129':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType127')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType129')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType127', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType129', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType127'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType129'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType127', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType129', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.DNS is not None:
             namespaceprefix_ = self.DNS_nsprefix_ + ':' if (UseCapturedNS_ and self.DNS_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -48921,20 +49252,20 @@
         elif nodeName_ == 'VCENTER_TEMPLATE_REF':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VCENTER_TEMPLATE_REF')
             value_ = self.gds_validate_string(value_, node, 'VCENTER_TEMPLATE_REF')
             self.VCENTER_TEMPLATE_REF = value_
             self.VCENTER_TEMPLATE_REF_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'TEMPLATEType127')
+            content_ = self.gds_build_any(child_, 'TEMPLATEType129')
             self.anytypeobjs_.append(content_)
-# end class TEMPLATEType127
+# end class TEMPLATEType129
 
 
-class AR_POOLType128(GeneratedsSuper):
+class AR_POOLType130(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, AR=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -48944,21 +49275,21 @@
             self.AR = []
         else:
             self.AR = AR
         self.AR_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, AR_POOLType128)
+                CurrentSubclassModule_, AR_POOLType130)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if AR_POOLType128.subclass:
-            return AR_POOLType128.subclass(*args_, **kwargs_)
+        if AR_POOLType130.subclass:
+            return AR_POOLType130.subclass(*args_, **kwargs_)
         else:
-            return AR_POOLType128(*args_, **kwargs_)
+            return AR_POOLType130(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_AR(self):
         return self.AR
@@ -48973,40 +49304,40 @@
     def _hasContent(self):
         if (
             self.AR
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='AR_POOLType128', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('AR_POOLType128')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='AR_POOLType130', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('AR_POOLType130')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'AR_POOLType128':
+        if self.original_tagname_ is not None and name_ == 'AR_POOLType130':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AR_POOLType128')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AR_POOLType130')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AR_POOLType128', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AR_POOLType130', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AR_POOLType128'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AR_POOLType130'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='AR_POOLType128', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='AR_POOLType130', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for AR_ in self.AR:
             namespaceprefix_ = self.AR_nsprefix_ + ':' if (UseCapturedNS_ and self.AR_nsprefix_) else ''
             AR_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='AR', pretty_print=pretty_print)
@@ -49021,22 +49352,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'AR':
-            obj_ = ARType129.factory(parent_object_=self)
+            obj_ = ARType131.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.AR.append(obj_)
             obj_.original_tagname_ = 'AR'
-# end class AR_POOLType128
+# end class AR_POOLType130
 
 
-class ARType129(GeneratedsSuper):
+class ARType131(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, AR_ID=None, GLOBAL_PREFIX=None, IP=None, MAC=None, PARENT_NETWORK_AR_ID=None, SIZE=None, TYPE=None, ULA_PREFIX=None, VN_MAD=None, MAC_END=None, IP_END=None, IP6_ULA=None, IP6_ULA_END=None, IP6_GLOBAL=None, IP6_GLOBAL_END=None, IP6=None, IP6_END=None, PORT_START=None, PORT_SIZE=None, USED_LEASES=None, LEASES=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -49083,21 +49414,21 @@
         self.USED_LEASES = USED_LEASES
         self.USED_LEASES_nsprefix_ = None
         self.LEASES = LEASES
         self.LEASES_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, ARType129)
+                CurrentSubclassModule_, ARType131)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if ARType129.subclass:
-            return ARType129.subclass(*args_, **kwargs_)
+        if ARType131.subclass:
+            return ARType131.subclass(*args_, **kwargs_)
         else:
-            return ARType129(*args_, **kwargs_)
+            return ARType131(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_AR_ID(self):
         return self.AR_ID
@@ -49206,40 +49537,40 @@
             self.PORT_SIZE is not None or
             self.USED_LEASES is not None or
             self.LEASES is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ARType129', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ARType129')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ARType131', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('ARType131')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'ARType129':
+        if self.original_tagname_ is not None and name_ == 'ARType131':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ARType129')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ARType131')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ARType129', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ARType131', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ARType129'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ARType131'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ARType129', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ARType131', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.AR_ID is not None:
             namespaceprefix_ = self.AR_ID_nsprefix_ + ':' if (UseCapturedNS_ and self.AR_ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -49458,15 +49789,15 @@
             self.USED_LEASES = value_
             self.USED_LEASES_nsprefix_ = child_.prefix
         elif nodeName_ == 'LEASES':
             obj_ = LEASESType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.LEASES = obj_
             obj_.original_tagname_ = 'LEASES'
-# end class ARType129
+# end class ARType131
 
 
 class LEASESType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LEASE=None, gds_collector_=None, **kwargs_):
@@ -49794,15 +50125,15 @@
             ival_ = self.gds_parse_integer(sval_, node, 'VROUTER')
             ival_ = self.gds_validate_integer(ival_, node, 'VROUTER')
             self.VROUTER = ival_
             self.VROUTER_nsprefix_ = child_.prefix
 # end class LEASEType
 
 
-class LOCKType130(GeneratedsSuper):
+class LOCKType132(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -49815,21 +50146,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType130)
+                CurrentSubclassModule_, LOCKType132)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType130.subclass:
-            return LOCKType130.subclass(*args_, **kwargs_)
+        if LOCKType132.subclass:
+            return LOCKType132.subclass(*args_, **kwargs_)
         else:
-            return LOCKType130(*args_, **kwargs_)
+            return LOCKType132(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -49853,40 +50184,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType130', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType130')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType132', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType132')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType130':
+        if self.original_tagname_ is not None and name_ == 'LOCKType132':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType130')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType132')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType130', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType132', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType130'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType132'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType130', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType132', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -49937,18 +50268,18 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType130
+# end class LOCKType132
 
 
-class PERMISSIONSType131(GeneratedsSuper):
+class PERMISSIONSType133(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -49971,21 +50302,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType131)
+                CurrentSubclassModule_, PERMISSIONSType133)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType131.subclass:
-            return PERMISSIONSType131.subclass(*args_, **kwargs_)
+        if PERMISSIONSType133.subclass:
+            return PERMISSIONSType133.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType131(*args_, **kwargs_)
+            return PERMISSIONSType133(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -50034,40 +50365,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType131', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType131')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType133', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType133')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType131':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType133':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType131')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType133')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType131', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType133', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType131'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType133'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType131', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType133', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -50168,18 +50499,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType131
+# end class PERMISSIONSType133
 
 
-class TEMPLATEType132(GeneratedsSuper):
+class TEMPLATEType134(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, VN_MAD=None, anytypeobjs_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -50190,21 +50521,21 @@
         if anytypeobjs_ is None:
             self.anytypeobjs_ = []
         else:
             self.anytypeobjs_ = anytypeobjs_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType132)
+                CurrentSubclassModule_, TEMPLATEType134)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType132.subclass:
-            return TEMPLATEType132.subclass(*args_, **kwargs_)
+        if TEMPLATEType134.subclass:
+            return TEMPLATEType134.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType132(*args_, **kwargs_)
+            return TEMPLATEType134(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VN_MAD(self):
         return self.VN_MAD
@@ -50218,40 +50549,40 @@
         if (
             self.VN_MAD is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType132', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType132')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType134', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType134')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType132':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType134':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType132')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType134')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType132', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType134', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType132'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType134'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType132', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType134', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.VN_MAD is not None:
             namespaceprefix_ = self.VN_MAD_nsprefix_ + ':' if (UseCapturedNS_ and self.VN_MAD_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -50278,20 +50609,20 @@
         if nodeName_ == 'VN_MAD':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'VN_MAD')
             value_ = self.gds_validate_string(value_, node, 'VN_MAD')
             self.VN_MAD = value_
             self.VN_MAD_nsprefix_ = child_.prefix
         else:
-            content_ = self.gds_build_any(child_, 'TEMPLATEType132')
+            content_ = self.gds_build_any(child_, 'TEMPLATEType134')
             self.anytypeobjs_.append(content_)
-# end class TEMPLATEType132
+# end class TEMPLATEType134
 
 
-class PERMISSIONSType133(GeneratedsSuper):
+class PERMISSIONSType135(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, OWNER_U=None, OWNER_M=None, OWNER_A=None, GROUP_U=None, GROUP_M=None, GROUP_A=None, OTHER_U=None, OTHER_M=None, OTHER_A=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -50314,21 +50645,21 @@
         self.OTHER_M = OTHER_M
         self.OTHER_M_nsprefix_ = None
         self.OTHER_A = OTHER_A
         self.OTHER_A_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, PERMISSIONSType133)
+                CurrentSubclassModule_, PERMISSIONSType135)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if PERMISSIONSType133.subclass:
-            return PERMISSIONSType133.subclass(*args_, **kwargs_)
+        if PERMISSIONSType135.subclass:
+            return PERMISSIONSType135.subclass(*args_, **kwargs_)
         else:
-            return PERMISSIONSType133(*args_, **kwargs_)
+            return PERMISSIONSType135(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_OWNER_U(self):
         return self.OWNER_U
@@ -50377,40 +50708,40 @@
             self.OTHER_U is not None or
             self.OTHER_M is not None or
             self.OTHER_A is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType133', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType133')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType135', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('PERMISSIONSType135')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType133':
+        if self.original_tagname_ is not None and name_ == 'PERMISSIONSType135':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType133')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType135')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType133', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType135', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType133'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType135'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType133', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PERMISSIONSType135', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.OWNER_U is not None:
             namespaceprefix_ = self.OWNER_U_nsprefix_ + ':' if (UseCapturedNS_ and self.OWNER_U_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -50511,18 +50842,18 @@
             self.OTHER_M_nsprefix_ = child_.prefix
         elif nodeName_ == 'OTHER_A' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'OTHER_A')
             ival_ = self.gds_validate_integer(ival_, node, 'OTHER_A')
             self.OTHER_A = ival_
             self.OTHER_A_nsprefix_ = child_.prefix
-# end class PERMISSIONSType133
+# end class PERMISSIONSType135
 
 
-class LOCKType134(GeneratedsSuper):
+class LOCKType136(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, LOCKED=None, OWNER=None, TIME=None, REQ_ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -50535,21 +50866,21 @@
         self.TIME = TIME
         self.TIME_nsprefix_ = None
         self.REQ_ID = REQ_ID
         self.REQ_ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, LOCKType134)
+                CurrentSubclassModule_, LOCKType136)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if LOCKType134.subclass:
-            return LOCKType134.subclass(*args_, **kwargs_)
+        if LOCKType136.subclass:
+            return LOCKType136.subclass(*args_, **kwargs_)
         else:
-            return LOCKType134(*args_, **kwargs_)
+            return LOCKType136(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOCKED(self):
         return self.LOCKED
@@ -50573,40 +50904,40 @@
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType134', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType134')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType136', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('LOCKType136')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'LOCKType134':
+        if self.original_tagname_ is not None and name_ == 'LOCKType136':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType134')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType136')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType134', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType136', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType134'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType136'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType134', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LOCKType136', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.LOCKED is not None:
             namespaceprefix_ = self.LOCKED_nsprefix_ + ':' if (UseCapturedNS_ and self.LOCKED_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -50657,18 +50988,18 @@
             self.TIME_nsprefix_ = child_.prefix
         elif nodeName_ == 'REQ_ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'REQ_ID')
             ival_ = self.gds_validate_integer(ival_, node, 'REQ_ID')
             self.REQ_ID = ival_
             self.REQ_ID_nsprefix_ = child_.prefix
-# end class LOCKType134
+# end class LOCKType136
 
 
-class VMSType135(GeneratedsSuper):
+class VMSType137(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -50678,21 +51009,21 @@
             self.ID = []
         else:
             self.ID = ID
         self.ID_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, VMSType135)
+                CurrentSubclassModule_, VMSType137)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if VMSType135.subclass:
-            return VMSType135.subclass(*args_, **kwargs_)
+        if VMSType137.subclass:
+            return VMSType137.subclass(*args_, **kwargs_)
         else:
-            return VMSType135(*args_, **kwargs_)
+            return VMSType137(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ID(self):
         return self.ID
@@ -50707,40 +51038,40 @@
     def _hasContent(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType135', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMSType135')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType137', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('VMSType137')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'VMSType135':
+        if self.original_tagname_ is not None and name_ == 'VMSType137':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMSType135')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMSType137')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMSType135', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMSType137', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMSType135'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMSType137'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType135', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType137', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for ID_ in self.ID:
             namespaceprefix_ = self.ID_nsprefix_ + ':' if (UseCapturedNS_ and self.ID_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -50761,15 +51092,15 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ID' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'ID')
             ival_ = self.gds_validate_integer(ival_, node, 'ID')
             self.ID.append(ival_)
             self.ID_nsprefix_ = child_.prefix
-# end class VMSType135
+# end class VMSType137
 
 
 class ZONEType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ID=None, NAME=None, STATE=None, TEMPLATE=None, SERVER_POOL=None, gds_collector_=None, **kwargs_):
@@ -50911,48 +51242,48 @@
         elif nodeName_ == 'STATE' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'STATE')
             ival_ = self.gds_validate_integer(ival_, node, 'STATE')
             self.STATE = ival_
             self.STATE_nsprefix_ = child_.prefix
         elif nodeName_ == 'TEMPLATE':
-            obj_ = TEMPLATEType136.factory(parent_object_=self)
+            obj_ = TEMPLATEType138.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TEMPLATE = obj_
             obj_.original_tagname_ = 'TEMPLATE'
         elif nodeName_ == 'SERVER_POOL':
             obj_ = SERVER_POOLType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SERVER_POOL = obj_
             obj_.original_tagname_ = 'SERVER_POOL'
 # end class ZONEType
 
 
-class TEMPLATEType136(GeneratedsSuper):
+class TEMPLATEType138(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ENDPOINT=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.ENDPOINT = ENDPOINT
         self.ENDPOINT_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType136)
+                CurrentSubclassModule_, TEMPLATEType138)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType136.subclass:
-            return TEMPLATEType136.subclass(*args_, **kwargs_)
+        if TEMPLATEType138.subclass:
+            return TEMPLATEType138.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType136(*args_, **kwargs_)
+            return TEMPLATEType138(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ENDPOINT(self):
         return self.ENDPOINT
@@ -50961,40 +51292,40 @@
     def _hasContent(self):
         if (
             self.ENDPOINT is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType136', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType136')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType138', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType138')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType136':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType138':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType136')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType138')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType136', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType138', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType136'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType138'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType136', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType138', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ENDPOINT is not None:
             namespaceprefix_ = self.ENDPOINT_nsprefix_ + ':' if (UseCapturedNS_ and self.ENDPOINT_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -51015,15 +51346,15 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ENDPOINT':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'ENDPOINT')
             value_ = self.gds_validate_string(value_, node, 'ENDPOINT')
             self.ENDPOINT = value_
             self.ENDPOINT_nsprefix_ = child_.prefix
-# end class TEMPLATEType136
+# end class TEMPLATEType138
 
 
 class SERVER_POOLType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, SERVER=None, gds_collector_=None, **kwargs_):
@@ -51249,36 +51580,36 @@
             value_ = self.gds_parse_string(value_, node, 'NAME')
             value_ = self.gds_validate_string(value_, node, 'NAME')
             self.NAME = value_
             self.NAME_nsprefix_ = child_.prefix
 # end class SERVERType
 
 
-class TEMPLATEType137(GeneratedsSuper):
+class TEMPLATEType139(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ENDPOINT=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.ENDPOINT = ENDPOINT
         self.ENDPOINT_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, TEMPLATEType137)
+                CurrentSubclassModule_, TEMPLATEType139)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if TEMPLATEType137.subclass:
-            return TEMPLATEType137.subclass(*args_, **kwargs_)
+        if TEMPLATEType139.subclass:
+            return TEMPLATEType139.subclass(*args_, **kwargs_)
         else:
-            return TEMPLATEType137(*args_, **kwargs_)
+            return TEMPLATEType139(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ENDPOINT(self):
         return self.ENDPOINT
@@ -51287,40 +51618,40 @@
     def _hasContent(self):
         if (
             self.ENDPOINT is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType137', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType137')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType139', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('TEMPLATEType139')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'TEMPLATEType137':
+        if self.original_tagname_ is not None and name_ == 'TEMPLATEType139':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType137')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType139')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType137', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType139', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType137'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType139'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType137', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType139', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ENDPOINT is not None:
             namespaceprefix_ = self.ENDPOINT_nsprefix_ + ':' if (UseCapturedNS_ and self.ENDPOINT_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -51341,18 +51672,18 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'ENDPOINT':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'ENDPOINT')
             value_ = self.gds_validate_string(value_, node, 'ENDPOINT')
             self.ENDPOINT = value_
             self.ENDPOINT_nsprefix_ = child_.prefix
-# end class TEMPLATEType137
+# end class TEMPLATEType139
 
 
-class SERVER_POOLType138(GeneratedsSuper):
+class SERVER_POOLType140(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, SERVER=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -51362,21 +51693,21 @@
             self.SERVER = []
         else:
             self.SERVER = SERVER
         self.SERVER_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SERVER_POOLType138)
+                CurrentSubclassModule_, SERVER_POOLType140)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if SERVER_POOLType138.subclass:
-            return SERVER_POOLType138.subclass(*args_, **kwargs_)
+        if SERVER_POOLType140.subclass:
+            return SERVER_POOLType140.subclass(*args_, **kwargs_)
         else:
-            return SERVER_POOLType138(*args_, **kwargs_)
+            return SERVER_POOLType140(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_SERVER(self):
         return self.SERVER
@@ -51391,40 +51722,40 @@
     def _hasContent(self):
         if (
             self.SERVER
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVER_POOLType138', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SERVER_POOLType138')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVER_POOLType140', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SERVER_POOLType140')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SERVER_POOLType138':
+        if self.original_tagname_ is not None and name_ == 'SERVER_POOLType140':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVER_POOLType138')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVER_POOLType140')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVER_POOLType138', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVER_POOLType140', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVER_POOLType138'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVER_POOLType140'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVER_POOLType138', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVER_POOLType140', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for SERVER_ in self.SERVER:
             namespaceprefix_ = self.SERVER_nsprefix_ + ':' if (UseCapturedNS_ and self.SERVER_nsprefix_) else ''
             SERVER_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='SERVER', pretty_print=pretty_print)
@@ -51439,22 +51770,22 @@
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         pass
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'SERVER':
-            obj_ = SERVERType139.factory(parent_object_=self)
+            obj_ = SERVERType141.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.SERVER.append(obj_)
             obj_.original_tagname_ = 'SERVER'
-# end class SERVER_POOLType138
+# end class SERVER_POOLType140
 
 
-class SERVERType139(GeneratedsSuper):
+class SERVERType141(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, ENDPOINT=None, ID=None, NAME=None, STATE=None, TERM=None, VOTEDFOR=None, COMMIT=None, LOG_INDEX=None, FEDLOG_INDEX=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -51477,21 +51808,21 @@
         self.LOG_INDEX = LOG_INDEX
         self.LOG_INDEX_nsprefix_ = None
         self.FEDLOG_INDEX = FEDLOG_INDEX
         self.FEDLOG_INDEX_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, SERVERType139)
+                CurrentSubclassModule_, SERVERType141)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if SERVERType139.subclass:
-            return SERVERType139.subclass(*args_, **kwargs_)
+        if SERVERType141.subclass:
+            return SERVERType141.subclass(*args_, **kwargs_)
         else:
-            return SERVERType139(*args_, **kwargs_)
+            return SERVERType141(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ENDPOINT(self):
         return self.ENDPOINT
@@ -51540,40 +51871,40 @@
             self.COMMIT is not None or
             self.LOG_INDEX is not None or
             self.FEDLOG_INDEX is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVERType139', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SERVERType139')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVERType141', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('SERVERType141')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'SERVERType139':
+        if self.original_tagname_ is not None and name_ == 'SERVERType141':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVERType139')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVERType141')
         if self._hasContent():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVERType139', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVERType141', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVERType139'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVERType141'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVERType139', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVERType141', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.ENDPOINT is not None:
             namespaceprefix_ = self.ENDPOINT_nsprefix_ + ':' if (UseCapturedNS_ and self.ENDPOINT_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -51674,15 +52005,15 @@
             self.LOG_INDEX_nsprefix_ = child_.prefix
         elif nodeName_ == 'FEDLOG_INDEX' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'FEDLOG_INDEX')
             ival_ = self.gds_validate_integer(ival_, node, 'FEDLOG_INDEX')
             self.FEDLOG_INDEX = ival_
             self.FEDLOG_INDEX_nsprefix_ = child_.prefix
-# end class SERVERType139
+# end class SERVERType141
 
 
 GDSClassesMapping = {
 }
 
 
 USAGE_TEXT = """
@@ -51883,307 +52214,310 @@
 __all__ = [
     "ACLType",
     "ACL_POOL",
     "ADMINSType",
     "ADMINSType13",
     "APP_CLONESType",
     "ARType",
-    "ARType129",
+    "ARType131",
     "AR_POOLType",
-    "AR_POOLType128",
+    "AR_POOLType130",
     "AUTH_MADType",
     "AUTH_MAD_CONFType",
     "BACKUPSType",
-    "BACKUPSType109",
+    "BACKUPSType111",
     "BACKUP_CONFIGType",
-    "BACKUP_CONFIGType110",
+    "BACKUP_CONFIGType112",
     "BACKUP_IDSType",
-    "BACKUP_IDSType111",
+    "BACKUP_IDSType113",
     "BACKUP_INCREMENTSType",
     "CALL_INFO",
     "CAPACITYType",
     "CLONESType",
     "CLUSTER",
     "CLUSTERSType",
-    "CLUSTERSType114",
-    "CLUSTERSType121",
-    "CLUSTERSType83",
+    "CLUSTERSType116",
+    "CLUSTERSType123",
+    "CLUSTERSType85",
     "CLUSTERType",
     "CLUSTER_POOL",
     "CONTEXT",
     "COREType",
     "DATASTORE",
     "DATASTORESType",
     "DATASTORESType32",
-    "DATASTORESType85",
+    "DATASTORESType87",
     "DATASTOREType",
     "DATASTOREType15",
     "DATASTOREType24",
-    "DATASTOREType48",
     "DATASTOREType5",
-    "DATASTOREType56",
-    "DATASTOREType66",
-    "DATASTOREType75",
-    "DATASTOREType86",
+    "DATASTOREType50",
+    "DATASTOREType58",
+    "DATASTOREType68",
+    "DATASTOREType77",
+    "DATASTOREType88",
     "DATASTORE_MADType",
     "DATASTORE_POOL",
     "DATASTORE_QUOTAType",
     "DATASTORE_QUOTAType14",
     "DATASTORE_QUOTAType23",
     "DATASTORE_QUOTAType4",
-    "DATASTORE_QUOTAType47",
-    "DATASTORE_QUOTAType55",
-    "DATASTORE_QUOTAType65",
-    "DATASTORE_QUOTAType74",
+    "DATASTORE_QUOTAType49",
+    "DATASTORE_QUOTAType57",
+    "DATASTORE_QUOTAType67",
+    "DATASTORE_QUOTAType76",
     "DBType",
     "DEFAULT_COSTType",
     "DEFAULT_GROUP_QUOTASType",
     "DEFAULT_GROUP_QUOTASType22",
     "DEFAULT_USER_QUOTASType",
-    "DEFAULT_USER_QUOTASType73",
+    "DEFAULT_USER_QUOTASType75",
     "DISKType",
-    "DISKType101",
+    "DISKType103",
     "DISK_SIZEType",
-    "DISK_SIZEType99",
+    "DISK_SIZEType101",
     "DOCUMENT",
     "DOCUMENT_POOL",
     "DS_MAD_CONFType",
     "ERROR_VMSType",
-    "ERROR_VMSType118",
-    "ERROR_VMSType126",
+    "ERROR_VMSType120",
+    "ERROR_VMSType128",
     "EXECUTION_RESULTType",
     "EXTRAType",
     "FEATURES",
     "FEDERATIONType",
     "GRAPHICS",
     "GROUP",
     "GROUPSType",
-    "GROUPSType63",
-    "GROUPSType82",
+    "GROUPSType65",
+    "GROUPSType84",
     "GROUPType",
     "GROUP_POOL",
     "HISTORY",
     "HISTORYType",
-    "HISTORYType106",
+    "HISTORYType108",
     "HISTORY_RECORDS",
     "HISTORY_RECORDSType",
-    "HISTORY_RECORDSType105",
+    "HISTORY_RECORDSType107",
     "HM_MADType",
     "HOOK",
     "HOOKLOGType",
     "HOOK_EXECUTION_RECORDType",
     "HOOK_LOG_CONFType",
     "HOOK_MESSAGE",
     "HOOK_POOL",
     "HOST",
     "HOSTSType",
-    "HOSTSType84",
+    "HOSTSType86",
     "HOSTType",
     "HOST_POOL",
     "HOST_SHAREType",
     "HUGEPAGEType",
+    "HUGEPAGEType34",
     "HYPERV_OPTIONS",
     "IMAGE",
     "IMAGESType",
     "IMAGEType",
     "IMAGEType11",
     "IMAGEType21",
     "IMAGEType30",
-    "IMAGEType54",
-    "IMAGEType62",
-    "IMAGEType72",
-    "IMAGEType81",
+    "IMAGEType56",
+    "IMAGEType64",
+    "IMAGEType74",
+    "IMAGEType83",
     "IMAGE_POOL",
     "IMAGE_QUOTAType",
     "IMAGE_QUOTAType10",
     "IMAGE_QUOTAType20",
     "IMAGE_QUOTAType29",
-    "IMAGE_QUOTAType53",
-    "IMAGE_QUOTAType61",
-    "IMAGE_QUOTAType71",
-    "IMAGE_QUOTAType80",
+    "IMAGE_QUOTAType55",
+    "IMAGE_QUOTAType63",
+    "IMAGE_QUOTAType73",
+    "IMAGE_QUOTAType82",
     "IM_MADType",
     "INCREMENTType",
     "INPUT",
     "IPAM_MADType",
     "LEASESType",
     "LEASEType",
     "LOCKType",
-    "LOCKType119",
-    "LOCKType130",
-    "LOCKType134",
-    "LOCKType34",
-    "LOCKType40",
-    "LOCKType89",
-    "LOCKType93",
-    "LOCKType97",
+    "LOCKType121",
+    "LOCKType132",
+    "LOCKType136",
+    "LOCKType36",
+    "LOCKType42",
+    "LOCKType91",
+    "LOCKType95",
+    "LOCKType99",
     "LOGIN_TOKENType",
-    "LOGIN_TOKENType64",
+    "LOGIN_TOKENType66",
     "LOGType",
     "MARKETPLACE",
     "MARKETPLACEAPP",
     "MARKETPLACEAPPSType",
     "MARKETPLACEAPP_POOL",
     "MARKETPLACE_POOL",
     "MARKET_MADType",
     "MARKET_MAD_CONFType",
     "MEMORYType",
+    "MEMORYType35",
     "MONITORING",
     "MONITORINGType",
-    "MONITORINGType43",
-    "MONITORINGType92",
-    "MONITORINGType98",
+    "MONITORINGType100",
+    "MONITORINGType45",
+    "MONITORINGType94",
     "MONITORING_DATA",
     "NETWORKType",
     "NETWORKType17",
     "NETWORKType26",
-    "NETWORKType50",
-    "NETWORKType58",
-    "NETWORKType68",
+    "NETWORKType52",
+    "NETWORKType60",
     "NETWORKType7",
-    "NETWORKType77",
+    "NETWORKType70",
+    "NETWORKType79",
     "NETWORK_QUOTAType",
     "NETWORK_QUOTAType16",
     "NETWORK_QUOTAType25",
-    "NETWORK_QUOTAType49",
-    "NETWORK_QUOTAType57",
+    "NETWORK_QUOTAType51",
+    "NETWORK_QUOTAType59",
     "NETWORK_QUOTAType6",
-    "NETWORK_QUOTAType67",
-    "NETWORK_QUOTAType76",
+    "NETWORK_QUOTAType69",
+    "NETWORK_QUOTAType78",
     "NICType",
-    "NICType102",
+    "NICType104",
     "NIC_ALIASType",
     "NIC_DEFAULT",
     "NODEType",
     "NUMA_NODE",
     "NUMA_NODESType",
+    "NUMA_NODEType",
     "OPENNEBULA_CONFIGURATION",
     "OS",
     "OUTDATED_VMSType",
-    "OUTDATED_VMSType116",
-    "OUTDATED_VMSType124",
+    "OUTDATED_VMSType118",
+    "OUTDATED_VMSType126",
     "PARAMETERSType",
     "PARAMETERType",
     "PCI",
     "PCIType",
     "PCI_DEVICESType",
     "PERMISSIONSType",
     "PERMISSIONSType1",
-    "PERMISSIONSType113",
-    "PERMISSIONSType120",
-    "PERMISSIONSType131",
+    "PERMISSIONSType115",
+    "PERMISSIONSType122",
     "PERMISSIONSType133",
+    "PERMISSIONSType135",
     "PERMISSIONSType2",
-    "PERMISSIONSType35",
-    "PERMISSIONSType41",
-    "PERMISSIONSType42",
+    "PERMISSIONSType37",
+    "PERMISSIONSType43",
     "PERMISSIONSType44",
-    "PERMISSIONSType88",
-    "PERMISSIONSType94",
+    "PERMISSIONSType46",
+    "PERMISSIONSType90",
     "PERMISSIONSType96",
+    "PERMISSIONSType98",
     "QUOTASType",
-    "QUOTASType46",
+    "QUOTASType48",
     "RAFT",
     "RAFTType",
     "RAW",
     "ROLESType",
     "ROLEType",
     "RULEType",
     "SCHED_ACTIONType",
     "SECURITY_GROUP",
     "SECURITY_GROUP_POOL",
     "SECURITY_GROUP_RULE",
     "SERVERType",
-    "SERVERType139",
+    "SERVERType141",
     "SERVER_POOLType",
-    "SERVER_POOLType138",
+    "SERVER_POOLType140",
     "SHOWBACKType",
     "SHOWBACK_RECORDS",
     "SNAPSHOTSType",
-    "SNAPSHOTSType107",
-    "SNAPSHOTSType38",
+    "SNAPSHOTSType109",
+    "SNAPSHOTSType40",
     "SNAPSHOTType",
-    "SNAPSHOTType103",
-    "SNAPSHOTType108",
-    "SNAPSHOTType39",
+    "SNAPSHOTType105",
+    "SNAPSHOTType110",
+    "SNAPSHOTType41",
     "SPICE_OPTIONS",
     "SYSTEMType",
     "TEMPLATEType",
-    "TEMPLATEType100",
-    "TEMPLATEType127",
-    "TEMPLATEType132",
-    "TEMPLATEType136",
-    "TEMPLATEType137",
+    "TEMPLATEType102",
+    "TEMPLATEType129",
+    "TEMPLATEType134",
+    "TEMPLATEType138",
+    "TEMPLATEType139",
     "TEMPLATEType31",
     "TEMPLATEType33",
-    "TEMPLATEType37",
-    "TEMPLATEType45",
-    "TEMPLATEType91",
-    "TEMPLATEType95",
+    "TEMPLATEType39",
+    "TEMPLATEType47",
+    "TEMPLATEType93",
+    "TEMPLATEType97",
     "TM_MADType",
     "TM_MAD_CONFType",
     "TOPOLOGY",
     "UPDATED_VMSType",
-    "UPDATED_VMSType115",
-    "UPDATED_VMSType123",
+    "UPDATED_VMSType117",
+    "UPDATED_VMSType125",
     "UPDATING_VMSType",
-    "UPDATING_VMSType117",
-    "UPDATING_VMSType125",
+    "UPDATING_VMSType119",
+    "UPDATING_VMSType127",
     "USER",
     "USERSType",
     "USERSType12",
     "USERType",
     "USER_POOL",
     "USER_TEMPLATEType",
-    "USER_TEMPLATEType104",
+    "USER_TEMPLATEType106",
     "VCENTER_RESOURCE_POOL_INFO",
     "VDC",
     "VDC_POOL",
     "VLAN_IDSType",
     "VM",
     "VMGROUP",
     "VMSType",
-    "VMSType135",
-    "VMSType36",
+    "VMSType137",
+    "VMSType38",
     "VMTEMPLATE",
     "VMTEMPLATE_POOL",
     "VMType",
     "VMType19",
     "VMType28",
     "VMType3",
-    "VMType52",
-    "VMType60",
-    "VMType70",
-    "VMType79",
+    "VMType54",
+    "VMType62",
+    "VMType72",
+    "VMType81",
     "VMType9",
-    "VMType90",
+    "VMType92",
     "VM_GROUP",
     "VM_GROUP_POOL",
     "VM_MADType",
     "VM_POOL",
     "VM_QUOTAType",
     "VM_QUOTAType18",
     "VM_QUOTAType27",
-    "VM_QUOTAType51",
-    "VM_QUOTAType59",
-    "VM_QUOTAType69",
-    "VM_QUOTAType78",
+    "VM_QUOTAType53",
+    "VM_QUOTAType61",
+    "VM_QUOTAType71",
     "VM_QUOTAType8",
+    "VM_QUOTAType80",
     "VNC_PORTSType",
     "VNET",
     "VNETSType",
-    "VNETSType87",
+    "VNETSType89",
     "VNETType",
-    "VNETType112",
+    "VNETType114",
     "VNET_POOL",
     "VNTEMPLATE",
     "VNTEMPLATE_POOL",
     "VN_MAD_CONFType",
     "VROUTER",
     "VROUTERSType",
-    "VROUTERSType122",
+    "VROUTERSType124",
     "VROUTER_POOL",
     "VXLAN_IDSType",
     "ZONE",
     "ZONEType",
     "ZONE_POOL"
 ]
```

### Comparing `pyone-6.6.0/pyone/helpers.py` & `pyone-6.6.1/pyone/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018 www.privaz.io Valletech AB
-# Copyright 2002-2022, OpenNebula Project, OpenNebula Systems
+# Copyright 2002-2023, OpenNebula Project, OpenNebula Systems
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pyone-6.6.0/pyone/server.py` & `pyone-6.6.1/pyone/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018 www.privaz.io Valletech AB
-# Copyright 2002-2022, OpenNebula Project, OpenNebula Systems
+# Copyright 2002-2023, OpenNebula Project, OpenNebula Systems
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pyone-6.6.0/pyone/tester.py` & `pyone-6.6.1/pyone/tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018 www.privaz.io Valletech AB
-# Copyright 2002-2022, OpenNebula Project, OpenNebula Systems
+# Copyright 2002-2023, OpenNebula Project, OpenNebula Systems
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pyone-6.6.0/pyone/util.py` & `pyone-6.6.1/pyone/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018 www.privaz.io Valletech AB
-# Copyright 2002-2022, OpenNebula Project, OpenNebula Systems
+# Copyright 2002-2023, OpenNebula Project, OpenNebula Systems
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pyone-6.6.0/pyone.egg-info/PKG-INFO` & `pyone-6.6.1/pyone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyone
-Version: 6.6.0
+Version: 6.6.1
 Summary: Python Bindings for OpenNebula XML-RPC API
 Home-page: http://opennebula.io
 Author: Rafael del Valle
 Author-email: rvalle@privaz.io
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: PyOne is an implementation of OpenNebula XML-RPC
                 bindings in Python. It works as a proxy over the XML-RPC api and
```

### Comparing `pyone-6.6.0/setup.py` & `pyone-6.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018 www.privaz.io Valletech AB
-# Copyright 2002-2022, OpenNebula Project, OpenNebula Systems
+# Copyright 2002-2023, OpenNebula Project, OpenNebula Systems
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,15 +32,15 @@
     'requests'
 ]
 
 # include future in python2
 if sys.version_info[0] < 3:
     install_requires.append('future')
 
-version = '6.6.0'
+version = '6.6.1'
 
 # mark pre-release
 v1 = int(version.split('.')[1])
 v2 = int(version.split('.')[2])
 
 if v1 >= 90 or v2 >= 90:
     pyone_version = version + 'rc1'
```

