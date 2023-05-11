# Comparing `tmp/djlds-2022.5.23.tar.gz` & `tmp/djlds-2023.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djlds-2022.5.23.tar", last modified: Mon May 23 09:47:47 2022, max compression
+gzip compressed data, was "dist\djlds-2023.5.11.tar", last modified: Thu May 11 06:31:54 2023, max compression
```

## Comparing `djlds-2022.5.23.tar` & `djlds-2023.5.11.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-05-23 09:47:47.000000 djlds-2022.5.23/
-drwxrwxrwx   0        0        0        0 2022-05-23 09:47:47.000000 djlds-2022.5.23/djlds/
--rw-rw-rw-   0        0        0    11680 2022-03-26 06:43:30.000000 djlds-2022.5.23/djlds/admin.py
--rw-rw-rw-   0        0        0    18599 2022-04-15 04:49:37.000000 djlds-2022.5.23/djlds/import_export.py
-drwxrwxrwx   0        0        0        0 2022-05-23 09:47:47.000000 djlds-2022.5.23/djlds/management/
-drwxrwxrwx   0        0        0        0 2022-05-23 09:47:47.000000 djlds-2022.5.23/djlds/management/commands/
--rw-rw-rw-   0        0        0    13971 2019-12-09 08:21:17.000000 djlds-2022.5.23/djlds/management/commands/admin_generator.py
--rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2022.5.23/djlds/management/commands/__init__.py
--rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2022.5.23/djlds/management/__init__.py
--rw-rw-rw-   0        0        0    21490 2022-05-23 09:46:09.000000 djlds-2022.5.23/djlds/model.py
--rw-rw-rw-   0        0        0      449 2022-05-18 10:49:19.000000 djlds-2022.5.23/djlds/timezone.py
--rw-rw-rw-   0        0        0     2367 2022-01-21 02:47:57.000000 djlds-2022.5.23/djlds/user.py
--rw-rw-rw-   0        0        0     2859 2020-07-01 04:00:38.000000 djlds-2022.5.23/djlds/util.py
--rw-rw-rw-   0        0        0     1240 2020-03-20 08:22:22.000000 djlds-2022.5.23/djlds/xlsx_util.py
--rw-rw-rw-   0        0        0      656 2019-12-09 05:46:20.000000 djlds-2022.5.23/djlds/__about__.py
--rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2022.5.23/djlds/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-23 09:47:47.000000 djlds-2022.5.23/djlds.egg-info/
--rw-rw-rw-   0        0        0        1 2022-05-23 09:47:46.000000 djlds-2022.5.23/djlds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-12-09 09:34:28.000000 djlds-2022.5.23/djlds.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1359 2022-05-23 09:47:46.000000 djlds-2022.5.23/djlds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2022-05-23 09:47:46.000000 djlds-2022.5.23/djlds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      469 2022-05-23 09:47:46.000000 djlds-2022.5.23/djlds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2022-05-23 09:47:46.000000 djlds-2022.5.23/djlds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-12-09 06:34:14.000000 djlds-2022.5.23/MANIFEST.in
--rw-rw-rw-   0        0        0     1359 2022-05-23 09:47:47.000000 djlds-2022.5.23/PKG-INFO
--rw-rw-rw-   0        0        0      329 2019-12-09 06:31:13.000000 djlds-2022.5.23/README.md
--rw-rw-rw-   0        0        0       42 2022-05-23 09:47:47.000000 djlds-2022.5.23/setup.cfg
--rw-rw-rw-   0        0        0     2916 2022-05-23 09:47:45.000000 djlds-2022.5.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/
+drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds/
+-rw-rw-rw-   0        0        0    11686 2022-11-22 10:26:59.000000 djlds-2023.5.11/djlds/admin.py
+-rw-rw-rw-   0        0        0    18794 2023-05-11 06:23:49.000000 djlds-2023.5.11/djlds/import_export.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds/management/
+drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds/management/commands/
+-rw-rw-rw-   0        0        0    13971 2019-12-09 08:21:17.000000 djlds-2023.5.11/djlds/management/commands/admin_generator.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.11/djlds/management/commands/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.11/djlds/management/__init__.py
+-rw-rw-rw-   0        0        0    22248 2022-10-14 11:21:38.000000 djlds-2023.5.11/djlds/model.py
+-rw-rw-rw-   0        0        0      449 2022-05-18 10:49:19.000000 djlds-2023.5.11/djlds/timezone.py
+-rw-rw-rw-   0        0        0     2367 2022-01-21 02:47:57.000000 djlds-2023.5.11/djlds/user.py
+-rw-rw-rw-   0        0        0     2859 2020-07-01 04:00:38.000000 djlds-2023.5.11/djlds/util.py
+-rw-rw-rw-   0        0        0     1240 2020-03-20 08:22:22.000000 djlds-2023.5.11/djlds/xlsx_util.py
+-rw-rw-rw-   0        0        0      656 2019-12-09 05:46:20.000000 djlds-2023.5.11/djlds/__about__.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 23:22:44.000000 djlds-2023.5.11/djlds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 06:31:54.000000 djlds-2023.5.11/djlds.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-12-09 09:34:28.000000 djlds-2023.5.11/djlds.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     1359 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      469 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 06:31:53.000000 djlds-2023.5.11/djlds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-12-09 06:34:14.000000 djlds-2023.5.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     1359 2023-05-11 06:31:54.000000 djlds-2023.5.11/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2019-12-09 06:31:13.000000 djlds-2023.5.11/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 06:31:54.000000 djlds-2023.5.11/setup.cfg
+-rw-rw-rw-   0        0        0     2916 2023-05-11 06:23:49.000000 djlds-2023.5.11/setup.py
```

### Comparing `djlds-2022.5.23/djlds/admin.py` & `djlds-2023.5.11/djlds/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 import csv
 
 from ilds.file import human_size
 
 from django.contrib import admin
 from django.contrib import messages
