# Comparing `tmp/stability-sdk-0.7.0.tar.gz` & `tmp/stability-sdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.7.0.tar", last modified: Thu Apr 27 17:02:42 2023, max compression
+gzip compressed data, was "stability-sdk-0.8.0.tar", last modified: Thu May 11 16:00:36 2023, max compression
```

## Comparing `stability-sdk-0.7.0.tar` & `stability-sdk-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.228326 stability-sdk-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37463 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-27 17:02:23.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.228326 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-27 17:02:25.000000 stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/src/stability_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/src/stability_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 17:02:42.000000 stability-sdk-0.7.0/src/stability_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:02:42.232326 stability-sdk-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-27 17:02:21.000000 stability-sdk-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.770250 stability-sdk-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.778250 stability-sdk-0.8.0/src/stability_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54884 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38386 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/animation_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28265 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37427 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.774250 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_animator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_utils.py
```

### Comparing `stability-sdk-0.7.0/LICENSE` & `stability-sdk-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/PKG-INFO` & `stability-sdk-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
@@ -25,14 +25,16 @@
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Raster-Based
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: anim
+Provides-Extra: anim_ui
 License-File: LICENSE
 
 # stability-sdk
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stability-ai/stability-sdk/blob/main/nbs/demo_colab.ipynb)
 
 Client implementations that interact with the Stability API. 
@@ -62,14 +64,22 @@
 `python3 -m stability_sdk generate -W 512 -H 512 "A stunning house."`
 
 It will generate and put PNGs in your current directory.
 
 To upscale:
 `python3 -m stability_sdk upscale -i "/path/to/image.png"`
 
+## Animation UI
+
+Install with 
+`pip install stability-sdk[anim_ui]`
+
+Then run with 
+`python3 -m stability_sdk animate --gui`
+
 ## SDK Usage
 
 Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
@@ -86,15 +96,15 @@
 options:
   -h, --help            show this help message and exit
   --height HEIGHT, -H HEIGHT
                         [512] height of image
   --width WIDTH, -W WIDTH
                         [512] width of image
   --start_schedule START_SCHEDULE
