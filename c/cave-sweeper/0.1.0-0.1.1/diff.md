# Comparing `tmp/cave_sweeper-0.1.0.tar.gz` & `tmp/cave_sweeper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_sweeper-0.1.0.tar", max compression
+gzip compressed data, was "cave_sweeper-0.1.1.tar", max compression
```

## Comparing `cave_sweeper-0.1.0.tar` & `cave_sweeper-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-11 20:24:03.431189 cave_sweeper-0.1.0/README.md
--rw-r--r--   0        0        0      176 2023-04-05 20:38:52.095284 cave_sweeper-0.1.0/cave_sweeper/.idea/.gitignore
--rw-r--r--   0        0        0        0 2023-05-11 10:09:22.707158 cave_sweeper-0.1.0/cave_sweeper/.idea/Icon
--rw-r--r--   0        0        0        0 2023-05-11 10:09:22.742133 cave_sweeper-0.1.0/cave_sweeper/.idea/inspectionProfiles/Icon
--rw-r--r--   0        0        0     2651 2023-04-05 20:42:33.148362 cave_sweeper-0.1.0/cave_sweeper/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-04-05 20:42:33.183083 cave_sweeper-0.1.0/cave_sweeper/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      284 2023-04-05 20:42:33.161709 cave_sweeper-0.1.0/cave_sweeper/.idea/mine_sweeper.iml
--rw-r--r--   0        0        0      197 2023-04-05 20:42:33.176791 cave_sweeper-0.1.0/cave_sweeper/.idea/misc.xml
--rw-r--r--   0        0        0      276 2023-04-05 20:42:33.167562 cave_sweeper-0.1.0/cave_sweeper/.idea/modules.xml
--rw-r--r--   0        0        0      183 2023-04-05 20:42:33.189296 cave_sweeper-0.1.0/cave_sweeper/.idea/vcs.xml
--rw-r--r--   0        0        0     4061 2023-04-08 10:56:50.511097 cave_sweeper-0.1.0/cave_sweeper/.idea/workspace.xml
--rw-r--r--   0        0        0        0 2023-05-11 07:45:24.031834 cave_sweeper-0.1.0/cave_sweeper/Icon
--rw-r--r--   0        0        0     5644 2023-05-07 16:02:31.619200 cave_sweeper-0.1.0/cave_sweeper/field_slot.py
--rw-r--r--   0        0        0      104 2023-05-05 21:40:39.835327 cave_sweeper-0.1.0/cave_sweeper/mine_sweeper.py
--rw-r--r--   0        0        0     4403 2023-05-07 14:56:43.303019 cave_sweeper-0.1.0/cave_sweeper/renderers.py
--rw-r--r--   0        0        0       55 2023-05-05 22:02:44.764403 cave_sweeper-0.1.0/cave_sweeper/settings.py
--rw-r--r--   0        0        0      188 2023-05-05 21:13:27.324715 cave_sweeper-0.1.0/cave_sweeper/utils.py
--rw-r--r--   0        0        0      288 2023-05-11 20:25:43.893759 cave_sweeper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 cave_sweeper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-11 20:24:03.431189 cave_sweeper-0.1.1/README.md
+-rw-r--r--   0        0        0     5644 2023-05-07 16:02:31.619200 cave_sweeper-0.1.1/cave_sweeper/field_slot.py
+-rw-r--r--   0        0        0      104 2023-05-05 21:40:39.835327 cave_sweeper-0.1.1/cave_sweeper/mine_sweeper.py
+-rw-r--r--   0        0        0     4403 2023-05-07 14:56:43.303019 cave_sweeper-0.1.1/cave_sweeper/renderers.py
+-rw-r--r--   0        0        0       55 2023-05-05 22:02:44.764403 cave_sweeper-0.1.1/cave_sweeper/settings.py
+-rw-r--r--   0        0        0      188 2023-05-05 21:13:27.324715 cave_sweeper-0.1.1/cave_sweeper/utils.py
+-rw-r--r--   0        0        0      288 2023-05-11 20:47:32.762486 cave_sweeper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 cave_sweeper-0.1.1/PKG-INFO
```

### Comparing `cave_sweeper-0.1.0/cave_sweeper/field_slot.py` & `cave_sweeper-0.1.1/cave_sweeper/field_slot.py`

 * *Files identical despite different names*

### Comparing `cave_sweeper-0.1.0/cave_sweeper/renderers.py` & `cave_sweeper-0.1.1/cave_sweeper/renderers.py`

 * *Files identical despite different names*

