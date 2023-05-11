# Comparing `tmp/voxel51-eta-0.8.4rc1.tar.gz` & `tmp/voxel51-eta-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxel51-eta-0.8.4rc1.tar", last modified: Tue Mar 14 15:42:11 2023, max compression
+gzip compressed data, was "voxel51-eta-0.9.0.tar", last modified: Tue Apr  4 13:14:44 2023, max compression
```

## Comparing `voxel51-eta-0.8.4rc1.tar` & `voxel51-eta-0.9.0.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.583875 voxel51-eta-0.8.4rc1/
--rw-r--r--   0 runner    (1001) docker     (116)     3159 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)    11349 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       70 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    13533 2023-03-14 15:42:11.583875 voxel51-eta-0.8.4rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    12160 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      704 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/config-example.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.563875 voxel51-eta-0.8.4rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)    55024 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/cli_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     4063 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/core_dev_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     4959 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/cuda_install_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     3976 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/custom_opencv_builds.md
--rw-r--r--   0 runner    (1001) docker     (116)     1966 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/docker_build_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     3334 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/export_tf_graphs_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)      277 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/guide2html.bash
--rw-r--r--   0 runner    (1001) docker     (116)      461 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/guide2tex.bash
--rw-r--r--   0 runner    (1001) docker     (116)     7997 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/image_labels_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     2446 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/linting_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     3324 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/logging_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     2262 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/markdown_style_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)    10973 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/models_dev_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)    34159 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/modules_dev_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)    12527 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/pipelines_dev_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     5668 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/python23_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     3745 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/python_style_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)    10590 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/storage_dev_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     9902 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/video_labels_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     3647 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/virtualenv_guide.md
--rw-r--r--   0 runner    (1001) docker     (116)     1593 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/docs/visualize_tf_graphs_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.563875 voxel51-eta-0.8.4rc1/eta/
--rw-r--r--   0 runner    (1001) docker     (116)     6601 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.563875 voxel51-eta-0.8.4rc1/eta/classifiers/
--rw-r--r--   0 runner    (1001) docker     (116)      466 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    19298 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/classifiers/tfslim_classifiers.py
--rw-r--r--   0 runner    (1001) docker     (116)     7167 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/classifiers/vgg16_classifiers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2770 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/classifiers/voting_classifiers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.571875 voxel51-eta-0.8.4rc1/eta/core/
--rw-r--r--   0 runner    (1001) docker     (116)       77 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    68688 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/annotations.py
--rw-r--r--   0 runner    (1001) docker     (116)    25550 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/builder.py
--rw-r--r--   0 runner    (1001) docker     (116)    12416 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/c3d.py
--rw-r--r--   0 runner    (1001) docker     (116)   126930 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    30762 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    61424 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.571875 voxel51-eta-0.8.4rc1/eta/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)      281 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15518 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/datasets/builders.py
--rw-r--r--   0 runner    (1001) docker     (116)    57824 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/datasets/labeled_datasets.py
--rw-r--r--   0 runner    (1001) docker     (116)     7599 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/datasets/split_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)    43475 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/datasets/transformers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3458 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     6299 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/datasets/video2image.py
--rw-r--r--   0 runner    (1001) docker     (116)    16559 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/diagram.py
--rw-r--r--   0 runner    (1001) docker     (116)   104509 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/events.py
--rw-r--r--   0 runner    (1001) docker     (116)    55227 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/features.py
--rw-r--r--   0 runner    (1001) docker     (116)    89316 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/frames.py
--rw-r--r--   0 runner    (1001) docker     (116)    19595 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/frameutils.py
--rw-r--r--   0 runner    (1001) docker     (116)    19351 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/geometry.py
--rw-r--r--   0 runner    (1001) docker     (116)     9301 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/gps.py
--rw-r--r--   0 runner    (1001) docker     (116)     3418 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)    56569 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/image.py
--rw-r--r--   0 runner    (1001) docker     (116)     4440 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/job.py
--rw-r--r--   0 runner    (1001) docker     (116)    32055 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (116)    30151 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/labels.py
--rw-r--r--   0 runner    (1001) docker     (116)    42595 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/learning.py
--rw-r--r--   0 runner    (1001) docker     (116)     5874 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (116)     5652 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/logo.py
--rw-r--r--   0 runner    (1001) docker     (116)    14361 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)    58387 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/models.py
--rw-r--r--   0 runner    (1001) docker     (116)    22215 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/module.py
--rw-r--r--   0 runner    (1001) docker     (116)     5401 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/numutils.py
--rw-r--r--   0 runner    (1001) docker     (116)    72420 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (116)    41672 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)    33729 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/polylines.py
--rw-r--r--   0 runner    (1001) docker     (116)    23553 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/primitives.py
--rw-r--r--   0 runner    (1001) docker     (116)    95900 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/serial.py
--rw-r--r--   0 runner    (1001) docker     (116)    10978 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/status.py
--rw-r--r--   0 runner    (1001) docker     (116)   129793 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (116)    15086 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/tfutils.py
--rw-r--r--   0 runner    (1001) docker     (116)    48191 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/types.py
--rw-r--r--   0 runner    (1001) docker     (116)   131890 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    19539 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (116)   142883 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/video.py
--rw-r--r--   0 runner    (1001) docker     (116)     7267 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/web.py
--rw-r--r--   0 runner    (1001) docker     (116)     5182 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/core/ziputils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.571875 voxel51-eta-0.8.4rc1/eta/detectors/
--rw-r--r--   0 runner    (1001) docker     (116)      474 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8508 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/detectors/efficientdet.py
--rw-r--r--   0 runner    (1001) docker     (116)    37283 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/detectors/tfmodels_detectors.py
--rw-r--r--   0 runner    (1001) docker     (116)      652 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/detectors/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5675 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/detectors/yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.571875 voxel51-eta-0.8.4rc1/eta/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     3906 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      353 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/clean.bash
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.571875 voxel51-eta-0.8.4rc1/eta/examples/demo_cats/
--rw-r--r--   0 runner    (1001) docker     (116)      642 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_cats/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1084 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_cats/detect-classify-cats.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.571875 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/
--rw-r--r--   0 runner    (1001) docker     (116)      991 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     2013 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_image.py
--rw-r--r--   0 runner    (1001) docker     (116)     1844 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_image_direct.py
--rw-r--r--   0 runner    (1001) docker     (116)      539 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_vgg16_module-config.json
--rw-r--r--   0 runner    (1001) docker     (116)       92 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_vgg16_module.bash
--rw-r--r--   0 runner    (1001) docker     (116)      399 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_vgg16_pipeline-config.json
--rw-r--r--   0 runner    (1001) docker     (116)      422 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_video-config.json
--rw-r--r--   0 runner    (1001) docker     (116)     2507 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_video.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.571875 voxel51-eta-0.8.4rc1/eta/examples/demo_image_classifier/
--rw-r--r--   0 runner    (1001) docker     (116)     1153 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_image_classifier/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      782 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_image_classifier/classify-images-tfslim-template.json
--rw-r--r--   0 runner    (1001) docker     (116)      748 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_image_classifier/classify-images-vgg16.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.575875 voxel51-eta-0.8.4rc1/eta/examples/demo_instance_segmentation/
--rw-r--r--   0 runner    (1001) docker     (116)      622 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_instance_segmentation/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      720 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_instance_segmentation/segment-people.json
--rw-r--r--   0 runner    (1001) docker     (116)      735 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_instance_segmentation/segment-vehicles.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.575875 voxel51-eta-0.8.4rc1/eta/examples/demo_object_detector/
--rw-r--r--   0 runner    (1001) docker     (116)      589 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_object_detector/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      806 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_object_detector/detect-people.json
--rw-r--r--   0 runner    (1001) docker     (116)      821 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_object_detector/detect-vehicles.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.575875 voxel51-eta-0.8.4rc1/eta/examples/demo_semantic_segmentation/
--rw-r--r--   0 runner    (1001) docker     (116)      486 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_semantic_segmentation/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      534 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_semantic_segmentation/segment-frames.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.575875 voxel51-eta-0.8.4rc1/eta/examples/demo_video_clipper/
--rw-r--r--   0 runner    (1001) docker     (116)      272 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_video_clipper/request.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.575875 voxel51-eta-0.8.4rc1/eta/examples/demo_video_formatter/
--rw-r--r--   0 runner    (1001) docker     (116)      267 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_video_formatter/request.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.575875 voxel51-eta-0.8.4rc1/eta/examples/demo_video_pipeline/
--rw-r--r--   0 runner    (1001) docker     (116)      230 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_video_pipeline/clip_videos.json
--rw-r--r--   0 runner    (1001) docker     (116)      350 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_video_pipeline/format_videos.json
--rw-r--r--   0 runner    (1001) docker     (116)      615 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/demo_video_pipeline/pipeline.json
--rw-r--r--   0 runner    (1001) docker     (116)      968 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/examples/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.575875 voxel51-eta-0.8.4rc1/eta/models/
--rw-r--r--   0 runner    (1001) docker     (116)    44907 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/models/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.579875 voxel51-eta-0.8.4rc1/eta/modules/
--rw-r--r--   0 runner    (1001) docker     (116)     5370 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_classifier_to_objects.json
--rw-r--r--   0 runner    (1001) docker     (116)    16584 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_classifier_to_objects.py
--rw-r--r--   0 runner    (1001) docker     (116)     4541 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_image_classifier.json
--rw-r--r--   0 runner    (1001) docker     (116)    14768 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_image_classifier.py
--rw-r--r--   0 runner    (1001) docker     (116)     2783 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_image_model.json
--rw-r--r--   0 runner    (1001) docker     (116)     8434 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_image_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     3127 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_image_semantic_segmenter.json
--rw-r--r--   0 runner    (1001) docker     (116)     9573 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_image_semantic_segmenter.py
--rw-r--r--   0 runner    (1001) docker     (116)     4432 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_object_detector.json
--rw-r--r--   0 runner    (1001) docker     (116)    14664 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (116)     1729 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_classifier.json
--rw-r--r--   0 runner    (1001) docker     (116)     5249 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_classifier.py
--rw-r--r--   0 runner    (1001) docker     (116)     1485 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_event_detector.json
--rw-r--r--   0 runner    (1001) docker     (116)     4447 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_event_detector.py
--rw-r--r--   0 runner    (1001) docker     (116)     2265 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_frames_classifier.json
--rw-r--r--   0 runner    (1001) docker     (116)     6772 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_frames_classifier.py
--rw-r--r--   0 runner    (1001) docker     (116)     1437 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_model.json
--rw-r--r--   0 runner    (1001) docker     (116)     4297 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/apply_video_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     1564 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/clip_videos.json
--rw-r--r--   0 runner    (1001) docker     (116)     4435 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/clip_videos.py
--rw-r--r--   0 runner    (1001) docker     (116)     1205 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/embed_vgg16.json
--rw-r--r--   0 runner    (1001) docker     (116)     4471 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/embed_vgg16.py
--rw-r--r--   0 runner    (1001) docker     (116)     3400 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/format_videos.json
--rw-r--r--   0 runner    (1001) docker     (116)     8974 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/format_videos.py
--rw-r--r--   0 runner    (1001) docker     (116)     3296 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/sample_videos.json
--rw-r--r--   0 runner    (1001) docker     (116)     9055 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/sample_videos.py
--rw-r--r--   0 runner    (1001) docker     (116)      669 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/video_stream_info.json
--rw-r--r--   0 runner    (1001) docker     (116)     2121 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/video_stream_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     1976 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/visualize_image_labels.json
--rw-r--r--   0 runner    (1001) docker     (116)     6497 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/visualize_image_labels.py
--rw-r--r--   0 runner    (1001) docker     (116)     1410 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/visualize_labels.json
--rw-r--r--   0 runner    (1001) docker     (116)     3963 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/modules/visualize_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.579875 voxel51-eta-0.8.4rc1/eta/pipelines/
--rw-r--r--   0 runner    (1001) docker     (116)     2376 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/detect_and_classify_images.json
--rw-r--r--   0 runner    (1001) docker     (116)     1621 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/image_classifier.json
--rw-r--r--   0 runner    (1001) docker     (116)     1893 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/object_detector.json
--rw-r--r--   0 runner    (1001) docker     (116)     1821 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/semantic_segmenter.json
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/video_clipper.json
--rw-r--r--   0 runner    (1001) docker     (116)      963 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/video_formatter.json
--rw-r--r--   0 runner    (1001) docker     (116)      685 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/video_stream_info.json
--rw-r--r--   0 runner    (1001) docker     (116)     1155 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/pipelines/visualize_labels.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.579875 voxel51-eta-0.8.4rc1/eta/resources/
--rw-r--r--   0 runner    (1001) docker     (116)      184 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/default-logo-config.json
--rw-r--r--   0 runner    (1001) docker     (116)      407 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/eta-ascii.txt
--rw-r--r--   0 runner    (1001) docker     (116)    14362 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/imagenet-labels-no-background.txt
--rw-r--r--   0 runner    (1001) docker     (116)    14378 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/imagenet-labels.txt
--rw-r--r--   0 runner    (1001) docker     (116)   120196 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/lato-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (116)      924 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/ms-coco-labels.txt
--rw-r--r--   0 runner    (1001) docker     (116)      346 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/tf-semantic-segmenters-cityscapes-train-labels-with-categories.txt
--rw-r--r--   0 runner    (1001) docker     (116)      197 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/tf-semantic-segmenters-cityscapes-train-labels.txt
--rw-r--r--   0 runner    (1001) docker     (116)    14362 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/tfslim-imagenet-labels-no-background.txt
--rw-r--r--   0 runner    (1001) docker     (116)    14378 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/tfslim-imagenet-labels.txt
--rw-r--r--   0 runner    (1001) docker     (116)    14366 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/vgg16-imagenet-labels.txt
--rw-r--r--   0 runner    (1001) docker     (116)      198 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/voc-labels.txt
--rw-r--r--   0 runner    (1001) docker     (116)    23951 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/voxel51-logo-600dpi.png
--rw-r--r--   0 runner    (1001) docker     (116)     5230 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/resources/voxel51-logo.pdf
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.579875 voxel51-eta-0.8.4rc1/eta/segmenters/
--rw-r--r--   0 runner    (1001) docker     (116)      223 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/segmenters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7650 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/segmenters/tf_segmenters.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.579875 voxel51-eta-0.8.4rc1/eta/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/tensorflow/install_automl.bash
--rw-r--r--   0 runner    (1001) docker     (116)      855 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/tensorflow/install_darkflow.bash
--rw-r--r--   0 runner    (1001) docker     (116)     1493 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/eta/tensorflow/install_models.bash
--rw-r--r--   0 runner    (1001) docker     (116)     7174 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/install.bash
--rw-r--r--   0 runner    (1001) docker     (116)    13387 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)       84 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.579875 voxel51-eta-0.8.4rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)      578 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (116)      233 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)       59 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/requirements/pipeline.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (116)      133 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/requirements/storage.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-14 15:42:11.583875 voxel51-eta-0.8.4rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4000 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.579875 voxel51-eta-0.8.4rc1/sphinx/
--rw-r--r--   0 runner    (1001) docker     (116)      638 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      370 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/sphinx/generate_docs.bash
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.583875 voxel51-eta-0.8.4rc1/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/sphinx/source/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2469 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       56 2023-03-14 15:41:51.000000 voxel51-eta-0.8.4rc1/sphinx/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 15:42:11.583875 voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    13533 2023-03-14 15:42:11.000000 voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6096 2023-03-14 15:42:11.000000 voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-14 15:42:11.000000 voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       42 2023-03-14 15:42:11.000000 voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      396 2023-03-14 15:42:11.000000 voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2023-03-14 15:42:11.000000 voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.848215 voxel51-eta-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3159 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    13465 2023-04-04 13:14:44.848215 voxel51-eta-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12145 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/config-example.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.824214 voxel51-eta-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)    55024 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/cli_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4063 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/core_dev_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4959 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/cuda_install_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/custom_opencv_builds.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/docker_build_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/export_tf_graphs_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/guide2html.bash
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/guide2tex.bash
+-rw-r--r--   0 runner    (1001) docker     (122)     7997 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/image_labels_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/linting_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/logging_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2262 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/markdown_style_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10973 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/models_dev_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34159 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/modules_dev_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)    12527 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/pipelines_dev_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5668 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/python23_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/python_style_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10590 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/storage_dev_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9902 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/video_labels_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/virtualenv_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/docs/visualize_tf_graphs_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.824214 voxel51-eta-0.9.0/eta/
+-rw-r--r--   0 runner    (1001) docker     (122)     6601 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.824214 voxel51-eta-0.9.0/eta/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19298 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/classifiers/tfslim_classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7167 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/classifiers/vgg16_classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/classifiers/voting_classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2174 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.832214 voxel51-eta-0.9.0/eta/core/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68688 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25550 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12416 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/c3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)   126930 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30762 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61424 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.832214 voxel51-eta-0.9.0/eta/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15518 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/datasets/builders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57824 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/datasets/labeled_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7599 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/datasets/split_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43475 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/datasets/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/datasets/video2image.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16559 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104509 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55227 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    89316 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/frames.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19595 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/frameutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19351 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9301 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/gps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3418 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56569 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4440 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32055 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30151 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42595 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5652 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14361 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58387 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22215 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/numutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    72420 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41672 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33729 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/polylines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23553 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)    95999 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10978 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)   160666 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/tfutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48191 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)   132670 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19539 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (122)   142883 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/video.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7267 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/web.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5182 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/core/ziputils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.832214 voxel51-eta-0.9.0/eta/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8508 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/detectors/efficientdet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37283 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/detectors/tfmodels_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/detectors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5675 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/detectors/yolo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.832214 voxel51-eta-0.9.0/eta/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      353 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/clean.bash
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.832214 voxel51-eta-0.9.0/eta/examples/demo_cats/
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_cats/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_cats/detect-classify-cats.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_image_direct.py
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_vgg16_module-config.json
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_vgg16_module.bash
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_vgg16_pipeline-config.json
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_video-config.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_video.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_image_classifier/
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_image_classifier/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_image_classifier/classify-images-tfslim-template.json
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_image_classifier/classify-images-vgg16.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_instance_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_instance_segmentation/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_instance_segmentation/segment-people.json
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_instance_segmentation/segment-vehicles.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_object_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_object_detector/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_object_detector/detect-people.json
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_object_detector/detect-vehicles.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_semantic_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_semantic_segmentation/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_semantic_segmentation/segment-frames.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_video_clipper/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_video_clipper/request.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_video_formatter/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_video_formatter/request.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/examples/demo_video_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_video_pipeline/clip_videos.json
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_video_pipeline/format_videos.json
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/demo_video_pipeline/pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/examples/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.836214 voxel51-eta-0.9.0/eta/models/
+-rw-r--r--   0 runner    (1001) docker     (122)    44907 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/models/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.840214 voxel51-eta-0.9.0/eta/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_classifier_to_objects.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16584 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_classifier_to_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_image_classifier.json
+-rw-r--r--   0 runner    (1001) docker     (122)    14768 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_image_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2783 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_image_model.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_image_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3127 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_image_semantic_segmenter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     9573 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_image_semantic_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_object_detector.json
+-rw-r--r--   0 runner    (1001) docker     (122)    14664 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_classifier.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5249 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_event_detector.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_event_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_frames_classifier.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6772 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_frames_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_model.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4297 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/apply_video_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1564 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/clip_videos.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4435 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/clip_videos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/embed_vgg16.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/embed_vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3400 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/format_videos.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/format_videos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/sample_videos.json
+-rw-r--r--   0 runner    (1001) docker     (122)     9055 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/sample_videos.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/video_stream_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/video_stream_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1976 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/visualize_image_labels.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6497 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/visualize_image_labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/visualize_labels.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/modules/visualize_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.844215 voxel51-eta-0.9.0/eta/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/detect_and_classify_images.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/image_classifier.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/object_detector.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/semantic_segmenter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/video_clipper.json
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/video_formatter.json
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/video_stream_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/pipelines/visualize_labels.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.844215 voxel51-eta-0.9.0/eta/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/default-logo-config.json
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/eta-ascii.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14362 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/imagenet-labels-no-background.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14378 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/imagenet-labels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   120196 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/lato-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/ms-coco-labels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/tf-semantic-segmenters-cityscapes-train-labels-with-categories.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/tf-semantic-segmenters-cityscapes-train-labels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14362 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/tfslim-imagenet-labels-no-background.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14378 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/tfslim-imagenet-labels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14366 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/vgg16-imagenet-labels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/voc-labels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    23951 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/voxel51-logo-600dpi.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5230 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/resources/voxel51-logo.pdf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.844215 voxel51-eta-0.9.0/eta/segmenters/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/segmenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7650 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/segmenters/tf_segmenters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.844215 voxel51-eta-0.9.0/eta/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/tensorflow/install_automl.bash
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/tensorflow/install_darkflow.bash
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/eta/tensorflow/install_models.bash
+-rw-r--r--   0 runner    (1001) docker     (122)     7174 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/install.bash
+-rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.848215 voxel51-eta-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/requirements/pipeline.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/requirements/storage.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 13:14:44.848215 voxel51-eta-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4040 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.848215 voxel51-eta-0.9.0/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/sphinx/generate_docs.bash
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.848215 voxel51-eta-0.9.0/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/sphinx/source/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-04 13:14:33.000000 voxel51-eta-0.9.0/sphinx/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 13:14:44.848215 voxel51-eta-0.9.0/voxel51_eta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13465 2023-04-04 13:14:44.000000 voxel51-eta-0.9.0/voxel51_eta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-04-04 13:14:44.000000 voxel51-eta-0.9.0/voxel51_eta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 13:14:44.000000 voxel51-eta-0.9.0/voxel51_eta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-04 13:14:44.000000 voxel51-eta-0.9.0/voxel51_eta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-04 13:14:44.000000 voxel51-eta-0.9.0/voxel51_eta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-04-04 13:14:44.000000 voxel51-eta-0.9.0/voxel51_eta.egg-info/top_level.txt
```

### Comparing `voxel51-eta-0.8.4rc1/Dockerfile` & `voxel51-eta-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/LICENSE` & `voxel51-eta-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/PKG-INFO` & `voxel51-eta-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxel51-eta
-Version: 0.8.4rc1
+Version: 0.9.0
 Summary: Extensible Toolkit for Analytics
 Home-page: https://github.com/voxel51/eta
 Author: Voxel51, Inc.
 Author-email: info@voxel51.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,22 +14,21 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pipeline
 Provides-Extra: storage
 License-File: LICENSE
 
 <div align="center">
 
