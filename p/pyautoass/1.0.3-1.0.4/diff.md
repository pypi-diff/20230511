# Comparing `tmp/pyautoass-1.0.3.tar.gz` & `tmp/pyautoass-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautoass-1.0.3.tar", last modified: Tue May  9 08:38:02 2023, max compression
+gzip compressed data, was "pyautoass-1.0.4.tar", last modified: Thu May 11 07:51:24 2023, max compression
```

## Comparing `pyautoass-1.0.3.tar` & `pyautoass-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:38:02.083229 pyautoass-1.0.3/
--rw-rw-rw-   0        0        0      161 2023-05-09 08:38:02.082230 pyautoass-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 08:38:02.058149 pyautoass-1.0.3/pyAutoAss/
--rw-rw-rw-   0        0        0       36 2023-05-09 08:28:39.000000 pyautoass-1.0.3/pyAutoAss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:38:02.060346 pyautoass-1.0.3/pyAutoAss/dependent/
--rw-rw-rw-   0        0        0     2217 2023-05-09 02:29:05.000000 pyautoass-1.0.3/pyAutoAss/dependent/DataType.py
--rw-rw-rw-   0        0        0     1807 2023-05-09 08:34:27.000000 pyautoass-1.0.3/pyAutoAss/pyAutoKeyboard.py
--rw-rw-rw-   0        0        0     4635 2023-05-09 08:37:14.000000 pyautoass-1.0.3/pyAutoAss/pyAutoMouse.py
--rw-rw-rw-   0        0        0     3145 2023-05-09 08:34:50.000000 pyautoass-1.0.3/pyAutoAss/pyautoAss.py
--rw-rw-rw-   0        0        0     1180 2023-05-09 08:34:59.000000 pyautoass-1.0.3/pyAutoAss/pyclipboard.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:38:02.066856 pyautoass-1.0.3/pyAutoAss/utils/
--rw-rw-rw-   0        0        0        0 2023-05-08 08:39:36.000000 pyautoass-1.0.3/pyAutoAss/utils/Hook.py
--rw-rw-rw-   0        0        0     2850 2023-05-09 03:51:11.000000 pyautoass-1.0.3/pyAutoAss/utils/Utils.py
--rw-rw-rw-   0        0        0     4158 2023-05-08 09:14:19.000000 pyautoass-1.0.3/pyAutoAss/utils/VKCODE.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:38:02.079221 pyautoass-1.0.3/pyautoass.egg-info/
--rw-rw-rw-   0        0        0      161 2023-05-09 08:38:01.000000 pyautoass-1.0.3/pyautoass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-05-09 08:38:01.000000 pyautoass-1.0.3/pyautoass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:38:01.000000 pyautoass-1.0.3/pyautoass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-09 08:38:01.000000 pyautoass-1.0.3/pyautoass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-09 08:38:01.000000 pyautoass-1.0.3/pyautoass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-09 07:57:12.000000 pyautoass-1.0.3/pyautoass.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-09 08:38:02.083229 pyautoass-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      528 2023-05-09 08:35:14.000000 pyautoass-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:51:24.981605 pyautoass-1.0.4/
+-rw-rw-rw-   0        0        0      161 2023-05-11 07:51:24.980604 pyautoass-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 07:51:24.962507 pyautoass-1.0.4/pyAutoAss/
+-rw-rw-rw-   0        0        0       36 2023-05-09 08:28:39.000000 pyautoass-1.0.4/pyAutoAss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:51:24.964871 pyautoass-1.0.4/pyAutoAss/dependent/
+-rw-rw-rw-   0        0        0     2217 2023-05-09 02:29:05.000000 pyautoass-1.0.4/pyAutoAss/dependent/DataType.py
+-rw-rw-rw-   0        0        0     1619 2023-05-11 07:35:39.000000 pyautoass-1.0.4/pyAutoAss/pyAutoGui.py
+-rw-rw-rw-   0        0        0     1807 2023-05-09 08:34:27.000000 pyautoass-1.0.4/pyAutoAss/pyAutoKeyboard.py
+-rw-rw-rw-   0        0        0     4635 2023-05-09 08:37:14.000000 pyautoass-1.0.4/pyAutoAss/pyAutoMouse.py
+-rw-rw-rw-   0        0        0     3143 2023-05-11 07:42:17.000000 pyautoass-1.0.4/pyAutoAss/pyautoAss.py
+-rw-rw-rw-   0        0        0     1180 2023-05-09 08:34:59.000000 pyautoass-1.0.4/pyAutoAss/pyclipboard.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:51:24.969606 pyautoass-1.0.4/pyAutoAss/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-08 08:39:36.000000 pyautoass-1.0.4/pyAutoAss/utils/Hook.py
+-rw-rw-rw-   0        0        0     2850 2023-05-09 03:51:11.000000 pyautoass-1.0.4/pyAutoAss/utils/Utils.py
+-rw-rw-rw-   0        0        0     4158 2023-05-08 09:14:19.000000 pyautoass-1.0.4/pyAutoAss/utils/VKCODE.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:51:24.978411 pyautoass-1.0.4/pyautoass.egg-info/
+-rw-rw-rw-   0        0        0      161 2023-05-11 07:51:24.000000 pyautoass-1.0.4/pyautoass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-05-11 07:51:24.000000 pyautoass-1.0.4/pyautoass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 07:51:24.000000 pyautoass-1.0.4/pyautoass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-11 07:51:24.000000 pyautoass-1.0.4/pyautoass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 07:51:24.000000 pyautoass-1.0.4/pyautoass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 07:57:12.000000 pyautoass-1.0.4/pyautoass.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-11 07:51:24.981605 pyautoass-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-05-11 07:42:51.000000 pyautoass-1.0.4/setup.py
```

### Comparing `pyautoass-1.0.3/pyAutoAss/dependent/DataType.py` & `pyautoass-1.0.4/pyAutoAss/dependent/DataType.py`

 * *Files identical despite different names*

### Comparing `pyautoass-1.0.3/pyAutoAss/pyAutoKeyboard.py` & `pyautoass-1.0.4/pyAutoAss/pyAutoKeyboard.py`

 * *Files identical despite different names*

### Comparing `pyautoass-1.0.3/pyAutoAss/pyAutoMouse.py` & `pyautoass-1.0.4/pyAutoAss/pyAutoMouse.py`

 * *Files identical despite different names*

### Comparing `pyautoass-1.0.3/pyAutoAss/pyautoAss.py` & `pyautoass-1.0.4/pyAutoAss/pyautoAss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
     name: pyautoAss
     author: awiseking
