# Comparing `tmp/gTixi-1.1.1.tar.gz` & `tmp/gTixi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gTixi-1.1.1.tar", last modified: Wed Apr 19 01:59:14 2023, max compression
+gzip compressed data, was "gTixi-1.2.0.tar", last modified: Thu May 11 05:43:31 2023, max compression
```

## Comparing `gTixi-1.1.1.tar` & `gTixi-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.540087 gTixi-1.1.1/
--rw-rw-rw-   0        0        0     1091 2022-12-02 07:39:30.000000 gTixi-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      123 2023-04-19 01:59:01.000000 gTixi-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    30481 2023-04-19 01:59:14.539084 gTixi-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    30047 2023-04-19 01:54:32.000000 gTixi-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.417084 gTixi-1.1.1/gTixi/
--rw-rw-rw-   0        0        0   456248 2023-04-10 07:25:40.000000 gTixi-1.1.1/gTixi/Dianzhen.ttf
--rw-rw-rw-   0        0        0     5570 2023-04-10 02:42:27.000000 gTixi-1.1.1/gTixi/SSD1306.py
--rw-rw-rw-   0        0        0     1116 2023-01-04 05:19:56.000000 gTixi-1.1.1/gTixi/__init__.py
--rw-rw-rw-   0        0        0    11875 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/alib.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.451091 gTixi-1.1.1/gTixi/gpio4/
--rw-rw-rw-   0        0        0    22841 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/gpio4/__init__.py
--rw-rw-rw-   0        0        0     4478 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/gpio4/arduino.py
--rw-rw-rw-   0        0        0     2107 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/gpio4/constants.py
--rw-rw-rw-   0        0        0     8211 2023-01-09 07:29:18.000000 gTixi-1.1.1/gTixi/gpioPins.py
--rw-rw-rw-   0        0        0     7559 2023-03-01 08:39:59.000000 gTixi-1.1.1/gTixi/starMod.py
--rw-rw-rw-   0        0        0     9243 2023-04-19 01:27:41.000000 gTixi-1.1.1/gTixi/starServer.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.535086 gTixi-1.1.1/gTixi/stardevice/
--rw-rw-rw-   0        0        0     1150 2022-12-08 00:17:57.000000 gTixi-1.1.1/gTixi/stardevice/favicon.ico
--rw-rw-rw-   0        0        0     3690 2023-04-19 01:15:50.000000 gTixi-1.1.1/gTixi/stardevice/index.html
--rw-rw-rw-   0        0        0   111756 2022-12-08 00:17:57.000000 gTixi-1.1.1/gTixi/stardevice/socket.io.js
--rw-rw-rw-   0        0        0   128872 2023-04-19 00:50:09.000000 gTixi-1.1.1/gTixi/stardevice/vue.global.js
--rw-rw-rw-   0        0        0     6388 2023-01-05 08:57:38.000000 gTixi-1.1.1/gTixi/wLTR390.py
--rw-rw-rw-   0        0        0    15044 2023-01-09 03:55:14.000000 gTixi-1.1.1/gTixi/waDrivers.py
--rw-rw-rw-   0        0        0     4118 2023-03-01 01:49:26.000000 gTixi-1.1.1/gTixi/waFile.py
--rw-rw-rw-   0        0        0     5983 2022-12-12 09:01:56.000000 gTixi-1.1.1/gTixi/waText.py
--rw-rw-rw-   0        0        0    22878 2023-04-11 00:41:59.000000 gTixi-1.1.1/gTixi/wadapter.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:59:14.442085 gTixi-1.1.1/gTixi.egg-info/
--rw-rw-rw-   0        0        0    30481 2023-04-19 01:59:13.000000 gTixi-1.1.1/gTixi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-04-19 01:59:14.000000 gTixi-1.1.1/gTixi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 01:59:13.000000 gTixi-1.1.1/gTixi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 01:59:13.000000 gTixi-1.1.1/gTixi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 01:59:14.540087 gTixi-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-19 01:51:25.000000 gTixi-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:43:31.895312 gTixi-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2022-12-02 07:39:30.000000 gTixi-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      123 2023-04-19 01:59:01.000000 gTixi-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    30690 2023-05-11 05:43:31.894311 gTixi-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    30256 2023-05-11 05:41:21.000000 gTixi-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 05:43:31.827311 gTixi-1.2.0/gTixi/
+-rw-rw-rw-   0        0        0   456248 2023-04-10 07:25:40.000000 gTixi-1.2.0/gTixi/Dianzhen.ttf
+-rw-rw-rw-   0        0        0     5570 2023-04-10 02:42:27.000000 gTixi-1.2.0/gTixi/SSD1306.py
+-rw-rw-rw-   0        0        0     1116 2023-01-04 05:19:56.000000 gTixi-1.2.0/gTixi/__init__.py
+-rw-rw-rw-   0        0        0    11875 2022-12-12 09:01:56.000000 gTixi-1.2.0/gTixi/alib.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:43:31.875348 gTixi-1.2.0/gTixi/gpio4/
+-rw-rw-rw-   0        0        0    22841 2022-12-12 09:01:56.000000 gTixi-1.2.0/gTixi/gpio4/__init__.py
+-rw-rw-rw-   0        0        0     4478 2022-12-12 09:01:56.000000 gTixi-1.2.0/gTixi/gpio4/arduino.py
+-rw-rw-rw-   0        0        0     2107 2022-12-12 09:01:56.000000 gTixi-1.2.0/gTixi/gpio4/constants.py
+-rw-rw-rw-   0        0        0     8211 2023-01-09 07:29:18.000000 gTixi-1.2.0/gTixi/gpioPins.py
+-rw-rw-rw-   0        0        0     7654 2023-05-11 05:26:48.000000 gTixi-1.2.0/gTixi/starMod.py
+-rw-rw-rw-   0        0        0    10686 2023-05-11 05:23:19.000000 gTixi-1.2.0/gTixi/starServer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:43:31.890311 gTixi-1.2.0/gTixi/stardevice/
+-rw-rw-rw-   0        0        0     1150 2022-12-08 00:17:57.000000 gTixi-1.2.0/gTixi/stardevice/favicon.ico
+-rw-rw-rw-   0        0        0     3688 2023-05-11 05:15:55.000000 gTixi-1.2.0/gTixi/stardevice/index.html
+-rw-rw-rw-   0        0        0   111756 2022-12-08 00:17:57.000000 gTixi-1.2.0/gTixi/stardevice/socket.io.js
+-rw-rw-rw-   0        0        0   128872 2023-04-19 00:50:09.000000 gTixi-1.2.0/gTixi/stardevice/vue.prod.js
+-rw-rw-rw-   0        0        0     6388 2023-01-05 08:57:38.000000 gTixi-1.2.0/gTixi/wLTR390.py
+-rw-rw-rw-   0        0        0    15044 2023-01-09 03:55:14.000000 gTixi-1.2.0/gTixi/waDrivers.py
+-rw-rw-rw-   0        0        0     4118 2023-03-01 01:49:26.000000 gTixi-1.2.0/gTixi/waFile.py
+-rw-rw-rw-   0        0        0     5983 2022-12-12 09:01:56.000000 gTixi-1.2.0/gTixi/waText.py
+-rw-rw-rw-   0        0        0    23628 2023-05-11 05:27:22.000000 gTixi-1.2.0/gTixi/wadapter.py
+drwxrwxrwx   0        0        0        0 2023-05-11 05:43:31.856313 gTixi-1.2.0/gTixi.egg-info/
+-rw-rw-rw-   0        0        0    30690 2023-05-11 05:43:30.000000 gTixi-1.2.0/gTixi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-11 05:43:30.000000 gTixi-1.2.0/gTixi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 05:43:30.000000 gTixi-1.2.0/gTixi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 05:43:30.000000 gTixi-1.2.0/gTixi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 05:43:31.895312 gTixi-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-05-11 05:43:09.000000 gTixi-1.2.0/setup.py
```

### Comparing `gTixi-1.1.1/LICENSE` & `gTixi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/PKG-INFO` & `gTixi-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gTixi
-Version: 1.1.1
+Version: 1.2.0
 Summary: 高效碳基演示体系核心模块
 Home-page: https://gitee.com/lxwk1spectre/walartminstar
 Author: Spectre Lee
 Author-email: lxwk1spectre@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -610,14 +610,19 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.2.0
