# Comparing `tmp/iotiumlib-23.5.0.tar.gz` & `tmp/iotiumlib-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotiumlib-23.5.0.tar", last modified: Wed Apr 19 16:17:41 2023, max compression
+gzip compressed data, was "iotiumlib-23.5.1.tar", last modified: Thu May 11 05:11:45 2023, max compression
```

## Comparing `iotiumlib-23.5.0.tar` & `iotiumlib-23.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.278106 iotiumlib-23.5.0/
--rw-rw-rw-   0        0        0        0 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/LICENSE
--rw-rw-rw-   0        0        0    15806 2023-04-19 16:17:41.264581 iotiumlib-23.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    15386 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.225728 iotiumlib-23.5.0/iotiumlib/
--rw-rw-rw-   0        0        0     1084 2023-04-18 16:17:48.000000 iotiumlib-23.5.0/iotiumlib/__init__.py
--rw-rw-rw-   0        0        0     8141 2023-04-18 15:55:13.000000 iotiumlib-23.5.0/iotiumlib/cluster.py
--rw-rw-rw-   0        0        0     6674 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/download.py
--rw-rw-rw-   0        0        0     7414 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/firewall.py
--rw-rw-rw-   0        0        0     5465 2022-11-18 11:01:08.000000 iotiumlib-23.5.0/iotiumlib/helper.py
--rw-rw-rw-   0        0        0     2948 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/image.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.263385 iotiumlib-23.5.0/iotiumlib/models/
--rw-rw-rw-   0        0        0        0 2022-08-19 08:13:17.000000 iotiumlib-23.5.0/iotiumlib/models/__init__.py
--rw-rw-rw-   0        0        0     7779 2022-10-27 06:17:54.000000 iotiumlib-23.5.0/iotiumlib/models/role_creation_vo.py
--rw-rw-rw-   0        0        0     6541 2022-10-27 06:18:04.000000 iotiumlib-23.5.0/iotiumlib/models/role_updation_vo.py
--rw-rw-rw-   0        0        0    10440 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_listener_creation_vo.py
--rw-rw-rw-   0        0        0     7208 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_listener_update_vo.py
--rw-rw-rw-   0        0        0     6417 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_ports_vo.py
--rw-rw-rw-   0        0        0     3576 2022-04-26 05:52:48.000000 iotiumlib-23.5.0/iotiumlib/models/service_selector_vo.py
--rw-rw-rw-   0        0        0    16868 2023-04-18 15:44:50.000000 iotiumlib-23.5.0/iotiumlib/network.py
--rw-rw-rw-   0        0        0    11025 2022-08-16 11:29:12.000000 iotiumlib-23.5.0/iotiumlib/node.py
--rw-rw-rw-   0        0        0     3457 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/nodecli.py
--rw-rw-rw-   0        0        0      538 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/orch.py
--rw-rw-rw-   0        0        0     2605 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/orchlogin.py
--rw-rw-rw-   0        0        0     5038 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/org.py
--rw-rw-rw-   0        0        0     2514 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/pki.py
--rw-rw-rw-   0        0        0     2407 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/profile.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.264581 iotiumlib-23.5.0/iotiumlib/requires/
--rw-rw-rw-   0        0        0     1425 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/Exceptions.py
--rw-rw-rw-   0        0        0       58 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/__init__.py
--rw-rw-rw-   0        0        0      687 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/commonVariables.py
--rw-rw-rw-   0        0        0     4802 2023-04-18 16:04:11.000000 iotiumlib-23.5.0/iotiumlib/requires/commonWrapper.py
--rw-rw-rw-   0        0        0       38 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/requires/constants.py
--rw-rw-rw-   0        0        0    68425 2023-04-18 16:03:29.000000 iotiumlib-23.5.0/iotiumlib/requires/resourcePayload.py
--rw-rw-rw-   0        0        0    24444 2022-08-19 08:13:17.000000 iotiumlib-23.5.0/iotiumlib/requires/utils.py
--rw-rw-rw-   0        0        0     4109 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/secret.py
--rw-rw-rw-   0        0        0    11742 2022-04-27 22:34:36.000000 iotiumlib-23.5.0/iotiumlib/service.py
--rw-rw-rw-   0        0        0     2918 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/sshkey.py
--rw-rw-rw-   0        0        0    15172 2022-03-28 06:43:21.000000 iotiumlib-23.5.0/iotiumlib/user.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:17:41.247112 iotiumlib-23.5.0/iotiumlib.egg-info/
--rw-rw-rw-   0        0        0    15806 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 16:17:41.000000 iotiumlib-23.5.0/iotiumlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 16:17:41.278106 iotiumlib-23.5.0/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-04-18 16:19:09.000000 iotiumlib-23.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:11:45.406850 iotiumlib-23.5.1/
+-rw-rw-rw-   0        0        0        0 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/LICENSE
+-rw-rw-rw-   0        0        0    15806 2023-05-11 05:11:45.406850 iotiumlib-23.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15386 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 05:11:45.216534 iotiumlib-23.5.1/iotiumlib/
+-rw-rw-rw-   0        0        0     1084 2023-05-11 05:06:44.000000 iotiumlib-23.5.1/iotiumlib/__init__.py
+-rw-rw-rw-   0        0        0     8141 2023-04-18 15:55:13.000000 iotiumlib-23.5.1/iotiumlib/cluster.py
+-rw-rw-rw-   0        0        0     6674 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/download.py
+-rw-rw-rw-   0        0        0     7414 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/firewall.py
+-rw-rw-rw-   0        0        0     5489 2023-05-09 06:39:43.000000 iotiumlib-23.5.1/iotiumlib/helper.py
+-rw-rw-rw-   0        0        0     2948 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/image.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:11:45.311681 iotiumlib-23.5.1/iotiumlib/models/
+-rw-rw-rw-   0        0        0        0 2022-08-19 08:13:17.000000 iotiumlib-23.5.1/iotiumlib/models/__init__.py
+-rw-rw-rw-   0        0        0     7779 2022-10-27 06:17:54.000000 iotiumlib-23.5.1/iotiumlib/models/role_creation_vo.py
+-rw-rw-rw-   0        0        0     6541 2022-10-27 06:18:04.000000 iotiumlib-23.5.1/iotiumlib/models/role_updation_vo.py
+-rw-rw-rw-   0        0        0    10440 2022-04-26 05:52:48.000000 iotiumlib-23.5.1/iotiumlib/models/service_listener_creation_vo.py
+-rw-rw-rw-   0        0        0     7208 2022-04-26 05:52:48.000000 iotiumlib-23.5.1/iotiumlib/models/service_listener_update_vo.py
+-rw-rw-rw-   0        0        0     6417 2022-04-26 05:52:48.000000 iotiumlib-23.5.1/iotiumlib/models/service_ports_vo.py
+-rw-rw-rw-   0        0        0     3576 2022-04-26 05:52:48.000000 iotiumlib-23.5.1/iotiumlib/models/service_selector_vo.py
+-rw-rw-rw-   0        0        0    16868 2023-04-18 15:44:50.000000 iotiumlib-23.5.1/iotiumlib/network.py
+-rw-rw-rw-   0        0        0    11505 2023-05-08 13:02:42.000000 iotiumlib-23.5.1/iotiumlib/node.py
+-rw-rw-rw-   0        0        0     3457 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/nodecli.py
+-rw-rw-rw-   0        0        0      538 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/orch.py
+-rw-rw-rw-   0        0        0     2605 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/orchlogin.py
+-rw-rw-rw-   0        0        0     5038 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/org.py
+-rw-rw-rw-   0        0        0     2514 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/pki.py
+-rw-rw-rw-   0        0        0     2407 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/profile.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:11:45.389349 iotiumlib-23.5.1/iotiumlib/requires/
+-rw-rw-rw-   0        0        0     1425 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/requires/Exceptions.py
+-rw-rw-rw-   0        0        0       58 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/requires/__init__.py
+-rw-rw-rw-   0        0        0      687 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/requires/commonVariables.py
+-rw-rw-rw-   0        0        0     4802 2023-05-08 12:42:02.000000 iotiumlib-23.5.1/iotiumlib/requires/commonWrapper.py
+-rw-rw-rw-   0        0        0       38 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/requires/constants.py
+-rw-rw-rw-   0        0        0    69685 2023-05-08 13:03:27.000000 iotiumlib-23.5.1/iotiumlib/requires/resourcePayload.py
+-rw-rw-rw-   0        0        0    24444 2022-08-19 08:13:17.000000 iotiumlib-23.5.1/iotiumlib/requires/utils.py
+-rw-rw-rw-   0        0        0     4109 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/secret.py
+-rw-rw-rw-   0        0        0    11742 2022-04-27 22:34:36.000000 iotiumlib-23.5.1/iotiumlib/service.py
+-rw-rw-rw-   0        0        0     2918 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/sshkey.py
+-rw-rw-rw-   0        0        0    15172 2022-03-28 06:43:21.000000 iotiumlib-23.5.1/iotiumlib/user.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:11:45.232174 iotiumlib-23.5.1/iotiumlib.egg-info/
+-rw-rw-rw-   0        0        0    15806 2023-05-11 05:11:44.000000 iotiumlib-23.5.1/iotiumlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-05-11 05:11:44.000000 iotiumlib-23.5.1/iotiumlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:11:44.000000 iotiumlib-23.5.1/iotiumlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-11 05:11:44.000000 iotiumlib-23.5.1/iotiumlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 05:11:44.000000 iotiumlib-23.5.1/iotiumlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:11:45.406850 iotiumlib-23.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-05-11 05:06:44.000000 iotiumlib-23.5.1/setup.py
```

### Comparing `iotiumlib-23.5.0/PKG-INFO` & `iotiumlib-23.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotiumlib
-Version: 23.5.0
+Version: 23.5.1
 Summary: ioTium API library
 Home-page: https://view.com
 Author: Rashtrapathy C
 Author-email: rashtrapathy.chandrasekar@view.com
 License: Copyright 2023 View, Inc. | All Rights Reserved.
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: OS Independent
```

### Comparing `iotiumlib-23.5.0/README.md` & `iotiumlib-23.5.1/README.md`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/__init__.py` & `iotiumlib-23.5.1/iotiumlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Rashtrapathy"
 __copyright__ = "Copyright 2023 View, Inc. | All Rights Reserved"
 __license__ = "All rights reserved."
-__version__ = "23.5.00"
+__version__ = "23.5.01"
 __credits__ = ["Rashtrapathy", "Thyagarajan", "Jawahar", "Venkatesan", "Raja"]
 __maintainer__ = "Rashtrapathy C"
 __email__ = "rashtrapathy.chandrasekar@view.com"
 __status__ = "Development"
 __name__ = "iotiumlib"
 
 from .node import *
```

