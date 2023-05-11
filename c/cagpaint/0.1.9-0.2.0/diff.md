# Comparing `tmp/cagpaint-0.1.9.tar.gz` & `tmp/cagpaint-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagpaint-0.1.9.tar", last modified: Mon May  8 10:59:09 2023, max compression
+gzip compressed data, was "cagpaint-0.2.0.tar", last modified: Thu May 11 12:14:45 2023, max compression
```

## Comparing `cagpaint-0.1.9.tar` & `cagpaint-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.455272 cagpaint-0.1.9/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.1.9/LICENSE
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-08 10:59:09.455272 cagpaint-0.1.9/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.1.9/README.md
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.451272 cagpaint-0.1.9/cagpaint/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:53:02.000000 cagpaint-0.1.9/cagpaint/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.451272 cagpaint-0.1.9/cagpaint/painter/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:49.000000 cagpaint-0.1.9/cagpaint/painter/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3932 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/install_fixes.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.455272 cagpaint-0.1.9/cagpaint/painter/src/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:53.000000 cagpaint-0.1.9/cagpaint/painter/src/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    43783 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/about.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6548 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/contrast_slider.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12269 2023-05-08 08:52:37.000000 cagpaint-0.1.9/cagpaint/painter/src/create_project.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6657 2023-05-08 09:04:20.000000 cagpaint-0.1.9/cagpaint/painter/src/file_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    16052 2023-05-08 09:05:33.000000 cagpaint-0.1.9/cagpaint/painter/src/graphics_scene.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2853 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/graphics_view.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12990 2023-05-03 08:00:12.000000 cagpaint-0.1.9/cagpaint/painter/src/im_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    24174 2023-05-08 09:03:45.000000 cagpaint-0.1.9/cagpaint/painter/src/im_viewer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3161 2022-11-29 09:34:29.000000 cagpaint-0.1.9/cagpaint/painter/src/instructions.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2347 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/lock.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3433 2023-05-08 08:49:26.000000 cagpaint-0.1.9/cagpaint/painter/src/main.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13163 2023-05-08 08:54:38.000000 cagpaint-0.1.9/cagpaint/painter/src/menus.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1649 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/name_edit_widget.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5421 2023-05-08 08:54:45.000000 cagpaint-0.1.9/cagpaint/painter/src/nav.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3620 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/palette.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8583 2023-05-08 08:54:54.000000 cagpaint-0.1.9/cagpaint/painter/src/patch_seg.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1808 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/progress_widget.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    37257 2023-05-08 09:02:57.000000 cagpaint-0.1.9/cagpaint/painter/src/root_painter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1304 2022-11-29 09:34:29.000000 cagpaint-0.1.9/cagpaint/painter/src/segment.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8471 2023-05-08 08:55:19.000000 cagpaint-0.1.9/cagpaint/painter/src/segment_folder.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4572 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/slice_nav.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3039 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/tcp_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       85 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/painter/src/view_state.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3080 2023-05-04 16:09:47.000000 cagpaint-0.1.9/cagpaint/painter/src/visibility_widget.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      124 2023-05-08 08:30:21.000000 cagpaint-0.1.9/cagpaint/setup.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.455272 cagpaint-0.1.9/cagpaint/trainer/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       30 2023-05-08 08:38:36.000000 cagpaint-0.1.9/cagpaint/trainer/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1204 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/trainer/data_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    19244 2023-05-08 09:09:39.000000 cagpaint-0.1.9/cagpaint/trainer/datasets.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2650 2022-11-26 14:08:31.000000 cagpaint-0.1.9/cagpaint/trainer/file_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    21207 2023-05-08 08:42:35.000000 cagpaint-0.1.9/cagpaint/trainer/im_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1789 2022-11-29 09:34:29.000000 cagpaint-0.1.9/cagpaint/trainer/instructions.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7422 2023-05-08 10:04:33.000000 cagpaint-0.1.9/cagpaint/trainer/loss.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2213 2023-05-08 08:46:32.000000 cagpaint-0.1.9/cagpaint/trainer/main.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2922 2022-09-20 07:40:58.000000 cagpaint-0.1.9/cagpaint/trainer/metrics.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15276 2023-05-08 09:33:38.000000 cagpaint-0.1.9/cagpaint/trainer/model_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7463 2023-05-08 07:44:59.000000 cagpaint-0.1.9/cagpaint/trainer/patch_seg.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1373 2023-05-05 17:55:24.000000 cagpaint-0.1.9/cagpaint/trainer/scp_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2587 2022-11-17 08:42:24.000000 cagpaint-0.1.9/cagpaint/trainer/startup.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    29805 2023-05-08 09:09:02.000000 cagpaint-0.1.9/cagpaint/trainer/trainer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7698 2023-05-08 09:33:09.000000 cagpaint-0.1.9/cagpaint/trainer/unet3d.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-08 10:59:09.451272 cagpaint-0.1.9/cagpaint.egg-info/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1565 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/SOURCES.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/dependency_links.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        9 2023-05-08 10:59:09.000000 cagpaint-0.1.9/cagpaint.egg-info/top_level.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-08 10:59:09.455272 cagpaint-0.1.9/setup.cfg
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-08 10:58:15.000000 cagpaint-0.1.9/setup.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-11 12:14:45.546871 cagpaint-0.2.0/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.2.0/LICENSE
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-11 12:14:45.546871 cagpaint-0.2.0/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.2.0/README.md
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-11 12:14:45.538871 cagpaint-0.2.0/cagpaint/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:53:02.000000 cagpaint-0.2.0/cagpaint/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-11 12:14:45.538871 cagpaint-0.2.0/cagpaint/painter/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:49.000000 cagpaint-0.2.0/cagpaint/painter/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3932 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/install_fixes.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-11 12:14:45.546871 cagpaint-0.2.0/cagpaint/painter/src/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-05-04 13:56:53.000000 cagpaint-0.2.0/cagpaint/painter/src/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    43783 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/about.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6548 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/contrast_slider.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12269 2023-05-08 08:52:37.000000 cagpaint-0.2.0/cagpaint/painter/src/create_project.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6657 2023-05-08 09:04:20.000000 cagpaint-0.2.0/cagpaint/painter/src/file_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    16052 2023-05-08 09:05:33.000000 cagpaint-0.2.0/cagpaint/painter/src/graphics_scene.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2853 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/graphics_view.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12990 2023-05-03 08:00:12.000000 cagpaint-0.2.0/cagpaint/painter/src/im_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    24174 2023-05-08 09:03:45.000000 cagpaint-0.2.0/cagpaint/painter/src/im_viewer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3161 2022-11-29 09:34:29.000000 cagpaint-0.2.0/cagpaint/painter/src/instructions.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2347 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/lock.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3433 2023-05-08 08:49:26.000000 cagpaint-0.2.0/cagpaint/painter/src/main.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13163 2023-05-08 08:54:38.000000 cagpaint-0.2.0/cagpaint/painter/src/menus.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1649 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/name_edit_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5421 2023-05-08 08:54:45.000000 cagpaint-0.2.0/cagpaint/painter/src/nav.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3620 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/palette.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8583 2023-05-08 08:54:54.000000 cagpaint-0.2.0/cagpaint/painter/src/patch_seg.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1808 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/progress_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    37257 2023-05-08 09:02:57.000000 cagpaint-0.2.0/cagpaint/painter/src/root_painter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1304 2022-11-29 09:34:29.000000 cagpaint-0.2.0/cagpaint/painter/src/segment.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8471 2023-05-08 08:55:19.000000 cagpaint-0.2.0/cagpaint/painter/src/segment_folder.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4572 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/slice_nav.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3039 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/tcp_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       85 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/painter/src/view_state.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3080 2023-05-04 16:09:47.000000 cagpaint-0.2.0/cagpaint/painter/src/visibility_widget.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      124 2023-05-08 08:30:21.000000 cagpaint-0.2.0/cagpaint/setup.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-11 12:14:45.546871 cagpaint-0.2.0/cagpaint/trainer/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       30 2023-05-11 12:03:09.000000 cagpaint-0.2.0/cagpaint/trainer/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1204 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/trainer/data_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    19244 2023-05-08 09:09:39.000000 cagpaint-0.2.0/cagpaint/trainer/datasets.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2650 2022-11-26 14:08:31.000000 cagpaint-0.2.0/cagpaint/trainer/file_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    21205 2023-05-11 12:00:09.000000 cagpaint-0.2.0/cagpaint/trainer/im_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1789 2022-11-29 09:34:29.000000 cagpaint-0.2.0/cagpaint/trainer/instructions.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7444 2023-05-11 12:02:17.000000 cagpaint-0.2.0/cagpaint/trainer/loss.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2213 2023-05-08 08:46:32.000000 cagpaint-0.2.0/cagpaint/trainer/main.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2922 2022-09-20 07:40:58.000000 cagpaint-0.2.0/cagpaint/trainer/metrics.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15276 2023-05-08 09:33:38.000000 cagpaint-0.2.0/cagpaint/trainer/model_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7463 2023-05-08 07:44:59.000000 cagpaint-0.2.0/cagpaint/trainer/patch_seg.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1373 2023-05-05 17:55:24.000000 cagpaint-0.2.0/cagpaint/trainer/scp_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2587 2022-11-17 08:42:24.000000 cagpaint-0.2.0/cagpaint/trainer/startup.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    29805 2023-05-08 09:09:02.000000 cagpaint-0.2.0/cagpaint/trainer/trainer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7698 2023-05-08 09:33:09.000000 cagpaint-0.2.0/cagpaint/trainer/unet3d.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-11 12:14:45.538871 cagpaint-0.2.0/cagpaint.egg-info/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-11 12:14:45.000000 cagpaint-0.2.0/cagpaint.egg-info/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1565 2023-05-11 12:14:45.000000 cagpaint-0.2.0/cagpaint.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-11 12:14:45.000000 cagpaint-0.2.0/cagpaint.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        9 2023-05-11 12:14:45.000000 cagpaint-0.2.0/cagpaint.egg-info/top_level.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-11 12:14:45.546871 cagpaint-0.2.0/setup.cfg
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-11 12:14:27.000000 cagpaint-0.2.0/setup.py
```

### Comparing `cagpaint-0.1.9/LICENSE` & `cagpaint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/install_fixes.py` & `cagpaint-0.2.0/cagpaint/painter/install_fixes.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/about.py` & `cagpaint-0.2.0/cagpaint/painter/src/about.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/contrast_slider.py` & `cagpaint-0.2.0/cagpaint/painter/src/contrast_slider.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/create_project.py` & `cagpaint-0.2.0/cagpaint/painter/src/create_project.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/file_utils.py` & `cagpaint-0.2.0/cagpaint/painter/src/file_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/graphics_scene.py` & `cagpaint-0.2.0/cagpaint/painter/src/graphics_scene.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/graphics_view.py` & `cagpaint-0.2.0/cagpaint/painter/src/graphics_view.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/im_utils.py` & `cagpaint-0.2.0/cagpaint/painter/src/im_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/im_viewer.py` & `cagpaint-0.2.0/cagpaint/painter/src/im_viewer.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/instructions.py` & `cagpaint-0.2.0/cagpaint/painter/src/instructions.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/lock.py` & `cagpaint-0.2.0/cagpaint/painter/src/lock.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/main.py` & `cagpaint-0.2.0/cagpaint/painter/src/main.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/menus.py` & `cagpaint-0.2.0/cagpaint/painter/src/menus.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/name_edit_widget.py` & `cagpaint-0.2.0/cagpaint/painter/src/name_edit_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/nav.py` & `cagpaint-0.2.0/cagpaint/painter/src/nav.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/palette.py` & `cagpaint-0.2.0/cagpaint/painter/src/palette.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/patch_seg.py` & `cagpaint-0.2.0/cagpaint/painter/src/patch_seg.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/progress_widget.py` & `cagpaint-0.2.0/cagpaint/painter/src/progress_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/root_painter.py` & `cagpaint-0.2.0/cagpaint/painter/src/root_painter.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/segment.py` & `cagpaint-0.2.0/cagpaint/painter/src/segment.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/segment_folder.py` & `cagpaint-0.2.0/cagpaint/painter/src/segment_folder.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/slice_nav.py` & `cagpaint-0.2.0/cagpaint/painter/src/slice_nav.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/tcp_utils.py` & `cagpaint-0.2.0/cagpaint/painter/src/tcp_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/painter/src/visibility_widget.py` & `cagpaint-0.2.0/cagpaint/painter/src/visibility_widget.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/data_utils.py` & `cagpaint-0.2.0/cagpaint/trainer/data_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/datasets.py` & `cagpaint-0.2.0/cagpaint/trainer/datasets.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/file_utils.py` & `cagpaint-0.2.0/cagpaint/trainer/file_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/im_utils.py` & `cagpaint-0.2.0/cagpaint/trainer/im_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
 
         # it's possible the image has a different extenstion
         # so use glob to get it
         fname_no_ext = fname.replace('.nii.gz', '').replace('.nrrd', '').replace('.dcm', '')
         image_path_part = os.path.join(dataset_dir, fname_no_ext)
         image_path = glob.glob(image_path_part + '.*')[0]
         image = load_image(image_path)