+- 230511
+    - 加入了对m5stack(mwu)的支持
+    - 修改了类的继承语法，使之支持3.4以及之前的版本
+    - 修复了1.1.1版本中网页界面websockets无法使用的问题
 ## 1.1.1
 - 230319
     - 加入MAINFEST.in文件，处理非py文件的打包
 ## 1.1.0
 - 230319
     - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
     - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
```

### Comparing `gTixi-1.1.1/README.md` & `gTixi-1.2.0/gTixi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: gTixi
+Version: 1.2.0
+Summary: 高效碳基演示体系核心模块
+Home-page: https://gitee.com/lxwk1spectre/walartminstar
+Author: Spectre Lee
+Author-email: lxwk1spectre@foxmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 高效碳基演示机体系模块
 gTixi适用于高效碳基芯片测试的函数库  
 由魏楠和李若铭开发  
 联系开发者：<lxwk1spectre@foxmail.com>  
 gitee项目：<https://gitee.com/lxwk1spectre/walartminstar>
 # 功能介绍
 该模块包含了树莓派，掌控板，未来版，未名系列演示机的通用演示架构。可以使用一套代码，兼容地运行在不同地设备上。
@@ -597,14 +610,19 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.2.0
+- 230511
+    - 加入了对m5stack(mwu)的支持
+    - 修改了类的继承语法，使之支持3.4以及之前的版本
+    - 修复了1.1.1版本中网页界面websockets无法使用的问题
 ## 1.1.1
 - 230319
     - 加入MAINFEST.in文件，处理非py文件的打包
 ## 1.1.0
 - 230319
     - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
     - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
