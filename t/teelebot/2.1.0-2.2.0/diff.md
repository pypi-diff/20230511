# Comparing `tmp/teelebot-2.1.0-py3-none-any.whl.zip` & `tmp/teelebot-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 38194 bytes, number of entries: 18
+Zip file size: 40299 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat     4126 b- defN 23-May-07 14:53 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-08 17:02 teelebot/__main__.py
--rw-rw-rw-  2.0 fat    31926 b- defN 23-May-09 03:02 teelebot/bot.py
--rw-rw-rw-  2.0 fat     7802 b- defN 23-May-09 00:52 teelebot/buffer.py
--rw-rw-rw-  2.0 fat    21867 b- defN 23-May-09 03:04 teelebot/handler.py
+-rw-rw-rw-  2.0 fat    42023 b- defN 23-May-11 15:08 teelebot/bot.py
+-rw-rw-rw-  2.0 fat     7835 b- defN 23-May-11 01:50 teelebot/buffer.py
+-rw-rw-rw-  2.0 fat    23836 b- defN 23-May-11 15:12 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1807 b- defN 23-May-03 00:00 teelebot/logger.py
 -rw-rw-rw-  2.0 fat      721 b- defN 23-May-03 00:01 teelebot/polling.py
 -rw-rw-rw-  2.0 fat     3700 b- defN 23-May-07 14:53 teelebot/request.py
 -rw-rw-rw-  2.0 fat     4075 b- defN 23-May-09 01:15 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      482 b- defN 23-May-09 01:11 teelebot/version.py
+-rw-rw-rw-  2.0 fat      482 b- defN 23-May-11 02:10 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 23-May-03 15:18 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-May-09 03:26 teelebot-2.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9052 b- defN 23-May-09 03:26 teelebot-2.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 03:26 teelebot-2.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-May-09 03:26 teelebot-2.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-09 03:26 teelebot-2.1.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-09 03:26 teelebot-2.1.0.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1406 b- defN 23-May-09 03:26 teelebot-2.1.0.dist-info/RECORD
-18 files, 125763 bytes uncompressed, 35916 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9624 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1406 b- defN 23-May-11 15:35 teelebot-2.2.0.dist-info/RECORD
+18 files, 138434 bytes uncompressed, 38021 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.1.0.dist-info/LICENSE
+Filename: teelebot-2.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.1.0.dist-info/METADATA
+Filename: teelebot-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.1.0.dist-info/WHEEL
+Filename: teelebot-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.1.0.dist-info/entry_points.txt
+Filename: teelebot-2.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.1.0.dist-info/top_level.txt
+Filename: teelebot-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.1.0.dist-info/zip-safe
+Filename: teelebot-2.2.0.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.1.0.dist-info/RECORD
+Filename: teelebot-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/bot.py

