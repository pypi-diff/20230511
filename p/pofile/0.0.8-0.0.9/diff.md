# Comparing `tmp/pofile-0.0.8.tar.gz` & `tmp/pofile-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pofile-0.0.8.tar", last modified: Sat Apr  1 04:43:29 2023, max compression
+gzip compressed data, was "pofile-0.0.9.tar", last modified: Sat Apr  1 08:31:08 2023, max compression
```

## Comparing `pofile-0.0.8.tar` & `pofile-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.151101 pofile-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofile-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5260 2023-04-01 04:43:29.152103 pofile-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4730 2022-10-28 04:35:32.000000 pofile-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.111085 pofile-0.0.8/pofile/
--rw-rw-rw-   0        0        0       31 2022-09-17 07:55:47.000000 pofile-0.0.8/pofile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.134073 pofile-0.0.8/pofile/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofile-0.0.8/pofile/api/__init__.py
--rw-rw-rw-   0        0        0     4410 2023-04-01 04:43:25.000000 pofile-0.0.8/pofile/api/file.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.140083 pofile-0.0.8/pofile/core/
--rw-rw-rw-   0        0        0     9063 2022-12-01 16:58:03.000000 pofile-0.0.8/pofile/core/FileType.py
--rw-rw-rw-   0        0        0     1288 2022-09-01 13:34:44.000000 pofile-0.0.8/pofile/core/SearchByContentType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofile-0.0.8/pofile/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.141081 pofile-0.0.8/pofile/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofile-0.0.8/pofile/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.146084 pofile-0.0.8/pofile/lib/image/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofile-0.0.8/pofile/lib/image/__init__.py
--rw-rw-rw-   0        0        0     2822 2022-09-01 13:34:44.000000 pofile-0.0.8/pofile/lib/image/add_watermark_service.py
--rw-rw-rw-   0        0        0     2237 2022-09-01 13:34:44.000000 pofile-0.0.8/pofile/lib/image/eliminate_background.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.130073 pofile-0.0.8/pofile.egg-info/
--rw-rw-rw-   0        0        0     5260 2023-04-01 04:43:28.000000 pofile-0.0.8/pofile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-04-01 04:43:28.000000 pofile-0.0.8/pofile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 04:43:28.000000 pofile-0.0.8/pofile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-19 03:17:02.000000 pofile-0.0.8/pofile.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-04-01 04:43:28.000000 pofile-0.0.8/pofile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-01 04:43:28.000000 pofile-0.0.8/pofile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      734 2023-04-01 04:43:29.154086 pofile-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofile-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-01 04:43:29.150087 pofile-0.0.8/tests/
--rw-rw-rw-   0        0        0      182 2022-09-17 07:55:47.000000 pofile-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1256 2023-04-01 04:33:02.000000 pofile-0.0.8/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.549691 pofile-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pofile-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5260 2023-04-01 08:31:08.550679 pofile-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4730 2022-10-28 04:35:32.000000 pofile-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.451961 pofile-0.0.9/pofile/
+-rw-rw-rw-   0        0        0       31 2022-09-17 07:55:47.000000 pofile-0.0.9/pofile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.491004 pofile-0.0.9/pofile/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofile-0.0.9/pofile/api/__init__.py
+-rw-rw-rw-   0        0        0     4481 2023-04-01 08:17:55.000000 pofile-0.0.9/pofile/api/file.py
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.513086 pofile-0.0.9/pofile/core/
+-rw-rw-rw-   0        0        0     9063 2022-12-01 16:58:03.000000 pofile-0.0.9/pofile/core/FileType.py
+-rw-rw-rw-   0        0        0     1288 2022-09-01 13:34:44.000000 pofile-0.0.9/pofile/core/SearchByContentType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofile-0.0.9/pofile/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.515086 pofile-0.0.9/pofile/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pofile-0.0.9/pofile/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.537147 pofile-0.0.9/pofile/lib/image/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 pofile-0.0.9/pofile/lib/image/__init__.py
+-rw-rw-rw-   0        0        0     2822 2022-09-01 13:34:44.000000 pofile-0.0.9/pofile/lib/image/add_watermark_service.py
+-rw-rw-rw-   0        0        0     2237 2022-09-01 13:34:44.000000 pofile-0.0.9/pofile/lib/image/eliminate_background.py
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.485601 pofile-0.0.9/pofile.egg-info/
+-rw-rw-rw-   0        0        0     5260 2023-04-01 08:31:08.000000 pofile-0.0.9/pofile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-04-01 08:31:08.000000 pofile-0.0.9/pofile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-01 08:31:08.000000 pofile-0.0.9/pofile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-19 03:17:02.000000 pofile-0.0.9/pofile.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-04-01 08:31:08.000000 pofile-0.0.9/pofile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-01 08:31:08.000000 pofile-0.0.9/pofile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      734 2023-04-01 08:31:08.554213 pofile-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pofile-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-01 08:31:08.546683 pofile-0.0.9/tests/
+-rw-rw-rw-   0        0        0      182 2022-09-17 07:55:47.000000 pofile-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1256 2023-04-01 04:33:02.000000 pofile-0.0.9/tests/test_file.py
```

### Comparing `pofile-0.0.8/LICENSE` & `pofile-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pofile-0.0.8/PKG-INFO` & `pofile-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pofile
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install pofile
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pofile/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pofile/blob/master/README.md
```

### Comparing `pofile-0.0.8/README.md` & `pofile-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pofile-0.0.8/pofile/api/file.py` & `pofile-0.0.9/pofile/api/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 
 
 def get_files(path: str, name: str = None, sub: bool = False, level: int = 0) -> list:
     """
         获取指定路径下的所有文件
     :param path: 必填，指定路径
     :param name: 可以不填，名字中包含的内容
-    :param sub: 必填，是否获取子文件夹内容
+    :param sub: 可以不填，是否获取子文件夹内容
+    :param level: 可以不填，获取第几层文件夹的内容
     :return: 装满文件路径的列表
     """
     result_file_path_name_list = []  # 指定路径下，待转换的docx文件。如果是目录，不递归
     abs_input_path = Path(path).absolute()
     # 如果不存在，则不做处理
     if not abs_input_path.exists():
         print("path does not exist path = " + path)
