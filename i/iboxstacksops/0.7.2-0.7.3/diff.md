# Comparing `tmp/iboxstacksops-0.7.2.tar.gz` & `tmp/iboxstacksops-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iboxstacksops-0.7.2.tar", last modified: Tue Apr 11 14:50:01 2023, max compression
+gzip compressed data, was "iboxstacksops-0.7.3.tar", last modified: Thu May 11 16:27:45 2023, max compression
```

## Comparing `iboxstacksops-0.7.2.tar` & `iboxstacksops-0.7.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.2/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.093030 iboxstacksops-0.7.2/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.093030 iboxstacksops-0.7.2/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.097030 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-04-11 14:50:00.000000 iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/iboxstacksops/
--rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.2/iboxstacksops/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.2/iboxstacksops/actions.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.2/iboxstacksops/aws.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4059 2023-03-30 09:41:57.000000 iboxstacksops-0.7.2/iboxstacksops/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5343 2023-03-30 13:07:04.000000 iboxstacksops-0.7.2/iboxstacksops/changeset.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4186 2023-03-29 07:47:32.000000 iboxstacksops-0.7.2/iboxstacksops/commands.py
--rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.2/iboxstacksops/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.2/iboxstacksops/dashboard.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.2/iboxstacksops/events.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.2/iboxstacksops/i_region.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6241 2023-04-11 14:33:36.000000 iboxstacksops-0.7.2/iboxstacksops/i_stack.py
--rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.2/iboxstacksops/msg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1299 2021-09-05 11:44:37.000000 iboxstacksops-0.7.2/iboxstacksops/outputs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8666 2023-04-11 14:46:17.000000 iboxstacksops-0.7.2/iboxstacksops/parameters.py
--rw-r--r--   0 mello     (1000) mello     (1000)    17122 2023-04-11 14:44:45.000000 iboxstacksops-0.7.2/iboxstacksops/parser.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.2/iboxstacksops/replica.py
--rw-r--r--   0 mello     (1000) mello     (1000)    10003 2023-03-22 10:22:38.000000 iboxstacksops-0.7.2/iboxstacksops/resolve.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.2/iboxstacksops/resources.py
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.2/iboxstacksops/route53.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.2/iboxstacksops/ssm.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.2/iboxstacksops/stacks.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.2/iboxstacksops/table.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2081 2021-10-28 09:48:26.000000 iboxstacksops-0.7.2/iboxstacksops/tags.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.2/iboxstacksops/template.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.2/iboxstacksops/tools.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.2/scripts/ibox_stacksops.py
--rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-04-11 14:50:01.109030 iboxstacksops-0.7.2/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-04-11 14:49:46.000000 iboxstacksops-0.7.2/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:27:45.247710 iboxstacksops-0.7.3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-11 16:27:45.247710 iboxstacksops-0.7.3/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.3/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:27:45.231710 iboxstacksops-0.7.3/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:27:45.231710 iboxstacksops-0.7.3/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:27:45.235710 iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-11 16:27:44.000000 iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-11 16:27:44.000000 iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-11 16:27:44.000000 iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-11 16:27:44.000000 iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-11 16:27:44.000000 iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:27:45.247710 iboxstacksops-0.7.3/iboxstacksops/
+-rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.3/iboxstacksops/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.3/iboxstacksops/actions.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.3/iboxstacksops/aws.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4070 2023-05-11 16:25:29.000000 iboxstacksops-0.7.3/iboxstacksops/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5343 2023-03-30 13:07:04.000000 iboxstacksops-0.7.3/iboxstacksops/changeset.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4186 2023-03-29 07:47:32.000000 iboxstacksops-0.7.3/iboxstacksops/commands.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.3/iboxstacksops/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.3/iboxstacksops/dashboard.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.3/iboxstacksops/events.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.3/iboxstacksops/i_region.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6241 2023-04-11 14:33:36.000000 iboxstacksops-0.7.3/iboxstacksops/i_stack.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.3/iboxstacksops/msg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1299 2021-09-05 11:44:37.000000 iboxstacksops-0.7.3/iboxstacksops/outputs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8666 2023-04-11 14:46:17.000000 iboxstacksops-0.7.3/iboxstacksops/parameters.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.3/iboxstacksops/parser.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.3/iboxstacksops/replica.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.3/iboxstacksops/resolve.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.3/iboxstacksops/resources.py
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.3/iboxstacksops/route53.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.3/iboxstacksops/ssm.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.3/iboxstacksops/stacks.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.3/iboxstacksops/table.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.3/iboxstacksops/tags.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.3/iboxstacksops/template.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.3/iboxstacksops/tools.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:27:45.247710 iboxstacksops-0.7.3/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.3/scripts/ibox_stacksops.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-11 16:27:45.251711 iboxstacksops-0.7.3/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-11 16:26:31.000000 iboxstacksops-0.7.3/setup.py
```

### Comparing `iboxstacksops-0.7.2/PKG-INFO` & `iboxstacksops-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.2
+Version: 0.7.3
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/PKG-INFO` & `iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.2
+Version: 0.7.3
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.2/build/lib/iboxstacksops.egg-info/SOURCES.txt` & `iboxstacksops-0.7.3/build/lib/iboxstacksops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/actions.py` & `iboxstacksops-0.7.3/iboxstacksops/actions.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/aws.py` & `iboxstacksops-0.7.3/iboxstacksops/aws.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/cfg.py` & `iboxstacksops-0.7.3/iboxstacksops/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # parser default cfg
-stack = role = type = topics = stack_args = []
+stack = role = type = topics = stack_args = cmd_args = []
 parallel = region = jobs = pause = version = template = None
 nowait = compact = dryrun = answer_yes = no_stacks = all_stacks = None
 debug = False
 max_retry_ecs_service_running_count = 0
 timedelta = 300
 dashboard = "OnChange"
 statistic = "Average"