```diff
@@ -1,48 +1,55 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-08-13
-@last modification: 2023-05-09
+@last modification: 2023-05-11
 @author: Pluto (github:plutobell)
-@version: 2.1.0
+@version: 2.2.0
 """
 import time
 import sys
 import os
+import copy
 import types
 import string
 import random
 import shutil
 import inspect
 import importlib
+import threading
 
 from pathlib import Path
-from typing import Union, Callable
+from typing import Union, Callable, Tuple
 from concurrent.futures import ThreadPoolExecutor
 
 from .handler import _config, _bridge, _plugin_info
 from .logger import _logger
 from .schedule import _Schedule
 from .buffer import _Buffer
 from .request import _Request
 
 
 class Bot(object):
     """机器人的基类"""
 
-    def __init__(self, key=""):
+    def __init__(self, key: str = None, debug: bool = False, proxies: dict = None):
         config = _config()
 
-        if key != "":
+        if key not in [None, "", " "]:
             self._key = key
-        elif key == "":
+            self._debug = debug
+            if proxies is not None:
+                self.__proxies = proxies
+            else:
+                self.__proxies = config["proxies"]
+        else:
             self._key = config["key"]
-        
-        self.__proxies = config["proxies"]
+            self._debug = config["debug"]
+            self.__proxies = config["proxies"]
 
         self._cloud_api_server = config["cloud_api_server"]
         self._local_api_server = config["local_api_server"]
         if self._local_api_server != "False":
             self._basic_url = config["local_api_server"]
         else:
             self._basic_url = self._cloud_api_server
@@ -56,15 +63,14 @@
             self._server_address = config["server_address"]
             self._server_port = config["server_port"]
             self._local_address = config["local_address"]
             self._local_port = config["local_port"]
             self._secret_token = self.__make_token()
         self._offset = 0
         self._timeout = 60
-        self._debug = config["debug"]
         self._pool_size = config["pool_size"]
         self._buffer_size = config["buffer_size"]
         self._drop_pending_updates = config["drop_pending_updates"]
         self._updates_chat_member = config["updates_chat_member"]
         self._allowed_updates = []
         if self._updates_chat_member:
             self._allowed_updates = [
@@ -85,14 +91,15 @@
                 "chat_join_request"
             ]
 
         self.__root_id = config["root_id"]
         self.__bot_id = self._key.split(":")[0]
         self.__common_pkg_prefix = config["common_pkg_prefix"]
         self.__inline_mode_prefix = config["inline_mode_prefix"]
+        self.__metadata_template = config["metadata_template"]
         self.__AUTHOR = config["author"]
         self.__VERSION = config["version"]
         self.__plugin_dir = config["plugin_dir"]
         self.__plugin_bridge = config["plugin_bridge"]
         self.__non_plugin_list = config["non_plugin_list"]
         self.__start_time = int(time.time())
         self.__response_times = 0
@@ -111,14 +118,15 @@
         self.__timer_thread_pool = ThreadPoolExecutor(
             max_workers=int(self._pool_size) * 5)
 
         self.__plugin_info = config["plugin_info"]
         self.__non_plugin_info = config["non_plugin_info"]
 
         self.__method_name = "Unknown"
+        self.__plugin_info_mutex = threading.Lock()
 
         del config
         del thread_pool_size
         del schedule_queue_size
 
     def __del__(self):
         self.__thread_pool.shutdown(wait=True)
@@ -129,15 +137,15 @@
     def __getattr__(self, method_name):
         self.__method_name = method_name
         
         return types.MethodType(self.__method_function, self)
 
     def __method_function(self, *args, **kwargs):
         # command = inspect.stack()[0].function
-        if self._debug and len(args) != 1:
+        if len(args) != 1:
             _logger.error(f"Method '{self.__method_name}' does not accept positional arguments")
 
         return self.request.postEverything(self.__method_name, **kwargs)
 
     def __threadpool_exception(self, fur):
         """
         线程池异常回调
@@ -426,14 +434,29 @@
         message_type, message = self.__mark_message_for_pluginRun(message) # 分类标记消息
 
         if message_type == "unknown":
             self.__logging_for_pluginRun(message, "unknown")
             return
 
         for plugin, command in plugin_bridge.items():
+            plugin_requires_version = ""
+            plugin_info = self.get_plugin_info(plugin_name=plugin)
+            if plugin_info["status"]:
+                plugin_requires_version = plugin_info.get("metadata", {}).get("data", {}).get("Requires-teelebot", self.version)
+                plugin_requires_version = plugin_requires_version.replace(">", "").replace("<", "").replace("=", "")
+                if plugin_requires_version in [None, "", " "]:
+                    _logger.warn(f"Skip run {plugin} plugin: failed to get the version of the plugin")
+                    continue
+            else:
+                _logger.warn(f"Skip run {plugin} plugin: failed to get information about the plugin (error: {plugin_info['error']})")
+                continue
+            if plugin_requires_version > self.version:
+                _logger.warn(f"Skip run {plugin} plugin: the plugin requires teelebot version >= {plugin_requires_version}")
+                continue
+
             if message_type == "query":
                 if command in ["", " ", None]:
                     continue
 
             if message.get(message_type)[:len(command)] == command:
                 try:
                     module = self.__import_module(plugin)
@@ -602,59 +625,249 @@
                 "error": "PluginNotFound"
             }
             return info
 
         command = ""
         description = ""
         buffer_permissions = "Error"
-        with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}__init__.py"), "r", encoding="utf-8") as init:
-            lines = init.readlines()
-            
-            buffer_permissions_str = "False:False"
-            if len(lines) >= 1:
-                command = lines[0][1:].strip()
-            if len(lines) >= 2:
-                description = lines[1][1:].strip()
-            if len(lines) >= 3:
-                buffer_permissions_str = lines[2][1:].strip()
-
-            buffer_permissions_list = buffer_permissions_str.split(":", 1)
-            if buffer_permissions_str in [None, "", " "]:
-                buffer_permissions = tuple(False, False)
-            elif len(buffer_permissions_list) == 2:
+        with self.__plugin_info_mutex:
+            with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}__init__.py"), "r", encoding="utf-8") as init:
+                lines = init.readlines()
+                
+                buffer_permissions_str = "False:False"
+                if len(lines) >= 1:
+                    command = lines[0][1:].strip()
+                if len(lines) >= 2:
+                    description = lines[1][1:].strip()
+                if len(lines) >= 3:
+                    buffer_permissions_str = lines[2][1:].strip()
+
                 bool_true = ["True", "true"]
                 bool_false = ["False", "false"]
-                read = buffer_permissions_list[0]
-                write = buffer_permissions_list[1]
+                bool_true_and_false = ["True", "true", "False", "false"]
+                buffer_permissions_list = buffer_permissions_str.split(":", 1)
+                if len(buffer_permissions_list) != 2 and \
+                    buffer_permissions_str not in [None, "", " "]:
+                    info  = {
+                        "status": False,
+                        "error": "BufferPermissionsFormatError"
+                    }
+                    return info
+                if len(buffer_permissions_list) == 2 and \
+                    (buffer_permissions_list[0] not in bool_true_and_false or \
+                    buffer_permissions_list[1] not in bool_true_and_false):
+                    info  = {
+                        "status": False,
+                        "error": "BufferPermissionsFormatError"
+                    }
+                    return info
+
+                if buffer_permissions_str in [None, "", " "]:
+                    buffer_permissions = tuple((False, False))
+                elif len(buffer_permissions_list) == 2:
+                    read = buffer_permissions_list[0]
+                    write = buffer_permissions_list[1]
+
+                    if read in bool_true:
+                        read = True
+                    elif read in bool_false:
+                        read = False
+                    else:
+                        read = False
+                    
+                    if write in bool_true:
+                        write = True
+                    elif write in bool_false:
+                        write = False
+                    else:
+                        read = False
 
-                if read in bool_true:
-                    read = True
-                elif read in bool_false:
-                    read = False
-                else:
-                    read = False
-                
-                if write in bool_true:
-                    write = True
-                elif write in bool_false:
-                    write = False
+                    buffer_permissions = tuple((read, write))
+        
+        metadata = {}
+        with self.__plugin_info_mutex:
+            with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}METADATA"), "r", encoding="utf-8") as meta:
+                lines = meta.readlines()
+                metadata_data = {}
+                for line in lines:
+                    line = line.strip("\n").strip(" ")
+                    if line in [None, "", " "]:
+                        continue
+                    line_list = line.split(":", 1)
+                    if len(line_list) == 2:
+                        metadata_data[line_list[0].replace(" ", "")] = line_list[1].strip(" ")
+                    elif len(line_list) == 1:
+                        metadata_data[line_list[0].replace(" ", "")] = ""
+
+                if not (list(metadata_data.keys()) == list(self.__metadata_template.keys())):
+                    metadata = {
+                        "status": False,
+                        "error": "MetadataFormatError",
+                        "data": {}
+                    }
                 else:
-                    read = False
+                    metadata = {
+                        "status": True,
+                        "data": metadata_data
+                    }
 
-                buffer_permissions = tuple((read, write))
-        
-        info  = {
-            "status": True,
-            "command": command,
-            "description": description,
-            "buffer_permissions": buffer_permissions
-        }
+            info  = {
+                "status": True,
+                "command": command,
+                "description": description,
+                "buffer_permissions": buffer_permissions,
+                "metadata": metadata
+            }
 
-        return info
+            return info
 
+    def set_plugin_info(self, plugin_name: str = None,
+                        command: str = None, description: str = None,
+                        buffer_permissions: Tuple[bool, bool] = None,
+                        metadata: dict = None) -> dict:
+        """
+        设置指定插件的信息
+        """
+        if plugin_name in [None, "", " "]:
+            plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
+        
+        if plugin_name not in list(self.plugin_bridge.keys()):
+            info  = {
+                "status": False,
+                "error": "PluginNotFound"
+            }
+            return info
+        if command is None and description is None and \
+            buffer_permissions is None and metadata is None:
+            info  = {
+                "status": True,
+                "error": "Skip"
+            }
+            return info
+        only_metadata = False
+        if command is None and description is None and buffer_permissions is None:
+            only_metadata = True
+
+        status = True
+        if not only_metadata:
+            old_info = self.get_plugin_info(plugin_name=plugin_name)
+            if not old_info["status"]:
+                info  = {
+                    "status": False,
+                    "error": "GetOlderPluginInfoError"
+                }
+                return info
+
+            if command is None:
+                command = f'{old_info["command"]}'
+            if description is None:
+                description = f'{old_info["description"]}'
+            
+            buffer_permissions_str = "False:False"
+            if buffer_permissions is not None:
+                if not isinstance(buffer_permissions, tuple) or \
+                    len(buffer_permissions) != 2 or \
+                    not isinstance(buffer_permissions[0], bool) or \
+                    not isinstance(buffer_permissions[0], bool):
+                    info  = {
+                        "status": False,
+                        "error": "BufferPermissionsFormatError"
+                    }
+                    return info
+                read = str(buffer_permissions[0])
+                write = str(buffer_permissions[1])
+                buffer_permissions_str = f'{read}:{write}'
+            else:
+                read = str(old_info["buffer_permissions"][0])
+                write = str(old_info["buffer_permissions"][1])
+                buffer_permissions_str = f'{read}:{write}'
+
+            new_init_info = [
+                f'#{command.strip()}\n',
+                f'#{description.strip()}\n',
+            ]
+            try:
+                with self.__plugin_info_mutex:
+                    with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}__init__.py"), "r", encoding="utf-8") as init:
+                        lines = init.readlines()
+                        if len(lines) < 2:
+                            info  = {
+                                "status": False,
+                                "error": "InitFileFormatError"
+                            }
+                            return info
+                        if len(lines) >= 3:
+                            if buffer_permissions is not None or \
+                                lines[2].strip() not in [None, "", " ", "#"]:
+                                new_init_info.append(f'#{buffer_permissions_str.strip()}\n')
+                            else:
+                                new_init_info.append("#\n")
+                        elif buffer_permissions is not None:
+                            new_init_info.append(f'#{buffer_permissions_str.strip()}\n')
+                        else:
+                            new_init_info.append("#\n")
+                        new_init_info.extend(lines[3:])
+                        new_init_info[-1] = new_init_info[-1].strip()
+                with self.__plugin_info_mutex:
+                    with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}__init__.py"), "w", encoding="utf-8") as init:
+                        init.writelines(new_init_info)
+
+                status = True
+                if metadata is None:
+                    info  = {
+                        "status": True,
+                    }
+                    return info
+            except Exception as e:
+                print(f"Modify plugin info error: {str(e)}")
+                status = False
+                info  = {
+                    "status": status,
+                    "error": "ModifyPluginInfoError"
+                }
+                return info
+
+        if status and metadata is not None:
+            if not isinstance(metadata, dict):
+                info  = {
+                    "status": False,
+                    "error": "MetadataMustBeDict"
+                }
+                return info
+            if not (list(metadata.keys()) == list(self.__metadata_template.keys())):
+                metadata = {
+                    "status": False,
+                    "error": "MetadataFormatError",
+                }
+                return info
+
+            try:
+                with self.__plugin_info_mutex:
+                    with open(self.path_converter(f"{self.plugin_dir}{plugin_name}{os.sep}METADATA"), "w", encoding="utf-8") as meta:
+                        metadata_list = []
+                        for key, value in metadata.items():
+                                metadata_list.append(f"{key}: {value}\n")
+                        metadata_list[-1] = metadata_list[-1].strip()
+                        if metadata_list[-1].split(":")[1].strip() in [None, ""]:
+                            metadata_list[-1] += " "
+
+                        meta.writelines(metadata_list)
+
+                        info = {
+                            "status": True,
+                        }
+                        return info
+            except Exception as e:
+                print(f"Modify plugin info error: {str(e)}")
+                info  = {
+                    "status": False,
+                    "error": "ModifyPluginInfoError"
+                }
+                return info
+            
     def getChatCreator(self, chat_id: str) -> Union[bool, dict]:
         """
         获取群组创建者信息
         """
         if str(chat_id)[0] == "-":
             req = self.getChatAdministrators(chat_id=str(chat_id))
             if req:
@@ -734,15 +947,15 @@
 
     @property
     def plugin_bridge(self):
         """
         获取插件桥
         """
 
-        return self.__plugin_bridge
+        return copy.deepcopy(self.__plugin_bridge)
 
     @property
     def plugin_dir(self):
         """
         获取插件路径
         """
 
@@ -797,24 +1010,31 @@
         return self.__response_times
 
     @property
     def response_chats(self):
         """
         获取框架启动后响应的所有群组ID
         """
-        return self.__response_chats
+        return copy.deepcopy(self.__response_chats)
 
     @property
     def response_users(self):
         """
         获取框架启动后响应的所有用户ID
         """
-        return self.__response_users
+        return copy.deepcopy(self.__response_users)
     
     @property
     def proxies(self):
         """
         获取代理信息
         """
-        return self.__proxies
-        
+        return copy.deepcopy(self.__proxies)
+    
+    @property
+    def metadata_template(self):
+        """
+        获取插件元素据模板
+        """
+        return copy.deepcopy(self.__metadata_template)
+
```

