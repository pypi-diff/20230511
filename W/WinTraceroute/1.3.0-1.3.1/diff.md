# Comparing `tmp/WinTraceroute-1.3.0.tar.gz` & `tmp/WinTraceroute-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinTraceroute-1.3.0.tar", last modified: Tue May  9 22:49:36 2023, max compression
+gzip compressed data, was "WinTraceroute-1.3.1.tar", last modified: Thu May 11 14:08:37 2023, max compression
```

## Comparing `WinTraceroute-1.3.0.tar` & `WinTraceroute-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/WinTraceroute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/traceroute/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/traceroute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/traceroute/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/traceroute/traceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:08:37.947989 WinTraceroute-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-11 14:07:59.000000 WinTraceroute-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-11 14:08:37.947989 WinTraceroute-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-11 14:07:59.000000 WinTraceroute-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:08:37.947989 WinTraceroute-1.3.1/WinTraceroute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-11 14:08:37.000000 WinTraceroute-1.3.1/WinTraceroute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 14:08:37.000000 WinTraceroute-1.3.1/WinTraceroute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:08:37.000000 WinTraceroute-1.3.1/WinTraceroute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 14:08:37.000000 WinTraceroute-1.3.1/WinTraceroute.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 14:08:37.000000 WinTraceroute-1.3.1/WinTraceroute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 14:08:37.000000 WinTraceroute-1.3.1/WinTraceroute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-11 14:07:59.000000 WinTraceroute-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:08:37.947989 WinTraceroute-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:08:37.947989 WinTraceroute-1.3.1/traceroute/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:07:59.000000 WinTraceroute-1.3.1/traceroute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-11 14:07:59.000000 WinTraceroute-1.3.1/traceroute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100486 2023-05-11 14:07:59.000000 WinTraceroute-1.3.1/traceroute/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-05-11 14:07:59.000000 WinTraceroute-1.3.1/traceroute/traceroute.py
```

### Comparing `WinTraceroute-1.3.0/LICENSE` & `WinTraceroute-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.0/PKG-INFO` & `WinTraceroute-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.0
+Version: 1.3.1
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.0/README.md` & `WinTraceroute-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 ```
 $ sudo wintraceroute 8.8.8.8
 
   1        8.238           4.052           3.911        ###.###.###.###
   2       12.462                          12.313        62.155.###.###
                             *                            (no response)
   3       21.610          19.516          18.816        217.5.118.26
-  4       19.093          19.010          20.092        87.128.238.134
+  4       19.093          19.010                        87.128.238.134
+                                          20.092        87.128.238.132
   5         *               *               *            (no response)
   6       21.839          21.319          27.482        8.8.8.8
 
 Destination '8.8.8.8' reached  in RTT min. 21.319, avg. 23.547, max. 27.482 ms  via 6 hops.
 ```
 
 See also the help page, available using the `-h` or `--help` option.
@@ -46,15 +47,15 @@
 
 ### Via `pip` / from PyPI
 
 If you are running *Python 3.9* or above, you may want to install WinTraceroute via `pip`. This also tries to register the `wintraceroute` command in your system.
 
 **Just run `pip install WinTraceroute` in your local Python environment** and make sure you have a *Pcap provider* installed, for example libpcap on Linux or Npcap on Windows.
 
