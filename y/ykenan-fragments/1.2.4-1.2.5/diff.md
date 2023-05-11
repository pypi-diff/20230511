# Comparing `tmp/ykenan_fragments-1.2.4.tar.gz` & `tmp/ykenan_fragments-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.2.4.tar", last modified: Wed May 10 13:09:49 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.2.5.tar", last modified: Thu May 11 02:32:09 2023, max compression
```

## Comparing `ykenan_fragments-1.2.4.tar` & `ykenan_fragments-1.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:09:49.507116 ykenan_fragments-1.2.4/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.4/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      971 2023-05-10 13:09:49.506117 ykenan_fragments-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.4/README.md
--rw-rw-rw-   0        0        0      773 2023-05-10 13:08:57.000000 ykenan_fragments-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 13:09:49.507116 ykenan_fragments-1.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 13:09:49.469086 ykenan_fragments-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:09:49.491086 ykenan_fragments-1.2.4/src/ykenan_fragments/
--rw-rw-rw-   0        0        0     2012 2023-05-10 13:00:59.000000 ykenan_fragments-1.2.4/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     3327 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.4/src/ykenan_fragments/genome_transformation.py
--rw-rw-rw-   0        0        0    16945 2023-05-10 12:49:55.000000 ykenan_fragments-1.2.4/src/ykenan_fragments/get_fragments.py
--rw-rw-rw-   0        0        0    15330 2023-05-10 12:28:25.000000 ykenan_fragments-1.2.4/src/ykenan_fragments/get_sort_fragments.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:09:49.505118 ykenan_fragments-1.2.4/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      971 2023-05-10 13:09:49.000000 ykenan_fragments-1.2.4/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-10 13:09:49.000000 ykenan_fragments-1.2.4/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:09:49.000000 ykenan_fragments-1.2.4/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 13:09:49.000000 ykenan_fragments-1.2.4/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-10 13:09:49.000000 ykenan_fragments-1.2.4/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 02:32:09.078816 ykenan_fragments-1.2.5/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      971 2023-05-11 02:32:09.078816 ykenan_fragments-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.5/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-11 01:37:58.000000 ykenan_fragments-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-05-11 01:21:49.000000 ykenan_fragments-1.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 02:32:09.078816 ykenan_fragments-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-11 02:32:08.832786 ykenan_fragments-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 02:32:09.007817 ykenan_fragments-1.2.5/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0     2012 2023-05-10 13:00:59.000000 ykenan_fragments-1.2.5/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     3148 2023-05-11 01:36:08.000000 ykenan_fragments-1.2.5/src/ykenan_fragments/genome_transformation.py
+-rw-rw-rw-   0        0        0    15901 2023-05-11 01:33:09.000000 ykenan_fragments-1.2.5/src/ykenan_fragments/get_fragments.py
+-rw-rw-rw-   0        0        0    14911 2023-05-11 01:35:21.000000 ykenan_fragments-1.2.5/src/ykenan_fragments/get_sort_fragments.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:32:09.077788 ykenan_fragments-1.2.5/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      971 2023-05-11 02:32:08.000000 ykenan_fragments-1.2.5/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-11 02:32:08.000000 ykenan_fragments-1.2.5/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 02:32:08.000000 ykenan_fragments-1.2.5/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-11 02:32:08.000000 ykenan_fragments-1.2.5/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-11 02:32:08.000000 ykenan_fragments-1.2.5/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.2.4/LICENSE` & `ykenan_fragments-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.4/PKG-INFO` & `ykenan_fragments-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.2.4
+Version: 1.2.5
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.2.4/pyproject.toml` & `ykenan_fragments-1.2.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
+requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.9", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
-dependencies = ["ykenan-log>=0.2.0", "ykenan-file>=0.1.7", "pandas>=1.5.3"]
+dependencies = ["ykenan-log>=0.2.0", "ykenan-file>=0.1.9", "pandas>=1.5.3"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 github = "https://github.com/YuZhengM/ykenan_fragments"
```

### Comparing `ykenan_fragments-1.2.4/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.2.5/src/ykenan_fragments/__init__.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.4/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.2.5/src/ykenan_fragments/genome_transformation.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,20 +54,17 @@
 
     def run(self):
 
         if not os.path.exists(self.source):
             self.log.error(f"输入文件夹 {self.source} 不存在")
             raise ValueError(f"输入文件夹 {self.source} 不存在")
 
-        if not os.path.exists(self.output):
-            self.log.info(f"创建 {self.output} 文件夹")
-            os.makedirs(self.output)
-        if not os.path.exists(self.unmap):
-            self.log.info(f"创建 {self.unmap} 文件夹")
-            os.makedirs(self.unmap)
+        # 创建文件夹
+        self.file.makedirs(self.output)
+        self.file.makedirs(self.unmap)
 
         # 获取没有执行的文件
         input_files = self.file.get_files(path=self.source)
         code_list = []
         finish_files = self.file.get_files(path=self.output)
         for input_file in input_files:
             if input_file not in finish_files:
```

### Comparing `ykenan_fragments-1.2.4/src/ykenan_fragments/get_fragments.py` & `ykenan_fragments-1.2.5/src/ykenan_fragments/get_fragments.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
 import os
-import shutil
 from multiprocessing.pool import ThreadPool
 
 from ykenan_log import Logger
 import ykenan_file as yf
 import gzip
 from multiprocessing.dummy import Pool
 
@@ -71,25 +70,25 @@
             for gz_file_before in gz_files_before:
                 gz_file_before_dir = os.path.join(self.base_path, gz_file_before)
                 gz_file_before_dirs.update({gz_file_before: gz_file_before_dir})
                 # Determine whether the folder is created
                 if os.path.exists(gz_file_before_dir):
                     continue
                 self.log.info(f"create folder {gz_file_before_dir}")
-                os.mkdir(gz_file_before_dir)
+                self.file.makedirs(gz_file_before_dir)
 
             # move file
             for gz_file in gz_files:
                 file_source = os.path.join(self.base_path, gz_file)
                 file_target = gz_file_before_dirs[gz_files_and_before[gz_file]]
-                self.log.info(f"move file {file_source} to {file_target}")
-                shutil.move(file_source, file_target)
+                # 复制文件
+                self.file.copy_file(file_source, file_target)
 
         # Get folder information
-        self.log.info(f"Starting to obtain information for processing ==========> ")
+        self.log.info(f"Starting to obtain information for processing ==========> {self.base_path} path")
         dirs_dict: dict = self.file.entry_dirs_dict(self.base_path)
         dirs_name = dirs_dict["name"]
 
         dirs_key: list = []
         dirs_key_dict: dict = {}
 
         # Determine if the folder contains three files
@@ -124,15 +123,15 @@
                 "key": dirs_key,
                 "path": dirs_key_dict
             }
         }
 
     def get_files(self, path: str) -> dict:
         # Obtain all file information under this path
