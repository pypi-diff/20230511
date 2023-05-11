# Comparing `tmp/aerleon-1.2.2.tar.gz` & `tmp/aerleon-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerleon-1.2.2.tar", max compression
+gzip compressed data, was "aerleon-1.2.3.tar", max compression
```

## Comparing `aerleon-1.2.2.tar` & `aerleon-1.2.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    11358 2023-03-30 05:56:37.789229 aerleon-1.2.2/LICENSE
--rw-r--r--   0        0        0     6805 2023-03-30 05:56:37.789229 aerleon-1.2.2/README.md
--rw-r--r--   0        0        0       15 2023-03-30 05:56:37.789229 aerleon-1.2.2/aerleon/__init__.py
--rw-r--r--   0        0        0     4200 2023-03-30 05:56:37.789229 aerleon-1.2.2/aerleon/aclcheck_cmdline.py
--rw-r--r--   0        0        0    17921 2023-03-30 05:56:37.789229 aerleon-1.2.2/aerleon/aclgen.py
--rw-r--r--   0        0        0    13124 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/api.py
--rw-r--r--   0        0        0    11358 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/COPYING
--rw-r--r--   0        0        0       29 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/__init__.py
--rwxr-xr-x   0        0        0    11008 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/aclcheck.py
--rw-r--r--   0        0        0    24211 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/aclgenerator.py
--rw-r--r--   0        0        0     4379 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/addressbook.py
--rw-r--r--   0        0        0     2792 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/arista.py
--rw-r--r--   0        0        0    36010 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/arista_tp.py
--rw-r--r--   0        0        0     9960 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/aruba.py
--rw-r--r--   0        0        0     1116 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/brocade.py
--rw-r--r--   0        0        0    39693 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/cisco.py
--rw-r--r--   0        0        0    14398 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/ciscoasa.py
--rw-r--r--   0        0        0     2754 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/cisconx.py
--rw-r--r--   0        0        0     2428 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/ciscoxr.py
--rw-r--r--   0        0        0     9944 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/cloudarmor.py
--rw-r--r--   0        0        0     7737 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/demo.py
--rw-r--r--   0        0        0    24959 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/gce.py
--rw-r--r--   0        0        0     4759 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/gcp.py
--rw-r--r--   0        0        0    24246 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/gcp_hf.py
--rw-r--r--   0        0        0     9076 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/ipset.py
--rw-r--r--   0        0        0    38752 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/iptables.py
--rw-r--r--   0        0        0    43610 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/juniper.py
--rw-r--r--   0        0        0     5090 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/juniperevo.py
--rw-r--r--   0        0        0    31792 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/junipermsmpc.py
--rw-r--r--   0        0        0    37589 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/junipersrx.py
--rw-r--r--   0        0        0    14357 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/k8s.py
--rw-r--r--   0        0        0    17948 2023-03-30 05:56:37.793229 aerleon-1.2.2/aerleon/lib/nacaddr.py
--rw-r--r--   0        0        0    38627 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/naming.py
--rw-r--r--   0        0        0    32482 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/nftables.py
--rw-r--r--   0        0        0    24510 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/nsxv.py
--rw-r--r--   0        0        0    10007 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/openconfig.py
--rw-r--r--   0        0        0    23249 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/packetfilter.py
--rw-r--r--   0        0        0    49360 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/paloaltofw.py
--rw-r--r--   0        0        0    17077 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/pcap.py
--rw-r--r--   0        0        0     3411 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/plugin.py
--rw-r--r--   0        0        0    13283 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/plugin_supervisor.py
--rw-r--r--   0        0        0    97241 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/policy.py
--rw-r--r--   0        0        0    39221 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/policy_builder.py
--rw-r--r--   0        0        0    21395 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/policy_simple.py
--rw-r--r--   0        0        0     9162 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/policyreader.py
--rw-r--r--   0        0        0     4940 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/port.py
--rw-r--r--   0        0        0    14617 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/recognizers.py
--rw-r--r--   0        0        0     1316 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/speedway.py
--rw-r--r--   0        0        0     2405 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/srxlo.py
--rw-r--r--   0        0        0     8991 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/summarizer.py
--rw-r--r--   0        0        0    14092 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/windows.py
--rw-r--r--   0        0        0     6118 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/windows_advfirewall.py
--rw-r--r--   0        0        0     9096 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/windows_ipsec.py
--rw-r--r--   0        0        0    12540 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/yaml.py
--rw-r--r--   0        0        0     1140 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/lib/yaml_loader.py
--rw-r--r--   0        0        0        0 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/utils/__init__.py
--rw-r--r--   0        0        0     3240 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/utils/config.py
--rw-r--r--   0        0        0     3592 2023-03-30 05:56:37.797229 aerleon-1.2.2/aerleon/utils/iputils.py
--rw-r--r--   0        0        0     2712 2023-03-30 05:56:37.805229 aerleon-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 05:56:37.857229 aerleon-1.2.2/tools/__init__.py
--rw-r--r--   0        0        0    16234 2023-03-30 05:56:37.857229 aerleon-1.2.2/tools/cgrep.py
--rw-r--r--   0        0        0     1794 2023-03-30 05:56:37.857229 aerleon-1.2.2/tools/iputilstools.py
--rw-r--r--   0        0        0     8210 1970-01-01 00:00:00.000000 aerleon-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-11 03:19:35.480076 aerleon-1.2.3/LICENSE
+-rw-r--r--   0        0        0     6805 2023-05-11 03:19:35.480076 aerleon-1.2.3/README.md
+-rw-r--r--   0        0        0       15 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/__init__.py
+-rw-r--r--   0        0        0     4200 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/aclcheck_cmdline.py
+-rw-r--r--   0        0        0    17921 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/aclgen.py
+-rw-r--r--   0        0        0    13124 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/api.py
+-rw-r--r--   0        0        0    11358 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/COPYING
+-rw-r--r--   0        0        0       29 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/__init__.py
+-rwxr-xr-x   0        0        0    11008 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/aclcheck.py
+-rw-r--r--   0        0        0    24649 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/aclgenerator.py
+-rw-r--r--   0        0        0     4517 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/addressbook.py
+-rw-r--r--   0        0        0     2792 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/arista.py
+-rw-r--r--   0        0        0    36176 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/arista_tp.py
+-rw-r--r--   0        0        0    10035 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/aruba.py
+-rw-r--r--   0        0        0     1116 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/brocade.py
+-rw-r--r--   0        0        0    39710 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/cisco.py
+-rw-r--r--   0        0        0    14390 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/ciscoasa.py
+-rw-r--r--   0        0        0     2754 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/cisconx.py
+-rw-r--r--   0        0        0     2428 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/ciscoxr.py
+-rw-r--r--   0        0        0     9968 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/cloudarmor.py
+-rw-r--r--   0        0        0     7737 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/demo.py
+-rw-r--r--   0        0        0    24978 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/gce.py
+-rw-r--r--   0        0        0     4759 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/gcp.py
+-rw-r--r--   0        0        0    24295 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/gcp_hf.py
+-rw-r--r--   0        0        0     9076 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/ipset.py
+-rw-r--r--   0        0        0    38752 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/iptables.py
+-rw-r--r--   0        0        0    43950 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/juniper.py
+-rw-r--r--   0        0        0     5090 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/juniperevo.py
+-rw-r--r--   0        0        0    32101 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/junipermsmpc.py
+-rw-r--r--   0        0        0    37947 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/junipersrx.py
+-rw-r--r--   0        0        0    14344 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/k8s.py
+-rw-r--r--   0        0        0    17897 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/nacaddr.py
+-rw-r--r--   0        0        0    38706 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/naming.py
+-rw-r--r--   0        0        0    33371 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/nftables.py
+-rw-r--r--   0        0        0    24741 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/nsxv.py
+-rw-r--r--   0        0        0     9988 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/openconfig.py
+-rw-r--r--   0        0        0    23249 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/packetfilter.py
+-rw-r--r--   0        0        0    49360 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/paloaltofw.py
+-rw-r--r--   0        0        0    17077 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/pcap.py
+-rw-r--r--   0        0        0     3411 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/plugin.py
+-rw-r--r--   0        0        0    13283 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/plugin_supervisor.py
+-rw-r--r--   0        0        0    97220 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/policy.py
+-rw-r--r--   0        0        0    39221 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/policy_builder.py
+-rw-r--r--   0        0        0    21391 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/policy_simple.py
+-rw-r--r--   0        0        0     9162 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/policyreader.py
+-rw-r--r--   0        0        0     4948 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/port.py
+-rw-r--r--   0        0        0    14617 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/recognizers.py
+-rw-r--r--   0        0        0     1316 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/speedway.py
+-rw-r--r--   0        0        0     2405 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/srxlo.py
+-rw-r--r--   0        0        0     9069 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/summarizer.py
+-rw-r--r--   0        0        0    14092 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/windows.py
+-rw-r--r--   0        0        0     6118 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/windows_advfirewall.py
+-rw-r--r--   0        0        0     9096 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/windows_ipsec.py
+-rw-r--r--   0        0        0    12540 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/yaml.py
+-rw-r--r--   0        0        0     1140 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/yaml_loader.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/utils/__init__.py
+-rw-r--r--   0        0        0     3240 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/utils/config.py
+-rw-r--r--   0        0        0     3592 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/utils/iputils.py
+-rw-r--r--   0        0        0     2712 2023-05-11 03:19:35.492076 aerleon-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 03:19:35.540077 aerleon-1.2.3/tools/__init__.py
+-rw-r--r--   0        0        0    16234 2023-05-11 03:19:35.540077 aerleon-1.2.3/tools/cgrep.py
+-rw-r--r--   0        0        0     1794 2023-05-11 03:19:35.540077 aerleon-1.2.3/tools/iputilstools.py
+-rw-r--r--   0        0        0     8210 1970-01-01 00:00:00.000000 aerleon-1.2.3/PKG-INFO
```

### Comparing `aerleon-1.2.2/LICENSE` & `aerleon-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/README.md` & `aerleon-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/aclcheck_cmdline.py` & `aerleon-1.2.3/aerleon/aclcheck_cmdline.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/aclgen.py` & `aerleon-1.2.3/aerleon/aclgen.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/api.py` & `aerleon-1.2.3/aerleon/api.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/COPYING` & `aerleon-1.2.3/aerleon/lib/COPYING`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/aclcheck.py` & `aerleon-1.2.3/aerleon/lib/aclcheck.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/aclgenerator.py` & `aerleon-1.2.3/aerleon/lib/aclgenerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """ACL Generator base class."""
 
 import copy
 import datetime
 import hashlib
 import re
 import string
-from typing import Dict, List, Union
+from typing import Dict, List, Set, Tuple, Union
 
 from absl import logging
 
 from aerleon.lib import policy
 
 
 # generic error class
@@ -121,30 +121,30 @@
 
     NO_AF_LOG_PROTO = string.Template(
         'Term $term will not be rendered, as it has'
         ' $proto match specified but the ACL is of'
         ' $af address family.'
     )
 
-    def __init__(self, term):
+    def __init__(self, term: policy.Term) -> None:
         if term.protocol:
             for protocol in term.protocol:
                 if protocol not in self.PROTO_MAP and str(protocol) not in [
                     str(p) for p in self.PROTO_MAP_BY_NUMBER
                 ]:
                     raise UnsupportedFilterError(
                         'Protocol(s) %s are not supported.' % str(term.protocol)
                     )
 
             term.protocol = ProtocolNameToNumber(
                 term.protocol, self.ALWAYS_PROTO_NUM, self.PROTO_MAP
             )
         self.term = term
 
-    def NormalizeAddressFamily(self, af):
+    def NormalizeAddressFamily(self, af: Union[int, str]) -> int:
         """Convert (if necessary) address family name to numeric value.
 
         Args:
           af: Address family, can be either numeric or string (e.g. 4 or 'inet')
 
         Returns:
           af: Numeric address family value
@@ -160,15 +160,17 @@
             af = self.AF_MAP[af]
         else:
             raise UnsupportedAFError(
                 'Address family %s is not supported, ' 'term %s.' % (af, self.term.name)
             )
         return af
 
-    def NormalizeIcmpTypes(self, icmp_types, protocols, af):
+    def NormalizeIcmpTypes(
+        self, icmp_types: List[str], protocols: List[str], af: int
+    ) -> List[int]:
         """Return verified list of appropriate icmp-types.
 
         Args:
           icmp_types: list of icmp_types
           protocols: list of protocols
           af: address family of this term, either numeric or text (see self.AF_MAP)
 
@@ -289,15 +291,15 @@
         ('replies', 'RPL'),
         ('request', 'REQ'),
     ]
     # Maximum term length. Can be overridden by generator to enforce
     # platform specific restrictions.
     _TERM_MAX_LENGTH = 62
 
-    def __init__(self, pol, exp_info):
+    def __init__(self, pol: policy.Policy, exp_info: int) -> None:
         """Initialise an ACLGenerator.  Store policy structure for processing."""
         supported_tokens, supported_sub_tokens = self._GetSupportedTokens()
 
         pol.filters[:] = [
             (header, terms)
             for (header, terms) in pol.filters
             if (self._PLATFORM in header.platforms)
@@ -343,20 +345,20 @@
             continue
         if all_err:
             raise UnsupportedFilterError('\n %s' % '\n'.join(all_err))
         if all_warn:
             logging.debug('\n %s', '\n'.join(all_warn))
         self._TranslatePolicy(pol, exp_info)
 
-    def _TranslatePolicy(self, pol, exp_info):
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int) -> None:
         # pylint: disable=unused-argument
         """Translate policy contents to platform specific data structures."""
         raise Error('%s does not implement _TranslatePolicies()' % self._PLATFORM)
 
-    def _BuildTokens(self):
+    def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Provide a default for supported tokens and sub tokens.
 
         Returns:
           tuple containing both supported tokens and sub tokens
         """
         # Set of supported keywords for a given platform.  Values should be in
         # undercase form, eg, icmp_type (not icmp-type)
@@ -401,15 +403,15 @@
                 'reject',
                 'reject-with-tcp-rst',
             },
             'icmp_type': set(list(Term.ICMP_TYPE[4].keys()) + list(Term.ICMP_TYPE[6].keys())),
         }
         return supported_tokens, supported_sub_tokens
 
-    def _GetSupportedTokens(self):
+    def _GetSupportedTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Build our supported tokens and sub tokens.
 
         Returns:
           tuple containing the supported tokens and sub tokens.
         Raises:
           UnsupportedFilterError: Raised when token is not supported.
         """
@@ -422,15 +424,17 @@
                 'Found undefined sub tokens missing from the supported token list! '
                 'These must match. (%s)' % ' '.join(undefined_st)
             )
         # all good.
         return supported_tokens, supported_sub_tokens
 
     # TODO(robankeny) Fix this function, it no longer does what it says.
-    def FixHighPorts(self, term, af='inet', all_protocols_stateful=False):
+    def FixHighPorts(
+        self, term: policy.Term, af: str = 'inet', all_protocols_stateful: bool = False
+    ):
         """Evaluate protocol and ports of term, return sane version of term.
 
         Args:
           term: Term object to be checked
           af: String presenting the address family, inet, inet6
           all_protocols_stateful: Boolean suggesting if protocols are all stateful.
 
@@ -481,15 +485,21 @@
                     raise EstablishedError(
                         '%s %s %s %s' % (errmsg, unstateful_protocols, 'in term', term.name)
                     )
                 break
 
         return mod
 
-    def FixTermLength(self, term_name, abbreviate=False, truncate=False, override_max_length=None):
+    def FixTermLength(
+        self,
+        term_name: str,
+        abbreviate: bool = False,
+        truncate: bool = False,
+        override_max_length: int = None,
+    ):
         """Return a term name which is equal or shorter than _TERM_MAX_LENGTH.
 
            New term is obtained in two steps. First, if allowed, automatic
            abbreviation is performed using hardcoded abbreviation table. Second,
            if allowed, term name is truncated to specified limit.
 
         Args:
@@ -519,15 +529,15 @@
         raise TermNameTooLongError(
             'Term %s (originally %s) is '
             'too long. Limit is %d characters (vs. %d) '
             'and no abbreviations remain or abbreviations '
             'disabled.' % (new_term, term_name, override_max_length, len(new_term))
         )
 
-    def HexDigest(self, name, truncation_length=None):
+    def HexDigest(self, name: str, truncation_length: int = None):
         """Return a hexadecimal digest of the name object.
 
         Args:
           name: Name to hash.
           truncation_length: Truncation to shorten the digest length if necessary.
         Returns:
           A hexadecimal digest of the input name.
@@ -536,15 +546,15 @@
         """
 
         if truncation_length is None:
             truncation_length = 64
         name_bytes = name.encode('UTF-8')
         return hashlib.sha256(name_bytes).hexdigest()[:truncation_length]
 
-    def _FilteredTerms(self, header, terms, exp_info):
+    def _FilteredTerms(self, header: policy.Header, terms: List[policy.Term], exp_info: int):
         new_terms = []
         filter_name = header.FilterName(self._PLATFORM)
         current_date = datetime.datetime.utcnow().date()
         exp_info_date = current_date + datetime.timedelta(weeks=exp_info)
 
         for term in terms:
             if term.expiration:
@@ -627,15 +637,15 @@
     if date:
         tags.append('%s%s' % (prefix, p4_date))
     if revision:
         tags.append('%s%s' % (prefix, p4_revision))
     return tags
 
 
-def WrapWords(textlist, size, joiner='\n'):
+def WrapWords(textlist: List[str], size: int, joiner: str = '\n'):
     r"""Insert breaks into the listed strings at specified width.
 
     Args:
       textlist: a list of text strings
       size: width of reformated strings
       joiner: text to insert at break.  eg. '\n  ' to add an indent.
     Returns:
```

