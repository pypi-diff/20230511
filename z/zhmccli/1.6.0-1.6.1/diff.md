# Comparing `tmp/zhmccli-1.6.0.tar.gz` & `tmp/zhmccli-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmccli-1.6.0.tar", last modified: Mon Mar 27 11:26:25 2023, max compression
+gzip compressed data, was "zhmccli-1.6.1.tar", last modified: Thu May 11 15:50:14 2023, max compression
```

## Comparing `zhmccli-1.6.0.tar` & `zhmccli-1.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:26:25.179613 zhmccli-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-03-27 11:25:33.000000 zhmccli-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-27 11:26:11.000000 zhmccli-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-03-27 11:26:25.179613 zhmccli-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-03-27 11:25:33.000000 zhmccli-1.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-27 11:25:33.000000 zhmccli-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 11:26:25.179613 zhmccli-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-03-27 11:25:33.000000 zhmccli-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:26:25.179613 zhmccli-1.6.0/zhmccli/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_capacitygroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_character_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    37856 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    32122 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    73313 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_storagegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_storagevolume.py
--rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_vfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_vstorageresource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_cmd_vswitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    54700 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-03-27 11:25:33.000000 zhmccli-1.6.0/zhmccli/zhmccli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 11:26:25.179613 zhmccli-1.6.0/zhmccli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-03-27 11:26:25.000000 zhmccli-1.6.0/zhmccli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-27 11:26:25.000000 zhmccli-1.6.0/zhmccli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 11:26:25.000000 zhmccli-1.6.0/zhmccli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 11:26:25.000000 zhmccli-1.6.0/zhmccli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-27 11:26:25.000000 zhmccli-1.6.0/zhmccli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 11:26:25.000000 zhmccli-1.6.0/zhmccli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 11:26:24.000000 zhmccli-1.6.0/zhmccli.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:50:14.812418 zhmccli-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-11 15:49:19.000000 zhmccli-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-11 15:50:02.000000 zhmccli-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-11 15:50:14.812418 zhmccli-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-11 15:49:19.000000 zhmccli-1.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-11 15:49:19.000000 zhmccli-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:50:14.812418 zhmccli-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-11 15:49:19.000000 zhmccli-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:50:14.808418 zhmccli-1.6.1/zhmccli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_capacitygroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_character_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37856 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32122 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73313 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_storagegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_storagevolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_vfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_vstorageresource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_vswitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54900 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/zhmccli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:50:14.812418 zhmccli-1.6.1/zhmccli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/zip-safe
```

### Comparing `zhmccli-1.6.0/LICENSE` & `zhmccli-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/MANIFEST.in` & `zhmccli-1.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/PKG-INFO` & `zhmccli-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.6.0
+Version: 1.6.1
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmccli-1.6.0/README.rst` & `zhmccli-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/requirements.txt` & `zhmccli-1.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/setup.py` & `zhmccli-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/__init__.py` & `zhmccli-1.6.1/zhmccli/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_adapter.py` & `zhmccli-1.6.1/zhmccli/_cmd_adapter.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_capacitygroup.py` & `zhmccli-1.6.1/zhmccli/_cmd_capacitygroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_character_rule.py` & `zhmccli-1.6.1/zhmccli/_cmd_character_rule.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_console.py` & `zhmccli-1.6.1/zhmccli/_cmd_console.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_cpc.py` & `zhmccli-1.6.1/zhmccli/_cmd_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_hba.py` & `zhmccli-1.6.1/zhmccli/_cmd_hba.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_info.py` & `zhmccli-1.6.1/zhmccli/_cmd_info.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_lpar.py` & `zhmccli-1.6.1/zhmccli/_cmd_lpar.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_metrics.py` & `zhmccli-1.6.1/zhmccli/_cmd_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_nic.py` & `zhmccli-1.6.1/zhmccli/_cmd_nic.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_partition.py` & `zhmccli-1.6.1/zhmccli/_cmd_partition.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_password_rule.py` & `zhmccli-1.6.1/zhmccli/_cmd_password_rule.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_port.py` & `zhmccli-1.6.1/zhmccli/_cmd_port.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_session.py` & `zhmccli-1.6.1/zhmccli/_cmd_session.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_storagegroup.py` & `zhmccli-1.6.1/zhmccli/_cmd_storagegroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_storagevolume.py` & `zhmccli-1.6.1/zhmccli/_cmd_storagevolume.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_user.py` & `zhmccli-1.6.1/zhmccli/_cmd_user.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_user_role.py` & `zhmccli-1.6.1/zhmccli/_cmd_user_role.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_vfunction.py` & `zhmccli-1.6.1/zhmccli/_cmd_vfunction.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_vstorageresource.py` & `zhmccli-1.6.1/zhmccli/_cmd_vstorageresource.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_cmd_vswitch.py` & `zhmccli-1.6.1/zhmccli/_cmd_vswitch.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli/_helper.py` & `zhmccli-1.6.1/zhmccli/_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,16 @@
         table.append(row)
 
     cmd_ctx.spinner.stop()
     if not table:
         click.echo("No resources.")
     else:
         sorted_table = sorted(table, key=lambda row: row[0])
