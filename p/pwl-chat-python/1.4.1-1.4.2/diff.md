# Comparing `tmp/pwl-chat-python-1.4.1.tar.gz` & `tmp/pwl-chat-python-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.1.tar", last modified: Wed May 10 01:31:14 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.2.tar", last modified: Thu May 11 06:40:54 2023, max compression
```

## Comparing `pwl-chat-python-1.4.1.tar` & `pwl-chat-python-1.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.967748 pwl-chat-python-1.4.1/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     1891 2023-05-10 01:31:14.967242 pwl-chat-python-1.4.1/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1292 2023-05-10 01:17:54.000000 pwl-chat-python-1.4.1/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.953730 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     1891 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-10 01:31:14.967907 pwl-chat-python-1.4.1/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.954101 pwl-chat-python-1.4.1/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.957551 pwl-chat-python-1.4.1/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1993 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.964428 pwl-chat-python-1.4.1/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2625 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-10 01:27:04.000000 pwl-chat-python-1.4.1/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1961 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.1/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)      991 2023-05-10 01:28:45.000000 pwl-chat-python-1.4.1/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.965956 pwl-chat-python-1.4.1/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-10 01:19:01.000000 pwl-chat-python-1.4.1/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.259082 pwl-chat-python-1.4.2/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-11 06:40:54.258795 pwl-chat-python-1.4.2/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1409 2023-05-11 06:39:39.000000 pwl-chat-python-1.4.2/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.243081 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2008 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-11 06:40:54.000000 pwl-chat-python-1.4.2/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-11 06:40:54.259179 pwl-chat-python-1.4.2/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.243545 pwl-chat-python-1.4.2/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.248970 pwl-chat-python-1.4.2/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1993 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.2/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.256760 pwl-chat-python-1.4.2/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2625 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-10 01:27:04.000000 pwl-chat-python-1.4.2/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1961 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.2/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)      991 2023-05-10 01:28:45.000000 pwl-chat-python-1.4.2/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-11 06:40:54.258074 pwl-chat-python-1.4.2/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.2/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-11 06:39:58.000000 pwl-chat-python-1.4.2/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.1/LICENSE` & `pwl-chat-python-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/PKG-INFO` & `pwl-chat-python-1.4.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.1
+Version: 1.4.2
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -34,14 +34,22 @@
 
 ## 运行
 
 ```bash
 pwl-chat-python -u username -p password -c <两步验证码>
 ```
 
+## 调试
+
+如果你已安装,请先卸载，否则启动调试会执行安装好的包
+
+```bash
+python core.py
+```
+
 ## 功能
 
 - 💬 基本聊天吹水；
 - ⬆️ 社区快捷命令
   - 领取昨日活跃度奖励
   - 查看个人积分
   - 查看签到状态
```

### Comparing `pwl-chat-python-1.4.1/README.md` & `pwl-chat-python-1.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 
 ## 运行
 
 ```bash
 pwl-chat-python -u username -p password -c <两步验证码>
 ```
 
+## 调试
+
+如果你已安装,请先卸载，否则启动调试会执行安装好的包
+
+```bash
+python core.py
+```
+
 ## 功能
 
 - 💬 基本聊天吹水；
 - ⬆️ 社区快捷命令
   - 领取昨日活跃度奖励
   - 查看个人积分
   - 查看签到状态
```

### Comparing `pwl-chat-python-1.4.1/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.2/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.1
+Version: 1.4.2
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -34,14 +34,22 @@
 
 ## 运行
 
 ```bash
 pwl-chat-python -u username -p password -c <两步验证码>
 ```
 
+## 调试
+
+如果你已安装,请先卸载，否则启动调试会执行安装好的包
+
+```bash
+python core.py
+```
+
 ## 功能
 
 - 💬 基本聊天吹水；
 - ⬆️ 社区快捷命令
   - 领取昨日活跃度奖励
   - 查看个人积分
   - 查看签到状态
```

### Comparing `pwl-chat-python-1.4.1/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.2/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/setup.py` & `pwl-chat-python-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/api/__init__.py` & `pwl-chat-python-1.4.2/src/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/api/chatroom.py` & `pwl-chat-python-1.4.2/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/api/user.py` & `pwl-chat-python-1.4.2/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/__init__.py` & `pwl-chat-python-1.4.2/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/blacklist.py` & `pwl-chat-python-1.4.2/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/chatroom.py` & `pwl-chat-python-1.4.2/src/core/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/cli.py` & `pwl-chat-python-1.4.2/src/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/config.py` & `pwl-chat-python-1.4.2/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/redpacket.py` & `pwl-chat-python-1.4.2/src/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/user.py` & `pwl-chat-python-1.4.2/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/core/websocket.py` & `pwl-chat-python-1.4.2/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/main.py` & `pwl-chat-python-1.4.2/src/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.1/src/utils/utils.py` & `pwl-chat-python-1.4.2/src/utils/utils.py`

 * *Files identical despite different names*

