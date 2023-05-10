# Comparing `tmp/enhanceezqq-1.0.0.6.tar.gz` & `tmp/enhanceezqq-1.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanceezqq-1.0.0.6.tar", last modified: Wed May 10 12:12:20 2023, max compression
+gzip compressed data, was "enhanceezqq-1.0.0.7.tar", last modified: Wed May 10 14:08:37 2023, max compression
```

## Comparing `enhanceezqq-1.0.0.6.tar` & `enhanceezqq-1.0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:12:20.174524 enhanceezqq-1.0.0.6/
--rw-rw-rw-   0        0        0      307 2023-05-10 12:12:20.173524 enhanceezqq-1.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2696 2023-04-16 04:39:07.000000 enhanceezqq-1.0.0.6/akpack.py
--rw-rw-rw-   0        0        0     5179 2023-04-15 07:50:36.000000 enhanceezqq-1.0.0.6/basefund.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:12:20.153520 enhanceezqq-1.0.0.6/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:12:20.163522 enhanceezqq-1.0.0.6/config/enhanceezqq/
--rw-rw-rw-   0        0        0      394 2023-04-15 01:21:04.000000 enhanceezqq-1.0.0.6/config/enhanceezqq/enhanceezqq_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 12:12:20.172524 enhanceezqq-1.0.0.6/enhanceezqq.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-10 12:12:20.000000 enhanceezqq-1.0.0.6/enhanceezqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-10 12:12:20.000000 enhanceezqq-1.0.0.6/enhanceezqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:12:20.000000 enhanceezqq-1.0.0.6/enhanceezqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-10 12:12:20.000000 enhanceezqq-1.0.0.6/enhanceezqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      299 2023-05-10 12:12:20.000000 enhanceezqq-1.0.0.6/enhanceezqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-05-10 12:12:20.000000 enhanceezqq-1.0.0.6/enhanceezqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18905 2023-05-10 12:12:05.000000 enhanceezqq-1.0.0.6/enhanceezqq.py
--rw-rw-rw-   0        0        0       42 2023-05-10 12:12:20.174524 enhanceezqq-1.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     6270 2023-05-10 12:12:05.000000 enhanceezqq-1.0.0.6/setup.py
--rw-rw-rw-   0        0        0     5674 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.6/ths.py
--rw-rw-rw-   0        0        0     5690 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.6/ttjj.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:08:37.795718 enhanceezqq-1.0.0.7/
+-rw-rw-rw-   0        0        0      307 2023-05-10 14:08:37.795718 enhanceezqq-1.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2696 2023-04-16 04:39:07.000000 enhanceezqq-1.0.0.7/akpack.py
+-rw-rw-rw-   0        0        0     5179 2023-04-15 07:50:36.000000 enhanceezqq-1.0.0.7/basefund.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:08:37.774713 enhanceezqq-1.0.0.7/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 14:08:37.784716 enhanceezqq-1.0.0.7/config/enhanceezqq/
+-rw-rw-rw-   0        0        0      394 2023-04-15 01:21:04.000000 enhanceezqq-1.0.0.7/config/enhanceezqq/enhanceezqq_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 14:08:37.793718 enhanceezqq-1.0.0.7/enhanceezqq.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-10 14:08:37.000000 enhanceezqq-1.0.0.7/enhanceezqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-10 14:08:37.000000 enhanceezqq-1.0.0.7/enhanceezqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:08:37.000000 enhanceezqq-1.0.0.7/enhanceezqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-10 14:08:37.000000 enhanceezqq-1.0.0.7/enhanceezqq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      299 2023-05-10 14:08:37.000000 enhanceezqq-1.0.0.7/enhanceezqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-05-10 14:08:37.000000 enhanceezqq-1.0.0.7/enhanceezqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19013 2023-05-10 14:04:14.000000 enhanceezqq-1.0.0.7/enhanceezqq.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 14:08:37.796718 enhanceezqq-1.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     6270 2023-05-10 14:08:09.000000 enhanceezqq-1.0.0.7/setup.py
+-rw-rw-rw-   0        0        0     5674 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.7/ths.py
+-rw-rw-rw-   0        0        0     5690 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.7/ttjj.py
```

### Comparing `enhanceezqq-1.0.0.6/akpack.py` & `enhanceezqq-1.0.0.7/akpack.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.6/basefund.py` & `enhanceezqq-1.0.0.7/basefund.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.6/enhanceezqq.py` & `enhanceezqq-1.0.0.7/enhanceezqq.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,23 +147,23 @@
             # 组合系统配置目录对应文件
             sysfileprocconfig = os.path.join(sys.prefix, fileprocconfig)
             if Path(sysfileprocconfig).is_file() is False:
                 print("本地配置文件：{}及系统原始配置文件{} 均不存在！".format(fileprocconfig, sysfileprocconfig))
                 sys.exit(-1)
             else:
                 # 判断本地配置目录是否存在，如果不存在则创建目录，逐层创建