@@ -668,8 +686,8 @@
 - 221203
 - 相对稳定的初始测试版本，使用相对import引入，使架构更加科学。
 ## 0.0.2
 - 221202
 - 去除了部分alib的内容改为字典或者临时类，避免了zkb的无限重启的问题。
 ## 0.0.1
 - 221202
-- 初始版本发布。
+- 初始版本发布。
```

### Comparing `gTixi-1.1.1/gTixi/Dianzhen.ttf` & `gTixi-1.2.0/gTixi/Dianzhen.ttf`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/SSD1306.py` & `gTixi-1.2.0/gTixi/SSD1306.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/__init__.py` & `gTixi-1.2.0/gTixi/__init__.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/alib.py` & `gTixi-1.2.0/gTixi/alib.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/gpio4/__init__.py` & `gTixi-1.2.0/gTixi/gpio4/__init__.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/gpio4/arduino.py` & `gTixi-1.2.0/gTixi/gpio4/arduino.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/gpio4/constants.py` & `gTixi-1.2.0/gTixi/gpio4/constants.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/gpioPins.py` & `gTixi-1.2.0/gTixi/gpioPins.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/starMod.py` & `gTixi-1.2.0/gTixi/starMod.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         with open(sfn,'w') as f:
             f.write(textstr)        
 
 #基础的循环采集模式
 #只需要重载loopUnit函数即可
 class loopMod(baseMod):
     def __init__(self,mi):
-        baseMod.__init__(self,mi)
+        super(loopMod,self).__init__(mi)
+        #baseMod.__init__(self,mi)
         self.pause = False
         self.stop = False
         self.pauseWait = 0.5
         self.loopDelay = 0.5
     def loopUnit(self):
         self.output("Looping...")
     def loop(self,_=None):
@@ -92,15 +93,16 @@
             self.pause = not self.pause
         elif key in "LRBNOY":
             self.stop = True
 
 #高级循环
 class loopPro(baseMod):
     def __init__(self,mi):
-        baseMod.__init__(self,mi)
+        super(loopPro,self).__init__(mi)
+        #baseMod.__init__(self,mi)
         self.pause = False
         self.stop = False
         self.isRunning = False
     def loop(self):
         pass
 
     def running(self,_=None):
@@ -131,15 +133,15 @@
             elif key in "LRBNOY":
                 self.backToMenu()
 
 #关机面板：内容为纯黑屏        
 #暂时退出，关闭屏幕，按下任意键重新启动
 class offStatus(baseMod):
     def __init__(self,mi):
-        baseMod.__init__(self,mi)
+        super(offStatus,self).__init__(mi)
     def show(self):
         self.output(" ")
 
 class menu():
     def __init__(self,sm,initData,select=([],0),):
         self.data = initData
         self.submenu = select[0] #第一个数字代表哪个子目录，列表代表根目录；第二个为当前选中元素的下标
```

### Comparing `gTixi-1.1.1/gTixi/starServer.py` & `gTixi-1.2.0/gTixi/starServer.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,50 @@
         touchpad_h.event_pressed = inputH
         touchpad_o.event_pressed = inputO
         touchpad_n.event_pressed = inputN
         button_a.event_pressed = inputA
         button_b.event_pressed = inputB
     sm.allServers.append(zkbControl)
 