### Comparing `aerleon-1.2.2/aerleon/lib/addressbook.py` & `aerleon-1.2.3/aerleon/lib/addressbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import collections
 import heapq
 import ipaddress
 import itertools
+from typing import List, Union
+
+from aerleon.lib.nacaddr import IPv4, IPv6
 
 
 class Addressbook:
-    def __init__(self):
+    def __init__(self) -> None:
         self.addressbook = collections.OrderedDict()
 
-    def AddAddresses(self, zone, address_list):
+    def AddAddresses(self, zone: str, address_list: List[Union[IPv4, IPv6]]):
         """Create the address book configuration entries.
 
         Args:
           zone: the zone these objects will reside in
           address_list: a list of naming library address objects
             that will reside in the zone
 
         _BuildAddressBook will add the given addresses to the address book
         for 'zone', grouped by address.parent_name. It will ignore any redundant networks.
         A redundant network is fully contained by an equal or larger network in the list.
         A smaller network already present in the address book will be removed if made redundant
         when new networks are added.
         """
 
-        def _drop_subnets(address_list):
+        def _drop_subnets(address_list: List[Union[IPv4, IPv6]]):
             """Remove any network contained by another network in this list.
 
             Args:
                 address_list: a list of IP objects sorted ascending by version and address.
 
             Yields:
                 yields the items of the address list in order with redundant subnets removed.
```

### Comparing `aerleon-1.2.2/aerleon/lib/arista.py` & `aerleon-1.2.3/aerleon/lib/arista.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/arista_tp.py` & `aerleon-1.2.3/aerleon/lib/arista_tp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 
 import copy
 import re
 from typing import Dict, List, Set, Tuple, Union
 
 from absl import logging
 
-from aerleon.lib import aclgenerator
+from aerleon.lib import aclgenerator, policy
 from aerleon.lib.nacaddr import IPv4, IPv6
-from aerleon.lib.policy import Policy
 
 """
           1         2         3
  123456789012345678901234567890123456789
  traffic-policies
     traffic-policy foo
       match dos-attaqrs-source-ip ipv4    << TERM_INDENT
@@ -147,15 +146,15 @@
             "addr_fam": "ipv4",
         },
         "inet6": {
             "addr_fam": "ipv6",
         },
     }
 
-    def __init__(self, term, term_type, noverbose) -> None:
+    def __init__(self, term: policy.Term, term_type: str, noverbose: bool) -> None:
         super().__init__(term)
         self.term = term
         self.term_type = term_type  # drives the address-family
         self.noverbose = noverbose
 
         if term_type not in self._TERM_TYPE:
             raise ValueError("unknown filter type: %s" % term_type)
@@ -389,28 +388,28 @@
         term_block.append([TERM_INDENT, "!", False])  # end of match entry
 
         for tindent, tstr, tverb in term_block:
             config.Append(tindent, tstr, verbatim=tverb)
 
         return str(config)
 
-    def _processPorts(self, term) -> str:
+    def _processPorts(self, term: policy.Term) -> str:
         port_str = ""
 
         # source port generation
         if term.source_port:
             port_str += " source port %s" % self._Group(term.source_port)
 
         # destination port
         if term.destination_port:
             port_str += " destination port %s" % self._Group(term.destination_port)
 
         return port_str
 
-    def _processICMP(self, term) -> Tuple[str, str]:
+    def _processICMP(self, term: policy.Term) -> Tuple[str, str]:
         icmp_types = [""]
         icmp_code_str = ""
         icmp_type_str = " type "
 
         if term.icmp_type:
             icmp_types = self.NormalizeIcmpTypes(term.icmp_type, term.protocol, self.term_type)
         if icmp_types != [""]:
@@ -425,15 +424,15 @@
         if self.term.icmp_code and len(icmp_types) <= 1:
             icmp_codes = self._Group(self.term.icmp_code)
             icmp_codes = re.sub(r" ", ",", icmp_codes)
             icmp_code_str += " code %s" % icmp_codes
 
         return icmp_type_str, icmp_code_str
 