-from django.utils.http import urlquote
+from urllib.parse import quote as urlquote
+
 from django.http import HttpResponse
 from django.db.models import Sum
 
 from djlds.model import ModelFields
 
 
 class ExportCsvMixin:
```

### Comparing `djlds-2022.5.23/djlds/import_export.py` & `djlds-2023.5.11/djlds/import_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # ---------------------------------------
 #   程序：import_export.py
-#   版本：0.7
+#   版本：0.8
 #   作者：lds
-#   日期：2022-04-15
+#   日期：2022-05-11
 #   语言：Python 3.X
 #   说明：django 导入和导出
 # ---------------------------------------
 
 import csv
 import time
 from pathlib import Path
 
+from django.db import transaction
 # 获取模型实例的字典
 from django.forms.models import model_to_dict
-from django.db import transaction
-from ilds.excel_xlsx import ReadXlsx
 from ilds.excel_xlrd import ReadXlsx as ReadXls
+from ilds.excel_xlsx import ReadXlsx
 
 from djlds.model import ModelFields, get_field_file_path, ModelData, TableData
 
 
 class BaseImportExcel:
     """
     导入 Excel 的基础类
@@ -108,19 +108,21 @@
                 del data[field]
 
     def parsing_boolean(self, field, data):
         """
         解析布尔字段
         """
         if field in data:
-            v = data[field]
-            if v in ['True', '有', ]:
+            v = str(data[field]).lower()
+            if v in ['true', '有', '是', ]:
                 data[field] = True
-            elif v in ['False', ]:
+            elif v in ['false', '无', '否', ] or not v:
                 data[field] = False
+            elif v in ['none', '未知', ]:
+                data[field] = None
 
     def get_revised(self):
         """
         需要修正的标题
         """
         return {}
 
@@ -132,14 +134,15 @@
 
     def init_title(self, datasets):
         """
         初始化标题
         """
         self.titles = next(datasets)
         ret = self.table.set_title(self.titles, exclude=self.exclude, **self.revised)
+        # print('set_title', self.titles, self.exclude, self.revised)
         if any([data['Name'] for data in ret]):
             print([data['Name'] for data in ret])
             raise ValueError(f'没有匹配的字段：{ret}')
         if self.table.duplicate_info:
             raise ValueError(f'重复的字段：{self.table.duplicate_info}')
         if self.debug:
             print(self.table.table_fields)
```

### Comparing `djlds-2022.5.23/djlds/management/commands/admin_generator.py` & `djlds-2023.5.11/djlds/management/commands/admin_generator.py`

 * *Files identical despite different names*

### Comparing `djlds-2022.5.23/djlds/model.py` & `djlds-2023.5.11/djlds/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #   作者：lds
 #   日期：2022-05-23
 #   语言：Python 3.X
 #   说明：django 模型相关的函数
 # ---------------------------------------
 
 import operator
+import os
 from functools import reduce
 # from collections import OrderedDict
 
 from colorama import Fore, Back, Style
 
 # from django.forms.models import model_to_dict  # 获取模型实例的字典
 from django.db.models.base import ModelBase, Model
@@ -20,14 +21,15 @@
 from django.apps import apps
 from django.db import models
 # group_by 这个分组 我喜欢
 from django.db.models import Aggregate, Avg, Count, Max, Min, StdDev, Sum, Variance
 from django.db.models import QuerySet
 # # from django.db.models import FileField
 from django.db.models import Sum
+from django.forms.models import model_to_dict
 
 from djlds.xlsx_util import xl_col_to_name
 
 """
 20181203 添加 搜索多个字段的函数
 20181203 ModelFields 添加 获取模型对象
 20181203 添加了获取模型的字段，名字和类型的类