### Comparing `iotiumlib-23.5.0/iotiumlib/cluster.py` & `iotiumlib-23.5.1/iotiumlib/cluster.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/download.py` & `iotiumlib-23.5.1/iotiumlib/download.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/firewall.py` & `iotiumlib-23.5.1/iotiumlib/firewall.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/helper.py` & `iotiumlib-23.5.1/iotiumlib/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,21 +116,21 @@
     else:
         return str1
 
 def get_all_networks_from_cluster(cluster_id):
 
     from iotiumlib import network
 
-    resp = network.getv2(filters={"cluster_id":cluster_id}).Response
+    resp = network.getv2(filters={"cluster_id":cluster_id, "inheritance":"false"}).Response
 
     op = list()
 
     if resp.output:
         for network in resp.output:
-            print(network)
+            #print(network)
             res = dict()
             res.update({'id':network['id'], 'name':network['name']})
             if 'is_wan_network' in network and network['is_wan_network']:
                 res.update({'wan':True})
             op.append(res)
 
     return op
```

### Comparing `iotiumlib-23.5.0/iotiumlib/image.py` & `iotiumlib-23.5.1/iotiumlib/image.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/models/role_creation_vo.py` & `iotiumlib-23.5.1/iotiumlib/models/role_creation_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/models/role_updation_vo.py` & `iotiumlib-23.5.1/iotiumlib/models/role_updation_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/models/service_listener_creation_vo.py` & `iotiumlib-23.5.1/iotiumlib/models/service_listener_creation_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/models/service_listener_update_vo.py` & `iotiumlib-23.5.1/iotiumlib/models/service_listener_update_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/models/service_ports_vo.py` & `iotiumlib-23.5.1/iotiumlib/models/service_ports_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/models/service_selector_vo.py` & `iotiumlib-23.5.1/iotiumlib/models/service_selector_vo.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/network.py` & `iotiumlib-23.5.1/iotiumlib/network.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/node.py` & `iotiumlib-23.5.1/iotiumlib/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,40 +60,45 @@
 
         def statssummary_inode(uri):
             return node.Stats(self, method='stats', uri=uri, filters=filters)
 
         def upgrade_inode(uri):
             return node.iNode(self, method='post', uri=uri)
 