-    def _processProtocol(self, term_type, term, flags) -> str:
+    def _processProtocol(self, term_type: str, term: policy.Term, flags: List[str]) -> str:
         anet_proto_map = {
             "inet": {
                 # <1-255> protocol  values(s) or range(s) of protocol  values
                 "ahp": "",
                 "bgp": "",
                 "icmp": "",
                 "igmp": "",
@@ -481,15 +480,15 @@
             protocol_str += "protocol %s" % self._Group(prots)
 
         if prots == ["tcp"] and flags:
             protocol_str += " flags " + " ".join(flags)
 
         return protocol_str
 
-    def _processProtocolExcept(self, term_type, term, flags) -> str:
+    def _processProtocolExcept(self, term_type: str, term: policy.Term, flags: List[str]) -> str:
         # EOS does not have a protocol-except keyword. it does, however, support
         # lists of protocol-ids. given a term this function will generate the
         # appropriate list of protocol-id's which *will* be permited. within the
         # supported range of addaress family protocols.
         protocol_range = {
             "inet": 1,
             "inet6": 0,
@@ -517,15 +516,17 @@
                 ptr = p + 1
 
         ex_str += str(ptr) + "-" + "255"
         protocol_str = "protocol " + ex_str
 
         return protocol_str
 
-    def _processTermOptions(self, term, options) -> Tuple[List[str], List[str]]:
+    def _processTermOptions(
+        self, term: policy.Term, options: List[str]
+    ) -> Tuple[List[str], List[str]]:
         flags = []
         misc_options = []
 
         for opt in [str(x) for x in options]:
             # note: traffic policies support additional tcp flags. for now,
             # only handle the required elements
             #
@@ -550,15 +551,15 @@
                 flags.append("rst")
             elif "fragment" in opt:
                 # handles the is-fragment and first-fragment options
                 misc_options.append("fragment")
 
         return flags, misc_options
 
-    def _Group(self, group, lc=True) -> str:
+    def _Group(self, group: List[Union[str, Tuple[int, int]]], lc: bool = True) -> str:
         """If 1 item return it, else return [item1 item2].
 
         Args:
           group: a list.  could be a list of strings(protocols) or a list of
                  tuples(ports)
           lc: return a lower cased result for text.  Default is True.
 
@@ -715,15 +716,15 @@
         for p in ex_pfxs:
             field_list += (" " * 6) + "except %s\n" % p
 
         fieldset_hdr = "field-set " + af + " prefix " + direction + "-" + ("%s" % name) + "\n"
         field_set = fieldset_hdr + field_list
         return field_set
 
-    def _TranslatePolicy(self, pol: Policy, exp_info: int) -> None:
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int) -> None:
         self.arista_traffic_policies = []
         af_map_txt = {"inet": "ipv4", "inet6": "ipv6"}
 
         for header, terms in pol.filters:
             filter_options = header.FilterOptions(self._PLATFORM)
             filter_name = header.FilterName(self._PLATFORM)
             noverbose = "noverbose" in filter_options[1:]
```

### Comparing `aerleon-1.2.2/aerleon/lib/aruba.py` & `aerleon-1.2.3/aerleon/lib/aruba.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Aruba generator."""
 
-from typing import Dict, List, Set, Tuple
+from typing import Dict, List, Set, Tuple, Union
 
-from absl import logging
-
-from aerleon.lib import aclgenerator
-from aerleon.lib.policy import Policy
+from aerleon.lib import aclgenerator, policy
+from aerleon.lib.nacaddr import IPv4, IPv6
 
 _COMMENT_MARKER = '#'
 _TERMINATOR_MARKER = '!'
 
 
 class Error(aclgenerator.Error):
     """Base error class."""
@@ -65,15 +63,15 @@
 
     _PROTOCOL_MAP = {
         'icmp': 1,
         'gre': 47,
         'esp': 50,
     }
 
-    def __init__(self, term, filter_type, verbose=True) -> None:
+    def __init__(self, term: policy.Term, filter_type: str, verbose: bool = True) -> None:
         super().__init__(term)
         self.term = term
         self.filter_type = filter_type
         self.netdestinations = []
         self.verbose = verbose
 
     def __str__(self) -> str:
@@ -153,15 +151,15 @@
             str_tok.append(self._ACTIONS.get(self.term.action[0]))
             ret_str.append(' '.join(t for t in str_tok if t))
 
         self.netdestinations = netdestinations
 
         return '\n'.join(t for t in ret_str if t)
 
-    def _GenerateNetdest(self, addr_netdestid, addresses, af) -> str:
+    def _GenerateNetdest(self, addr_netdestid: str, addresses: Union[IPv4, IPv6], af: int) -> str:
         """Generates the netdestinations text block.
 
         Args:
           addr_netdestid: netdestinations identifier.
           addresses: IP addresses.
           af: address family.
         Returns:
@@ -177,15 +175,15 @@
         for address in addresses:
             ret_str.append('%s%s' % (self._IDENT, self._GenerateNetworkOrHostTokens(address)))
 
         ret_str.append('%s\n' % _TERMINATOR_MARKER)
 
         return '\n'.join(t for t in ret_str if t)
 
-    def _GenerateNetworkOrHostTokens(self, address) -> str:
+    def _GenerateNetworkOrHostTokens(self, address: Union[IPv4, IPv6]) -> str:
         """Generates the text block host or network identifier for netdestinations.
 
         Args:
           address: IP address.
         Returns:
           A string line using either 'host' or 'network', properly formatted for
           Aruba ACLs.
@@ -263,15 +261,15 @@
             }
         )
 
         del supported_sub_tokens['icmp_type']
 
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol: Policy, exp_info: int) -> None:
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int) -> None:
         self.aruba_policies = []
 
         for header, terms in pol.filters:
             filter_name = header.FilterName(self._PLATFORM)
             filter_options = header.FilterOptions(self._PLATFORM)
             verbose = True
             if 'noverbose' in filter_options:
```

### Comparing `aerleon-1.2.2/aerleon/lib/brocade.py` & `aerleon-1.2.3/aerleon/lib/brocade.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/cisco.py` & `aerleon-1.2.3/aerleon/lib/cisco.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     # Full port map data structure
     _PORT_MAP = {
         'cisco': {'tcp': _CISCO_PORTS_TCP, 'udp': _CISCO_PORTS_UDP, 'icmp': _TYPES_ICMP},
         'arista': {'tcp': _ARISTA_PORTS_TCP, 'udp': _ARISTA_PORTS_UDP, 'icmp': _TYPES_ICMP},
     }
 
     @staticmethod
-    def GetProtocol(port_num, proto, platform='cisco'):
+    def GetProtocol(port_num: int, proto: str, platform: str = 'cisco'):
         """Converts a port number to a name or returns the number.
 
         Args:
           port_num: integer representing the port number.
           proto: string representing proto (tcp, udp, etc).
           platform: string representing platform (cisco, arista)
```

### Comparing `aerleon-1.2.2/aerleon/lib/ciscoasa.py` & `aerleon-1.2.3/aerleon/lib/ciscoasa.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,33 +227,33 @@
         # inet4
         if isinstance(saddr, nacaddr.IPv4) or isinstance(saddr, ipaddress.IPv4Network):
             saddr = cast(self.IPV4_ADDRESS, saddr)
             if saddr.num_addresses > 1:
                 saddr = '%s %s' % (saddr.network_address, saddr.netmask)
             else:
                 saddr = 'host %s' % (saddr.network_address)
-        elif isinstance(daddr, nacaddr.IPv4) or isinstance(daddr, ipaddress.IPv4Network):
+        if isinstance(daddr, nacaddr.IPv4) or isinstance(daddr, ipaddress.IPv4Network):
             daddr = cast(self.IPV4_ADDRESS, daddr)
             if daddr.num_addresses > 1:
                 daddr = '%s %s' % (daddr.network_address, daddr.netmask)
             else:
                 daddr = 'host %s' % (daddr.network_address)
-        elif isinstance(saddr, summarizer.DSMNet):
+        if isinstance(saddr, summarizer.DSMNet):
             saddr = '%s %s' % summarizer.ToDottedQuad(saddr, negate=False)
 
         if isinstance(daddr, summarizer.DSMNet):
             daddr = '%s %s' % summarizer.ToDottedQuad(daddr, negate=False)
         # inet6
-        elif isinstance(saddr, nacaddr.IPv6) or isinstance(saddr, ipaddress.IPv6Network):
+        if isinstance(saddr, nacaddr.IPv6) or isinstance(saddr, ipaddress.IPv6Network):
             saddr = cast(self.IPV6_ADDRESS, saddr)
             if saddr.num_addresses > 1:
                 saddr = '%s/%s' % (saddr.network_address, saddr.prefixlen)
             else:
                 saddr = 'host %s' % (saddr.network_address)
-        elif isinstance(daddr, nacaddr.IPv6) or isinstance(daddr, ipaddress.IPv6Network):
+        if isinstance(daddr, nacaddr.IPv6) or isinstance(daddr, ipaddress.IPv6Network):
             daddr = cast(self.IPV6_ADDRESS, daddr)
             if daddr.num_addresses > 1:
                 daddr = '%s/%s' % (daddr.network_address, daddr.prefixlen)
             else:
                 daddr = 'host %s' % (daddr.network_address)
 
         # fix ports
```

### Comparing `aerleon-1.2.2/aerleon/lib/cisconx.py` & `aerleon-1.2.3/aerleon/lib/cisconx.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/ciscoxr.py` & `aerleon-1.2.3/aerleon/lib/ciscoxr.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/cloudarmor.py` & `aerleon-1.2.3/aerleon/lib/cloudarmor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 import copy
 import json
 import sys
 from typing import Dict, List, Set, Tuple
 
 from absl import logging
 
-from aerleon.lib import aclgenerator
-from aerleon.lib.policy import Policy
+from aerleon.lib import aclgenerator, policy
 
 if sys.version_info < (3, 8):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 # Generic error class
@@ -49,24 +48,26 @@
     # Max srcIpRanges within a single term
     _MAX_IP_RANGES_PER_TERM = 5
 
     ACTION_MAP = {'accept': 'allow', 'deny': 'deny(404)'}
 
     _MAX_TERM_COMMENT_LENGTH = 64
 
-    def __init__(self, term, address_family='inet', verbose=True) -> None:
+    def __init__(
+        self, term: policy.Term, address_family: str = 'inet', verbose: bool = True
+    ) -> None:
         super().__init__(term)
         self.term = term
         self.address_family = address_family
         self.verbose = verbose
 
     def __str__(self) -> str:
         return ''
 
-    def ConvertToDict(self, priority_index) -> List[PolicyRule]:
+    def ConvertToDict(self, priority_index: int) -> List[PolicyRule]:
         """Converts term to dictionary representation of CloudArmor's JSON format.
 
         Takes all of the attributes associated with a term (match, action, etc) and
         converts them into a dictionary which most closely represents
         the CloudArmor API's JSON rule format. Additionally, splits a single term
         into multiple terms if the number of srcIpRanges exceed
         _MAX_IP_RANGES_PER_TERM.