## teelebot/buffer.py

```diff
@@ -1,10 +1,10 @@
 '''
 @creation date: 2021-04-25
-@last modification: 2023-05-09
+@last modification: 2023-05-11
 '''
 from __future__ import print_function
 from sys import getsizeof, stderr
 from itertools import chain
 from collections import deque
 from pathlib import Path
 from typing import Tuple, Union
@@ -76,22 +76,22 @@
         """
         isSelf = False
         if plugin_name in [None, "", " "]:
             isSelf = True
             plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
 
         if plugin_name in self.__buffer.keys():
-            ok, permission = self.__permission_check(plugin_name)
+            ok, permissions = self.__permissions_check(plugin_name)
             if ok:
-                permission_read = permission[0]
-                # permission_write = permission[1]
-                if not permission_read and not isSelf:
+                permissions_read = permissions[0]
+                # permissions_write = permissions[1]
+                if not permissions_read and not isSelf:
                     return False, "NoPermissionToRead"
             else:
-                return False, permission
+                return False, permissions
 
             with self.__buffer_mutex:
                 return True, copy.deepcopy(self.__buffer.get(plugin_name, {}))
         else:
             return False, "NoPlugin"
 
     def write(self, buffer: any, plugin_name: str = None) -> Tuple[bool, Union[str, tuple]]:
@@ -100,22 +100,22 @@
         """
         isSelf = False
         if plugin_name in [None, "", " "]:
             isSelf = True
             plugin_name = os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]
 
         if plugin_name in self.__buffer.keys():
-            ok, permission = self.__permission_check(plugin_name)
+            ok, permissions = self.__permissions_check(plugin_name)
             if ok:
-                # permission_read = permission[0]
-                permission_write = permission[1]
-                if not permission_write and not isSelf:
+                # permissions_read = permissions[0]
+                permissions_write = permissions[1]
+                if not permissions_write and not isSelf:
                     return False, "NoPermissionToWrite"
             else:
-                return False, permission
+                return False, permissions
 
             with self.__buffer_mutex:
                 old_total_used = self.__total_size(self.__buffer)
                 old_buffer_used = self.__total_size(self.__buffer[plugin_name])
                 new_buffer_used = self.__total_size(buffer)
 
                 if (old_total_used - old_buffer_used) + new_buffer_used > self.__buffer_size:
@@ -138,47 +138,47 @@
                     if plugin_name not in self.__buffer.keys(): # 添加新插件
                         self.__buffer[plugin_name] = {}
 
             return True
         else:
             return False
 
-    def __permission_check(self, plugin_name):
+    def __permissions_check(self, plugin_name):
         if plugin_name in self.__buffer.keys():
             if plugin_name != os.path.splitext(os.path.basename(inspect.stack()[1][1]))[0]: # 读写权限检查
                 with open(Path(self.__plugin_dir + plugin_name + os.sep + "__init__.py"), "r", encoding="utf-8") as init:
                     lines = init.readlines()
 
                 for i, _ in enumerate(lines):
                     lines[i] = lines[i].strip("\n")
                     lines[i] = lines[i].strip("\r")
                     lines[i] = lines[i].strip("")
                     lines[i] = lines[i].strip()
 
                 if len(lines) > 2:
-                    permission = lines[2][1:]
+                    permissions = lines[2][1:]
                     if lines[2] == "#":
-                        permission = "False:False"
+                        permissions = "False:False"
                 else:
-                    permission = "False:False" # 格式 读:写
+                    permissions = "False:False" # 格式 读:写
 
-                if len(permission.split(":")) == 2:
-                    permission_read = permission.split(":")[0]
-                    permission_write = permission.split(":")[1]
-                    if permission_read in ["True", "False", "true", "false"] and \
-                        permission_write in ["True", "False", "true", "false"]:
+                if len(permissions.split(":")) == 2:
+                    permissions_read = permissions.split(":")[0]
+                    permissions_write = permissions.split(":")[1]
+                    if permissions_read in ["True", "False", "true", "false"] and \
+                        permissions_write in ["True", "False", "true", "false"]:
                         bool_dict = {
                             "True": True,
                             "true": True,
                             "False": False,
                             "false": False
                         }
-                        permission_read = bool_dict[permission_read]
-                        permission_write = bool_dict[permission_write]
-                        return True, tuple((permission_read, permission_write))
+                        permissions_read = bool_dict[permissions_read]
+                        permissions_write = bool_dict[permissions_write]
+                        return True, tuple((permissions_read, permissions_write))
                     else:
                         return False, "PermissionFormatError"
                 else:
                     return False, "PermissionFormatError"
 
     def __total_size(self, o, handlers={}, verbose=False):
         dict_handler = lambda d: chain.from_iterable(d.items())
```