@@ -51,15 +50,15 @@
 </div>
 
 ## Requirements
 
 ETA is very portable:
 
 -   Installable on Mac or Linux
--   Supports Python 2.7 and Python 3.6 or later
+-   Supports Python 3.6 or later
 -   Supports TensorFlow 1.X and 2.X
 -   Supports OpenCV 2.4+ and OpenCV 3.0+
 -   Supports CPU-only and GPU-enabled installations
 -   Supports CUDA 8, 9 and 10 for GPU installations
 
 ## Installation
```

### Comparing `voxel51-eta-0.8.4rc1/README.md` & `voxel51-eta-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 </div>
 
 ## Requirements
 
 ETA is very portable:
 
 -   Installable on Mac or Linux
--   Supports Python 2.7 and Python 3.6 or later
+-   Supports Python 3.6 or later
 -   Supports TensorFlow 1.X and 2.X
 -   Supports OpenCV 2.4+ and OpenCV 3.0+
 -   Supports CPU-only and GPU-enabled installations
 -   Supports CUDA 8, 9 and 10 for GPU installations
 
 ## Installation
```

### Comparing `voxel51-eta-0.8.4rc1/config-example.json` & `voxel51-eta-0.9.0/config-example.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/cli_guide.md` & `voxel51-eta-0.9.0/docs/cli_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/core_dev_guide.md` & `voxel51-eta-0.9.0/docs/core_dev_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/cuda_install_guide.md` & `voxel51-eta-0.9.0/docs/cuda_install_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/custom_opencv_builds.md` & `voxel51-eta-0.9.0/docs/custom_opencv_builds.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/docker_build_guide.md` & `voxel51-eta-0.9.0/docs/docker_build_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/export_tf_graphs_guide.md` & `voxel51-eta-0.9.0/docs/export_tf_graphs_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/image_labels_guide.md` & `voxel51-eta-0.9.0/docs/image_labels_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/linting_guide.md` & `voxel51-eta-0.9.0/docs/linting_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/logging_guide.md` & `voxel51-eta-0.9.0/docs/logging_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/markdown_style_guide.md` & `voxel51-eta-0.9.0/docs/markdown_style_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/models_dev_guide.md` & `voxel51-eta-0.9.0/docs/models_dev_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/modules_dev_guide.md` & `voxel51-eta-0.9.0/docs/modules_dev_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/pipelines_dev_guide.md` & `voxel51-eta-0.9.0/docs/pipelines_dev_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/python23_guide.md` & `voxel51-eta-0.9.0/docs/python23_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/python_style_guide.md` & `voxel51-eta-0.9.0/docs/python_style_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/storage_dev_guide.md` & `voxel51-eta-0.9.0/docs/storage_dev_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/video_labels_guide.md` & `voxel51-eta-0.9.0/docs/video_labels_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/virtualenv_guide.md` & `voxel51-eta-0.9.0/docs/virtualenv_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/docs/visualize_tf_graphs_guide.md` & `voxel51-eta-0.9.0/docs/visualize_tf_graphs_guide.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/__init__.py` & `voxel51-eta-0.9.0/eta/__init__.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/classifiers/tfslim_classifiers.py` & `voxel51-eta-0.9.0/eta/classifiers/tfslim_classifiers.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/classifiers/vgg16_classifiers.py` & `voxel51-eta-0.9.0/eta/classifiers/vgg16_classifiers.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/classifiers/voting_classifiers.py` & `voxel51-eta-0.9.0/eta/classifiers/voting_classifiers.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/constants.py` & `voxel51-eta-0.9.0/eta/constants.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/annotations.py` & `voxel51-eta-0.9.0/eta/core/annotations.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/builder.py` & `voxel51-eta-0.9.0/eta/core/builder.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/c3d.py` & `voxel51-eta-0.9.0/eta/core/c3d.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/cli.py` & `voxel51-eta-0.9.0/eta/core/cli.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/config.py` & `voxel51-eta-0.9.0/eta/core/config.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/data.py` & `voxel51-eta-0.9.0/eta/core/data.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/datasets/builders.py` & `voxel51-eta-0.9.0/eta/core/datasets/builders.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/datasets/labeled_datasets.py` & `voxel51-eta-0.9.0/eta/core/datasets/labeled_datasets.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/datasets/split_methods.py` & `voxel51-eta-0.9.0/eta/core/datasets/split_methods.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/datasets/transformers.py` & `voxel51-eta-0.9.0/eta/core/datasets/transformers.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/datasets/utils.py` & `voxel51-eta-0.9.0/eta/core/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/datasets/video2image.py` & `voxel51-eta-0.9.0/eta/core/datasets/video2image.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/diagram.py` & `voxel51-eta-0.9.0/eta/core/diagram.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/events.py` & `voxel51-eta-0.9.0/eta/core/events.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/features.py` & `voxel51-eta-0.9.0/eta/core/features.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/frames.py` & `voxel51-eta-0.9.0/eta/core/frames.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/frameutils.py` & `voxel51-eta-0.9.0/eta/core/frameutils.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/geometry.py` & `voxel51-eta-0.9.0/eta/core/geometry.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/gps.py` & `voxel51-eta-0.9.0/eta/core/gps.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/graph.py` & `voxel51-eta-0.9.0/eta/core/graph.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/image.py` & `voxel51-eta-0.9.0/eta/core/image.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/job.py` & `voxel51-eta-0.9.0/eta/core/job.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/keypoints.py` & `voxel51-eta-0.9.0/eta/core/keypoints.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/labels.py` & `voxel51-eta-0.9.0/eta/core/labels.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/learning.py` & `voxel51-eta-0.9.0/eta/core/learning.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/logging.py` & `voxel51-eta-0.9.0/eta/core/logging.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/logo.py` & `voxel51-eta-0.9.0/eta/core/logo.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/metadata.py` & `voxel51-eta-0.9.0/eta/core/metadata.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/models.py` & `voxel51-eta-0.9.0/eta/core/models.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/module.py` & `voxel51-eta-0.9.0/eta/core/module.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/numutils.py` & `voxel51-eta-0.9.0/eta/core/numutils.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/objects.py` & `voxel51-eta-0.9.0/eta/core/objects.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/pipeline.py` & `voxel51-eta-0.9.0/eta/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/polylines.py` & `voxel51-eta-0.9.0/eta/core/polylines.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/primitives.py` & `voxel51-eta-0.9.0/eta/core/primitives.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/serial.py` & `voxel51-eta-0.9.0/eta/core/serial.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import numbers
 import os
 import pickle as _pickle
 import pprint
 from uuid import uuid4
 import zlib
 
