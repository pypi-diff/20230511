# Comparing `tmp/pulumi_ngrok-0.0.14.tar.gz` & `tmp/pulumi_ngrok-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_ngrok-0.0.14.tar", last modified: Tue Apr 11 17:02:06 2023, max compression
+gzip compressed data, was "dist/pulumi_ngrok-0.0.15.tar", last modified: Thu May 11 11:02:20 2023, max compression
```

## Comparing `pulumi_ngrok-0.0.14.tar` & `pulumi_ngrok-0.0.15.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95968 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/agent_ingress.py
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/certificate_authority.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    51897 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/endpoint_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/event_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/ip_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/ip_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/ip_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    90020 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/reserved_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    34359 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/reserved_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_certificate_authority.py
--rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_host_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    39340 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_user_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24665 2023-04-11 17:02:05.000000 pulumi_ngrok-0.0.14/pulumi_ngrok/tls_certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-11 17:02:06.000000 pulumi_ngrok-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95968 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/agent_ingress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/certificate_authority.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51897 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/endpoint_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/event_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/ip_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/ip_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/ip_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90020 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/reserved_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34359 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/reserved_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_certificate_authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_host_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39340 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_user_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24665 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/pulumi_ngrok/tls_certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:02:20.000000 pulumi_ngrok-0.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-11 11:02:19.000000 pulumi_ngrok-0.0.15/setup.py
```

### Comparing `pulumi_ngrok-0.0.14/PKG-INFO` & `pulumi_ngrok-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ngrok
-Version: 0.0.14
+Version: 0.0.15
 Summary: A Pulumi package for creating and managing ngrok cloud resources.
 Home-page: https://ngrok.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-ngrok
 Description: # Terraform Bridge Provider Boilerplate
         
         This repository contains boilerplate code for building a new Pulumi provider which wraps an existing Terraform provider.
```

### Comparing `pulumi_ngrok-0.0.14/README.md` & `pulumi_ngrok-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/__init__.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/_inputs.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/_utilities.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/agent_ingress.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/agent_ingress.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/api_key.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/certificate_authority.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/config/vars.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/credential.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/endpoint_configuration.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/endpoint_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/event_destination.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/event_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/event_subscription.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/event_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/ip_policy.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/ip_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/ip_policy_rule.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/ip_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/ip_restriction.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/ip_restriction.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/outputs.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/provider.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/reserved_address.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/reserved_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/reserved_domain.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/reserved_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_certificate_authority.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_certificate_authority.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_credential.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_host_certificate.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_host_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/ssh_user_certificate.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/ssh_user_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok/tls_certificate.py` & `pulumi_ngrok-0.0.15/pulumi_ngrok/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/PKG-INFO` & `pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-ngrok
-Version: 0.0.14
+Version: 0.0.15
 Summary: A Pulumi package for creating and managing ngrok cloud resources.
 Home-page: https://ngrok.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-ngrok
 Description: # Terraform Bridge Provider Boilerplate
         
         This repository contains boilerplate code for building a new Pulumi provider which wraps an existing Terraform provider.
```

### Comparing `pulumi_ngrok-0.0.14/pulumi_ngrok.egg-info/SOURCES.txt` & `pulumi_ngrok-0.0.15/pulumi_ngrok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ngrok-0.0.14/setup.py` & `pulumi_ngrok-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.14"
-PLUGIN_VERSION = "0.0.14"
+VERSION = "0.0.15"
+PLUGIN_VERSION = "0.0.15"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'ngrok', PLUGIN_VERSION, '--server', 'github://api.github.com/pierskarsenbarg/pulumi-ngrok'])
         except OSError as error:
```

