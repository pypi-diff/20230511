# Comparing `tmp/aiuv-0.3.tar.gz` & `tmp/aiuv-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiuv-0.3.tar", last modified: Thu May 11 13:49:37 2023, max compression
+gzip compressed data, was "aiuv-0.4.tar", last modified: Thu May 11 14:02:50 2023, max compression
```

## Comparing `aiuv-0.3.tar` & `aiuv-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 13:49:37.866423 aiuv-0.3/
--rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.3/Licence.txt
--rw-rw-rw-   0        0        0      144 2023-05-11 13:49:37.865423 aiuv-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 13:49:37.855418 aiuv-0.3/aiuv.egg-info/
--rw-rw-rw-   0        0        0      144 2023-05-11 13:49:37.000000 aiuv-0.3/aiuv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-11 13:49:37.000000 aiuv-0.3/aiuv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 13:49:37.000000 aiuv-0.3/aiuv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-11 13:49:37.000000 aiuv-0.3/aiuv.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 13:49:37.863422 aiuv-0.3/pkg/
--rw-rw-rw-   0        0        0     5114 2023-05-11 13:49:01.000000 aiuv-0.3/pkg/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-11 13:49:37.866423 aiuv-0.3/setup.cfg
--rw-rw-rw-   0        0        0      183 2023-05-11 13:49:34.000000 aiuv-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 14:02:50.335082 aiuv-0.4/
+-rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.4/Licence.txt
+-rw-rw-rw-   0        0        0      144 2023-05-11 14:02:50.334088 aiuv-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-11 14:02:50.324082 aiuv-0.4/aiuv.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-05-11 14:02:50.000000 aiuv-0.4/aiuv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-11 14:02:50.000000 aiuv-0.4/aiuv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 14:02:50.000000 aiuv-0.4/aiuv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-11 14:02:50.000000 aiuv-0.4/aiuv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 14:02:50.332081 aiuv-0.4/pkg/
+-rw-rw-rw-   0        0        0    14980 2023-05-11 14:01:48.000000 aiuv-0.4/pkg/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-11 14:02:50.336088 aiuv-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      183 2023-05-11 14:02:14.000000 aiuv-0.4/setup.py
```

