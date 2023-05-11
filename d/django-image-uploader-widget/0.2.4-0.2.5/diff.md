# Comparing `tmp/django-image-uploader-widget-0.2.4.tar.gz` & `tmp/django-image-uploader-widget-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-image-uploader-widget-0.2.4.tar", last modified: Thu Apr  6 00:17:35 2023, max compression
+gzip compressed data, was "django-image-uploader-widget-0.2.5.tar", last modified: Thu May 11 17:10:41 2023, max compression
```

## Comparing `django-image-uploader-widget-0.2.4.tar` & `django-image-uploader-widget-0.2.5.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-06 00:17:35.000000 django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-06 00:17:35.000000 django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 00:17:35.000000 django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 00:17:35.000000 django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 00:17:35.000000 django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.749662 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.749662 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.749662 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.749662 django-image-uploader-widget-0.2.4/image_uploader_widget/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.749662 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/css/
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/css/image-uploader-inline.css
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/css/image-uploader-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13895 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/js/image-uploader-inline.js
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/js/image-uploader-modal.js
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/js/image-uploader-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.749662 django-image-uploader-widget-0.2.4/image_uploader_widget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/templates/admin/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/templates/admin/edit_inline/image_uploader.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/image_uploader_widget/templates/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/image_uploader_widget/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 00:17:35.753661 django-image-uploader-widget-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-06 00:17:26.000000 django-image-uploader-widget-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.049371 django-image-uploader-widget-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-11 17:10:41.049371 django-image-uploader-widget-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-11 17:10:41.000000 django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-11 17:10:41.000000 django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:10:41.000000 django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 17:10:40.000000 django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 17:10:41.000000 django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.045371 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.045371 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.045371 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.045371 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/css/image-uploader-inline.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/css/image-uploader-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.045371 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13895 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/js/image-uploader-inline.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/js/image-uploader-modal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/js/image-uploader-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.041371 django-image-uploader-widget-0.2.5/image_uploader_widget/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.045371 django-image-uploader-widget-0.2.5/image_uploader_widget/templates/admin/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/templates/admin/edit_inline/image_uploader.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 17:10:41.049371 django-image-uploader-widget-0.2.5/image_uploader_widget/templates/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/image_uploader_widget/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 17:10:41.049371 django-image-uploader-widget-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-11 17:10:28.000000 django-image-uploader-widget-0.2.5/setup.py
```

### Comparing `django-image-uploader-widget-0.2.4/LICENSE` & `django-image-uploader-widget-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/PKG-INFO` & `django-image-uploader-widget-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-image-uploader-widget
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simple Image Uploader Widget for Django-Admin
 Home-page: https://github.com/inventare/django-image-uploader-widget
 Author: Eduardo Oliveira
 Author-email: eduardo_y05@outlook.com
 License: MIT
 Keywords: django,admin,widget,image,uploader
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-image-uploader-widget-0.2.4/README.md` & `django-image-uploader-widget-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/PKG-INFO` & `django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-image-uploader-widget
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simple Image Uploader Widget for Django-Admin
 Home-page: https://github.com/inventare/django-image-uploader-widget
 Author: Eduardo Oliveira
 Author-email: eduardo_y05@outlook.com
 License: MIT
 Keywords: django,admin,widget,image,uploader
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-image-uploader-widget-0.2.4/django_image_uploader_widget.egg-info/SOURCES.txt` & `django-image-uploader-widget-0.2.5/django_image_uploader_widget.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 image_uploader_widget/__init__.py
 image_uploader_widget/admin.py
 image_uploader_widget/widgets.py
 image_uploader_widget/locale/es/LC_MESSAGES/django.mo
 image_uploader_widget/locale/es/LC_MESSAGES/django.po
 image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo
 image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.po
+image_uploader_widget/locale/ru/LC_MESSAGES/django.mo
+image_uploader_widget/locale/ru/LC_MESSAGES/django.po
 image_uploader_widget/static/admin/css/image-uploader-inline.css
 image_uploader_widget/static/admin/css/image-uploader-widget.css
 image_uploader_widget/static/admin/js/image-uploader-inline.js
 image_uploader_widget/static/admin/js/image-uploader-modal.js
 image_uploader_widget/static/admin/js/image-uploader-widget.js
 image_uploader_widget/templates/admin/edit_inline/image_uploader.html
 image_uploader_widget/templates/admin/widgets/image_uploader_widget.html
```

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/admin.py` & `django-image-uploader-widget-0.2.5/image_uploader_widget/admin.py`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/locale/es/LC_MESSAGES/django.mo` & `django-image-uploader-widget-0.2.5/image_uploader_widget/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/locale/es/LC_MESSAGES/django.po` & `django-image-uploader-widget-0.2.5/image_uploader_widget/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo` & `django-image-uploader-widget-0.2.5/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.po` & `django-image-uploader-widget-0.2.5/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/css/image-uploader-inline.css` & `django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/css/image-uploader-inline.css`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/css/image-uploader-widget.css` & `django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/css/image-uploader-widget.css`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/js/image-uploader-inline.js` & `django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/js/image-uploader-inline.js`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/js/image-uploader-modal.js` & `django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/js/image-uploader-modal.js`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/static/admin/js/image-uploader-widget.js` & `django-image-uploader-widget-0.2.5/image_uploader_widget/static/admin/js/image-uploader-widget.js`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/templates/admin/edit_inline/image_uploader.html` & `django-image-uploader-widget-0.2.5/image_uploader_widget/templates/admin/edit_inline/image_uploader.html`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html` & `django-image-uploader-widget-0.2.5/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/image_uploader_widget/widgets.py` & `django-image-uploader-widget-0.2.5/image_uploader_widget/widgets.py`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.2.4/setup.py` & `django-image-uploader-widget-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 f = open(os.path.join(os.path.dirname(__file__), 'README.md'))
 readme = f.read()
 f.close()
 
 setup(
     name='django-image-uploader-widget',
-    version='0.2.4',
+    version='0.2.5',
     description='Simple Image Uploader Widget for Django-Admin',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Eduardo Oliveira',
     author_email='eduardo_y05@outlook.com',
     url='https://github.com/inventare/django-image-uploader-widget',
     license='MIT',
```