@@ -197,15 +198,15 @@
             'source_address_exclude',
             'source_port',
             'verbatim',
         }
         supported_sub_tokens = {'action': {'accept', 'deny'}}
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol: Policy, exp_info: int) -> None:
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int) -> None:
         """Translates a Aerleon policy into a CloudArmor-specific data structure.
 
         Takes in a POL file, parses each term and populates the cloudarmor_policies
         list. Each term in this list is a dictionary formatted according to
         CloudArmor's rule API specification.
 
         Args:
```

### Comparing `aerleon-1.2.2/aerleon/lib/demo.py` & `aerleon-1.2.3/aerleon/lib/demo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/gce.py` & `aerleon-1.2.3/aerleon/lib/gce.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 import json
 import re
 import sys
 from typing import Dict, List, Set, Tuple, Union
 
 from absl import logging
 
-from aerleon.lib import gcp, nacaddr
-from aerleon.lib.policy import Policy, Term
+from aerleon.lib import gcp, nacaddr, policy
 
 if sys.version_info < (3, 8):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 
@@ -68,15 +67,15 @@
         "denied": "list[L4Matcher]",
         "direction": str,  # Actually Enum
         "logConfig": LogConfig,
     },
 )
 
 
-def IsDefaultDeny(term: Term) -> bool:
+def IsDefaultDeny(term: policy.Term) -> bool:
     """Returns true if a term is a default deny without IPs, ports, etc."""
     skip_attrs = [
         'flattened',
         'flattened_addr',
         'flattened_saddr',
         'flattened_daddr',
         'action',
@@ -143,15 +142,17 @@
             'all',  # Needed for default deny, do not use in policy file.
         ]
     )
 
     # Any protocol not in _ALLOW_PROTO_NAME must be passed by number.
     ALWAYS_PROTO_NUM = set(gcp.Term.PROTO_MAP.keys()) - _ALLOW_PROTO_NAME
 
-    def __init__(self, term, inet_version='inet', policy_inet_version='inet') -> None:
+    def __init__(
+        self, term: policy.Term, inet_version: str = 'inet', policy_inet_version: str = 'inet'
+    ) -> None:
         super().__init__(term)
         self.term = term
         self.inet_version = inet_version
         # This is to handle mixed, where the policy_inet_version is mixed,
         # but the term inet version is either inet/inet6.
         # This is only useful for term name and priority.
         self.policy_inet_version = policy_inet_version
@@ -462,15 +463,15 @@
         # remove unsupported things
         supported_tokens -= {'icmp_type', 'verbatim'}
         # easier to make a new structure
         supported_sub_tokens = {'action': {'accept', 'deny'}}
 
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol: Policy, exp_info: int) -> None:
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int) -> None:
         self.gce_policies = []
         max_attribute_count = 0
         total_attribute_count = 0
         total_rule_count = 0
 
         for header, terms in pol.filters:
             filter_options = header.FilterOptions(self._PLATFORM)
```

### Comparing `aerleon-1.2.2/aerleon/lib/gcp.py` & `aerleon-1.2.3/aerleon/lib/gcp.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/gcp_hf.py` & `aerleon-1.2.3/aerleon/lib/gcp_hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 import copy
 import re
 import sys
 from typing import Dict, List, Set, Tuple, Union
 
 from absl import logging
 
-from aerleon.lib import gcp, nacaddr
-from aerleon.lib.policy import Policy
+from aerleon.lib import gcp, nacaddr, policy
 
 if sys.version_info < (3, 8):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 
@@ -90,15 +89,19 @@
     _TERM_ADDRESS_LIMIT = 256
 
     _TERM_TARGET_RESOURCES_LIMIT = 256
 
     _TERM_DESTINATION_PORTS_LIMIT = 256
 
     def __init__(
-        self, term, address_family='inet', policy_inet_version='inet', api_version='beta'
+        self,
+        term: policy.Term,
+        address_family: str = 'inet',
+        policy_inet_version: str = 'inet',
+        api_version: str = 'beta',
     ) -> None:
         super().__init__(term)
         self.address_family = address_family
         self.term = term
         self.skip = False
         self._ValidateTerm()
         self.api_version = api_version
@@ -159,15 +162,15 @@
         # naturally. Something has gone horribly wrong if you encounter this error.
         if self.address_family == 'mixed':
             raise gcp.TermError(
                 'Hierarchical firewall rule has incorrect inet_version for rule: %s'
                 % self.term.name
             )
 
-    def ConvertToDict(self, priority_index) -> List[OrganizationPolicy]:
+    def ConvertToDict(self, priority_index: int) -> List[OrganizationPolicy]:
         """Converts term to dict representation of SecurityPolicy.Rule JSON format.
 
         Takes all of the attributes associated with a term (match, action, etc) and
         converts them into a dictionary which most closely represents
         the SecurityPolicy.Rule JSON format.
 
         Args:
@@ -395,15 +398,15 @@
             'source_address_exclude',
             'verbatim',
         }
 
         supported_sub_tokens = {'action': {'accept', 'deny', 'next'}}
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol: Policy, exp_info: int) -> None:
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int) -> None:
         """Translates a Aerleon policy into a HF-specific data structure.
 
         Takes in a POL file, parses each term and populates the policy
         dict. Each term in this list is a dictionary formatted according to
         HF's rule API specification.  Additionally, checks for its quota.
 
         Args:
```

### Comparing `aerleon-1.2.2/aerleon/lib/ipset.py` & `aerleon-1.2.3/aerleon/lib/ipset.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/iptables.py` & `aerleon-1.2.3/aerleon/lib/iptables.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/juniper.py` & `aerleon-1.2.3/aerleon/lib/juniper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Juniper JCL generator."""
 
 
+from typing import Dict, List, Set, Tuple, Union
+
 from absl import logging
 
-from aerleon.lib import aclgenerator, nacaddr, summarizer
+from aerleon.lib import aclgenerator, nacaddr, policy, summarizer
 
 
 # generic error class
 class Error(aclgenerator.Error):
     pass
 
 
@@ -71,28 +73,28 @@
 
     Attributes:
       indent: The number of leading spaces on the current line.
       tabstop: The number of spaces to indent for a new level.
       lines: the text lines of the configuration.
     """
 
-    def __init__(self, indent=0, tabstop=4):
+    def __init__(self, indent: int = 0, tabstop: int = 4):
         self.indent = indent
         self._initial_indent = indent
         self.tabstop = tabstop
         self.lines = []
 
     def __str__(self):
         if self.indent != self._initial_indent:
             raise JuniperIndentationError(
                 'Expected indent %d but got %d' % (self._initial_indent, self.indent)
             )
         return '\n'.join(self.lines)
 
-    def Append(self, line, verbatim=False):
+    def Append(self, line: str, verbatim=False):
         """Append one line to the configuration.
 
         Args:
           line: The string to append to the config.
           verbatim: append line without adjusting indentation. Default False.
         Raises:
           JuniperIndentationError: If the indentation would be further left
@@ -178,15 +180,21 @@
             'protocol': 'ip-protocol',
             'protocol-except': 'ip-protocol-except',
             'tcp-est': 'tcp-flags "(ack|rst)"',
         },
     }
 
     def __init__(
-        self, term, term_type, enable_dsmo, noverbose, filter_direction=None, interface_type=None
+        self,
+        term: policy.Term,
+        term_type: str,
+        enable_dsmo: bool,
+        noverbose: bool,
+        filter_direction: str = None,
+        interface_type: str = None,
     ):
         super().__init__(term)
         self.term = term
         self.term_type = term_type
         self.enable_dsmo = enable_dsmo
         self.noverbose = noverbose
         # Filter direction and interface type are needed in juniperevo sub-class for IPv6 filters.
@@ -202,17 +210,14 @@
             if 'hopopt' in self.term.protocol_except:
                 loc = self.term.protocol_except.index('hopopt')
                 self.term.protocol_except[loc] = 'hop-by-hop'
 
             # some options need to modify the actions
             self.extra_actions = []
 
-    # TODO(pmoody): get rid of all of the default string concatenation here.
-    #  eg, indent(8) + 'foo;' -> '%s%s;' % (indent(8), 'foo'). pyglint likes this
-    #  more.
     def __str__(self):
         config = Config(indent=self._DEFAULT_INDENT)
         from_str = []
         # Don't render icmpv6 protocol terms under inet, or icmp under inet6
         if (self.term_type == 'inet6' and 'icmp' in self.term.protocol) or (
             self.term_type == 'inet'
             and ('icmpv6' in self.term.protocol or 'icmp6' in self.term.protocol)
@@ -697,15 +702,15 @@
             config.Append('}')  # end then{...}
 
         config.Append('}')  # end term accept-foo-to-bar { ... }
 
         return str(config)
 
     @staticmethod
-    def NextIpCheck(next_ip, term_name):
+    def NextIpCheck(next_ip: List[Union[nacaddr.IPv4, nacaddr.IPv6]], term_name: str):
         if len(next_ip) > 1:
             raise JuniperNextIpError(
                 'The following term has more ' 'than one next IP value: %s' % term_name
             )
         if next_ip[0].num_addresses > 1:
             raise JuniperNextIpError(
                 'The following term has a subnet ' 'instead of a host: %s' % term_name
@@ -718,15 +723,19 @@
         if self.term.routing_instance:
             action.add(self.term.routing_instance)
         if len(action) > 1:
             raise JuniperMultipleTerminatingActionError(
                 'The following term has multiple terminating actions: %s' % self.term.name
             )
 
-    def _MinimizePrefixes(self, include, exclude):
+    def _MinimizePrefixes(
+        self,
+        include: List[Union[nacaddr.IPv4, nacaddr.IPv6]],
+        exclude: List[Union[nacaddr.IPv4, nacaddr.IPv6]],
+    ):
         """Calculate a minimal set of prefixes for Juniper match conditions.
 
         Args:
           include: Iterable of nacaddr objects, prefixes to match.
           exclude: Iterable of nacaddr objects, prefixes to exclude.
         Returns:
           A tuple (I,E) where I and E are lists containing the minimized
@@ -752,15 +761,20 @@
             for include_prefix in include_result:
                 if exclude_prefix.subnet_of(include_prefix):
                     exclude_result.append(exclude_prefix)
                     break
 
         return include_result, exclude_result
 
-    def _Comment(self, addr, exclude=False, line_length=132):
+    def _Comment(
+        self,
+        addr: Union[nacaddr.IPv4, nacaddr.IPv6, summarizer.DSMNet],
+        exclude: bool = False,
+        line_length: int = 132,
+    ):
         """Returns address comment field if it exists.
 
         Args:
           addr: nacaddr.IPv4 object (?)
           exclude: bool - address excludes have different indentations
           line_length: integer - this is the length to which a comment will be
             truncated, no matter what.  ie, a 1000 character comment will be
@@ -844,39 +858,39 @@
 
                     rval[-1] += ' */'
         else:
             # should we be paying attention to any other addr type?
             logging.warning('Ignoring non IPv4 or IPv6 address: %s', addr)
         return rval
 
-    def _Group(self, group, lc=True):
+    def _Group(self, group: List[str], lc: bool = True):
         """If 1 item return it, else return [ item1 item2 ].
 
         Args:
           group: a list.  could be a list of strings (protocols) or a list of
                  tuples (ports)
           lc: return a lower cased result for text.  Default is True.
 
         Returns:
           rval: a string surrounded by '[' and '];' if len(group) > 1
                 or with just ';' appended if len(group) == 1
         """
 
-        def _FormattedGroup(el, lc=True):
+        def _FormattedGroup(el: List[str], lc: bool = True):
             """Return the actual formatting of an individual element.
 
             Args:
               el: either a string (protocol) or a tuple (ports)
               lc: return lower cased result for text.  Default is True.
 
             Returns:
               string: either the lower()'ed string or the ports, hyphenated
                       if they're a range, or by itself if it's not.
             """
-            if isinstance(el, str) or isinstance(el, str):
+            if isinstance(el, str):
                 if lc:
                     return el
                 else:
                     return el.lower()
             elif isinstance(el, int):
                 return str(el)
             # type is a tuple below here
@@ -904,15 +918,15 @@
 
     _PLATFORM = 'juniper'
     _DEFAULT_PROTOCOL = 'ip'
     _SUPPORTED_AF = frozenset(('inet', 'inet6', 'bridge', 'mixed'))
     _TERM = Term
     SUFFIX = '.jcl'
 
-    def _BuildTokens(self):
+    def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Build supported tokens for platform.
 
         Returns:
           tuple containing both supported tokens and sub tokens
         """
         supported_tokens, supported_sub_tokens = super()._BuildTokens()
 
@@ -965,15 +979,15 @@
                     'tcp-initial',
                     'inactive',
                 }
             }
         )
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol, exp_info):
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int):
         self.juniper_policies = []
         for header, terms in pol.filters:
             filter_options = header.FilterOptions(self._PLATFORM)
             filter_name = header.FilterName(self._PLATFORM)
 
             # Check for the position independent options and remove them from
             # the list.
```

### Comparing `aerleon-1.2.2/aerleon/lib/juniperevo.py` & `aerleon-1.2.3/aerleon/lib/juniperevo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/junipermsmpc.py` & `aerleon-1.2.3/aerleon/lib/junipermsmpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Juniper MS-MPC  generator for Aerleon."""
 
+from typing import Dict, List, Set, Tuple
+
 from absl import logging
 
-from aerleon.lib import aclgenerator, juniper, nacaddr
+from aerleon.lib import aclgenerator, juniper, nacaddr, policy
 
 MAX_IDENTIFIER_LEN = 55  # It is really 63, but leaving room for added chars
 
 
 class Term(juniper.Term):
     """Representation of an individual Juniper MS-MPC term.
 
@@ -51,29 +53,36 @@
         'pim',
         'rsvp',
         'sctp',
         'tcp',
         'udp',
     )
 
-    def __init__(self, term, term_type, noverbose, filter_name, apply_groups):
+    def __init__(
+        self,
+        term: policy.Term,
+        term_type: str,
+        noverbose: bool,
+        filter_name: str,
+        apply_groups: bool,
+    ) -> None:
         enable_dsmo = False
         super().__init__(term, term_type, enable_dsmo, noverbose)
         self.term = term
         self.term_type = term_type
         self.noverbose = noverbose
         self.apply_groups = apply_groups
         self.filter_name = filter_name
 
         for prot in self.term.protocol:
             if prot not in self._SUPPORTED_PROTOCOL_NAMES:
                 loc = self.term.protocol.index(prot)
                 self.term.protocol[loc] = str(self.PROTO_MAP.get(prot, prot))
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.enable_dsmo:
             raise NotImplementedError('enable_dsmo not implemented for msmpc')
 
         if self.apply_groups:
             indent = self._DEFAULT_INDENT
         else:
             indent = self._NO_APPLY_GROUPS_INDENT
@@ -361,19 +370,19 @@
 
     _OPTIONAL_SUPPORTED_KEYWORDS = frozenset(
         [
             'expiration',
         ]
     )
 
-    def __init__(self, pol, exp_info):
+    def __init__(self, pol: policy.Policy, exp_info: int):
         self.applications = {}
         super().__init__(pol, exp_info)
 
-    def _BuildTokens(self):
+    def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Build supported tokens for platform.
 
         Returns:
           tuple containing both supported tokens and sub tokens
         """
         supported_tokens, supported_sub_tokens = super()._BuildTokens()
 
@@ -395,15 +404,15 @@
                     'tcp-established',
                     'inactive',
                 }
             }
         )
         return supported_tokens, supported_sub_tokens
 
