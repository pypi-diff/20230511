# Comparing `tmp/batframes-1.0.0.6.tar.gz` & `tmp/batframes-1.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batframes-1.0.0.6.tar", last modified: Wed May 10 14:01:12 2023, max compression
+gzip compressed data, was "batframes-1.0.0.7.tar", last modified: Wed May 10 21:55:50 2023, max compression
```

## Comparing `batframes-1.0.0.6.tar` & `batframes-1.0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:01:12.743739 batframes-1.0.0.6/
--rw-rw-rw-   0        0        0      330 2023-05-10 14:01:12.742739 batframes-1.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-04-06 11:08:10.000000 batframes-1.0.0.6/README.md
--rw-rw-rw-   0        0        0     9590 2023-04-07 22:32:48.000000 batframes-1.0.0.6/bat_function_call_define.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:01:12.719733 batframes-1.0.0.6/bat_inner_module/
--rw-rw-rw-   0        0        0      227 2023-04-07 22:37:37.000000 batframes-1.0.0.6/bat_inner_module/inner_demo.py
--rw-rw-rw-   0        0        0      143 2023-04-07 15:30:40.000000 batframes-1.0.0.6/bat_inner_module/inner_demo1.py
--rw-rw-rw-   0        0        0      173 2023-04-07 10:56:05.000000 batframes-1.0.0.6/bat_inner_module/readme_for_inner.md
--rw-rw-rw-   0        0        0    68212 2023-04-08 01:59:23.000000 batframes-1.0.0.6/bat_menu_auto.py
--rw-rw-rw-   0        0        0    42764 2023-05-10 13:59:58.000000 batframes-1.0.0.6/batframe_main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:01:12.729736 batframes-1.0.0.6/batframes.egg-info/
--rw-rw-rw-   0        0        0      330 2023-05-10 14:01:12.000000 batframes-1.0.0.6/batframes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-05-10 14:01:12.000000 batframes-1.0.0.6/batframes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:01:12.000000 batframes-1.0.0.6/batframes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-10 14:01:12.000000 batframes-1.0.0.6/batframes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      308 2023-05-10 14:01:12.000000 batframes-1.0.0.6/batframes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       77 2023-05-10 14:01:12.000000 batframes-1.0.0.6/batframes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 14:01:12.705731 batframes-1.0.0.6/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:01:12.731737 batframes-1.0.0.6/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 batframes-1.0.0.6/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 14:01:12.733737 batframes-1.0.0.6/config/batframe/
--rw-rw-rw-   0        0        0     2816 2023-04-11 01:59:57.000000 batframes-1.0.0.6/config/batframe/bat_tools_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 14:01:12.740739 batframes-1.0.0.6/config/img/
--rw-rw-rw-   0        0        0     7631 2023-04-06 08:06:16.000000 batframes-1.0.0.6/config/img/Excel.png
--rw-rw-rw-   0        0        0     1962 2023-04-06 08:06:16.000000 batframes-1.0.0.6/config/img/excel.gif
--rw-rw-rw-   0        0        0    10200 2023-04-06 08:06:16.000000 batframes-1.0.0.6/config/img/little_bear.png
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 batframes-1.0.0.6/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 batframes-1.0.0.6/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0      585 2023-04-08 00:42:18.000000 batframes-1.0.0.6/nuitka_dependency_files.py
--rw-rw-rw-   0        0        0       42 2023-05-10 14:01:12.743739 batframes-1.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     6956 2023-05-10 14:00:23.000000 batframes-1.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.242826 batframes-1.0.0.7/
+-rw-rw-rw-   0        0        0      330 2023-05-10 21:55:50.241826 batframes-1.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-04-06 11:08:10.000000 batframes-1.0.0.7/README.md
+-rw-rw-rw-   0        0        0     9590 2023-04-07 22:32:48.000000 batframes-1.0.0.7/bat_function_call_define.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.221821 batframes-1.0.0.7/bat_inner_module/
+-rw-rw-rw-   0        0        0      227 2023-04-07 22:37:37.000000 batframes-1.0.0.7/bat_inner_module/inner_demo.py
+-rw-rw-rw-   0        0        0      143 2023-04-07 15:30:40.000000 batframes-1.0.0.7/bat_inner_module/inner_demo1.py
+-rw-rw-rw-   0        0        0      173 2023-04-07 10:56:05.000000 batframes-1.0.0.7/bat_inner_module/readme_for_inner.md
+-rw-rw-rw-   0        0        0    68212 2023-04-08 01:59:23.000000 batframes-1.0.0.7/bat_menu_auto.py
+-rw-rw-rw-   0        0        0    42908 2023-05-10 21:54:19.000000 batframes-1.0.0.7/batframe_main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.229823 batframes-1.0.0.7/batframes.egg-info/
+-rw-rw-rw-   0        0        0      330 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      308 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       77 2023-05-10 21:55:50.000000 batframes-1.0.0.7/batframes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.209819 batframes-1.0.0.7/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.231824 batframes-1.0.0.7/config/DFTrans/
+-rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 batframes-1.0.0.7/config/DFTrans/DFTrans_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.232824 batframes-1.0.0.7/config/batframe/
+-rw-rw-rw-   0        0        0     2816 2023-04-11 01:59:57.000000 batframes-1.0.0.7/config/batframe/bat_tools_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 21:55:50.240826 batframes-1.0.0.7/config/img/
+-rw-rw-rw-   0        0        0     7631 2023-04-06 08:06:16.000000 batframes-1.0.0.7/config/img/Excel.png
+-rw-rw-rw-   0        0        0     1962 2023-04-06 08:06:16.000000 batframes-1.0.0.7/config/img/excel.gif
+-rw-rw-rw-   0        0        0    10200 2023-04-06 08:06:16.000000 batframes-1.0.0.7/config/img/little_bear.png
+-rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 batframes-1.0.0.7/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 batframes-1.0.0.7/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0      585 2023-04-08 00:42:18.000000 batframes-1.0.0.7/nuitka_dependency_files.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 21:55:50.242826 batframes-1.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     6956 2023-05-10 21:54:48.000000 batframes-1.0.0.7/setup.py
```

### Comparing `batframes-1.0.0.6/bat_function_call_define.py` & `batframes-1.0.0.7/bat_function_call_define.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/bat_menu_auto.py` & `batframes-1.0.0.7/bat_menu_auto.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/batframe_main.py` & `batframes-1.0.0.7/batframe_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 from DFTrans_main import *
 
 
 # 工具启动的整体配置文件
 sysdefaultdirectory = "./config"
 battoolsconfig = "config/batframe/bat_tools_config.json"
 