@@ -609,7 +611,33 @@
             return
     except ModuleNotFoundError:
         from djlds.util import confirm_yes_no
         if confirm_yes_no(title=title, text=f'正在修改数据库({name})，是否继续？\n输入 y 确认，其他任意字符表示取消'):
             print(f'{Fore.MAGENTA}{message}({name}){Style.RESET_ALL}')
             return
     exit(f'退出程序，不修改数据库({name})！')
+
+
+def sync_model(model, src, dst, fields=None, exclude=None, is_clear=False):
+    """
+    同步模型数据
+    :param model:
+    :param src:
+    :param dst:
+    :param fields:
+    :param exclude:
+    :param is_clear:
+    :return:
+    """
+
+    load_list = []
+
+    for obj in model.objects.using(src).all():
+        kwargs = model_to_dict(obj, fields=fields, exclude=exclude)
+        load_list.append(model(**kwargs))
+
+    if load_list:
+        if is_clear:
+            print('删除数据', model.objects.using(dst).all().delete())
+        print('成功导入 %s 行' % len(model.objects.using(dst).bulk_create(load_list)))
+    else:
+        print('没有数据导入！')
```

### Comparing `djlds-2022.5.23/djlds/user.py` & `djlds-2023.5.11/djlds/user.py`

 * *Files identical despite different names*

### Comparing `djlds-2022.5.23/djlds/util.py` & `djlds-2023.5.11/djlds/util.py`

 * *Files identical despite different names*

### Comparing `djlds-2022.5.23/djlds/xlsx_util.py` & `djlds-2023.5.11/djlds/xlsx_util.py`

 * *Files identical despite different names*

### Comparing `djlds-2022.5.23/djlds/__about__.py` & `djlds-2023.5.11/djlds/__about__.py`

 * *Files identical despite different names*

### Comparing `djlds-2022.5.23/djlds.egg-info/PKG-INFO` & `djlds-2023.5.11/djlds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djlds
-Version: 2022.5.23
+Version: 2023.5.11
 Summary: 常用 Django 功能集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/django-utils-lds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/django-utils-lds
 Description: # django-utils-lds
```

### Comparing `djlds-2022.5.23/PKG-INFO` & `djlds-2023.5.11/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djlds
-Version: 2022.5.23
+Version: 2023.5.11
 Summary: 常用 Django 功能集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/django-utils-lds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/django-utils-lds
 Description: # django-utils-lds
```

### Comparing `djlds-2022.5.23/setup.py` & `djlds-2023.5.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿import os
 import sys
 
 from setuptools import setup, find_packages
 
-version = '2022.5.23'
+version = '2023.5.11'
 
 """
 pip install -U spider-utils
 pip --no-cache-dir install -U spider-utils
 
 # 检查错误
 # twine check dist/*
```