@@ -105,12 +106,12 @@
         result_file_path_name_list.append(str(path))
     # 如果是目录，则遍历目录下面的文件
     elif abs_input_path.is_dir():
         for dirpath, dirnames, filenames in simple_progress(os.walk(str(abs_input_path))):
             for filename in filenames:
                 if not name:
                     result_file_path_name_list.append(os.path.join(dirpath, filename))
-                elif filename.find(name):
+                elif name in filename:
                     result_file_path_name_list.append(os.path.join(dirpath, filename))
 
     print(f'一共有{len(result_file_path_name_list)}个文件')
     return result_file_path_name_list
```

### Comparing `pofile-0.0.8/pofile/core/FileType.py` & `pofile-0.0.9/pofile/core/FileType.py`

 * *Files identical despite different names*

### Comparing `pofile-0.0.8/pofile/core/SearchByContentType.py` & `pofile-0.0.9/pofile/core/SearchByContentType.py`

 * *Files identical despite different names*

### Comparing `pofile-0.0.8/pofile/lib/image/add_watermark_service.py` & `pofile-0.0.9/pofile/lib/image/add_watermark_service.py`

 * *Files identical despite different names*

### Comparing `pofile-0.0.8/pofile/lib/image/eliminate_background.py` & `pofile-0.0.9/pofile/lib/image/eliminate_background.py`

 * *Files identical despite different names*

### Comparing `pofile-0.0.8/pofile.egg-info/PKG-INFO` & `pofile-0.0.9/pofile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pofile
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install pofile
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pofile/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pofile/blob/master/README.md
```

### Comparing `pofile-0.0.8/pofile.egg-info/SOURCES.txt` & `pofile-0.0.9/pofile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pofile-0.0.8/setup.cfg` & `pofile-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f66 696c 650d 0a76 6572 7369   = pofile..versi
-00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6465 7363  on = 0.0.8..desc
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6465 7363  on = 0.0.9..desc
 00000030: 7269 7074 696f 6e20 3d20 7069 7020 696e  ription = pip in
 00000040: 7374 616c 6c20 706f 6669 6c65 0d0a 6c6f  stall pofile..lo
 00000050: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
 00000060: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
 00000070: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000080: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
 00000090: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
```

### Comparing `pofile-0.0.8/tests/test_file.py` & `pofile-0.0.9/tests/test_file.py`

 * *Files identical despite different names*