-    def _BuildPort(self, ports):
+    def _BuildPort(self, ports: List[Tuple[int, int]]):
         """Transform specified ports into list and ranges.
 
         Args:
           ports: a policy terms list of ports
 
         Returns:
           port_list: list of ports and port ranges
@@ -412,15 +421,15 @@
         for p in ports:
             if p[0] == p[1]:
                 port_list.append(str(p[0]))
             else:
                 port_list.append('%s-%s' % (str(p[0]), str(p[1])))
         return port_list
 
-    def _GenerateApplications(self, filter_name):
+    def _GenerateApplications(self, filter_name: str):
         target = []
         apps_set_list = []
         target.append('applications {')
         done_apps = []
         for app in sorted(self.applications[filter_name], key=lambda x: x['name']):
             app_list = []
             if app in done_apps:
@@ -498,15 +507,15 @@
         # Return the output only if there is content inside of
         # the "applications {\n}" lines, otherwise return nothing.
         if len(target) > 2:
             return target
         else:
             return []
 
-    def _TranslatePolicy(self, pol, exp_info):
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int):
         self.junipermsmpc_policies = []
         for header, terms in pol.filters:
             filter_options = header.FilterOptions(self._PLATFORM)
             filter_name = header.FilterName(self._PLATFORM)
             filter_options.remove(filter_name)
             apply_groups = 'no-apply-groups' not in filter_options
             filter_direction = None
@@ -641,28 +650,28 @@
                     new_application_set['name'] = modified_term_name
                     self.applications[filter_name].append(new_application_set)
 
             self.junipermsmpc_policies.append(
                 (header, filter_name, filter_direction, new_terms, apply_groups)
             )
 
-    def _Group(self, group, lc=True):
+    def _Group(self, group: List[str], lc: bool = True):
         """If 1 item return it, else return [ item1 item2 ].
 
         Args:
           group: a list.  could be a list of strings (protocols) or a list of tuples
             (ports)
           lc: return a lower cased result for text.  Default is True.
 
         Returns:
           rval: a string surrounded by '[' and '];' if len(group) > 1
                 or with just ';' appended if len(group) == 1
         """
 
-        def _FormattedGroup(el, lc=True):
+        def _FormattedGroup(el: List[str], lc: bool = True):
             """Return the actual formatting of an individual element.
 
             Args:
               el: either a string (protocol) or a tuple (ports)
               lc: return lower cased result for text.  Default is True.
 
             Returns:
@@ -684,15 +693,15 @@
 
         if len(group) > 1:
             rval = '[ ' + ' '.join([_FormattedGroup(x, lc=lc) for x in group]) + ' ];'
         else:
             rval = _FormattedGroup(group[0], lc=lc) + ';'
         return rval
 
-    def __str__(self):
+    def __str__(self) -> str:
         target = juniper.Config()
         for (
             header,
             filter_name,
             filter_direction,
             terms,
             apply_groups,
```

### Comparing `aerleon-1.2.2/aerleon/lib/junipersrx.py` & `aerleon-1.2.3/aerleon/lib/junipersrx.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,20 @@
 
 """SRX generator."""
 # pylint: disable=super-init-not-called
 
 
 import collections
 import copy
-import heapq
-import ipaddress
 import itertools
+from typing import Dict, List, Set, Tuple, Union
 
 from absl import logging
 
-from aerleon.lib import aclgenerator, addressbook, nacaddr
+from aerleon.lib import aclgenerator, addressbook, nacaddr, policy
 
 ICMP_TERM_LIMIT = 8
 
 
 def JunipersrxList(name, data):
     return '%s [ %s ];' % (name, ' '.join(data))
 
@@ -68,15 +67,15 @@
 
 
 class ConflictingApplicationSetsError(Error):
     pass
 
 
 class IndentList(list):
-    def __init__(self, indent, *args, **kwargs):
+    def __init__(self, indent: str, *args, **kwargs):
         self._indent = indent
         super().__init__(*args, **kwargs)
 
     def IndentAppend(self, size, data):
         self.append('%s%s' % (self._indent * size, data))
 
 
@@ -96,24 +95,31 @@
         'reject': 'reject',
         'count': 'count',
         'log': 'log',
         'expresspath': 'services-offload',
         'dscp': 'dscp',
     }
 
-    def __init__(self, term, from_zone, to_zone, expresspath=False, verbose=True):
+    def __init__(
+        self,
+        term: policy.Term,
+        from_zone: str,
+        to_zone: str,
+        expresspath: bool = False,
+        verbose: bool = True,
+    ):
         super().__init__(term)
         self.term = term
         self.from_zone = from_zone
         self.to_zone = to_zone
         self.verbose = verbose
         if expresspath:
             self.term.action = [a.replace('accept', 'expresspath') for a in self.term.action]
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Render config output from this term object."""
         ret_str = IndentList(JuniperSRX.INDENT)
 
         # COMMENTS
         comment_max_width = 68
         if self.term.owner and self.verbose:
             self.term.comment.append('Owner: %s' % self.term.owner)
@@ -227,27 +233,27 @@
 
             ret_str.IndentAppend(4, '}')
 
             ret_str.IndentAppend(3, '}')
 
         return '\n'.join(ret_str)
 
-    def _Group(self, group):
+    def _Group(self, group: List[str]):
         """If 1 item return it, else return [ item1 item2 ].
 
         Args:
           group: a list.  could be a list of strings (protocols) or a list of
                  tuples (ports)
 
         Returns:
           rval: a string surrounded by '[' and '];' if len(group) > 1
                 or with just ';' appended if len(group) == 1
         """
 
-        def _FormattedGroup(el):
+        def _FormattedGroup(el: List[str]):
             """Return the actual formatting of an individual element.
 
             Args:
               el: either a string (protocol) or a tuple (ports)
 
             Returns:
               string: either the lower()'ed string or the ports, hyphenated
@@ -296,25 +302,25 @@
     _MAX_HEADER_COMMENT_LENGTH = 71
     # The SRX platform is limited in how many IP addresses can be used in
     # a single policy.
     _ADDRESS_LENGTH_LIMIT = 1023
     # IPv6 are 32 bytes compared to IPv4, this is used as a multiplier.
     _IPV6_SIZE = 4
 
-    def __init__(self, pol, exp_info):
+    def __init__(self, pol: policy.Policy, exp_info: int):
         self.srx_policies = []
         self.addressbook = addressbook.Addressbook()
         self.applications = []
         self.ports = []
         self.from_zone = ''
         self.to_zone = ''
         self.addr_book_type = set()
         super().__init__(pol, exp_info)
 
-    def _BuildTokens(self):
+    def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Build supported tokens for platform.
 
         Returns:
           tuple containing both supported tokens and sub tokens
         """
         supported_tokens, supported_sub_tokens = super()._BuildTokens()
 
@@ -336,15 +342,15 @@
             {
                 'action': {'accept', 'deny', 'reject', 'count', 'log', 'dscp'},
             }
         )
         del supported_sub_tokens['option']
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol, exp_info):
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int):
         # pylint: disable=attribute-defined-outside-init
         """Transform a policy object into a JuniperSRX object.
 
         Args:
           pol: policy.Policy object
           exp_info: print a info message when a term is set to expire
                     in that many weeks
@@ -609,27 +615,27 @@
 
                 if new_application_set:
                     new_application_set['name'] = term.name
                     self.applications.append(new_application_set)
 
             self.srx_policies.append((header, new_terms, filter_options))
 
-    def _FixLargePolices(self, terms, address_family):
+    def _FixLargePolices(self, terms: List[policy.Term], address_family: str):
         """Loops over all terms finding terms exceeding SRXs policy limit.
 
         Args:
           terms: List of terms from a policy.
           address_family: Tuple containing address family versions.
 
         See the following URL for more information
         http://www.juniper.net/techpubs/en_US/junos12.1x44/topics/reference/
         general/address-address-sets-limitations.html
         """
 
-        def Chunks(addresses):
+        def Chunks(addresses: List[Union[nacaddr.IPv4, nacaddr.IPv6]]):
             """Splits a list of IP addresses into smaller lists based on byte size."""
             return_list = [[]]
             counter = 0
             index = 0
             for i in addresses:
                 # Size is split in half due to the max size being a sum of src and dst.
                 if counter > (self._ADDRESS_LENGTH_LIMIT / 2):
@@ -671,15 +677,15 @@
                     counter += 1
             else:
                 expanded_terms.append(term)
         if expanded_terms:
             del terms[:]
             terms.extend(expanded_terms)
 