-                        [0.5] start schedule for init image (must be greater than 0, 1 is full strength
+                        [0.5] start schedule for init image (must be greater than 0; 1 is full strength
                         text prompt, no trace of image)
   --end_schedule END_SCHEDULE
                         [0.01] end schedule for init image
   --cfg_scale CFG_SCALE, -C CFG_SCALE
                         [7.0] CFG scale factor
   --sampler SAMPLER, -A SAMPLER
                         [auto-select] (ddim, plms, k_euler, k_euler_ancestral, k_heun, k_dpm_2,
@@ -160,12 +170,13 @@
 
 - [protobuf spec](https://github.com/Stability-AI/api-interfaces/blob/main/src/proto/)
 
 ## Community-contributed clients
 
 * Typescript client: https://github.com/jakiestfu/stability-ts
 * Guide to building for Ruby: https://github.com/kmcphillips/stability-sdk/blob/main/src/ruby/README.md
+* C# client: https://github.com/Katarzyna-Kadziolka/StabilityClient.Net
 
 ## Stability API TOS
 
 Usage of the Stability API falls under the [STABILITY AI API Terms of Service.
 ](https://platform.stability.ai/docs/terms-of-service)
```

### Comparing `stability-sdk-0.7.0/README.md` & `stability-sdk-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 `python3 -m stability_sdk generate -W 512 -H 512 "A stunning house."`
 
 It will generate and put PNGs in your current directory.
 
 To upscale:
 `python3 -m stability_sdk upscale -i "/path/to/image.png"`
 
+## Animation UI
+
+Install with 
+`pip install stability-sdk[anim_ui]`
+
+Then run with 
+`python3 -m stability_sdk animate --gui`
+
 ## SDK Usage
 
 Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
@@ -53,15 +61,15 @@
 options:
   -h, --help            show this help message and exit
   --height HEIGHT, -H HEIGHT
                         [512] height of image
   --width WIDTH, -W WIDTH
                         [512] width of image
   --start_schedule START_SCHEDULE
-                        [0.5] start schedule for init image (must be greater than 0, 1 is full strength
+                        [0.5] start schedule for init image (must be greater than 0; 1 is full strength
                         text prompt, no trace of image)
   --end_schedule END_SCHEDULE
                         [0.01] end schedule for init image
   --cfg_scale CFG_SCALE, -C CFG_SCALE
                         [7.0] CFG scale factor
   --sampler SAMPLER, -A SAMPLER
                         [auto-select] (ddim, plms, k_euler, k_euler_ancestral, k_heun, k_dpm_2,
@@ -127,12 +135,13 @@
 
 - [protobuf spec](https://github.com/Stability-AI/api-interfaces/blob/main/src/proto/)
 
 ## Community-contributed clients
 
 * Typescript client: https://github.com/jakiestfu/stability-ts
 * Guide to building for Ruby: https://github.com/kmcphillips/stability-sdk/blob/main/src/ruby/README.md
+* C# client: https://github.com/Katarzyna-Kadziolka/StabilityClient.Net
 
 ## Stability API TOS
 
 Usage of the Stability API falls under the [STABILITY AI API Terms of Service.
 ](https://platform.stability.ai/docs/terms-of-service)
```

### Comparing `stability-sdk-0.7.0/setup.py` & `stability-sdk-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 # fmt: off
 
-from setuptools import setup, find_namespace_packages
+from setuptools import (
+    setup,
+    find_namespace_packages,
+)
 
 with open('README.md','r') as f:
     README = f.read()
 
 setup(
     name='stability-sdk',
-    version='0.7.0',
+    version='0.8.0',
     author='Stability AI',
     author_email='support@stability.ai',
     maintainer='Stability AI',
     maintainer_email='support@stability.ai',
     url='https://beta.dreamstudio.ai/',
     download_url='https://github.com/Stability-AI/stability-sdk/',
-
     description='Python SDK for interacting with stability.ai APIs',
     long_description=README,
     long_description_content_type="text/markdown",
-
     install_requires=[
         'Pillow',
         'grpcio==1.53.0',
         'grpcio-tools==1.53.0',
         'python-dotenv',
+        'param',
         'protobuf==4.21.12'
     ],
     extras_require={
         'dev': [
             'pytest',
             'grpcio-testing'
-    ]},
+        ],
+        'anim': [
+            'keyframed',
+            'numpy',
+            'opencv-python-headless',
+        ],
+        'anim_ui': [
+            'keyframed',
+            'gradio',
+            'numpy',
+            'opencv-python-headless',
+            'tqdm',
+        ]
+    },
     packages=find_namespace_packages(
         where='src',
         include=['stability_sdk*'],
     ),
     package_dir = {"": "src"},
-
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Science/Research',
         'Topic :: Artistic Software',
         'Topic :: Education',
```

### Comparing `stability-sdk-0.7.0/src/stability_sdk/__main__.py` & `stability-sdk-0.8.0/src/stability_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/client.py` & `stability-sdk-0.8.0/src/stability_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,70 +1,44 @@
 #!/bin/which python3
 
 # fmt: off
 
-import pathlib
-import sys
+import getpass
+import grpc
+import logging
+import mimetypes
 import os
-import uuid
 import random
-import io
-import logging
+import sys
 import time
-import mimetypes
+import uuid
 
-import grpc
 from argparse import ArgumentParser, Namespace
-from typing import Dict, Generator, List, Optional, Union, Any, Sequence, Tuple
 from google.protobuf.json_format import MessageToJson
 from google.protobuf.struct_pb2 import Struct
 from PIL import Image
-
-try:
-    from dotenv import load_dotenv
-except ModuleNotFoundError:
-    pass
-else:
-    load_dotenv()
+from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, Union
 
 import stability_sdk.interfaces.gooseai.generation.generation_pb2 as generation
 import stability_sdk.interfaces.gooseai.generation.generation_pb2_grpc as generation_grpc
 
-from stability_sdk.utils import (
+from .api import open_channel
+from .utils import (
     SAMPLERS,
     MAX_FILENAME_SZ,
-    artifact_type_to_str,
-    truncate_fit,
-    get_sampler_from_str,
+    artifact_type_to_string,
+    image_to_prompt,
     open_images,
+    sampler_from_string,
+    truncate_fit,
 )
 
-
 logger = logging.getLogger(__name__)
 logger.setLevel(level=logging.INFO)
 
-def image_to_prompt(im, init: bool = False, mask: bool = False) -> generation.Prompt:
-    if init and mask:
-        raise ValueError("init and mask cannot both be True")
-    buf = io.BytesIO()
-    im.save(buf, format="PNG")
-    buf.seek(0)
-    if mask:
-        return generation.Prompt(
-            artifact=generation.Artifact(
-                type=generation.ARTIFACT_MASK, binary=buf.getvalue()
-            )
-        )
-    return generation.Prompt(
-        artifact=generation.Artifact(
-            type=generation.ARTIFACT_IMAGE, binary=buf.getvalue()
-        ),
-        parameters=generation.PromptParameters(init=init),
-    )
-
 
 def process_artifacts_from_answers(
     prefix: str,
     prompt: str,
     answers: Union[
         Generator[generation.Answer, None, None], Sequence[generation.Answer]
     ],
@@ -96,25 +70,25 @@
             elif artifact.type == generation.ARTIFACT_TEXT:
                 ext = ".pb.json"
                 contents = MessageToJson(artifact).encode("utf-8")
             else:
                 ext = ".pb"
                 contents = artifact.SerializeToString()
             out_p = truncate_fit(prefix, prompt, ext, int(artifact_start), idx, MAX_FILENAME_SZ)
-            is_allowed_type = filter_types is None or artifact_type_to_str(artifact.type) in filter_types
+            is_allowed_type = filter_types is None or artifact_type_to_string(artifact.type) in filter_types
             if write:
                 if is_allowed_type:
                     with open(out_p, "wb") as f:
                         f.write(bytes(contents))
                         if verbose:
-                            logger.info(f"wrote {artifact_type_to_str(artifact.type)} to {out_p}")
+                            logger.info(f"wrote {artifact_type_to_string(artifact.type)} to {out_p}")
                 else:
                     if verbose:
                         logger.info(
-                            f"skipping {artifact_type_to_str(artifact.type)} due to artifact type filter")
+                            f"skipping {artifact_type_to_string(artifact.type)} due to artifact type filter")
 
             yield (out_p, artifact)
             idx += 1
 
 
 class StabilityInference:
     def __init__(
@@ -138,15 +112,14 @@
             to fail immediately.
         """
         self.verbose = verbose
         self.engine = engine
         self.upscale_engine = upscale_engine
 
         self.grpc_args = {"wait_for_ready": wait_for_ready}
-
         if verbose:
             logger.info(f"Opening channel to {host}")
 
         call_credentials = []
 
         # Increase the max message size to 10MB to allow for larger images.
         max_message_size: int = os.getenv("MAX_MESSAGE_SIZE")
@@ -255,18 +228,18 @@
 
         # NB: Specifying schedule when there's no init image causes washed out results
         if init_image is not None:
             step_parameters['schedule'] = generation.ScheduleParameters(
                 start=start_schedule,
                 end=end_schedule,
             )
-            prompts += [image_to_prompt(init_image, init=True)]
+            prompts += [image_to_prompt(init_image)]
 
             if mask_image is not None:
-                prompts += [image_to_prompt(mask_image, mask=True)]
+                prompts += [image_to_prompt(mask_image, type=generation.ARTIFACT_MASK)]
 
 
         if guidance_prompt:
             if isinstance(guidance_prompt, str):
                 guidance_prompt = generation.Prompt(text=guidance_prompt)
             elif not isinstance(guidance_prompt, generation.Prompt):
                 raise ValueError("guidance_prompt must be a string or Prompt object")
@@ -356,15 +329,15 @@
             height=height,
             width=width,
             seed=[seed],
             steps=steps,
             parameters=[generation.StepParameter(**step_parameters)],
         )
 
-        prompts = [image_to_prompt(init_image, init=True)]
+        prompts = [image_to_prompt(init_image)]
 
         if prompt:
             if isinstance(prompt, str):
                 prompt = generation.Prompt(text=prompt)
             elif not isinstance(prompt, generation.Prompt):
                 raise ValueError("prompt must be a string or Prompt object")
             prompts.append(prompt)
@@ -399,15 +372,15 @@
 
         start = time.time()
         for answer in self.stub.Generate(rq, **self.grpc_args):
             duration = time.time() - start
             if self.verbose:
                 if len(answer.artifacts) > 0:
                     artifact_ts = [
-                        artifact_type_to_str(artifact.type)
+                        artifact_type_to_string(artifact.type)
                         for artifact in answer.artifacts
                     ]
                     logger.info(
                         f"Got answer {answer.answer_id} with artifact types {artifact_ts} in "
                         f"{duration:0.2f}s"
                     )
                 else:
@@ -442,25 +415,20 @@
             "[Deprecation Warning] instead do this:"
             "[Deprecation Warning]    $ python -m stability_sdk ...  "
         )
 
     STABILITY_HOST = os.getenv("STABILITY_HOST", "grpc.stability.ai:443")
     STABILITY_KEY = os.getenv("STABILITY_KEY", "")
 
-    if not STABILITY_HOST:
-        logger.warning("STABILITY_HOST environment variable needs to be set.")
-        sys.exit(1)
-
     if not STABILITY_KEY:
-        logger.warning(
-            "STABILITY_KEY environment variable needs to be set. You may"
-            " need to login to the Stability website to obtain the"
-            " API key."
+        print(
+            "Please enter your API key from dreamstudio.ai or set the "
+            "STABILITY_KEY environment variable to skip this prompt."
         )
-        sys.exit(1)
+        STABILITY_KEY = getpass.getpass("Enter your Stability API key: ")
 
     # CLI parsing
     parser = ArgumentParser()
     subparsers = parser.add_subparsers(dest='command')
 
     parser_upscale = subparsers.add_parser('upscale')
     parser_upscale.add_argument(
@@ -511,14 +479,20 @@
         type=str,
         help="engine to use for upscale",
         default="esrgan-v1-x2plus",
     )
     parser_upscale.add_argument(
         "prompt", nargs="*"
     )
+
+
+    parser_animate = subparsers.add_parser('animate')
+    parser_animate.add_argument("--gui", action="store_true", help="serve Gradio UI")
+    parser_animate.add_argument("--share", action="store_true", help="create shareable UI link")
+    parser_animate.add_argument("--output", "-o", type=str, default=".", help="root output folder")    
     
 
     parser_generate = subparsers.add_parser('generate')
     parser_generate.add_argument(
         "--height", "-H", type=int, default=512, help="[512] height of image"
     )
     parser_generate.add_argument(
@@ -597,18 +571,18 @@
     input_args = sys.argv[1:]
     command = None
     if len(input_args)>0:
         command = input_args[0]
     if command not in subparsers.choices.keys() and command != '-h' and command != '--help':
         logger.warning(f"command {command} not recognized, defaulting to 'generate'")
         logger.warning(
-        "[Deprecation Warning] The method you have used to invoke the sdk will be deprecated shortly."
-        "[Deprecation Warning] Please modify your code to call the sdk with the following syntax:"
-        "[Deprecation Warning] python -m stability_sdk <command> <args>"
-        "[Deprecation Warning] Where <command> is one of: upscale, generate"
+            "[Deprecation Warning] The method you have used to invoke the sdk will be deprecated shortly."
+            "[Deprecation Warning] Please modify your code to call the sdk with the following syntax:"
+            "[Deprecation Warning] python -m stability_sdk <command> <args>"
+            "[Deprecation Warning] Where <command> is one of: upscale, generate"
         )
         input_args = ['generate'] + input_args
       
     args = parser.parse_args(input_args)
     
     if args.command == "upscale":
         args.init_image = Image.open(args.init_image)
@@ -620,15 +594,15 @@
             "height": args.height,
             "width": args.width,
             "init_image": args.init_image,
             "steps": args.steps,
             "seed": args.seed,
             "cfg_scale": args.cfg_scale,
             "prompt": args.prompt,
-            }
+        }
         stability_api = StabilityInference(
             STABILITY_HOST, STABILITY_KEY, upscale_engine=args.engine, verbose=True
         )
         answers = stability_api.upscale(**request)
         artifacts = process_artifacts_from_answers(
             args.prefix, args.prompt, answers, write=not args.no_store, verbose=True,
             filter_types=args.artifact_types,
@@ -656,27 +630,39 @@
             "seed": args.seed,
             "samples": args.num_samples,
             "init_image": args.init_image,
             "mask_image": args.mask_image,
         }
 
         if args.sampler:
-            request["sampler"] = get_sampler_from_str(args.sampler)
+            request["sampler"] = sampler_from_string(args.sampler)
 
         if args.steps:
             request["steps"] = args.steps
 
         stability_api = StabilityInference(
             STABILITY_HOST, STABILITY_KEY, engine=args.engine, verbose=True
         )
         answers = stability_api.generate(args.prompt, **request)
         artifacts = process_artifacts_from_answers(
             args.prefix, args.prompt, answers, write=not args.no_store, verbose=True,
             filter_types=args.artifact_types,
         )
+    elif args.command == "animate":
+        if args.gui:
+            from .animation_ui import create_ui
+            from .api import Context
+            ui = create_ui(Context(STABILITY_HOST, STABILITY_KEY), args.output)
+            ui.queue(concurrency_count=2, max_size=2)
+            ui.launch(show_api=False, debug=True, height=768, share=args.share, show_error=True)
+            sys.exit(0)
+        else:
+            logger.warning("animate must be invoked with --gui")
+            sys.exit(1)
+
     
     if args.show:
         for artifact in open_images(artifacts, verbose=True):
             pass
     else:
         for artifact in artifacts:
             pass
```

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 import tensors_pb2 as tensors__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10generation.proto\x12\x07gooseai\x1a\x1cgoogle/protobuf/struct.proto\x1a\rtensors.proto\"/\n\x05Token\x12\x11\n\x04text\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\rB\x07\n\x05_text\"T\n\x06Tokens\x12\x1e\n\x06tokens\x18\x01 \x03(\x0b\x32\x0e.gooseai.Token\x12\x19\n\x0ctokenizer_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0f\n\r_tokenizer_id\"\xf3\x02\n\x08\x41rtifact\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\x04type\x18\x02 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x0c\n\x04mime\x18\x03 \x01(\t\x12\x12\n\x05magic\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x06\x62inary\x18\x05 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x06 \x01(\tH\x00\x12!\n\x06tokens\x18\x07 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12\x33\n\nclassifier\x18\x0b \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12!\n\x06tensor\x18\x0e \x01(\x0b\x32\x0f.tensors.TensorH\x00\x12\r\n\x05index\x18\x08 \x01(\r\x12,\n\rfinish_reason\x18\t \x01(\x0e\x32\x15.gooseai.FinishReason\x12\x0c\n\x04seed\x18\n \x01(\r\x12\x0c\n\x04uuid\x18\x0c \x01(\t\x12\x0c\n\x04size\x18\r \x01(\x04\x42\x06\n\x04\x64\x61taB\x08\n\x06_magic\"N\n\x10PromptParameters\x12\x11\n\x04init\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06weight\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x07\n\x05_initB\t\n\x07_weight\"\xaf\x01\n\x06Prompt\x12\x32\n\nparameters\x18\x01 \x01(\x0b\x32\x19.gooseai.PromptParametersH\x01\x88\x01\x01\x12\x0e\n\x04text\x18\x02 \x01(\tH\x00\x12!\n\x06tokens\x18\x03 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12%\n\x08\x61rtifact\x18\x04 \x01(\x0b\x32\x11.gooseai.ArtifactH\x00\x42\x08\n\x06promptB\r\n\x0b_parameters\"\xd7\x02\n\x11SamplerParameters\x12\x10\n\x03\x65ta\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0esampling_steps\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0flatent_channels\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12 \n\x13\x64ownsampling_factor\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tcfg_scale\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x1d\n\x10init_noise_scale\x18\x06 \x01(\x02H\x05\x88\x01\x01\x12\x1d\n\x10step_noise_scale\x18\x07 \x01(\x02H\x06\x88\x01\x01\x42\x06\n\x04_etaB\x11\n\x0f_sampling_stepsB\x12\n\x10_latent_channelsB\x16\n\x14_downsampling_factorB\x0c\n\n_cfg_scaleB\x13\n\x11_init_noise_scaleB\x13\n\x11_step_noise_scale\"\x8b\x01\n\x15\x43onditionerParameters\x12 \n\x13vector_adjust_prior\x18\x01 \x01(\tH\x00\x88\x01\x01\x12(\n\x0b\x63onditioner\x18\x02 \x01(\x0b\x32\x0e.gooseai.ModelH\x01\x88\x01\x01\x42\x16\n\x14_vector_adjust_priorB\x0e\n\x0c_conditioner\"j\n\x12ScheduleParameters\x12\x12\n\x05start\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x10\n\x03\x65nd\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05value\x18\x03 \x01(\x02H\x02\x88\x01\x01\x42\x08\n\x06_startB\x06\n\x04_endB\x08\n\x06_value\"\xe4\x01\n\rStepParameter\x12\x13\n\x0bscaled_step\x18\x01 \x01(\x02\x12\x30\n\x07sampler\x18\x02 \x01(\x0b\x32\x1a.gooseai.SamplerParametersH\x00\x88\x01\x01\x12\x32\n\x08schedule\x18\x03 \x01(\x0b\x32\x1b.gooseai.ScheduleParametersH\x01\x88\x01\x01\x12\x32\n\x08guidance\x18\x04 \x01(\x0b\x32\x1b.gooseai.GuidanceParametersH\x02\x88\x01\x01\x42\n\n\x08_samplerB\x0b\n\t_scheduleB\x0b\n\t_guidance\"\x97\x01\n\x05Model\x12\x30\n\x0c\x61rchitecture\x18\x01 \x01(\x0e\x32\x1a.gooseai.ModelArchitecture\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x02\x12\x18\n\x10semantic_version\x18\x05 \x01(\t\x12\r\n\x05\x61lias\x18\x06 \x01(\t\"\xbc\x01\n\x10\x43utoutParameters\x12*\n\x07\x63utouts\x18\x01 \x03(\x0b\x32\x19.gooseai.CutoutParameters\x12\x12\n\x05\x63ount\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04gray\x18\x03 \x01(\x02H\x01\x88\x01\x01\x12\x11\n\x04\x62lur\x18\x04 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsize_power\x18\x05 \x01(\x02H\x03\x88\x01\x01\x42\x08\n\x06_countB\x07\n\x05_grayB\x07\n\x05_blurB\r\n\x0b_size_power\"=\n\x1aGuidanceScheduleParameters\x12\x10\n\x08\x64uration\x18\x01 \x01(\x02\x12\r\n\x05value\x18\x02 \x01(\x02\"\x97\x02\n\x1aGuidanceInstanceParameters\x12\x1e\n\x06models\x18\x02 \x03(\x0b\x32\x0e.gooseai.Model\x12\x1e\n\x11guidance_strength\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x35\n\x08schedule\x18\x04 \x03(\x0b\x32#.gooseai.GuidanceScheduleParameters\x12/\n\x07\x63utouts\x18\x05 \x01(\x0b\x32\x19.gooseai.CutoutParametersH\x01\x88\x01\x01\x12$\n\x06prompt\x18\x06 \x01(\x0b\x32\x0f.gooseai.PromptH\x02\x88\x01\x01\x42\x14\n\x12_guidance_strengthB\n\n\x08_cutoutsB\t\n\x07_prompt\"~\n\x12GuidanceParameters\x12\x30\n\x0fguidance_preset\x18\x01 \x01(\x0e\x32\x17.gooseai.GuidancePreset\x12\x36\n\tinstances\x18\x02 \x03(\x0b\x32#.gooseai.GuidanceInstanceParameters\"n\n\rTransformType\x12.\n\tdiffusion\x18\x01 \x01(\x0e\x32\x19.gooseai.DiffusionSamplerH\x00\x12%\n\x08upscaler\x18\x02 \x01(\x0e\x32\x11.gooseai.UpscalerH\x00\x42\x06\n\x04type\"\xbd\x03\n\x0fImageParameters\x12\x13\n\x06height\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05width\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x0c\n\x04seed\x18\x03 \x03(\r\x12\x14\n\x07samples\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05steps\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12.\n\ttransform\x18\x06 \x01(\x0b\x32\x16.gooseai.TransformTypeH\x04\x88\x01\x01\x12*\n\nparameters\x18\x07 \x03(\x0b\x32\x16.gooseai.StepParameter\x12\x36\n\x10masked_area_init\x18\x08 \x01(\x0e\x32\x17.gooseai.MaskedAreaInitH\x05\x88\x01\x01\x12\x31\n\rweight_method\x18\t \x01(\x0e\x32\x15.gooseai.WeightMethodH\x06\x88\x01\x01\x12\x15\n\x08quantize\x18\n \x01(\x08H\x07\x88\x01\x01\x42\t\n\x07_heightB\x08\n\x06_widthB\n\n\x08_samplesB\x08\n\x06_stepsB\x0c\n\n_transformB\x13\n\x11_masked_area_initB\x10\n\x0e_weight_methodB\x0b\n\t_quantize\"J\n\x11\x43lassifierConcept\x12\x0f\n\x07\x63oncept\x18\x01 \x01(\t\x12\x16\n\tthreshold\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x0c\n\n_threshold\"\xf4\x01\n\x12\x43lassifierCategory\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x1a.gooseai.ClassifierConcept\x12\x17\n\nadjustment\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x0f.gooseai.ActionH\x01\x88\x01\x01\x12\x35\n\x0f\x63lassifier_mode\x18\x05 \x01(\x0e\x32\x17.gooseai.ClassifierModeH\x02\x88\x01\x01\x42\r\n\x0b_adjustmentB\t\n\x07_actionB\x12\n\x10_classifier_mode\"\xb8\x01\n\x14\x43lassifierParameters\x12/\n\ncategories\x18\x01 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12,\n\x07\x65xceeds\x18\x02 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12-\n\x0frealized_action\x18\x03 \x01(\x0e\x32\x0f.gooseai.ActionH\x00\x88\x01\x01\x42\x12\n\x10_realized_action\"]\n\x15InterpolateParameters\x12\x0e\n\x06ratios\x18\x01 \x03(\x02\x12+\n\x04mode\x18\x02 \x01(\x0e\x32\x18.gooseai.InterpolateModeH\x00\x88\x01\x01\x42\x07\n\x05_mode\"\x9c\x03\n\x14TransformColorAdjust\x12\x17\n\nbrightness\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x15\n\x08\x63ontrast\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x10\n\x03hue\x18\x03 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsaturation\x18\x04 \x01(\x02H\x03\x88\x01\x01\x12\x16\n\tlightness\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12+\n\x0bmatch_image\x18\x06 \x01(\x0b\x32\x11.gooseai.ArtifactH\x05\x88\x01\x01\x12\x30\n\nmatch_mode\x18\x07 \x01(\x0e\x32\x17.gooseai.ColorMatchModeH\x06\x88\x01\x01\x12\x19\n\x0cnoise_amount\x18\x08 \x01(\x02H\x07\x88\x01\x01\x12\x17\n\nnoise_seed\x18\t \x01(\rH\x08\x88\x01\x01\x42\r\n\x0b_brightnessB\x0b\n\t_contrastB\x06\n\x04_hueB\r\n\x0b_saturationB\x0c\n\n_lightnessB\x0e\n\x0c_match_imageB\r\n\x0b_match_modeB\x0f\n\r_noise_amountB\r\n\x0b_noise_seed\"\x8c\x01\n\x12TransformDepthCalc\x12\x19\n\x0c\x62lend_weight\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0b\x62lur_radius\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x14\n\x07reverse\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x0f\n\r_blend_weightB\x0e\n\x0c_blur_radiusB\n\n\x08_reverse\"#\n\x0fTransformMatrix\x12\x10\n\x04\x64\x61ta\x18\x01 \x03(\x02\x42\x02\x10\x01\"\x86\x02\n\x11TransformResample\x12(\n\x0b\x62order_mode\x18\x01 \x01(\x0e\x32\x13.gooseai.BorderMode\x12+\n\ttransform\x18\x02 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x35\n\x0eprev_transform\x18\x03 \x01(\x0b\x32\x18.gooseai.TransformMatrixH\x00\x88\x01\x01\x12\x17\n\ndepth_warp\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x18\n\x0b\x65xport_mask\x18\x05 \x01(\x08H\x02\x88\x01\x01\x42\x11\n\x0f_prev_transformB\r\n\x0b_depth_warpB\x0e\n\x0c_export_mask\"}\n\x10\x43\x61meraParameters\x12(\n\x0b\x63\x61mera_type\x18\x01 \x01(\x0e\x32\x13.gooseai.CameraType\x12\x12\n\nnear_plane\x18\x02 \x01(\x02\x12\x11\n\tfar_plane\x18\x03 \x01(\x02\x12\x10\n\x03\x66ov\x18\x04 \x01(\x02H\x00\x88\x01\x01\x42\x06\n\x04_fov\"\x82\x02\n\x13TransformCameraPose\x12\x36\n\x14world_to_view_matrix\x18\x01 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x34\n\x11\x63\x61mera_parameters\x18\x02 \x01(\x0b\x32\x19.gooseai.CameraParameters\x12\x12\n\ndo_prefill\x18\x05 \x01(\x08\x12.\n\x11image_render_mode\x18\x06 \x01(\x0e\x32\x13.gooseai.RenderMode\x12-\n\x10mask_render_mode\x18\x07 \x01(\x0e\x32\x13.gooseai.RenderModeJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"\xf1\x01\n\x13TransformParameters\x12\x35\n\x0c\x63olor_adjust\x18\x02 \x01(\x0b\x32\x1d.gooseai.TransformColorAdjustH\x00\x12\x31\n\ndepth_calc\x18\x04 \x01(\x0b\x32\x1b.gooseai.TransformDepthCalcH\x00\x12.\n\x08resample\x18\x05 \x01(\x0b\x32\x1a.gooseai.TransformResampleH\x00\x12\x33\n\x0b\x63\x61mera_pose\x18\x06 \x01(\x0b\x32\x1c.gooseai.TransformCameraPoseH\x00\x42\x0b\n\ttransform\"k\n\x0f\x41ssetParameters\x12$\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x14.gooseai.AssetAction\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x1e\n\x03use\x18\x03 \x01(\x0e\x32\x11.gooseai.AssetUse\"\x94\x01\n\nAnswerMeta\x12\x13\n\x06gpu_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x63pu_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07node_id\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tengine_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\t\n\x07_gpu_idB\t\n\x07_cpu_idB\n\n\x08_node_idB\x0c\n\n_engine_id\"\xa9\x01\n\x06\x41nswer\x12\x11\n\tanswer_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x10\n\x08received\x18\x03 \x01(\x04\x12\x0f\n\x07\x63reated\x18\x04 \x01(\x04\x12&\n\x04meta\x18\x06 \x01(\x0b\x32\x13.gooseai.AnswerMetaH\x00\x88\x01\x01\x12$\n\tartifacts\x18\x07 \x03(\x0b\x32\x11.gooseai.ArtifactB\x07\n\x05_meta\"A\n\x0b\x41nswerBatch\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12 \n\x07\x61nswers\x18\x02 \x03(\x0b\x32\x0f.gooseai.Answer\"\x8f\x04\n\x07Request\x12\x11\n\tengine_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12-\n\x0erequested_type\x18\x03 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x1f\n\x06prompt\x18\x04 \x03(\x0b\x32\x0f.gooseai.Prompt\x12)\n\x05image\x18\x05 \x01(\x0b\x32\x18.gooseai.ImageParametersH\x00\x12\x33\n\nclassifier\x18\x07 \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12)\n\x05\x61sset\x18\x08 \x01(\x0b\x32\x18.gooseai.AssetParametersH\x00\x12\x35\n\x0binterpolate\x18\x0b \x01(\x0b\x32\x1e.gooseai.InterpolateParametersH\x00\x12\x31\n\ttransform\x18\x0c \x01(\x0b\x32\x1c.gooseai.TransformParametersH\x00\x12\x38\n\x0b\x63onditioner\x18\x06 \x01(\x0b\x32\x1e.gooseai.ConditionerParametersH\x01\x88\x01\x01\x12-\n\x06\x65xtras\x18\xff\x0f \x01(\x0b\x32\x17.google.protobuf.StructH\x02\x88\x01\x01\x42\x08\n\x06paramsB\x0e\n\x0c_conditionerB\t\n\x07_extrasJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"w\n\x08OnStatus\x12%\n\x06reason\x18\x01 \x03(\x0e\x32\x15.gooseai.FinishReason\x12\x13\n\x06target\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x03 \x03(\x0e\x32\x14.gooseai.StageActionB\t\n\x07_target\"\\\n\x05Stage\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07request\x18\x02 \x01(\x0b\x32\x10.gooseai.Request\x12$\n\ton_status\x18\x03 \x03(\x0b\x32\x11.gooseai.OnStatus\"A\n\x0c\x43hainRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x1d\n\x05stage\x18\x02 \x03(\x0b\x32\x0e.gooseai.Stage*E\n\x0c\x46inishReason\x12\x08\n\x04NULL\x10\x00\x12\n\n\x06LENGTH\x10\x01\x12\x08\n\x04STOP\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\n\n\x06\x46ILTER\x10\x04*\xf8\x01\n\x0c\x41rtifactType\x12\x11\n\rARTIFACT_NONE\x10\x00\x12\x12\n\x0e\x41RTIFACT_IMAGE\x10\x01\x12\x12\n\x0e\x41RTIFACT_VIDEO\x10\x02\x12\x11\n\rARTIFACT_TEXT\x10\x03\x12\x13\n\x0f\x41RTIFACT_TOKENS\x10\x04\x12\x16\n\x12\x41RTIFACT_EMBEDDING\x10\x05\x12\x1c\n\x18\x41RTIFACT_CLASSIFICATIONS\x10\x06\x12\x11\n\rARTIFACT_MASK\x10\x07\x12\x13\n\x0f\x41RTIFACT_LATENT\x10\x08\x12\x13\n\x0f\x41RTIFACT_TENSOR\x10\t\x12\x12\n\x0e\x41RTIFACT_DEPTH\x10\n*g\n\x0eMaskedAreaInit\x12\x19\n\x15MASKED_AREA_INIT_ZERO\x10\x00\x12\x1b\n\x17MASKED_AREA_INIT_RANDOM\x10\x01\x12\x1d\n\x19MASKED_AREA_INIT_ORIGINAL\x10\x02*5\n\x0cWeightMethod\x12\x10\n\x0cTEXT_ENCODER\x10\x00\x12\x13\n\x0f\x43ROSS_ATTENTION\x10\x01*\x98\x02\n\x10\x44iffusionSampler\x12\x10\n\x0cSAMPLER_DDIM\x10\x00\x12\x10\n\x0cSAMPLER_DDPM\x10\x01\x12\x13\n\x0fSAMPLER_K_EULER\x10\x02\x12\x1d\n\x19SAMPLER_K_EULER_ANCESTRAL\x10\x03\x12\x12\n\x0eSAMPLER_K_HEUN\x10\x04\x12\x13\n\x0fSAMPLER_K_DPM_2\x10\x05\x12\x1d\n\x19SAMPLER_K_DPM_2_ANCESTRAL\x10\x06\x12\x11\n\rSAMPLER_K_LMS\x10\x07\x12 \n\x1cSAMPLER_K_DPMPP_2S_ANCESTRAL\x10\x08\x12\x16\n\x12SAMPLER_K_DPMPP_2M\x10\t\x12\x17\n\x13SAMPLER_K_DPMPP_SDE\x10\n*F\n\x08Upscaler\x12\x10\n\x0cUPSCALER_RGB\x10\x00\x12\x13\n\x0fUPSCALER_GFPGAN\x10\x01\x12\x13\n\x0fUPSCALER_ESRGAN\x10\x02*\xd8\x01\n\x0eGuidancePreset\x12\x18\n\x14GUIDANCE_PRESET_NONE\x10\x00\x12\x1a\n\x16GUIDANCE_PRESET_SIMPLE\x10\x01\x12\x1d\n\x19GUIDANCE_PRESET_FAST_BLUE\x10\x02\x12\x1e\n\x1aGUIDANCE_PRESET_FAST_GREEN\x10\x03\x12\x18\n\x14GUIDANCE_PRESET_SLOW\x10\x04\x12\x1a\n\x16GUIDANCE_PRESET_SLOWER\x10\x05\x12\x1b\n\x17GUIDANCE_PRESET_SLOWEST\x10\x06*\x91\x01\n\x11ModelArchitecture\x12\x1b\n\x17MODEL_ARCHITECTURE_NONE\x10\x00\x12\x1f\n\x1bMODEL_ARCHITECTURE_CLIP_VIT\x10\x01\x12\"\n\x1eMODEL_ARCHITECTURE_CLIP_RESNET\x10\x02\x12\x1a\n\x16MODEL_ARCHITECTURE_LDM\x10\x03*\xa2\x01\n\x06\x41\x63tion\x12\x16\n\x12\x41\x43TION_PASSTHROUGH\x10\x00\x12\x1f\n\x1b\x41\x43TION_REGENERATE_DUPLICATE\x10\x01\x12\x15\n\x11\x41\x43TION_REGENERATE\x10\x02\x12\x1e\n\x1a\x41\x43TION_OBFUSCATE_DUPLICATE\x10\x03\x12\x14\n\x10\x41\x43TION_OBFUSCATE\x10\x04\x12\x12\n\x0e\x41\x43TION_DISCARD\x10\x05*D\n\x0e\x43lassifierMode\x12\x17\n\x13\x43LSFR_MODE_ZEROSHOT\x10\x00\x12\x19\n\x15\x43LSFR_MODE_MULTICLASS\x10\x01*\x8c\x01\n\x0fInterpolateMode\x12\x16\n\x12INTERPOLATE_LINEAR\x10\x00\x12\x14\n\x10INTERPOLATE_RIFE\x10\x01\x12\x1a\n\x16INTERPOLATE_VAE_LINEAR\x10\x02\x12\x19\n\x15INTERPOLATE_VAE_SLERP\x10\x03\x12\x14\n\x10INTERPOLATE_FILM\x10\x04*l\n\nBorderMode\x12\x12\n\x0e\x42ORDER_REFLECT\x10\x00\x12\x14\n\x10\x42ORDER_REPLICATE\x10\x01\x12\x0f\n\x0b\x42ORDER_WRAP\x10\x02\x12\x0f\n\x0b\x42ORDER_ZERO\x10\x03\x12\x12\n\x0e\x42ORDER_PREFILL\x10\x04*O\n\x0e\x43olorMatchMode\x12\x13\n\x0f\x43OLOR_MATCH_HSV\x10\x00\x12\x13\n\x0f\x43OLOR_MATCH_LAB\x10\x01\x12\x13\n\x0f\x43OLOR_MATCH_RGB\x10\x02*=\n\nCameraType\x12\x16\n\x12\x43\x41MERA_PERSPECTIVE\x10\x00\x12\x17\n\x13\x43\x41MERA_ORTHOGRAPHIC\x10\x01*4\n\nRenderMode\x12\x0f\n\x0bRENDER_MESH\x10\x00\x12\x15\n\x11RENDER_POINTCLOUD\x10\x01*=\n\x0b\x41ssetAction\x12\r\n\tASSET_PUT\x10\x00\x12\r\n\tASSET_GET\x10\x01\x12\x10\n\x0c\x41SSET_DELETE\x10\x02*\x81\x01\n\x08\x41ssetUse\x12\x17\n\x13\x41SSET_USE_UNDEFINED\x10\x00\x12\x13\n\x0f\x41SSET_USE_INPUT\x10\x01\x12\x14\n\x10\x41SSET_USE_OUTPUT\x10\x02\x12\x1a\n\x16\x41SSET_USE_INTERMEDIATE\x10\x03\x12\x15\n\x11\x41SSET_USE_PROJECT\x10\x04*W\n\x0bStageAction\x12\x15\n\x11STAGE_ACTION_PASS\x10\x00\x12\x18\n\x14STAGE_ACTION_DISCARD\x10\x01\x12\x17\n\x13STAGE_ACTION_RETURN\x10\x02\x32\x83\x01\n\x11GenerationService\x12\x31\n\x08Generate\x12\x10.gooseai.Request\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x12;\n\rChainGenerate\x12\x15.gooseai.ChainRequest\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x42;Z9github.com/stability-ai/api-interfaces/gooseai/generationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10generation.proto\x12\x07gooseai\x1a\x1cgoogle/protobuf/struct.proto\x1a\rtensors.proto\"/\n\x05Token\x12\x11\n\x04text\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\rB\x07\n\x05_text\"T\n\x06Tokens\x12\x1e\n\x06tokens\x18\x01 \x03(\x0b\x32\x0e.gooseai.Token\x12\x19\n\x0ctokenizer_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0f\n\r_tokenizer_id\"\xf3\x02\n\x08\x41rtifact\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\x04type\x18\x02 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x0c\n\x04mime\x18\x03 \x01(\t\x12\x12\n\x05magic\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x06\x62inary\x18\x05 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x06 \x01(\tH\x00\x12!\n\x06tokens\x18\x07 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12\x33\n\nclassifier\x18\x0b \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12!\n\x06tensor\x18\x0e \x01(\x0b\x32\x0f.tensors.TensorH\x00\x12\r\n\x05index\x18\x08 \x01(\r\x12,\n\rfinish_reason\x18\t \x01(\x0e\x32\x15.gooseai.FinishReason\x12\x0c\n\x04seed\x18\n \x01(\r\x12\x0c\n\x04uuid\x18\x0c \x01(\t\x12\x0c\n\x04size\x18\r \x01(\x04\x42\x06\n\x04\x64\x61taB\x08\n\x06_magic\"N\n\x10PromptParameters\x12\x11\n\x04init\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06weight\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x07\n\x05_initB\t\n\x07_weight\"\xaf\x01\n\x06Prompt\x12\x32\n\nparameters\x18\x01 \x01(\x0b\x32\x19.gooseai.PromptParametersH\x01\x88\x01\x01\x12\x0e\n\x04text\x18\x02 \x01(\tH\x00\x12!\n\x06tokens\x18\x03 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12%\n\x08\x61rtifact\x18\x04 \x01(\x0b\x32\x11.gooseai.ArtifactH\x00\x42\x08\n\x06promptB\r\n\x0b_parameters\"\xd7\x02\n\x11SamplerParameters\x12\x10\n\x03\x65ta\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0esampling_steps\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0flatent_channels\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12 \n\x13\x64ownsampling_factor\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tcfg_scale\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x1d\n\x10init_noise_scale\x18\x06 \x01(\x02H\x05\x88\x01\x01\x12\x1d\n\x10step_noise_scale\x18\x07 \x01(\x02H\x06\x88\x01\x01\x42\x06\n\x04_etaB\x11\n\x0f_sampling_stepsB\x12\n\x10_latent_channelsB\x16\n\x14_downsampling_factorB\x0c\n\n_cfg_scaleB\x13\n\x11_init_noise_scaleB\x13\n\x11_step_noise_scale\"\x8b\x01\n\x15\x43onditionerParameters\x12 \n\x13vector_adjust_prior\x18\x01 \x01(\tH\x00\x88\x01\x01\x12(\n\x0b\x63onditioner\x18\x02 \x01(\x0b\x32\x0e.gooseai.ModelH\x01\x88\x01\x01\x42\x16\n\x14_vector_adjust_priorB\x0e\n\x0c_conditioner\"j\n\x12ScheduleParameters\x12\x12\n\x05start\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x10\n\x03\x65nd\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05value\x18\x03 \x01(\x02H\x02\x88\x01\x01\x42\x08\n\x06_startB\x06\n\x04_endB\x08\n\x06_value\"\xe4\x01\n\rStepParameter\x12\x13\n\x0bscaled_step\x18\x01 \x01(\x02\x12\x30\n\x07sampler\x18\x02 \x01(\x0b\x32\x1a.gooseai.SamplerParametersH\x00\x88\x01\x01\x12\x32\n\x08schedule\x18\x03 \x01(\x0b\x32\x1b.gooseai.ScheduleParametersH\x01\x88\x01\x01\x12\x32\n\x08guidance\x18\x04 \x01(\x0b\x32\x1b.gooseai.GuidanceParametersH\x02\x88\x01\x01\x42\n\n\x08_samplerB\x0b\n\t_scheduleB\x0b\n\t_guidance\"\x97\x01\n\x05Model\x12\x30\n\x0c\x61rchitecture\x18\x01 \x01(\x0e\x32\x1a.gooseai.ModelArchitecture\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x02\x12\x18\n\x10semantic_version\x18\x05 \x01(\t\x12\r\n\x05\x61lias\x18\x06 \x01(\t\"\xbc\x01\n\x10\x43utoutParameters\x12*\n\x07\x63utouts\x18\x01 \x03(\x0b\x32\x19.gooseai.CutoutParameters\x12\x12\n\x05\x63ount\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04gray\x18\x03 \x01(\x02H\x01\x88\x01\x01\x12\x11\n\x04\x62lur\x18\x04 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsize_power\x18\x05 \x01(\x02H\x03\x88\x01\x01\x42\x08\n\x06_countB\x07\n\x05_grayB\x07\n\x05_blurB\r\n\x0b_size_power\"=\n\x1aGuidanceScheduleParameters\x12\x10\n\x08\x64uration\x18\x01 \x01(\x02\x12\r\n\x05value\x18\x02 \x01(\x02\"\x97\x02\n\x1aGuidanceInstanceParameters\x12\x1e\n\x06models\x18\x02 \x03(\x0b\x32\x0e.gooseai.Model\x12\x1e\n\x11guidance_strength\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x35\n\x08schedule\x18\x04 \x03(\x0b\x32#.gooseai.GuidanceScheduleParameters\x12/\n\x07\x63utouts\x18\x05 \x01(\x0b\x32\x19.gooseai.CutoutParametersH\x01\x88\x01\x01\x12$\n\x06prompt\x18\x06 \x01(\x0b\x32\x0f.gooseai.PromptH\x02\x88\x01\x01\x42\x14\n\x12_guidance_strengthB\n\n\x08_cutoutsB\t\n\x07_prompt\"~\n\x12GuidanceParameters\x12\x30\n\x0fguidance_preset\x18\x01 \x01(\x0e\x32\x17.gooseai.GuidancePreset\x12\x36\n\tinstances\x18\x02 \x03(\x0b\x32#.gooseai.GuidanceInstanceParameters\"n\n\rTransformType\x12.\n\tdiffusion\x18\x01 \x01(\x0e\x32\x19.gooseai.DiffusionSamplerH\x00\x12%\n\x08upscaler\x18\x02 \x01(\x0e\x32\x11.gooseai.UpscalerH\x00\x42\x06\n\x04type\"\xbd\x03\n\x0fImageParameters\x12\x13\n\x06height\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05width\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x0c\n\x04seed\x18\x03 \x03(\r\x12\x14\n\x07samples\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05steps\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12.\n\ttransform\x18\x06 \x01(\x0b\x32\x16.gooseai.TransformTypeH\x04\x88\x01\x01\x12*\n\nparameters\x18\x07 \x03(\x0b\x32\x16.gooseai.StepParameter\x12\x36\n\x10masked_area_init\x18\x08 \x01(\x0e\x32\x17.gooseai.MaskedAreaInitH\x05\x88\x01\x01\x12\x31\n\rweight_method\x18\t \x01(\x0e\x32\x15.gooseai.WeightMethodH\x06\x88\x01\x01\x12\x15\n\x08quantize\x18\n \x01(\x08H\x07\x88\x01\x01\x42\t\n\x07_heightB\x08\n\x06_widthB\n\n\x08_samplesB\x08\n\x06_stepsB\x0c\n\n_transformB\x13\n\x11_masked_area_initB\x10\n\x0e_weight_methodB\x0b\n\t_quantize\"J\n\x11\x43lassifierConcept\x12\x0f\n\x07\x63oncept\x18\x01 \x01(\t\x12\x16\n\tthreshold\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x0c\n\n_threshold\"\xf4\x01\n\x12\x43lassifierCategory\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x1a.gooseai.ClassifierConcept\x12\x17\n\nadjustment\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x0f.gooseai.ActionH\x01\x88\x01\x01\x12\x35\n\x0f\x63lassifier_mode\x18\x05 \x01(\x0e\x32\x17.gooseai.ClassifierModeH\x02\x88\x01\x01\x42\r\n\x0b_adjustmentB\t\n\x07_actionB\x12\n\x10_classifier_mode\"\xb8\x01\n\x14\x43lassifierParameters\x12/\n\ncategories\x18\x01 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12,\n\x07\x65xceeds\x18\x02 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12-\n\x0frealized_action\x18\x03 \x01(\x0e\x32\x0f.gooseai.ActionH\x00\x88\x01\x01\x42\x12\n\x10_realized_action\"]\n\x15InterpolateParameters\x12\x0e\n\x06ratios\x18\x01 \x03(\x02\x12+\n\x04mode\x18\x02 \x01(\x0e\x32\x18.gooseai.InterpolateModeH\x00\x88\x01\x01\x42\x07\n\x05_mode\"\x9c\x03\n\x14TransformColorAdjust\x12\x17\n\nbrightness\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x15\n\x08\x63ontrast\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x10\n\x03hue\x18\x03 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsaturation\x18\x04 \x01(\x02H\x03\x88\x01\x01\x12\x16\n\tlightness\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12+\n\x0bmatch_image\x18\x06 \x01(\x0b\x32\x11.gooseai.ArtifactH\x05\x88\x01\x01\x12\x30\n\nmatch_mode\x18\x07 \x01(\x0e\x32\x17.gooseai.ColorMatchModeH\x06\x88\x01\x01\x12\x19\n\x0cnoise_amount\x18\x08 \x01(\x02H\x07\x88\x01\x01\x12\x17\n\nnoise_seed\x18\t \x01(\rH\x08\x88\x01\x01\x42\r\n\x0b_brightnessB\x0b\n\t_contrastB\x06\n\x04_hueB\r\n\x0b_saturationB\x0c\n\n_lightnessB\x0e\n\x0c_match_imageB\r\n\x0b_match_modeB\x0f\n\r_noise_amountB\r\n\x0b_noise_seed\"\x8c\x01\n\x12TransformDepthCalc\x12\x19\n\x0c\x62lend_weight\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0b\x62lur_radius\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x14\n\x07reverse\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x0f\n\r_blend_weightB\x0e\n\x0c_blur_radiusB\n\n\x08_reverse\"#\n\x0fTransformMatrix\x12\x10\n\x04\x64\x61ta\x18\x01 \x03(\x02\x42\x02\x10\x01\"\x86\x02\n\x11TransformResample\x12(\n\x0b\x62order_mode\x18\x01 \x01(\x0e\x32\x13.gooseai.BorderMode\x12+\n\ttransform\x18\x02 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x35\n\x0eprev_transform\x18\x03 \x01(\x0b\x32\x18.gooseai.TransformMatrixH\x00\x88\x01\x01\x12\x17\n\ndepth_warp\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x18\n\x0b\x65xport_mask\x18\x05 \x01(\x08H\x02\x88\x01\x01\x42\x11\n\x0f_prev_transformB\r\n\x0b_depth_warpB\x0e\n\x0c_export_mask\"}\n\x10\x43\x61meraParameters\x12(\n\x0b\x63\x61mera_type\x18\x01 \x01(\x0e\x32\x13.gooseai.CameraType\x12\x12\n\nnear_plane\x18\x02 \x01(\x02\x12\x11\n\tfar_plane\x18\x03 \x01(\x02\x12\x10\n\x03\x66ov\x18\x04 \x01(\x02H\x00\x88\x01\x01\x42\x06\n\x04_fov\"\xd9\x01\n\x13TransformCameraPose\x12\x36\n\x14world_to_view_matrix\x18\x01 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x34\n\x11\x63\x61mera_parameters\x18\x02 \x01(\x0b\x32\x19.gooseai.CameraParameters\x12\x12\n\ndo_prefill\x18\x05 \x01(\x08\x12(\n\x0brender_mode\x18\x08 \x01(\x0e\x32\x13.gooseai.RenderModeJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xf1\x01\n\x13TransformParameters\x12\x35\n\x0c\x63olor_adjust\x18\x02 \x01(\x0b\x32\x1d.gooseai.TransformColorAdjustH\x00\x12\x31\n\ndepth_calc\x18\x04 \x01(\x0b\x32\x1b.gooseai.TransformDepthCalcH\x00\x12.\n\x08resample\x18\x05 \x01(\x0b\x32\x1a.gooseai.TransformResampleH\x00\x12\x33\n\x0b\x63\x61mera_pose\x18\x06 \x01(\x0b\x32\x1c.gooseai.TransformCameraPoseH\x00\x42\x0b\n\ttransform\"k\n\x0f\x41ssetParameters\x12$\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x14.gooseai.AssetAction\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x1e\n\x03use\x18\x03 \x01(\x0e\x32\x11.gooseai.AssetUse\"\x94\x01\n\nAnswerMeta\x12\x13\n\x06gpu_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x63pu_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07node_id\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tengine_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\t\n\x07_gpu_idB\t\n\x07_cpu_idB\n\n\x08_node_idB\x0c\n\n_engine_id\"\xa9\x01\n\x06\x41nswer\x12\x11\n\tanswer_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x10\n\x08received\x18\x03 \x01(\x04\x12\x0f\n\x07\x63reated\x18\x04 \x01(\x04\x12&\n\x04meta\x18\x06 \x01(\x0b\x32\x13.gooseai.AnswerMetaH\x00\x88\x01\x01\x12$\n\tartifacts\x18\x07 \x03(\x0b\x32\x11.gooseai.ArtifactB\x07\n\x05_meta\"A\n\x0b\x41nswerBatch\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12 \n\x07\x61nswers\x18\x02 \x03(\x0b\x32\x0f.gooseai.Answer\"\x8f\x04\n\x07Request\x12\x11\n\tengine_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12-\n\x0erequested_type\x18\x03 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x1f\n\x06prompt\x18\x04 \x03(\x0b\x32\x0f.gooseai.Prompt\x12)\n\x05image\x18\x05 \x01(\x0b\x32\x18.gooseai.ImageParametersH\x00\x12\x33\n\nclassifier\x18\x07 \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12)\n\x05\x61sset\x18\x08 \x01(\x0b\x32\x18.gooseai.AssetParametersH\x00\x12\x35\n\x0binterpolate\x18\x0b \x01(\x0b\x32\x1e.gooseai.InterpolateParametersH\x00\x12\x31\n\ttransform\x18\x0c \x01(\x0b\x32\x1c.gooseai.TransformParametersH\x00\x12\x38\n\x0b\x63onditioner\x18\x06 \x01(\x0b\x32\x1e.gooseai.ConditionerParametersH\x01\x88\x01\x01\x12-\n\x06\x65xtras\x18\xff\x0f \x01(\x0b\x32\x17.google.protobuf.StructH\x02\x88\x01\x01\x42\x08\n\x06paramsB\x0e\n\x0c_conditionerB\t\n\x07_extrasJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"w\n\x08OnStatus\x12%\n\x06reason\x18\x01 \x03(\x0e\x32\x15.gooseai.FinishReason\x12\x13\n\x06target\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x03 \x03(\x0e\x32\x14.gooseai.StageActionB\t\n\x07_target\"\\\n\x05Stage\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07request\x18\x02 \x01(\x0b\x32\x10.gooseai.Request\x12$\n\ton_status\x18\x03 \x03(\x0b\x32\x11.gooseai.OnStatus\"A\n\x0c\x43hainRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x1d\n\x05stage\x18\x02 \x03(\x0b\x32\x0e.gooseai.Stage*E\n\x0c\x46inishReason\x12\x08\n\x04NULL\x10\x00\x12\n\n\x06LENGTH\x10\x01\x12\x08\n\x04STOP\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\n\n\x06\x46ILTER\x10\x04*\xf8\x01\n\x0c\x41rtifactType\x12\x11\n\rARTIFACT_NONE\x10\x00\x12\x12\n\x0e\x41RTIFACT_IMAGE\x10\x01\x12\x12\n\x0e\x41RTIFACT_VIDEO\x10\x02\x12\x11\n\rARTIFACT_TEXT\x10\x03\x12\x13\n\x0f\x41RTIFACT_TOKENS\x10\x04\x12\x16\n\x12\x41RTIFACT_EMBEDDING\x10\x05\x12\x1c\n\x18\x41RTIFACT_CLASSIFICATIONS\x10\x06\x12\x11\n\rARTIFACT_MASK\x10\x07\x12\x13\n\x0f\x41RTIFACT_LATENT\x10\x08\x12\x13\n\x0f\x41RTIFACT_TENSOR\x10\t\x12\x12\n\x0e\x41RTIFACT_DEPTH\x10\n*g\n\x0eMaskedAreaInit\x12\x19\n\x15MASKED_AREA_INIT_ZERO\x10\x00\x12\x1b\n\x17MASKED_AREA_INIT_RANDOM\x10\x01\x12\x1d\n\x19MASKED_AREA_INIT_ORIGINAL\x10\x02*5\n\x0cWeightMethod\x12\x10\n\x0cTEXT_ENCODER\x10\x00\x12\x13\n\x0f\x43ROSS_ATTENTION\x10\x01*\x98\x02\n\x10\x44iffusionSampler\x12\x10\n\x0cSAMPLER_DDIM\x10\x00\x12\x10\n\x0cSAMPLER_DDPM\x10\x01\x12\x13\n\x0fSAMPLER_K_EULER\x10\x02\x12\x1d\n\x19SAMPLER_K_EULER_ANCESTRAL\x10\x03\x12\x12\n\x0eSAMPLER_K_HEUN\x10\x04\x12\x13\n\x0fSAMPLER_K_DPM_2\x10\x05\x12\x1d\n\x19SAMPLER_K_DPM_2_ANCESTRAL\x10\x06\x12\x11\n\rSAMPLER_K_LMS\x10\x07\x12 \n\x1cSAMPLER_K_DPMPP_2S_ANCESTRAL\x10\x08\x12\x16\n\x12SAMPLER_K_DPMPP_2M\x10\t\x12\x17\n\x13SAMPLER_K_DPMPP_SDE\x10\n*F\n\x08Upscaler\x12\x10\n\x0cUPSCALER_RGB\x10\x00\x12\x13\n\x0fUPSCALER_GFPGAN\x10\x01\x12\x13\n\x0fUPSCALER_ESRGAN\x10\x02*\xd8\x01\n\x0eGuidancePreset\x12\x18\n\x14GUIDANCE_PRESET_NONE\x10\x00\x12\x1a\n\x16GUIDANCE_PRESET_SIMPLE\x10\x01\x12\x1d\n\x19GUIDANCE_PRESET_FAST_BLUE\x10\x02\x12\x1e\n\x1aGUIDANCE_PRESET_FAST_GREEN\x10\x03\x12\x18\n\x14GUIDANCE_PRESET_SLOW\x10\x04\x12\x1a\n\x16GUIDANCE_PRESET_SLOWER\x10\x05\x12\x1b\n\x17GUIDANCE_PRESET_SLOWEST\x10\x06*\x91\x01\n\x11ModelArchitecture\x12\x1b\n\x17MODEL_ARCHITECTURE_NONE\x10\x00\x12\x1f\n\x1bMODEL_ARCHITECTURE_CLIP_VIT\x10\x01\x12\"\n\x1eMODEL_ARCHITECTURE_CLIP_RESNET\x10\x02\x12\x1a\n\x16MODEL_ARCHITECTURE_LDM\x10\x03*\xa2\x01\n\x06\x41\x63tion\x12\x16\n\x12\x41\x43TION_PASSTHROUGH\x10\x00\x12\x1f\n\x1b\x41\x43TION_REGENERATE_DUPLICATE\x10\x01\x12\x15\n\x11\x41\x43TION_REGENERATE\x10\x02\x12\x1e\n\x1a\x41\x43TION_OBFUSCATE_DUPLICATE\x10\x03\x12\x14\n\x10\x41\x43TION_OBFUSCATE\x10\x04\x12\x12\n\x0e\x41\x43TION_DISCARD\x10\x05*D\n\x0e\x43lassifierMode\x12\x17\n\x13\x43LSFR_MODE_ZEROSHOT\x10\x00\x12\x19\n\x15\x43LSFR_MODE_MULTICLASS\x10\x01*\x8c\x01\n\x0fInterpolateMode\x12\x16\n\x12INTERPOLATE_LINEAR\x10\x00\x12\x14\n\x10INTERPOLATE_RIFE\x10\x01\x12\x1a\n\x16INTERPOLATE_VAE_LINEAR\x10\x02\x12\x19\n\x15INTERPOLATE_VAE_SLERP\x10\x03\x12\x14\n\x10INTERPOLATE_FILM\x10\x04*l\n\nBorderMode\x12\x12\n\x0e\x42ORDER_REFLECT\x10\x00\x12\x14\n\x10\x42ORDER_REPLICATE\x10\x01\x12\x0f\n\x0b\x42ORDER_WRAP\x10\x02\x12\x0f\n\x0b\x42ORDER_ZERO\x10\x03\x12\x12\n\x0e\x42ORDER_PREFILL\x10\x04*O\n\x0e\x43olorMatchMode\x12\x13\n\x0f\x43OLOR_MATCH_HSV\x10\x00\x12\x13\n\x0f\x43OLOR_MATCH_LAB\x10\x01\x12\x13\n\x0f\x43OLOR_MATCH_RGB\x10\x02*=\n\nCameraType\x12\x16\n\x12\x43\x41MERA_PERSPECTIVE\x10\x00\x12\x17\n\x13\x43\x41MERA_ORTHOGRAPHIC\x10\x01*4\n\nRenderMode\x12\x0f\n\x0bRENDER_MESH\x10\x00\x12\x15\n\x11RENDER_POINTCLOUD\x10\x01*=\n\x0b\x41ssetAction\x12\r\n\tASSET_PUT\x10\x00\x12\r\n\tASSET_GET\x10\x01\x12\x10\n\x0c\x41SSET_DELETE\x10\x02*\x81\x01\n\x08\x41ssetUse\x12\x17\n\x13\x41SSET_USE_UNDEFINED\x10\x00\x12\x13\n\x0f\x41SSET_USE_INPUT\x10\x01\x12\x14\n\x10\x41SSET_USE_OUTPUT\x10\x02\x12\x1a\n\x16\x41SSET_USE_INTERMEDIATE\x10\x03\x12\x15\n\x11\x41SSET_USE_PROJECT\x10\x04*W\n\x0bStageAction\x12\x15\n\x11STAGE_ACTION_PASS\x10\x00\x12\x18\n\x14STAGE_ACTION_DISCARD\x10\x01\x12\x17\n\x13STAGE_ACTION_RETURN\x10\x02\x32\x83\x01\n\x11GenerationService\x12\x31\n\x08Generate\x12\x10.gooseai.Request\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x12;\n\rChainGenerate\x12\x15.gooseai.ChainRequest\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x42;Z9github.com/stability-ai/api-interfaces/gooseai/generationb\x06proto3')
 
 _FINISHREASON = DESCRIPTOR.enum_types_by_name['FinishReason']
 FinishReason = enum_type_wrapper.EnumTypeWrapper(_FINISHREASON)
 _ARTIFACTTYPE = DESCRIPTOR.enum_types_by_name['ArtifactType']
 ArtifactType = enum_type_wrapper.EnumTypeWrapper(_ARTIFACTTYPE)
 _MASKEDAREAINIT = DESCRIPTOR.enum_types_by_name['MaskedAreaInit']
 MaskedAreaInit = enum_type_wrapper.EnumTypeWrapper(_MASKEDAREAINIT)
@@ -422,50 +422,50 @@
 _GENERATIONSERVICE = DESCRIPTOR.services_by_name['GenerationService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z9github.com/stability-ai/api-interfaces/gooseai/generation'
   _TRANSFORMMATRIX.fields_by_name['data']._options = None
   _TRANSFORMMATRIX.fields_by_name['data']._serialized_options = b'\020\001'
-  _FINISHREASON._serialized_start=6454
-  _FINISHREASON._serialized_end=6523
-  _ARTIFACTTYPE._serialized_start=6526
-  _ARTIFACTTYPE._serialized_end=6774
-  _MASKEDAREAINIT._serialized_start=6776
-  _MASKEDAREAINIT._serialized_end=6879
-  _WEIGHTMETHOD._serialized_start=6881
-  _WEIGHTMETHOD._serialized_end=6934
-  _DIFFUSIONSAMPLER._serialized_start=6937
-  _DIFFUSIONSAMPLER._serialized_end=7217
-  _UPSCALER._serialized_start=7219
-  _UPSCALER._serialized_end=7289
-  _GUIDANCEPRESET._serialized_start=7292
-  _GUIDANCEPRESET._serialized_end=7508
-  _MODELARCHITECTURE._serialized_start=7511
-  _MODELARCHITECTURE._serialized_end=7656
-  _ACTION._serialized_start=7659
-  _ACTION._serialized_end=7821
-  _CLASSIFIERMODE._serialized_start=7823
-  _CLASSIFIERMODE._serialized_end=7891
-  _INTERPOLATEMODE._serialized_start=7894
-  _INTERPOLATEMODE._serialized_end=8034
-  _BORDERMODE._serialized_start=8036
-  _BORDERMODE._serialized_end=8144
-  _COLORMATCHMODE._serialized_start=8146
-  _COLORMATCHMODE._serialized_end=8225
-  _CAMERATYPE._serialized_start=8227
-  _CAMERATYPE._serialized_end=8288
-  _RENDERMODE._serialized_start=8290
-  _RENDERMODE._serialized_end=8342
-  _ASSETACTION._serialized_start=8344
-  _ASSETACTION._serialized_end=8405
-  _ASSETUSE._serialized_start=8408
-  _ASSETUSE._serialized_end=8537
-  _STAGEACTION._serialized_start=8539
-  _STAGEACTION._serialized_end=8626
+  _FINISHREASON._serialized_start=6413
+  _FINISHREASON._serialized_end=6482
+  _ARTIFACTTYPE._serialized_start=6485
+  _ARTIFACTTYPE._serialized_end=6733
+  _MASKEDAREAINIT._serialized_start=6735
+  _MASKEDAREAINIT._serialized_end=6838
+  _WEIGHTMETHOD._serialized_start=6840
+  _WEIGHTMETHOD._serialized_end=6893
+  _DIFFUSIONSAMPLER._serialized_start=6896
+  _DIFFUSIONSAMPLER._serialized_end=7176
+  _UPSCALER._serialized_start=7178
+  _UPSCALER._serialized_end=7248
+  _GUIDANCEPRESET._serialized_start=7251
+  _GUIDANCEPRESET._serialized_end=7467
+  _MODELARCHITECTURE._serialized_start=7470
+  _MODELARCHITECTURE._serialized_end=7615
+  _ACTION._serialized_start=7618
+  _ACTION._serialized_end=7780
+  _CLASSIFIERMODE._serialized_start=7782
+  _CLASSIFIERMODE._serialized_end=7850
+  _INTERPOLATEMODE._serialized_start=7853
+  _INTERPOLATEMODE._serialized_end=7993
+  _BORDERMODE._serialized_start=7995
+  _BORDERMODE._serialized_end=8103
+  _COLORMATCHMODE._serialized_start=8105
+  _COLORMATCHMODE._serialized_end=8184
+  _CAMERATYPE._serialized_start=8186
+  _CAMERATYPE._serialized_end=8247
+  _RENDERMODE._serialized_start=8249
+  _RENDERMODE._serialized_end=8301
+  _ASSETACTION._serialized_start=8303
+  _ASSETACTION._serialized_end=8364
+  _ASSETUSE._serialized_start=8367
+  _ASSETUSE._serialized_end=8496
+  _STAGEACTION._serialized_start=8498
+  _STAGEACTION._serialized_end=8585
   _TOKEN._serialized_start=74
   _TOKEN._serialized_end=121
   _TOKENS._serialized_start=123
   _TOKENS._serialized_end=207
   _ARTIFACT._serialized_start=210
   _ARTIFACT._serialized_end=581
   _PROMPTPARAMETERS._serialized_start=583
@@ -509,29 +509,29 @@
   _TRANSFORMMATRIX._serialized_start=4209
   _TRANSFORMMATRIX._serialized_end=4244
   _TRANSFORMRESAMPLE._serialized_start=4247
   _TRANSFORMRESAMPLE._serialized_end=4509
   _CAMERAPARAMETERS._serialized_start=4511
   _CAMERAPARAMETERS._serialized_end=4636
   _TRANSFORMCAMERAPOSE._serialized_start=4639
-  _TRANSFORMCAMERAPOSE._serialized_end=4897
-  _TRANSFORMPARAMETERS._serialized_start=4900
-  _TRANSFORMPARAMETERS._serialized_end=5141
-  _ASSETPARAMETERS._serialized_start=5143
-  _ASSETPARAMETERS._serialized_end=5250
-  _ANSWERMETA._serialized_start=5253
-  _ANSWERMETA._serialized_end=5401
-  _ANSWER._serialized_start=5404
-  _ANSWER._serialized_end=5573
-  _ANSWERBATCH._serialized_start=5575
-  _ANSWERBATCH._serialized_end=5640
-  _REQUEST._serialized_start=5643
-  _REQUEST._serialized_end=6170
-  _ONSTATUS._serialized_start=6172
-  _ONSTATUS._serialized_end=6291
-  _STAGE._serialized_start=6293
-  _STAGE._serialized_end=6385
-  _CHAINREQUEST._serialized_start=6387
-  _CHAINREQUEST._serialized_end=6452
-  _GENERATIONSERVICE._serialized_start=8629
-  _GENERATIONSERVICE._serialized_end=8760
+  _TRANSFORMCAMERAPOSE._serialized_end=4856
+  _TRANSFORMPARAMETERS._serialized_start=4859
+  _TRANSFORMPARAMETERS._serialized_end=5100
+  _ASSETPARAMETERS._serialized_start=5102
+  _ASSETPARAMETERS._serialized_end=5209
+  _ANSWERMETA._serialized_start=5212
+  _ANSWERMETA._serialized_end=5360
+  _ANSWER._serialized_start=5363
+  _ANSWER._serialized_end=5532
+  _ANSWERBATCH._serialized_start=5534
+  _ANSWERBATCH._serialized_end=5599
+  _REQUEST._serialized_start=5602
+  _REQUEST._serialized_end=6129
+  _ONSTATUS._serialized_start=6131
+  _ONSTATUS._serialized_end=6250
+  _STAGE._serialized_start=6252
+  _STAGE._serialized_end=6344
+  _CHAINREQUEST._serialized_start=6346
+  _CHAINREQUEST._serialized_end=6411
+  _GENERATIONSERVICE._serialized_start=8588
+  _GENERATIONSERVICE._serialized_end=8719
 # @@protoc_insertion_point(module_scope)
```

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,24 @@
                 response_deserializer=project__pb2.Project.FromString,
                 )
         self.Delete = channel.unary_unary(
                 '/gooseai.ProjectService/Delete',
                 request_serializer=project__pb2.DeleteProjectRequest.SerializeToString,
                 response_deserializer=project__pb2.Project.FromString,
                 )
+        self.TagAssets = channel.unary_unary(
+                '/gooseai.ProjectService/TagAssets',
+                request_serializer=project__pb2.TagAssetsRequest.SerializeToString,
+                response_deserializer=project__pb2.TagAssetsResponse.FromString,
+                )
+        self.UntagAssets = channel.unary_unary(
+                '/gooseai.ProjectService/UntagAssets',
+                request_serializer=project__pb2.UntagAssetsRequest.SerializeToString,
+                response_deserializer=project__pb2.UntagAssetsResponse.FromString,
+                )
         self.QueryAssets = channel.unary_unary(
                 '/gooseai.ProjectService/QueryAssets',
                 request_serializer=project__pb2.QueryAssetsRequest.SerializeToString,
                 response_deserializer=project__pb2.QueryAssetsResponse.FromString,
                 )
         self.DeleteAssets = channel.unary_unary(
                 '/gooseai.ProjectService/DeleteAssets',
@@ -91,14 +101,27 @@
     def Delete(self, request, context):
         """Delete a project
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def TagAssets(self, request, context):
+        """Add or remove tags from an asset
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UntagAssets(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def QueryAssets(self, request, context):
         """Query the assets of a project, with additional filtering
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -133,14 +156,24 @@
                     response_serializer=project__pb2.Project.SerializeToString,
             ),
             'Delete': grpc.unary_unary_rpc_method_handler(
                     servicer.Delete,
                     request_deserializer=project__pb2.DeleteProjectRequest.FromString,
                     response_serializer=project__pb2.Project.SerializeToString,
             ),
+            'TagAssets': grpc.unary_unary_rpc_method_handler(
+                    servicer.TagAssets,
+                    request_deserializer=project__pb2.TagAssetsRequest.FromString,
+                    response_serializer=project__pb2.TagAssetsResponse.SerializeToString,
+            ),
+            'UntagAssets': grpc.unary_unary_rpc_method_handler(
+                    servicer.UntagAssets,
+                    request_deserializer=project__pb2.UntagAssetsRequest.FromString,
+                    response_serializer=project__pb2.UntagAssetsResponse.SerializeToString,
+            ),
             'QueryAssets': grpc.unary_unary_rpc_method_handler(
                     servicer.QueryAssets,
                     request_deserializer=project__pb2.QueryAssetsRequest.FromString,
                     response_serializer=project__pb2.QueryAssetsResponse.SerializeToString,
             ),
             'DeleteAssets': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteAssets,
@@ -242,14 +275,48 @@
         return grpc.experimental.unary_unary(request, target, '/gooseai.ProjectService/Delete',
             project__pb2.DeleteProjectRequest.SerializeToString,
             project__pb2.Project.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def TagAssets(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/gooseai.ProjectService/TagAssets',
+            project__pb2.TagAssetsRequest.SerializeToString,
+            project__pb2.TagAssetsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UntagAssets(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/gooseai.ProjectService/UntagAssets',
+            project__pb2.UntagAssetsRequest.SerializeToString,
+            project__pb2.UntagAssetsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def QueryAssets(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py` & `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.7.0/src/stability_sdk.egg-info/PKG-INFO` & `stability-sdk-0.8.0/src/stability_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
@@ -25,14 +25,16 @@
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Raster-Based
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: anim
+Provides-Extra: anim_ui
 License-File: LICENSE
 
 # stability-sdk
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stability-ai/stability-sdk/blob/main/nbs/demo_colab.ipynb)
 
 Client implementations that interact with the Stability API. 
@@ -62,14 +64,22 @@
 `python3 -m stability_sdk generate -W 512 -H 512 "A stunning house."`
 
 It will generate and put PNGs in your current directory.
 
 To upscale:
 `python3 -m stability_sdk upscale -i "/path/to/image.png"`
 
+## Animation UI
+
+Install with 
+`pip install stability-sdk[anim_ui]`
+
+Then run with 
+`python3 -m stability_sdk animate --gui`
+
 ## SDK Usage
 
 Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
@@ -86,15 +96,15 @@
 options:
   -h, --help            show this help message and exit
   --height HEIGHT, -H HEIGHT
                         [512] height of image
   --width WIDTH, -W WIDTH
                         [512] width of image
   --start_schedule START_SCHEDULE
-                        [0.5] start schedule for init image (must be greater than 0, 1 is full strength
+                        [0.5] start schedule for init image (must be greater than 0; 1 is full strength
                         text prompt, no trace of image)
   --end_schedule END_SCHEDULE
                         [0.01] end schedule for init image
   --cfg_scale CFG_SCALE, -C CFG_SCALE
                         [7.0] CFG scale factor
   --sampler SAMPLER, -A SAMPLER
                         [auto-select] (ddim, plms, k_euler, k_euler_ancestral, k_heun, k_dpm_2,
@@ -160,12 +170,13 @@
 
 - [protobuf spec](https://github.com/Stability-AI/api-interfaces/blob/main/src/proto/)
 
 ## Community-contributed clients
 
 * Typescript client: https://github.com/jakiestfu/stability-ts
 * Guide to building for Ruby: https://github.com/kmcphillips/stability-sdk/blob/main/src/ruby/README.md
+* C# client: https://github.com/Katarzyna-Kadziolka/StabilityClient.Net
 
 ## Stability API TOS
 
 Usage of the Stability API falls under the [STABILITY AI API Terms of Service.
 ](https://platform.stability.ai/docs/terms-of-service)
```

### Comparing `stability-sdk-0.7.0/src/stability_sdk.egg-info/SOURCES.txt` & `stability-sdk-0.8.0/src/stability_sdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/stability_sdk/__init__.py
 src/stability_sdk/__main__.py
+src/stability_sdk/animation.py
+src/stability_sdk/animation_ui.py
+src/stability_sdk/api.py
 src/stability_sdk/client.py
+src/stability_sdk/matrix.py
 src/stability_sdk/utils.py
 src/stability_sdk.egg-info/PKG-INFO
 src/stability_sdk.egg-info/SOURCES.txt
 src/stability_sdk.egg-info/dependency_links.txt
 src/stability_sdk.egg-info/requires.txt
 src/stability_sdk.egg-info/top_level.txt
 src/stability_sdk/interfaces/__init__.py
@@ -26,9 +30,11 @@
 src/stability_sdk/interfaces/src/tensorizer/__init__.py
 src/stability_sdk/interfaces/src/tensorizer/protobuf.py
 src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
 src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
 src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
 src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
 src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+tests/test_animator.py
+tests/test_api.py
 tests/test_client.py
 tests/test_utils.py
```

### Comparing `stability-sdk-0.7.0/tests/test_client.py` & `stability-sdk-0.8.0/tests/test_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,32 @@
-import pytest
 from PIL import Image
+from typing import Generator
 
 from stability_sdk import client
-import stability_sdk.interfaces.gooseai.generation.generation_pb2 as generation
-import stability_sdk.interfaces.gooseai.generation.generation_pb2_grpc as generation_grpc
-
-import grpc
-
-# feel like we should be using this, not sure how/where
-import grpc_testing
+from stability_sdk.api import generation
 
-from typing import Generator
-
-def test_client_import():
-    from stability_sdk import client
-    assert True
 
 def test_StabilityInference_init():
-    class_instance = client.StabilityInference(key='thisIsNotARealKey')
+    _ = client.StabilityInference(key='thisIsNotARealKey')
     assert True
 
-def test_StabilityInference_init_nokey_error():
-    try:
-        class_instance = client.StabilityInference()
-        assert False
-    except ValueError:
-        assert True
-
 def test_StabilityInference_init_nokey_insecure_host():
-    class_instance = client.StabilityInference(host='foo.bar.baz')
+    _ = client.StabilityInference(host='foo.bar.baz')
     assert True
 
-def test_image_to_prompt():
-    im = Image.new('RGB',(1,1))
-    prompt = client.image_to_prompt(im, init=False, mask=False)
-    assert isinstance(prompt, generation.Prompt)
-
 def test_image_to_prompt_init():
-    im = Image.new('RGB',(1,1))
-    prompt = client.image_to_prompt(im, init=True, mask=False)
+    im = Image.new('RGB', (1,1))
+    prompt = client.image_to_prompt(im)
     assert isinstance(prompt, generation.Prompt)
 
 def test_image_to_prompt_mask():
-    im = Image.new('RGB',(1,1))
-    prompt = client.image_to_prompt(im, init=False, mask=True)
+    im = Image.new('RGB', (1,1))
+    prompt = client.image_to_prompt(im, type=generation.ARTIFACT_MASK)
     assert isinstance(prompt, generation.Prompt)
 
-def test_image_to_prompt_init_mask():
-    im = Image.new('RGB',(1,1))
-    try:
-        prompt = client.image_to_prompt(im, init=True, mask=True)
-        assert False
-    except ValueError:
-        assert True
-
-
 def test_server_mocking(grpc_server, grpc_addr):
     class_instance = client.StabilityInference(host=grpc_addr[0])
     response = class_instance.generate(prompt="foo bar")
     print(response)
     # might need this link later:
     # - https://stackoverflow.com/questions/54541338/calling-function-that-yields-from-a-pytest-fixture
     assert isinstance(response, Generator)
```