-    version: 1.0.3
+    version: 1.0.4
     des: 基于键鼠、图片定位的自动化gui工作套件。
         
 """
-from time import sleep
 import cv2 as cv
 from .utils.Utils import *
 from .pyclipboard import PyClipboard
 from .pyAutoKeyboard import PyAutoKeyboard
 from .pyAutoMouse import PyAutoMouse
-import pyautogui
+from .pyAutoGui import PyAutoGui
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
-class AutoOperation(PyAutoKeyboard,PyAutoMouse):
+class AutoOperation(PyAutoKeyboard,PyAutoMouse,PyAutoGui):
 
     def __init__(self,app_name:str="app") -> None:
         """自动化套件
         初始化自动化套件所需组件，自动进行数据处理等工作。
         :param app_name -- 应用名
 
         :var self.app_name -- 应用名
@@ -46,15 +45,15 @@
     # 获取图片所在坐标
     def getXY(self, img_path:str="./input/pic/template.png"):
         """
         图片中心在屏幕坐标
         :param img_path: 图片路径
         :return avg: 图片中心在屏幕坐标
         """
-        pyautogui.screenshot().save("./input/pic/screenshot.png")
+        self.screenShotSaveFile("./input/pic/screenshot.png")
 
         screenshot_img = cv.imread("./input/pic/screenshot.png")
         template_img = cv.imread(img_path)
 
         # 获取图片宽高
         height, width, channel = template_img.shape
```

### Comparing `pyautoass-1.0.3/pyAutoAss/pyclipboard.py` & `pyautoass-1.0.4/pyAutoAss/pyclipboard.py`

 * *Files identical despite different names*

### Comparing `pyautoass-1.0.3/pyAutoAss/utils/Utils.py` & `pyautoass-1.0.4/pyAutoAss/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `pyautoass-1.0.3/pyAutoAss/utils/VKCODE.py` & `pyautoass-1.0.4/pyAutoAss/utils/VKCODE.py`

 * *Files identical despite different names*

### Comparing `pyautoass-1.0.3/setup.py` & `pyautoass-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 setuptools.setup(
     name='pyautoass',
-    version='1.0.3',
+    version='1.0.4',
     description='基于键鼠、图片定位的自动化gui工作套件。',
     author='awise',
     packages=["pyAutoAss","pyAutoAss.utils","pyAutoAss.dependent"],
     install_requires=['pyautogui','opencv-python',"pywin32"],
     # 指定项目依赖的 Python 版本。
     python_requires='>=3',
     # 是否使用静态文件，为true时静态文件生效，否则不起作用
```