-        out_str = tabulate(sorted_table, prop_names, tablefmt=table_format)
+        out_str = tabulate(sorted_table, prop_names, tablefmt=table_format,
+                           disable_numparse=True)
         click.echo(out_str)
 
 
 def print_dicts_as_table(
         cmd_ctx, dicts, table_format, show_list=None, additions=None,
         all=False):
     # pylint: disable=redefined-builtin
@@ -792,15 +793,16 @@
         table.append(row)
 
     cmd_ctx.spinner.stop()
     if not table:
         click.echo("No items.")
     else:
         sorted_table = sorted(table, key=lambda row: row[0])
-        out_str = tabulate(sorted_table, prop_names, tablefmt=table_format)
+        out_str = tabulate(sorted_table, prop_names, tablefmt=table_format,
+                           disable_numparse=True)
         click.echo(out_str)
 
 
 def dict_as_table(data, headers, table_format, show_list=None):
     """
     Return a string with the dictionary data in tabular output format.
 
@@ -823,15 +825,16 @@
         table = []
         inner_format = INNER_TABLE_FORMAT.get(table_format, table_format)
         sorted_fields = sorted(data)
         for field in sorted_fields:
             if show_list is None or field in show_list:
                 value = value_as_table(data[field], inner_format)
                 table.append((field, value))
-        ret_str = tabulate(table, headers, tablefmt=table_format)
+        ret_str = tabulate(table, headers, tablefmt=table_format,
+                           disable_numparse=True)
     return ret_str
 
 
 def list_as_table(data, table_format):
     """
     Return a string with the list data in tabular output format.
 
@@ -847,15 +850,16 @@
         ret_str = repr(data)
     else:
         table = []
         inner_format = INNER_TABLE_FORMAT.get(table_format, table_format)
         for value in data:
             value = value_as_table(value, inner_format)
             table.append((value,))
-        ret_str = tabulate(table, headers=[], tablefmt=table_format)
+        ret_str = tabulate(table, headers=[], tablefmt=table_format,
+                           disable_numparse=True)
     return ret_str
 
 
 def value_as_table(value, table_format):
     """
     Return the value in the table format.
```

### Comparing `zhmccli-1.6.0/zhmccli/_version.py` & `zhmccli-1.6.1/zhmccli/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.U.dev1": A not yet released version M.N.U
 #: * "M.N.U": A released version M.N.U
-__version__ = '1.6.0'
+__version__ = '1.6.1'
```

### Comparing `zhmccli-1.6.0/zhmccli/zhmccli.py` & `zhmccli-1.6.1/zhmccli/zhmccli.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli.egg-info/PKG-INFO` & `zhmccli-1.6.1/zhmccli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.6.0
+Version: 1.6.1
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmccli-1.6.0/zhmccli.egg-info/SOURCES.txt` & `zhmccli-1.6.1/zhmccli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.0/zhmccli.egg-info/requires.txt` & `zhmccli-1.6.1/zhmccli.egg-info/requires.txt`

 * *Files identical despite different names*