-:information_source: Tip for *Linux/Debian* users: Use the `--system` pip option to install for all users, so that you don't have to install using `sudo`.
+:information_source: Tip for *Linux/Debian* users: If available, use the `--system` pip option to install for all users, so that you don't have to install using `sudo`.
 
 :exclamation: If you have problems with this strategy of installation, consider loading / building a binary for your respective operating system -- see below.
 
 You may also want to head over to [this project on PyPI](https://pypi.org/project/WinTraceroute/).
 
 ### Windows Binary
 
@@ -80,14 +81,15 @@
  * You can find the output binary in the `_dist_out/lnx/` directory.
 
 ### run directly from source
 
 You can also just run this program on your *Python 3.9* or newer environment from source by cloning/downloading the code, entering the directory and then running
  * `<your_python> -m traceroute`
     * ... where for example `<your_python>` == `python3`.
-    * Note: `traceroute` is the "traceroute" directory in the source, *not* `traceroute.py` within that directory!
+    * :information_source: Note: `traceroute` is the "traceroute" directory in the source, *not* `traceroute.py` within that directory!
+    * :exclamation: Make sure you type `traceroute`, not for example `traceroute/` with a slash. 
 
 ## License
 
 This project is published under the GPL v2.0 license.
 
 Scapy, which this project uses, is published under the GPL v2.0 license, at the time of writing.
```

### Comparing `WinTraceroute-1.3.0/WinTraceroute.egg-info/PKG-INFO` & `WinTraceroute-1.3.1/WinTraceroute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.0
+Version: 1.3.1
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.0/pyproject.toml` & `WinTraceroute-1.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "bumpver", "scapy==2.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WinTraceroute"
-version = "1.3.0"
+version = "1.3.1"
 description = "A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta"
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pyinstaller==5.10.1"]
 
 [project.urls]
 Homepage = "https://github.com/NiRit100/WinTraceroute"
 
 [tool.bumpver]
-current_version = "1.3.0"
+current_version = "1.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 # (BETA) tells setuptools you will be using a readme file for the long description field for your pypi profile.
```

### Comparing `WinTraceroute-1.3.0/traceroute/__main__.py` & `WinTraceroute-1.3.1/traceroute/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,21 +59,33 @@
         help="""source address of outgoing packets.
                 (default is address of adapter used)""")
     parser.add_argument('-M', '--module', \
                         default='UDP', choices=['UDP', 'ICMP'], \
         help="""module (or method) for traceroute
                 operations.
                 (default = UDP)""")
+    parser.add_argument('-j', '--udp-junk', default='42', \
+                        choices=['42', 'zeros', '00', 'loremipsum', 'asc'],
+        help="""contents of the to-be-sent UDP segments in UDP mode.
+                It has no further purpose than adding weight to the 
+                segments, but there are several available.""")
+    parser.add_argument('-i', '--no-ip-id-variation', \
+                        action='store_const', \
+                        const=True, default=False, \
+        help="""do *not* vary the IP segment 
+                'Identification' field.""")
     parser.add_argument('--no-legacy-python-notice', \
                         dest='show_legacy_py_notice', \
                         action='store_const', \
                         const=False, default=True, \
-        help="""Disable the legacy python version notice.""")
+        help="""disables the legacy python version notice.""")
     args = parser.parse_args()
     
+    # TODO: make id vary by default and add switch to turn it off
+    
     if args.show_legacy_py_notice and py_version_info <= (3, 9):
         print()
         print()
         print("NOTE: This software runs best under Python 3.9 and later.")
         print("      It is currently running on Python " + \
             str(py_version_info.major) + "." + str(py_version_info.minor) + ".")
         print("      The program can still be executed, but it might show some" \
@@ -90,25 +102,27 @@
             trace_udp(args.remote_host,
                     udp_length=int(args.packet_length),
                     min_ttl=int(args.minttl),
                     max_ttl=int(args.maxttl),
                     num_per_fleet=int(args.fleetsize),
                     timeout=int(args.timeout),
                     port=int(args.port),
-                    source=args.source)
+                    udp_content=args.udp_junk,
+                    source=args.source,
+                    ip_id_variation=(not args.no_ip_id_variation))
         elif args.module == 'ICMP':
             print("Note: ICMP mode is experimental.")
             print()
             trace_icmp(args.remote_host,
                     min_ttl=int(args.minttl),
                     max_ttl=int(args.maxttl),
                     num_per_fleet=int(args.fleetsize),
                     timeout=int(args.timeout),
-                    port=int(args.port),
-                    source=args.source)
+                    source=args.source,
+                    ip_id_variation=(not args.no_ip_id_variation))
         else:
             print('Module ' + args.module + ' is not supported.')
         return 0
     except PermissionError:
         print("Error: Please run this program with higher privileges.")
         exit(1)
```

### Comparing `WinTraceroute-1.3.0/traceroute/traceroute.py` & `WinTraceroute-1.3.1/traceroute/traceroute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import sys, math
+import sys, math, random
 from typing import Callable, Any
 from abc import ABC, abstractmethod
 from scapy.plist import SndRcvList, PacketList