-        contents_dict: dict = self.file.entry_contents_dict(path, 1)
+        contents_dict: dict = self.file.entry_files_dict(path)
         filenames: list = contents_dict["name"]
         barcodes_file: dict = {}
         mtx_file: dict = {}
         peaks_file: dict = {}
         # pick up information
         self.log.info(f"Obtain three file information for {path}")
         for filename in filenames:
@@ -159,43 +158,27 @@
                     self.log.info(f"{self.peaks_key} file: {peaks_file}")
         return {
             self.barcodes_key: barcodes_file,
             self.mtx_key: mtx_file,
             self.peaks_key: peaks_file
         }
 
-    @staticmethod
-    def get_file_content(path: str, file: dict):
+    def get_file_content(self, path: str, file: dict):
         txt_file: str = os.path.join(path, file["name"].split(".txt")[0]) + ".txt"
         # Determine if the file exists
         if txt_file.endswith(".mtx.gz.txt"):
             if not os.path.exists(txt_file):
                 with open(txt_file, 'wb') as w:
                     with gzip.open(file["path"], 'rb') as f:
                         # Form a file
                         w.write(f.read())
             return txt_file
         else:
-            if os.path.exists(txt_file):
-                f = gzip.open(file["path"], 'rb')
-                # Obtaining Content Information
-                file_content: list = f.read().decode().rstrip().split("\n")
-                f.close()
-                return file_content
-            else:
-                w = open(txt_file, 'wb')
-                f = gzip.open(file["path"], 'rb')
-                read = f.read()
-                # Form a file
-                w.write(read)
-                # Obtaining Content Information
-                file_content: list = read.decode().rstrip().split("\n")
-                f.close()
-                w.close()
-                return file_content
+            # 解压文件得到内容
+            return self.file.unzip_gz(file["path"], generate_file=txt_file)
 
     def fragments_file_name(self, key: str) -> str:
         return f"{key}{self.suffix_fragments}"
 
     @staticmethod
     def judge_mtx_is_true(one_len: str, two_len: str, peaks_len: int, barcodes_len: int) -> bool:
         return int(one_len) + 1 != peaks_len and int(two_len) + 1 != barcodes_len
@@ -297,45 +280,34 @@
                         self.log.error(f"mtx information ===> content: {split}, line number: {mtx_count}")
                         self.log.error(f"Write error: {e}")
                     mtx_count += 1
         self.log.info(f"The number of rows ignored is {error_count}, {round(error_count / mtx_all_number, 4) * 100} % of total")
         self.log.info(f"Complete the formation of {mtx_path} fragments file")
         self.log.info(f"Complete processing of {key} related files (folders)")
 
