# Comparing `tmp/ultralytics-8.0.97.tar.gz` & `tmp/ultralytics-8.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.0.97.tar", last modified: Tue May  9 19:22:34 2023, max compression
+gzip compressed data, was "ultralytics-8.0.98.tar", last modified: Wed May 10 23:16:51 2023, max compression
```

## Comparing `ultralytics-8.0.97.tar` & `ultralytics-8.0.98.tar`

### file list

```diff
@@ -1,180 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.956794 ultralytics-8.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-09 19:20:55.000000 ultralytics-8.0.97/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 19:20:55.000000 ultralytics-8.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-09 19:20:55.000000 ultralytics-8.0.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-09 19:22:34.956794 ultralytics-8.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-09 19:20:55.000000 ultralytics-8.0.97/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-09 19:20:55.000000 ultralytics-8.0.97/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-09 19:20:55.000000 ultralytics-8.0.97/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-09 19:22:34.956794 ultralytics-8.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-09 19:20:55.000000 ultralytics-8.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.936794 ultralytics-8.0.97/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-09 19:20:55.000000 ultralytics-8.0.97/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-09 19:20:55.000000 ultralytics-8.0.97/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-09 19:20:55.000000 ultralytics-8.0.97/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.936794 ultralytics-8.0.97/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.940794 ultralytics-8.0.97/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.940794 ultralytics-8.0.97/ultralytics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/datasets/xView.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.940794 ultralytics-8.0.97/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.936794 ultralytics-8.0.97/ultralytics/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.940794 ultralytics-8.0.97/ultralytics/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.940794 ultralytics-8.0.97/ultralytics/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.944794 ultralytics-8.0.97/ultralytics/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.944794 ultralytics-8.0.97/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24243 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/nn/autobackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/nn/autoshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/nn/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.944794 ultralytics-8.0.97/ultralytics/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.944794 ultralytics-8.0.97/ultralytics/tracker/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/cfg/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/cfg/bytetrack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.944794 ultralytics-8.0.97/ultralytics/tracker/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/trackers/byte_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.944794 ultralytics-8.0.97/ultralytics/tracker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/tracker/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.944794 ultralytics-8.0.97/ultralytics/vit/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.948794 ultralytics-8.0.97/ultralytics/vit/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/autosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.948794 ultralytics-8.0.97/ultralytics/vit/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/modules/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/modules/prompt_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/vit/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.948794 ultralytics-8.0.97/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.948794 ultralytics-8.0.97/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.948794 ultralytics-8.0.97/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.948794 ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/stream_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/v5augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/v5loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.952794 ultralytics-8.0.97/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.952794 ultralytics-8.0.97/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.952794 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20019 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.952794 ultralytics-8.0.97/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.956794 ultralytics-8.0.97/ultralytics/yolo/v8/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.956794 ultralytics-8.0.97/ultralytics/yolo/v8/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/detect/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.956794 ultralytics-8.0.97/ultralytics/yolo/v8/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.956794 ultralytics-8.0.97/ultralytics/yolo/v8/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-09 19:20:55.000000 ultralytics-8.0.97/ultralytics/yolo/v8/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:22:34.940794 ultralytics-8.0.97/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-09 19:22:34.000000 ultralytics-8.0.97/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-09 19:22:34.000000 ultralytics-8.0.97/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:22:34.000000 ultralytics-8.0.97/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 19:22:34.000000 ultralytics-8.0.97/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-09 19:22:34.000000 ultralytics-8.0.97/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 19:22:34.000000 ultralytics-8.0.97/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.723256 ultralytics-8.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-10 23:15:33.000000 ultralytics-8.0.98/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-10 23:15:33.000000 ultralytics-8.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-10 23:15:33.000000 ultralytics-8.0.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-10 23:16:51.723256 ultralytics-8.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-10 23:15:33.000000 ultralytics-8.0.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-05-10 23:15:33.000000 ultralytics-8.0.98/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-10 23:15:33.000000 ultralytics-8.0.98/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-10 23:16:51.723256 ultralytics-8.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-10 23:15:33.000000 ultralytics-8.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.703256 ultralytics-8.0.98/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-10 23:15:33.000000 ultralytics-8.0.98/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-10 23:15:33.000000 ultralytics-8.0.98/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-10 23:15:33.000000 ultralytics-8.0.98/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.703256 ultralytics-8.0.98/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/datasets/xView.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.699256 ultralytics-8.0.98/ultralytics/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/rt-detr/rt-detr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/rt-detr/rt-detr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.707256 ultralytics-8.0.98/ultralytics/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/autobackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/autoshape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28327 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/cfg/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/cfg/bytetrack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/trackers/byte_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/tracker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/tracker/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/vit/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.711256 ultralytics-8.0.98/ultralytics/vit/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/autosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/vit/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22502 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/prompt_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/vit/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/stream_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51260 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23582 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.715256 ultralytics-8.0.98/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40265 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24037 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/v8/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.719256 ultralytics-8.0.98/ultralytics/yolo/v8/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/detect/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.723256 ultralytics-8.0.98/ultralytics/yolo/v8/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.723256 ultralytics-8.0.98/ultralytics/yolo/v8/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-10 23:15:33.000000 ultralytics-8.0.98/ultralytics/yolo/v8/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:16:51.703256 ultralytics-8.0.98/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 23:16:51.000000 ultralytics-8.0.98/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.0.97/CONTRIBUTING.md` & `ultralytics-8.0.98/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/LICENSE` & `ultralytics-8.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/PKG-INFO` & `ultralytics-8.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.97
+Version: 8.0.98
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.97 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.98 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Home-page: https://github.com/
 ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics Keywords: machine-
 learning,deep-