-import ndjson
+import jsonlines
 import numpy as np
 
 import eta.core.utils as etau
 
 
 logger = logging.getLogger(__name__)
 
@@ -130,24 +130,24 @@
 
     Args:
         path: the path to the NDJSON file
 
     Returns:
         a list of JSON dicts
     """
-    with open(path, "rt") as f:
-        return ndjson.load(f)
+    with jsonlines.open(path) as r:
+        return list(r.iter(skip_empty=True))
 
 
 def load_ndjson(path_or_str):
     """Loads NDJSON from the input argument.
 
     The input argument can be any of the following:
         (a) the path to a NDJSON file on disk
-        (b) a string that can be directly parsed via `ndjson.loads`
+        (b) an NDJSON string or bytes
 
     Args:
         path_or_str: the NDJSON path or string
 
     Returns:
         the loaded NDJSON
 
@@ -158,18 +158,21 @@
         return read_ndjson(path_or_str)
 
     return _load_ndjson(path_or_str)
 
 
 def _load_ndjson(str_or_bytes):
     try:
-        return ndjson.loads(str_or_bytes)
-    except TypeError:
-        # Must be a Python version for which ndjson.loads() cannot handle bytes
-        return ndjson.loads(str_or_bytes.decode("utf-8"))
+        ndjson_str = str_or_bytes.decode("utf-8")
+    except AttributeError:
+        ndjson_str = str_or_bytes
+
+    with io.StringIO(ndjson_str) as f:
+        with jsonlines.Reader(f) as r:
+            return list(r.iter(skip_empty=True))
 
 
 def write_ndjson(obj, path, append=False):
     """Writes the list of JSON dicts to disk in NDJSON format.
 
     Args:
         obj: a list of JSON dicts
@@ -181,15 +184,19 @@
     if append and os.path.exists(path) and os.path.getsize(path) > 0:
         prefix = os.linesep
     else:
         prefix = ""
 
     mode = "at" if append else "wt"
     with open(path, mode) as f:
-        f.write(prefix + ndjson.dumps(obj))
+        if prefix:
+            f.write(prefix)
+
+        with jsonlines.Writer(f) as w:
+            w.write_all(obj)
 
 
 def json_to_str(obj, pretty_print=True):
     """Converts the JSON object to a string.
 
     Args:
         obj: a JSON dictionary or an instance of a Serializable subclass
@@ -1138,16 +1145,16 @@
             path: the path to the element JSON file on disk
         """
         raise NotImplementedError("subclasses must implement add_by_path()")
 
     def add_iterable(self, elements):
         """Adds the elements in the given iterable to the Big iterable.
 
