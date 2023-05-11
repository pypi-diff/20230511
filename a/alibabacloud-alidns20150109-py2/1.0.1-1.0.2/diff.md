# Comparing `tmp/alibabacloud_alidns20150109_py2-1.0.1.tar.gz` & `tmp/alibabacloud_alidns20150109_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alidns20150109_py2-1.0.1.tar", last modified: Mon Apr  3 07:51:33 2023, max compression
+gzip compressed data, was "dist/alibabacloud_alidns20150109_py2-1.0.2.tar", last modified: Tue Apr  4 03:51:01 2023, max compression
```

## Comparing `alibabacloud_alidns20150109_py2-1.0.1.tar` & `alibabacloud_alidns20150109_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109/__init__.py
--rw-r--r--   0 root         (0) root         (0)   236947 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109/client.py
--rw-r--r--   0 root         (0) root         (0)  1167933 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2023-04-03 07:51:33.000000 alibabacloud_alidns20150109_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   236947 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109/client.py
+-rw-r--r--   0 root         (0) root         (0)  1168182 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-04-04 03:51:01.000000 alibabacloud_alidns20150109_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/LICENSE` & `alibabacloud_alidns20150109_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/PKG-INFO` & `alibabacloud_alidns20150109_py2-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alidns20150109_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Alidns (20150109) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/README-CN.md` & `alibabacloud_alidns20150109_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/README.md` & `alibabacloud_alidns20150109_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109/client.py` & `alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109/models.py` & `alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -22315,18 +22315,19 @@
             self.start_date = m.get('StartDate')
         if m.get('Threshold') is not None:
             self.threshold = m.get('Threshold')
         return self
 
 
 class DescribeRecordResolveStatisticsSummaryResponseBodyStatistics(TeaModel):
-    def __init__(self, count=None, domain_name=None, domain_type=None):
+    def __init__(self, count=None, domain_name=None, domain_type=None, sub_domain=None):
         self.count = count  # type: str
         self.domain_name = domain_name  # type: str
         self.domain_type = domain_type  # type: str
+        self.sub_domain = sub_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRecordResolveStatisticsSummaryResponseBodyStatistics, self).to_map()
         if _map is not None:
@@ -22335,24 +22336,28 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, page_number=None, page_size=None, request_id=None, statistics=None, total_items=None,
                  total_pages=None):
         self.page_number = page_number  # type: int
```

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/alibabacloud_alidns20150109_py2.egg-info/PKG-INFO` & `alibabacloud_alidns20150109_py2-1.0.2/alibabacloud_alidns20150109_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alidns20150109-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Alidns (20150109) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alidns20150109_py2-1.0.1/setup.py` & `alibabacloud_alidns20150109_py2-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alidns20150109_py2.
 
-Created on 03/04/2023
+Created on 04/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alidns20150109"
 NAME = "alibabacloud_alidns20150109_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alidns (20150109) SDK Library for Python2"
```