```

### Comparing `ultralytics-8.0.97/README.md` & `ultralytics-8.0.98/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/README.zh-CN.md` & `ultralytics-8.0.98/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/requirements.txt` & `ultralytics-8.0.98/requirements.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/setup.cfg` & `ultralytics-8.0.98/setup.cfg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/setup.py` & `ultralytics-8.0.98/setup.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/tests/test_cli.py` & `ultralytics-8.0.98/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/tests/test_engine.py` & `ultralytics-8.0.98/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/tests/test_python.py` & `ultralytics-8.0.98/tests/test_python.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     # Paddle protobuf requirements conflicting with onnx protobuf requirements
     if enabled:
         model = YOLO(MODEL)
         model.export(format='paddle')
 
 
 def test_all_model_yamls():
-    for m in list((ROOT / 'models').rglob('*.yaml')):
+    for m in list((ROOT / 'models').rglob('yolo*.yaml')):
         YOLO(m.name)
 
 
 def test_workflow():
     model = YOLO(MODEL)
     model.train(data='coco8.yaml', epochs=1, imgsz=32)
     model.val()
```

### Comparing `ultralytics-8.0.97/ultralytics/assets/bus.jpg` & `ultralytics-8.0.98/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/assets/zidane.jpg` & `ultralytics-8.0.98/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/Argoverse.yaml` & `ultralytics-8.0.98/ultralytics/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/GlobalWheat2020.yaml` & `ultralytics-8.0.98/ultralytics/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/ImageNet.yaml` & `ultralytics-8.0.98/ultralytics/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/Objects365.yaml` & `ultralytics-8.0.98/ultralytics/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/SKU-110K.yaml` & `ultralytics-8.0.98/ultralytics/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/VOC.yaml` & `ultralytics-8.0.98/ultralytics/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/VisDrone.yaml` & `ultralytics-8.0.98/ultralytics/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/coco-pose.yaml` & `ultralytics-8.0.98/ultralytics/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/coco.yaml` & `ultralytics-8.0.98/ultralytics/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/coco128-seg.yaml` & `ultralytics-8.0.98/ultralytics/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/coco128.yaml` & `ultralytics-8.0.98/ultralytics/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/coco8-pose.yaml` & `ultralytics-8.0.98/ultralytics/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/coco8-seg.yaml` & `ultralytics-8.0.98/ultralytics/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/coco8.yaml` & `ultralytics-8.0.98/ultralytics/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/datasets/xView.yaml` & `ultralytics-8.0.98/ultralytics/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/hub/__init__.py` & `ultralytics-8.0.98/ultralytics/hub/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,19 +67,17 @@
     from ultralytics.yolo.engine.exporter import export_formats
     return list(export_formats()['Argument'][1:]) + ['ultralytics_tflite', 'ultralytics_coreml']
 
 
 def export_model(model_id='', format='torchscript'):
     """Export a model to all formats."""
     assert format in export_fmts_hub(), f"Unsupported export format '{format}', valid formats are {export_fmts_hub()}"
