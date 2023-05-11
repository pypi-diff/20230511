# Comparing `tmp/django-dprog-jfu-2.2.4.tar.gz` & `tmp/django-dprog-jfu-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dprog-jfu-2.2.4.tar", last modified: Sat Sep  5 19:27:47 2020, max compression
+gzip compressed data, was "django-dprog-jfu-3.0.0.tar", last modified: Thu May 11 13:02:29 2023, max compression
```

## Comparing `django-dprog-jfu-2.2.4.tar` & `django-dprog-jfu-3.0.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1505 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/LICENSE
--rw-r--r--   0 philippe  (1000) philippe  (1000)     7693 2020-09-05 19:27:10.000000 django-dprog-jfu-2.2.4/README.rst
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1038 2020-09-05 16:39:43.000000 django-dprog-jfu-2.2.4/setup.py
--rw-r--r--   0 philippe  (1000) philippe  (1000)      384 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/CHANGELOG
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1972 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/http.py
--rw-r--r--   0 philippe  (1000) philippe  (1000)      144 2020-09-05 16:39:43.000000 django-dprog-jfu-2.2.4/jfu/__init__.py
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/templatetags/
--rw-r--r--   0 philippe  (1000) philippe  (1000)        0 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/templatetags/__init__.py
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1165 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/templatetags/jfutags.py
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/templates/
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/templates/jfu/
--rw-r--r--   0 philippe  (1000) philippe  (1000)    16253 2020-09-05 16:42:43.000000 django-dprog-jfu-2.2.4/jfu/templates/jfu/upload_form.html
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/locale/
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/locale/fr/
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/locale/fr/LC_MESSAGES/
--rw-r--r--   0 philippe  (1000) philippe  (1000)      686 2018-05-07 19:46:54.000000 django-dprog-jfu-2.2.4/jfu/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1165 2018-05-07 19:46:11.000000 django-dprog-jfu-2.2.4/jfu/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/img/
--rw-r--r--   0 philippe  (1000) philippe  (1000)     2216 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/img/error.png
--rw-r--r--   0 philippe  (1000) philippe  (1000)     3897 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/img/loading.gif
--rw-r--r--   0 philippe  (1000) philippe  (1000)      306 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/img/error.svg
--rw-r--r--   0 philippe  (1000) philippe  (1000)     3323 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/img/progressbar.gif
--rw-r--r--   0 philippe  (1000) philippe  (1000)      274 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/img/video-play.svg
--rw-r--r--   0 philippe  (1000) philippe  (1000)      606 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/img/play-pause.png
--rw-r--r--   0 philippe  (1000) philippe  (1000)     2811 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/img/video-play.png
--rw-r--r--   0 philippe  (1000) philippe  (1000)      382 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/img/play-pause.svg
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/css/
--rw-r--r--   0 philippe  (1000) philippe  (1000)      285 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/css/style.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1115 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/css/jquery-ui-demo.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)      682 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/css/jquery.fileupload.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)      387 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/css/jquery-ui-demo-ie8.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1093 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/css/jquery.fileupload-ui.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)      433 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/css/jquery.fileupload-noscript.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)      362 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/css/jquery.fileupload-ui-noscript.css
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/demo/
--rw-r--r--   0 philippe  (1000) philippe  (1000)     2072 2018-03-28 15:20:38.000000 django-dprog-jfu-2.2.4/jfu/static/demo/jquery.blueimp-gallery.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     5706 2018-03-28 15:20:38.000000 django-dprog-jfu-2.2.4/jfu/static/demo/blueimp-gallery.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)    32556 2018-03-28 15:20:38.000000 django-dprog-jfu-2.2.4/jfu/static/demo/jquery.blueimp-gallery.min.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)      977 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/demo/tmpl.min.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     7288 2018-03-28 15:20:38.000000 django-dprog-jfu-2.2.4/jfu/static/demo/blueimp-gallery.min.css
--rw-r--r--   0 philippe  (1000) philippe  (1000)     1028 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/demo/canvas-to-blob.min.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)    16315 2018-05-06 19:04:28.000000 django-dprog-jfu-2.2.4/jfu/static/demo/load-image.min.js
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/js/
--rw-r--r--   0 philippe  (1000) philippe  (1000)    64004 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)    12299 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-image.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     5272 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-jquery-ui.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     2474 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/main.js
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/js/vendor/
--rw-r--r--   0 philippe  (1000) philippe  (1000)    22644 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/vendor/jquery.ui.widget.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     4248 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-validate.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)    17101 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-angular.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     3604 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-audio.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     6161 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-process.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     3579 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/app.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     3604 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-video.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)    28065 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-ui.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)    10891 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/jquery.iframe-transport.js
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/js/cors/
--rw-r--r--   0 philippe  (1000) philippe  (1000)     3414 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/cors/jquery.xdr-transport.js
--rw-r--r--   0 philippe  (1000) philippe  (1000)     4470 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/js/cors/jquery.postmessage-transport.js
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/jfu/static/cors/
--rw-r--r--   0 philippe  (1000) philippe  (1000)     2046 2018-05-07 20:12:33.000000 django-dprog-jfu-2.2.4/jfu/static/cors/postmessage.html
--rw-r--r--   0 philippe  (1000) philippe  (1000)      528 2018-02-19 12:12:29.000000 django-dprog-jfu-2.2.4/jfu/static/cors/result.html
--rw-rw-r--   0 philippe  (1000) philippe  (1000)       38 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/setup.cfg
-drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/django_dprog_jfu.egg-info/
--rw-rw-r--   0 philippe  (1000) philippe  (1000)        4 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/django_dprog_jfu.egg-info/top_level.txt
--rw-rw-r--   0 philippe  (1000) philippe  (1000)     1813 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/django_dprog_jfu.egg-info/SOURCES.txt
--rw-rw-r--   0 philippe  (1000) philippe  (1000)        1 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/django_dprog_jfu.egg-info/dependency_links.txt
--rw-rw-r--   0 philippe  (1000) philippe  (1000)    10543 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/django_dprog_jfu.egg-info/PKG-INFO
--rw-rw-r--   0 philippe  (1000) philippe  (1000)    10543 2020-09-05 19:27:47.000000 django-dprog-jfu-2.2.4/PKG-INFO
--rw-r--r--   0 philippe  (1000) philippe  (1000)      149 2018-05-07 20:54:30.000000 django-dprog-jfu-2.2.4/MANIFEST.in
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      438 2023-05-11 10:54:10.000000 django-dprog-jfu-3.0.0/CHANGELOG
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1536 2023-05-11 12:57:56.000000 django-dprog-jfu-3.0.0/LICENSE
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      149 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/MANIFEST.in
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     8496 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     7693 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/README.rst
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/django_dprog_jfu.egg-info/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     8496 2023-05-11 13:02:29.000000 django-dprog-jfu-3.0.0/django_dprog_jfu.egg-info/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1813 2023-05-11 13:02:29.000000 django-dprog-jfu-3.0.0/django_dprog_jfu.egg-info/SOURCES.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)        1 2023-05-11 13:02:29.000000 django-dprog-jfu-3.0.0/django_dprog_jfu.egg-info/dependency_links.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)        4 2023-05-11 13:02:29.000000 django-dprog-jfu-3.0.0/django_dprog_jfu.egg-info/top_level.txt
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      162 2023-05-11 12:57:56.000000 django-dprog-jfu-3.0.0/jfu/__init__.py
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1893 2023-05-11 10:58:22.000000 django-dprog-jfu-3.0.0/jfu/http.py
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/locale/
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/locale/fr/
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      686 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1165 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/static/
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/static/cors/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     2046 2023-05-11 10:49:33.000000 django-dprog-jfu-3.0.0/jfu/static/cors/postmessage.html
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      528 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/cors/result.html
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/static/css/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      387 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/css/jquery-ui-demo-ie8.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1115 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/css/jquery-ui-demo.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      433 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/css/jquery.fileupload-noscript.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      362 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/css/jquery.fileupload-ui-noscript.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1093 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/css/jquery.fileupload-ui.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      682 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/css/jquery.fileupload.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      285 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/css/style.css
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/static/demo/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     5706 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/demo/blueimp-gallery.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     7237 2023-05-11 11:24:42.000000 django-dprog-jfu-3.0.0/jfu/static/demo/blueimp-gallery.min.css
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1028 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/demo/canvas-to-blob.min.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     2072 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/demo/jquery.blueimp-gallery.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    32502 2023-05-11 11:24:42.000000 django-dprog-jfu-3.0.0/jfu/static/demo/jquery.blueimp-gallery.min.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    16315 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/demo/load-image.min.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      977 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/demo/tmpl.min.js
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/static/img/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     2216 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/error.png
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      306 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/error.svg
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     3897 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/loading.gif
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      606 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/play-pause.png
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      382 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/play-pause.svg
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     3323 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/progressbar.gif
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     2811 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/video-play.png
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      274 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/img/video-play.svg
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/jfu/static/js/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     3579 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/app.js
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/jfu/static/js/cors/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     4470 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/cors/jquery.postmessage-transport.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     3414 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/cors/jquery.xdr-transport.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    17101 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-angular.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     3604 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-audio.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    12299 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-image.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     5272 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-jquery-ui.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     6161 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-process.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    28065 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-ui.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     4248 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-validate.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     3604 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-video.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    64004 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    10891 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/jquery.iframe-transport.js
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     2474 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/main.js
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/jfu/static/js/vendor/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    22644 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/static/js/vendor/jquery.ui.widget.js
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.402607 django-dprog-jfu-3.0.0/jfu/templates/
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/jfu/templates/jfu/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)    16253 2023-05-11 10:49:22.000000 django-dprog-jfu-3.0.0/jfu/templates/jfu/upload_form.html
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/jfu/templatetags/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)        0 2023-05-11 10:47:25.000000 django-dprog-jfu-3.0.0/jfu/templatetags/__init__.py
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1139 2023-05-11 10:55:52.000000 django-dprog-jfu-3.0.0/jfu/templatetags/jfutags.py
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       38 2023-05-11 13:02:29.406607 django-dprog-jfu-3.0.0/setup.cfg
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      991 2023-05-11 10:55:52.000000 django-dprog-jfu-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-dprog-jfu-2.2.4/LICENSE` & `django-dprog-jfu-3.0.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2008-2013 by Alem (http://www.alemcode.com)
+Copyright © 2008-2013 by Alem (http://www.alemcode.com), 2016-2023 by Philippe Docourt
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
  * Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
```

### Comparing `django-dprog-jfu-2.2.4/README.rst` & `django-dprog-jfu-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/http.py` & `django-dprog-jfu-3.0.0/jfu/http.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 import json
 from django.http import HttpResponse
 
 
-def upload_receive( request ):
+def upload_receive(request):
     """
     Returns the file(s) uploaded by the user.
     """
-    return request.FILES['files[]'] if request.FILES else None
+    return request.FILES["files[]"] if request.FILES else None
 
 
-class JFUResponse( HttpResponse ):
+class JFUResponse(HttpResponse):
     """
     Returns an HTTP response with its data encoded in JSON format.
 
-    Content-Type negotation is handled transparently by inspecting the
+    Content-Type negotiation is handled transparently by inspecting the
     request object. If the client accepts JSON, the MIME-type of the response
     is set to JSON. Otherwise, the MIME-type defaults to 'text/plain'.
 
-    This approach suports jQuery File Upload's use of an Iframe Transport
+    This approach supports jQuery File Upload's use of an Iframe Transport
     module for the browsers (IE & Opera) incapable of handling XmlHttpRequest
     file uploads and who present download dialogs for iFrame responses that
     declare a JSON MIME-type.
     """
 
-    def __init__( self, request, data = True, *args, **kwargs ):
-        data   = json.dumps( data )
-        j      = "application/json"
-        accept = request.META.get('HTTP_ACCEPT')
+    def __init__(self, request, data=True, *args, **kwargs):
+        data = json.dumps(data)
+        j = "application/json"
+        accept = request.META.get("HTTP_ACCEPT")
 
-        mime = j if accept and j in accept else 'text/plain'
+        mime = j if accept and j in accept else "text/plain"
 
-        super( JFUResponse, self ).__init__( data, mime, *args, **kwargs )
-    
+        super().__init__(data, mime, *args, **kwargs)
 
-class UploadResponse( JFUResponse ):
+
+class UploadResponse(JFUResponse):
     """
     Takes a dictionary containing the required jQuery File Upload fileupload
     response data and returns a JFUResponse.
 
     The dictionary may take the following form:
     {
-       'name': 'file name', 
+       'name': 'file name',
        'size': 12345,
-       'url' : 'file url', 
+       'url' : 'file url',
        'thumbnailUrl': 'thumbnail url',
        'deleteUrl'   : 'delete url',
-       'deleteType'  : 'delete type', 
+       'deleteType'  : 'delete type',
     }
 
     Refer to the jQuery File Upload documentation for acceptable response data.
     [https://github.com/blueimp/jQuery-File-Upload/wiki/Setup]
     """
 
-    def __init__( self, request, file_dict, *args, **kwargs ):
-        files = file_dict if isinstance( file_dict, list ) else [ file_dict ]
-        data  = { 'files' : files }
-        super( UploadResponse, self ).__init__( request, data, *args, **kwargs )
+    def __init__(self, request, file_dict, *args, **kwargs):
+        files = file_dict if isinstance(file_dict, list) else [file_dict]
+        data = {"files": files}
+        super().__init__(request, data, *args, **kwargs)
```

### Comparing `django-dprog-jfu-2.2.4/jfu/templatetags/jfutags.py` & `django-dprog-jfu-3.0.0/jfu/templatetags/jfutags.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,39 +2,34 @@
 from django.urls import reverse
 from django.template import Library, loader
 
 register = Library()
 
 
 @register.simple_tag(takes_context=True)
-def jfu(
-        context,
-        template_name='jfu/upload_form.html',
-        upload_handler_name='jfu_upload',
-        *args, **kwargs
-):
+def jfu(context, template_name="jfu/upload_form.html", upload_handler_name="jfu_upload", *args, **kwargs):
     """
     Displays a form for uploading files using jQuery File Upload.
 
     A user may use both a custom template or a custom upload-handling URL
     name by supplying values for template_name and upload_handler_name
     respectively.
 
     Any additionally supplied positional and keyword arguments are directly
     forwarded to the named custom upload-handling URL.
     """
-    context.update({
-        'JQ_OPEN': '{%',
-        'JQ_CLOSE': '%}',
-        'upload_handler_url': reverse(
-            upload_handler_name, args=args, kwargs=kwargs
-        ),
-    })
+    context.update(
+        {
+            "JQ_OPEN": "{%",
+            "JQ_CLOSE": "%}",
+            "upload_handler_url": reverse(upload_handler_name, args=args, kwargs=kwargs),
+        }
+    )
 
     # Use the request context variable, injected
     # by django.core.context_processors.request,
     # to generate the CSRF token.
-    context.update(csrf(context.get('request')))
+    context.update(csrf(context.get("request")))
 
     t = loader.get_template(template_name)
 
     return t.render(context.flatten())
```

### Comparing `django-dprog-jfu-2.2.4/jfu/templates/jfu/upload_form.html` & `django-dprog-jfu-3.0.0/jfu/templates/jfu/upload_form.html`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
 
 {% block JS_SCRIPTS %}
 {% block JS_JQUERY %}
 {% comment %}
  jQuery
 {% endcomment %}
-<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
+<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.4/jquery.min.js"></script>
 {% endblock %}
 
 {% block JS_JQUERY_UI_WIDGET %}
 {% comment %}
  The jQuery UI widget factory, can be omitted if jQuery UI is already included
 {% endcomment %}
 <script src="{% static 'js/vendor/jquery.ui.widget.js' %}"></script>
```

### Comparing `django-dprog-jfu-2.2.4/jfu/locale/fr/LC_MESSAGES/django.mo` & `django-dprog-jfu-3.0.0/jfu/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/locale/fr/LC_MESSAGES/django.po` & `django-dprog-jfu-3.0.0/jfu/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/img/error.png` & `django-dprog-jfu-3.0.0/jfu/static/img/error.png`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/img/loading.gif` & `django-dprog-jfu-3.0.0/jfu/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/img/progressbar.gif` & `django-dprog-jfu-3.0.0/jfu/static/img/progressbar.gif`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/img/play-pause.png` & `django-dprog-jfu-3.0.0/jfu/static/img/play-pause.png`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/img/video-play.png` & `django-dprog-jfu-3.0.0/jfu/static/img/video-play.png`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/css/jquery-ui-demo.css` & `django-dprog-jfu-3.0.0/jfu/static/css/jquery-ui-demo.css`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/css/jquery.fileupload.css` & `django-dprog-jfu-3.0.0/jfu/static/css/jquery.fileupload.css`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/css/jquery.fileupload-ui.css` & `django-dprog-jfu-3.0.0/jfu/static/css/jquery.fileupload-ui.css`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/demo/jquery.blueimp-gallery.js` & `django-dprog-jfu-3.0.0/jfu/static/demo/jquery.blueimp-gallery.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/demo/blueimp-gallery.css` & `django-dprog-jfu-3.0.0/jfu/static/demo/blueimp-gallery.css`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/demo/jquery.blueimp-gallery.min.js` & `django-dprog-jfu-3.0.0/jfu/static/demo/jquery.blueimp-gallery.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -809,9 +809,8 @@
                 container: o[0],
                 index: this,
                 event: i
             }, a),
             r = t(this).closest("[data-gallery-group], body").find('[data-gallery="' + s + '"]');
         return l.filter && (r = r.filter(l.filter)), new e(r, l)
     })
