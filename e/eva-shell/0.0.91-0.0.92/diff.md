# Comparing `tmp/eva-shell-0.0.91.tar.gz` & `tmp/eva-shell-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva-shell-0.0.91.tar", last modified: Tue Jan 31 19:57:00 2023, max compression
+gzip compressed data, was "eva-shell-0.0.92.tar", last modified: Thu May 11 15:47:04 2023, max compression
```

## Comparing `eva-shell-0.0.91.tar` & `eva-shell-0.0.92.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-01-31 19:57:00.014638 eva-shell-0.0.91/
--rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:07.000000 eva-shell-0.0.91/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      459 2023-01-31 19:57:00.014638 eva-shell-0.0.91/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.0.91/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-01-31 19:57:00.014638 eva-shell-0.0.91/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.0.91/bin/eva
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-01-31 19:57:00.014638 eva-shell-0.0.91/eva4_shell/
--rw-r--r--   0 divisor   (1000) root         (0)       75 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    47320 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/ap.py
--rw-r--r--   0 divisor   (1000) root         (0)     7078 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/charts.py
--rw-r--r--   0 divisor   (1000) root         (0)    51423 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/cli.py
--rw-r--r--   0 divisor   (1000) root         (0)     2634 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/client.py
--rw-r--r--   0 divisor   (1000) root         (0)     4332 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/compl.py
--rw-r--r--   0 divisor   (1000) root         (0)      653 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/sharedobj.py
--rw-r--r--   0 divisor   (1000) root         (0)     1701 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/shell.py
--rw-r--r--   0 divisor   (1000) root         (0)    13863 2023-01-31 19:56:58.000000 eva-shell-0.0.91/eva4_shell/tools.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-01-31 19:57:00.014638 eva-shell-0.0.91/eva_shell.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      459 2023-01-31 19:56:59.000000 eva-shell-0.0.91/eva_shell.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      382 2023-01-31 19:56:59.000000 eva-shell-0.0.91/eva_shell.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-01-31 19:56:59.000000 eva-shell-0.0.91/eva_shell.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)      166 2023-01-31 19:56:59.000000 eva-shell-0.0.91/eva_shell.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       11 2023-01-31 19:56:59.000000 eva-shell-0.0.91/eva_shell.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-01-31 19:57:00.014638 eva-shell-0.0.91/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1188 2023-01-31 19:56:58.000000 eva-shell-0.0.91/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:07.000000 eva-shell-0.0.92/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-11 15:47:04.744640 eva-shell-0.0.92/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.0.92/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.0.92/bin/eva
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/eva4_shell/
+-rw-r--r--   0 divisor   (1000) root         (0)       75 2023-05-04 21:53:31.000000 eva-shell-0.0.92/eva4_shell/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    47371 2023-05-04 21:53:31.000000 eva-shell-0.0.92/eva4_shell/ap.py
+-rw-r--r--   0 divisor   (1000) root         (0)     7078 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/charts.py
+-rw-r--r--   0 divisor   (1000) root         (0)    51586 2023-05-04 21:53:31.000000 eva-shell-0.0.92/eva4_shell/cli.py
+-rw-r--r--   0 divisor   (1000) root         (0)     2634 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/client.py
+-rw-r--r--   0 divisor   (1000) root         (0)     4332 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/compl.py
+-rw-r--r--   0 divisor   (1000) root         (0)      653 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/sharedobj.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1701 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/shell.py
+-rw-r--r--   0 divisor   (1000) root         (0)    13863 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/tools.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/eva_shell.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      382 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)      166 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       11 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-11 15:47:04.744640 eva-shell-0.0.92/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1188 2023-05-04 21:53:31.000000 eva-shell-0.0.92/setup.py
```

### Comparing `eva-shell-0.0.91/LICENSE` & `eva-shell-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.91/eva4_shell/ap.py` & `eva-shell-0.0.92/eva4_shell/ap.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,16 @@
                    help='limit action list to')
 
 
 def append_broker_cli(root_sp):
     ap = root_sp.add_parser('broker', help='bus broker commands')
     sp = ap.add_subparsers(dest='_subc', help='sub command')
 
-    sp.add_parser('client.list', help='list registered bus clients')
+    p = sp.add_parser('client.list', help='list registered bus clients')
+    p.add_argument('-x', '--filter', type=str)
     sp.add_parser('test', help='test broker')
     sp.add_parser('info', help='broker info')
     sp.add_parser('stats', help='broker stats')
 
 
 def append_svc_cli(root_sp):
     ap = root_sp.add_parser('svc', help='service commands')
```

### Comparing `eva-shell-0.0.91/eva4_shell/charts.py` & `eva-shell-0.0.92/eva4_shell/charts.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.91/eva4_shell/cli.py` & `eva-shell-0.0.92/eva4_shell/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -624,16 +624,20 @@
         data = call_rpc('info', target='.broker')
         print_result(data, need_header=False, name_value=True)
 
     def broker_stats(self):
         data = call_rpc('stats', target='.broker')
         print_result(data, need_header=False, name_value=True)
 
-    def broker_client_list(self):
-        data = call_rpc('client.list', target='.broker')
+    def broker_client_list(self, filter=None):
+        if filter is None:
+            params = None
+        else:
+            params = dict(filter='^' + filter.replace('.', '\\.') + '.*$')
+        data = call_rpc('client.list', params, target='.broker')
         if current_command.json:
             print_result(data)
         else:
             print_result(
                 [d for d in data['clients'] if d['name'] != common.bus_name],
                 cols=[
                     'name', 'kind|n=type', 'source', 'port', 'r_frames',
```

### Comparing `eva-shell-0.0.91/eva4_shell/client.py` & `eva-shell-0.0.92/eva4_shell/client.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.91/eva4_shell/compl.py` & `eva-shell-0.0.92/eva4_shell/compl.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.91/eva4_shell/sharedobj.py` & `eva-shell-0.0.92/eva4_shell/sharedobj.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.91/eva4_shell/shell.py` & `eva-shell-0.0.92/eva4_shell/shell.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.91/eva4_shell/tools.py` & `eva-shell-0.0.92/eva4_shell/tools.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.91/setup.py` & `eva-shell-0.0.92/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.91'
+__version__ = '0.0.92'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eva-shell',
```