-    r = requests.post('https://api.ultralytics.com/export',
-                      json={
-                          'apiKey': Auth().api_key,
-                          'modelId': model_id,
-                          'format': format})
+    r = requests.post(f'https://api.ultralytics.com/v1/models/{model_id}/export',
+                      json={'format': format},
+                      headers={'x-api-key': Auth().api_key})
     assert r.status_code == 200, f'{PREFIX}{format} export failure {r.status_code} {r.reason}'
     LOGGER.info(f'{PREFIX}{format} export started ✅')
 
 
 def get_export(model_id='', format='torchscript'):
     """Get an exported model dictionary with download URL."""
     assert format in export_fmts_hub(), f"Unsupported export format '{format}', valid formats are {export_fmts_hub()}"
```

### Comparing `ultralytics-8.0.97/ultralytics/hub/auth.py` & `ultralytics-8.0.98/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/hub/session.py` & `ultralytics-8.0.98/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/hub/utils.py` & `ultralytics-8.0.98/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v3/yolov3-spp.yaml` & `ultralytics-8.0.98/ultralytics/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v3/yolov3-tiny.yaml` & `ultralytics-8.0.98/ultralytics/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v3/yolov3.yaml` & `ultralytics-8.0.98/ultralytics/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v5/yolov5-p6.yaml` & `ultralytics-8.0.98/ultralytics/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v5/yolov5.yaml` & `ultralytics-8.0.98/ultralytics/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v8/yolov8-cls.yaml` & `ultralytics-8.0.98/ultralytics/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v8/yolov8-p2.yaml` & `ultralytics-8.0.98/ultralytics/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v8/yolov8-p6.yaml` & `ultralytics-8.0.98/ultralytics/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v8/yolov8-pose.yaml` & `ultralytics-8.0.98/ultralytics/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v8/yolov8-seg.yaml` & `ultralytics-8.0.98/ultralytics/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/models/v8/yolov8.yaml` & `ultralytics-8.0.98/ultralytics/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/nn/autobackend.py` & `ultralytics-8.0.98/ultralytics/nn/autobackend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
+
 import ast
 import contextlib
 import json
 import platform
 import zipfile
 from collections import OrderedDict, namedtuple
 from pathlib import Path
```

### Comparing `ultralytics-8.0.97/ultralytics/nn/autoshape.py` & `ultralytics-8.0.98/ultralytics/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/nn/tasks.py` & `ultralytics-8.0.98/ultralytics/nn/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from copy import deepcopy
 from pathlib import Path
 
 import thop
 import torch
 import torch.nn as nn
 
-from ultralytics.nn.modules import (C1, C2, C3, C3TR, SPP, SPPF, Bottleneck, BottleneckCSP, C2f, C3Ghost, C3x, Classify,
-                                    Concat, Conv, ConvTranspose, Detect, DWConv, DWConvTranspose2d, Ensemble, Focus,
-                                    GhostBottleneck, GhostConv, Pose, Segment)
+from ultralytics.nn.modules import (AIFI, C1, C2, C3, C3TR, SPP, SPPF, Bottleneck, BottleneckCSP, C2f, C3Ghost, C3x,
+                                    Classify, Concat, Conv, ConvTranspose, Detect, DWConv, DWConvTranspose2d, Focus,
+                                    GhostBottleneck, GhostConv, HGBlock, HGStem, Pose, RepC3, RepConv, RTDETRDecoder,
+                                    Segment)
 from ultralytics.yolo.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, colorstr, emojis, yaml_load
 from ultralytics.yolo.utils.checks import check_requirements, check_suffix, check_yaml
 from ultralytics.yolo.utils.plotting import feature_visualization
 from ultralytics.yolo.utils.torch_utils import (fuse_conv_and_bn, fuse_deconv_and_bn, initialize_weights,
                                                 intersect_dicts, make_divisible, model_info, scale_img, time_sync)
 
 