-    def _BuildPort(self, ports):
+    def _BuildPort(self, ports: List[Tuple[int, int]]):
         """Transform specified ports into list and ranges.
 
         Args:
           ports: a policy terms list of ports
 
         Returns:
           port_list: list of ports and port ranges
@@ -688,15 +694,15 @@
         for i in ports:
             if i[0] == i[1]:
                 port_list.append(str(i[0]))
             else:
                 port_list.append('%s-%s' % (str(i[0]), str(i[1])))
         return port_list
 
-    def _GenerateAddressBook(self):
+    def _GenerateAddressBook(self) -> IndentList:
         """Creates address book."""
         target = IndentList(self.INDENT)
 
         # create address books if address-book-type set to global
         if self._GLOBAL_ADDR_BOOK in self.addr_book_type:
             global_address_book = collections.defaultdict(list)
 
@@ -759,15 +765,15 @@
                     target.IndentAppend(4, '}')
                 target.IndentAppend(3, '}')
                 target.IndentAppend(2, '}')
             target.IndentAppend(1, '}')
 
         return target
 
-    def _GenerateApplications(self):
+    def _GenerateApplications(self) -> IndentList:
         target = IndentList(self.INDENT)
         apps_set_list = IndentList(self.INDENT)
         target.append('replace: applications {')
         done_apps = []
         for app in sorted(self.applications, key=lambda x: x['name']):
             app_list = IndentList(self.INDENT)
             if app in done_apps:
@@ -866,15 +872,15 @@
             target.append('delete: applications;')
             return target
 
         target.extend(apps_set_list)
         target.append('}\n')
         return target
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Render the output of the JuniperSRX policy into config."""
         target = IndentList(self.INDENT)
         target.append('security {')
 
         # ADDRESSBOOK
         target.extend(self._GenerateAddressBook())
```

### Comparing `aerleon-1.2.2/aerleon/lib/k8s.py` & `aerleon-1.2.3/aerleon/lib/k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 https://kubernetes.io/docs/concepts/services-networking/network-policies/
 https://kubernetes.io/docs/tasks/administer-cluster/declare-network-policy/
 """
 
 import copy
 import re
 import sys
-from typing import Dict, List, Set, Tuple, Union
+from typing import Dict, Set, Tuple
 
 import yaml
 from absl import logging
 
 from aerleon.lib import aclgenerator
 from aerleon.lib.policy import Policy, Term
```

### Comparing `aerleon-1.2.2/aerleon/lib/nacaddr.py` & `aerleon-1.2.3/aerleon/lib/nacaddr.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,27 +94,27 @@
                 ip_string.network_address._ip,
                 ip_string.prefixlen,
             )  # pylint disable=protected-access # pytype: disable=attribute-error
         else:
             ip = ip_string
         super().__init__(ip, strict)
 
-    def subnet_of(self, other: "IPv4") -> bool:
+    def subnet_of(self, other: IPv4) -> bool:
         """Return True if this network is a subnet of other."""
         if self.version != other.version:
             return False
         return self._is_subnet_of(self, other)
 
     def supernet_of(self, other: Union[IPv4, IPv6]) -> bool:
         """Return True if this network is a supernet of other."""
         if self.version != other.version:
             return False
         return self._is_subnet_of(other, self)
 
-    def __deepcopy__(self, memo):
+    def __deepcopy__(self, memo: dict):
         result = self.__class__(self)
         result.text = self.text
         result.token = self.token
         result.parent_token = self.parent_token
         return result
 
     def AddComment(self, comment: str = '') -> None:
@@ -158,15 +158,14 @@
             comment=self.text,
             token=self.token,
         )
         return ret_addr
 
     # Backwards compatibility name from v1.
     Supernet = supernet
-    _is_subnet_of = _is_subnet_of
 
 
 class IPv6(ipaddress.IPv6Network):
     """This subclass allows us to keep text comments related to each object."""
 
     def __init__(
         self,
@@ -186,27 +185,27 @@
                 ip_string.network_address._ip,
                 ip_string.prefixlen,
             )  # pylint disable=protected-access # pytype: disable=attribute-error
         else:
             ip = ip_string
         super().__init__(ip, strict)
 
-    def subnet_of(self, other: "IPv6") -> bool:
+    def subnet_of(self, other: IPv6) -> bool:
         """Return True if this network is a subnet of other."""
         if self.version != other.version:
             return False
         return self._is_subnet_of(self, other)
 
-    def supernet_of(self, other: "IPv6") -> bool:
+    def supernet_of(self, other: IPv6) -> bool:
         """Return True if this network is a supernet of other."""
         if self.version != other.version:
             return False
         return self._is_subnet_of(other, self)
 
-    def __deepcopy__(self, memo):
+    def __deepcopy__(self, memo: dict):
         result = self.__class__(self)
         result.text = self.text
         result.token = self.token
         result.parent_token = self.parent_token
         return result
 
     def supernet(self, prefixlen_diff: int = 1) -> "IPv6":
@@ -235,15 +234,14 @@
             comment=self.text,
             token=self.token,
         )
         return ret_addr
 
     # Backwards compatibility name from v1.
     Supernet = supernet
-    _is_subnet_of = _is_subnet_of
 
     def AddComment(self, comment: str = '') -> None:
         """Append comment to self.text, comma separated.
 
         Don't add the comment if it's the same as self.text.
 
         Args:
@@ -273,15 +271,15 @@
     """Returns True if subnets are fully consumed by supernets."""
     for net in subnets:
         if not _InNetList(supernets, net):
             return False
     return True
 
 
-def CollapseAddrListPreserveTokens(addresses: List[IPv4]) -> List[IPv4]:
+def CollapseAddrListPreserveTokens(addresses: List[Union[IPv4, IPv6]]) -> List[Union[IPv4, IPv6]]:
     """Collapse an array of IPs only when their tokens are the same.
 
     Args:
        addresses: list of ipaddress.IPNetwork objects.
 
     Returns:
       list of ipaddress.IPNetwork objects.
@@ -443,22 +441,22 @@
         if ca.network_address in address_set:
             complements_dict[ca.network_address].append(ca)
     return _CollapseAddrListInternal(
         sorted(addresses, key=ipaddress.get_mixed_type_key), complements_dict
     )
 
 
-def SortAddrList(addresses: List[Union[Any, IPv6, IPv4]]) -> List[Union[Any, IPv6, IPv4]]:
+def SortAddrList(addresses: List[Union[IPv6, IPv4]]) -> List[Union[IPv6, IPv4]]:
     """Return a sorted list of nacaddr objects."""
     return sorted(addresses, key=ipaddress.get_mixed_type_key)
 
 
 def RemoveAddressFromList(
     superset: List[Union[IPv4, IPv6]], exclude: Union[IPv4, IPv6]
-) -> List[Union[Any, IPv6, IPv4]]:
+) -> List[Union[IPv6, IPv4]]:
     """Remove a single address from a list of addresses.
 
     Args:
       superset: a List of nacaddr IPv4 or IPv6 addresses
       exclude: a single nacaddr IPv4 or IPv6 address
 
     Returns:
```

### Comparing `aerleon-1.2.2/aerleon/lib/naming.py` & `aerleon-1.2.3/aerleon/lib/naming.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,26 +121,28 @@
         filename: The name of the file in which this error or message originated.
         line: The line where this error or message originated.
         include_chain: If the error or message originated while processing an included
             file, include_chain will list the include file chain as a list of file/line tuples.
             The top-level file should be the first item in the list.
     """
 
-    message: str
-    filename: str
-    line: int
-    include_chain: "list[Tuple[str, int]]"
-
-    def __init__(self, message, *, filename, line=None, include_chain=None):
+    def __init__(
+        self,
+        message: str,
+        *,
+        filename: str,
+        line: int = None,
+        include_chain: List[Tuple[str, int]] = None,
+    ):
         self.message = message
         self.filename = filename
         self.line = line
         self.include_chain = include_chain
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Display user-facing error message with include chain (if present).
 
         e.g.
         Excessive recursion: include depth limit of 5 reached. File=include_1.pol-include.yaml, Line=3.
         Include stack:
         > File='policy_with_include.pol.yaml', Line=11 (Top Level)
         > File='include_1.pol-include.yaml', Line=3
@@ -157,19 +159,19 @@
             error_context += "\nInclude stack:"
             for i, (File, Line) in enumerate(self.include_chain):
                 error_context += f"\n> File='{File}', Line={Line}"
                 if i == 0:
                     error_context += " (Top Level)"
         return error_context
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"UserMessage(\"{str(self)}\")"
 
 
-def is_yaml_suffix(suffix):
+def is_yaml_suffix(suffix: str) -> bool:
     return suffix == '.yaml' or suffix == '.yml'
 
 
 class _ItemUnit:
     """This class is a container for an index key and a list of associated values.
 
     An ItemUnit will contain the name of either a service or network group,
@@ -407,15 +409,15 @@
         try:
             item = item.strip()
             nacaddr.IP(item, strict=False)
             return True
         except ValueError:
             return False
 
-    def GetServiceNames(self):
+    def GetServiceNames(self) -> List[str]:
         """Returns the list of all known service names."""
         return list(self.services.keys())
 
     def GetService(self, query: str) -> List[str]:
         """Given a service name, return a list of associated ports and protocols.
 
         Args:
@@ -451,15 +453,15 @@
                     except UndefinedServiceError as e:
                         # One of the services in query is undefined, refine the error msg.
                         raise UndefinedServiceError('%s (in %s)' % (e, query))
             else:
                 expandset.add(service)
         return sorted(expandset)
 
-    def GetPortParents(self, query, proto):
+    def GetPortParents(self, query: str, proto: str) -> List[str]:
         """Returns a list of all service tokens containing the port/protocol pair.
 
         Args:
             query: port number ('22') as str
             proto: protocol name ('tcp') as str
 
         Returns:
@@ -595,28 +597,27 @@
                     # if net was something like 'FOO', or the name of another token which
                     # needs to be dereferenced, nacaddr.IP() will return a ValueError
                     returnlist.extend(self.GetNet(net))
         for i in returnlist:
             i.parent_token = token
         return returnlist
 
-    def _Parse(self, definitions_directory):
+    def _Parse(self, definitions_directory: str) -> None:
         """Parse files for tokens and values.
 
         Given a directory name, grab all the appropriate files in that
         directory and parse them for definitions.
 
         Args:
           defdirectory: Path to directory containing definition files.
           def_type: Type of definitions to parse
 
         Raises:
           NoDefinitionsError: if no definitions are found.
         """
-
         file_def_type = {
             '.net': DEF_TYPE_NETWORKS,
             '.svc': DEF_TYPE_SERVICES,
             '.yaml': 'yaml',
             '.yml': 'yaml',
         }
```

### Comparing `aerleon-1.2.2/aerleon/lib/nftables.py` & `aerleon-1.2.3/aerleon/lib/nftables.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """NFtables policy generator for Aerleon."""
 
 import collections
 import copy
+from typing import DefaultDict, Dict, List, Set, Tuple, Union
 
 from absl import logging
 
-from aerleon.lib import aclgenerator, nacaddr
+from aerleon.lib import aclgenerator, nacaddr, policy
 
 # NFTables and Aerleon have conflicting definitions of 'address family'
 # In Aerleon:
 # 'mixed' refers to a 'mixed address policy IPv4/IPv6'
 # 'inet6' refers to IPv6 only.
 # 'inet' refers to IPv4 only.
 # In nftables:
@@ -34,29 +35,29 @@
 # Therefore; we use static global variables in this generator to refer to the
 # real intent, values are the NFtable AF format.
 ip4 = 'ip'
 ip6 = 'ip6'
 mixed = 'inet'
 
 