+if sm.shipei.name == 'mwu':
+    from m5stack import btnA,btnB,btnC
+    from m5stack_ui import M5Btn,FONT_UNICODE_24
+    def inputA():
+        sm.workModule.InputKey("U")
+    def inputB():
+        sm.workModule.InputKey("D")
+    def inputC():
+        sm.workModule.InputKey("B")
+    def inputD():
+        sm.workModule.InputKey("L")
+    def mwuControl():
+        btnWidth = 60
+        btnHeight = 40
+        btnY = 186
+        touch_button0 = M5Btn(
+            text='↑', x=30, y=btnY, w=btnWidth, h=btnHeight, bg_c=0xbfffc9, 
+            text_c=0x1a09c0, font=FONT_UNICODE_24, parent=None)
+        touch_button1 = M5Btn(
+            text='↓', x=125, y=btnY, w=btnWidth, h=btnHeight, bg_c=0xbfffc9, 
+            text_c=0x1a09c0, font=FONT_UNICODE_24, parent=None)
+        touch_button2 = M5Btn(
+            text='进入', x=220, y=btnY, w=btnWidth, h=btnHeight, bg_c=0xbfffc9, 
+            text_c=0x1a09c0, font=FONT_UNICODE_24, parent=None)
+        touch_button3 = M5Btn(
+            text='返回', x=247, y=20, w=btnWidth, h=btnHeight, bg_c=0xbfffc9, 
+            text_c=0x1a09c0, font=FONT_UNICODE_24, parent=None)
+        touch_button0.pressed(inputA)
+        touch_button1.pressed(inputB)
+        touch_button2.pressed(inputC)
+        touch_button3.pressed(inputD)
+        btnA.wasPressed(inputA)
+        btnB.wasPressed(inputB)
+        btnC.wasPressed(inputC)
+    sm.allServers.append(mwuControl)
+
 if sm.shipei.name == 'wlb':
     def wlbKey(_):
         from future import sensor
         while True:
             sm.shipei.Sleep(0.2)
             if sensor.btnValue("a"):
                 sm.workModule.InputKey("A")
```

### Comparing `gTixi-1.1.1/gTixi/stardevice/favicon.ico` & `gTixi-1.2.0/gTixi/stardevice/favicon.ico`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/stardevice/index.html` & `gTixi-1.2.0/gTixi/stardevice/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html>
 <head>
 <meta charset="utf-8">
 
 <script src="socket.io.js"></script> 
-<script src="vue.global.js"></script> 
+<script src="vue.prod.js"></script> 
 
 <title>starDevice</title>
 <link rel="icon" href="favicon.ico">
 <style type="text/css">
     body{
         font-size:22px;
     }
```

### Comparing `gTixi-1.1.1/gTixi/stardevice/socket.io.js` & `gTixi-1.2.0/gTixi/stardevice/socket.io.js`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/stardevice/vue.global.js` & `gTixi-1.2.0/gTixi/stardevice/vue.prod.js`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/wLTR390.py` & `gTixi-1.2.0/gTixi/wLTR390.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/waDrivers.py` & `gTixi-1.2.0/gTixi/waDrivers.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/waFile.py` & `gTixi-1.2.0/gTixi/waFile.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/waText.py` & `gTixi-1.2.0/gTixi/waText.py`

 * *Files identical despite different names*