-BATFRAME_SYSTEM_DATA_FILES = [battoolsconfig, SYSTEM_ICON]
+BATFRAME_SYSTEM_DATA_FILES = [battoolsconfig, SYSTEM_ICON,
+                              "config/img/excel.gif", "config/img/Excel.png",
+                              "config/img/little_bear.png", "config/img/table_arrow9_transparent_256.png"]
 
 commandtypelist = []
 commandtype2valuedic = {}
 
 
 def GraphicButton(text: str, key: str, image_data):
     text = text.replace('_', ' ')
@@ -826,16 +828,14 @@
         if debugpath.is_dir():
             commanddefaultfile = os.path.join(debugpathstring, commandfile)
         else:
             commanddefaultfile = os.path.join(".", commandfile)
 
         debugswitchdefault = 'n'
 
-        fileprocconfig = battoolsconfig
-
         # 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
         # 判断本地目录是否存在fileprocconfig
         result = sys_data_files_copy(BATFRAME_SYSTEM_DATA_FILES)
         if result[0] is False:
             print(result[1])
             sys.exit(-1)
```

### Comparing `batframes-1.0.0.6/batframes.egg-info/SOURCES.txt` & `batframes-1.0.0.7/batframes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/config/DFTrans/DFTrans_config.json` & `batframes-1.0.0.7/config/DFTrans/DFTrans_config.json`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/config/batframe/bat_tools_config.json` & `batframes-1.0.0.7/config/batframe/bat_tools_config.json`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/config/img/Excel.png` & `batframes-1.0.0.7/config/img/Excel.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/config/img/excel.gif` & `batframes-1.0.0.7/config/img/excel.gif`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/config/img/little_bear.png` & `batframes-1.0.0.7/config/img/little_bear.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/config/img/table_arrow9_transparent_256.png` & `batframes-1.0.0.7/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/config/img/table_arrow9_transparent_64.ico` & `batframes-1.0.0.7/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/nuitka_dependency_files.py` & `batframes-1.0.0.7/nuitka_dependency_files.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.6/setup.py` & `batframes-1.0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 00000b60: 6f6e 6669 6764 6972 2c20 5b6f 7267 696e  onfigdir, [orgin
 00000b70: 636f 6e66 6967 6669 6c65 5d29 2c0d 0a20  configfile]),.. 
 00000b80: 2020 2020 2020 205d 0d0a 2020 2020 7265         ]..    re
 00000b90: 7475 726e 2064 6174 615f 6669 6c65 730d  turn data_files.
 00000ba0: 0a0d 0a0d 0a73 6574 7570 280d 0a20 2020  .....setup(..   
 00000bb0: 206e 616d 653d 2762 6174 6672 616d 6573   name='batframes
 00000bc0: 272c 0d0a 2020 2020 7665 7273 696f 6e3d  ',..    version=
-00000bd0: 2731 2e30 2e30 2e36 272c 0d0a 2020 2020  '1.0.0.6',..    
+00000bd0: 2731 2e30 2e30 2e37 272c 0d0a 2020 2020  '1.0.0.7',..    
 00000be0: 6465 7363 7269 7074 696f 6e3d 27e5 8faf  description='...
 00000bf0: e4bb a5e9 858d e7bd aee5 b086 e5a4 9ae4  ................
 00000c00: b8aa e58f afe6 89a7 e8a1 8ce6 9687 e4bb  ................
 00000c10: b6e5 928c e586 85e9 83a8 e591 bde4 bba4  ................
 00000c20: e4b8 b2e6 8ea5 e688 90e4 b880 e4b8 aae5  ................
 00000c30: ae8c e695 b4e5 91bd e4bb a4e6 89a7 e8a1  ................
 00000c40: 8ce7 9a84 e6a1 86e6 9eb6 e5b7 a5e5 85b7  ................
```

