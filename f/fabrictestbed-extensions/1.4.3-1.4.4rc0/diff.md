# Comparing `tmp/fabrictestbed-extensions-1.4.3.tar.gz` & `tmp/fabrictestbed-extensions-1.4.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.4.3.tar", last modified: Sat Apr 22 14:14:37 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.4.4rc0.tar", last modified: Thu May 11 21:15:21 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.4.3.tar` & `fabrictestbed-extensions-1.4.4rc0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-02-13 18:31:49.552350 fabrictestbed-extensions-1.4.3/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-04-06 16:18:57.453917 fabrictestbed-extensions-1.4.3/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-04-06 16:18:57.454239 fabrictestbed-extensions-1.4.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2022-08-18 16:55:06.303125 fabrictestbed-extensions-1.4.3/.gitignore
--rw-r--r--   0        0        0      666 2023-02-13 18:31:49.552528 fabrictestbed-extensions-1.4.3/.readthedocs.yaml
--rw-r--r--   0        0        0     2670 2023-04-22 14:13:43.304083 fabrictestbed-extensions-1.4.3/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-08-18 16:55:06.303384 fabrictestbed-extensions-1.4.3/LICENSE
--rw-r--r--   0        0        0     4054 2023-04-21 21:53:04.312013 fabrictestbed-extensions-1.4.3/README.md
--rw-r--r--   0        0        0      638 2022-08-18 16:55:06.303668 fabrictestbed-extensions-1.4.3/docs/Makefile
--rw-r--r--   0        0        0      799 2022-08-18 16:55:06.303743 fabrictestbed-extensions-1.4.3/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-02-13 18:31:49.552781 fabrictestbed-extensions-1.4.3/docs/source/conf.py
--rw-r--r--   0        0        0     8869 2022-10-28 15:15:07.136211 fabrictestbed-extensions-1.4.3/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-04-06 16:18:57.455278 fabrictestbed-extensions-1.4.3/docs/source/index.rst
--rw-r--r--   0        0        0      147 2023-04-22 14:13:43.304224 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.553082 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-02-13 18:31:49.553270 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-02-13 18:31:49.553528 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-02-13 18:31:49.553650 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2022-08-18 16:55:06.304986 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-02-13 18:31:49.553839 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21062 2023-04-20 18:01:14.628314 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    76799 2023-04-20 18:01:14.628593 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-02-13 18:31:49.554628 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    25967 2023-04-22 14:13:43.304449 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    39140 2023-04-20 18:01:14.628864 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    95919 2023-04-22 14:13:43.304819 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    34672 2023-04-20 18:01:14.629639 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81904 2023-04-20 18:01:14.629937 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555813 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2022-08-18 16:55:06.307676 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2022-08-18 16:55:06.307757 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2022-08-18 16:55:06.307862 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555903 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-02-13 18:31:49.556039 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-02-13 18:31:49.556263 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-02-13 18:31:49.556325 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-02-13 18:31:49.556445 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-02-13 18:31:49.556551 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-02-13 18:31:49.556711 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-02-13 18:31:49.556814 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-02-13 18:31:49.557045 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-02-13 18:31:49.557127 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-04-06 16:18:57.459146 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-02-13 18:31:49.557261 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-02-13 18:31:49.557349 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-02-13 18:31:49.557428 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-02-13 18:31:49.557517 fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1326 2023-04-21 16:27:35.017398 fabrictestbed-extensions-1.4.3/pyproject.toml
--rwxr-xr-x   0        0        0      122 2022-08-18 16:55:06.309489 fabrictestbed-extensions-1.4.3/sphinx.sh
--rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.4.4rc0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.4.4rc0/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.4.4rc0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1806 2023-05-11 21:15:01.565615 fabrictestbed-extensions-1.4.4rc0/.gitignore
+-rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.4.4rc0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2670 2023-05-11 18:23:24.342247 fabrictestbed-extensions-1.4.4rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.4.4rc0/LICENSE
+-rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.4.4rc0/README.md
+-rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.4.4rc0/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.4.4rc0/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.4.4rc0/docs/source/conf.py
+-rw-r--r--   0        0        0     8869 2023-05-11 18:23:24.343461 fabrictestbed-extensions-1.4.4rc0/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.4.4rc0/docs/source/index.rst
+-rw-r--r--   0        0        0      150 2023-05-11 21:11:09.747922 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21062 2023-05-11 18:23:24.345997 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    76799 2023-05-11 18:23:24.346796 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5807 2023-05-11 18:23:24.347162 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    25967 2023-05-11 18:23:24.347819 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    39991 2023-05-11 21:14:19.003686 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    95919 2023-05-11 18:23:24.348593 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    34672 2023-05-11 18:23:24.349105 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81904 2023-05-11 18:23:24.349763 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34231 2023-05-11 18:23:24.353058 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1326 2023-05-11 18:23:24.356954 fabrictestbed-extensions-1.4.4rc0/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.4.4rc0/sphinx.sh
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.4rc0/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.4.3/.github/workflows/build.yml` & `fabrictestbed-extensions-1.4.4rc0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.4.4rc0/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/.github/workflows/test.yml` & `fabrictestbed-extensions-1.4.4rc0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/.gitignore` & `fabrictestbed-extensions-1.4.4rc0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -123,7 +123,8 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+.idea/
```

### Comparing `fabrictestbed-extensions-1.4.3/.readthedocs.yaml` & `fabrictestbed-extensions-1.4.4rc0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/CHANGELOG.md` & `fabrictestbed-extensions-1.4.4rc0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/LICENSE` & `fabrictestbed-extensions-1.4.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/README.md` & `fabrictestbed-extensions-1.4.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/docs/Makefile` & `fabrictestbed-extensions-1.4.4rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/docs/make.bat` & `fabrictestbed-extensions-1.4.4rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/docs/source/conf.py` & `fabrictestbed-extensions-1.4.4rc0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/docs/source/fablib.rst` & `fabrictestbed-extensions-1.4.4rc0/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/docs/source/index.rst` & `fabrictestbed-extensions-1.4.4rc0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/interface.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -785,14 +785,33 @@
                 logging.debug(f"adding IP {i}")
                 ip_list.append(gateway + i + 1)
             return ip_list
         except Exception as e:
             logging.warning(f"Failed to get_available_ips: {e}")
             return None
 
+    def get_public_ips(self) -> List[IPv4Address] or List[IPv6Address] or None:
+        """
+        Get list of public IPs assigned to the FabNetv*Ext service
+        :return: List of Public IPs
+        :rtype: List[IPv4Address] or List[IPv6Address] or None
+        """
+        if self.get_fim_network_service().labels is not None:
+            if self.get_fim_network_service().labels.ipv4 is not None:
+                result = []
+                for x in self.get_fim_network_service().labels.ipv4:
+                    result.append(IPv4Address(x))
+                return result
+            elif self.get_fim_network_service().labels.ipv6 is not None:
+                result = []
+                for x in self.get_fim_network_service().labels.ipv6:
+                    result.append(IPv4Address(x))
+                return result
+        return None
+
     def get_subnet(self) -> IPv4Network or IPv6Network or None:
         """
         Gets the assigned subnet for a FABnet L3 IPv6 or IPv4 network
 
         :return: gateway IP
         :rtype: IPv4Network or IPv6Network
         """
```

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/fablib/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.4.4rc0/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/pyproject.toml` & `fabrictestbed-extensions-1.4.4rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.3/PKG-INFO` & `fabrictestbed-extensions-1.4.4rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.4.3
+Version: 1.4.4rc0
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