-from scapy.all import IP, UDP, ICMP, sr1
+from scapy.all import IP, UDP, ICMP, Raw, sr1
+from traceroute.lorem import lorem
 
 
-PRINT_FILE = sys.stdout
-
+_WINTRACEROUTE_PRINT_FILE = sys.stdout
+_WINTRACEROUTE_IP_ID = 42
 
 def trace(host:str,
           IP_PACKET_SUPPLIER=Callable[[str,str,int],Any],
           DATAGRAM_SUPPLIER=Callable[[int],Any],
           min_ttl:int=1,
           max_ttl:int=30,
           num_per_fleet:int=3,
@@ -29,15 +30,15 @@
     dest_reached = False
     for ttl in range(min_ttl, max_ttl+1):
         # this is for each ttl
         ttl_responses = list()
         ttl_times = list()
         # print ttl index
         print(' ', f_ttl_str_format.format(ttl), "\t",  sep='', end='', \
-                file=PRINT_FILE)
+                file=_WINTRACEROUTE_PRINT_FILE)
         for _ in range(num_per_fleet):
             # this is for each packet in the fleet (3 by default)
             packet = IP_PACKET_SUPPLIER(host, source, ttl) / \
                      DATAGRAM_SUPPLIER(port)
             response = sr1(packet, timeout=timeout, verbose=False)
             if response:
                 ttl_responses.append(response)
@@ -68,35 +69,46 @@
 def trace_udp(host:str,
               udp_length=2,
               min_ttl:int=1,
               max_ttl:int=30,
               num_per_fleet:int=3,
               timeout:int=5,
               port:int=33434,
-              source:str=None):
+              udp_content:str='asc',
+              source:str=None,
+              ip_id_variation:bool=True):
+    
+    change_ip_id(True)
+    
     ip_packet_supplier = \
         lambda host, source, ttl: \
-            make_ip_packet(host=host, source=source, ttl=ttl)
+            make_ip_packet(host=host, source=source, 
+                           ttl=ttl, ip_id_variation=ip_id_variation)
     datagram_supplier = \
         lambda port: \
-            make_udp_packet(port=port) / get_junk(udp_length)
+            make_udp_packet(port=port) / get_junk(udp_length, kind=udp_content)
     trace(host, ip_packet_supplier, datagram_supplier,
           min_ttl=min_ttl, max_ttl=max_ttl, num_per_fleet=num_per_fleet,
           timeout=timeout, port=port, source=source)
 
 def trace_icmp(host:str,
                min_ttl:int=1,
                max_ttl:int=30,
                num_per_fleet:int=3,
                timeout:int=5,
                port:int=33434,
-               source:str=None):
+               source:str=None,
+               ip_id_variation:bool=True):
+    
+    change_ip_id(True)
+        
     ip_packet_supplier = \
         lambda host, source, ttl: \
-            make_ip_packet(host=host, source=source, ttl=ttl)
+            make_ip_packet(host=host, source=source, 
+                           ttl=ttl, ip_id_variation=ip_id_variation)
     datagram_supplier = \
         lambda port: \
             make_icmp_packet()  # ignore port on icmp
     trace(host, ip_packet_supplier, datagram_supplier,
           min_ttl=min_ttl, max_ttl=max_ttl, num_per_fleet=num_per_fleet,
           timeout=timeout, port=port, source=source)
 
@@ -117,53 +129,56 @@
             sorted_responses[response_source].append(i)
         else:
             sorted_responses[response_source] = [i]
     # now print results
     is_first_line = True
     for host in sorted_responses.keys():
         if is_first_line:
-            print(firstline_pfx, end='', file=PRINT_FILE)
+            print(firstline_pfx, end='', file=_WINTRACEROUTE_PRINT_FILE)
         else:
-            print(restlines_pfx, end='', file=PRINT_FILE)
+            print(restlines_pfx, end='', file=_WINTRACEROUTE_PRINT_FILE)
         indices = sorted_responses[host]
         for i in range(0, fleetsize):
             if i in indices:
                 time = times[i]
                 if time == None:
-                    print(' '*(time_str_width-4) + '*   ' + '\t', end='', file=PRINT_FILE)
+                    print(' '*(time_str_width-4) + '*   ' + '\t', end='', 
+                          file=_WINTRACEROUTE_PRINT_FILE)
                 else:
-                    print(time_str_format.format(time) + '\t', end='', file=PRINT_FILE)
+                    print(time_str_format.format(time) + '\t', end='', 
+                          file=_WINTRACEROUTE_PRINT_FILE)
             else:
-                print(' '*time_str_width + '\t', end='', file=PRINT_FILE)
-        print(host, file=PRINT_FILE)
+                print(' '*time_str_width + '\t', end='', 
+                      file=_WINTRACEROUTE_PRINT_FILE)
+        print(host, file=_WINTRACEROUTE_PRINT_FILE)
         is_first_line = False
 
 def is_dest_reached(responses:list, dest):
     for rt in responses:
         if rt == None:
             continue
         else:
             rt_icmp = rt[ICMP]
             if rt_icmp.type == 3 or rt.src == dest:
                 return True  # Dest unreachable, port unavailable
     return False
 
 def summarize_termination(host, times, ttl, dest_reached):
-    print(file=PRINT_FILE)
+    print(file=_WINTRACEROUTE_PRINT_FILE)
     if dest_reached:
         print("Destination '" + host + "' reached " + \
             " in RTT " + summarize_times(times, as_string=True) + " ms " + \
             " via " + str(ttl) + " hops.", \
-            file=PRINT_FILE)
+            file=_WINTRACEROUTE_PRINT_FILE)
     else:
         print("Maximum TTL reached, but no '" + host + "' in sight. Aborting.", \
-            file=PRINT_FILE)
+            file=_WINTRACEROUTE_PRINT_FILE)
         print("If you wish to continue the search, consider increasing the `--maxttl`\n" + \
             "  setting on the next try. Besides that, try a different `--module`, maybe?", \
-            file=PRINT_FILE)
+            file=_WINTRACEROUTE_PRINT_FILE)
 
 def summarize_times(times:list,
                     as_string:bool=False):
     min = times[0]
     max = times[0]
     sum = times[0]
 
@@ -179,27 +194,57 @@
 
     if as_string:
         return "min. %.3f, avg. %.3f, max. %.3f" % (min, avg, max)
     else:
         return (min, avg, max)
 
 
-def make_ip_packet(host:str, source:str, ttl:int):
+def make_ip_packet(host:str, source:str, ttl:int, ip_id_variation:bool):
+    if ip_id_variation:
+        change_ip_id()
     if source != None:
-        packet = IP(dst=host, src=source, ttl=ttl)
+        packet = IP(id=_WINTRACEROUTE_IP_ID, 
+                    dst=host, 
+                    src=source, 
+                    ttl=ttl)
     else:
-        packet = IP(dst=host, ttl=ttl)
+        packet = IP(id=_WINTRACEROUTE_IP_ID,
+                    dst=host, 
+                    ttl=ttl)
     return packet
 
 def make_udp_packet(port:int):
     return UDP(dport=port)
 
 def make_icmp_packet():
     return ICMP(type=8)
     #return ICMP()
+    
 
-
-def get_junk(length=2):
-    ret = "42" * int(length/2)
-    if length%2 != 0:
-        ret += "!"
-    return ret
+def change_ip_id(first_time:bool=False):
+    global _WINTRACEROUTE_IP_ID
+    if first_time:
+        random.seed()
+    # the IP Identification field is 16 bits
+    _WINTRACEROUTE_IP_ID = random.randint(0, 2**16-1)
+    print(" --" + str(_WINTRACEROUTE_IP_ID) + "-- ")
+
+
+def get_junk(length=2, kind='42'):
+    if kind == '42':
+        ret = b"42" * int(length/2)
+        if length%2 != 0:
+            ret += "!"
+        return ret
+    elif kind == 'zeros':
+        return Raw(b"\x00"*length)
+    elif kind == '00':
+        return b"0"*length
+    elif kind == 'loremipsum':
+        return lorem[0:length]
+    elif kind == 'asc':
+        byts = bytes([n%256 for n in range(length)])
+        return Raw(byts)
+    else:
+        junk_msg = 'invalid kind of junk! '
+        junk_msg_infl = junk_msg * (int(length / 20) + 1)
+        return junk_msg_infl[0:length]
```