-    def copy_file(self, source_file: str, target_file: str) -> None:
-        if os.path.exists(target_file):
-            self.log.warn(f"{target_file} The file already exists, it has been copied by default")
-        else:
-            self.log.info(f"Start copying file {source_file}")
-            shutil.copy(source_file, target_file)
-            self.log.info(f"End of copying file  {source_file}")
-
     def cp_files(self, param: tuple) -> None:
         path: str = param[0]
         key: str = param[1]
         self.log.info(f"Start copying files to the specified path for {key}")
         fragments_file_name = self.fragments_file_name(key)
         fragments_file: str = os.path.join(path, fragments_file_name)
         # Determine if it exists
         if not (os.path.exists(fragments_file)):
             self.log.error(f"file does not exist: {fragments_file}")
             raise ValueError(f"file does not exist: {fragments_file}")
         # Two folders
         fragments_cp_dir = os.path.join(self.cp_path, "fragments")
-        if not os.path.exists(fragments_cp_dir):
-            self.log.info(f"create folder {fragments_cp_dir}")
-            os.makedirs(fragments_cp_dir)
         # copy
         fragments_gz_file = os.path.join(fragments_cp_dir, f"{fragments_file_name}.gz")
         if os.path.exists(fragments_gz_file):
             self.log.warn(f"The file has been compressed into {fragments_gz_file}, Default copy completed")
         elif os.path.exists(os.path.join(fragments_cp_dir, fragments_file_name)):
             self.log.warn(f"The file has been copy into {fragments_gz_file}, Default copy completed")
         else:
-            self.copy_file(fragments_file, os.path.join(fragments_cp_dir, fragments_file_name))
+            self.file.copy_file(fragments_file, os.path.join(fragments_cp_dir, fragments_file_name))
         self.log.info(f"Copy file to specified path for {key} completed")
 
     def exec_fragments(self):
         # Classify the types and place them in different folders
         source_files: dict = self.handler_source_files()
         no_finish_infor = source_files["no_finish"]
         no_finish_keys = no_finish_infor["key"]
@@ -347,14 +319,18 @@
             write_fragments_param_list.append((no_finish_paths[key], key))
         # 实例化线程对象
         pool: ThreadPool = Pool(self.thread_count)
         # Form fragments file
         pool.map(self.write_fragments, write_fragments_param_list)
         pool.close()
 
+        # create folders
+        fragments_cp_dir = os.path.join(self.cp_path, "fragments")
+        self.file.makedirs(fragments_cp_dir)
+
         # All information
         all_infor = source_files["all"]
         all_infor_keys = all_infor["key"]
         all_infor_paths = all_infor["path"]
         # 参数信息
         cp_files_param_list = []
         for key in all_infor_keys:
```

### Comparing `ykenan_fragments-1.2.4/src/ykenan_fragments/get_sort_fragments.py` & `ykenan_fragments-1.2.5/src/ykenan_fragments/get_sort_fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,26 +55,23 @@
             self.log.error(f"The input file {self.fragments_path} does not exist. Please check")
             raise ValueError(f"The input file {self.fragments_path} does not exist. Please check")
         # Obtain tsv file information under the folder
         files_dict: dict = self.file.entry_contents_dict(self.fragments_path, type_=1, suffix=".tsv")
         files_dict_name = files_dict["name"]
         self.log.info(f"tsv file information: {files_dict_name}")
         need_handler_fragments_result: dict = {}
-        if not os.path.exists(self.merge_input_path):
-            self.log.info(f"create folder {self.merge_input_path}")
-            os.makedirs(self.merge_input_path)
+        # 创建输出文件夹
+        self.file.makedirs(self.merge_input_path)
 
         # Add processing files
         for genome in self.genomes:
 
             # 创建文件夹
             merge_input_path_genome = os.path.join(self.merge_input_path, genome)
-            if not os.path.exists(merge_input_path_genome):
-                self.log.info(f"创建 {merge_input_path_genome} 文件夹")
-                os.makedirs(merge_input_path_genome)
+            self.file.makedirs(merge_input_path_genome)
 
             need_handler_fragments: list = []
             need_handler_fragments_path: dict = {}
             for file in files_dict_name:
                 # 排序后的文件
                 archr_fragments_file: str = os.path.join(merge_input_path_genome, file)
                 if os.path.exists(archr_fragments_file):
@@ -282,20 +279,16 @@
         for genome in self.genomes:
 
             # 判断是否继续
             if not self.lift_over_path and genome == self.genome_generate:
                 continue
             files_name: list = files_dict[genome]["name"]
             files_path: dict = files_dict[genome]["path"]
-
             # 创建文件夹
             merge_input_path_genome = os.path.join(self.merge_input_path, genome)
-            if not os.path.exists(merge_input_path_genome):
-                self.log.info(f"create {merge_input_path_genome} 文件夹")
-                os.makedirs(merge_input_path_genome)
 
             param_list: list = []
             for file in files_name:
                 # output file
                 chr_sort_fragments_file: str = os.path.join(merge_input_path_genome, file)
 
                 if os.path.exists(chr_sort_fragments_file):
```

### Comparing `ykenan_fragments-1.2.4/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.2.5/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.2.4
+Version: 1.2.5
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