### Comparing `gTixi-1.1.1/gTixi/wadapter.py` & `gTixi-1.2.0/gTixi/wadapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 [GTmcp|包含mcp23017和LTR390的扩展板]
 [GTamp|PKU RCCE, 可测转移曲线的扩展板]]'''
 #以上模块可在GTixi的任何主机上使用
 
 def AWaEnv():
     '''收集当前系统信息'''
     import os
+    import sys
+    aWaEnv['pythonVersion'] = sys.version
     try:
         un=os.uname()
         aWaEnv['sSysname']=un.sysname
         aWaEnv['sNodename']=un.nodename
         aWaEnv['sRelease']=un.release
         aWaEnv['sVersion']=un.version
         aWaEnv['sMachine']=un.machine
@@ -606,14 +608,32 @@
         if input:
             lines = input.split("\n")
             for i in range(len(lines)):
                 if i<4:
                     screen.textCh(self.str2unicode(lines[i]),0,25+20*i,1,(238,238,0) if i==0 else (0,238,238))
             screen.refresh()
 
+class SpMwu(Shipei):
+    def __init__(self,aenv):
+        super(SpMwu,self).__init__(aenv)
+        #Shipei.__init__(self,aenv)
+        self.name = "mwu"
+        self.oSvg = SvgScreen()
+        self.tag.extend(['debug'])
+        from m5stack_ui import M5Screen,M5Label,FONT_UNICODE_24
+        screen = M5Screen()
+        screen.clean_screen()
+        screen.set_screen_bg_color(0xFFFFFF)
+        label0 = M5Label('Loading...', x=16, y=19, color=0x000, font=FONT_UNICODE_24, parent=None)
+
+
+    def DrawStdLines(self,input):
+        self.label0.set_text(input)
+        return self.oSvg.DrawStdLines(input)
+
 class SpWin(Shipei):
     def __init__(self,aenv):
         Shipei.__init__(self,aenv)
         self.name = "win"
         self.oSvg = SvgScreen()
         self.tag.extend(['web','debug'])
     def CheckKey(self):
@@ -641,14 +661,16 @@
         ip='no network'
     aWaEnv['sIp']=ip
     return ip
 def Wa(aenv=aWaEnv):
     #if aenv == 'debug':
     if "SMP" in aenv['sVersion']:
         return SpSmp(aenv)
+    elif 'M5Stack' in aenv['sMachine']:
+        return SpMwu(aenv)
     elif 'mpython' in aenv['sMachine']:
         return SpZkb(aenv)
     elif 'Future' in aenv['sMachine']:
         return SpWlb(aenv)
     elif 'v7l' in aenv['sMachine']:
         if 'localhost' in aenv['sNodename']:
             return SpBdz(aenv)
```

### Comparing `gTixi-1.1.1/gTixi.egg-info/PKG-INFO` & `gTixi-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: gTixi
-Version: 1.1.1
-Summary: 高效碳基演示体系核心模块
-Home-page: https://gitee.com/lxwk1spectre/walartminstar
-Author: Spectre Lee
-Author-email: lxwk1spectre@foxmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 高效碳基演示机体系模块
 gTixi适用于高效碳基芯片测试的函数库  
 由魏楠和李若铭开发  
 联系开发者：<lxwk1spectre@foxmail.com>  
 gitee项目：<https://gitee.com/lxwk1spectre/walartminstar>
 # 功能介绍
 该模块包含了树莓派，掌控板，未来版，未名系列演示机的通用演示架构。可以使用一套代码，兼容地运行在不同地设备上。
@@ -610,14 +597,19 @@
 ### gpiopin(p0,p1)
 gpio调试工具，可以用于掌控版和未来板
 - p0:bool,p1:bool
     - p0针脚和p1针脚的输出，True为高电平，False为低电平
 - 返回：sf:str
     - 用于显示在显示屏上的字符串
 # 版本迭代
+## 1.2.0
+- 230511
+    - 加入了对m5stack(mwu)的支持
+    - 修改了类的继承语法，使之支持3.4以及之前的版本
+    - 修复了1.1.1版本中网页界面websockets无法使用的问题
 ## 1.1.1
 - 230319
     - 加入MAINFEST.in文件，处理非py文件的打包
 ## 1.1.0
 - 230319
     - 将smp的字体文件，webUI的网页文件压缩，一起内置如gTixi中，整个包大小控制在了1M以内。
     - 禁止了httpserver和websocketsServer的自启动，现在在import gTixi时不会启动任何服务，仅在需要的时候开启。
@@ -681,8 +673,8 @@
 - 221203
 - 相对稳定的初始测试版本，使用相对import引入，使架构更加科学。
 ## 0.0.2
 - 221202
 - 去除了部分alib的内容改为字典或者临时类，避免了zkb的无限重启的问题。
 ## 0.0.1
 - 221202
-- 初始版本发布。
+- 初始版本发布。
```

### Comparing `gTixi-1.1.1/gTixi.egg-info/SOURCES.txt` & `gTixi-1.2.0/gTixi.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 gTixi.egg-info/top_level.txt
 gTixi/gpio4/__init__.py
 gTixi/gpio4/arduino.py
 gTixi/gpio4/constants.py
 gTixi/stardevice/favicon.ico
 gTixi/stardevice/index.html
 gTixi/stardevice/socket.io.js
-gTixi/stardevice/vue.global.js
+gTixi/stardevice/vue.prod.js
```

### Comparing `gTixi-1.1.1/setup.py` & `gTixi-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gTixi",
-    version="1.1.1",
+    version="1.2.0",
     author="Spectre Lee",
     author_email="lxwk1spectre@foxmail.com",
     description="高效碳基演示体系核心模块",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://gitee.com/lxwk1spectre/walartminstar",
```