## teelebot/handler.py

```diff
@@ -1,25 +1,40 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-08-23
-@last modification: 2023-05-09
+@last modification: 2023-05-10
 '''
 import configparser
 import argparse
 import os
 import sys
+import copy
 import shutil
 import requests
 
 from pathlib import Path
 from .version import __author__, __github__, __version__
 
 cloud_api_server = "https://api.telegram.org/"
 common_pkg_prefix = "~~"
 inline_mode_prefix = "?:"
+metadata_template = { # METADATA v1.0
+    "Metadata-version": "1.0",
+    "Plugin-name": "",
+    "Version": "",
+    "Summary": "",
+    "Home-page": "",
+    "Author": "",
+    "Author-email": "",
+    "License": "",
+    "Keywords": "",
+    "Requires-teelebot": "",
+    "Requires-dist": "",
+    "Source": ""
+}
 
 parser = argparse.ArgumentParser(description="teelebot console command list")
 parser.add_argument("-c", "--config", type=str,
                     help="specify the configuration file")
 parser.add_argument("-k", "--key", type=str,
                     help="specify the bot api token")
 parser.add_argument("-r", "--root", type=str,
@@ -97,16 +112,17 @@
                 "cert_pub = " + "\n",
                 "server_address = " + "\n",
                 "server_port = " + "\n",
                 "local_address = " + "\n",
                 "local_port = " + "\n",
                 "proxy = "
             ])
+            os.system("")
             print("The configuration file has been created automatically.")
-            print("Configuration file path: " + str(config_dir))
+            print("Configuration file path: \033[1;32m" + str(config_dir) + "\033[0m") # Green
         if not args.key or not args.root:
             print("Please modify the relevant parameters and restart the teelebot.")
             os._exit(0)
         # else:
         #     print("\n")
 
     conf = configparser.ConfigParser()
@@ -192,15 +208,16 @@
         plugin_name = args.make_plugin
         if not os.path.exists(str(Path(plugin_dir + plugin_name))):
             os.mkdir(str(Path(plugin_dir + plugin_name)))
             if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + "__init__.py"))):
                 with open(str(Path(plugin_dir + plugin_name + os.sep + "__init__.py")), "w", encoding="utf-8") as init:
                     init.writelines([
                         "#/" + plugin_name.lower() + "\n",
-                        "#" + plugin_name + " Plugin\n"
+                        "#" + plugin_name + " Plugin\n",
+                        "#"
                     ])
             if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + plugin_name + ".py"))):
                 with open(str(Path(plugin_dir + plugin_name + os.sep + plugin_name + ".py")), "w", encoding="utf-8") as enter:
                     enter.writelines([
                         "# -*- coding: utf-8 -*-\n",
                         "\n",
                         "def " + plugin_name + "(bot, message):\n",
@@ -214,15 +231,17 @@
                         "    # plugin_dir = bot.plugin_dir\n" + \
                         "    # plugin_bridge = bot.plugin_bridge\n" + \
                         "\n" + \
                         "    # uptime = bot.uptime\n" + \
                         "    # response_times = bot.response_times\n" + \
                         "    # response_chats = bot.response_chats\n" + \
                         "    # response_users = bot.response_users\n" + \
+                        "\n" + \
                         "    # proxies = bot.proxies\n" + \
+                        "    # metadata_template = bot.metadata_template\n" + \
                         "\n" + \
                         '    chat_id = message["chat"]["id"]\n' + \
                         '    user_id = message["from"]["id"]\n' + \
                         '    message_id = message["message_id"]\n' + \
                         "\n" + \
                         '    message_type = message["message_type"]\n' + \
                         '    chat_type = message["chat"]["type"]\n' + \
@@ -233,32 +252,31 @@
                         '        command = plugin_info.get("command", "")\n' + \
                         "\n\n" + \
                         "    # Write your plugin code below"
                     ])
             if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + "README.md"))):
                 with open(str(Path(plugin_dir + plugin_name + os.sep + "README.md")), "w", encoding='utf-8') as readme:
                     readme.writelines([
-                        "# " + plugin_name + " #\n"
+                        "# " + plugin_name + "\n"
                     ])
             if not os.path.exists(str(Path(plugin_dir + plugin_name + os.sep + "METADATA"))):
                 with open(str(Path(plugin_dir + plugin_name + os.sep + "METADATA")), "w", encoding='utf-8') as metadata:
-                    metadata.writelines([
-                        "Metadata-version: 1.0\n",
-                        "Plugin-name: " + plugin_name + "\n",
-                        "Version: 0.1.0\n",
-                        "Summary: \n",
-                        "Home-page: \n",
-                        "Author: \n",
-                        "Author-email: \n",
-                        "License: \n",
-                        "Keywords: \n",
-                        "Requires-teelebot: >=" + __version__ + "\n",
-                        "Requires-dist: \n",
-                        "Source: "
-                    ])
+                    metadata_data = copy.deepcopy(metadata_template)
+                    metadata_data["Plugin-name"] = plugin_name
+                    metadata_data["Version"] = "0.1.0"
+                    metadata_data["Requires-teelebot"] = f">={__version__}"
+
+                    metadata_list = []
+                    for key, value in metadata_data.items():
+                        metadata_list.append(f"{key}: {value}\n")
+                    metadata_list[-1] = metadata_list[-1].strip()
+                    if metadata_list[-1].split(":")[1].strip() in [None, ""]:
+                            metadata_list[-1] += " "
+
+                    metadata.writelines(metadata_list)
 
             print("Plugin " + plugin_name + " was created successfully.")
         else:
             print("Plugin " + plugin_name + " already exists.")
         os._exit(0)
     elif args.make_plugin and not plugin_dir_in_config:
         print("The plugin_dir is not set in the configuration file.")
@@ -366,14 +384,15 @@
     config["plugin_info"] = _plugin_info(
         config["plugin_bridge"].keys(), config["plugin_dir"])
     config["non_plugin_info"] = _plugin_info(
         config["non_plugin_list"], config["plugin_dir"])
     config["cloud_api_server"] = cloud_api_server
     config["common_pkg_prefix"] = common_pkg_prefix
     config["inline_mode_prefix"] = inline_mode_prefix
+    config["metadata_template"] = metadata_template
 
     # print(config)
     return config
 
 def _bridge(plugin_dir):
     '''
     获取插件和指令的映射
@@ -402,19 +421,40 @@
                         entrance_count += content.count(f"def {plugi}(message, bot):")
                         entrance_count += content.count(f"def {plugi}(bot,message):")
                         entrance_count += content.count(f"def {plugi}(message,bot):")
             except Exception as e:
                 os.system("")
                 print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + str(e))
 
+            metadata_ok = False
+            try:
+                with open(str(Path(f"{plugin_dir}{plugi}{os.sep}METADATA")), "r", encoding="utf-8") as meta:
+                    lines = meta.readlines()
+                    metadata_data = {}
+                    for line in lines:
+                        line = line.strip("\n").strip(" ")
+                        if line in [None, "", " "]:
+                            continue
+                        line_list = line.split(":", 1)
+                        if len(line_list) == 2:
+                            metadata_data[line_list[0].replace(" ", "")] = line_list[1].strip(" ")
+                        elif len(line_list) == 1:
+                            metadata_data[line_list[0].replace(" ", "")] = ""
+
+                    if list(metadata_data.keys()) == list(metadata_template.keys()):
+                        metadata_ok = True
+            except Exception as e:
+                os.system("")
+                print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + str(e))
+
             package_file_list = os.listdir(str(Path(plugin_dir + plugi)))
             if plugi + ".py" in package_file_list and \
                 "__init__.py" in package_file_list and \
                 "METADATA" in package_file_list and \
-                entrance_exist and entrance_count == 1:
+                entrance_exist and entrance_count == 1 and metadata_ok:
                 plugin_list.append(plugi)
             else:
                 corrupted_plugin_list.append(plugi)
 
                 missing_files_count = 0
                 error = f"plugin missing "
                 if f"{plugi}.py" not in package_file_list:
@@ -435,14 +475,19 @@
                     os.system("")
                     print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + error)
                 elif entrance_exist and entrance_count != 1:
                     error = f"multiple entrance functions exist in plugin"
                     os.system("")
                     print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + error)
 
+                if not metadata_ok:
+                    error = f"metadata format error"
+                    os.system("")
+                    print("\033[1;31mThe " + plugi + " plugin is corrupted: " + "\033[0m" + error)
+
     for plugin in plugin_list:
         with open(str(Path(plugin_dir + plugin + r"/__init__.py")), encoding="utf-8") as f:
             row_one = f.readline().strip()[1:]
             if row_one != common_pkg_prefix:  # Hidden plugin
                 plugin_bridge[plugin] = row_one
             else:
                 if plugin in corrupted_plugin_list:
```