```

### Comparing `iboxstacksops-0.7.2/iboxstacksops/changeset.py` & `iboxstacksops-0.7.3/iboxstacksops/changeset.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/commands.py` & `iboxstacksops-0.7.3/iboxstacksops/commands.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/common.py` & `iboxstacksops-0.7.3/iboxstacksops/common.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/dashboard.py` & `iboxstacksops-0.7.3/iboxstacksops/dashboard.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/events.py` & `iboxstacksops-0.7.3/iboxstacksops/events.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/i_region.py` & `iboxstacksops-0.7.3/iboxstacksops/i_region.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/i_stack.py` & `iboxstacksops-0.7.3/iboxstacksops/i_stack.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/msg.py` & `iboxstacksops-0.7.3/iboxstacksops/msg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/outputs.py` & `iboxstacksops-0.7.3/iboxstacksops/outputs.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/parameters.py` & `iboxstacksops-0.7.3/iboxstacksops/parameters.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/parser.py` & `iboxstacksops-0.7.3/iboxstacksops/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,14 +382,21 @@
     )
     parser.add_argument(
         "--disable_rollback",
         help="Preserve the state of previously provisioned "
         "resources when an operation fails",
         action="store_true",
     )
+    parser.add_argument(
+        "--tags",
+        nargs="+",
+        help="Tags, space separated, to associate with this stack. Use syntax: Key=Value",
+        type=str,
+        default=[],
+    )
 
     return parser
 
 
 # parse main argumets
 def get_parser():
     parser = argparse.ArgumentParser(
```

### Comparing `iboxstacksops-0.7.2/iboxstacksops/replica.py` & `iboxstacksops-0.7.3/iboxstacksops/replica.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/resolve.py` & `iboxstacksops-0.7.3/iboxstacksops/resolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 r_value = _recursive_resolve(n, l)
 
                 if not _awsnovalue(r_value):
                     r_root.append(r_value)
 
             return r_root
 
-        elif isinstance(value, (int, str)):
+        elif isinstance(value, (int, str, float)):
 
             return value
 
     def _resolve_sub(name, value):
         if isinstance(value, list):
             sub_string = value[0]
             sub_data = value[1]
```

### Comparing `iboxstacksops-0.7.2/iboxstacksops/resources.py` & `iboxstacksops-0.7.3/iboxstacksops/resources.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/route53.py` & `iboxstacksops-0.7.3/iboxstacksops/route53.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/ssm.py` & `iboxstacksops-0.7.3/iboxstacksops/ssm.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/stacks.py` & `iboxstacksops-0.7.3/iboxstacksops/stacks.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/table.py` & `iboxstacksops-0.7.3/iboxstacksops/table.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/tags.py` & `iboxstacksops-0.7.3/iboxstacksops/tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from .common import *
 
 
 def get_action_tags(istack, stack_tags):
+    # cmd lines tags
+    cmd_tags = {n.split("=")[0]: n.split("=")[1] for n in istack.cfg.tags}
+    tags_cmd = {}
+    tags_remove = {}
+
     # unchanged tags
     tags_default = {}
 
     # changed tags - same value as corresponding stack param
     tags_changed = {}
     final_tags = []
 
@@ -30,37 +35,53 @@
 
             # tags value cannot be empty
             if len(value) == 0:
                 value = "empty"
 
             tags_changed[key] = "%s => %s" % (current_value, value)
 
+        # remove tags using cmd --tags with tag value REMOVE
+        elif key in cmd_tags and cmd_tags[key] == "REMOVE":
+            tags_remove[key] = "REMOVE"
+            continue
         # keep current tag value
         else:
             value = current_value
 
             # tags value cannot be empty
             if len(value) == 0:
                 value = "empty"
 
             tags_default[key] = value
 
         final_tags.append({"Key": key, "Value": value})
 
+    # Add cmd tags that do not have as Value REMOVE
+    for key, value in cmd_tags.items():
+        if value != "REMOVE":
+            final_tags.append({"Key": key, "Value": value})
+            tags_cmd[key] = value
+
     # Add LastUpdate Tag with current time
     # Currently disabled:
     # Some resource, like CloudFormation Distribution, take time to be updated.
     # Does it make sense to have a tag with LastUpdateTime even if resource properties are not changed at all ?
     # If a resource is created by CloudFormation i can simply look at Stack LastUpdateTime
     # to have the same information derived by tagging it (i know that with tagging is simpler to do this).
     # final_tags.append({"Key": "LastUpdate", "Value": str(datetime.now())})
 
-    if len(tags_default) > 0:
+    if tags_default:
         istack.mylog(
             "DEFAULT - STACK TAGS\n%s\n" % pformat(tags_default, width=1000000)
         )
-    if len(tags_changed) > 0:
+    if tags_changed:
         istack.mylog(
             "CHANGED - STACK TAGS\n%s\n" % pformat(tags_changed, width=1000000)
         )
+    if tags_cmd:
+        istack.mylog(
+            "COMMAND LINE - STACK TAGS\n%s\n" % pformat(tags_cmd, width=1000000)
+        )
+    if tags_remove:
+        istack.mylog("REMOVE - STACK TAGS\n%s\n" % pformat(tags_remove, width=1000000))
 
     return final_tags
```

### Comparing `iboxstacksops-0.7.2/iboxstacksops/template.py` & `iboxstacksops-0.7.3/iboxstacksops/template.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/iboxstacksops/tools.py` & `iboxstacksops-0.7.3/iboxstacksops/tools.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.2/setup.py` & `iboxstacksops-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iboxstacksops",
-    version="0.7.2",
+    version="0.7.3",
     author="Mello",
     author_email="mello+python@ankot.org",
     description="AWS Infrastructure in a Box - Stacks management program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mello7tre/AwsIBoxStackOps",
     packages=["iboxstacksops",],
```