+        def convert_to_cluster_inode(uri):
+            return node.iNode(self, method='post', uri=uri)
+
         _function_mapping = {
             'add': add_inode,
             'edit': edit_inode,
             'delete': delete_inode,
             'get': get_inode,
             'reboot': reboot_inode,
             'get_node_id': get_node_id_inode,
             'getv2': getv2_inode,
             'notifications': notifications_inode,
             'stats':stats_inode,
             'statssummary':statssummary_inode,
-            'upgrade': upgrade_inode
+            'upgrade': upgrade_inode,
+            'convert_to_cluster': convert_to_cluster_inode
         }
 
         self.uri = {
             add_inode: 'api/v1/node',
             get_inode: 'api/v1/node',
             getv2_inode: 'api/v2/node',
             edit_inode: 'api/v1/node/{nodeId}',
             delete_inode: 'api/v1/node/{nodeId}',
             get_node_id_inode: 'api/v1/node/{nodeId}',
             reboot_inode: 'api/v1/node/{nodeId}/reboot',
             notifications_inode:'api/v2/notification/node/{nodeId}/event',
             stats_inode:'api/v1/report/node/{nodeId}/stats',
             statssummary_inode: 'api/v1/report/node/{nodeId}/stats',
-            upgrade_inode: 'api/v1/node/{nodeId}/upgrade'
+            upgrade_inode: 'api/v1/node/{nodeId}/upgrade',
+            convert_to_cluster_inode: 'api/v1/node/{nodeId}/convert-to-cluster'
         }
 
         self.payload = resourcePaylod.iNode(payload).__dict__
 
         self.nodeId = node_id
         self.orgId = orch.id
 
