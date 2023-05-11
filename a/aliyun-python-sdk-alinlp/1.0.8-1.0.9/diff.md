# Comparing `tmp/aliyun-python-sdk-alinlp-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-alinlp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-alinlp-1.0.8.tar", last modified: Fri Jul 31 08:08:44 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-alinlp-1.0.9.tar", last modified: Mon Aug  3 07:16:25 2020, max compression
```

## Comparing `aliyun-python-sdk-alinlp-1.0.8.tar` & `aliyun-python-sdk-alinlp-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/
--rw-rw-r--   0 admin     (1017) admin     (1017)       21 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/
--rw-rw-r--   0 admin     (1017) admin     (1017)     1945 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomTitleRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1591 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetNerChMedicalRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1917 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetPosChEcomRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1949 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomCommentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1953 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEntertainmentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1593 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetSummaryChEcomRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1949 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomContentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1933 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChO2ORequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/__init__.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1771 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaGeneralRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1589 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetEcChGeneralRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1765 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaEcomRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1941 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChGeneralRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1891 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetTsChEcomRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2205 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChCommentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2203 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChSearchRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1589 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetEcEnGeneralRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1583 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetDpChEcomRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2199 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChEcomRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2217 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChEntertainmentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1759 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetNerCustomizedChEcomRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1088 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/endpoint.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/MANIFEST.in
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/
--rw-rw-r--   0 admin     (1017) admin     (1017)        1 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       16 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       31 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/requires.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1684 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/SOURCES.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1552 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)       38 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/setup.cfg
--rw-rw-r--   0 admin     (1017) admin     (1017)      533 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/README.rst
--rw-rw-r--   0 admin     (1017) admin     (1017)     1552 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)     2467 2020-07-31 08:08:44.000000 aliyun-python-sdk-alinlp-1.0.8/setup.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/
+-rw-rw-r--   0 admin      (531) admin      (531)       38 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/setup.cfg
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/
+-rw-rw-r--   0 admin      (531) admin      (531)       21 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1088 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/endpoint.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/__init__.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1593 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetSummaryChEcomRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2217 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChEntertainmentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1949 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomCommentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1891 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetTsChEcomRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1759 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetNerCustomizedChEcomRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2199 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChEcomRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2203 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChSearchRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1771 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaGeneralRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1583 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetDpChEcomRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1933 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChO2ORequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2205 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChCommentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1605 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetDpChGeneralStanfordRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1941 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChGeneralRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1591 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetNerChMedicalRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1917 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetPosChEcomRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1589 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetEcChGeneralRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1949 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomContentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1953 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEntertainmentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1595 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetDpChGeneralCTBRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1945 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomTitleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1765 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaEcomRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1589 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetEcEnGeneralRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2467 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/setup.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/
+-rw-rw-r--   0 admin      (531) admin      (531)        1 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       31 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/requires.txt
+-rw-rw-r--   0 admin      (531) admin      (531)     1813 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       16 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/top_level.txt
+-rw-rw-r--   0 admin      (531) admin      (531)     1552 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/PKG-INFO
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/MANIFEST.in
+-rw-rw-r--   0 admin      (531) admin      (531)      533 2020-08-03 07:16:24.000000 aliyun-python-sdk-alinlp-1.0.9/README.rst
+-rw-rw-r--   0 admin      (531) admin      (531)     1552 2020-08-03 07:16:25.000000 aliyun-python-sdk-alinlp-1.0.9/PKG-INFO
```

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomTitleRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomTitleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetNerChMedicalRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetNerChMedicalRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetPosChEcomRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetPosChEcomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomCommentRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomCommentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEntertainmentRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEntertainmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetSummaryChEcomRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetSummaryChEcomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomContentRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChEcomContentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChO2ORequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChO2ORequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaGeneralRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaGeneralRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetEcChGeneralRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetEcChGeneralRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaEcomRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedSeaEcomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChGeneralRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWsCustomizedChGeneralRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetTsChEcomRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetTsChEcomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChCommentRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChCommentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChSearchRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChSearchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetEcEnGeneralRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetEcEnGeneralRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetDpChEcomRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetDpChEcomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChEcomRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChEcomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetWeChEntertainmentRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetWeChEntertainmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/request/v20200629/GetNerCustomizedChEcomRequest.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/request/v20200629/GetNerCustomizedChEcomRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyunsdkalinlp/endpoint.py` & `aliyun-python-sdk-alinlp-1.0.9/aliyunsdkalinlp/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/SOURCES.txt` & `aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 aliyun_python_sdk_alinlp.egg-info/dependency_links.txt
 aliyun_python_sdk_alinlp.egg-info/requires.txt
 aliyun_python_sdk_alinlp.egg-info/top_level.txt
 aliyunsdkalinlp/__init__.py
 aliyunsdkalinlp/endpoint.py
 aliyunsdkalinlp/request/__init__.py
 aliyunsdkalinlp/request/v20200629/GetDpChEcomRequest.py
+aliyunsdkalinlp/request/v20200629/GetDpChGeneralCTBRequest.py
+aliyunsdkalinlp/request/v20200629/GetDpChGeneralStanfordRequest.py
 aliyunsdkalinlp/request/v20200629/GetEcChGeneralRequest.py
 aliyunsdkalinlp/request/v20200629/GetEcEnGeneralRequest.py
 aliyunsdkalinlp/request/v20200629/GetNerChMedicalRequest.py
 aliyunsdkalinlp/request/v20200629/GetNerCustomizedChEcomRequest.py
 aliyunsdkalinlp/request/v20200629/GetPosChEcomRequest.py
 aliyunsdkalinlp/request/v20200629/GetSummaryChEcomRequest.py
 aliyunsdkalinlp/request/v20200629/GetTsChEcomRequest.py
```

### Comparing `aliyun-python-sdk-alinlp-1.0.8/aliyun_python_sdk_alinlp.egg-info/PKG-INFO` & `aliyun-python-sdk-alinlp-1.0.9/aliyun_python_sdk_alinlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alinlp
-Version: 1.0.8
+Version: 1.0.9
 Summary: The alinlp module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alinlp
```

### Comparing `aliyun-python-sdk-alinlp-1.0.8/README.rst` & `aliyun-python-sdk-alinlp-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alinlp-1.0.8/PKG-INFO` & `aliyun-python-sdk-alinlp-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alinlp
-Version: 1.0.8
+Version: 1.0.9
 Summary: The alinlp module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alinlp
```

### Comparing `aliyun-python-sdk-alinlp-1.0.8/setup.py` & `aliyun-python-sdk-alinlp-1.0.9/setup.py`

 * *Files identical despite different names*

