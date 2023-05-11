# Comparing `tmp/ccdt-2.0.8.tar.gz` & `tmp/ccdt-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.0.8.tar", last modified: Tue May  9 07:32:24 2023, max compression
+gzip compressed data, was "ccdt-2.0.9.tar", last modified: Tue May  9 08:14:29 2023, max compression
```

## Comparing `ccdt-2.0.8.tar` & `ccdt-2.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.550187 ccdt-2.0.8/
--rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     4319 2023-05-09 07:32:24.548185 ccdt-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.466393 ccdt-2.0.8/ccdt/
--rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.8/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.493321 ccdt-2.0.8/ccdt/dataset/
--rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.8/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.500302 ccdt-2.0.8/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.8/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.8/ccdt/dataset/base_coco/coco.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.514265 ccdt-2.0.8/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.8/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.8/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    63679 2023-05-09 06:00:55.000000 ccdt-2.0.8/ccdt/dataset/base_labelme/base_labelme.py
--rw-rw-rw-   0        0        0      471 2023-05-08 06:44:57.000000 ccdt-2.0.8/ccdt/dataset/base_labelme/test_async_io.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.517256 ccdt-2.0.8/ccdt/dataset/logs/
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.8/ccdt/dataset/logs/__init__.py
--rw-rw-rw-   0        0        0    12305 2023-05-09 05:41:22.000000 ccdt-2.0.8/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.534211 ccdt-2.0.8/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      251 2023-05-09 03:47:20.000000 ccdt-2.0.8/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      894 2023-05-09 03:47:20.000000 ccdt-2.0.8/ccdt/dataset/utils/async_dirIterator.py
--rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.8/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    17244 2023-05-09 03:37:25.000000 ccdt-2.0.8/ccdt/dataset/utils/labelme_load.py
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.8/ccdt/dataset/utils/logs.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.544184 ccdt-2.0.8/ccdt/video_tool/
--rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.8/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.8/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.8/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:32:24.486375 ccdt-2.0.8/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4319 2023-05-09 07:32:24.000000 ccdt-2.0.8/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-05-09 07:32:24.000000 ccdt-2.0.8/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 07:32:24.000000 ccdt-2.0.8/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-09 07:32:24.000000 ccdt-2.0.8/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-05-09 07:32:24.000000 ccdt-2.0.8/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-09 07:32:24.000000 ccdt-2.0.8/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 07:32:24.551185 ccdt-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2278 2023-05-09 07:31:48.000000 ccdt-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.982794 ccdt-2.0.9/
+-rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4319 2023-05-09 08:14:29.980797 ccdt-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.909988 ccdt-2.0.9/ccdt/
+-rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.9/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.932927 ccdt-2.0.9/ccdt/dataset/
+-rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.9/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.939908 ccdt-2.0.9/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.9/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.9/ccdt/dataset/base_coco/coco.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.951875 ccdt-2.0.9/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    63485 2023-05-09 08:13:56.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/base_labelme.py
+-rw-rw-rw-   0        0        0      471 2023-05-08 06:44:57.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/test_async_io.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.954867 ccdt-2.0.9/ccdt/dataset/logs/
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.9/ccdt/dataset/logs/__init__.py
+-rw-rw-rw-   0        0        0    12305 2023-05-09 07:48:32.000000 ccdt-2.0.9/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.968829 ccdt-2.0.9/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      251 2023-05-09 03:47:20.000000 ccdt-2.0.9/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      894 2023-05-09 03:47:20.000000 ccdt-2.0.9/ccdt/dataset/utils/async_dirIterator.py
+-rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.9/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    17244 2023-05-09 03:37:25.000000 ccdt-2.0.9/ccdt/dataset/utils/labelme_load.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.9/ccdt/dataset/utils/logs.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.977805 ccdt-2.0.9/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.9/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.9/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.9/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.927938 ccdt-2.0.9/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4319 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 08:14:29.983789 ccdt-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2278 2023-05-09 08:13:56.000000 ccdt-2.0.9/setup.py
```

### Comparing `ccdt-2.0.8/LICENSE` & `ccdt-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/PKG-INFO` & `ccdt-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.8
+Version: 2.0.9
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.8/README.md` & `ccdt-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt/dataset/base_coco/coco.py` & `ccdt-2.0.9/ccdt/dataset/base_coco/coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.0.9/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.0.9/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,31 +189,29 @@
         num_tb = pt.PrettyTable(['num_images', 'num_labelme', 'num_background', 'num_shapes'])
         label_value = []
         print_data = list()
         title = ''
         print(f'筛选及重组满足打印条件的labelme数据集')
         for data_info in tqdm(self.datasets):
             title = data_info.get('input_dir')