-def TabSpacer(number_spaces, string):
+def TabSpacer(number_spaces: int, string: str) -> str:
     """Configuration indentation utility function."""
     blank_space = ' '
     return (blank_space * number_spaces) + string
 
 
-def Add(statement):
+def Add(statement: str) -> str:
     """Prefix space appending utility to handle text joins."""
     if statement:
         return TabSpacer(1, statement)
     else:
         return statement
 
 
-def ChainFormat(kind, name, ruleset):
+def ChainFormat(kind: str, name: str, ruleset: List[str]) -> str:
     """Builds a chain in NFtables configuration format.
 
     Args:
       kind: type string (chain or counter)
       name: name to give the chain.
       ruleset: the list returned from RulesetGenerator function.
 
@@ -102,40 +103,41 @@
     """
 
     _ALLOWED_PROTO_NAME = frozenset(
         ['tcp', 'udp', 'icmp', 'esp', 'udp', 'ah', 'comp', 'udplite', 'dccp', 'sctp', 'icmpv6']
     )
     _ACTIONS = {'accept': 'accept', 'deny': 'drop'}
 
-    def __init__(self, term, nf_af, nf_hook, verbose=True):
+    def __init__(self, term: policy.Term, nf_af: str, nf_hook: str, verbose: bool = True):
         """Individual instances of a Term for NFtables.
 
         Args:
           term: Term data.
           nf_af: nftables table type IPv4 only (ip), IPv6 (ip6) or dual-stack
             (inet).
           nf_hook: INPUT or OUTPUT (packet processing/direction of traffic).
           verbose: used for comment handling.
         """
         self.term = term
         self.address_family = nf_af
         self.hook = nf_hook
         self.verbose = verbose
 
-    def MapICMPtypes(self, af, term_icmp_types):
+    def MapICMPtypes(self, af: SyntaxWarning, term_icmp_types: List[str]) -> List[str]:
         """Normalize certain ICMP_TYPES for NFTables rendering.
 
         If we encounter certain keyword values in policy.Term.ICMP_TYPE keywords,
         we override them with NFTable specific values in order for rendered
         policy to be semantically correct with what NFT expects.
         https://www.netfilter.org/projects/nftables/manpage.html
 
         Function is used inside PortsAndProtocols.
 
         Args:
+          af:
           term_icmp_types: ICMP types keywords.
 
         Returns:
           normalized list of icmp_types.
         """
         ICMP_TYPE_REMAP = {
             6: {
@@ -170,15 +172,15 @@
             if af == ip6:
                 # IPv6 ICMP
                 if item in ICMP_TYPE_REMAP[6]:
                     # Replace with NFT expected value.
                     term_icmp_types[term_icmp_types.index(item)] = ICMP_TYPE_REMAP[6].get(item)
         return term_icmp_types
 
-    def CreateAnonymousSet(self, data):
+    def CreateAnonymousSet(self, data: List[str]) -> str:
         """Build a nftables anonymous set from some elements.
 
         Anonymous are formatted using curly braces then some data. These sets are
         bound to a rule, have no specific name and cannot be updated.
 
         Args:
           data: a list of strings to format.
@@ -209,15 +211,15 @@
           icmp_type: special ICMP type flag.
 
         Returns:
           list of statements related to ports and protocols.
 
         """
 
-        def PortStatement(protocol, source, destination):
+        def PortStatement(protocol: List[str], source: str, destination: str) -> List[str]:
             """NFT port statement. Returns empty if no ports defined."""
             ports_list = []
 
             # SOURCE PORTS.
             if source:
                 ports_list.append('%s sport %s' % (protocol, self.CreateAnonymousSet(source)))
 
@@ -302,15 +304,15 @@
                             statement_lines.append(PortStatement(proto, src_p, dst_p))
                         else:
                             # Single proto, no ports.
                             statement_lines.append('meta l4proto' + Add(proto))
 
         return statement_lines
 
-    def _OptionsHandler(self, term):
+    def _OptionsHandler(self, term: policy.Term) -> str:
         """Term 'option' handler.
 
         Function used to evaluate term.logging and also term.option values. Then
         it builds any statement that would be appended before a veredict.
         Results of this function are then used in GroupExpressions() to combine
         a final valid NFTables chain.
 
@@ -346,15 +348,17 @@
 
         # Build the final statement to be returned.
         if options:
             return ' '.join(options)
         else:
             return ''
 
-    def GroupExpressions(self, address_expr, pp_expr, options, verdict):
+    def GroupExpressions(
+        self, address_expr: List[str], pp_expr: List[str], options: str, verdict: str
+    ) -> List[str]:
         """Combines all expressions with a verdict (decision).
 
         The inputs are already pre-sanitized by RulesetGenerator. NFTables processes
         rules from left-to-right - ending in a verdict. We form our ruleset then
         towards the end append any term.options from _OptionsHandler.
 
         Args:
@@ -386,15 +390,20 @@
             for pstat in pp_expr:
                 statement.append(pstat + Add(options) + Add(verdict))
         else:
             # If no addresses or ports & protocol. Verdict only statement.
             statement.append((Add(options) + verdict))
         return statement
 
-    def _AddrStatement(self, address_family, src_addr, dst_addr):
+    def _AddrStatement(
+        self,
+        address_family: str,
+        src_addr: List[Union[nacaddr.IPv4, nacaddr.IPv6]],
+        dst_addr: List[Union[nacaddr.IPv4, nacaddr.IPv6]],
+    ) -> List[str]:
         """Builds an NFTables address statement.
 
         Args:
           address_family: NFTables address family.
           src_addr: prefiltered list of src addresses.
           dst_addr: prefiltered list of dst addresses.
 
@@ -446,15 +455,15 @@
             if address_family == 'inet' or address_family == 'ip6':
                 if dst_addr_book['ip6']:
                     address_statement.append(
                         'ip6 daddr ' + self.CreateAnonymousSet(dst_addr_book['ip6'])
                     )
         return address_statement
 
-    def RulesetGenerator(self, term):
+    def RulesetGenerator(self, term: policy.Term) -> List[str]:
         """Generate string rules of a given Term.
 
         Rules are constructed from Terms() and are contained within chains.
         This function generates rules that will be present inside a regular
         (non-base) chain. Each item in list represents a line break for later
         parsing.
 
@@ -492,15 +501,17 @@
         # STATEMENT VERDICT / ACTION.
         verdict = self._ACTIONS[self.term.action[0]]
         # TODO: If verdict is not supported, drop nftable_rule for it.
         nftable_rule = self.GroupExpressions(address_list, proto_and_ports, opt, verdict)
         term_ruleset.extend(nftable_rule)
         return term_ruleset
 
-    def _AddressClassifier(self, address_to_classify):
+    def _AddressClassifier(
+        self, address_to_classify: List[Union[nacaddr.IPv4, nacaddr.IPv6]]
+    ) -> DefaultDict[str, List[Union[nacaddr.IPv4, nacaddr.IPv6]]]:
         """Organizes network addresses according to IP family in a dict.
 
         Args:
           address_to_classify: nacaddr.IP list of network addresses.
 
         Returns:
           dictionary of network addresses classified by AF.
@@ -509,15 +520,15 @@
         for addr in address_to_classify:
             if addr.version == 4:
                 addresses['ip'].append(str(addr))
             if addr.version == 6:
                 addresses['ip6'].append(str(addr))
         return addresses
 
-    def _Group(self, group):
+    def _Group(self, group: List[Tuple[int, int]]) -> str:
         """If 1 item return it, else return [ item1 item2 ].
 
         Args:
           group: a list.  could be a list of strings (protocols) or a list of tuples
             (ports)
 
         Returns:
@@ -538,15 +549,15 @@
         elif len(group) == 1:
             rval = _FormatPorts(group[0])
         else:
             # Ports undefined/empty.
             rval = ''
         return rval
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Terms printing function.
 
         Each term is expressed as its own chain. Later referenced to a parent chain
         with filter directionality (input/output).
         """
         return ChainFormat('chain', self.term.name, self.RulesetGenerator(self.term))
 
@@ -569,15 +580,15 @@
     )
 
     _AF_MAP = {'inet': (4,), 'inet6': (6,), 'mixed': (4, 6)}
     # Below mapping converts Aerleon HEADER native to nftables table.
     # In Nftables 'inet' contains both IPv4 and IPv6 addresses and rules.
     NF_TABLE_AF_MAP = {'inet': 'ip', 'inet6': 'ip6', 'mixed': 'inet'}
 
-    def _BuildTokens(self):
+    def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """NFTables generator list of supported tokens and sub tokens.
 
         Returns:
           tuple containing both supported tokens and sub tokens
         """
         supported_tokens, supported_sub_tokens = super()._BuildTokens()
         # Set of supported keywords for a given platform.  Values should be in
@@ -614,15 +625,15 @@
                 'accept',
                 'deny',
             },
             'icmp_type': set(list(Term.ICMP_TYPE[4].keys()) + list(Term.ICMP_TYPE[6].keys())),
         }
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol, exp_info):
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int):
         """Translates a Aerleon policy file into NFtables specific data structure.
 
         Reads a POL file, filters for NFTables specific data, parses each term
         and populates the nftables_policies list.
 
         Args:
           pol: A Policy() object representing a given POL file.
@@ -698,15 +709,15 @@
                     nf_priority,
                     filter_policy_default_action,
                     verbose,
                     child_chains,
                 )
             )
 
-    def _ProcessHeader(self, header_options):
+    def _ProcessHeader(self, header_options: List[str]) -> Tuple[str, str, int, str, bool]:
         """Aerleon policy header processing.
 
         Args:
           header_options: Aerleon policy header data (filter_options)
 
         Raises:
           HeaderError: Raised when the policy header format requirements are not
@@ -752,15 +763,17 @@
                 raise HeaderError('Too many integers in header.')
         verbose = True
         if 'noverbose' in header_options:
             verbose = False
             header_options.remove('noverbose')
         return netfilter_family, netfilter_hook, netfilter_priority, policy_default_action, verbose
 
-    def _ConfigurationDictionary(self, nft_pol):
+    def _ConfigurationDictionary(
+        self, nft_pol: List[Union[policy.Header, str, int, bool, DefaultDict]]
+    ) -> DefaultDict[str, Union[str, DefaultDict]]:
         """NFTables configuration object.
 
         Organizes policies into a data structure that can keep relationships with
         NFTables address family (tables) and the parent base chain (+ child chains).
 
         Args:
           nft_pol: Object containing pre-processed data from _TranslatePolicy.