-         Args:
-            elements: an iterable of elements
+        Args:
+           elements: an iterable of elements
         """
         raise NotImplementedError("subclasses must implement add_iterable()")
 
     def clear(self):
         """Deletes all elements from the Big iterable."""
         super(BigMixin, self).clear()
         etau.delete_dir(self.backing_dir)
```

### Comparing `voxel51-eta-0.8.4rc1/eta/core/status.py` & `voxel51-eta-0.9.0/eta/core/status.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/storage.py` & `voxel51-eta-0.9.0/eta/core/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,27 +30,31 @@
 # pragma pylint: enable=unused-wildcard-import
 # pragma pylint: enable=wildcard-import
 
 import configparser
 import datetime
 import dateutil.parser
 import io
+import itertools
 import logging
 import os
 import re
 import requests
 
 try:
     import urllib.parse as urlparse  # Python 3
 except ImportError:
     import urlparse  # Python 2
 
 import urllib3
 
 try:
+    import azure.identity as azi
+    import azure.storage.blob as azb
+    import azure.core.exceptions as aze
     import boto3
     import botocore
     import botocore.config as bcc
     import botocore.exceptions as bce
     import google.api_core.exceptions as gae
     import google.api_core.retry as gar
     import google.auth as ga
@@ -69,14 +73,19 @@
         e,
     )
 
 import eta.constants as etac
 import eta.core.serial as etas
 import eta.core.utils as etau
 
+aks = etau.lazy_import(
+    "azure.keyvault.secrets",
+    callback=lambda: etau.ensure_package("azure-keyvault-secrets"),
+)
+
 
 logger = logging.getLogger(__name__)
 
 
 # Suppress non-critical logging from third-party libraries
 logging.getLogger("googleapiclient").setLevel(logging.ERROR)
 logging.getLogger("paramiko").setLevel(logging.ERROR)
@@ -954,27 +963,27 @@
             folder_name += "/"
 
         kwargs = {"Bucket": bucket, "Prefix": folder_name}
         if not recursive:
             kwargs["Delimiter"] = "/"
 
         paths_or_metadata = []
-        prefix = self._get_prefix(cloud_folder) + bucket
+        prefix = self._get_prefix(cloud_folder) + bucket + "/"
         while True:
             resp = self._client.list_objects_v2(**kwargs)
 
             for obj in resp.get("Contents", []):
                 path = obj["Key"]
                 if not path.endswith("/"):
                     if return_metadata:
                         paths_or_metadata.append(
                             self._get_object_metadata(bucket, obj)
                         )
                     else:
-                        paths_or_metadata.append(prefix + "/" + path)
+                        paths_or_metadata.append(prefix + path)
 
             try:
                 kwargs["ContinuationToken"] = resp["NextContinuationToken"]
             except KeyError:
                 break
 
         return paths_or_metadata
@@ -1165,15 +1174,14 @@
 
         (2) loading credentials from `~/.eta/aws-credentials.ini` that have
             been activated via `cls.activate_credentials()`
 
         (3) setting credentials in any manner used by Boto3
             https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html
 
-
     In the above, the `.ini` file should have syntax similar to the following::
 
         [default]
         aws_access_key_id = ...
         aws_secret_access_key = ...
         aws_session_token = ...  # if applicable
         region = ...
@@ -1390,15 +1398,14 @@
 
         (4) setting the `MINIO_SHARED_CREDENTIALS_FILE` environment variable to
             point to a valid credentials `.ini` file
 
         (5) setting the `MINIO_CONFIG_FILE` environment variable to point to a
             valid credentials `.ini` file
 
-
     In the above, the `.ini` file should have syntax similar to the following::
 
         [default]
         access_key = ...
         secret_access_key = ...
         endpoint_url = ...
         alias = ...  # optional
@@ -1505,15 +1512,15 @@
                     "Loading endpoint URL from 'MINIO_ENDPOINT_URL' "
                     "environment variable"
                 )
                 credentials["endpoint_url"] = os.environ["MINIO_ENDPOINT_URL"]
 
             if "MINIO_ALIAS" in os.environ:
                 logger.debug(
-                    "Loading region from 'MINIO_ALIAS' environment variable"
+                    "Loading alias from 'MINIO_ALIAS' environment variable"
                 )
                 credentials["alias"] = os.environ["MINIO_ALIAS"]
 
             if "MINIO_REGION" in os.environ:
                 logger.debug(
                     "Loading region from 'MINIO_REGION' environment variable"
                 )
@@ -1661,16 +1668,14 @@
 
         (2) loading credentials from `~/.eta/google-credentials.json` that have
             been activated via `cls.activate_credentials()`
 
         (3) setting credentials in any manner used by Application Default Credentials
             https://cloud.google.com/docs/authentication/production#automatically
 
-
-
     In the above, the service account JSON file should have syntax similar to
     the following::
 
         {
           "type": "service_account",
           "project_id": "<project-id>",
           "private_key_id": "<private-key-id>",
@@ -1825,15 +1830,14 @@
             chunk_size: an optional chunk size (in bytes) to use for uploads
                 and downloads
             max_pool_connections: an optional maximum number of connections to
                 keep in the connection pool
             **kwargs: optional keyword arguments for
                 `google.cloud.storage.Client(**kwargs)`
         """
-
         if credentials is None:
             credentials, _ = self.load_credentials()
 
         try:
             client = gcs.Client(credentials=credentials, **kwargs)
         except ga.exceptions.DefaultCredentialsError:
             raise GoogleCredentialsError("No Google credentials found")
@@ -2217,14 +2221,861 @@
 
         if len(chunks) != 2:
             return chunks[0], ""
 
         return chunks[0], chunks[1]
 
 