@@ -101,14 +102,17 @@
                     m.conv = fuse_conv_and_bn(m.conv, m.bn)  # update conv
                     delattr(m, 'bn')  # remove batchnorm
                     m.forward = m.forward_fuse  # update forward
                 if isinstance(m, ConvTranspose) and hasattr(m, 'bn'):
                     m.conv_transpose = fuse_deconv_and_bn(m.conv_transpose, m.bn)
                     delattr(m, 'bn')  # remove batchnorm
                     m.forward = m.forward_fuse  # update forward
+                if isinstance(m, RepConv):
+                    m.fuse_convs()
+                    m.forward = m.forward_fuse  # update forward
             self.info(verbose=verbose)
 
         return self
 
     def is_fused(self, thresh=10):
         """
         Check if the model has less than a certain threshold of BatchNorm layers.
@@ -330,14 +334,30 @@
                     m[i] = nn.Linear(m[i].in_features, nc)
             elif nn.Conv2d in types:
                 i = types.index(nn.Conv2d)  # nn.Conv2d index
                 if m[i].out_channels != nc:
                     m[i] = nn.Conv2d(m[i].in_channels, nc, m[i].kernel_size, m[i].stride, bias=m[i].bias is not None)
 
 
+class Ensemble(nn.ModuleList):
+    """Ensemble of models."""
+
+    def __init__(self):
+        """Initialize an ensemble of models."""
+        super().__init__()
+
+    def forward(self, x, augment=False, profile=False, visualize=False):
+        """Function generates the YOLOv5 network's final layer."""
+        y = [module(x, augment, profile, visualize)[0] for module in self]
+        # y = torch.stack(y).max(0)[0]  # max ensemble
+        # y = torch.stack(y).mean(0)  # mean ensemble
+        y = torch.cat(y, 2)  # nms ensemble, y shape(B, HW, C)
+        return y, None  # inference, train output
+
+
 # Functions ------------------------------------------------------------------------------------------------------------
 
 
 def torch_safe_load(weight):
     """
     This function attempts to load a PyTorch model with the torch.load() function. If a ModuleNotFoundError is raised,
     it catches the error, logs a warning message, and attempts to install the missing module via the
@@ -411,15 +431,15 @@
     assert all(ensemble[0].nc == m.nc for m in ensemble), f'Models differ in class counts {[m.nc for m in ensemble]}'
     return ensemble
 
 
 def attempt_load_one_weight(weight, device=None, inplace=True, fuse=False):
     """Loads a single model weights."""
     ckpt, weight = torch_safe_load(weight)  # load ckpt
-    args = {**DEFAULT_CFG_DICT, **ckpt['train_args']}  # combine model and default args, preferring model args
+    args = {**DEFAULT_CFG_DICT, **(ckpt.get('train_args', {}))}  # combine model and default args, preferring model args
     model = (ckpt.get('ema') or ckpt['model']).to(device).float()  # FP32 model
 
     # Model compatibility updates
     model.args = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}  # attach args to model
     model.pt_path = weight  # attach *.pt file path to model
     model.task = guess_model_task(model)
     if not hasattr(model, 'stride'):
@@ -468,28 +488,37 @@
         for j, a in enumerate(args):
             if isinstance(a, str):
                 with contextlib.suppress(ValueError):
                     args[j] = locals()[a] if a in locals() else ast.literal_eval(a)
 
         n = n_ = max(round(n * depth), 1) if n > 1 else n  # depth gain
         if m in (Classify, Conv, ConvTranspose, GhostConv, Bottleneck, GhostBottleneck, SPP, SPPF, DWConv, Focus,
-                 BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, nn.ConvTranspose2d, DWConvTranspose2d, C3x):
+                 BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, nn.ConvTranspose2d, DWConvTranspose2d, C3x, RepC3):
             c1, c2 = ch[f], args[0]
             if c2 != nc:  # if c2 not equal to number of classes (i.e. for Classify() output)
                 c2 = make_divisible(min(c2, max_channels) * width, 8)
 
             args = [c1, c2, *args[1:]]
-            if m in (BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, C3x):
+            if m in (BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, C3x, RepC3):
                 args.insert(2, n)  # number of repeats
                 n = 1
+        elif m is AIFI:
+            args = [ch[f], *args]
+        elif m in (HGStem, HGBlock):
+            c1, cm, c2 = ch[f], args[0], args[1]
+            args = [c1, cm, c2, *args[2:]]
+            if m is HGBlock:
+                args.insert(4, n)  # number of repeats
+                n = 1
+
         elif m is nn.BatchNorm2d:
             args = [ch[f]]
         elif m is Concat:
             c2 = sum(ch[x] for x in f)
-        elif m in (Detect, Segment, Pose):
+        elif m in (Detect, Segment, Pose, RTDETRDecoder):
             args.append([ch[x] for x in f])
             if m is Segment:
                 args[2] = make_divisible(min(args[2], max_channels) * width, 8)
         else:
             c2 = ch[f]
 
         m_ = nn.Sequential(*(m(*args) for _ in range(n))) if n > 1 else m(*args)  # module
```

### Comparing `ultralytics-8.0.97/ultralytics/tracker/cfg/botsort.yaml` & `ultralytics-8.0.98/ultralytics/tracker/cfg/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/cfg/bytetrack.yaml` & `ultralytics-8.0.98/ultralytics/tracker/cfg/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/track.py` & `ultralytics-8.0.98/ultralytics/tracker/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/trackers/basetrack.py` & `ultralytics-8.0.98/ultralytics/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/trackers/bot_sort.py` & `ultralytics-8.0.98/ultralytics/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/trackers/byte_tracker.py` & `ultralytics-8.0.98/ultralytics/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/utils/gmc.py` & `ultralytics-8.0.98/ultralytics/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/utils/kalman_filter.py` & `ultralytics-8.0.98/ultralytics/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/tracker/utils/matching.py` & `ultralytics-8.0.98/ultralytics/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/amg.py` & `ultralytics-8.0.98/ultralytics/vit/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/autosize.py` & `ultralytics-8.0.98/ultralytics/vit/sam/autosize.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/build.py` & `ultralytics-8.0.98/ultralytics/vit/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/model.py` & `ultralytics-8.0.98/ultralytics/vit/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/modules/decoders.py` & `ultralytics-8.0.98/ultralytics/vit/sam/modules/decoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,9 +153,9 @@
         self.sigmoid_output = sigmoid_output
 
     def forward(self, x):
         """Executes feedforward within the neural network module and applies activation."""
         for i, layer in enumerate(self.layers):
             x = F.relu(layer(x)) if i < self.num_layers - 1 else layer(x)
         if self.sigmoid_output:
-            x = F.sigmoid(x)
+            x = torch.sigmoid(x)
         return x
```

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/modules/encoders.py` & `ultralytics-8.0.98/ultralytics/vit/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/modules/mask_generator.py` & `ultralytics-8.0.98/ultralytics/vit/sam/modules/mask_generator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/modules/prompt_predictor.py` & `ultralytics-8.0.98/ultralytics/vit/sam/modules/prompt_predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/modules/sam.py` & `ultralytics-8.0.98/ultralytics/vit/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/modules/transformer.py` & `ultralytics-8.0.98/ultralytics/vit/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/vit/sam/predict.py` & `ultralytics-8.0.98/ultralytics/vit/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/cfg/__init__.py` & `ultralytics-8.0.98/ultralytics/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/cfg/default.yaml` & `ultralytics-8.0.98/ultralytics/yolo/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/annotator.py` & `ultralytics-8.0.98/ultralytics/yolo/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/augment.py` & `ultralytics-8.0.98/ultralytics/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/base.py` & `ultralytics-8.0.98/ultralytics/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/build.py` & `ultralytics-8.0.98/ultralytics/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/converter.py` & `ultralytics-8.0.98/ultralytics/yolo/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/stream_loaders.py` & `ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/v5augmentations.py` & `ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/dataloaders/v5loader.py` & `ultralytics-8.0.98/ultralytics/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/dataset.py` & `ultralytics-8.0.98/ultralytics/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/dataset_wrappers.py` & `ultralytics-8.0.98/ultralytics/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/data/utils.py` & `ultralytics-8.0.98/ultralytics/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/engine/exporter.py` & `ultralytics-8.0.98/ultralytics/yolo/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/engine/model.py` & `ultralytics-8.0.98/ultralytics/yolo/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/engine/predictor.py` & `ultralytics-8.0.98/ultralytics/yolo/engine/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,26 +111,36 @@
     def preprocess(self, im):
         """Prepares input image before inference.
 
         Args:
             im (torch.Tensor | List(np.ndarray)): (N, 3, h, w) for tensor, [(h, w, 3) x N] for list.
         """
         if not isinstance(im, torch.Tensor):
-            same_shapes = all(x.shape == im[0].shape for x in im)
-            auto = same_shapes and self.model.pt
-            im = np.stack([LetterBox(self.imgsz, auto=auto, stride=self.model.stride)(image=x) for x in im])
+            im = np.stack(self.pre_transform(im))
             im = im[..., ::-1].transpose((0, 3, 1, 2))  # BGR to RGB, BHWC to BCHW, (n, 3, h, w)
             im = np.ascontiguousarray(im)  # contiguous
             im = torch.from_numpy(im)
         # NOTE: assuming im with (b, 3, h, w) if it's a tensor
         img = im.to(self.device)
         img = img.half() if self.model.fp16 else img.float()  # uint8 to fp16/32
         img /= 255  # 0 - 255 to 0.0 - 1.0
         return img
 
+    def pre_transform(self, im):
+        """Pre-tranform input image before inference.
+
+        Args:
+            im (List(np.ndarray)): (N, 3, h, w) for tensor, [(h, w, 3) x N] for list.
+
+        Return: A list of transformed imgs.
+        """
+        same_shapes = all(x.shape == im[0].shape for x in im)
+        auto = same_shapes and self.model.pt
+        return [LetterBox(self.imgsz, auto=auto, stride=self.model.stride)(image=x) for x in im]
+
     def write_results(self, idx, results, batch):
         """Write inference results to a file or directory."""
         p, im, _ = batch
         log_string = ''
         if len(im.shape) == 3:
             im = im[None]  # expand for batch dim
         self.seen += 1
```

### Comparing `ultralytics-8.0.97/ultralytics/yolo/engine/results.py` & `ultralytics-8.0.98/ultralytics/yolo/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/engine/trainer.py` & `ultralytics-8.0.98/ultralytics/yolo/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/engine/validator.py` & `ultralytics-8.0.98/ultralytics/yolo/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/__init__.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/autobatch.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/benchmarks.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/base.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/clearml.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/comet.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/hub.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/mlflow.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/neptune.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/tensorboard.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/callbacks/wb.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/checks.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/dist.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/downloads.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/downloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from tqdm import tqdm
 
 from ultralytics.yolo.utils import LOGGER, checks, clean_url, emojis, is_online, url2file
 
 GITHUB_ASSET_NAMES = [f'yolov8{k}{suffix}.pt' for k in 'nsmlx' for suffix in ('', '6', '-cls', '-seg', '-pose')] + \
                      [f'yolov5{k}u.pt' for k in 'nsmlx'] + \
                      [f'yolov3{k}u.pt' for k in ('', '-spp', '-tiny')] + \
-                     [f'sam_{k}.pt' for k in 'bl']
+                     [f'sam_{k}.pt' for k in 'bl'] + \
+                     [f'rtdetr-{k}.pt' for k in 'lx']
 GITHUB_ASSET_STEMS = [Path(k).stem for k in GITHUB_ASSET_NAMES]
 
 
 def is_url(url, check=True):
     """Check if string is URL and check if URL exists."""
     with contextlib.suppress(Exception):
         url = str(url)
```

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/files.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     """
     path = Path(path)  # os-agnostic
     if path.exists() and not exist_ok:
         path, suffix = (path.with_suffix(''), path.suffix) if path.is_file() else (path, '')
 
         # Method 1
         for n in range(2, 9999):