-            if data_info.get('image_file') and data_info.get('labelme_info') is None:
-                num_background += 1
-            if data_info.get('image_file'):
-                num_images += 1
+            num_images += 1
             if data_info.get('image_file') and data_info.get('labelme_info'):
                 num_labelme += 1
-                # if not data_info.get('labelme_info').get('shapes'):
-                if data_info.get('background') is False:
-                    for shape in data_info.get('labelme_info').get('shapes'):
-                        num_shapes += 1
-                        if shape.get('label') not in label_value:
-                            rebuild_shape = {}
-                            label_value.append(shape.get('label'))
-                            rebuild_shape.update({'label': shape.get('label')})
-                            rebuild_shape.update({'shape_type': shape.get('shape_type')})
-                            rebuild_shape.update({'flags': shape.get('flags')})
-                            print_data.append(rebuild_shape)
+            if data_info.get('background') is True:
+                num_background += 1
+            if data_info.get('background') is False:
+                for shape in data_info.get('labelme_info').get('shapes'):
+                    num_shapes += 1
+                    if shape.get('label') not in label_value:
+                        rebuild_shape = {}
+                        label_value.append(shape.get('label'))
+                        rebuild_shape.update({'label': shape.get('label')})
+                        rebuild_shape.update({'shape_type': shape.get('shape_type')})
+                        rebuild_shape.update({'flags': shape.get('flags')})
+                        print_data.append(rebuild_shape)
         num_tb.add_row([num_images, num_labelme, num_background, num_shapes])
         # print(f'打印满足重组条件的labelme数据集')
         for data in print_data:
             property_tb.add_row([data.get('label'), data.get('shape_type'), data.get('flags')])
         # print(property_tb)
         # print(num_tb)
         print(num_tb.get_string(title=title))
```

### Comparing `ccdt-2.0.8/ccdt/dataset/main.py` & `ccdt-2.0.9/ccdt/dataset/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,16 +120,16 @@
     if args.function == 'compress':  # 对抽取数据集进行压缩。数据压缩无需对数据进行封装后操作
         zip_package = data_info.compress_labelme()  # 封装压缩路径及压缩对象
         data_info.make_compress(zip_package)  # 开始压缩
     else:
         import time
         async_time = time.time()
         data_info = LabelmeLoad(args)  # 初始化输入参数
-        dataset_info = data_info.get_multiprocess_dir_currency()  # 多进程封装数据处理
-        # dataset_info = data_info.get_dir_currency()  # 单进程封装数据处理
+        # dataset_info = data_info.get_multiprocess_dir_currency()  # 多进程封装数据处理
+        dataset_info = data_info.get_dir_currency()  # 单进程封装数据处理
         print('异步耗时')
         print(time.time() - async_time)
         dataset = BaseLabelme(dataset_info)  # 初始化labelme基类
         if args.function == 'merge':  # 合并功能
             dataset.merge_labelme(args)
             # BaseLabelme.merge(datasets)
         elif args.function == 'matting':  # 抠出标注位置保存labelme
```

### Comparing `ccdt-2.0.8/ccdt/dataset/utils/async_dirIterator.py` & `ccdt-2.0.9/ccdt/dataset/utils/async_dirIterator.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt/dataset/utils/encoder.py` & `ccdt-2.0.9/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.0.9/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt/video_tool/split.py` & `ccdt-2.0.9/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt/video_tool/video_main.py` & `ccdt-2.0.9/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/ccdt.egg-info/PKG-INFO` & `ccdt-2.0.9/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.8
+Version: 2.0.9
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.8/ccdt.egg-info/SOURCES.txt` & `ccdt-2.0.9/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.8/setup.py` & `ccdt-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.0.8',
+    version='2.0.9',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