@@ -309,7 +314,11 @@
     @staticmethod
     def statssummary(node_id):
         return node(node_id=node_id, action="statssummary")
 
     @staticmethod
     def upgrade(node_id, policy=None):
         return node(action='upgrade', node_id=node_id, payload=locals())
+
+    @staticmethod
+    def convert_to_cluster(node_id, cluster_name, election_network_type='WAN', instance_id=100, election_network_id=None):
+        return node(action='convert_to_cluster', node_id=node_id, payload=locals())
```

### Comparing `iotiumlib-23.5.0/iotiumlib/nodecli.py` & `iotiumlib-23.5.1/iotiumlib/nodecli.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/orch.py` & `iotiumlib-23.5.1/iotiumlib/orch.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/orchlogin.py` & `iotiumlib-23.5.1/iotiumlib/orchlogin.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/org.py` & `iotiumlib-23.5.1/iotiumlib/org.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/pki.py` & `iotiumlib-23.5.1/iotiumlib/pki.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/profile.py` & `iotiumlib-23.5.1/iotiumlib/profile.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/requires/Exceptions.py` & `iotiumlib-23.5.1/iotiumlib/requires/Exceptions.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/requires/commonVariables.py` & `iotiumlib-23.5.1/iotiumlib/requires/commonVariables.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/requires/commonWrapper.py` & `iotiumlib-23.5.1/iotiumlib/requires/commonWrapper.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/requires/resourcePayload.py` & `iotiumlib-23.5.1/iotiumlib/requires/resourcePayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,34 @@
                 self.container_timezone = getattr(containerTimeZoneObj, 'container_timezone')
 
             upgradePolicyObj = resourcePaylod.UpgradePolicy.Channel()
             if 'policy' in payload and payload['policy'] is not None:
                 setattr(upgradePolicyObj, 'policy', payload['policy'])
                 self.channel = getattr(upgradePolicyObj, 'policy')
 
