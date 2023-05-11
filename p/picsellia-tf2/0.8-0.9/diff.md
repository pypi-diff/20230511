# Comparing `tmp/picsellia_tf2-0.8.tar.gz` & `tmp/picsellia_tf2-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/picsellia_tf2-0.8.tar", last modified: Fri Nov 27 17:20:44 2020, max compression
+gzip compressed data, was "dist/picsellia_tf2-0.9.tar", last modified: Mon Nov 30 16:59:14 2020, max compression
```

## Comparing `picsellia_tf2-0.8.tar` & `picsellia_tf2-0.9.tar`

### file list

```diff
@@ -1,578 +1,578 @@
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/
--rw-rw-r--   0 pn        (1000) pn        (1000)       38 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/setup.cfg
--rw-rw-r--   0 pn        (1000) pn        (1000)     1332 2020-11-27 17:20:40.000000 picsellia_tf2-0.8/setup.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/slim/
--rw-rw-r--   0 pn        (1000) pn        (1000)     1407 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/export_inference_graph_test.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/
--rw-rw-r--   0 pn        (1000) pn        (1000)     9709 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/pix2pix.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7342 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/alexnet_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3378 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nets_factory_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7253 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nets_factory.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12015 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18020 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v1.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6151 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/alexnet.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11210 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/i3d_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    14544 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v3_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4629 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/cifarnet.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16519 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v4.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    14608 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/vgg.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10888 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/cyclegan.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    23312 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/s3dg.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/
--rw-rw-r--   0 pn        (1000) pn        (1000)    10541 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/pnasnet.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2508 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    20805 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11211 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/pnasnet_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    20453 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    19056 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    22516 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3079 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    27003 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6381 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/i3d.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5886 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/pix2pix_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16875 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v1.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6283 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/s3dg_test.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/
--rw-rw-r--   0 pn        (1000) pn        (1000)    68394 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5913 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18445 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18334 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/conv_blocks.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8994 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7902 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6189 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/i3d_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16902 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11826 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4283 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/dcgan_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13029 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v4_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    27159 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6926 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/post_training_quantization.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    20270 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7647 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1_train.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18455 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_resnet_v2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    28406 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v3.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    26623 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    23270 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/vgg_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4229 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/cyclegan_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3852 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/lenet.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4939 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1_eval.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7569 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/dcgan.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15499 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1676 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5965 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/overfeat.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7142 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/overfeat_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15185 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_resnet_v2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3125 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/download_and_convert_data.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/
--rw-rw-r--   0 pn        (1000) pn        (1000)    15551 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/inception_preprocessing.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3692 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/preprocessing_factory.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1804 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/lenet_preprocessing.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13583 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/vgg_preprocessing.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5330 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/cifarnet_preprocessing.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5939 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/export_inference_graph.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7062 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/eval_image_classifier.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    21229 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/train_image_classifier.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1009 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/setup.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/slim/deployment/
--rw-rw-r--   0 pn        (1000) pn        (1000)    24284 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/deployment/model_deploy_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/deployment/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    23855 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/deployment/model_deploy.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/
--rw-rw-r--   0 pn        (1000) pn        (1000)     7295 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/imagenet.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11608 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords_lib.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3251 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/flowers.py
--rwxrwxr-x   0 pn        (1000) pn        (1000)     3069 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/preprocess_imagenet_validation_data.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6539 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6335 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_cifar10.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1995 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/dataset_factory.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    26229 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/build_imagenet_data.py
--rwxrwxr-x   0 pn        (1000) pn        (1000)     8858 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/process_bounding_boxes.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7151 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/dataset_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4353 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/visualwakewords.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7399 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_mnist.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3246 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/cifar10.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3273 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/mnist.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7298 2020-11-24 16:30:49.000000 picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_flowers.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10046 2020-11-24 16:37:27.000000 picsellia_tf2-0.8/picsellia_tf2/pxl_tf.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/
--rw-rw-r--   0 pn        (1000) pn        (1000)     9871 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/trainer_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17685 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/trainer.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12937 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/evaluator.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5462 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/eval.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6874 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/train.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    58508 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4887 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_graph_tf2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10330 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_lib_v2.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/
--rw-rw-r--   0 pn        (1000) pn        (1000)     5516 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/detection_inference.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4266 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/infer_detections.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6521 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/detection_inference_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4514 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_main.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/
--rw-rw-r--   0 pn        (1000) pn        (1000)     7818 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    43004 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_tools.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4607 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_metrics.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10576 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_tools.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    97259 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_evaluation_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5874 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5871 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7800 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/tf_example_parser_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6259 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/tf_example_parser.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10266 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6489 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9253 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_evaluation_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4475 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_metrics_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5841 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12929 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5718 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17225 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_tools_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5684 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_tools_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    89948 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    21452 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1227 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/io_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7597 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_evaluation_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2241 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1796 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_hparams.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/
--rw-rw-r--   0 pn        (1000) pn        (1000)    13023 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/seq_example_util_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4850 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4043 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7318 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12116 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_pet_tf_record.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1819 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9606 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/seq_example_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13073 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8529 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7127 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16192 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3915 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1718 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    22961 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5208 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_oid_tf_record.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5134 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    22448 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_ava_actions_tf_record.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/
--rw-rw-r--   0 pn        (1000) pn        (1000)     8166 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15163 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13130 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10884 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    37517 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9914 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12408 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11636 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_main.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    22171 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5894 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_ssd_graph.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/
--rw-rw-r--   0 pn        (1000) pn        (1000)     7117 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_box_predictor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5742 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6065 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5825 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    42980 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2972 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    41945 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_box_predictor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18473 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_box_predictor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6338 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    21534 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3056 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_box_predictor_tf1_test.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/
--rw-rw-r--   0 pn        (1000) pn        (1000)     4617 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/box_head_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9295 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_mask_head_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6903 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/mask_head_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18650 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_mask_head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    14771 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_class_head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4595 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keypoint_head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11148 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/box_head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13680 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_box_head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7075 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/class_head_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12829 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/class_head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2645 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2298 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keypoint_head_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7624 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_class_head_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7322 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_box_head_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    14583 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/mask_head.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8449 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/
--rw-rw-r--   0 pn        (1000) pn        (1000)     2737 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/dataset_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    19491 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/colab_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7611 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    46544 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/config_util_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3848 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/model_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2295 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/static_shape.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    48048 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/object_detection_evaluation_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17950 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/shape_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4120 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2694 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/json_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    20918 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    26713 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/spatial_transform_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1208 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/context_manager_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    34228 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10087 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/target_assigner_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6814 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/variables_helper.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1987 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/category_util_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3598 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/json_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    49223 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12318 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/label_map_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10185 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/variables_helper_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    25710 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/spatial_transform_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10396 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    63931 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/visualization_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    35342 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_evaluation_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2518 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/category_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13898 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/label_map_util_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15587 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/bifpn_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1416 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/dataset_util_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5297 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    65476 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/autoaugment_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8156 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2541 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3328 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7233 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/metrics.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3627 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_mask_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    26028 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/vrd_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5789 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/learning_schedules_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6162 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/metrics_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    25764 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/visualization_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2604 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2009 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/static_shape_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)      996 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/tf_version.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4325 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_mask_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17006 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9561 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11183 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/vrd_evaluation_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2187 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/model_util_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18467 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/target_assigner_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3431 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9183 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/learning_schedules.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    58491 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/object_detection_evaluation.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4656 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    41652 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/config_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3448 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/patch_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5138 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/patch_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1277 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/context_manager.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11265 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_case.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    67048 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15305 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/shape_utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15693 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2776 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_case_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    51786 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/inputs.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/
--rw-rw-r--   0 pn        (1000) pn        (1000)     5082 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/grid_anchor_generator_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    20026 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/image_resizer_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    26725 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/hyperparams_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4176 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/target_assigner_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    35788 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/box_predictor_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    44445 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/center_net_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6257 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/fpn_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2184 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/mean_stddev_box_coder_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4359 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/argmax_matcher_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9582 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/region_similarity_calculator_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6848 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/anchor_generator_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17395 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/train_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    27275 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/ssd_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    42522 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/losses_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3882 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/matcher_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    24908 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/calibration_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2175 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/bipartite_matcher_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6105 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/flexible_grid_anchor_generator_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2944 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/square_box_coder_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)   131829 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/preprocessor_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6208 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/box_coder_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    30321 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/faster_rcnn_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    28451 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/optimizer_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3445 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/faster_rcnn_box_coder_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4438 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/multiscale_anchor_generator_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9652 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/string_int_label_map_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6430 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/pipeline_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11764 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/post_processing_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    26300 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/eval_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3810 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/keypoint_box_coder_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4720 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/graph_rewriter_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7278 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/ssd_anchor_generator_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    22716 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/input_reader_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6788 2020-11-24 19:15:25.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/model_pb2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    55565 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/eval_util.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    44660 2020-11-27 16:39:31.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib_v2.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/
--rw-rw-r--   0 pn        (1000) pn        (1000)     2315 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9156 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/faster_rcnn.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7757 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2034 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/utils_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2602 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9247 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/ssd.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/testdata/
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/testdata/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1795 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9635 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/export_inference_graph.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/
--rw-rw-r--   0 pn        (1000) pn        (1000)   161979 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    33283 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)   141413 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    87998 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    21716 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5387 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17843 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    23101 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5081 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8672 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2299 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9287 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    19471 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9337 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test_lib.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    93899 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test_lib.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    61007 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    20418 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    47073 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    73772 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/inputs_test.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/
--rw-rw-r--   0 pn        (1000) pn        (1000)     5971 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13817 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    60908 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_example_decoder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    39694 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_example_decoder.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/
--rw-rw-r--   0 pn        (1000) pn        (1000)    12854 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9212 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6584 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12582 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6757 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12490 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16669 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4519 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8179 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4776 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_main_tf2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12721 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_lib_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10070 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7217 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_main_v2.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/
--rw-rw-r--   0 pn        (1000) pn        (1000)     6414 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/keypoint_box_coder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6799 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/keypoint_box_coder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5104 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/square_box_coder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2498 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5071 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2592 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3847 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4286 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/square_box_coder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    27629 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/
--rw-rw-r--   0 pn        (1000) pn        (1000)    48427 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7725 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/image_resizer_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    26445 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_predictor_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    46984 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_predictor_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3343 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/optimizer_builder_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    18122 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/losses_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8728 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/image_resizer_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1715 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/target_assigner_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2667 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10348 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/calibration_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2948 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/graph_rewriter_builder_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16781 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/hyperparams_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    33333 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/hyperparams_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3155 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/decoder_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7418 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/optimizer_builder_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8384 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/decoder_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10982 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5410 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/anchor_generator_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    25788 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/dataset_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4144 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/matcher_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13047 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    14320 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/anchor_generator_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7499 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/optimizer_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3843 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/input_reader_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2888 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_coder_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17764 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/preprocessor_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7791 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/post_processing_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2436 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/matcher_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2368 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9485 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/losses_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    28234 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/preprocessor_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2383 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1763 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/target_assigner_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8140 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/post_processing_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2019 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/graph_rewriter_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10599 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/dataset_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12269 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/input_reader_builder_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10328 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/calibration_builder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5168 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_coder_builder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    20157 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/eval_util_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5589 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/model_tpu_main.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/
--rw-rw-r--   0 pn        (1000) pn        (1000)    12399 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/keypoint_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16315 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/densepose_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6859 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    24204 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/model.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6512 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/anchor_generator.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10193 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_predictor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15569 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/keypoint_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    34921 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/losses.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2744 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/model_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5420 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/region_similarity_calculator_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    22866 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/multiclass_nms_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8989 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/matcher_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4622 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/prefetcher_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7732 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/freezable_batch_norm_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    48598 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6616 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/class_agnostic_nms_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6645 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/region_similarity_calculator.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6109 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/batcher_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1645 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/data_parser.py
--rw-rw-r--   0 pn        (1000) pn        (1000)   175171 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/preprocessor_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1472 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/data_decoder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4409 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/preprocessor_cache.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    59011 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/post_processing.py
--rw-rw-r--   0 pn        (1000) pn        (1000)   105843 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/target_assigner.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6942 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/densepose_ops_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2845 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/minibatch_sampler_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    66425 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/losses_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2166 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_coder_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11632 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3231 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/minibatch_sampler.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2536 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/prefetcher.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2992 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/freezable_batch_norm.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9959 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/matcher.py
--rw-rw-r--   0 pn        (1000) pn        (1000)   108295 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/target_assigner_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5765 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/batcher.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    32678 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/batch_multiclass_nms_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5144 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_coder.py
--rw-rw-r--   0 pn        (1000) pn        (1000)   194107 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/preprocessor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4812 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    46338 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list_ops.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8871 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    15637 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/core/standard_fields.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11170 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    14113 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/
--rw-rw-r--   0 pn        (1000) pn        (1000)     4286 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/bipartite_matcher_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2834 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/bipartite_matcher.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9524 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/argmax_matcher.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4391 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/hungarian_matcher_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10744 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/argmax_matcher_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2258 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/hungarian_matcher.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/
--rw-rw-r--   0 pn        (1000) pn        (1000)    20777 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5606 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10626 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8350 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7657 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12578 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5411 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2565 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7200 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3424 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_testbase.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4375 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2124 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1801 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11223 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7390 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4718 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4210 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9440 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8934 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5645 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5420 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7748 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8728 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    44824 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1713 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7991 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4652 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6055 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6657 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6664 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17933 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4543 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_testbase.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9437 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf2_test.py
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/
--rw-rw-r--   0 pn        (1000) pn        (1000)    21027 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/resnet_v1.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    21032 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/hourglass_network.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2964 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/convert_keras_models.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    14960 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9282 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13461 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    11541 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/test_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9725 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8515 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10309 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5882 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/hourglass_network_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1913 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/model_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8565 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/resnet_v1_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5086 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9286 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7009 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    17007 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5420 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3528 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4560 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_testbase.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10357 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     2048 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    21529 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5786 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8456 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7566 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_testbase.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4510 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7130 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3983 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    10784 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    36345 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/feature_map_generators.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13116 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9609 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8651 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5186 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8347 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    22520 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3732 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6316 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1968 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    16337 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7955 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     7894 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8786 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    12438 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     5585 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     1735 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     9695 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_feature_extractor_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3411 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3327 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    13420 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf1_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6871 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_keras_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     6749 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3293 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    35575 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/feature_map_generators_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3025 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     4117 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     3698 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)     8796 2020-11-23 12:49:32.000000 picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf2_test.py
--rw-rw-r--   0 pn        (1000) pn        (1000)      402 2020-11-24 17:39:22.000000 picsellia_tf2-0.8/picsellia_tf2/__init__.py
--rw-rw-r--   0 pn        (1000) pn        (1000)    30009 2020-11-27 17:20:31.000000 picsellia_tf2-0.8/picsellia_tf2/pxl_utils.py
--rw-rw-r--   0 pn        (1000) pn        (1000)      197 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/PKG-INFO
-drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2.egg-info/
--rw-rw-r--   0 pn        (1000) pn        (1000)    34303 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2.egg-info/SOURCES.txt
--rw-rw-r--   0 pn        (1000) pn        (1000)       14 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2.egg-info/top_level.txt
--rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2.egg-info/dependency_links.txt
--rw-rw-r--   0 pn        (1000) pn        (1000)      154 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2.egg-info/requires.txt
--rw-rw-r--   0 pn        (1000) pn        (1000)      197 2020-11-27 17:20:44.000000 picsellia_tf2-0.8/picsellia_tf2.egg-info/PKG-INFO
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/
+-rw-rw-r--   0 pn        (1000) pn        (1000)       38 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/setup.cfg
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1332 2020-11-30 16:59:09.000000 picsellia_tf2-0.9/setup.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:13.000000 picsellia_tf2-0.9/picsellia_tf2/
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/slim/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1407 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/export_inference_graph_test.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9709 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/pix2pix.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7342 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/alexnet_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3378 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nets_factory_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7253 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nets_factory.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12015 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18020 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v1.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6151 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/alexnet.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11210 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/i3d_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    14544 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v3_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4629 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/cifarnet.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16519 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v4.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    14608 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/vgg.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10888 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/cyclegan.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    23312 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/s3dg.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10541 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/pnasnet.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2508 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20805 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11211 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/pnasnet_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20453 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    19056 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    22516 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3079 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    27003 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6381 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/i3d.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5886 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/pix2pix_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16875 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v1.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6283 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/s3dg_test.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    68394 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5913 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18445 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18334 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/conv_blocks.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8994 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7902 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6189 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/i3d_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16902 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11826 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4283 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/dcgan_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13029 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v4_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    27159 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6926 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/post_training_quantization.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20270 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7647 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1_train.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18455 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_resnet_v2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    28406 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v3.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    26623 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    23270 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/vgg_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4229 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/cyclegan_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3852 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/lenet.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4939 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1_eval.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7569 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/dcgan.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15499 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1676 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5965 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/overfeat.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7142 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/overfeat_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15185 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_resnet_v2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3125 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/download_and_convert_data.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15551 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/inception_preprocessing.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3692 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/preprocessing_factory.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1804 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/lenet_preprocessing.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13583 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/vgg_preprocessing.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5330 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/cifarnet_preprocessing.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5939 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/export_inference_graph.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7062 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/eval_image_classifier.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    21229 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/train_image_classifier.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1009 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/setup.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/slim/deployment/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    24284 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/deployment/model_deploy_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/deployment/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    23855 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/deployment/model_deploy.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7295 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/imagenet.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11608 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords_lib.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3251 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/flowers.py
+-rwxrwxr-x   0 pn        (1000) pn        (1000)     3069 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/preprocess_imagenet_validation_data.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6539 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6335 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_cifar10.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1995 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/dataset_factory.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    26229 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/build_imagenet_data.py
+-rwxrwxr-x   0 pn        (1000) pn        (1000)     8858 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/process_bounding_boxes.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7151 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/dataset_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4353 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/visualwakewords.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7399 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_mnist.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3246 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/cifar10.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3273 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/mnist.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7298 2020-11-24 16:30:49.000000 picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_flowers.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10046 2020-11-24 16:37:27.000000 picsellia_tf2-0.9/picsellia_tf2/pxl_tf.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9871 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/trainer_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17685 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/trainer.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12937 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/evaluator.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5462 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/eval.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6874 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/train.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    58508 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4887 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_graph_tf2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10330 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_lib_v2.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5516 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/detection_inference.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4266 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/infer_detections.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6521 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/detection_inference_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4514 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_main.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7818 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    43004 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_tools.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4607 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_metrics.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10576 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_tools.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    97259 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_evaluation_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5874 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5871 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7800 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/tf_example_parser_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6259 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/tf_example_parser.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10266 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6489 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9253 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_evaluation_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4475 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_metrics_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5841 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12929 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5718 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17225 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_tools_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5684 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_tools_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    89948 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    21452 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1227 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/io_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7597 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_evaluation_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2241 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1796 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_hparams.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13023 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/seq_example_util_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4850 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4043 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7318 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12116 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_pet_tf_record.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1819 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9606 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/seq_example_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13073 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8529 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7127 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16192 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3915 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1718 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    22961 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5208 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_oid_tf_record.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5134 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    22448 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_ava_actions_tf_record.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8166 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15163 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13130 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10884 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    37517 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9914 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12408 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11636 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_main.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    22171 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5894 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_ssd_graph.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7117 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_box_predictor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5742 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6065 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5825 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    42980 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2972 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    41945 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_box_predictor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18473 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_box_predictor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6338 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    21534 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3056 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_box_predictor_tf1_test.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4617 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/box_head_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9295 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_mask_head_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6903 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/mask_head_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18650 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_mask_head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    14771 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_class_head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4595 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keypoint_head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11148 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/box_head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13680 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_box_head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7075 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/class_head_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12829 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/class_head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2645 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2298 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keypoint_head_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7624 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_class_head_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7322 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_box_head_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    14583 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/mask_head.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8449 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2737 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/dataset_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    19491 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/colab_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7611 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    46544 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/config_util_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3848 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/model_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2295 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/static_shape.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    48048 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/object_detection_evaluation_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17950 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/shape_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4120 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2694 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/json_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20918 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    26713 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/spatial_transform_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1208 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/context_manager_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    34228 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10087 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/target_assigner_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6814 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/variables_helper.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1987 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/category_util_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3598 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/json_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    49223 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12318 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/label_map_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10185 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/variables_helper_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    25710 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/spatial_transform_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10396 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    63931 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/visualization_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    35342 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_evaluation_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2518 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/category_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13898 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/label_map_util_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15587 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/bifpn_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1416 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/dataset_util_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5297 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    65476 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/autoaugment_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8156 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2541 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3328 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7233 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/metrics.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3627 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_mask_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    26028 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/vrd_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5789 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/learning_schedules_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6162 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/metrics_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    25764 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/visualization_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2604 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2009 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/static_shape_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)      996 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/tf_version.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4325 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_mask_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17006 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9561 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11183 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/vrd_evaluation_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2187 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/model_util_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18467 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/target_assigner_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3431 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9183 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/learning_schedules.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    58491 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/object_detection_evaluation.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4656 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    41652 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/config_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3448 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/patch_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5138 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/patch_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1277 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/context_manager.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11265 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_case.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    67048 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15305 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/shape_utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15693 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2776 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_case_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    51786 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/inputs.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5082 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/grid_anchor_generator_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20026 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/image_resizer_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    26725 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/hyperparams_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4176 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/target_assigner_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    35788 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/box_predictor_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    44445 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/center_net_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6257 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/fpn_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2184 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/mean_stddev_box_coder_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4359 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/argmax_matcher_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9582 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/region_similarity_calculator_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6848 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/anchor_generator_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17395 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/train_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    27275 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/ssd_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    42522 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/losses_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3882 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/matcher_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    24908 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/calibration_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2175 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/bipartite_matcher_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6105 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/flexible_grid_anchor_generator_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2944 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/square_box_coder_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)   131829 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/preprocessor_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6208 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/box_coder_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    30321 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/faster_rcnn_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    28451 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/optimizer_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3445 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/faster_rcnn_box_coder_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4438 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/multiscale_anchor_generator_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9652 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/string_int_label_map_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6430 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/pipeline_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11764 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/post_processing_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    26300 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/eval_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3810 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/keypoint_box_coder_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4720 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/graph_rewriter_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7278 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/ssd_anchor_generator_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    22716 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/input_reader_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6788 2020-11-24 19:15:25.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/model_pb2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    55565 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/eval_util.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    44660 2020-11-27 16:39:31.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib_v2.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2315 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9156 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/faster_rcnn.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7757 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2034 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/utils_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2602 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9247 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/ssd.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/testdata/
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/testdata/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1795 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9635 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/export_inference_graph.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/
+-rw-rw-r--   0 pn        (1000) pn        (1000)   161979 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    33283 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)   141413 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    87998 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    21716 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5387 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17843 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    23101 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5081 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8672 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2299 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9287 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    19471 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9337 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test_lib.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    93899 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test_lib.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    61007 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20418 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    47073 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    73772 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/inputs_test.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5971 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13817 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    60908 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_example_decoder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    39694 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_example_decoder.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12854 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9212 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6584 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12582 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6757 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12490 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16669 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4519 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8179 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4776 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_main_tf2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12721 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_lib_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10070 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7217 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_main_v2.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6414 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/keypoint_box_coder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6799 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/keypoint_box_coder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5104 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/square_box_coder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2498 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5071 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2592 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3847 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4286 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/square_box_coder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    27629 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    48427 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7725 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/image_resizer_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    26445 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_predictor_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    46984 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_predictor_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3343 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/optimizer_builder_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    18122 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/losses_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8728 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/image_resizer_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1715 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/target_assigner_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2667 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10348 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/calibration_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2948 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/graph_rewriter_builder_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16781 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/hyperparams_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    33333 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/hyperparams_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3155 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/decoder_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7418 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/optimizer_builder_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8384 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/decoder_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10982 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5410 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/anchor_generator_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    25788 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/dataset_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4144 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/matcher_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13047 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    14320 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/anchor_generator_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7499 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/optimizer_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3843 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/input_reader_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2888 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_coder_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17764 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/preprocessor_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7791 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/post_processing_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2436 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/matcher_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2368 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9485 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/losses_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    28234 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/preprocessor_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2383 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1763 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/target_assigner_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8140 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/post_processing_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2019 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/graph_rewriter_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10599 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/dataset_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12269 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/input_reader_builder_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10328 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/calibration_builder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5168 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_coder_builder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20157 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/eval_util_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5589 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/model_tpu_main.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12399 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/keypoint_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16315 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/densepose_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6859 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    24204 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/model.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6512 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/anchor_generator.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10193 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_predictor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15569 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/keypoint_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    34921 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/losses.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2744 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/model_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5420 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/region_similarity_calculator_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    22866 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/multiclass_nms_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8989 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/matcher_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4622 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/prefetcher_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7732 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/freezable_batch_norm_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    48598 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6616 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/class_agnostic_nms_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6645 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/region_similarity_calculator.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6109 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/batcher_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1645 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/data_parser.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)   175171 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/preprocessor_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1472 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/data_decoder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4409 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/preprocessor_cache.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    59011 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/post_processing.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)   105843 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/target_assigner.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6942 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/densepose_ops_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2845 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/minibatch_sampler_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    66425 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/losses_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2166 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_coder_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11632 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3231 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/minibatch_sampler.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2536 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/prefetcher.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2992 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/freezable_batch_norm.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9959 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/matcher.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)   108295 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/target_assigner_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5765 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/batcher.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    32678 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/batch_multiclass_nms_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5144 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_coder.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)   194107 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/preprocessor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4812 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    46338 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list_ops.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8871 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    15637 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/core/standard_fields.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11170 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    14113 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4286 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/bipartite_matcher_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2834 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/bipartite_matcher.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9524 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/argmax_matcher.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4391 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/hungarian_matcher_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10744 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/argmax_matcher_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2258 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/hungarian_matcher.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    20777 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5606 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10626 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8350 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7657 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12578 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5411 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2565 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7200 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3424 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_testbase.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4375 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2124 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1801 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11223 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7390 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4718 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4210 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9440 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8934 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5645 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5420 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7748 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8728 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    44824 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1713 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7991 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4652 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6055 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6657 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6664 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17933 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4543 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_testbase.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9437 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf2_test.py
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    21027 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/resnet_v1.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    21032 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/hourglass_network.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2964 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/convert_keras_models.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    14960 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9282 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13461 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    11541 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/test_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9725 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8515 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10309 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5882 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/hourglass_network_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1913 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/model_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8565 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/resnet_v1_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5086 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9286 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7009 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    17007 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5420 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3528 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4560 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_testbase.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10357 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     2048 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    21529 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5786 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8456 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7566 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_testbase.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4510 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7130 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3983 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    10784 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    36345 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/feature_map_generators.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13116 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9609 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8651 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)        0 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5186 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8347 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    22520 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3732 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6316 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1968 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    16337 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7955 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     7894 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8786 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    12438 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     5585 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     1735 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     9695 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_feature_extractor_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3411 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3327 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    13420 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf1_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6871 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_keras_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     6749 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3293 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    35575 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/feature_map_generators_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3025 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     4117 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     3698 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)     8796 2020-11-23 12:49:32.000000 picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf2_test.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)      402 2020-11-24 17:39:22.000000 picsellia_tf2-0.9/picsellia_tf2/__init__.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)    29728 2020-11-30 16:58:35.000000 picsellia_tf2-0.9/picsellia_tf2/pxl_utils.py
+-rw-rw-r--   0 pn        (1000) pn        (1000)      197 2020-11-30 16:59:14.000000 picsellia_tf2-0.9/PKG-INFO
+drwxrwxr-x   0 pn        (1000) pn        (1000)        0 2020-11-30 16:59:13.000000 picsellia_tf2-0.9/picsellia_tf2.egg-info/
+-rw-rw-r--   0 pn        (1000) pn        (1000)    34303 2020-11-30 16:59:13.000000 picsellia_tf2-0.9/picsellia_tf2.egg-info/SOURCES.txt
+-rw-rw-r--   0 pn        (1000) pn        (1000)       14 2020-11-30 16:59:13.000000 picsellia_tf2-0.9/picsellia_tf2.egg-info/top_level.txt
+-rw-rw-r--   0 pn        (1000) pn        (1000)        1 2020-11-30 16:59:13.000000 picsellia_tf2-0.9/picsellia_tf2.egg-info/dependency_links.txt
+-rw-rw-r--   0 pn        (1000) pn        (1000)      154 2020-11-30 16:59:13.000000 picsellia_tf2-0.9/picsellia_tf2.egg-info/requires.txt
+-rw-rw-r--   0 pn        (1000) pn        (1000)      197 2020-11-30 16:59:13.000000 picsellia_tf2-0.9/picsellia_tf2.egg-info/PKG-INFO
```

### Comparing `picsellia_tf2-0.8/setup.py` & `picsellia_tf2-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'scipy',
     'pandas',
     'tf-models-official'
 ]
 
 setup(
     name='picsellia_tf2',
-    version='0.8',
+    version='0.9',
     install_requires=REQUIRED_PACKAGES,
     include_package_data=True,
     packages=(
         [p for p in find_packages(where='.')]),
         # [p for p in find_packages() if p.startswith('object_detection')] +
         # find_packages(where=os.path.join('.', 'slim'))),
     package_dir={
```

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/export_inference_graph_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/export_inference_graph_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/pix2pix.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/pix2pix.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/alexnet_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/alexnet_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nets_factory_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nets_factory_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nets_factory.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nets_factory.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v1.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v1.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/alexnet.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/alexnet.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/i3d_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/i3d_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v3_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v3_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/cifarnet.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/cifarnet.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v4.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v4.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/vgg.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/vgg.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/cyclegan.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/cyclegan.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/s3dg.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/s3dg.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/pnasnet.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/pnasnet.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/pnasnet_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/pnasnet_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/nasnet/nasnet_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/nasnet/nasnet_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/i3d.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/i3d.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/pix2pix_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/pix2pix_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v1.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v1.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/s3dg_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/s3dg_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v3_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/conv_blocks.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet/mobilenet_v2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/i3d_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/i3d_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/dcgan_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/dcgan_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v4_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v4_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/post_training_quantization.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/post_training_quantization.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1_train.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1_train.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_resnet_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v3.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v3.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/vgg_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/vgg_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/cyclegan_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/cyclegan_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/lenet.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/lenet.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/mobilenet_v1_eval.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/mobilenet_v1_eval.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/dcgan.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/dcgan.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/resnet_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/overfeat.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/overfeat.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/overfeat_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/overfeat_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/nets/inception_resnet_v2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/nets/inception_resnet_v2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/download_and_convert_data.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/download_and_convert_data.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/inception_preprocessing.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/inception_preprocessing.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/preprocessing_factory.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/preprocessing_factory.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/lenet_preprocessing.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/lenet_preprocessing.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/vgg_preprocessing.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/vgg_preprocessing.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/preprocessing/cifarnet_preprocessing.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/preprocessing/cifarnet_preprocessing.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/export_inference_graph.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/export_inference_graph.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/eval_image_classifier.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/eval_image_classifier.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/train_image_classifier.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/train_image_classifier.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/setup.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/setup.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/deployment/model_deploy_test.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/deployment/model_deploy_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/deployment/model_deploy.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/deployment/model_deploy.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/imagenet.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords_lib.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords_lib.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/flowers.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/flowers.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/preprocess_imagenet_validation_data.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/preprocess_imagenet_validation_data.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_visualwakewords.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_cifar10.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_cifar10.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/dataset_factory.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/build_imagenet_data.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/build_imagenet_data.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/process_bounding_boxes.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/process_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/dataset_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/visualwakewords.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/visualwakewords.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_mnist.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_mnist.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/cifar10.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/mnist.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/slim/datasets/download_and_convert_flowers.py` & `picsellia_tf2-0.9/picsellia_tf2/slim/datasets/download_and_convert_flowers.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/pxl_tf.py` & `picsellia_tf2-0.9/picsellia_tf2/pxl_tf.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/trainer_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/trainer_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/trainer.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/trainer.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/evaluator.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/evaluator.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/eval.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/eval.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/legacy/train.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/legacy/train.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_graph_tf2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_graph_tf2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_lib_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_lib_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/detection_inference.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/detection_inference.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/infer_detections.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/infer_detections.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/inference/detection_inference_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/inference/detection_inference_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_main.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_main.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_tools.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_tools.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_metrics.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_metrics.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_tools.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_tools.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_evaluation_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/tf_example_parser_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/tf_example_parser_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/tf_example_parser.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/tf_example_parser.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_evaluation_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_evaluation_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/calibration_metrics_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/calibration_metrics_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_challenge_evaluation_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/oid_vrd_challenge_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_tools_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_tools_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_tools_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_tools_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/coco_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/io_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/io_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/lvis_evaluation_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/lvis_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/metrics/offline_eval_map_corloc_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_hparams.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_hparams.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/seq_example_util_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/seq_example_util_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_pet_tf_record.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_pet_tf_record.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/seq_example_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/seq_example_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_kitti_tf_record.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_pascal_tf_record.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_hierarchical_labels_expansion_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/tf_record_creation_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_coco_tf_record.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_oid_tf_record.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_oid_tf_record.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/oid_tfrecord_creation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/create_ava_actions_tf_record.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/create_ava_actions_tf_record.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/add_context_to_examples.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_detection_data_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/generate_embedding_data.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_main.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/dataset_tools/context_rcnn/create_cococameratraps_tfexample_main.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_ssd_graph.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_ssd_graph.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_box_predictor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_box_predictor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_keras_box_predictor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_box_predictor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_box_predictor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_box_predictor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_box_predictor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/mask_rcnn_box_predictor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/convolutional_keras_box_predictor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_box_predictor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_box_predictor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/box_head_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/box_head_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_mask_head_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_mask_head_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/mask_head_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/mask_head_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_mask_head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_mask_head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_class_head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_class_head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keypoint_head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/box_head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/box_head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_box_head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_box_head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/class_head_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/class_head_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/class_head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/class_head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keypoint_head_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keypoint_head_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_class_head_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_class_head_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/keras_box_head_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/keras_box_head_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/heads/mask_head.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/predictors/rfcn_keras_box_predictor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/dataset_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/dataset_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/colab_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/colab_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/config_util_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/config_util_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/model_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/model_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/static_shape.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/static_shape.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/object_detection_evaluation_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/object_detection_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/shape_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/shape_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/json_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/spatial_transform_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/spatial_transform_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/context_manager_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/context_manager_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/target_assigner_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/target_assigner_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/variables_helper.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/variables_helper.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/category_util_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/category_util_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/json_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/label_map_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/label_map_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/variables_helper_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/variables_helper_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/spatial_transform_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/spatial_transform_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_vrd_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/visualization_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/per_image_evaluation_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/per_image_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/category_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/category_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/label_map_util_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/label_map_util_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/bifpn_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/bifpn_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/dataset_util_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/dataset_util_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/autoaugment_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/autoaugment_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/metrics.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_mask_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_mask_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/vrd_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/vrd_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/learning_schedules_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/learning_schedules_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/metrics_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/metrics_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/visualization_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/visualization_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/static_shape_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/static_shape_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/tf_version.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/tf_version.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_mask_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_mask_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/vrd_evaluation_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/vrd_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/model_util_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/model_util_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/target_assigner_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/target_assigner_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/learning_schedules.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/learning_schedules.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/object_detection_evaluation.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/object_detection_evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_list.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_list.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/config_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/patch_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/patch_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/patch_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/patch_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/context_manager.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/context_manager.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_case.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_case.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/shape_utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/shape_utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/np_box_mask_list_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/np_box_mask_list_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/utils/test_case_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/utils/test_case_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/inputs.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/inputs.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/grid_anchor_generator_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/grid_anchor_generator_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/image_resizer_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/image_resizer_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/hyperparams_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/hyperparams_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/target_assigner_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/target_assigner_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/box_predictor_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/box_predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/center_net_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/center_net_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/fpn_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/fpn_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/mean_stddev_box_coder_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/mean_stddev_box_coder_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/argmax_matcher_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/argmax_matcher_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/region_similarity_calculator_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/region_similarity_calculator_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/anchor_generator_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/anchor_generator_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/train_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/train_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/ssd_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/ssd_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/losses_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/losses_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/matcher_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/matcher_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/calibration_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/calibration_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/bipartite_matcher_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/bipartite_matcher_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/flexible_grid_anchor_generator_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/flexible_grid_anchor_generator_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/square_box_coder_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/square_box_coder_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/preprocessor_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/preprocessor_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/box_coder_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/box_coder_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/faster_rcnn_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/faster_rcnn_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/optimizer_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/optimizer_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/faster_rcnn_box_coder_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/faster_rcnn_box_coder_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/multiscale_anchor_generator_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/multiscale_anchor_generator_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/string_int_label_map_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/string_int_label_map_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/pipeline_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/post_processing_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/post_processing_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/eval_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/eval_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/keypoint_box_coder_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/keypoint_box_coder_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/graph_rewriter_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/graph_rewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/ssd_anchor_generator_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/ssd_anchor_generator_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/input_reader_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/input_reader_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/protos/model_pb2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/protos/model_pb2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/eval_util.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/eval_util.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/faster_rcnn.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/utils_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/utils_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/export_saved_model_tpu_lib_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/ssd.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/ssd.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/tpu_exporters/utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/tpu_exporters/utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/export_inference_graph.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/export_inference_graph.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/center_net_meta_arch_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_meta_arch.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/context_rcnn_lib_tf2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/rfcn_meta_arch.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test_lib.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch_test_lib.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test_lib.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/faster_rcnn_meta_arch_test_lib.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/meta_architectures/ssd_meta_arch.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/inputs_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/inputs_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_sequence_example_decoder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_example_decoder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_example_decoder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/data_decoders/tf_example_decoder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/data_decoders/tf_example_decoder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/flexible_grid_anchor_generator_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiscale_grid_anchor_generator_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/multiple_grid_anchor_generator.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/anchor_generators/grid_anchor_generator_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_lib_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_lib_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_main_tf2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_main_tf2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_lib_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_lib_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter_main_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter_main_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/keypoint_box_coder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/keypoint_box_coder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/keypoint_box_coder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/keypoint_box_coder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/square_box_coder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/square_box_coder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/mean_stddev_box_coder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/faster_rcnn_box_coder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/box_coders/square_box_coder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/box_coders/square_box_coder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/exporter.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/exporter.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/image_resizer_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/image_resizer_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_predictor_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_predictor_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_predictor_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_predictor_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/optimizer_builder_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/optimizer_builder_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/losses_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/losses_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/image_resizer_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/image_resizer_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/target_assigner_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/target_assigner_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/calibration_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/calibration_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/graph_rewriter_builder_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/graph_rewriter_builder_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/hyperparams_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/hyperparams_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/hyperparams_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/hyperparams_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/decoder_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/decoder_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/optimizer_builder_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/optimizer_builder_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/decoder_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/decoder_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/anchor_generator_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/anchor_generator_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/dataset_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/dataset_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/matcher_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/matcher_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/anchor_generator_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/anchor_generator_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/optimizer_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/optimizer_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/input_reader_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/input_reader_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_coder_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_coder_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/preprocessor_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/preprocessor_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/post_processing_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/post_processing_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/matcher_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/matcher_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/model_builder_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/model_builder_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/losses_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/losses_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/preprocessor_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/preprocessor_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/region_similarity_calculator_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/target_assigner_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/target_assigner_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/post_processing_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/post_processing_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/graph_rewriter_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/graph_rewriter_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/dataset_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/input_reader_builder_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/input_reader_builder_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/calibration_builder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/calibration_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/builders/box_coder_builder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/builders/box_coder_builder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/eval_util_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/eval_util_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/model_tpu_main.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/model_tpu_main.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/keypoint_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/keypoint_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/densepose_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/densepose_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/model.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/model.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/anchor_generator.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_predictor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_predictor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/keypoint_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/keypoint_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/losses.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/losses.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/model_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/model_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/region_similarity_calculator_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/region_similarity_calculator_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/multiclass_nms_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/multiclass_nms_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/matcher_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/matcher_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/prefetcher_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/prefetcher_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/freezable_batch_norm_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/freezable_batch_norm_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/class_agnostic_nms_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/class_agnostic_nms_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/region_similarity_calculator.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/region_similarity_calculator.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/batcher_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/batcher_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/data_parser.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/data_parser.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/preprocessor_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/preprocessor_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/data_decoder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/data_decoder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/preprocessor_cache.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/preprocessor_cache.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/post_processing.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/post_processing.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/target_assigner.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/target_assigner.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/densepose_ops_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/densepose_ops_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/minibatch_sampler_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/minibatch_sampler_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/losses_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/losses_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_coder_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_coder_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/minibatch_sampler.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/minibatch_sampler.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/prefetcher.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/prefetcher.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/freezable_batch_norm.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/freezable_batch_norm.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/matcher.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/matcher.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/target_assigner_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/target_assigner_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/batcher.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/batcher.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/batch_multiclass_nms_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/batch_multiclass_nms_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_coder.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_coder.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/preprocessor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/preprocessor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/box_list_ops.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/box_list_ops.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/balanced_positive_negative_sampler_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/core/standard_fields.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/core/standard_fields.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_graph_lib_tf2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/export_tflite_ssd_graph_lib.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/bipartite_matcher_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/bipartite_matcher_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/bipartite_matcher.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/bipartite_matcher.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/argmax_matcher.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/argmax_matcher.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/hungarian_matcher_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/hungarian_matcher_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/argmax_matcher_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/argmax_matcher_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/matchers/hungarian_matcher.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/matchers/hungarian_matcher.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_testbase.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_testbase.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_v2_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_fpn_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_efficientnet_bifpn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v2_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_testbase.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_testbase.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/resnet_v1.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/resnet_v1.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/hourglass_network.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/hourglass_network.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/convert_keras_models.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/convert_keras_models.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v1_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/test_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/test_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/mobilenet_v2_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/hourglass_network_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/hourglass_network_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/model_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/model_utils.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/keras_models/resnet_v1_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/keras_models/resnet_v1_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_pnas_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_testbase.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor_testbase.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_edgetpu_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/bidirectional_feature_pyramid_generators.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_testbase.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_testbase.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_pnasnet_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/feature_map_generators.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/feature_map_generators.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_nas_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v3_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobiledet_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_inception_resnet_v2_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_resnet_v1_fpn_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_mnasfpn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_mobilenet_v1_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_inception_v3_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_mobilenet_v2_fpn_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_feature_extractor_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_feature_extractor_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_fpn_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_resnet_v1_ppn_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf1_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v2_fpn_feature_extractor_tf1_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_keras_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_keras_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/embedded_ssd_mobilenet_v1_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_ppn_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/feature_map_generators_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/feature_map_generators_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/center_net_hourglass_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_v1_fpn_keras_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/faster_rcnn_resnet_keras_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf2_test.py` & `picsellia_tf2-0.9/picsellia_tf2/object_detection/models/ssd_mobilenet_v1_feature_extractor_tf2_test.py`

 * *Files identical despite different names*

### Comparing `picsellia_tf2-0.8/picsellia_tf2/pxl_utils.py` & `picsellia_tf2-0.9/picsellia_tf2/pxl_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,24 +248,18 @@
         config_dict: A configuration dictionnary loaded from the protobuf file with config_util.get_configs_from_pipeline_file().
         incremental_or_transfer: String name to identify use case "transfer" of "incremental".
     Raises:
         ValueError
     '''
     if not FromSratch:
         config_dict["train_config"].from_detection_checkpoint = True
-    if incremental_or_transfer == "incremental":
-        config_dict["train_config"].load_all_detection_checkpoint_vars = True
-    elif incremental_or_transfer == "transfer":
-        config_dict["train_config"].load_all_detection_checkpoint_vars = False
-    else:
-        raise ValueError("Please choose if you want to do transfer or incremental learning") 
 
 
 
-def edit_config(model_selected, config_output_dir, num_steps, label_map_path, record_dir, eval_number, annotation_type, 
+def edit_config(model_selected, config_dir, num_steps, label_map_path, record_dir, eval_number, annotation_type, 
                 batch_size=None, learning_rate=None, resizer_size=None, incremental_or_transfer="transfer"):
     '''
         Wrapper to edit the essential values inside the base configuration protobuf file provided with an object-detection/segmentation checkpoint.
         This configuration file is what will entirely define your model, pre-processing, training, evaluation etc. It is the most important file of a model with the checkpoint file and should never be deleted. 
         This is why it is saved in almost every directory where you did something to keep redondancy but also to be sure to have the right config file used at this moment.
         For advanced users, if you want to dwell deep inside the configuration file you should read the proto definitions inside the proto directory of the object-detection API.
 
@@ -291,20 +285,20 @@
     file_list = os.listdir(model_selected)
     ckpt_ids = []
     for p in file_list:
         if "index" in p:
             if "-" in p:
                 ckpt_ids.append(int(p.split('-')[1].split('.')[0]))
     if len(ckpt_ids)>0:
-        ckpt_path = os.path.join(model_selected,"model.ckpt-{}".format(str(max(ckpt_ids))))
+        ckpt_path = os.path.join(model_selected,"ckpt-{}".format(str(max(ckpt_ids))))
     
     else:
-        ckpt_path = os.path.join(model_selected, "model.ckpt")
+        ckpt_path = os.path.join(model_selected, "ckpt")
 
-    configs = config_util.get_configs_from_pipeline_file(os.path.join(model_selected,'pipeline.config'))
+    configs = config_util.get_configs_from_pipeline_file(os.path.join(config_dir,'pipeline.config'))
     label_map = label_map_util.load_labelmap(label_map_path)
 
     config_util._update_train_steps(configs, num_steps)
     update_different_paths(configs, ckpt_path=ckpt_path, 
                             label_map_path=label_map_path, 
                             train_record_path=os.path.join(record_dir, "train.record"), 
                             eval_record_path=os.path.join(record_dir,"eval.record"))
@@ -324,16 +318,17 @@
 
     if incremental_or_transfer is not None:
         set_variable_loader(configs, incremental_or_transfer)
     
     edit_eval_config(configs, annotation_type, eval_number)
     update_num_classes(configs, label_map)
     config_proto = config_util.create_pipeline_proto_from_configs(configs)
-    config_util.save_pipeline_config(config_proto, directory=config_output_dir)
-    print(f"Configuration successfully edited and saved at {config_output_dir}")
+    config_util._update_batch_size(configs, batch_size)
+    config_util.save_pipeline_config(config_proto, directory=config_dir)
+    print(f"Configuration successfully edited and saved at {config_dir}")
 
 
 def train(ckpt_dir='', config='', train_steps=1000, use_tpu=False, checkpoint_every_n=100,
           record_summaries=True):
 
     if config.endswith('.config'):
         if not os.path.isfile(config):
@@ -341,15 +336,15 @@
     else:
         if os.path.isdir(config):
             files = os.listdir(config)
             file_found = False
             for f in files:
                 if not file_found:
                     if f.endswith('.config'):
-                        config = f 
+                        config = os.path.join(config,f)
                         file_found = True 
     if not file_found:
         raise FileNotFoundError('No config file found in this directory {}'.format(config))
 
     tf.config.set_soft_device_placement(True)
     strategy = tf.compat.v2.distribute.MirroredStrategy()
 
@@ -483,15 +478,15 @@
     else:
         if os.path.isdir(config):
             files = os.listdir(config)
             file_found = False
             for f in files:
                 if not file_found:
                     if f.endswith('.config'):
-                        config = f 
+                        config = os.path.join(config,f)
                         file_found = True 
     if not file_found:
         raise FileNotFoundError('No config file found in this directory {}'.format(config))
 
     tf.config.set_soft_device_placement(True)
     model_lib_v2.eval_continuously(
         pipeline_config_path=config,
@@ -519,15 +514,15 @@
     else:
         if os.path.isdir(path):
             files = os.listdir(path)
             file_found = False
             for f in files:
                 if not file_found:
                     if f.startswith('events.out'):
-                        path = f 
+                        path = os.path.join(path,f)
                         file_found = True 
     if not file_found:
         raise FileNotFoundError('No tfEvent file found in this directory {}'.format(path))
     for summary in summary_iterator(path):
         for v in summary.summary.value:
             if not 'image' in v.tag:
                 if v.tag in log_dict.keys():
```

### Comparing `picsellia_tf2-0.8/picsellia_tf2.egg-info/SOURCES.txt` & `picsellia_tf2-0.9/picsellia_tf2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