-            p = f'{path}{sep}{str(n).zfill(4)}{suffix}'  # increment path
+            p = f'{path}{sep}{n}{suffix}'  # increment path
             if not os.path.exists(p):  #
                 break
         path = Path(p)
 
     if mkdir:
         path.mkdir(parents=True, exist_ok=True)  # make directory
```

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/instance.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/loss.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/metrics.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/ops.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/plotting.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/tal.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/torch_utils.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/torch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ultralytics.yolo.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, RANK, __version__
 from ultralytics.yolo.utils.checks import check_version
 
 TORCHVISION_0_10 = check_version(torchvision.__version__, '0.10.0')
 TORCH_1_9 = check_version(torch.__version__, '1.9.0')
 TORCH_1_11 = check_version(torch.__version__, '1.11.0')
 TORCH_1_12 = check_version(torch.__version__, '1.12.0')
-TORCH_2_X = check_version(torch.__version__, minimum='2.0')
+TORCH_2_0 = check_version(torch.__version__, minimum='2.0')
 
 
 @contextmanager
 def torch_distributed_zero_first(local_rank: int):
     """Decorator to make all processes in distributed training wait for each local_master to do something."""
     initialized = torch.distributed.is_available() and torch.distributed.is_initialized()
     if initialized and local_rank not in (-1, 0):
@@ -81,15 +81,15 @@
             raise ValueError(f"'batch={batch}' must be a multiple of GPU count {n}. Try 'batch={batch // n * n}' or "
                              f"'batch={batch // n * n + n}', the nearest batch sizes evenly divisible by {n}.")
         space = ' ' * (len(s) + 1)
         for i, d in enumerate(devices):
             p = torch.cuda.get_device_properties(i)
             s += f"{'' if i == 0 else space}CUDA:{d} ({p.name}, {p.total_memory / (1 << 20):.0f}MiB)\n"  # bytes to MB
         arg = 'cuda:0'
-    elif mps and getattr(torch, 'has_mps', False) and torch.backends.mps.is_available() and TORCH_2_X:
+    elif mps and getattr(torch, 'has_mps', False) and torch.backends.mps.is_available() and TORCH_2_0:
         # Prefer MPS if available
         s += 'MPS\n'
         arg = 'mps'
     else:  # revert to CPU
         s += 'CPU\n'
         arg = 'cpu'
 
@@ -270,19 +270,22 @@
     """Initialize random number generator (RNG) seeds https://pytorch.org/docs/stable/notes/randomness.html."""
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)  # for Multi-GPU, exception safe
     # torch.backends.cudnn.benchmark = True  # AutoBatch problem https://github.com/ultralytics/yolov5/issues/9287
-    if deterministic and TORCH_1_12:  # https://github.com/ultralytics/yolov5/pull/8213
-        torch.use_deterministic_algorithms(True)
-        torch.backends.cudnn.deterministic = True
-        os.environ['CUBLAS_WORKSPACE_CONFIG'] = ':4096:8'
-        os.environ['PYTHONHASHSEED'] = str(seed)
+    if deterministic:  # https://github.com/ultralytics/yolov5/pull/8213
+        if TORCH_2_0:
+            torch.use_deterministic_algorithms(True)
+            torch.backends.cudnn.deterministic = True
+            os.environ['CUBLAS_WORKSPACE_CONFIG'] = ':4096:8'
+            os.environ['PYTHONHASHSEED'] = str(seed)
+        else:
+            LOGGER.warning('WARNING ⚠️ Upgrade to torch>=2.0.0 for deterministic training.')
 
 
 class ModelEMA:
     """Updated Exponential Moving Average (EMA) from https://github.com/rwightman/pytorch-image-models
     Keeps a moving average of everything in the model state_dict (parameters and buffers)
     For EMA details see https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
     To disable EMA set the `enabled` attribute to `False`.
```