+            cluster_name_Obj = resourcePaylod.Cluster.ClusterName()
+            if 'cluster_name' in payload and payload['cluster_name'] is not None:
+                setattr(cluster_name_Obj, 'name', payload['cluster_name'])
+                self.name = getattr(cluster_name_Obj, 'name')
+
+            cluster_config_Obj = resourcePaylod.Cluster.ClusterConfig()
+            self.config = dict()
+            if 'election_network_type' in payload and payload['election_network_type'] is not None:
+                setattr(cluster_config_Obj, 'election_network_type', payload['election_network_type'])
+                self.config.update(getattr(cluster_config_Obj, 'election_network_type'))
+
+            if 'instance_id' in payload and payload['instance_id'] is not None and payload['instance_id']:
+                setattr(cluster_config_Obj, "instance_id", payload["instance_id"])
+                self.config.update(getattr(cluster_config_Obj, 'instance_id'))
+
+            if 'election_network_id' in payload and payload['election_network_id'] is not None:
+                setattr(cluster_config_Obj, 'election_network_id', payload['election_network_id'])
+                self.config.update(getattr(cluster_config_Obj, 'election_network_id'))
+
+
         class nodeName(object):
             def __init__(self):
                 self._nodeName = str()
 
             @property
             def name(self):
                 return self._nodeName
```

### Comparing `iotiumlib-23.5.0/iotiumlib/requires/utils.py` & `iotiumlib-23.5.1/iotiumlib/requires/utils.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/secret.py` & `iotiumlib-23.5.1/iotiumlib/secret.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/service.py` & `iotiumlib-23.5.1/iotiumlib/service.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/sshkey.py` & `iotiumlib-23.5.1/iotiumlib/sshkey.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib/user.py` & `iotiumlib-23.5.1/iotiumlib/user.py`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/iotiumlib.egg-info/PKG-INFO` & `iotiumlib-23.5.1/iotiumlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotiumlib
-Version: 23.5.0
+Version: 23.5.1
 Summary: ioTium API library
 Home-page: https://view.com
 Author: Rashtrapathy C
 Author-email: rashtrapathy.chandrasekar@view.com
 License: Copyright 2023 View, Inc. | All Rights Reserved.
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: OS Independent
```

### Comparing `iotiumlib-23.5.0/iotiumlib.egg-info/SOURCES.txt` & `iotiumlib-23.5.1/iotiumlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iotiumlib-23.5.0/setup.py` & `iotiumlib-23.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iotiumlib",
-    version="23.5.00",
+    version="23.5.01",
     author="Rashtrapathy C",
     author_email="rashtrapathy.chandrasekar@view.com",
     description="ioTium API library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://view.com",
     packages=setuptools.find_packages(),
```

