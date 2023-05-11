# Comparing `tmp/pulumi_tls-5.1.0a1683613744.tar.gz` & `tmp/pulumi_tls-5.1.0a1683788254.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tls-5.1.0a1683613744.tar", last modified: Tue May  9 06:47:12 2023, max compression
+gzip compressed data, was "pulumi_tls-5.1.0a1683788254.tar", last modified: Thu May 11 07:02:32 2023, max compression
```

## Comparing `pulumi_tls-5.1.0a1683613744.tar` & `pulumi_tls-5.1.0a1683788254.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:47:12.609274 pulumi_tls-5.1.0a1683613744/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-09 06:47:12.609274 pulumi_tls-5.1.0a1683613744/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:47:12.609274 pulumi_tls-5.1.0a1683613744/pulumi_tls/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/cert_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:47:12.609274 pulumi_tls-5.1.0a1683613744/pulumi_tls/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/get_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    42903 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/locally_signed_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54199 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls/self_signed_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:47:12.609274 pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:47:12.609274 pulumi_tls-5.1.0a1683613744/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-09 06:47:12.000000 pulumi_tls-5.1.0a1683613744/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:02:32.817825 pulumi_tls-5.1.0a1683788254/
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-11 07:02:32.817825 pulumi_tls-5.1.0a1683788254/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:02:32.813825 pulumi_tls-5.1.0a1683788254/pulumi_tls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/cert_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:02:32.817825 pulumi_tls-5.1.0a1683788254/pulumi_tls/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/get_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42903 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/locally_signed_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54199 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls/self_signed_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:02:32.813825 pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:02:32.817825 pulumi_tls-5.1.0a1683788254/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-11 07:02:32.000000 pulumi_tls-5.1.0a1683788254/setup.py
```

### Comparing `pulumi_tls-5.1.0a1683613744/PKG-INFO` & `pulumi_tls-5.1.0a1683788254/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1683613744
+Version: 5.1.0a1683788254
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1683613744/README.md` & `pulumi_tls-5.1.0a1683788254/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/__init__.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/_inputs.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/_utilities.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/cert_request.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/config/outputs.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/config/vars.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/get_certificate.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/get_public_key.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/get_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/locally_signed_cert.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/locally_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/outputs.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/private_key.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/provider.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls/self_signed_cert.py` & `pulumi_tls-5.1.0a1683788254/pulumi_tls/self_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/PKG-INFO` & `pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-tls
-Version: 5.1.0a1683613744
+Version: 5.1.0a1683788254
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1683613744/pulumi_tls.egg-info/SOURCES.txt` & `pulumi_tls-5.1.0a1683788254/pulumi_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1683613744/setup.py` & `pulumi_tls-5.1.0a1683788254/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.1.0a1683613744"
-PLUGIN_VERSION = "5.1.0-alpha.1683613744+7c6979e1"
+VERSION = "5.1.0a1683788254"
+PLUGIN_VERSION = "5.1.0-alpha.1683788254+d2e07d5a"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'tls', PLUGIN_VERSION])
         except OSError as error:
```