### Comparing `ultralytics-8.0.97/ultralytics/yolo/utils/tuner.py` & `ultralytics-8.0.98/ultralytics/yolo/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/classify/predict.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/classify/train.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/classify/val.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/detect/predict.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/detect/train.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/detect/val.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/pose/predict.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/pose/train.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/pose/val.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/segment/predict.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/segment/train.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics/yolo/v8/segment/val.py` & `ultralytics-8.0.98/ultralytics/yolo/v8/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.0.97/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.0.98/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.0.97
+Version: 8.0.98
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/ultralytics/ultralytics
 Author: Ultralytics
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.0.97 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.0.98 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Home-page: https://github.com/
 ultralytics/ultralytics Author: Ultralytics Author-email: hello@ultralytics.com
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics Keywords: machine-
 learning,deep-
```

### Comparing `ultralytics-8.0.97/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.0.98/ultralytics.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 ultralytics/datasets/coco8-seg.yaml
 ultralytics/datasets/coco8.yaml
 ultralytics/datasets/xView.yaml
 ultralytics/hub/__init__.py
 ultralytics/hub/auth.py
 ultralytics/hub/session.py
 ultralytics/hub/utils.py
+ultralytics/models/rt-detr/rt-detr-l.yaml
+ultralytics/models/rt-detr/rt-detr-x.yaml
 ultralytics/models/v3/yolov3-spp.yaml
 ultralytics/models/v3/yolov3-tiny.yaml
 ultralytics/models/v3/yolov3.yaml
 ultralytics/models/v5/yolov5-p6.yaml
 ultralytics/models/v5/yolov5.yaml
 ultralytics/models/v8/yolov8-cls.yaml
 ultralytics/models/v8/yolov8-p2.yaml