## teelebot/version.py

```diff
@@ -1,17 +1,17 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-11-15
-@last modification: 2023-05-09
+@last modification: 2023-05-11
 @author: Pluto (github:plutobell)
-@version: 2.1.0
+@version: 2.2.0
 """
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
```

## Comparing `teelebot-2.1.0.dist-info/LICENSE` & `teelebot-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.1.0.dist-info/METADATA` & `teelebot-2.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.1.0
+Version: 2.2.0
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
@@ -319,14 +319,34 @@
 teelebot -c/--config <configure file path>
 ```
 
 路径必须为绝对路径，并且配置文件名也应当包含在路径内，此情况下会在指定的配置文件不存在时自动生成配置文件 。
 
 
 
+#### 四、导入使用
+
+```python
+# 导入Bot类
+from teelebot import Bot
+
+# 实例化Bot类
+# 不传参数时会使用teelebot默认配置文件路径下的配置文件实例化Bot类
+# 在v2.2.0及以上版本，可传递参数覆盖配置文件的设定，可用参数:
+#     Bot(key: str = None, debug: bool = False, proxies: dict = None)
+bot = Bot()
+
+# 使用Bot类
+bot.sendMessage(chat_id="chat_id", text="Hello World!")
+```
+
+**Tip: 导入使用时需要确保默认配置文件路径中存在配置文件,并且必须的字段已经填写**
+
+
+
 
 
 ## 联系我
 
 * Email：hi#ojoll.com ( # == @ )
 * Blog:    [北及](https://ojoll.com)
 * Telegram Group：[teelebot official](https://t.me/teelebot_official)（t.me/teelebot_official）
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.1.0 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.2.0 Summary: teelebot is a
 robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com Author: Pluto Author-email: hi@ojoll.com License:
 GPLv3 Keywords: teelebot telegram bot telegram bot api telegram Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
@@ -104,12 +104,20 @@
 `config.cfg`ã * å¨Linuxä¸ï¼ä¼èªå¨å¨ç¨æ·ç®å½ä¸åå»ºæä»¶å¤¹
 `.teelebot` ï¼å¹¶çæéç½®æä»¶ `config.cfg` * å¨Windowsä¸ï¼åä¼å¨
 `C:\Users\` ç®å½ä¸åå»ºæä»¶å¤¹ `.teelebot` ï¼å¹¶çæéç½®æä»¶
 `config.cfg` 2.æå®éç½®æä»¶ Linux å Windows
 é½å¯å¨å½ä»¤è¡éè¿åæ°æå¨æå®éç½®æä»¶è·¯å¾ï¼å½ä»¤æ ¼å¼ï¼
 ``` teelebot -c/--config  ```
 è·¯å¾å¿é¡»ä¸ºç»å¯¹è·¯å¾ï¼å¹¶ä¸éç½®æä»¶åä¹åºå½åå«å¨è·¯å¾åï¼æ­¤æåµä¸ä¼å¨æå®çéç½®æä»¶ä¸å­å¨æ¶èªå¨çæéç½®æä»¶
-ã ## èç³»æ * Emailï¼hi#ojoll.com ( # == @ ) * Blog: [åå](https://
+ã #### åãå¯¼å¥ä½¿ç¨ ```python # å¯¼å¥Botç±» from teelebot import Bot #
+å®ä¾åBotç±» #
+ä¸ä¼ åæ°æ¶ä¼ä½¿ç¨teeleboté»è®¤éç½®æä»¶è·¯å¾ä¸çéç½®æä»¶å®ä¾åBotç±»
+#
+å¨v2.2.0åä»¥ä¸çæ¬ï¼å¯ä¼ éåæ°è¦çéç½®æä»¶çè®¾å®ï¼å¯ç¨åæ°:
+# Bot(key: str = None, debug: bool = False, proxies: dict = None) bot = Bot() #
+ä½¿ç¨Botç±» bot.sendMessage(chat_id="chat_id", text="Hello World!") ``` **Tip:
+å¯¼å¥ä½¿ç¨æ¶éè¦ç¡®ä¿é»è®¤éç½®æä»¶è·¯å¾ä¸­å­å¨éç½®æä»¶,å¹¶ä¸å¿é¡»çå­æ®µå·²ç»å¡«å**
+## èç³»æ * Emailï¼hi#ojoll.com ( # == @ ) * Blog: [åå](https://
 ojoll.com) * Telegram Groupï¼[teelebot official](https://t.me/
 teelebot_official)ï¼t.me/teelebot_officialï¼ * ~~Telegram Groupï¼
 [teelebotä½éªç¾¤](http://t.me/teelebot_chat)ï¼t.me/teelebot_chatï¼~~ *
 å¶ä»ï¼æ¬repo ç Issue
```

