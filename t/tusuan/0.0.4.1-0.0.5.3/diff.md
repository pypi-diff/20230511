# Comparing `tmp/tusuan-0.0.4.1.tar.gz` & `tmp/tusuan-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tusuan-0.0.4.1.tar", last modified: Tue Apr 25 16:51:10 2023, max compression
+gzip compressed data, was "tusuan-0.0.5.3.tar", last modified: Mon May  8 18:14:27 2023, max compression
```

## Comparing `tusuan-0.0.4.1.tar` & `tusuan-0.0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.759826 tusuan-0.0.4.1/
--rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.4.1/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-04-25 16:51:10.759698 tusuan-0.0.4.1/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.4.1/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-04-25 16:51:10.759870 tusuan-0.0.4.1/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1634 2023-04-25 16:50:57.000000 tusuan-0.0.4.1/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.758425 tusuan-0.0.4.1/tusuan/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.4.1/tusuan/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.4.1/tusuan/file_function.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.4.1/tusuan/hello.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.759539 tusuan-0.0.4.1/tusuan/image_video_utils/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.4.1/tusuan/image_video_utils/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2132 2023-04-21 16:34:53.000000 tusuan-0.0.4.1/tusuan/image_video_utils/cropper.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      819 2023-03-29 17:22:55.000000 tusuan-0.0.4.1/tusuan/image_video_utils/display.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.4.1/tusuan/image_video_utils/image_visual_selector.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     3591 2023-04-25 16:48:57.000000 tusuan-0.0.4.1/tusuan/image_video_utils/readers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2213 2023-04-25 16:49:11.000000 tusuan-0.0.4.1/tusuan/image_video_utils/writers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.4.1/tusuan/path_utils.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.758903 tusuan-0.0.4.1/tusuan.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      507 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.744439 tusuan-0.0.5.3/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.5.3/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-08 18:14:27.744319 tusuan-0.0.5.3/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.5.3/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)       84 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-05-08 18:14:27.744480 tusuan-0.0.5.3/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1648 2023-05-08 18:14:20.000000 tusuan-0.0.5.3/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.743037 tusuan-0.0.5.3/tusuan/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.5.3/tusuan/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.5.3/tusuan/file_function.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.5.3/tusuan/hello.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.744153 tusuan-0.0.5.3/tusuan/image_video_utils/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.5.3/tusuan/image_video_utils/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2137 2023-05-08 05:08:27.000000 tusuan-0.0.5.3/tusuan/image_video_utils/croppers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1163 2023-05-07 17:43:48.000000 tusuan-0.0.5.3/tusuan/image_video_utils/display.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.5.3/tusuan/image_video_utils/image_visual_selector.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     4013 2023-05-08 05:14:00.000000 tusuan-0.0.5.3/tusuan/image_video_utils/readers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2583 2023-05-08 18:11:39.000000 tusuan-0.0.5.3/tusuan/image_video_utils/writers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.5.3/tusuan/path_utils.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.743489 tusuan-0.0.5.3/tusuan.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      508 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       84 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/top_level.txt
```

### Comparing `tusuan-0.0.4.1/PKG-INFO` & `tusuan-0.0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.4.1
+Version: 0.0.5.3
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.4.1/setup.py` & `tusuan-0.0.5.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from read import read
 from setuptools import setup, find_packages
 
 setup(name='tusuan',  # 包名
       python_requires='>=3.8.0',  # python环境
-      version='0.0.4.1',  # 包的版本
+      version='0.0.5.3',  # 包的版本
       description="useful functions.",  # 包简介，显示在PyPI上
 
       long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
       long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
       author="tusuan",  # 作者相关信息
       author_email='btk@qq.com',
@@ -28,14 +28,15 @@
           'Natural Language :: English',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10'
       ])
 
 """
+rm -rf ./dist
 pipreqs ./ --encoding=utf8 --force --mode no-pin
 python3 setup.py sdist 
 twine upload --repository tusuan@testpypi dist/*
 pip install -i https://test.pypi.org/simple/ -U tusuan
 
 twine upload --repository tusuan@pypi dist/*
 """
```

### Comparing `tusuan-0.0.4.1/tusuan/file_function.py` & `tusuan-0.0.5.3/tusuan/file_function.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.4.1/tusuan/image_video_utils/cropper.py` & `tusuan-0.0.5.3/tusuan/image_video_utils/croppers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy
 
 
 def crop_image(image: numpy.ndarray,
                x1: int, y1: int, x2: int, y2: int,
                h_axis: int = 0, w_axis: int = 1) -> numpy.ndarray:
     """
-    可对任意维度的图像进行截取，返回截取后的数组。
+    可对图像(h w [c])进行截取，返回截取后的数组。
     :param image: numpy.array, 输入图像或视频的帧。
     :param x1: int, 左上角 x 坐标。
     :param y1: int, 左上角 y 坐标。
     :param x2: int, 右下角 x 坐标。
     :param y2: int, 右下角 y 坐标。
     :param h_axis: int, 数组中表示高度（height）的轴。
     :param w_axis: int, 数组中表示宽度（width）的轴。
@@ -34,15 +34,15 @@
 
     return cropped_image
 
 
 def crop_video(video: numpy.ndarray, x1: int, y1: int, x2: int, y2: int, h_axis: int = 1,
                w_axis: int = 2) -> numpy.ndarray:
     """
-    对视频中的每一帧进行截取，返回截取后的视频。
+    对视频(f h w [c])中的每一帧进行截取，返回截取后的视频。
     实际上是将视频看成一个多维图像，直接采用`crop_image`函数对多维图像进行切割。
 
     :param video: numpy.array, 输入视频。
     :param x1: int, 左上角 x 坐标。
     :param y1: int, 左上角 y 坐标。
     :param x2: int, 右下角 x 坐标。
     :param y2: int, 右下角 y 坐标。