@@ -48,29 +50,38 @@
 ultralytics/models/v8/yolov8-pose-p6.yaml
 ultralytics/models/v8/yolov8-pose.yaml
 ultralytics/models/v8/yolov8-seg.yaml
 ultralytics/models/v8/yolov8.yaml
 ultralytics/nn/__init__.py
 ultralytics/nn/autobackend.py
 ultralytics/nn/autoshape.py
-ultralytics/nn/modules.py
 ultralytics/nn/tasks.py
+ultralytics/nn/modules/__init__.py
+ultralytics/nn/modules/block.py
+ultralytics/nn/modules/conv.py
+ultralytics/nn/modules/head.py
+ultralytics/nn/modules/transformer.py
+ultralytics/nn/modules/utils.py
 ultralytics/tracker/__init__.py
 ultralytics/tracker/track.py
 ultralytics/tracker/cfg/botsort.yaml
 ultralytics/tracker/cfg/bytetrack.yaml
 ultralytics/tracker/trackers/__init__.py
 ultralytics/tracker/trackers/basetrack.py
 ultralytics/tracker/trackers/bot_sort.py
 ultralytics/tracker/trackers/byte_tracker.py
 ultralytics/tracker/utils/__init__.py
 ultralytics/tracker/utils/gmc.py
 ultralytics/tracker/utils/kalman_filter.py
 ultralytics/tracker/utils/matching.py
 ultralytics/vit/__init__.py
+ultralytics/vit/rtdetr/__init__.py
+ultralytics/vit/rtdetr/model.py
+ultralytics/vit/rtdetr/predict.py
+ultralytics/vit/rtdetr/val.py
 ultralytics/vit/sam/__init__.py
 ultralytics/vit/sam/amg.py
 ultralytics/vit/sam/autosize.py
 ultralytics/vit/sam/build.py
 ultralytics/vit/sam/model.py
 ultralytics/vit/sam/predict.py
 ultralytics/vit/sam/modules/__init__.py
```