-                os.makedirs(os.path.dirname(fileprocconfig))
+                localdir = os.path.dirname(fileprocconfig)
+                if Path(localdir).is_dir() is False:
+                    os.makedirs(os.path.dirname(localdir))
                 # 拷贝系统配置文件到本地
                 shutil.copy(sysfileprocconfig, fileprocconfig)
         except Exception as err:
             print("拷贝系统原始配置到本地配置文件：{} 失败：{}".format(fileprocconfig, err))
             sys.exit(-1)
 
-
-
     try:
         with open(STOCK_RESEARCH_CONFIG, "r", encoding="utf-8") as fp:
             configdic = json.load(fp)
             databaseinfo = configdic["database"]
             fp.close()
     except Exception as err:
         print("读取配置文件：{}失败：{}".format(STOCK_RESEARCH_CONFIG, err))
```

### Comparing `enhanceezqq-1.0.0.6/setup.py` & `enhanceezqq-1.0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 00000940: 7269 6769 6e63 6f6e 6669 6764 6972 2c20  riginconfigdir, 
 00000950: 5b6f 7267 696e 636f 6e66 6967 6669 6c65  [orginconfigfile
 00000960: 5d29 2c0d 0a20 2020 2020 2020 205d 0d0a  ]),..        ]..
 00000970: 2020 2020 7265 7475 726e 2064 6174 615f      return data_
 00000980: 6669 6c65 730d 0a0d 0a0d 0a73 6574 7570  files......setup
 00000990: 280d 0a20 2020 206e 616d 653d 2765 6e68  (..    name='enh
 000009a0: 616e 6365 657a 7171 272c 0d0a 2020 2020  anceezqq',..    
-000009b0: 7665 7273 696f 6e3d 2731 2e30 2e30 2e36  version='1.0.0.6
+000009b0: 7665 7273 696f 6e3d 2731 2e30 2e30 2e37  version='1.0.0.7
 000009c0: 272c 0d0a 2020 2020 6465 7363 7269 7074  ',..    descript
 000009d0: 696f 6e3d 27e7 94a8 e4ba 8ee5 afb9 657a  ion='.........ez
 000009e0: 7171 e6a8 a1e5 9d97 e5a2 9ee5 bcba e58a  qq..............
 000009f0: 9fe8 83bd efbc 8ce8 83bd e5a4 9fe8 8eb7  ................
 00000a00: e58f 96e5 8e86 e58f b2e6 95b0 e68d aee4  ................
 00000a10: bf9d e5ad 98e5 88b0 e695 b0e6 8dae e5ba  ................
 00000a20: 93ef bc8c e5b9 b6e4 bb8e e695 b0e6 8dae  ................
```

### Comparing `enhanceezqq-1.0.0.6/ths.py` & `enhanceezqq-1.0.0.7/ths.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.6/ttjj.py` & `enhanceezqq-1.0.0.7/ttjj.py`

 * *Files identical despite different names*