```

### Comparing `tusuan-0.0.4.1/tusuan/image_video_utils/image_visual_selector.py` & `tusuan-0.0.5.3/tusuan/image_video_utils/image_visual_selector.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.4.1/tusuan/image_video_utils/readers.py` & `tusuan-0.0.5.3/tusuan/image_video_utils/readers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-import sys
-
 import cv2
+import imagesize
 import numpy
-from PIL import Image
 
 
-def get_image_info(image_path):
+def get_image_size(image_path):
     """
-    要获取图像的尺寸，最快的方式是使用Pillow库中的Image类，而不是使用OpenCV。
-
     :param image_path: 图像路径
-    :return:  width, height
+    :return: height, width
     """
-    with Image.open(image_path) as img:
+
+    width, height = imagesize.get(image_path)
+
+    if (height, width) == (-1, -1):
+        image: numpy.ndarray = cv2.imread(image_path, cv2.IMREAD_GRAYSCALE)
         # 获取图像尺寸
-        width, height = img.size
+        height, width = image.shape
 
     return height, width
 
 
-def read_image(image_path, grey: bool = False, resize=None, to_rgb: bool = False):
+def read_image(image_path, grey: bool = False, resize=None, rgb_mode: bool = True):
     """
     读取图像函数
 
     :param image_path: 图像路径
     :param grey: 是否将图像转换为灰度图像，默认为False
     :param resize: (h, w)，默认为None
-    :param to_rgb: 是否将图像转换为RGB格式，默认为True
+    :param rgb_mode: 使用opencv读出的图像是BGR格式，是否将图像转换为RGB格式，默认为True
     :return: 读取到的图像数组
     """
+
     if grey:
         # 读取灰度图像
         image = cv2.imread(image_path, cv2.IMREAD_GRAYSCALE)
     else:
         # 读取彩色图像
         image = cv2.imread(image_path)
-        if to_rgb:
+        if rgb_mode:
             # 将BGR格式转换为RGB格式
             image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+
     if resize:
         image = cv2.resize(image, resize)
+
     return image
 
 
 def get_video_info(video_path):
     """
     获取帧速率、帧数、宽度和高度
     :param video_path: 视频文件地址
     :return: 帧数、宽度、高度和帧速率。如果视频文件无法打开，则返回None。
     """
+
     # 打开视频文件
     cap = cv2.VideoCapture(video_path)
 
     # 检查视频文件是否成功打开
     if not cap.isOpened():
         return None
 
@@ -65,51 +69,69 @@
     # 释放VideoCapture对象
     cap.release()
 
     # 返回帧数、宽度、高度和帧速率
     return frames_count, fps, height, width
 
 
-def read_video(video_path, stop: int = sys.maxsize, step: int = 1, *, resize=None, to_rgb=False):
+def read_video(video_path, *, start: int = 0, stop: int = -1, step: int = 1, resize=None, rgb_mode=True):
     """
     这个函数可以读取视频文件，并返回指定范围内的帧。
 
     :param video_path: 视频文件路径
-    :param start: 要读取的起始帧索引（默认为 0）
-    :param stop: 要读取的结束帧索引（默认为 sys.maxsize，即读取所有帧）
+    :param start: 要读取的起始帧索引，负数代表倒数（默认为 0）
+    :param stop: 要读取的结束帧索引，负数代表倒数（默认为 -1，即读取到最后一帧）
     :param step: 读取帧的步长（默认为 1）
     :param resize: (h, w)，默认为None
-    :param to_rgb: 是否转化为RGB图像（默认为 False，保持和cv2返回结果一致）
-    :return: 读取成功返回一个代表对应帧所组成的numpy数组，读取失败返回None
+    :param rgb_mode: 是否转化为RGB图像（默认为 True）
+    :return: 读取成功返回一个代表对应帧所组成的numpy数组(h w c)，读取失败返回None
     """
+
     cap = cv2.VideoCapture(video_path)
 
     if not cap.isOpened():
         return None
 
     # 结束帧数不应超过总帧数
     frames_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    stop = min(frames_count, stop)
 
-    # cap_iter = iter(lambda: cap.read(), null)
+    start = start % frames_count
+    stop = stop % frames_count
+
+    reverse_flag = False
+    if start > stop:
+        start, stop = sorted([start, stop])
+        reverse_flag = not reverse_flag
+
+    if step < 0:
+        step = abs(step)
+        reverse_flag = not reverse_flag
 
+    print(start, stop, step, reverse_flag)
     # 按给定的范围读取视频帧
     # 由于视频不能跳帧读取，所以先读取完整的一段，再筛选其中符合特定步长的帧
     video = []
-    for i in range(stop):
+    for i in range(start):
+        cap.grab()
+
+    for i in range(stop - start + 1):
         # 只选取其中符合特定步长的帧
         if i % step == 0:
             ret, frame = cap.read()
             if ret:
-                if to_rgb:
+                if rgb_mode:
                     frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
                 if resize:
                     frame = cv2.resize(frame, resize)
                 video.append(frame)
         else:
             ret = cap.grab()
 
         if not ret:
             break
 
     cap.release()
+
+    if reverse_flag:
+        video = video[::-1]
+
     return numpy.stack(video, axis=0)
```

### Comparing `tusuan-0.0.4.1/tusuan.egg-info/PKG-INFO` & `tusuan-0.0.5.3/tusuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.4.1
+Version: 0.0.5.3
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