-});
-//# sourceMappingURL=jquery.blueimp-gallery.min.js.map
+});
```

### Comparing `django-dprog-jfu-2.2.4/jfu/static/demo/tmpl.min.js` & `django-dprog-jfu-3.0.0/jfu/static/demo/tmpl.min.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/demo/blueimp-gallery.min.css` & `django-dprog-jfu-3.0.0/jfu/static/demo/blueimp-gallery.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,2 +1 @@
 @charset "UTF-8";.blueimp-gallery,.blueimp-gallery>.slides>.slide>.slide-content{position:absolute;top:0;right:0;bottom:0;left:0;-moz-backface-visibility:hidden}.blueimp-gallery>.slides>.slide>.slide-content{margin:auto;width:auto;height:auto;max-width:100%;max-height:100%;opacity:1}.blueimp-gallery{position:fixed;z-index:999999;overflow:hidden;background:#000;background:rgba(0,0,0,.9);opacity:0;display:none;direction:ltr;-ms-touch-action:none;touch-action:none}.blueimp-gallery-carousel{position:relative;z-index:auto;margin:1em auto;padding-bottom:56.25%;box-shadow:0 0 10px #000;-ms-touch-action:pan-y;touch-action:pan-y}.blueimp-gallery-display{display:block;opacity:1}.blueimp-gallery>.slides{position:relative;height:100%;overflow:hidden}.blueimp-gallery-carousel>.slides{position:absolute}.blueimp-gallery>.slides>.slide{position:relative;float:left;height:100%;text-align:center;-webkit-transition-timing-function:cubic-bezier(.645,.045,.355,1);-moz-transition-timing-function:cubic-bezier(.645,.045,.355,1);-ms-transition-timing-function:cubic-bezier(.645,.045,.355,1);-o-transition-timing-function:cubic-bezier(.645,.045,.355,1);transition-timing-function:cubic-bezier(.645,.045,.355,1)}.blueimp-gallery,.blueimp-gallery>.slides>.slide>.slide-content{-webkit-transition:opacity .2s linear;-moz-transition:opacity .2s linear;-ms-transition:opacity .2s linear;-o-transition:opacity .2s linear;transition:opacity .2s linear}.blueimp-gallery>.slides>.slide-loading{background:url(../img/loading.gif) center no-repeat;background-size:64px 64px}.blueimp-gallery>.slides>.slide-loading>.slide-content{opacity:0}.blueimp-gallery>.slides>.slide-error{background:url(../img/error.png) center no-repeat}.blueimp-gallery>.slides>.slide-error>.slide-content{display:none}.blueimp-gallery>.next,.blueimp-gallery>.prev{position:absolute;top:50%;left:15px;width:40px;height:40px;margin-top:-23px;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:60px;font-weight:100;line-height:30px;color:#fff;text-decoration:none;text-shadow:0 0 2px #000;text-align:center;background:#222;background:rgba(0,0,0,.5);-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;border:3px solid #fff;-webkit-border-radius:23px;-moz-border-radius:23px;border-radius:23px;opacity:.5;cursor:pointer;display:none}.blueimp-gallery>.next{left:auto;right:15px}.blueimp-gallery>.close,.blueimp-gallery>.title{position:absolute;top:15px;left:15px;margin:0 40px 0 0;font-size:20px;line-height:30px;color:#fff;text-shadow:0 0 2px #000;opacity:.8;display:none}.blueimp-gallery>.close{padding:15px;right:15px;left:auto;margin:-15px;font-size:30px;text-decoration:none;cursor:pointer}.blueimp-gallery>.play-pause{position:absolute;right:15px;bottom:15px;width:15px;height:15px;background:url(../img/play-pause.png) 0 0 no-repeat;cursor:pointer;opacity:.5;display:none}.blueimp-gallery-playing>.play-pause{background-position:-15px 0}.blueimp-gallery>.close:hover,.blueimp-gallery>.next:hover,.blueimp-gallery>.play-pause:hover,.blueimp-gallery>.prev:hover,.blueimp-gallery>.title:hover{color:#fff;opacity:1}.blueimp-gallery-controls>.close,.blueimp-gallery-controls>.next,.blueimp-gallery-controls>.play-pause,.blueimp-gallery-controls>.prev,.blueimp-gallery-controls>.title{display:block;-webkit-transform:translateZ(0);-moz-transform:translateZ(0);-ms-transform:translateZ(0);-o-transform:translateZ(0);transform:translateZ(0)}.blueimp-gallery-left>.prev,.blueimp-gallery-right>.next,.blueimp-gallery-single>.next,.blueimp-gallery-single>.play-pause,.blueimp-gallery-single>.prev{display:none}.blueimp-gallery>.close,.blueimp-gallery>.next,.blueimp-gallery>.play-pause,.blueimp-gallery>.prev,.blueimp-gallery>.slides>.slide>.slide-content{-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}body:last-child .blueimp-gallery>.slides>.slide-error{background-image:url(../img/error.svg)}body:last-child .blueimp-gallery>.play-pause{width:20px;height:20px;background-size:40px 20px;background-image:url(../img/play-pause.svg)}body:last-child .blueimp-gallery-playing>.play-pause{background-position:-20px 0}*+html .blueimp-gallery>.slides>.slide{min-height:300px}*+html .blueimp-gallery>.slides>.slide>.slide-content{position:relative}.blueimp-gallery>.indicator{position:absolute;top:auto;right:15px;bottom:15px;left:15px;margin:0 40px;padding:0;list-style:none;text-align:center;line-height:10px;display:none}.blueimp-gallery>.indicator>li{display:inline-block;width:9px;height:9px;margin:6px 3px 0 3px;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;border:1px solid transparent;background:#ccc;background:rgba(255,255,255,.25) center no-repeat;border-radius:5px;box-shadow:0 0 2px #000;opacity:.5;cursor:pointer}.blueimp-gallery>.indicator>.active,.blueimp-gallery>.indicator>li:hover{background-color:#fff;border-color:#fff;opacity:1}.blueimp-gallery>.indicator>li:after{opacity:0;display:block;position:absolute;content:'';top:-5em;width:75px;height:75px;transition:transform .6s ease-out,opacity .4s ease-out;transform:translateX(-50%) translateY(0) translateZ(0);pointer-events:none}.blueimp-gallery>.indicator>li:hover:after{opacity:1;border-radius:50%;background:inherit;transform:translateX(-50%) translateY(-5px) translateZ(0)}.blueimp-gallery>.indicator>.active:after{display:none}.blueimp-gallery-controls>.indicator{display:block;-webkit-transform:translateZ(0);-moz-transform:translateZ(0);-ms-transform:translateZ(0);-o-transform:translateZ(0);transform:translateZ(0)}.blueimp-gallery-single>.indicator{display:none}.blueimp-gallery>.indicator{-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}*+html .blueimp-gallery>.indicator>li{display:inline}.blueimp-gallery>.slides>.slide>.video-content>img{position:absolute;top:0;right:0;bottom:0;left:0;margin:auto;width:auto;height:auto;max-width:100%;max-height:100%;-moz-backface-visibility:hidden}.blueimp-gallery>.slides>.slide>.video-content>video{position:absolute;top:0;left:0;width:100%;height:100%}.blueimp-gallery>.slides>.slide>.video-content>iframe{position:absolute;top:100%;left:0;width:100%;height:100%;border:none}.blueimp-gallery>.slides>.slide>.video-playing>iframe{top:0}.blueimp-gallery>.slides>.slide>.video-content>a{position:absolute;top:50%;right:0;left:0;margin:-64px auto 0;width:128px;height:128px;background:url(../img/video-play.png) center no-repeat;opacity:.8;cursor:pointer}.blueimp-gallery>.slides>.slide>.video-content>a:hover{opacity:1}.blueimp-gallery>.slides>.slide>.video-playing>a,.blueimp-gallery>.slides>.slide>.video-playing>img{display:none}.blueimp-gallery>.slides>.slide>.video-content>video{display:none}.blueimp-gallery>.slides>.slide>.video-playing>video{display:block}.blueimp-gallery>.slides>.slide>.video-loading>a{background:url(../img/loading.gif) center no-repeat;background-size:64px 64px}body:last-child .blueimp-gallery>.slides>.slide>.video-content:not(.video-loading)>a{background-image:url(../img/video-play.svg)}*+html .blueimp-gallery>.slides>.slide>.video-content{height:100%}*+html .blueimp-gallery>.slides>.slide>.video-content>a{left:50%;margin-left:-64px}
-/*# sourceMappingURL=blueimp-gallery.min.css.map */
```

### Comparing `django-dprog-jfu-2.2.4/jfu/static/demo/canvas-to-blob.min.js` & `django-dprog-jfu-3.0.0/jfu/static/demo/canvas-to-blob.min.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/demo/load-image.min.js` & `django-dprog-jfu-3.0.0/jfu/static/demo/load-image.min.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-image.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-image.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-jquery-ui.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-jquery-ui.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/main.js` & `django-dprog-jfu-3.0.0/jfu/static/js/main.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/vendor/jquery.ui.widget.js` & `django-dprog-jfu-3.0.0/jfu/static/js/vendor/jquery.ui.widget.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-validate.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-validate.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-angular.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-angular.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-audio.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-audio.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-process.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-process.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/app.js` & `django-dprog-jfu-3.0.0/jfu/static/js/app.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-video.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-video.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.fileupload-ui.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.fileupload-ui.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/jquery.iframe-transport.js` & `django-dprog-jfu-3.0.0/jfu/static/js/jquery.iframe-transport.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/cors/jquery.xdr-transport.js` & `django-dprog-jfu-3.0.0/jfu/static/js/cors/jquery.xdr-transport.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/js/cors/jquery.postmessage-transport.js` & `django-dprog-jfu-3.0.0/jfu/static/js/cors/jquery.postmessage-transport.js`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/jfu/static/cors/postmessage.html` & `django-dprog-jfu-3.0.0/jfu/static/cors/postmessage.html`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
  * https://opensource.org/licenses/MIT
  */
 -->
 <html lang="en">
 <head>
 <meta charset="utf-8">
 <title>jQuery File Upload Plugin postMessage API</title>
-<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
+<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.4/jquery.min.js"></script>
 </head>
 <body>
 <script>
 /*jslint unparam: true, regexp: true */
 /*global $, Blob, FormData, location */
 'use strict';
 var origin = /^http:\/\/example.org/,
```

### Comparing `django-dprog-jfu-2.2.4/jfu/static/cors/result.html` & `django-dprog-jfu-3.0.0/jfu/static/cors/result.html`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/django_dprog_jfu.egg-info/SOURCES.txt` & `django-dprog-jfu-3.0.0/django_dprog_jfu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dprog-jfu-2.2.4/django_dprog_jfu.egg-info/PKG-INFO` & `django-dprog-jfu-3.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,274 +1,273 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-dprog-jfu
-Version: 2.2.4
+Version: 3.0.0
 Summary: A Django Library for jQuery File Upload.
 Home-page: http://packages.python.org/jfu
-Author: Z. Alem
+Author: Z. Alem, Philippe Docourt
 Author-email: alem@cidola.com
 Maintainer: Philippe Docourt
 License: BSD License
-Description: Note: This project is forked from https://github.com/jpic/django-jfu. This fork aims to localize the project and keep it compatible with recent versions of Django. It also updates some rather obsolete dependencies.
-        
-        ----------------------------------------------------
-        Django-JFU - A Django Library for jQuery File Upload 
-        ----------------------------------------------------
-        
-        Django-JFU is designed to simplify the tasks involved in integrating jQuery
-        File Upload (https://github.com/blueimp/jquery-file-upload) into Django.
-        Django-JFU assumes very little and leaves the model/view design up to the user. 
-        
-        Other Django - jQuery File Upload implementations are full-featured but
-        generally serve more as demonstrations than libraries for existing
-        applications.
-        
-        If you seek a tool to ease the integration of jQuery File Upload into your
-        Django application while still having a great degree of freedom, you may find
-        this package useful.
-        
-        Demo_
-        
-        .. _Demo: http://djfu-demo.cidola.com
-        
-        Installation
-        ------------
-        
-        1. ``pip install django-jfu``.
-        2. Add 'jfu' to ``INSTALLED_APPS`` in your project settings.py file.
-        3. Run `python manage.py collectstatic`.
-        
-        
-        Usage
-        -----
-        
-        Django-JFU provides simple customizable template tags and override-able
-        templates that do the work of integrating the jQuery File Upload CSS and
-        JavaScipt and the HTML implementation found in the jQuery File Upload demo.
-        
-        To place the jQuery File Upload widget in a template, simply insert the
-        following within it::
-            
-            {% load jfutags %}
-            {% jfu %}
-        
-        Then create a view that will handle the uploaded files. 
-        The URL for the view is expected to be named **'jfu_upload'** by default,
-        although this can be customized (see Customization below).
-        
-        Here is an example implementation:
-        
-        In your ``urls.py`` file::
-        
-            ...
-            url( r'upload/', views.upload, name = 'jfu_upload' ),
-        
-            # You may optionally define a delete url as well
-            url( r'^delete/(?P<pk>\d+)$', views.upload_delete, name = 'jfu_delete' ),
-        
-        In your ``views.py`` file::
-            
-            import os
-            from django.conf import settings
-            from django.core.urlresolvers import reverse
-            from django.views import generic
-            from django.views.decorators.http import require_POST
-            from jfu.http import upload_receive, UploadResponse, JFUResponse
-        
-            from YOURAPP.models import YOURMODEL
-        
-            @require_POST
-            def upload( request ):
-        
-                # The assumption here is that jQuery File Upload
-                # has been configured to send files one at a time.
-                # If multiple files can be uploaded simulatenously,
-                # 'file' may be a list of files.
-                file = upload_receive( request )
-        
-                instance = YOURMODEL( file = file )
-                instance.save()
-        
-                basename = os.path.basename( instance.file.path )
-                
-                file_dict = {
-                    'name' : basename,
-                    'size' : file.size,
-        
-                    'url': settings.MEDIA_URL + basename,
-                    'thumbnailUrl': settings.MEDIA_URL + basename,
-        
-                    'deleteUrl': reverse('jfu_delete', kwargs = { 'pk': instance.pk }),
-                    'deleteType': 'POST',
-                }
-        
-                return UploadResponse( request, file_dict )
-        
-            @require_POST
-            def upload_delete( request, pk ):
-                success = True
-                try:
-                    instance = YOURMODEL.objects.get( pk = pk )
-                    os.unlink( instance.file.path )
-                    instance.delete()
-                except YOURMODEL.DoesNotExist:
-                    success = False
-        
-                return JFUResponse( request, success )
-        
-        Customization
-        -------------
-        
-        Django-JFU is designed to be very customizable.  
-        
-        The Django-JFU template tag optionally takes two arguments: the name of the
-        template to load and the name of the URL pointing to the upload-handling
-        view.::
-        
-            {% load jfutags %}
-            {% jfu 'your_fileuploader.html' 'your_uploader_URL_name' %}
-        
-        A custom template can extend from the master Django-JFU template
-        `jfu/upload_form.html`.  There are several blocks which may be overriden for
-        the purpose of customization:
-        
-        * JS_OPTS - The options supplied to the jQuery File Upload ``fileupload`` function. 
-        * JS_INIT - The initializing JavaScript
-        * FILE_INPUT - The file input for the upload form.
-        
-        The blocks above are most-likely what you will want to override when seeking to
-        customize. For instance, one would go about adding a few options to the
-        fileupload function in this manner::
-        
-            # your_fileuploader.html
-            {% extends 'jfu/upload_form.html' %}
-            
-            {% block JS_OPTS %}
-            autoUpload: true,
-            maxNumberOfFiles: 5,
-            sequentialUploads: true,
-            {% endblock %}
-        
-        There are several other blocks too:
-        
-        
-        HTML Components
-        ===============
-        
-        * MODAL_GALLERY - The modal gallery
-        * UPLOAD_FORM   - The file upload form used as target for the file upload widget.
-        
-          * UPLOAD_FORM_LISTING - The table listing the files available for upload/download.
-          * UPLOAD_FORM_LINDICATOR - The loading indicator shown during file processing.
-          * UPLOAD_FORM_PROGRESS_BAR - The global progress information.
-          * UPLOAD_FORM_BUTTON_BAR - The fileupload-buttonbar contains buttons to add/delete files and start/cancel the upload.
-        
-            * UPLOAD_FORM_BUTTON_BAR_CONTROL - Contains buttons to start/cancel the upload or delete files. 
-            * UPLOAD_FORM_BUTTON_BAR_ADD     - Contains the file input used to add files.
-                * FILE_INPUT or UPLOAD_FORM_BUTTON_BAR_ADD_FILE_INPUT - Contains the file input.
-                * UPLOAD_FORM_BUTTON_BAR_ADD_EXTRA - An empty block allowing the addition of extra inputs.
-            * UPLOAD_FORM_BUTTON_BAR_EXTRA  - An empty block allowing the addition of extra components.
-        
-          * UPLOAD_FORM_EXTRA - An empty block allowing the addition of extra components.
-        
-        CSS Components
-        ==============
-        
-        * CSS
-        
-          * CSS_BOOTSTRAP 
-          * CSS_BLUEIMP_GALLERY 
-          * CSS_JQUERY_FILE_UPLOAD
-          * CSS_JQUERY_FILE_UPLOAD_UI
-          * CSS_HTML5_SHIM 
-          * CSS_EXTRA 
-        
-        JS Components
-        =============
-        
-        * JS_TEMPLATES
-        
-          * JS_DOWNLOAD_TEMPLATE
-        
-            * JS_DOWNLOAD_TEMPLATE_DELETE 
-            * JS_DOWNLOAD_TEMPLATE_DOWNLOAD
-            * JS_DOWNLOAD_TEMPLATE_PREVIEW 
-            * JS_DOWNLOAD_TEMPLATE_ERROR 
-            * JS_DOWNLOAD_TEMPLATE_FSIZE
-        
-          * JS_UPLOAD_TEMPLATE
-        
-            * JS_UPLOAD_TEMPLATE_PREVIEW
-            * JS_UPLOAD_TEMPLATE_UPLOAD
-            * JS_UPLOAD_TEMPLATE_CONTROLS
-        
-                * JS_UPLOAD_TEMPLATE_START
-                * JS_UPLOAD_TEMPLATE_CANCEL
-        
-            * JS_UPLOAD_TEMPLATE_PROGRESSBAR
-        
-        * JS_SCRIPTS
-        
-          * JS_JQUERY 
-          * JS_JQUERY_UI_WIDGET
-          * JS_TEMPLATES_PLUGIN
-          * JS_LOAD_IMAGE
-          * JS_CANVAS_TO_BLOB 
-          * JS_BOOTSTRAP 
-          * JS_BLUEIMP_GALLERY 
-          * JS_BOOTSTRAP_IFRAME_TRANSPORT
-          * JS_JQUERY_FILE_UPLOAD
-          * JS_JQUERY_FILE_UPLOAD_FP
-          * JS_JQUERY_FILE_UPLOAD_IMAGE
-          * JS_JQUERY_FILE_UPLOAD_AUDIO
-          * JS_JQUERY_FILE_UPLOAD_VIDEO
-          * JS_JQUERY_FILE_UPLOAD_VALIDATE
-          * JS_JQUERY_FILEUPLOAD_UI 
-          * JS_XDR_TRANSPORT 
-          * JS_EXTRA
-        
-        The included JavaScript and CSS can be updated or suppressed by overriding
-        these blocks ::
-        
-            # your_fileuploader.html
-            {% extends 'jfu/upload_form.html' %}
-        
-            {% block JS_JQUERY %}
-                <script src={{STATIC_URL}}/js/my.newer.jquery.js />
-            {% endblock %}
-        
-            {% block CSS_BOOTSTRAP %}
-                {% comment %}
-                This is already included.
-                {% endcomment %}
-            {% endblock %}
-        
-        or by replacing the static files themselves.
-        
-        Demo
-        ----
-        If you have downloaded from the repository, a simple demo application has been
-        included in the 'demo' directory. 
-        To test it out, enter the 'demo' directory and run ::
-        
-                ./setup && ./run
-        
-        Note that virtualenv is required for the demo to function.
-        
-        Contribution
-        ------------           
-        Django-JFU is wholly open source and welcomes contributions of any kind. Feel
-        free to either extend it, report bugs, or provide suggestions for improvements.
-        The author of Django-JFU can be contacted at alem@cidola.com.
-        
 Keywords: django,jquery file upload,multi-upload
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+Note: This project is forked from https://github.com/jpic/django-jfu. This fork aims to localize the project and keep it compatible with recent versions of Django. It also updates some rather obsolete dependencies.
+
+----------------------------------------------------
+Django-JFU - A Django Library for jQuery File Upload 
+----------------------------------------------------
+
+Django-JFU is designed to simplify the tasks involved in integrating jQuery
+File Upload (https://github.com/blueimp/jquery-file-upload) into Django.
+Django-JFU assumes very little and leaves the model/view design up to the user. 
+
+Other Django - jQuery File Upload implementations are full-featured but
+generally serve more as demonstrations than libraries for existing
+applications.
+
+If you seek a tool to ease the integration of jQuery File Upload into your
+Django application while still having a great degree of freedom, you may find
+this package useful.
+
+Demo_
+
+.. _Demo: http://djfu-demo.cidola.com
+
+Installation
+------------
+
+1. ``pip install django-jfu``.
+2. Add 'jfu' to ``INSTALLED_APPS`` in your project settings.py file.
+3. Run `python manage.py collectstatic`.
+
+
+Usage
+-----
+
+Django-JFU provides simple customizable template tags and override-able
+templates that do the work of integrating the jQuery File Upload CSS and
+JavaScipt and the HTML implementation found in the jQuery File Upload demo.
+
+To place the jQuery File Upload widget in a template, simply insert the
+following within it::
+    
+    {% load jfutags %}
+    {% jfu %}
+
+Then create a view that will handle the uploaded files. 
+The URL for the view is expected to be named **'jfu_upload'** by default,
+although this can be customized (see Customization below).
+
+Here is an example implementation:
+
+In your ``urls.py`` file::
+
+    ...
+    url( r'upload/', views.upload, name = 'jfu_upload' ),
+
+    # You may optionally define a delete url as well
+    url( r'^delete/(?P<pk>\d+)$', views.upload_delete, name = 'jfu_delete' ),
+
+In your ``views.py`` file::
+    
+    import os
+    from django.conf import settings
+    from django.core.urlresolvers import reverse
+    from django.views import generic
+    from django.views.decorators.http import require_POST
+    from jfu.http import upload_receive, UploadResponse, JFUResponse
+
+    from YOURAPP.models import YOURMODEL
+
+    @require_POST
+    def upload( request ):
+
+        # The assumption here is that jQuery File Upload
+        # has been configured to send files one at a time.
+        # If multiple files can be uploaded simulatenously,
+        # 'file' may be a list of files.
+        file = upload_receive( request )
+
+        instance = YOURMODEL( file = file )
+        instance.save()
+
+        basename = os.path.basename( instance.file.path )
+        
+        file_dict = {
+            'name' : basename,
+            'size' : file.size,
+
+            'url': settings.MEDIA_URL + basename,
+            'thumbnailUrl': settings.MEDIA_URL + basename,
+
+            'deleteUrl': reverse('jfu_delete', kwargs = { 'pk': instance.pk }),
+            'deleteType': 'POST',
+        }
+
+        return UploadResponse( request, file_dict )
+
+    @require_POST
+    def upload_delete( request, pk ):
+        success = True
+        try:
+            instance = YOURMODEL.objects.get( pk = pk )
+            os.unlink( instance.file.path )
+            instance.delete()
+        except YOURMODEL.DoesNotExist:
+            success = False
+
+        return JFUResponse( request, success )
+
+Customization
+-------------
+
+Django-JFU is designed to be very customizable.  
+
+The Django-JFU template tag optionally takes two arguments: the name of the
+template to load and the name of the URL pointing to the upload-handling
+view.::
+
+    {% load jfutags %}
+    {% jfu 'your_fileuploader.html' 'your_uploader_URL_name' %}
+
+A custom template can extend from the master Django-JFU template
+`jfu/upload_form.html`.  There are several blocks which may be overriden for
+the purpose of customization:
+
+* JS_OPTS - The options supplied to the jQuery File Upload ``fileupload`` function. 
+* JS_INIT - The initializing JavaScript
+* FILE_INPUT - The file input for the upload form.
+
+The blocks above are most-likely what you will want to override when seeking to
+customize. For instance, one would go about adding a few options to the
+fileupload function in this manner::
+
+    # your_fileuploader.html
+    {% extends 'jfu/upload_form.html' %}
+    
+    {% block JS_OPTS %}
+    autoUpload: true,
+    maxNumberOfFiles: 5,
+    sequentialUploads: true,
+    {% endblock %}
+
+There are several other blocks too:
+
+
+HTML Components
+===============
+
+* MODAL_GALLERY - The modal gallery
+* UPLOAD_FORM   - The file upload form used as target for the file upload widget.
+
+  * UPLOAD_FORM_LISTING - The table listing the files available for upload/download.
+  * UPLOAD_FORM_LINDICATOR - The loading indicator shown during file processing.
+  * UPLOAD_FORM_PROGRESS_BAR - The global progress information.
+  * UPLOAD_FORM_BUTTON_BAR - The fileupload-buttonbar contains buttons to add/delete files and start/cancel the upload.
+
+    * UPLOAD_FORM_BUTTON_BAR_CONTROL - Contains buttons to start/cancel the upload or delete files. 
+    * UPLOAD_FORM_BUTTON_BAR_ADD     - Contains the file input used to add files.
+        * FILE_INPUT or UPLOAD_FORM_BUTTON_BAR_ADD_FILE_INPUT - Contains the file input.
+        * UPLOAD_FORM_BUTTON_BAR_ADD_EXTRA - An empty block allowing the addition of extra inputs.
+    * UPLOAD_FORM_BUTTON_BAR_EXTRA  - An empty block allowing the addition of extra components.
+
+  * UPLOAD_FORM_EXTRA - An empty block allowing the addition of extra components.
+
+CSS Components
+==============
+
+* CSS
+
+  * CSS_BOOTSTRAP 
+  * CSS_BLUEIMP_GALLERY 
+  * CSS_JQUERY_FILE_UPLOAD
+  * CSS_JQUERY_FILE_UPLOAD_UI
+  * CSS_HTML5_SHIM 
+  * CSS_EXTRA 
+
+JS Components
+=============
+
+* JS_TEMPLATES
+
+  * JS_DOWNLOAD_TEMPLATE
+
+    * JS_DOWNLOAD_TEMPLATE_DELETE 
+    * JS_DOWNLOAD_TEMPLATE_DOWNLOAD
+    * JS_DOWNLOAD_TEMPLATE_PREVIEW 
+    * JS_DOWNLOAD_TEMPLATE_ERROR 
+    * JS_DOWNLOAD_TEMPLATE_FSIZE
+
+  * JS_UPLOAD_TEMPLATE
+
+    * JS_UPLOAD_TEMPLATE_PREVIEW
+    * JS_UPLOAD_TEMPLATE_UPLOAD
+    * JS_UPLOAD_TEMPLATE_CONTROLS
+
+        * JS_UPLOAD_TEMPLATE_START
+        * JS_UPLOAD_TEMPLATE_CANCEL
+
+    * JS_UPLOAD_TEMPLATE_PROGRESSBAR
+
+* JS_SCRIPTS
+
+  * JS_JQUERY 
+  * JS_JQUERY_UI_WIDGET
+  * JS_TEMPLATES_PLUGIN
+  * JS_LOAD_IMAGE
+  * JS_CANVAS_TO_BLOB 
+  * JS_BOOTSTRAP 
+  * JS_BLUEIMP_GALLERY 
+  * JS_BOOTSTRAP_IFRAME_TRANSPORT
+  * JS_JQUERY_FILE_UPLOAD
+  * JS_JQUERY_FILE_UPLOAD_FP
+  * JS_JQUERY_FILE_UPLOAD_IMAGE
+  * JS_JQUERY_FILE_UPLOAD_AUDIO
+  * JS_JQUERY_FILE_UPLOAD_VIDEO
+  * JS_JQUERY_FILE_UPLOAD_VALIDATE
+  * JS_JQUERY_FILEUPLOAD_UI 
+  * JS_XDR_TRANSPORT 
+  * JS_EXTRA
+
+The included JavaScript and CSS can be updated or suppressed by overriding
+these blocks ::
+
+    # your_fileuploader.html
+    {% extends 'jfu/upload_form.html' %}
+
+    {% block JS_JQUERY %}
+        <script src={{STATIC_URL}}/js/my.newer.jquery.js />
+    {% endblock %}
+
+    {% block CSS_BOOTSTRAP %}
+        {% comment %}
+        This is already included.
+        {% endcomment %}
+    {% endblock %}
+
+or by replacing the static files themselves.
+
+Demo
+----
+If you have downloaded from the repository, a simple demo application has been
+included in the 'demo' directory. 
+To test it out, enter the 'demo' directory and run ::
+
+        ./setup && ./run
+
+Note that virtualenv is required for the demo to function.
+
+Contribution
+------------           
+Django-JFU is wholly open source and welcomes contributions of any kind. Feel
+free to either extend it, report bugs, or provide suggestions for improvements.
+The author of Django-JFU can be contacted at alem@cidola.com.
```

### Comparing `django-dprog-jfu-2.2.4/PKG-INFO` & `django-dprog-jfu-3.0.0/django_dprog_jfu.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,274 +1,273 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-dprog-jfu
-Version: 2.2.4
+Version: 3.0.0
 Summary: A Django Library for jQuery File Upload.
 Home-page: http://packages.python.org/jfu
-Author: Z. Alem
+Author: Z. Alem, Philippe Docourt
 Author-email: alem@cidola.com
 Maintainer: Philippe Docourt
 License: BSD License
-Description: Note: This project is forked from https://github.com/jpic/django-jfu. This fork aims to localize the project and keep it compatible with recent versions of Django. It also updates some rather obsolete dependencies.
-        
-        ----------------------------------------------------
-        Django-JFU - A Django Library for jQuery File Upload 
-        ----------------------------------------------------
-        
-        Django-JFU is designed to simplify the tasks involved in integrating jQuery
-        File Upload (https://github.com/blueimp/jquery-file-upload) into Django.
-        Django-JFU assumes very little and leaves the model/view design up to the user. 
-        
-        Other Django - jQuery File Upload implementations are full-featured but
-        generally serve more as demonstrations than libraries for existing
-        applications.
-        
-        If you seek a tool to ease the integration of jQuery File Upload into your
-        Django application while still having a great degree of freedom, you may find
-        this package useful.
-        
-        Demo_
-        
-        .. _Demo: http://djfu-demo.cidola.com
-        
-        Installation
-        ------------
-        
-        1. ``pip install django-jfu``.
-        2. Add 'jfu' to ``INSTALLED_APPS`` in your project settings.py file.
-        3. Run `python manage.py collectstatic`.
-        
-        
-        Usage
-        -----
-        
-        Django-JFU provides simple customizable template tags and override-able
-        templates that do the work of integrating the jQuery File Upload CSS and
-        JavaScipt and the HTML implementation found in the jQuery File Upload demo.
-        
-        To place the jQuery File Upload widget in a template, simply insert the
-        following within it::
-            
-            {% load jfutags %}
-            {% jfu %}
-        
-        Then create a view that will handle the uploaded files. 
-        The URL for the view is expected to be named **'jfu_upload'** by default,
-        although this can be customized (see Customization below).
-        
-        Here is an example implementation:
-        
-        In your ``urls.py`` file::
-        
-            ...
-            url( r'upload/', views.upload, name = 'jfu_upload' ),
-        
-            # You may optionally define a delete url as well
-            url( r'^delete/(?P<pk>\d+)$', views.upload_delete, name = 'jfu_delete' ),
-        
-        In your ``views.py`` file::
-            
-            import os
-            from django.conf import settings
-            from django.core.urlresolvers import reverse
-            from django.views import generic
-            from django.views.decorators.http import require_POST
-            from jfu.http import upload_receive, UploadResponse, JFUResponse
-        
-            from YOURAPP.models import YOURMODEL
-        
-            @require_POST
-            def upload( request ):
-        
-                # The assumption here is that jQuery File Upload
-                # has been configured to send files one at a time.
-                # If multiple files can be uploaded simulatenously,
-                # 'file' may be a list of files.
-                file = upload_receive( request )
-        
-                instance = YOURMODEL( file = file )
-                instance.save()
-        
-                basename = os.path.basename( instance.file.path )
-                
-                file_dict = {
-                    'name' : basename,
-                    'size' : file.size,
-        
-                    'url': settings.MEDIA_URL + basename,
-                    'thumbnailUrl': settings.MEDIA_URL + basename,
-        
-                    'deleteUrl': reverse('jfu_delete', kwargs = { 'pk': instance.pk }),
-                    'deleteType': 'POST',
-                }
-        
-                return UploadResponse( request, file_dict )
-        
-            @require_POST
-            def upload_delete( request, pk ):
-                success = True
-                try:
-                    instance = YOURMODEL.objects.get( pk = pk )
-                    os.unlink( instance.file.path )
-                    instance.delete()
-                except YOURMODEL.DoesNotExist:
-                    success = False
-        
-                return JFUResponse( request, success )
-        
-        Customization
-        -------------
-        
-        Django-JFU is designed to be very customizable.  
-        
-        The Django-JFU template tag optionally takes two arguments: the name of the
-        template to load and the name of the URL pointing to the upload-handling
-        view.::
-        
-            {% load jfutags %}
-            {% jfu 'your_fileuploader.html' 'your_uploader_URL_name' %}
-        
-        A custom template can extend from the master Django-JFU template
-        `jfu/upload_form.html`.  There are several blocks which may be overriden for
-        the purpose of customization:
-        
-        * JS_OPTS - The options supplied to the jQuery File Upload ``fileupload`` function. 
-        * JS_INIT - The initializing JavaScript
-        * FILE_INPUT - The file input for the upload form.
-        
-        The blocks above are most-likely what you will want to override when seeking to
-        customize. For instance, one would go about adding a few options to the
-        fileupload function in this manner::
-        
-            # your_fileuploader.html
-            {% extends 'jfu/upload_form.html' %}
-            
-            {% block JS_OPTS %}
-            autoUpload: true,
-            maxNumberOfFiles: 5,
-            sequentialUploads: true,
-            {% endblock %}
-        
-        There are several other blocks too:
-        
-        
-        HTML Components
-        ===============
-        
-        * MODAL_GALLERY - The modal gallery
-        * UPLOAD_FORM   - The file upload form used as target for the file upload widget.
-        
-          * UPLOAD_FORM_LISTING - The table listing the files available for upload/download.
-          * UPLOAD_FORM_LINDICATOR - The loading indicator shown during file processing.
-          * UPLOAD_FORM_PROGRESS_BAR - The global progress information.
-          * UPLOAD_FORM_BUTTON_BAR - The fileupload-buttonbar contains buttons to add/delete files and start/cancel the upload.
-        
-            * UPLOAD_FORM_BUTTON_BAR_CONTROL - Contains buttons to start/cancel the upload or delete files. 
-            * UPLOAD_FORM_BUTTON_BAR_ADD     - Contains the file input used to add files.
-                * FILE_INPUT or UPLOAD_FORM_BUTTON_BAR_ADD_FILE_INPUT - Contains the file input.
-                * UPLOAD_FORM_BUTTON_BAR_ADD_EXTRA - An empty block allowing the addition of extra inputs.
-            * UPLOAD_FORM_BUTTON_BAR_EXTRA  - An empty block allowing the addition of extra components.
-        
-          * UPLOAD_FORM_EXTRA - An empty block allowing the addition of extra components.
-        
-        CSS Components
-        ==============
-        
-        * CSS
-        
-          * CSS_BOOTSTRAP 
-          * CSS_BLUEIMP_GALLERY 
-          * CSS_JQUERY_FILE_UPLOAD
-          * CSS_JQUERY_FILE_UPLOAD_UI
-          * CSS_HTML5_SHIM 
-          * CSS_EXTRA 
-        
-        JS Components
-        =============
-        
-        * JS_TEMPLATES
-        
-          * JS_DOWNLOAD_TEMPLATE
-        
-            * JS_DOWNLOAD_TEMPLATE_DELETE 
-            * JS_DOWNLOAD_TEMPLATE_DOWNLOAD
-            * JS_DOWNLOAD_TEMPLATE_PREVIEW 
-            * JS_DOWNLOAD_TEMPLATE_ERROR 
-            * JS_DOWNLOAD_TEMPLATE_FSIZE
-        
-          * JS_UPLOAD_TEMPLATE
-        
-            * JS_UPLOAD_TEMPLATE_PREVIEW
-            * JS_UPLOAD_TEMPLATE_UPLOAD
-            * JS_UPLOAD_TEMPLATE_CONTROLS
-        
-                * JS_UPLOAD_TEMPLATE_START
-                * JS_UPLOAD_TEMPLATE_CANCEL
-        
-            * JS_UPLOAD_TEMPLATE_PROGRESSBAR
-        
-        * JS_SCRIPTS
-        
-          * JS_JQUERY 
-          * JS_JQUERY_UI_WIDGET
-          * JS_TEMPLATES_PLUGIN
-          * JS_LOAD_IMAGE
-          * JS_CANVAS_TO_BLOB 
-          * JS_BOOTSTRAP 
-          * JS_BLUEIMP_GALLERY 
-          * JS_BOOTSTRAP_IFRAME_TRANSPORT
-          * JS_JQUERY_FILE_UPLOAD
-          * JS_JQUERY_FILE_UPLOAD_FP
-          * JS_JQUERY_FILE_UPLOAD_IMAGE
-          * JS_JQUERY_FILE_UPLOAD_AUDIO
-          * JS_JQUERY_FILE_UPLOAD_VIDEO
-          * JS_JQUERY_FILE_UPLOAD_VALIDATE
-          * JS_JQUERY_FILEUPLOAD_UI 
-          * JS_XDR_TRANSPORT 
-          * JS_EXTRA
-        
-        The included JavaScript and CSS can be updated or suppressed by overriding
-        these blocks ::
-        
-            # your_fileuploader.html
-            {% extends 'jfu/upload_form.html' %}
-        
-            {% block JS_JQUERY %}
-                <script src={{STATIC_URL}}/js/my.newer.jquery.js />
-            {% endblock %}
-        
-            {% block CSS_BOOTSTRAP %}
-                {% comment %}
-                This is already included.
-                {% endcomment %}
-            {% endblock %}
-        
-        or by replacing the static files themselves.
-        
-        Demo
-        ----
-        If you have downloaded from the repository, a simple demo application has been
-        included in the 'demo' directory. 
-        To test it out, enter the 'demo' directory and run ::
-        
-                ./setup && ./run
-        
-        Note that virtualenv is required for the demo to function.
-        
-        Contribution
-        ------------           
-        Django-JFU is wholly open source and welcomes contributions of any kind. Feel
-        free to either extend it, report bugs, or provide suggestions for improvements.
-        The author of Django-JFU can be contacted at alem@cidola.com.
-        
 Keywords: django,jquery file upload,multi-upload
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+Note: This project is forked from https://github.com/jpic/django-jfu. This fork aims to localize the project and keep it compatible with recent versions of Django. It also updates some rather obsolete dependencies.
+
+----------------------------------------------------
+Django-JFU - A Django Library for jQuery File Upload 
+----------------------------------------------------
+
+Django-JFU is designed to simplify the tasks involved in integrating jQuery
+File Upload (https://github.com/blueimp/jquery-file-upload) into Django.
+Django-JFU assumes very little and leaves the model/view design up to the user. 
+
+Other Django - jQuery File Upload implementations are full-featured but
+generally serve more as demonstrations than libraries for existing
+applications.
+
+If you seek a tool to ease the integration of jQuery File Upload into your
+Django application while still having a great degree of freedom, you may find
+this package useful.
+
+Demo_
+
+.. _Demo: http://djfu-demo.cidola.com
+
+Installation
+------------
+
+1. ``pip install django-jfu``.
+2. Add 'jfu' to ``INSTALLED_APPS`` in your project settings.py file.
+3. Run `python manage.py collectstatic`.
+
+
+Usage
+-----
+
+Django-JFU provides simple customizable template tags and override-able
+templates that do the work of integrating the jQuery File Upload CSS and
+JavaScipt and the HTML implementation found in the jQuery File Upload demo.
+
+To place the jQuery File Upload widget in a template, simply insert the
+following within it::
+    
+    {% load jfutags %}
+    {% jfu %}
+
+Then create a view that will handle the uploaded files. 
+The URL for the view is expected to be named **'jfu_upload'** by default,
+although this can be customized (see Customization below).
+
+Here is an example implementation:
+
+In your ``urls.py`` file::
+
+    ...
+    url( r'upload/', views.upload, name = 'jfu_upload' ),
+
+    # You may optionally define a delete url as well
+    url( r'^delete/(?P<pk>\d+)$', views.upload_delete, name = 'jfu_delete' ),
+
+In your ``views.py`` file::
+    
+    import os
+    from django.conf import settings
+    from django.core.urlresolvers import reverse
+    from django.views import generic
+    from django.views.decorators.http import require_POST
+    from jfu.http import upload_receive, UploadResponse, JFUResponse
+
+    from YOURAPP.models import YOURMODEL
+
+    @require_POST
+    def upload( request ):
+
+        # The assumption here is that jQuery File Upload
+        # has been configured to send files one at a time.
+        # If multiple files can be uploaded simulatenously,
+        # 'file' may be a list of files.
+        file = upload_receive( request )
+
+        instance = YOURMODEL( file = file )
+        instance.save()
+
+        basename = os.path.basename( instance.file.path )
+        
+        file_dict = {
+            'name' : basename,
+            'size' : file.size,
+
+            'url': settings.MEDIA_URL + basename,
+            'thumbnailUrl': settings.MEDIA_URL + basename,
+
+            'deleteUrl': reverse('jfu_delete', kwargs = { 'pk': instance.pk }),
+            'deleteType': 'POST',
+        }
+
+        return UploadResponse( request, file_dict )
+
+    @require_POST
+    def upload_delete( request, pk ):
+        success = True
+        try:
+            instance = YOURMODEL.objects.get( pk = pk )
+            os.unlink( instance.file.path )
+            instance.delete()
+        except YOURMODEL.DoesNotExist:
+            success = False
+
+        return JFUResponse( request, success )
+
+Customization
+-------------
+
+Django-JFU is designed to be very customizable.  
+
+The Django-JFU template tag optionally takes two arguments: the name of the
+template to load and the name of the URL pointing to the upload-handling
+view.::
+
+    {% load jfutags %}
+    {% jfu 'your_fileuploader.html' 'your_uploader_URL_name' %}
+
+A custom template can extend from the master Django-JFU template
+`jfu/upload_form.html`.  There are several blocks which may be overriden for
+the purpose of customization:
+
+* JS_OPTS - The options supplied to the jQuery File Upload ``fileupload`` function. 
+* JS_INIT - The initializing JavaScript
+* FILE_INPUT - The file input for the upload form.
+
+The blocks above are most-likely what you will want to override when seeking to
+customize. For instance, one would go about adding a few options to the
+fileupload function in this manner::
+
+    # your_fileuploader.html
+    {% extends 'jfu/upload_form.html' %}
+    
+    {% block JS_OPTS %}
+    autoUpload: true,
+    maxNumberOfFiles: 5,
+    sequentialUploads: true,
+    {% endblock %}
+
+There are several other blocks too:
+
+
+HTML Components
+===============
+
+* MODAL_GALLERY - The modal gallery
+* UPLOAD_FORM   - The file upload form used as target for the file upload widget.
+
+  * UPLOAD_FORM_LISTING - The table listing the files available for upload/download.
+  * UPLOAD_FORM_LINDICATOR - The loading indicator shown during file processing.
+  * UPLOAD_FORM_PROGRESS_BAR - The global progress information.
+  * UPLOAD_FORM_BUTTON_BAR - The fileupload-buttonbar contains buttons to add/delete files and start/cancel the upload.
+
+    * UPLOAD_FORM_BUTTON_BAR_CONTROL - Contains buttons to start/cancel the upload or delete files. 
+    * UPLOAD_FORM_BUTTON_BAR_ADD     - Contains the file input used to add files.
+        * FILE_INPUT or UPLOAD_FORM_BUTTON_BAR_ADD_FILE_INPUT - Contains the file input.
+        * UPLOAD_FORM_BUTTON_BAR_ADD_EXTRA - An empty block allowing the addition of extra inputs.
+    * UPLOAD_FORM_BUTTON_BAR_EXTRA  - An empty block allowing the addition of extra components.
+
+  * UPLOAD_FORM_EXTRA - An empty block allowing the addition of extra components.
+
+CSS Components
+==============
+
+* CSS
+
+  * CSS_BOOTSTRAP 
+  * CSS_BLUEIMP_GALLERY 
+  * CSS_JQUERY_FILE_UPLOAD
+  * CSS_JQUERY_FILE_UPLOAD_UI
+  * CSS_HTML5_SHIM 
+  * CSS_EXTRA 
+
+JS Components
+=============
+
+* JS_TEMPLATES
+
+  * JS_DOWNLOAD_TEMPLATE
+
+    * JS_DOWNLOAD_TEMPLATE_DELETE 
+    * JS_DOWNLOAD_TEMPLATE_DOWNLOAD
+    * JS_DOWNLOAD_TEMPLATE_PREVIEW 
+    * JS_DOWNLOAD_TEMPLATE_ERROR 
+    * JS_DOWNLOAD_TEMPLATE_FSIZE
+
+  * JS_UPLOAD_TEMPLATE
+
+    * JS_UPLOAD_TEMPLATE_PREVIEW
+    * JS_UPLOAD_TEMPLATE_UPLOAD
+    * JS_UPLOAD_TEMPLATE_CONTROLS
+
+        * JS_UPLOAD_TEMPLATE_START
+        * JS_UPLOAD_TEMPLATE_CANCEL
+
+    * JS_UPLOAD_TEMPLATE_PROGRESSBAR
+
+* JS_SCRIPTS
+
+  * JS_JQUERY 
+  * JS_JQUERY_UI_WIDGET
+  * JS_TEMPLATES_PLUGIN
+  * JS_LOAD_IMAGE
+  * JS_CANVAS_TO_BLOB 
+  * JS_BOOTSTRAP 
+  * JS_BLUEIMP_GALLERY 
+  * JS_BOOTSTRAP_IFRAME_TRANSPORT
+  * JS_JQUERY_FILE_UPLOAD
+  * JS_JQUERY_FILE_UPLOAD_FP
+  * JS_JQUERY_FILE_UPLOAD_IMAGE
+  * JS_JQUERY_FILE_UPLOAD_AUDIO
+  * JS_JQUERY_FILE_UPLOAD_VIDEO
+  * JS_JQUERY_FILE_UPLOAD_VALIDATE
+  * JS_JQUERY_FILEUPLOAD_UI 
+  * JS_XDR_TRANSPORT 
+  * JS_EXTRA
+
+The included JavaScript and CSS can be updated or suppressed by overriding
+these blocks ::
+
+    # your_fileuploader.html
+    {% extends 'jfu/upload_form.html' %}
+
+    {% block JS_JQUERY %}
+        <script src={{STATIC_URL}}/js/my.newer.jquery.js />
+    {% endblock %}
+
+    {% block CSS_BOOTSTRAP %}
+        {% comment %}
+        This is already included.
+        {% endcomment %}
+    {% endblock %}
+
+or by replacing the static files themselves.
+
+Demo
+----
+If you have downloaded from the repository, a simple demo application has been
+included in the 'demo' directory. 
+To test it out, enter the 'demo' directory and run ::
+
+        ./setup && ./run
+
+Note that virtualenv is required for the demo to function.
+
+Contribution
+------------           
+Django-JFU is wholly open source and welcomes contributions of any kind. Feel
+free to either extend it, report bugs, or provide suggestions for improvements.
+The author of Django-JFU can be contacted at alem@cidola.com.
```