## Comparing `teelebot-2.1.0.dist-info/RECORD` & `teelebot-2.2.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 teelebot/__init__.py,sha256=_RulqeVSYAqRhTaljCZfWctBfVdmjCIC8Qp-ewpeOY4,4126
 teelebot/__main__.py,sha256=_j6f3hj0VtlcCsabcIvuS0uBI0NVbCVwmH138tqYGFo,165
-teelebot/bot.py,sha256=QWqYYWhmUUxGbYHjOjjZphL1Uj_O8hMGlrEMZ5SakNs,31926
-teelebot/buffer.py,sha256=YS69_8lqrzZp0WCideDY1nsuNZCGCRguz6KlZsjdvxA,7802
-teelebot/handler.py,sha256=_XoyJfQYSQM9pDNvg7hKo3xNqrqbTQNt7mhd3cm8oYg,21867
+teelebot/bot.py,sha256=Gepj4s9ZPL2yNZAR_Df7PfJfWPMqvQr5LVy2NGGoiRU,42023
+teelebot/buffer.py,sha256=2h1dT2bz6G7H69dpclDZoGBWsFcoXbNUh2ytsXMrXGc,7835
+teelebot/handler.py,sha256=RHmXCz_Ooqqci_JN_KYQgAYtcM9HiJAB3gxPe_OsZEg,23836
 teelebot/logger.py,sha256=_QWA2Kbj-JWNYDtgeK6IE7q34Brxrq6cUgHEH4YTu2M,1807
 teelebot/polling.py,sha256=7lPDDeVInhk8MH-ZQhzGXYW-uI5t-F0XtMYkMrcEDEU,721
 teelebot/request.py,sha256=aYrdPV-IRJPdiZgZlIjU4es8QokOzs8Jn_bZVd_aI3I,3700
 teelebot/schedule.py,sha256=GGcFlEwpfO254D-2-ALBdAv539i97r_nAUnCJLBnA4o,4075
-teelebot/version.py,sha256=YzTDbJBL3pDhc5ICyZ3Oy1X4jPucTjIH-bCTtTF9oFA,482
+teelebot/version.py,sha256=KH4QIKWu9j8DbB2tEDDblnkbRd_m351qOb0dSkLTuxc,482
 teelebot/webhook.py,sha256=IomyaLxak_caDNYKNnLaTLtqkFToYq4sHWsD7kahV4Y,2665
-teelebot-2.1.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-2.1.0.dist-info/METADATA,sha256=FgXovssbpbKCYPmZ2KejITaUCOJ0I2-CA6SQM0WyQ74,9052
-teelebot-2.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-2.1.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-2.1.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-2.1.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-2.1.0.dist-info/RECORD,,
+teelebot-2.2.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.2.0.dist-info/METADATA,sha256=9MF5dBUKrbWOcXCSUiTz8U7L0LM4N3X640XmZjW1z24,9624
+teelebot-2.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-2.2.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.2.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.2.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.2.0.dist-info/RECORD,,
```