+class NeedsAzureCredentials(object):
+    """Mixin for classes that need Azure credentials to take authenticated
+    actions.
+
+    Storage clients that derive from this class should allow users to provide
+    credentials in the following ways (in order of precedence):
+
+        (1) manually constructing an instance of the class via the
+            `cls.from_ini()` method by providing a path to a valid
+            credentials file
+
+        (2) loading credentials from `~/.eta/azure-credentials.ini` that have
+            been activated via `cls.activate_credentials()`
+
+        (3) setting the `AZURE_CREDENTIALS_FILE` environment variable to point
+            to a valid credentials `.ini` file
+
+        (4) setting the following environment variables directly:
+
+            -   `AZURE_STORAGE_CONNECTION_STRING`
+
+        (5) setting the following environment variables directly:
+
+            -   `AZURE_STORAGE_ACCOUNT`
+            -   `AZURE_STORAGE_KEY`
+
+        (6) setting the following environment variables directly:
+
+            -   `AZURE_CLIENT_ID`
+            -   `AZURE_CLIENT_SECRET`
+            -   `AZURE_TENANT_ID`
+            -   `AZURE_STORAGE_ACCOUNT`
+
+        (7) setting credentials in any manner recognized by
+            `azure.identity.DefaultAzureCredential`
+
+    In the above, the credentials file should have syntax simliar to one of the
+    following::
+
+        [default]
+        conn_str = ...
+        alias = ...  # optional
+
+        [default]
+        account_name = ...
+        account_key = ...
+        alias = ...  # optional
+
+        [default]
+        client_id = ...
+        secret = ...
+        tenant = ...
+        account_name = ...
+
+    See the following pages for more information:
+
+    -   https://learn.microsoft.com/en-us/azure/storage/blobs/authorize-data-operations-cli
+    -   https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/storage/azure-storage-blob
+    """
+
+    CREDENTIALS_PATH = os.path.join(
+        etac.ETA_CONFIG_DIR, "azure-credentials.ini"
+    )
+
+    @classmethod
+    def activate_credentials(cls, credentials_path):
+        """Activate the credentials by copying them to
+        `~/.eta/azure-credentials.ini`.
+
+        Args:
+            credentials_path: the path to a credentials `.ini` file
+        """
+        etau.copy_file(credentials_path, cls.CREDENTIALS_PATH)
+        logger.info(
+            "Azure credentials successfully activated at '%s'",
+            cls.CREDENTIALS_PATH,
+        )
+
+    @classmethod
+    def deactivate_credentials(cls):
+        """Deactivates (deletes) the currently active credentials, if any.
+
+        Active credentials (if any) are at `~/.eta/azure-credentials.ini`.
+        """
+        try:
+            os.remove(cls.CREDENTIALS_PATH)
+            logger.info(
+                "Azure credentials '%s' successfully deactivated",
+                cls.CREDENTIALS_PATH,
+            )
+        except OSError:
+            logger.info("No Azure credentials to deactivate")
+
+    @classmethod
+    def has_active_credentials(cls):
+        """Determines whether there are any active credentials stored at
+        `~/.eta/azure-credentials.ini`.
+
+        Returns:
+            True/False
+        """
+        return os.path.isfile(cls.CREDENTIALS_PATH)
+
+    @classmethod
+    def load_credentials(cls, credentials_path=None, profile=None):
+        """Loads the Azure credentials as a dictionary.
+
+        Args:
+            credentials_path: an optional path to a credentials `.ini` file.
+                If omitted, active credentials are located using the strategy
+                described in the class docstring of `NeedsAzureCredentials`
+            profile: an optional profile to load when a credentials `.ini` file
+                is loaded (if applicable). If not provided, the "default"
+                section is loaded
+
+        Returns:
+            a (credentials, path) tuple containing the credentials and the path
+                from which they were loaded. If no credentials can be loaded,
+                `credentials` and `path` will be both be None.
+        """
+        if credentials_path:
+            logger.debug(
+                "Loading Azure credentials from manually provided path '%s'",
+                credentials_path,
+            )
+        elif cls.has_active_credentials():
+            credentials_path = cls.CREDENTIALS_PATH
+            logger.debug(
+                "Loading activated Azure credentials from '%s'",
+                credentials_path,
+            )
+        else:
+            credentials = {}
+
+            if "AZURE_STORAGE_CONNECTION_STRING" in os.environ:
+                logger.debug(
+                    "Loading connection string from "
+                    "'AZURE_STORAGE_CONNECTION_STRING' environment variable"
+                )
+                conn_str = os.environ["AZURE_STORAGE_CONNECTION_STRING"]
+                credentials["conn_str"] = conn_str
+
+            if "AZURE_STORAGE_ACCOUNT_URL" in os.environ:
+                logger.debug(
+                    "Loading account URL from 'AZURE_STORAGE_ACCOUNT_URL' "
+                    "environment variable"
+                )
+                account_url = os.environ["AZURE_STORAGE_ACCOUNT_URL"]
+                credentials["account_url"] = account_url
+
+            if "AZURE_STORAGE_ACCOUNT" in os.environ:
+                logger.debug(
+                    "Loading account name from 'AZURE_STORAGE_ACCOUNT' "
+                    "environment variable"
+                )
+                account_name = os.environ["AZURE_STORAGE_ACCOUNT"]
+                credentials["account_name"] = account_name
+
+            if "AZURE_STORAGE_KEY" in os.environ:
+                logger.debug(
+                    "Loading account key from 'AZURE_STORAGE_KEY' "
+                    "environment variable"
+                )
+                credentials["account_key"] = os.environ["AZURE_STORAGE_KEY"]
+
+            if "AZURE_CLIENT_ID" in os.environ:
+                logger.debug(
+                    "Loading client ID from 'AZURE_CLIENT_ID' environment "
+                    "variable"
+                )
+                credentials["client_id"] = os.environ["AZURE_CLIENT_ID"]
+
+            if "AZURE_CLIENT_SECRET" in os.environ:
+                logger.debug(
+                    "Loading client secret from 'AZURE_CLIENT_SECRET' "
+                    "environment variable"
+                )
+                credentials["secret"] = os.environ["AZURE_CLIENT_SECRET"]
+
+            if "AZURE_TENANT_ID" in os.environ:
+                logger.debug(
+                    "Loading tenant ID from 'AZURE_TENANT_ID' environment "
+                    "variable"
+                )
+                credentials["tenant"] = os.environ["AZURE_TENANT_ID"]
+
+            if "AZURE_ALIAS" in os.environ:
+                logger.debug(
+                    "Loading alias from 'AZURE_ALIAS' environment variable"
+                )
+                credentials["alias"] = os.environ["AZURE_ALIAS"]
+
+            return credentials, None
+
+        if profile is None and "AZURE_PROFILE" in os.environ:
+            logger.debug(
+                "Loading profile from 'AZURE_PROFILE' environment variable"
+            )
+            profile = os.environ["AZURE_PROFILE"]
+
+        credentials = cls._load_credentials_ini(
+            credentials_path, profile=profile
+        )
+
+        return credentials, credentials_path
+
+    @classmethod
+    def load_secret(cls, key_vault_url, secret_name, credential):
+        """Loads the secret with the given name from Azure Key Vault.
+
+        Args:
+            key_vault_url: the key vault URL
+            secret_name: the name of the secret to load
+            credential: an `azure.core.credentials.TokenCredential` to use
+        """
+        # Reference
+        # https://learn.microsoft.com/en-us/azure/key-vault/secrets/quick-create-python?tabs=azure-cli
+        client = aks.SecretClient(
+            vault_url=key_vault_url, credential=credential
+        )
+        return client.get_secret(secret_name).value
+
+    @classmethod
+    def from_ini(cls, credentials_path, profile=None):
+        """Creates a `cls` instance from the given credentials `.ini` file.
+
+        Args:
+            credentials_path: the path to a credentials `.ini` file
+            profile: an optional profile to load. If not provided the "default"
+                section is loaded
+
+        Returns:
+            an instance of cls with the given credentials
+        """
+        credentials, _ = cls.load_credentials(
+            credentials_path=credentials_path, profile=profile
+        )
+        return cls(credentials=credentials)
+
+    @classmethod
+    def _load_credentials_ini(cls, credentials_path, profile=None):
+        if profile is None:
+            profile = "default"
+
+        if not os.path.isfile(credentials_path):
+            raise FileNotFoundError(
+                "File '%s' does not exist" % credentials_path
+            )
+
+        config = configparser.ConfigParser()
+        config.read(credentials_path)
+        return dict(config[profile])
+
+
+class AzureCredentialsError(Exception):
+    """Error raised when a problem with Azure credentials is encountered."""
+
+    def __init__(self, message):
+        """Creates an AzureCredentialsError instance.
+
+        Args:
+            message: the error message
+        """
+        super(AzureCredentialsError, self).__init__(
+            "%s. Read the documentation for "
+            "`eta.core.storage.NeedsAzureCredentials` for more information "
+            "about authenticating with Azure services." % message
+        )
+
+
+class AzureStorageClient(
+    StorageClient, CanSyncDirectories, NeedsAzureCredentials
+):
+    """Client for reading/writing data from Azure Blob Storage.
+
+    All cloud path strings used by this class should have the form
+    "https://<account>.blob.core.windows.net/<container>/<path/to/object>".
+
+    See `NeedsAzureCredentials` for more information about the authentication
+    strategy used by this class.
+    """
+
+    def __init__(self, credentials=None, max_pool_connections=None):
+        """Creates an AzureStorageClient instance.
+
+        Args:
+            credentials: the credentials to use. If not provided, this is
+                automatically loaded as described in `NeedsAzureCredentials`
+            max_pool_connections: an optional maximum number of connections to
+                keep in the connection pool
+        """
+        if credentials is None:
+            credentials, _ = self.load_credentials()
+
+        tenant_id = credentials.get("tenant", None)
+        client_id = credentials.get("client_id", None)
+        client_secret = credentials.get("secret", None)
+        account_url = credentials.get("account_url", None)
+        account_name = credentials.get("account_name", None)
+        account_key = credentials.get("account_key", None)
+        conn_str = credentials.get("conn_str", None)
+        alias = credentials.pop("alias", None)
+
+        # https://github.com/Azure/azure-sdk-for-python/issues/12102#issuecomment-645641481
+        if max_pool_connections is not None:
+            adapter = requests.adapters.HTTPAdapter(
+                pool_maxsize=max_pool_connections
+            )
+
+            session = requests.Session()
+            session.mount("http://", adapter)
+            session.mount("https://", adapter)
+        else:
+            session = None
+
+        if conn_str is not None:
+            client = azb.BlobServiceClient.from_connection_string(
+                conn_str=conn_str,
+                session=session,
+            )
+
+            account_name = client.account_name
+            account_url = client.url
+            account_key = getattr(client.credential, "account_key", None)
+            credential = client.credential
+        else:
+            if account_key is not None:
+                if account_url is not None:
+                    if account_name is None:
+                        raise AzureCredentialsError(
+                            "You must also provide your account name when "
+                            "using a custom account URL"
+                        )
+
+                    credential = {
+                        "account_name": account_name,
+                        "account_key": account_key,
+                    }
+                else:
+                    credential = account_key
+            elif tenant_id and client_id and client_secret:
+                credential = azi.ClientSecretCredential(
+                    tenant_id, client_id, client_secret
+                )
+            else:
+                credential = azi.DefaultAzureCredential()
+
+            if account_url is None:
+                if account_name is None:
+                    raise AzureCredentialsError(
+                        "You must provide an account name, account URL, or "
+                        "connection string"
+                    )
+
+                account_url = "https://%s.blob.core.windows.net" % account_name
+
+            client = azb.BlobServiceClient(
+                account_url=account_url,
+                credential=credential,
+                session=session,
+            )
+
+            account_name = client.account_name
+
+        # Load `account_key` from secret
+        # https://learn.microsoft.com/en-us/azure/key-vault/secrets/quick-create-python?tabs=azure-cli
+        if account_key is None and (
+            "AZURE_KEY_VAULT_URL" in os.environ
+            and "AZURE_ACOUNT_KEY_SECRET_NAME" in os.environ
+        ):
+            logger.debug(
+                "Loading vault URL and secret name from 'AZURE_KEY_VAULT_URL' "
+                "and 'AZURE_ACOUNT_KEY_SECRET_NAME' environment variables"
+            )
+            vault_url = os.environ["AZURE_KEY_VAULT_URL"]
+            secret_name = os.environ["AZURE_ACOUNT_KEY_SECRET_NAME"]
+            account_key = self.load_secret(vault_url, secret_name, credential)
+
+        prefixes = []
+        if alias is not None:
+            prefixes.append(alias + "://")
+
+        prefixes.append(account_url.rstrip("/") + "/")
+
+        self._client = client
+        self._account_name = account_name
+        self._account_url = account_url.rstrip("/")
+        self._account_key = account_key
+        self._alias = alias
+        self._prefixes = tuple(prefixes)
+
+        self._user_delegation_key = None
+        self._user_delegation_expiration = None
+
+        if self._account_key is None:
+            self._generate_user_delegation_key()
+
+        self._permissions = {
+            "GET": azb.BlobSasPermissions(read=True),
+            "PUT": azb.BlobSasPermissions(create=True),
+            "DELETE": azb.BlobSasPermissions(delete=True),
+        }
+
+    def upload(self, local_path, cloud_path, content_type=None, metadata=None):
+        """Uploads the file to Azure Storage.
+
+        Args:
+            local_path: the path to the file to upload
+            cloud_path: the path to the Azure object to create
+            content_type: the optional type of the content being uploaded. If
+                no value is provided, it is guessed from the filename
+            metadata: an optional dictionary of custom object metadata to store
+        """
+        with open(local_path, "rb") as f:
+            self._do_upload(
+                f, cloud_path, content_type=content_type, metadata=metadata
+            )
+
+    def upload_bytes(
+        self, bytes_str, cloud_path, content_type=None, metadata=None
+    ):
+        """Uploads the given bytes to Azure Storage.
+
+        Args:
+            bytes_str: the bytes string to upload
+            cloud_path: the path to the Azure object to create
+            content_type: the optional type of the content being uploaded. If
+                no value is provided, it is guessed from the filename
+            metadata: an optional dictionary of custom object metadata to store
+        """
+        with io.BytesIO(_to_bytes(bytes_str)) as f:
+            self._do_upload(
+                f, cloud_path, content_type=content_type, metadata=metadata
+            )
+
+    def upload_stream(
+        self, file_obj, cloud_path, content_type=None, metadata=None
+    ):
+        """Uploads the contents of the given file-like object to Azure Storage.
+
+        Args:
+            file_obj: the file-like object to upload, which must be open for
+                reading
+            cloud_path: the path to the Azure object to create
+            content_type: the optional type of the content being uploaded. If
+                no value is provided, it is guessed from the filename
+            metadata: an optional dictionary of custom object metadata to store
+        """
+        self._do_upload(
+            file_obj, cloud_path, content_type=content_type, metadata=metadata
+        )
+
+    def download(self, cloud_path, local_path):
+        """Downloads the file from Azure Storage to the given location.
+
+        Args:
+            cloud_path: the path to the Azure Storage object to download
+            local_path: the local disk path to store the downloaded file
+        """
+        self._do_download(cloud_path, local_path=local_path)
+
+    def download_bytes(self, cloud_path, start=None, end=None):
+        """Downloads the file from Azure Storage and returns the bytes string.
+
+        Args:
+            cloud_path: the path to the Azure Storage object to download
+            start: an optional first byte in a range to download
+            end: an optional last byte in a range to download
+
+        Returns:
+            the downloaded bytes string
+        """
+        with io.BytesIO() as f:
+            self._do_download(cloud_path, file_obj=f, start=start, end=end)
+            return f.getvalue()
+
+    def download_stream(self, cloud_path, file_obj):
+        """Downloads the file from Azure Storage to the given file-like object.
+
+        Args:
+            cloud_path: the path to the Azure Storage object to download
+            file_obj: the file-like object to which to write the download,
+                which must be open for writing
+        """
+        self._do_download(cloud_path, file_obj=file_obj)
+
+    def delete(self, cloud_path):
+        """Deletes the given file from Azure Storage.
+
+        Args:
+            cloud_path: the path to the Azure Storage object to delete
+        """
+        blob = self._get_blob_client(cloud_path)
+        blob.delete_blob()
+
+    def delete_folder(self, cloud_folder):
+        """Deletes all files in the given Azure Storage "folder".
+
+        Args:
+            cloud_folder: a string like
+                `https://<account-name>.blob.core.windows.net/<container-name>/<folder-path>`
+        """
+        container_name, folder_name = self._parse_path(cloud_folder)
+        if folder_name and not folder_name.endswith("/"):
+            folder_name += "/"
+
+        blobs = self._list_blobs(container_name, prefix=folder_name)
+
+        client = self._client.get_container_client(container_name)
+        for _blobs in etau.iter_batches(blobs, 256):
+            client.delete_blobs(*[b.name for b in _blobs])
+
+    def get_file_metadata(self, cloud_path):
+        """Returns metadata about the given file in Azure Storage.
+
+        Args:
+            cloud_path: the path to the Azure Storage object
+
+        Returns:
+            a dictionary containing metadata about the file, including its
+                `bucket`, `object_name`, `name`, `size`, `mime_type`,
+                `last_modified`, `etag`, and `metadata`
+        """
+        blob = self._get_blob_client(cloud_path)
+        blob_properties = blob.get_blob_properties()
+        return self._get_file_metadata(blob_properties)
+
+    def get_folder_metadata(self, cloud_folder):
+        """Returns metadata about the given "folder" in Azure Storage.
+
+        Note that this method is *expensive*; the only way to compute this
+        information is to call `list_files_in_folder(..., recursive=True)` and
+        compute stats from individual files!
+
+        Args:
+            cloud_folder: a string like
+                `https://<account-name>.blob.core.windows.net/<container-name>/<folder-path>`
+
+        Returns:
+            a dictionary containing metadata about the "folder", including its
+                `bucket`, `path`, `num_files`, `size`, and `last_modified`
+        """
+        files = self.list_files_in_folder(
+            cloud_folder, recursive=True, return_metadata=True
+        )
+
+        container_name, path = self._parse_path(cloud_folder)
+        path = path.rstrip("/")
+
+        if files:
+            num_files = len(files)
+            size = sum(f["size"] for f in files)
+            last_modified = max(f["last_modified"] for f in files)
+        else:
+            num_files = 0
+            size = 0
+            last_modified = "-"
+
+        return {
+            "bucket": container_name,
+            "path": path,
+            "num_files": num_files,
+            "size": size,
+            "last_modified": last_modified,
+        }
+
+    def is_file(self, cloud_path):
+        """Determines whether the given Azure Storage file exists.
+
+        Args:
+            cloud_path: the path to the Azure Storage object
+
+        Returns:
+            True/False
+        """
+        blob = self._get_blob_client(cloud_path)
+        return blob.exists()
+
+    def is_folder(self, cloud_folder):
+        """Determines whether the given Azure Storage "folder" contains at
+        least one object.
+
+        Args:
+            cloud_folder: a string like
+                `https://<account-name>.blob.core.windows.net/<container-name>/<folder-path>`
+
+        Returns:
+            True/False
+        """
+        container_name, folder_name = self._parse_path(cloud_folder)
+        if folder_name and not folder_name.endswith("/"):
+            folder_name += "/"
+
+        blobs = self._list_blobs(
+            container_name, prefix=folder_name, max_results=1
+        )
+
+        return bool(list(blobs))
+
+    def list_files_in_folder(
+        self, cloud_folder, recursive=True, return_metadata=False
+    ):
+        """Returns a list of the files in the given "folder" in Azure Storage.
+
+        Args:
+            cloud_folder: a string like
+                `https://<account-name>.blob.core.windows.net/<container-name>/<folder-path>`
+            recursive: whether to recursively traverse sub-"folders". By
+                default, this is True
+            return_metadata: whether to return a metadata dictionary for each
+                file, including its  `bucket`, `object_name`, `name`, `size`,
+                `mime_type`, `last_modified`, `etag`, and `metadata`. By
+                default, only the paths to the files are returned
+
+        Returns:
+            a list of full cloud paths (when `return_metadata == False`) or a
+                list of metadata dictionaries (when `return_metadata == True`)
+                for the files in the folder
+        """
+        container_name, folder_name = self._parse_path(cloud_folder)
+        if folder_name and not folder_name.endswith("/"):
+            folder_name += "/"
+
+        blobs = self._list_blobs(
+            container_name, prefix=folder_name, recursive=recursive
+        )
+
+        # Return metadata dictionaries for each file
+        if return_metadata:
+            metadata = []
+            for blob in blobs:
+                if not blob.name.endswith("/"):
+                    metadata.append(self._get_file_metadata(blob))
+
+            return metadata
+
+        # Return paths for each file
+        paths = []
+        prefix = self._get_prefix(cloud_folder) + container_name + "/"
+        for blob in blobs:
+            if not blob.name.endswith("/"):
+                paths.append(prefix + blob.name)
+
+        return paths
+
+    def generate_signed_url(
+        self, cloud_path, method="GET", hours=24, content_type=None
+    ):
+        """Generates a signed URL for accessing the given Azure Storage object.
+
+        Anyone with the URL can access the object with the permission until it
+        expires.
+
+        Note that you should use `PUT`, not `POST`, to upload objects!
+
+        Args:
+            cloud_path: the path to the Azure Storage object
+            method: the HTTP verb (GET, PUT, DELETE) to authorize
+            hours: the number of hours that the URL is valid
+            content_type: (PUT actions only) the optional type of the content
+                being uploaded
+
+        Returns:
+            a URL for accessing the object via HTTP request
+        """
+        container_name, blob_name = self._parse_path(cloud_path)
+
+        self._refresh_user_delegation_key_if_necessary()
+
+        permission = self._permissions[method.upper()]
+        expiry = datetime.datetime.utcnow() + datetime.timedelta(hours=hours)
+
+        signature = azb.generate_blob_sas(
+            account_name=self._account_name,
+            container_name=container_name,
+            blob_name=blob_name,
+            account_key=self._account_key,
+            user_delegation_key=self._user_delegation_key,
+            permission=permission,
+            expiry=expiry,
+            content_type=content_type,
+        )
+
+        root = self._account_url
+        return root + "/" + container_name + "/" + blob_name + "?" + signature
+
+    def add_metadata(self, cloud_path, metadata):
+        """Adds custom metadata key-value pairs to the given Azure Storage
+        object.
+
+        Args:
+            cloud_path: the path to the Azure Storage object
+            metadata: a dictionary of custom metadata
+        """
+        blob = self._get_blob_client(cloud_path)
+
+        blob_metadata = blob.get_blob_properties().metadata
+        blob_metadata.update(metadata)
+        blob.set_blob_metadata(metadata=blob_metadata)
+
+    def _refresh_user_delegation_key_if_necessary(self):
+        if self._user_delegation_key is None:
+            return
+
+        if datetime.datetime.utcnow() > self._user_delegation_expiration:
+            self._generate_user_delegation_key()
+
+    def _generate_user_delegation_key(self, hours=24):
+        # Requires `_client` to have been initialized with a token credential?
+        # https://azuresdkdocs.blob.core.windows.net/$web/python/azure-storage-blob/12.0.0b5/_modules/azure/storage/blob/_shared_access_signature.html
+        now = datetime.datetime.utcnow()
+        expiration = now + datetime.timedelta(hours=hours)
+        key = self._client.get_user_delegation_key(now, expiration)
+
+        self._user_delegation_key = key
+        self._user_delegation_expiration = expiration
+
+    def _get_container_client(self, cloud_path):
+        container_name, _ = self._parse_path(cloud_path)
+        return self._client.get_container_client(container_name)
+
+    def _get_blob_client(self, cloud_path):
+        container_name, blob_name = self._parse_path(cloud_path)
+        return self._client.get_blob_client(container_name, blob_name)
+
+    def _parse_path(self, cloud_path):
+        try:
+            client = azb.BlobClient.from_blob_url(cloud_path)
+            return client.container_name, client.blob_name
+        except ValueError as e:
+            try:
+                client = azb.ContainerClient.from_container_url(cloud_path)
+                return client.container_name, ""
+            except:
+                raise e
+
+    def _get_prefix(self, cloud_path):
+        return _get_prefix(cloud_path, self._prefixes)
+
+    def _strip_prefix(self, cloud_path):
+        _cloud_path = _strip_prefix(cloud_path, self._prefixes)
+
+        if _cloud_path is None:
+            if len(self._prefixes) == 1:
+                valid_prefixes = "'%s'" % self._prefixes[0]
+            else:
+                valid_prefixes = self._prefixes
+
+            raise ValueError(
+                "Invalid path '%s'; must start with %s"
+                % (cloud_path, valid_prefixes)
+            )
+
+        return _cloud_path
+
+    def _do_upload(
+        self, file_obj, cloud_path, content_type=None, metadata=None
+    ):
+        if content_type is None:
+            content_type = etau.guess_mime_type(cloud_path)
+
+        blob = self._get_blob_client(cloud_path)
+        content_settings = azb.ContentSettings(content_type=content_type)
+
+        blob.upload_blob(
+            file_obj,
+            metadata=metadata,
+            overwrite=True,
+            content_settings=content_settings,
+        )
+
+    def _do_download(
+        self,
+        cloud_path,
+        local_path=None,
+        file_obj=None,
+        start=None,
+        end=None,
+    ):
+        blob = self._get_blob_client(cloud_path)
+
+        offset = None
+        length = None
+        if start is not None:
+            offset = start
+            if end is not None:
+                length = end - start
+        elif end is not None:
+            length = end
+
+        if local_path is not None:
+            etau.ensure_basedir(local_path)
+            with open(local_path, "wb") as f:
+                blob.download_blob(offset=offset, length=length).readinto(f)
+
+        if file_obj is not None:
+            blob.download_blob(offset=offset, length=length).readinto(file_obj)
+
+    def _list_blobs(
+        self, container_name, prefix=None, recursive=True, max_results=None
+    ):
+        container = self._client.get_container_client(container_name)
+
+        try:
+            if recursive:
+                r = container.list_blobs(name_starts_with=prefix)
+            else:
+                r = container.walk_blobs(
+                    name_starts_with=prefix, delimiter="/"
+                )
+
+            if max_results is not None:
+                return itertools.islice(r, max_results)
+
+            return r
+        except aze.ResourceNotFoundError:
+            return []
+
+    @staticmethod
+    def _to_account_url(conn_str=None, account_name=None):
+        if conn_str is not None:
+            client = azb.BlobServiceClient.from_connection_string(
+                conn_str=conn_str
+            )
+            return client.url
+
+        if account_name is not None:
+            return "https://%s.blob.core.windows.net" % account_name
+
+    @staticmethod
+    def _get_file_metadata(blob_properties):
+        mime_type = blob_properties.content_settings.content_type
+        if not mime_type:
+            mime_type = etau.guess_mime_type(blob_properties.name)
+
+        return {
+            "bucket": blob_properties.container,
+            "object_name": blob_properties.name,
+            "name": os.path.basename(blob_properties.name),
+            "size": blob_properties.size,
+            "mime_type": mime_type,
+            "last_modified": blob_properties.creation_time,
+            "etag": blob_properties.etag,
+            "metadata": blob_properties.metadata,
+        }
+
+
 class GoogleDriveStorageClient(StorageClient, NeedsGoogleCredentials):
     """Client for reading/writing data from Google Drive.
 
     The service account credentials you use must have access permissions for
     any Drive folders you intend to access.
 
     See `NeedsGoogleCredentials` for more information about the authentication
@@ -2498,14 +3349,15 @@
         Returns:
             the name of the Team Drive
 
         Raises:
             GoogleDriveStorageClientError: if the Team Drive was not found
         """
         try:
+            # pylint: disable=no-member
             response = (
                 self._service.teamdrives().get(teamDriveId=drive_id).execute()
             )
             return response["name"]
         except:
             raise GoogleDriveStorageClientError(
                 "Team Drive with ID '%s' not found" % drive_id
```

### Comparing `voxel51-eta-0.8.4rc1/eta/core/tfutils.py` & `voxel51-eta-0.9.0/eta/core/tfutils.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/types.py` & `voxel51-eta-0.9.0/eta/core/types.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/utils.py` & `voxel51-eta-0.9.0/eta/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,19 @@
 import itertools as it
 import logging
 import math
 import mimetypes
 import numbers
 import os
 from packaging.requirements import Requirement
-import patoolib
 import pkg_resources
+import py7zr
 import pytz
 import random
+import rarfile
 import re
 import shutil
 import signal
 import string
 import subprocess
 import sys
 import tarfile
@@ -3555,67 +3556,37 @@
 
     return os.path.splitext(archive_path)
 
 
 def extract_archive(archive_path, outdir=None, delete_archive=False):
     """Extracts the contents of an archive.
 
-    The following formats are guaranteed to work:
-    `.zip`, `.tar`, `.tar.gz`, `.tgz`, `.tar.bz`, `.tbz`.
-
-    If an archive *not* in the above list is found, extraction will be
-    attempted via the `patool` package, which supports many formats but may
-    require that additional system packages be installed.
+    The following formats are supported:
+    `.zip`, `.tar`, `.tar.gz`, `.tgz`, `.tar.bz`, `.tbz`, `.7z`, and `.rar`.
 
     Args:
         archive_path: the path to the archive file
         outdir: the directory into which to extract the archive contents. By
             default, the directory containing the archive is used
         delete_archive: whether to delete the archive after extraction. By
             default, this is False
     """
     if archive_path.endswith(".zip"):
         extract_zip(archive_path, outdir=outdir, delete_zip=delete_archive)
-    elif archive_path.endswith(".rar"):
-        extract_rar(archive_path, outdir=outdir, delete_rar=delete_archive)
     elif archive_path.endswith((".tar", ".tar.gz", ".tgz", ".tar.bz", ".tbz")):
         extract_tar(archive_path, outdir=outdir, delete_tar=delete_archive)
+    elif archive_path.endswith(".7z"):
+        extract_7z(archive_path, outdir=outdir, delete_zip=delete_archive)
+    elif archive_path.endswith(".rar"):
+        extract_rar(archive_path, outdir=outdir, delete_rar=delete_archive)
     else:
-        # Fallback to `patoolib`, which handles a lot of stuff, possibly
-        # requiring the user to install system packages
-        _extract_archive_patoolib(
-            archive_path, outdir=outdir, delete_archive=delete_archive
-        )
-
-
-def extract_rar(rar_path, outdir=None, delete_rar=False):
-    """Extracts the contents of a .rar file.
-
-    This method will complain if you do not have a system package like `unrar`
-    installed that can perform the actual extraction.
-
-    Args:
-        rar_path: the path to the RAR file
-        outdir: the directory into which to extract the RAR contents. By
-            default, the directory containing the RAR file is used
-        delete_rar: whether to delete the RAR after extraction. By default,
-            this is False
-    """
-    try:
-        _extract_archive_patoolib(
-            rar_path, outdir=outdir, delete_archive=delete_rar
+        raise ValueError(
+            "Expected file '%s' to have extension .zip, .tar, .tar.gz, .tgz, "
+            ".tar.bz, .tbz, .7z, or .rar in order to extract it" % archive_path
         )
-    except patoolib.util.PatoolError as e:
-        message = (
-            "Failed to extract RAR file '%s'. Extracting RAR files requires a "
-            "system package like `unrar` to be installed on your machine, "
-            "which you may need to install. Check the error message above for "
-            "more information."
-        ) % rar_path
-        six.raise_from(IOError(message), e)
 
 
 def extract_zip(zip_path, outdir=None, delete_zip=False):
     """Extracts the contents of a .zip file.
 
     Args:
         zip_path: the path to the zip file
@@ -3654,32 +3625,70 @@
     else:
         raise ValueError(
             "Expected file '%s' to have extension .tar, .tar.gz, .tgz,"
             ".tar.bz, or .tbz in order to extract it" % tar_path
         )
 
     outdir = outdir or os.path.dirname(tar_path) or "."
+
     with tarfile.open(tar_path, fmt) as f:
         f.extractall(path=outdir)
 
     if delete_tar:
         delete_file(tar_path)
 
 
-def _extract_archive_patoolib(archive_path, outdir=None, delete_archive=False):
-    outdir = outdir or os.path.dirname(archive_path) or "."
+def extract_7z(zip_path, outdir=None, delete_zip=False):
+    """Extracts the contents of a .7z file.
 
-    ensure_dir(outdir)
+    Args:
+        zip_path: the path to the zip file
+        outdir: the directory into which to extract the zip contents. By
+            default, the directory containing the zip file is used
+        delete_zip: whether to delete the zip after extraction. By default,
+            this is False
+    """
+    outdir = outdir or os.path.dirname(zip_path) or "."
 
-    patoolib.extract_archive(
-        archive_path, outdir=outdir, verbosity=-1, interactive=False
-    )
+    with py7zr.SevenZipFile(zip_path, "r") as f:
+        f.extractall(path=outdir)
+
+    if delete_zip:
+        delete_file(zip_path)
 
-    if delete_archive:
-        delete_file(archive_path)
+
+def extract_rar(rar_path, outdir=None, delete_rar=False):
+    """Extracts the contents of a .rar file.
+
+    This method will complain if you do not have a system package like `unrar`
+    installed that can perform the actual extraction.
+
+    Args:
+        rar_path: the path to the RAR file
+        outdir: the directory into which to extract the RAR contents. By
+            default, the directory containing the RAR file is used
+        delete_rar: whether to delete the RAR after extraction. By default,
+            this is False
+    """
+    outdir = outdir or os.path.dirname(rar_path) or "."
+
+    try:
+        with rarfile.RarFile(rar_path, "r") as f:
+            f.extractall(path=outdir)
+    except ValueError as e:
+        message = (
+            "Failed to extract RAR file '%s'. Extracting RAR files requires a "
+            "system package like `unrar` to be installed on your machine, "
+            "which you may need to install. Check the error message above for "
+            "more information."
+        ) % rar_path
+        six.raise_from(IOError(message), e)
+
+    if delete_rar:
+        delete_file(rar_path)
 
 
 def multiglob(*patterns, **kwargs):
     """Returns an iterable over the glob mathces for multiple patterns.
 
     Note that if a given file matches multiple patterns that you provided, it
     will appear multiple times in the output iterable.
@@ -4507,14 +4516,15 @@
             )
             return w, h
     except OSError as e:
         if e.errno in (
             getattr(errno, "ENOTTY", None),
             getattr(errno, "ENXIO", None),
             getattr(errno, "EBADF", None),
+            getattr(errno, "EOPNOTSUPP", None),
         ):
             return (80, 24)
 
         raise
 
 
 def save_window_snapshot(window_name, filepath):
@@ -4523,7 +4533,28 @@
 
     Args:
         window_name: the name of the window
         filepath: the path to write the snapshot image
     """
     ensure_basedir(filepath)
     _run_system_os_cmd(["import", "-window", window_name, filepath])
+
+
+def iter_batches(iterable, batch_size):
+    """Iterates over the given iterable in batches.
+
+    Args:
+        iterable: an iterable
+        batch_size: the desired batch size, or None to return the contents in
+            a single batch
+
+    Returns:
+        a generator that emits tuples of elements of the requested batch size
+        from the input
+    """
+    i = iter(iterable)
+    while True:
+        chunk = tuple(it.islice(i, batch_size))
+        if not chunk:
+            return
+
+        yield chunk
```

### Comparing `voxel51-eta-0.8.4rc1/eta/core/vgg16.py` & `voxel51-eta-0.9.0/eta/core/vgg16.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/video.py` & `voxel51-eta-0.9.0/eta/core/video.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/web.py` & `voxel51-eta-0.9.0/eta/core/web.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/core/ziputils.py` & `voxel51-eta-0.9.0/eta/core/ziputils.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/detectors/efficientdet.py` & `voxel51-eta-0.9.0/eta/detectors/efficientdet.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/detectors/tfmodels_detectors.py` & `voxel51-eta-0.9.0/eta/detectors/tfmodels_detectors.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/detectors/utils.py` & `voxel51-eta-0.9.0/eta/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/detectors/yolo.py` & `voxel51-eta-0.9.0/eta/detectors/yolo.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/README.md` & `voxel51-eta-0.9.0/eta/examples/README.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_cats/README.md` & `voxel51-eta-0.9.0/eta/examples/demo_cats/README.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_cats/detect-classify-cats.json` & `voxel51-eta-0.9.0/eta/examples/demo_cats/detect-classify-cats.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/README.md` & `voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/README.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_image.py` & `voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_image.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_image_direct.py` & `voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_image_direct.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_vgg16_module-config.json` & `voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_vgg16_module-config.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_embed_vgg16/embed_video.py` & `voxel51-eta-0.9.0/eta/examples/demo_embed_vgg16/embed_video.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_image_classifier/README.md` & `voxel51-eta-0.9.0/eta/examples/demo_image_classifier/README.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_image_classifier/classify-images-tfslim-template.json` & `voxel51-eta-0.9.0/eta/examples/demo_image_classifier/classify-images-tfslim-template.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_image_classifier/classify-images-vgg16.json` & `voxel51-eta-0.9.0/eta/examples/demo_image_classifier/classify-images-vgg16.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_instance_segmentation/README.md` & `voxel51-eta-0.9.0/eta/examples/demo_instance_segmentation/README.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_instance_segmentation/segment-people.json` & `voxel51-eta-0.9.0/eta/examples/demo_instance_segmentation/segment-people.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_instance_segmentation/segment-vehicles.json` & `voxel51-eta-0.9.0/eta/examples/demo_instance_segmentation/segment-vehicles.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_object_detector/README.md` & `voxel51-eta-0.9.0/eta/examples/demo_object_detector/README.md`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_object_detector/detect-people.json` & `voxel51-eta-0.9.0/eta/examples/demo_object_detector/detect-people.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_object_detector/detect-vehicles.json` & `voxel51-eta-0.9.0/eta/examples/demo_object_detector/detect-vehicles.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_semantic_segmentation/segment-frames.json` & `voxel51-eta-0.9.0/eta/examples/demo_semantic_segmentation/segment-frames.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/demo_video_pipeline/pipeline.json` & `voxel51-eta-0.9.0/eta/examples/demo_video_pipeline/pipeline.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/examples/download_data.py` & `voxel51-eta-0.9.0/eta/examples/download_data.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/models/manifest.json` & `voxel51-eta-0.9.0/eta/models/manifest.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_classifier_to_objects.json` & `voxel51-eta-0.9.0/eta/modules/apply_classifier_to_objects.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_classifier_to_objects.py` & `voxel51-eta-0.9.0/eta/modules/apply_classifier_to_objects.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_image_classifier.json` & `voxel51-eta-0.9.0/eta/modules/apply_image_classifier.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_image_classifier.py` & `voxel51-eta-0.9.0/eta/modules/apply_image_classifier.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_image_model.json` & `voxel51-eta-0.9.0/eta/modules/apply_image_model.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_image_model.py` & `voxel51-eta-0.9.0/eta/modules/apply_image_model.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_image_semantic_segmenter.json` & `voxel51-eta-0.9.0/eta/modules/apply_image_semantic_segmenter.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_image_semantic_segmenter.py` & `voxel51-eta-0.9.0/eta/modules/apply_image_semantic_segmenter.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_object_detector.json` & `voxel51-eta-0.9.0/eta/modules/apply_object_detector.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_object_detector.py` & `voxel51-eta-0.9.0/eta/modules/apply_object_detector.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_classifier.json` & `voxel51-eta-0.9.0/eta/modules/apply_video_classifier.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_classifier.py` & `voxel51-eta-0.9.0/eta/modules/apply_video_classifier.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_event_detector.json` & `voxel51-eta-0.9.0/eta/modules/apply_video_event_detector.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_event_detector.py` & `voxel51-eta-0.9.0/eta/modules/apply_video_event_detector.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_frames_classifier.json` & `voxel51-eta-0.9.0/eta/modules/apply_video_frames_classifier.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_frames_classifier.py` & `voxel51-eta-0.9.0/eta/modules/apply_video_frames_classifier.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_model.json` & `voxel51-eta-0.9.0/eta/modules/apply_video_model.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/apply_video_model.py` & `voxel51-eta-0.9.0/eta/modules/apply_video_model.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/clip_videos.json` & `voxel51-eta-0.9.0/eta/modules/clip_videos.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/clip_videos.py` & `voxel51-eta-0.9.0/eta/modules/clip_videos.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/embed_vgg16.json` & `voxel51-eta-0.9.0/eta/modules/embed_vgg16.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/embed_vgg16.py` & `voxel51-eta-0.9.0/eta/modules/embed_vgg16.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/format_videos.json` & `voxel51-eta-0.9.0/eta/modules/format_videos.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/format_videos.py` & `voxel51-eta-0.9.0/eta/modules/format_videos.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/sample_videos.json` & `voxel51-eta-0.9.0/eta/modules/sample_videos.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/sample_videos.py` & `voxel51-eta-0.9.0/eta/modules/sample_videos.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/video_stream_info.json` & `voxel51-eta-0.9.0/eta/modules/video_stream_info.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/video_stream_info.py` & `voxel51-eta-0.9.0/eta/modules/video_stream_info.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/visualize_image_labels.json` & `voxel51-eta-0.9.0/eta/modules/visualize_image_labels.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/visualize_image_labels.py` & `voxel51-eta-0.9.0/eta/modules/visualize_image_labels.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/visualize_labels.json` & `voxel51-eta-0.9.0/eta/modules/visualize_labels.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/modules/visualize_labels.py` & `voxel51-eta-0.9.0/eta/modules/visualize_labels.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/detect_and_classify_images.json` & `voxel51-eta-0.9.0/eta/pipelines/detect_and_classify_images.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/image_classifier.json` & `voxel51-eta-0.9.0/eta/pipelines/image_classifier.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/object_detector.json` & `voxel51-eta-0.9.0/eta/pipelines/object_detector.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/semantic_segmenter.json` & `voxel51-eta-0.9.0/eta/pipelines/semantic_segmenter.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/video_clipper.json` & `voxel51-eta-0.9.0/eta/pipelines/video_clipper.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/video_formatter.json` & `voxel51-eta-0.9.0/eta/pipelines/video_formatter.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/video_stream_info.json` & `voxel51-eta-0.9.0/eta/pipelines/video_stream_info.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/pipelines/visualize_labels.json` & `voxel51-eta-0.9.0/eta/pipelines/visualize_labels.json`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/imagenet-labels-no-background.txt` & `voxel51-eta-0.9.0/eta/resources/imagenet-labels-no-background.txt`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/imagenet-labels.txt` & `voxel51-eta-0.9.0/eta/resources/imagenet-labels.txt`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/lato-regular.ttf` & `voxel51-eta-0.9.0/eta/resources/lato-regular.ttf`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/ms-coco-labels.txt` & `voxel51-eta-0.9.0/eta/resources/ms-coco-labels.txt`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/tfslim-imagenet-labels-no-background.txt` & `voxel51-eta-0.9.0/eta/resources/tfslim-imagenet-labels-no-background.txt`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/tfslim-imagenet-labels.txt` & `voxel51-eta-0.9.0/eta/resources/tfslim-imagenet-labels.txt`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/vgg16-imagenet-labels.txt` & `voxel51-eta-0.9.0/eta/resources/vgg16-imagenet-labels.txt`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/voxel51-logo-600dpi.png` & `voxel51-eta-0.9.0/eta/resources/voxel51-logo-600dpi.png`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/resources/voxel51-logo.pdf` & `voxel51-eta-0.9.0/eta/resources/voxel51-logo.pdf`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/segmenters/tf_segmenters.py` & `voxel51-eta-0.9.0/eta/segmenters/tf_segmenters.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/tensorflow/install_automl.bash` & `voxel51-eta-0.9.0/eta/tensorflow/install_automl.bash`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/tensorflow/install_darkflow.bash` & `voxel51-eta-0.9.0/eta/tensorflow/install_darkflow.bash`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/eta/tensorflow/install_models.bash` & `voxel51-eta-0.9.0/eta/tensorflow/install_models.bash`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/install.bash` & `voxel51-eta-0.9.0/install.bash`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/pylintrc` & `voxel51-eta-0.9.0/pylintrc`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/requirements/common.txt` & `voxel51-eta-0.9.0/requirements/common.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 argcomplete==1.11.0
 contextlib2==0.5.5
 Cython>=0.28.5 # 0.29.28
 dill==0.2.7.1
 future==0.16.0
 glob2==0.6
 importlib-metadata==1.3.0; python_version<"3.8"
+jsonlines==3.1.0
 lxml==4.9.1
-ndjson==0.3.1
 numpy>=1.16.3
 opencv-python-headless<5,>=4.1.0.25
 packaging==19.2
-patool==1.12
 Pillow==9.3.0
+py7zr=0.20.4
 python-dateutil==2.7.0
 pytz==2019.3
+rarfile=4.0.0
 requests-toolbelt==0.8.0
 requests>=2.21.0
 retrying==1.3.3
 scikit-image>=0.16.2
 scipy>=0.19.1
 setuptools==44.0.0;python_version<"3"
 setuptools==45.2.0;python_version>="3"
```

### Comparing `voxel51-eta-0.8.4rc1/setup.py` & `voxel51-eta-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 from pkg_resources import DistributionNotFound, get_distribution
 import re
 from setuptools import setup, find_packages
 from wheel.bdist_wheel import bdist_wheel
 
 
-VERSION = "0.8.4"
+VERSION = "0.9.0"
 
 
 class BdistWheelCustom(bdist_wheel):
     def finalize_options(self):
         bdist_wheel.finalize_options(self)
         # Pure Python, so build a wheel for any Python version
         self.universal = True
@@ -24,21 +24,22 @@
 
 INSTALL_REQUIRES = [
     "argcomplete",
     "dill",
     "future",
     "glob2",
     "importlib-metadata; python_version<'3.8'",
-    "ndjson",
+    "jsonlines",
     "numpy",
     "packaging",
-    "patool",
     "Pillow>=6.2",
+    "py7zr",
     "python-dateutil",
     "pytz",
+    "rarfile",
     "requests",
     "retrying",
     "six",
     "scikit-image",
     "sortedcontainers",
     "tabulate",
     "tzlocal",
@@ -110,14 +111,16 @@
     include_package_data=True,
     install_requires=get_install_requirements(
         INSTALL_REQUIRES, CHOOSE_INSTALL_REQUIRES
     ),
     extras_require={
         "pipeline": ["blockdiag", "Sphinx", "sphinxcontrib-napoleon"],
         "storage": [
+            "azure-identity",
+            "azure-storage-blob>=12.4.0",
             "boto3>=1.15",
             "google-api-python-client",
             "google-cloud-storage>=1.36",
             "httplib2<=0.15",
             "pysftp",
         ],
     },
@@ -130,19 +133,18 @@
         "Topic :: Scientific/Engineering :: Image Processing",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Visualization",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     entry_points={"console_scripts": ["eta=eta.core.cli:main"]},
-    python_requires=">=2.7",
+    python_requires=">=3.6",
     cmdclass={"bdist_wheel": BdistWheelCustom},
 )
```

### Comparing `voxel51-eta-0.8.4rc1/sphinx/Makefile` & `voxel51-eta-0.9.0/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/sphinx/source/conf.py` & `voxel51-eta-0.9.0/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/PKG-INFO` & `voxel51-eta-0.9.0/voxel51_eta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxel51-eta
-Version: 0.8.4rc1
+Version: 0.9.0
 Summary: Extensible Toolkit for Analytics
 Home-page: https://github.com/voxel51/eta
 Author: Voxel51, Inc.
 Author-email: info@voxel51.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,22 +14,21 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pipeline
 Provides-Extra: storage
 License-File: LICENSE
 
 <div align="center">
 
@@ -51,15 +50,15 @@
 </div>
 
 ## Requirements
 
 ETA is very portable:
 
 -   Installable on Mac or Linux
--   Supports Python 2.7 and Python 3.6 or later
+-   Supports Python 3.6 or later
 -   Supports TensorFlow 1.X and 2.X
 -   Supports OpenCV 2.4+ and OpenCV 3.0+
 -   Supports CPU-only and GPU-enabled installations
 -   Supports CUDA 8, 9 and 10 for GPU installations
 
 ## Installation
```

### Comparing `voxel51-eta-0.8.4rc1/voxel51_eta.egg-info/SOURCES.txt` & `voxel51-eta-0.9.0/voxel51_eta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

