# Comparing `tmp/alibabacloud_alidns20150109-3.0.2.tar.gz` & `tmp/alibabacloud_alidns20150109-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alidns20150109-3.0.2.tar", last modified: Mon Apr  3 07:52:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_alidns20150109-3.0.3.tar", last modified: Tue Apr  4 03:51:24 2023, max compression
```

## Comparing `alibabacloud_alidns20150109-3.0.2.tar` & `alibabacloud_alidns20150109-3.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/
--rw-r--r--   0 root         (0) root         (0)      444 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109/__init__.py
--rw-r--r--   0 root         (0) root         (0)   577861 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109/client.py
--rw-r--r--   0 root         (0) root         (0)  1155494 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2625 2023-04-03 07:52:06.000000 alibabacloud_alidns20150109-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   577861 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109/client.py
+-rw-r--r--   0 root         (0) root         (0)  1155745 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-04-04 03:51:24.000000 alibabacloud_alidns20150109-3.0.3/setup.py
```

### Comparing `alibabacloud_alidns20150109-3.0.2/LICENSE` & `alibabacloud_alidns20150109-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109-3.0.2/PKG-INFO` & `alibabacloud_alidns20150109-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alidns20150109
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud Alidns (20150109) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alidns20150109-3.0.2/README-CN.md` & `alibabacloud_alidns20150109-3.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109-3.0.2/README.md` & `alibabacloud_alidns20150109-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109/client.py` & `alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109/models.py` & `alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -25090,18 +25090,20 @@
 
 class DescribeRecordResolveStatisticsSummaryResponseBodyStatistics(TeaModel):
     def __init__(
         self,
         count: str = None,
         domain_name: str = None,
         domain_type: str = None,
+        sub_domain: str = None,
     ):
         self.count = count
         self.domain_name = domain_name
         self.domain_type = domain_type
+        self.sub_domain = sub_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -25110,24 +25112,28 @@
         result = dict()
         if self.count is not None:
             result['Count'] = self.count
         if self.domain_name is not None:
             result['DomainName'] = self.domain_name
         if self.domain_type is not None:
             result['DomainType'] = self.domain_type
+        if self.sub_domain is not None:
+            result['SubDomain'] = self.sub_domain
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Count') is not None:
             self.count = m.get('Count')
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         if m.get('DomainType') is not None:
             self.domain_type = m.get('DomainType')
+        if m.get('SubDomain') is not None:
+            self.sub_domain = m.get('SubDomain')
         return self
 
 
 class DescribeRecordResolveStatisticsSummaryResponseBody(TeaModel):
     def __init__(
         self,
         page_number: int = None,
```

### Comparing `alibabacloud_alidns20150109-3.0.2/alibabacloud_alidns20150109.egg-info/PKG-INFO` & `alibabacloud_alidns20150109-3.0.3/alibabacloud_alidns20150109.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alidns20150109
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud Alidns (20150109) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alidns20150109-3.0.2/setup.py` & `alibabacloud_alidns20150109-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alidns20150109.
 
-Created on 03/04/2023
+Created on 04/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alidns20150109"
 NAME = "alibabacloud_alidns20150109" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alidns (20150109) SDK Library for Python"
```