@@ -788,15 +801,15 @@
                 'comment': base_chain_comment,
                 'priority': nf_priority,
                 'policy': filter_policy_default_action,
                 'rules': child_chains,
             }
         return nftables
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Render the policy as Nftables configuration."""
         nft_config = []
         configuration = self._ConfigurationDictionary(self.nftables_policies)
 
         for address_family in configuration:
             nft_config.append('table %s filtering_policies {' % address_family)
             base_chain_dict = configuration[address_family]
```

### Comparing `aerleon-1.2.2/aerleon/lib/nsxv.py` & `aerleon-1.2.3/aerleon/lib/nsxv.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 # limitations under the License.
 #
 
 """Nsxv generator."""
 
 import re
 import xml
+from typing import Dict, List, Set, Tuple
 
 from absl import logging
 
-from aerleon.lib import aclgenerator, nacaddr
+from aerleon.lib import aclgenerator, nacaddr, policy
 
 _ACTION_TABLE = {
     'accept': 'allow',
     'deny': 'deny',
     'reject': 'reject',
     'reject-with-tcp-rst': 'reject',  # tcp rst not supported
 }
@@ -105,23 +106,23 @@
 
     pass
 
 
 class Term(aclgenerator.Term):
     """Creates a  single ACL Term for Nsxv."""
 
-    def __init__(self, term, filter_type, applied_to=None, af=4):
+    def __init__(self, term: policy.Term, filter_type: str, applied_to: str = None, af: int = 4):
         self.term = term
         # Our caller should have already verified the address family.
         assert af in (4, 6)
         self.af = af
         self.filter_type = filter_type
         self.applied_to = applied_to
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Convert term to a rule string.
 
         Returns:
           A rule as a string.
 
         Raises:
           NsxvAclTermError: When unknown icmp-types are specified
@@ -387,15 +388,17 @@
         )
 
         # remove any trailing spaces and replace multiple spaces with singles
         stripped_ret_lines = [re.sub(r'\s+', ' ', x).rstrip() for x in ret_lines]
         ret_str.extend(stripped_ret_lines)
         return ''.join(ret_str)
 
-    def _ServiceToString(self, proto, sports, dports, icmp_types):
+    def _ServiceToString(
+        self, proto: int, sports: Tuple[int, int], dports: Tuple[int, int], icmp_types: List[str]
+    ):
         """Converts service to string.
 
         Args:
           proto: str, protocl
           sports: str list or none, the source port
           dports: str list or none, the destination port
           icmp_types: icmp-type numeric specification (if any)
@@ -491,30 +494,30 @@
         [
             'expiration',
             'logging',
         ]
     )
     _FILTER_OPTIONS_DICT = {}
 
-    def _BuildTokens(self):
+    def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Build supported tokens for platform.
 
         Returns:
           tuple containing both supported tokens and sub tokens
         """
         supported_tokens, supported_sub_tokens = super()._BuildTokens()
 
         supported_tokens |= {'logging'}
         supported_sub_tokens.update(
             {'action': {'accept', 'deny', 'reject', 'reject-with-tcp-rst'}}
         )
         del supported_sub_tokens['option']
         return supported_tokens, supported_sub_tokens
 
-    def _TranslatePolicy(self, pol, exp_info):
+    def _TranslatePolicy(self, pol: policy.Policy, exp_info: int):
         self.nsxv_policies = []
         for header, terms in pol.filters:
             filter_options = header.FilterOptions(self._PLATFORM)
             if len(filter_options) >= 2:
                 filter_name = filter_options[1]
 
             # get filter type, section id and applied To
@@ -568,15 +571,15 @@
                         inet6_term = self.FixHighPorts(term, 'inet6')
                         if not inet6_term:
                             continue
                         new_terms.append(Term(inet6_term, filter_type, applied_to, 6))
 
             self.nsxv_policies.append((header, filter_name, [filter_type], new_terms))
 
-    def _ParseFilterOptions(self, filter_options):
+    def _ParseFilterOptions(self, filter_options: List[str]):
         """Parses the target in header for filter type, section_id and applied_to.
 
         Args:
           filter_options: list of remaining target options
 
         Returns:
           A dictionary that contains fields necessary to create the firewall
@@ -627,15 +630,15 @@
                         )
 
         self._FILTER_OPTIONS_DICT['section_name'] = section_name
         self._FILTER_OPTIONS_DICT['filter_type'] = filter_type
         self._FILTER_OPTIONS_DICT['section_id'] = section_id
         self._FILTER_OPTIONS_DICT['applied_to'] = applied_to
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Render the output of the Nsxv policy."""
 
         target_header = []
         target = []
 
         # add the p4 tags
         target.append('<!--')
```

### Comparing `aerleon-1.2.2/aerleon/lib/openconfig.py` & `aerleon-1.2.3/aerleon/lib/openconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 """Openconfig yang ACL generator.
 
 More information about the Openconfig ACL model schema:
 http://ops.openconfig.net/branches/models/master/openconfig-acl.html
 """
 
 import copy
-import ipaddress
 import json
-import re
 import sys
 from collections import defaultdict
 from typing import Any, DefaultDict, Dict, List, Set, Tuple, Union
 
 from absl import logging
 
 from aerleon.lib import aclgenerator
@@ -90,15 +88,15 @@
         self.term = term
         self.inet_version = inet_version
 
         # Combine (flatten) addresses with their exclusions into a resulting
         # flattened_saddr, flattened_daddr, flattened_addr.
         self.term.FlattenAll()
 
-    def __str__(self):
+    def __str__(self) -> None:
         """Convert term to a string."""
         rules = self.ConvertToDict()
         json.dumps(rules, indent=2)
 
     def ConvertToDict(
         self,
     ) -> List[ACLEntry]:
```

### Comparing `aerleon-1.2.2/aerleon/lib/packetfilter.py` & `aerleon-1.2.3/aerleon/lib/packetfilter.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/paloaltofw.py` & `aerleon-1.2.3/aerleon/lib/paloaltofw.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/pcap.py` & `aerleon-1.2.3/aerleon/lib/pcap.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/plugin.py` & `aerleon-1.2.3/aerleon/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/plugin_supervisor.py` & `aerleon-1.2.3/aerleon/lib/plugin_supervisor.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/policy.py` & `aerleon-1.2.3/aerleon/lib/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from __future__ import annotations
 
 import datetime
 import os
 import pathlib
 import sys
 from typing import TYPE_CHECKING, Any, List, Optional, Tuple, Union
-from unittest.mock import MagicMock
 
 from absl import logging
 from ply import lex, yacc
 from ply.lex import LexToken
 from ply.yacc import YaccProduction
 
 from aerleon.lib import nacaddr, naming
@@ -1764,21 +1763,21 @@
     def __init__(self, target: List[str]) -> None:
         self.platform = target[0]
         self.options = target[1:]
 
     def __str__(self) -> str:
         return self.platform
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.__str__()
 
     def __eq__(self, other: Target) -> bool:
         return self.platform == other.platform and self.options == other.options
 
-    def __ne__(self, other):
+    def __ne__(self, other) -> bool:
         return not self.__eq__(other)
 
 
 # Lexing/Parsing starts here
 tokens = (
     'ACTION',
     'ADDR',
```

### Comparing `aerleon-1.2.2/aerleon/lib/policy_builder.py` & `aerleon-1.2.3/aerleon/lib/policy_builder.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/policy_simple.py` & `aerleon-1.2.3/aerleon/lib/policy_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,20 +41,20 @@
         for k, v in field_map.items():
             if t == v:
                 f = k
                 break
         indent = len(f) + 5
         return '%s::%s' % (f, self.ValueStr().replace('\n', '\n' + ' ' * indent))
 
-    def __eq__(self, o: "Target") -> bool:
+    def __eq__(self, o: Target) -> bool:
         if not isinstance(o, self.__class__):
             return False
         return self.value == o.value
 
-    def __ne__(self, o: "Target") -> bool:
+    def __ne__(self, o: Target) -> bool:
         return not self == o
 
     def Append(self, value: str) -> None:
         self.value += value
 
     def ValueStr(self) -> str:
         return self.value
```

### Comparing `aerleon-1.2.2/aerleon/lib/policyreader.py` & `aerleon-1.2.3/aerleon/lib/policyreader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/port.py` & `aerleon-1.2.3/aerleon/lib/port.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 class PPP:
     """PPP: [P]ort [P]rotocol [P]airs.
 
     Make port/protocol pairs an object for easy comparisons
     """
 
-    def __init__(self, service):
+    def __init__(self, service) -> None:
         """Init for PPP object.
 
         Args:
           service: A port/protocol pair as str (eg: '80/tcp', '22-23/tcp') or
                    a nested service name (eg: 'SSH')
         """
         # remove comments (if any)
```

### Comparing `aerleon-1.2.2/aerleon/lib/recognizers.py` & `aerleon-1.2.3/aerleon/lib/recognizers.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/speedway.py` & `aerleon-1.2.3/aerleon/lib/speedway.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/srxlo.py` & `aerleon-1.2.3/aerleon/lib/srxlo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/summarizer.py` & `aerleon-1.2.3/aerleon/lib/summarizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,58 +39,58 @@
           netmask: subnet mask as int.
           text: text comment.
         """
         self.address = address
         self.netmask = netmask
         self.text = text
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(str(self.address) + str(self.netmask))
 
     def __eq__(self, other: DSMNet) -> bool:
         try:
             return self.address == other.address and self.netmask == other.netmask
         except AttributeError:
             return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: DSMNet) -> bool:
         eq = self.__eq__(other)
         if eq is NotImplemented:
             return NotImplemented
         return not eq
 
-    def __le__(self, other):
+    def __le__(self, other: DSMNet) -> bool:
         gt = self.__gt__(other)
         if gt is NotImplemented:
             return NotImplemented
         return not gt
 
-    def __ge__(self, other):
+    def __ge__(self, other: DSMNet) -> bool:
         lt = self.__lt__(other)
         if lt is NotImplemented:
             return NotImplemented
         return not lt
 
     def __lt__(self, other: DSMNet) -> bool:
         try:
             if self.address != other.address:
                 return self.address < other.address
         except AttributeError:
             return NotImplemented
         return False
 
-    def __gt__(self, other):
+    def __gt__(self, other: DSMNet) -> bool:
         try:
             if self.address != other.address:
                 return self.address > other.address
         except AttributeError:
             return NotImplemented
         return False
 
-    def __str__(self):
+    def __str__(self) -> str:
         return ' '.join([self.address, self.netmask])
 
     def MergeText(self, text: str = '') -> str:
         """Returns self.text joined with optional text.
 
         Don't join the text if it's already contained in self.text.
```

### Comparing `aerleon-1.2.2/aerleon/lib/windows.py` & `aerleon-1.2.3/aerleon/lib/windows.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/windows_advfirewall.py` & `aerleon-1.2.3/aerleon/lib/windows_advfirewall.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/windows_ipsec.py` & `aerleon-1.2.3/aerleon/lib/windows_ipsec.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/yaml.py` & `aerleon-1.2.3/aerleon/lib/yaml.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/lib/yaml_loader.py` & `aerleon-1.2.3/aerleon/lib/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/utils/config.py` & `aerleon-1.2.3/aerleon/utils/config.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/aerleon/utils/iputils.py` & `aerleon-1.2.3/aerleon/utils/iputils.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/pyproject.toml` & `aerleon-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aerleon"
-version = "1.2.2"
+version = "1.2.3"
 description = "A firewall generation tool"
 authors = ["Rob Ankeny <ankenyr@gmail.com>", "Jason Benterou <jason.benterou@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/aerleon/aerleon"
 repository = "https://github.com/aerleon/aerleon"
 keywords = ["firewall", "networking", "security"]
```

### Comparing `aerleon-1.2.2/tools/cgrep.py` & `aerleon-1.2.3/tools/cgrep.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/tools/iputilstools.py` & `aerleon-1.2.3/tools/iputilstools.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.2/PKG-INFO` & `aerleon-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerleon
-Version: 1.2.2
+Version: 1.2.3
 Summary: A firewall generation tool
 Home-page: https://github.com/aerleon/aerleon
 License: Apache-2.0
 Keywords: firewall,networking,security
 Author: Rob Ankeny
 Author-email: ankenyr@gmail.com
 Requires-Python: >=3.7,<4.0
```