-      #  image = pad_image(image, 34) # removed 22nov
+        image = pad_image(image, 34) # added 11 may
         #  needs to be swapped to channels first and rotated etc
         # to be consistent with everything else.
         # todo: consider removing this soon.
         #image = np.rot90(image, k=3)
        # image = np.moveaxis(image, -1, 0) # depth moved to beginning
         # reverse lr and ud
       #  image = image[::-1, :, ::-1]
```

### Comparing `cagpaint-0.1.9/cagpaint/trainer/instructions.py` & `cagpaint-0.2.0/cagpaint/trainer/instructions.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/loss.py` & `cagpaint-0.2.0/cagpaint/trainer/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
                     masks.append(mask)
                     fg_tiles.append(fg_tile)
                     class_outputs.append(class_output)
 
                     seg_tile = batch_seg_tiles[im_idx][i]
                     if seg_tile is not None:
-                        seg_tile = torch.from_numpy(seg_tile).to(device)
+                        seg_tile = torch.from_numpy(seg_tile[17:-17,17:-17,17:-17]).to(device)
                        # seg_tile = seg_tile.to(device)
                         # for this purpose we ensure segmentation never disagrees with annotation.
                         seg_tile[fg_tile] = 1
                         seg_tile[bg_tile] = 0
                         seg_tiles.append(seg_tile)
                         seg_class_outputs.append(class_output)
```

### Comparing `cagpaint-0.1.9/cagpaint/trainer/main.py` & `cagpaint-0.2.0/cagpaint/trainer/main.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/metrics.py` & `cagpaint-0.2.0/cagpaint/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/model_utils.py` & `cagpaint-0.2.0/cagpaint/trainer/model_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/patch_seg.py` & `cagpaint-0.2.0/cagpaint/trainer/patch_seg.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/scp_utils.py` & `cagpaint-0.2.0/cagpaint/trainer/scp_utils.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/startup.py` & `cagpaint-0.2.0/cagpaint/trainer/startup.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/trainer.py` & `cagpaint-0.2.0/cagpaint/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint/trainer/unet3d.py` & `cagpaint-0.2.0/cagpaint/trainer/unet3d.py`

 * *Files identical despite different names*

### Comparing `cagpaint-0.1.9/cagpaint.egg-info/SOURCES.txt` & `cagpaint-0.2.0/cagpaint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

