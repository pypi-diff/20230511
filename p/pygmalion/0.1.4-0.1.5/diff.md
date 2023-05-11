# Comparing `tmp/pygmalion-0.1.4.tar.gz` & `tmp/pygmalion-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmalion-0.1.4.tar", last modified: Tue Apr 11 20:18:03 2023, max compression
+gzip compressed data, was "pygmalion-0.1.5.tar", last modified: Thu May 11 00:52:19 2023, max compression
```

## Comparing `pygmalion-0.1.4.tar` & `pygmalion-0.1.5.tar`

### file list

```diff
@@ -1,84 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.689890 pygmalion-0.1.4/
--rw-rw-rw-   0        0        0     1085 2023-02-19 10:00:21.000000 pygmalion-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     7481 2023-04-11 20:18:03.689890 pygmalion-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6942 2023-03-27 11:47:38.000000 pygmalion-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.643849 pygmalion-0.1.4/pygmalion/
--rw-rw-rw-   0        0        0      179 2023-02-26 08:55:42.000000 pygmalion-0.1.4/pygmalion/__init__.py
--rw-rw-rw-   0        0        0       53 2023-04-11 20:17:46.000000 pygmalion-0.1.4/pygmalion/_info.py
--rw-rw-rw-   0        0        0     1858 2023-04-08 20:30:29.000000 pygmalion-0.1.4/pygmalion/_model.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.666869 pygmalion-0.1.4/pygmalion/datasets/
--rw-rw-rw-   0        0        0      330 2023-04-08 21:42:29.000000 pygmalion-0.1.4/pygmalion/datasets/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-08 21:42:37.000000 pygmalion-0.1.4/pygmalion/datasets/_airline_tweets.py
--rw-rw-rw-   0        0        0      334 2023-04-08 21:42:48.000000 pygmalion-0.1.4/pygmalion/datasets/_aquarium.py
--rw-rw-rw-   0        0        0      353 2023-04-08 21:42:46.000000 pygmalion-0.1.4/pygmalion/datasets/_boston_housing.py
--rw-rw-rw-   0        0        0      342 2023-04-08 21:42:51.000000 pygmalion-0.1.4/pygmalion/datasets/_cityscapes.py
--rw-rw-rw-   0        0        0      341 2023-04-08 21:43:00.000000 pygmalion-0.1.4/pygmalion/datasets/_fashion_mnist.py
--rw-rw-rw-   0        0        0      323 2023-04-08 21:43:03.000000 pygmalion-0.1.4/pygmalion/datasets/_iris.py
--rw-rw-rw-   0        0        0      385 2023-04-08 21:43:06.000000 pygmalion-0.1.4/pygmalion/datasets/_sentence_pairs.py
--rw-rw-rw-   0        0        0      332 2023-04-08 21:43:09.000000 pygmalion-0.1.4/pygmalion/datasets/_titanic.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.669873 pygmalion-0.1.4/pygmalion/datasets/generators/
--rw-rw-rw-   0        0        0      159 2023-04-08 20:29:21.000000 pygmalion-0.1.4/pygmalion/datasets/generators/__init__.py
--rw-rw-rw-   0        0        0     3698 2023-02-26 08:07:23.000000 pygmalion-0.1.4/pygmalion/datasets/generators/_circles_generator.py
--rw-rw-rw-   0        0        0     2335 2023-03-18 11:53:06.000000 pygmalion-0.1.4/pygmalion/datasets/generators/_roman_numerals_generator.py
--rw-rw-rw-   0        0        0     4063 2023-04-11 18:11:29.000000 pygmalion-0.1.4/pygmalion/datasets/generators/_shapes_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.677879 pygmalion-0.1.4/pygmalion/neural_networks/
--rw-rw-rw-   0        0        0      383 2023-04-09 11:47:43.000000 pygmalion-0.1.4/pygmalion/neural_networks/__init__.py
--rw-rw-rw-   0        0        0     9292 2023-04-09 13:28:07.000000 pygmalion-0.1.4/pygmalion/neural_networks/_conversions.py
--rw-rw-rw-   0        0        0     3132 2023-03-24 13:39:04.000000 pygmalion-0.1.4/pygmalion/neural_networks/_dense_classifier.py
--rw-rw-rw-   0        0        0     4037 2023-03-24 13:37:40.000000 pygmalion-0.1.4/pygmalion/neural_networks/_dense_regressor.py
--rw-rw-rw-   0        0        0     2863 2023-03-24 13:39:04.000000 pygmalion-0.1.4/pygmalion/neural_networks/_image_classifier.py
--rw-rw-rw-   0        0        0    15902 2023-04-11 18:30:31.000000 pygmalion-0.1.4/pygmalion/neural_networks/_image_object_detector.py
--rw-rw-rw-   0        0        0     4251 2023-03-24 13:39:04.000000 pygmalion-0.1.4/pygmalion/neural_networks/_image_segmenter.py
--rw-rw-rw-   0        0        0     4598 2023-04-10 17:40:55.000000 pygmalion-0.1.4/pygmalion/neural_networks/_loss_functions.py
--rw-rw-rw-   0        0        0    10521 2023-04-08 21:56:10.000000 pygmalion-0.1.4/pygmalion/neural_networks/_neural_network.py
--rw-rw-rw-   0        0        0     6422 2023-03-28 16:59:24.000000 pygmalion-0.1.4/pygmalion/neural_networks/_text_classifier.py
--rw-rw-rw-   0        0        0     6565 2023-03-28 17:00:06.000000 pygmalion-0.1.4/pygmalion/neural_networks/_text_segmenter.py
--rw-rw-rw-   0        0        0    18376 2023-04-09 09:44:05.000000 pygmalion-0.1.4/pygmalion/neural_networks/_text_translator.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.682884 pygmalion-0.1.4/pygmalion/neural_networks/layers/
--rw-rw-rw-   0        0        0      602 2023-03-11 11:30:46.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/__init__.py
--rw-rw-rw-   0        0        0     1218 2023-04-08 21:26:11.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/_activation.py
--rw-rw-rw-   0        0        0     2328 2023-04-06 12:15:33.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/_conv_block.py
--rw-rw-rw-   0        0        0     3451 2023-03-05 10:47:16.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/_normalizer.py
--rw-rw-rw-   0        0        0     3167 2023-02-24 14:25:21.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/_padded_conv.py
--rw-rw-rw-   0        0        0     2375 2023-03-14 15:30:15.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/_positional_encoding.py
--rw-rw-rw-   0        0        0     1791 2023-02-24 15:48:47.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/_upsampling.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.686887 pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/
--rw-rw-rw-   0        0        0      108 2023-03-12 12:44:54.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/__init__.py
--rw-rw-rw-   0        0        0    11373 2023-03-18 18:53:35.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_attention.py
--rw-rw-rw-   0        0        0     4689 2023-03-18 18:52:48.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_multihead_attention.py
--rw-rw-rw-   0        0        0     4887 2023-03-14 08:58:05.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_stack.py
--rw-rw-rw-   0        0        0     6934 2023-03-14 13:01:02.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_stages.py
--rw-rw-rw-   0        0        0     1333 2023-03-13 14:05:17.000000 pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.689890 pygmalion-0.1.4/pygmalion/tokenizers/
--rw-rw-rw-   0        0        0      188 2023-03-11 22:05:58.000000 pygmalion-0.1.4/pygmalion/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     1452 2023-03-27 11:23:04.000000 pygmalion-0.1.4/pygmalion/tokenizers/_ascii_char_tokenizer.py
--rw-rw-rw-   0        0        0     9881 2023-04-08 22:43:59.000000 pygmalion-0.1.4/pygmalion/tokenizers/_byte_pair_encoder.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.689890 pygmalion-0.1.4/pygmalion/tokenizers/_utilities/
--rw-rw-rw-   0        0        0      176 2023-04-08 21:17:04.000000 pygmalion-0.1.4/pygmalion/tokenizers/_utilities/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-03-03 15:19:46.000000 pygmalion-0.1.4/pygmalion/tokenizers/_utilities/_bytes_tree.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 17:57:11.000000 pygmalion-0.1.4/pygmalion/tokenizers/_utilities/_functions.py
--rw-rw-rw-   0        0        0      483 2023-02-26 09:01:48.000000 pygmalion-0.1.4/pygmalion/tokenizers/_utilities/_special_token.py
--rw-rw-rw-   0        0        0     3709 2023-04-08 21:17:06.000000 pygmalion-0.1.4/pygmalion/tokenizers/_utilities/_tokenizer.py
--rw-rw-rw-   0        0        0     3004 2023-03-10 17:17:36.000000 pygmalion-0.1.4/pygmalion/tokenizers/_words_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.689890 pygmalion-0.1.4/pygmalion/unsupervised/
--rw-rw-rw-   0        0        0       22 2023-02-26 08:42:10.000000 pygmalion-0.1.4/pygmalion/unsupervised/__init__.py
--rw-rw-rw-   0        0        0     3469 2023-04-08 20:31:17.000000 pygmalion-0.1.4/pygmalion/unsupervised/pca.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.689890 pygmalion-0.1.4/pygmalion/utilities/
--rw-rw-rw-   0        0        0      277 2023-04-08 21:44:23.000000 pygmalion-0.1.4/pygmalion/utilities/__init__.py
--rw-rw-rw-   0        0        0     2677 2023-02-19 10:02:35.000000 pygmalion-0.1.4/pygmalion/utilities/_cross_validation.py
--rw-rw-rw-   0        0        0     3775 2023-02-19 10:00:21.000000 pygmalion-0.1.4/pygmalion/utilities/_decorators.py
--rw-rw-rw-   0        0        0     2215 2023-04-09 11:51:21.000000 pygmalion-0.1.4/pygmalion/utilities/_download.py
--rw-rw-rw-   0        0        0     1774 2023-04-11 20:17:18.000000 pygmalion-0.1.4/pygmalion/utilities/_load_model.py
--rw-rw-rw-   0        0        0     6453 2023-02-19 10:02:35.000000 pygmalion-0.1.4/pygmalion/utilities/_metrics.py
--rw-rw-rw-   0        0        0     6916 2023-04-10 18:08:54.000000 pygmalion-0.1.4/pygmalion/utilities/_ploting.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.659864 pygmalion-0.1.4/pygmalion.egg-info/
--rw-rw-rw-   0        0        0     7481 2023-04-11 20:18:03.000000 pygmalion-0.1.4/pygmalion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2773 2023-04-11 20:18:03.000000 pygmalion-0.1.4/pygmalion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 20:18:03.000000 pygmalion-0.1.4/pygmalion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-04-11 20:18:03.000000 pygmalion-0.1.4/pygmalion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 20:18:03.000000 pygmalion-0.1.4/pygmalion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 20:18:03.689890 pygmalion-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1262 2023-03-31 19:08:49.000000 pygmalion-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:18:03.689890 pygmalion-0.1.4/test/
--rw-rw-rw-   0        0        0      596 2023-03-14 13:51:25.000000 pygmalion-0.1.4/test/test_decoder_stage.py
--rw-rw-rw-   0        0        0     5062 2023-03-12 12:47:08.000000 pygmalion-0.1.4/test/test_kernelized_attention.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.081575 pygmalion-0.1.5/
+-rw-rw-rw-   0        0        0     1085 2023-02-19 10:00:21.000000 pygmalion-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     7481 2023-05-11 00:52:19.081575 pygmalion-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6942 2023-03-27 11:47:38.000000 pygmalion-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.001438 pygmalion-0.1.5/pygmalion/
+-rw-rw-rw-   0        0        0      179 2023-02-26 08:55:42.000000 pygmalion-0.1.5/pygmalion/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-05-11 00:51:54.000000 pygmalion-0.1.5/pygmalion/_info.py
+-rw-rw-rw-   0        0        0     1858 2023-04-08 20:30:29.000000 pygmalion-0.1.5/pygmalion/_model.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.021431 pygmalion-0.1.5/pygmalion/datasets/
+-rw-rw-rw-   0        0        0      369 2023-04-17 09:37:44.000000 pygmalion-0.1.5/pygmalion/datasets/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-08 21:42:37.000000 pygmalion-0.1.5/pygmalion/datasets/_airline_tweets.py
+-rw-rw-rw-   0        0        0      334 2023-04-08 21:42:48.000000 pygmalion-0.1.5/pygmalion/datasets/_aquarium.py
+-rw-rw-rw-   0        0        0      353 2023-04-08 21:42:46.000000 pygmalion-0.1.5/pygmalion/datasets/_boston_housing.py
+-rw-rw-rw-   0        0        0      342 2023-04-08 21:42:51.000000 pygmalion-0.1.5/pygmalion/datasets/_cityscapes.py
+-rw-rw-rw-   0        0        0      341 2023-04-08 21:43:00.000000 pygmalion-0.1.5/pygmalion/datasets/_fashion_mnist.py
+-rw-rw-rw-   0        0        0      323 2023-04-08 21:43:03.000000 pygmalion-0.1.5/pygmalion/datasets/_iris.py
+-rw-rw-rw-   0        0        0      385 2023-04-08 21:43:06.000000 pygmalion-0.1.5/pygmalion/datasets/_sentence_pairs.py
+-rw-rw-rw-   0        0        0      332 2023-04-08 21:43:09.000000 pygmalion-0.1.5/pygmalion/datasets/_titanic.py
+-rw-rw-rw-   0        0        0      330 2023-04-17 09:37:25.000000 pygmalion-0.1.5/pygmalion/datasets/_usa_economy.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.040742 pygmalion-0.1.5/pygmalion/datasets/generators/
+-rw-rw-rw-   0        0        0      159 2023-04-08 20:29:21.000000 pygmalion-0.1.5/pygmalion/datasets/generators/__init__.py
+-rw-rw-rw-   0        0        0     3698 2023-02-26 08:07:23.000000 pygmalion-0.1.5/pygmalion/datasets/generators/_circles_generator.py
+-rw-rw-rw-   0        0        0     2335 2023-03-18 11:53:06.000000 pygmalion-0.1.5/pygmalion/datasets/generators/_roman_numerals_generator.py
+-rw-rw-rw-   0        0        0     4063 2023-04-11 18:11:29.000000 pygmalion-0.1.5/pygmalion/datasets/generators/_shapes_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.041749 pygmalion-0.1.5/pygmalion/neural_networks/
+-rw-rw-rw-   0        0        0      383 2023-04-09 11:47:43.000000 pygmalion-0.1.5/pygmalion/neural_networks/__init__.py
+-rw-rw-rw-   0        0        0     9292 2023-04-09 13:28:07.000000 pygmalion-0.1.5/pygmalion/neural_networks/_conversions.py
+-rw-rw-rw-   0        0        0     3159 2023-05-08 18:56:45.000000 pygmalion-0.1.5/pygmalion/neural_networks/_dense_classifier.py
+-rw-rw-rw-   0        0        0     3925 2023-05-08 19:14:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/_dense_regressor.py
+-rw-rw-rw-   0        0        0     2618 2023-05-01 13:40:52.000000 pygmalion-0.1.5/pygmalion/neural_networks/_image_classifier.py
+-rw-rw-rw-   0        0        0    15671 2023-05-01 13:37:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/_image_object_detector.py
+-rw-rw-rw-   0        0        0     3917 2023-05-10 06:32:14.000000 pygmalion-0.1.5/pygmalion/neural_networks/_image_segmenter.py
+-rw-rw-rw-   0        0        0     4627 2023-04-28 08:55:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/_loss_functions.py
+-rw-rw-rw-   0        0        0    12897 2023-05-01 14:08:12.000000 pygmalion-0.1.5/pygmalion/neural_networks/_neural_network.py
+-rw-rw-rw-   0        0        0     6341 2023-04-24 21:23:40.000000 pygmalion-0.1.5/pygmalion/neural_networks/_text_classifier.py
+-rw-rw-rw-   0        0        0     6484 2023-04-26 18:21:07.000000 pygmalion-0.1.5/pygmalion/neural_networks/_text_segmenter.py
+-rw-rw-rw-   0        0        0    18204 2023-04-24 21:24:15.000000 pygmalion-0.1.5/pygmalion/neural_networks/_text_translator.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.052365 pygmalion-0.1.5/pygmalion/neural_networks/layers/
+-rw-rw-rw-   0        0        0      235 2023-05-08 18:36:43.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     1218 2023-04-08 21:26:11.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_activation.py
+-rw-rw-rw-   0        0        0     1698 2023-05-08 19:15:35.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_dropout.py
+-rw-rw-rw-   0        0        0     6262 2023-05-08 19:14:00.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_normalization.py
+-rw-rw-rw-   0        0        0     2375 2023-05-01 13:38:55.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_positional_encoding.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.052365 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/
+-rw-rw-rw-   0        0        0      285 2023-05-01 12:29:29.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/__init__.py
+-rw-rw-rw-   0        0        0     2614 2023-05-08 18:29:06.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_conv_block.py
+-rw-rw-rw-   0        0        0     3090 2023-05-01 12:53:43.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_padded_conv.py
+-rw-rw-rw-   0        0        0     4082 2023-05-01 14:00:12.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_stack.py
+-rw-rw-rw-   0        0        0     3319 2023-05-01 13:58:21.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_stages.py
+-rw-rw-rw-   0        0        0     1791 2023-02-24 15:48:47.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_upsampling.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.060871 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/
+-rw-rw-rw-   0        0        0      108 2023-05-01 13:38:49.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/__init__.py
+-rw-rw-rw-   0        0        0    11373 2023-03-18 18:53:35.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_attention.py
+-rw-rw-rw-   0        0        0     4689 2023-03-18 18:52:48.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_multihead_attention.py
+-rw-rw-rw-   0        0        0     4887 2023-03-14 08:58:05.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stack.py
+-rw-rw-rw-   0        0        0     6543 2023-04-24 21:25:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stages.py
+-rw-rw-rw-   0        0        0     1333 2023-03-13 14:05:17.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.061881 pygmalion-0.1.5/pygmalion/tokenizers/
+-rw-rw-rw-   0        0        0      188 2023-03-11 22:05:58.000000 pygmalion-0.1.5/pygmalion/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     1452 2023-03-27 11:23:04.000000 pygmalion-0.1.5/pygmalion/tokenizers/_ascii_char_tokenizer.py
+-rw-rw-rw-   0        0        0     9881 2023-04-08 22:43:59.000000 pygmalion-0.1.5/pygmalion/tokenizers/_byte_pair_encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.061881 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/
+-rw-rw-rw-   0        0        0      176 2023-04-08 21:17:04.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-03-03 15:19:46.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_bytes_tree.py
+-rw-rw-rw-   0        0        0     1334 2023-02-26 17:57:11.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_functions.py
+-rw-rw-rw-   0        0        0      483 2023-02-26 09:01:48.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_special_token.py
+-rw-rw-rw-   0        0        0     3709 2023-04-08 21:17:06.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_tokenizer.py
+-rw-rw-rw-   0        0        0     3004 2023-03-10 17:17:36.000000 pygmalion-0.1.5/pygmalion/tokenizers/_words_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.061881 pygmalion-0.1.5/pygmalion/unsupervised/
+-rw-rw-rw-   0        0        0       22 2023-02-26 08:42:10.000000 pygmalion-0.1.5/pygmalion/unsupervised/__init__.py
+-rw-rw-rw-   0        0        0     3469 2023-04-08 20:31:17.000000 pygmalion-0.1.5/pygmalion/unsupervised/pca.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.081575 pygmalion-0.1.5/pygmalion/utilities/
+-rw-rw-rw-   0        0        0      277 2023-04-08 21:44:23.000000 pygmalion-0.1.5/pygmalion/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-02-19 10:02:35.000000 pygmalion-0.1.5/pygmalion/utilities/_cross_validation.py
+-rw-rw-rw-   0        0        0     3775 2023-02-19 10:00:21.000000 pygmalion-0.1.5/pygmalion/utilities/_decorators.py
+-rw-rw-rw-   0        0        0     2215 2023-04-09 11:51:21.000000 pygmalion-0.1.5/pygmalion/utilities/_download.py
+-rw-rw-rw-   0        0        0     1774 2023-04-11 20:17:18.000000 pygmalion-0.1.5/pygmalion/utilities/_load_model.py
+-rw-rw-rw-   0        0        0     6453 2023-02-19 10:02:35.000000 pygmalion-0.1.5/pygmalion/utilities/_metrics.py
+-rw-rw-rw-   0        0        0     6916 2023-04-10 18:08:54.000000 pygmalion-0.1.5/pygmalion/utilities/_ploting.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.021431 pygmalion-0.1.5/pygmalion.egg-info/
+-rw-rw-rw-   0        0        0     7481 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3066 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 00:52:19.081575 pygmalion-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1262 2023-03-31 19:08:49.000000 pygmalion-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.081575 pygmalion-0.1.5/test/
+-rw-rw-rw-   0        0        0      596 2023-03-14 13:51:25.000000 pygmalion-0.1.5/test/test_decoder_stage.py
+-rw-rw-rw-   0        0        0     5062 2023-03-12 12:47:08.000000 pygmalion-0.1.5/test/test_kernelized_attention.py
```

### Comparing `pygmalion-0.1.4/LICENSE` & `pygmalion-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/PKG-INFO` & `pygmalion-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmalion
-Version: 0.1.4
+Version: 0.1.5
 Summary: A machine learning package
 Home-page: https://github.com/BFavier/Pygmalion
 Author: Benoit Favier
 Author-email: benoitfamillefavier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmalion-0.1.4/README.md` & `pygmalion-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/_model.py` & `pygmalion-0.1.5/pygmalion/_model.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/datasets/generators/_circles_generator.py` & `pygmalion-0.1.5/pygmalion/datasets/generators/_circles_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/datasets/generators/_roman_numerals_generator.py` & `pygmalion-0.1.5/pygmalion/datasets/generators/_roman_numerals_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/datasets/generators/_shapes_generator.py` & `pygmalion-0.1.5/pygmalion/datasets/generators/_shapes_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_conversions.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_conversions.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_dense_classifier.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_dense_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import pandas as pd
-from typing import List, Union, Iterable, Optional, Sequence
+from typing import List, Union, Iterable, Optional
 from ._conversions import classes_to_tensor, tensor_to_classes
 from ._conversions import named_to_tensor, tensor_to_probabilities
 from ._neural_network import NeuralNetworkClassifier
 from ._loss_functions import cross_entropy
-from .layers import Activation, Normalizer
+from .layers import Activation, Normalizer, FeaturesNorm, Dropout
 
 
 class DenseClassifier(NeuralNetworkClassifier):
 
     def __init__(self, inputs: Iterable[str],
                  target: str, classes: Iterable[str],
                  hidden_layers: Iterable[int],
@@ -27,29 +27,29 @@
 
         """
         super().__init__(classes)
         self.inputs = tuple(inputs)
         self.target = str(target)
         self.layers = torch.nn.ModuleList()
         in_features = len(inputs)
-        if normalize:
-            self.layers.append(Normalizer(in_features, affine=False))
+        self.input_normalizer = Normalizer(1, in_features, affine=False)
         for out_features in hidden_layers:
             self.layers.append(torch.nn.Linear(in_features, out_features))
             if normalize:
-                self.layers.append(Normalizer(out_features))
+                self.layers.append(FeaturesNorm(1, out_features))
             self.layers.append(Activation(activation))
             if dropout is not None:
-                self.layers.append(torch.nn.Dropout(dropout))
+                self.layers.append(Dropout(dropout))
             in_features = out_features
         out_features = len(self.classes)
         self.output = torch.nn.Linear(in_features, out_features)
 
     def forward(self, X: torch.Tensor):
         X = X.to(self.device)
+        X = self.input_normalizer(X)
         for layer in self.layers:
             X = layer(X)
         return self.output(X)
 
     def loss(self, x: torch.Tensor, y_target: torch.Tensor,
              weights: Optional[torch.Tensor] = None):
         y_pred = self(x)
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_dense_regressor.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_dense_regressor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 import pandas as pd
 import numpy as np
-from typing import Sequence, Union, Iterable, Optional
+from typing import Union, Iterable, Optional
 from ._conversions import floats_to_tensor, tensor_to_floats
 from ._conversions import named_to_tensor, tensor_to_dataframe
 from ._neural_network import NeuralNetwork
 from ._loss_functions import MSE
-from .layers import Activation, Normalizer
+from .layers import Activation, Normalizer, FeaturesNorm, Dropout
 
 
 class DenseRegressor(NeuralNetwork):
     """
     DenseRegressor is an implementation of a fully connected NeuralNetwork
     for tabular regression.
 
@@ -42,42 +42,37 @@
             the dropout after each hidden layer if provided
         """
         super().__init__()
         self.inputs = tuple(inputs)
         self.target = target if isinstance(target, str) else tuple(target)
         self.layers = torch.nn.ModuleList()
         in_features = len(inputs)
-        if normalize:
-            self.layers.append(Normalizer(in_features, affine=False))
+        self.input_normalizer = Normalizer(1, in_features, affine=False)
         for out_features in hidden_layers:
             self.layers.append(torch.nn.Linear(in_features, out_features))
             if normalize:
-                self.layers.append(Normalizer(out_features))
+                self.layers.append(FeaturesNorm(1, out_features))
             self.layers.append(Activation(activation))
-            if dropout is not None:
-                self.layers.append(torch.nn.Dropout(dropout))
+            self.layers.append(Dropout(dropout))
             in_features = out_features
         out_features = 1 if isinstance(target, str) else len(self.target)
         self.output = torch.nn.Linear(in_features, out_features)
-        if normalize:
-            self.target_norm = Normalizer(out_features, affine=False)
-        else:
-            self.target_norm = None
+        self.target_normalizer = Normalizer(1, out_features, affine=False)
 
     def forward(self, X: torch.Tensor):
         X = X.to(self.device)
+        X = self.input_normalizer(X)
         for layer in self.layers:
             X = layer(X)
         return self.output(X)
 
     def loss(self, x: torch.Tensor, y_target: torch.Tensor,
              weights: Optional[torch.Tensor] = None):
         y_pred = self(x)
-        if self.target_norm is not None:
-            y_target = self.target_norm(y_target)
+        y_target = self.target_normalizer(y_target)
         return MSE(y_pred, y_target, weights)
 
     @property
     def device(self) -> torch.device:
         return self.output.weight.device
 
     def _x_to_tensor(self, x: Union[pd.DataFrame, dict, Iterable],
@@ -86,13 +81,13 @@
 
     def _y_to_tensor(self, y: Union[pd.DataFrame, dict, Iterable],
                      device: Optional[torch.device] = None) -> torch.Tensor:
         target = [self.target] if isinstance(self.target, str) else list(self.target)
         return named_to_tensor(y, target, device=device)
 
     def _tensor_to_y(self, tensor: torch.Tensor) -> np.ndarray:
-        if self.target_norm is not None:
-            tensor = self.target_norm.unscale(tensor)
+        if self.target_normalizer is not None:
+            tensor = self.target_normalizer.unscale(tensor)
         if isinstance(self.target, str):
             return tensor_to_floats(tensor).reshape(-1)
         else:
             return tensor_to_dataframe(tensor, self.target)
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_image_classifier.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_image_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,47 @@
 import torch
 import pandas as pd
 import numpy as np
-from typing import Union, List, Iterable, Tuple, Optional
-from .layers import ConvBlock
+from typing import List, Iterable, Tuple, Optional
+from .layers.convolutions import ConvolutionalEncoder
 from ._conversions import tensor_to_classes
 from ._conversions import classes_to_tensor, images_to_tensor
 from ._conversions import tensor_to_probabilities
 from ._neural_network import NeuralNetworkClassifier
 from ._loss_functions import cross_entropy
 
 
 class ImageClassifier(NeuralNetworkClassifier):
 
     def __init__(self, in_channels: int,
                  classes: Iterable[str],
                  features: Iterable[int],
                  kernel_size: Tuple[int, int] = (3, 3),
-                 pooling_size: Optional[Tuple[int, int]] = (2, 2),
+                 pooling_size: Tuple[int, int] = (2, 2),
                  stride: Tuple[int, int] = (1, 1),
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
-                 dropout: Optional[float] = None):
+                 dropout: Optional[float] = None,
+                 low_memory: bool = True):
         """
         Parameters
         ----------
         ...
         """
         super().__init__(classes)
-        self.layers = torch.nn.ModuleList()
-        in_features = in_channels
-        for out_features in features:
-            self.layers.append(
-                ConvBlock(in_features, out_features, kernel_size, stride, activation,
-                          normalize, residuals, n_convs_per_block, dropout))
-            if pooling_size is not None:
-                self.layers.append(torch.nn.MaxPool2d(pooling_size))
-            in_features = out_features
-        self.output = torch.nn.Linear(out_features, len(self.classes))
+        self.encoder = ConvolutionalEncoder(
+            in_channels, features, kernel_size, pooling_size, stride, activation,
+            n_convs_per_block, normalize, residuals, dropout, low_memory)
+        self.output = torch.nn.Linear(features[-1], len(self.classes))
 
     def forward(self, X: torch.Tensor):
         X = X.to(self.device)
-        for layer in self.layers:
-            X = layer(X)
+        X = self.encoder(X)
         N, C, H, W = X.shape
         X = X.reshape(N, C, -1).mean(dim=-1)
         return self.output(X)
 
     def loss(self, x: torch.Tensor, y_target: torch.Tensor,
              weights: Optional[torch.Tensor] = None,
              class_weights: Optional[torch.Tensor] = None):
@@ -66,8 +60,8 @@
                      device: Optional[torch.device] = None) -> torch.Tensor:
         return classes_to_tensor(y, self.classes, device=device)
 
     def _tensor_to_y(self, tensor: torch.Tensor) -> List[str]:
         return tensor_to_classes(tensor, self.classes)
 
     def _tensor_to_proba(self, tensor: torch.Tensor) -> pd.DataFrame:
-        return tensor_to_probabilities(tensor, self.classes)
+        return tensor_to_probabilities(tensor, self.classes)
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_image_object_detector.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_image_object_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 import torch
 import pandas as pd
 import numpy as np
 import torch.nn.functional as F
 from typing import List, Sequence, Iterable, Tuple, Optional
-from .layers import ConvBlock
+from .layers.convolutions import ConvolutionalEncoder, PaddedConv2d
 from ._conversions import tensor_to_classes
 from ._conversions import classes_to_tensor, images_to_tensor, floats_to_tensor
 from ._conversions import tensor_to_probabilities
 from ._neural_network import NeuralNetworkClassifier
-from ._loss_functions import cross_entropy, MSE
+from ._loss_functions import cross_entropy, RMSE
 
 
 class ImageObjectDetector(NeuralNetworkClassifier):
 
     def __init__(self, in_channels: int,
                  classes: Iterable[str],
                  features: Iterable[int],
                  bboxes_per_cell: int = 5,
                  kernel_size: Tuple[int, int] = (3, 3),
-                 pooling_size: Optional[Tuple[int, int]] = (2, 2),
+                 pooling_size: Tuple[int, int] = (2, 2),
                  stride: Tuple[int, int] = (1, 1),
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
-                 dropout: Optional[float] = None):
+                 dropout: Optional[float] = None,
+                 low_memory: bool = True):
         """
         Parameters
         ----------
         ...
         """
         super().__init__(classes)
         self.cells_dimensions = tuple((s*mp) ** len(features) for s, mp in zip(stride, pooling_size or (1, 1)))
         self.layers = torch.nn.ModuleList()
         self.bboxes_per_cell = bboxes_per_cell
-        in_features = in_channels
-        for out_features in features:
-            self.layers.append(
-                ConvBlock(in_features, out_features, kernel_size, stride, activation,
-                          normalize, residuals, n_convs_per_block, dropout))
-            if pooling_size is not None:
-                self.layers.append(torch.nn.MaxPool2d(pooling_size))
-            in_features = out_features
-        self.confidence = torch.nn.Conv2d(out_features, self.bboxes_per_cell, (1, 1))
-        self.positions = torch.nn.Conv2d(out_features, self.bboxes_per_cell*2, (1, 1))
-        self.dimensions = torch.nn.Conv2d(out_features, self.bboxes_per_cell*2, (1, 1))
-        self.objects_class = torch.nn.Conv2d(out_features, self.bboxes_per_cell*len(self.classes), (1, 1))
+        self.encoder = ConvolutionalEncoder(
+            in_channels, features, kernel_size, pooling_size, stride, activation,
+            n_convs_per_block, normalize, residuals, dropout, low_memory)
+        self.confidence = PaddedConv2d(features[-1], self.bboxes_per_cell, kernel_size)
+        self.positions = PaddedConv2d(features[-1], self.bboxes_per_cell*2, kernel_size)
+        self.dimensions = PaddedConv2d(features[-1], self.bboxes_per_cell*2, kernel_size)
+        self.objects_class = PaddedConv2d(features[-1], self.bboxes_per_cell*len(self.classes), kernel_size)
 
     def forward(self, X: torch.Tensor):
         """
         Parameters
         ----------
         X : torch.Tensor
             tensor of float images of shape (N, C, H, W)
@@ -64,18 +60,17 @@
                tensor of floats of shape (N, bboxes_per_cell, 2, h, w)
             * 'dimension' relative (w, h) dimension of the detected object in each cell,
               tensor of floats of shape (N, bboxes_per_cell, 2, h, w)
             * 'object_class' probability (once softmaxed) of each class in each cell,
               tensor of floats of shape (N, bboxes_per_cell, n_classes, h, w)
         """
         X = X.to(self.device)
-        for layer in self.layers:
-            X = layer(X)
+        X = self.encoder(X)
         N, C, H, W = X.shape
-        confidence = self.confidence(X).reshape(N, self.bboxes_per_cell, H, W)
+        confidence = torch.sigmoid(self.confidence(X)).reshape(N, self.bboxes_per_cell, H, W)
         position = torch.sigmoid(self.positions(X)).reshape(N, self.bboxes_per_cell, 2, H, W)
         dimension = torch.log(1 + torch.exp(self.dimensions(X))).reshape(N, self.bboxes_per_cell, 2, H, W)
         object_class = self.objects_class(X).reshape(N, self.bboxes_per_cell, len(self.classes), H, W)
         return confidence, position, dimension, object_class
 
     def _weighted_mean(self, tensor: torch.Tensor, weights: torch.Tensor) -> torch.Tensor:
         """
@@ -111,22 +106,22 @@
             ).squeeze(2).permute(0, 2, 3, 1)  # IoU of shape (N, H, W, bboxes_per_cell)
         # changing axes order and calculating weights
         confidence_pred, position_pred, dimension_pred, class_pred = (
             torch.moveaxis(t, 1, -1) for t in (confidence_pred, position_pred, dimension_pred, class_pred))  # reshape to (N, *, H, W, bboxes_per_cell)
         weights = self._softscale(confidence_pred, dim=-1)  # weights of shape (N, H, W, bboxes_per_cell)
         # Compute losses
         absent = ~presence
-        absence_loss = self._weighted_mean(-torch.log(1 - torch.sigmoid(confidence_pred[absent])), weights[absent])
+        absence_loss = self._weighted_mean(-torch.log(1 - confidence_pred[absent]), weights[absent])
         if presence.any():
             presence_2d = presence.unsqueeze(1).expand(-1, 2, -1, -1)
             weights_presence_2d = weights.unsqueeze(1).expand(-1, 2, -1, -1, -1)[presence_2d]
-            bboxe_confidence_loss = MSE(torch.sigmoid(confidence_pred[presence]), IoU[presence])
+            bboxe_confidence_loss = RMSE(confidence_pred[presence], IoU[presence])
             return (absence_loss + bboxe_confidence_loss 
-                    + MSE(position_pred[presence_2d], positions[presence_2d].unsqueeze(-1), weights=weights_presence_2d)
-                    + MSE(dimension_pred[presence_2d], dimensions[presence_2d].unsqueeze(-1), weights=weights_presence_2d)
+                    + RMSE(position_pred[presence_2d], positions[presence_2d].unsqueeze(-1), weights=weights_presence_2d)
+                    + RMSE(dimension_pred[presence_2d], dimensions[presence_2d].unsqueeze(-1), weights=weights_presence_2d)
                     + cross_entropy(class_pred.moveaxis(1, -2)[presence],
                                     object_class[presence].unsqueeze(-1).expand(-1, self.bboxes_per_cell),
                                     weights=weights[presence],
                                     class_weights=class_weights))
         else:
             return absence_loss
 
@@ -148,15 +143,14 @@
             h_cell, w_cell = self.cells_dimensions
             N, _, h_grid, w_grid = confidence.shape
             # select most confident bboxe for each cell
             confidence, bboxe_index = confidence.max(dim=1)
             position, dimension, object_class = (
                 torch.gather(tensor, 1, bboxe_index.reshape(N, 1, 1, h_grid, w_grid).expand(-1, -1, tensor.shape[2], -1, -1)).squeeze(1)
                 for tensor in (position, dimension, object_class))
-            confidence = torch.sigmoid(confidence)
             # converting from grid coordinates to pixel coordinates
             grid_pos = torch.stack(torch.meshgrid(torch.arange(0, w_image, w_cell, dtype=position.dtype, device=self.device),
                                 torch.arange(0, h_image, h_cell, dtype=position.dtype, device=self.device),
                                 indexing="xy"), dim=0)
             cell_dimension = torch.tensor([w_cell, h_cell], dtype=torch.float, device=self.device).reshape(1, 2, 1, 1)
             pixel_position = grid_pos.unsqueeze(0) + position * cell_dimension
             pixel_dimension = dimension * cell_dimension
@@ -251,15 +245,15 @@
     @staticmethod
     def _softscale(X: torch.Tensor, dim: int=0) -> torch.Tensor:
         X = torch.exp(X)
         return X / X.max(dim=dim).values.unsqueeze(dim)
 
     @property
     def device(self) -> torch.device:
-        return self.confidence.weight.device
+        return self.confidence.conv.weight.device
 
     def _x_to_tensor(self, x: np.ndarray,
                      device: Optional[torch.device] = None):
         return images_to_tensor(x, device=device)
 
     def _y_to_tensor(self, x: np.ndarray, y: Iterable[dict],
                      device: Optional[torch.device] = None) -> torch.Tensor:
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_image_segmenter.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_image_segmenter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import torch
 import pandas as pd
 import numpy as np
 from typing import List, Iterable, Tuple, Optional
-from .layers import ConvBlock, Upsampling2d, UPSAMPLING_METHOD
+from .layers.convolutions import ConvBlock, Upsampling2d, PaddedConv2d, UPSAMPLING_METHOD
+from .layers.convolutions import ConvolutionalEncoder, ConvolutionalDecoder
 from ._conversions import tensor_to_index
 from ._conversions import longs_to_tensor, images_to_tensor
 from ._conversions import tensor_to_floats
 from ._neural_network import NeuralNetworkClassifier
-from ._loss_functions import cross_entropy
+from ._loss_functions import cross_entropy, soft_dice_loss
 
 
 class ImageSegmenter(NeuralNetworkClassifier):
 
     def __init__(self, in_channels: int,
                  classes: Iterable[str],
                  features: Iterable[int],
@@ -19,65 +20,55 @@
                  pooling_size: Optional[Tuple[int, int]] = (2, 2),
                  stride: Tuple[int, int] = (1, 1),
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
                  upsampling_method: UPSAMPLING_METHOD = "nearest",
-                 dropout: Optional[float] = None):
+                 dropout: Optional[float] = None,
+                 entropy_dice_mixture: float = 0.9,
+                 low_memory: bool = True):
         """
         Parameters
         ----------
         ...
         """
         super().__init__(classes)
-        self.encoder = torch.nn.ModuleList()
+        self.entropy_dice_mixture = entropy_dice_mixture
         scale_factor = tuple(a*b for a, b in zip(stride, pooling_size or (1, 1)))
-        in_features = in_channels
-        for out_features in features:
-            layer = torch.nn.ModuleDict(
-                {"convolutions": ConvBlock(in_features, out_features, kernel_size, stride, activation,
-                                           normalize, residuals, n_convs_per_block, dropout),
-                 "downsampling": torch.nn.MaxPool2d(pooling_size) if pooling_size is not None else None})
-            self.encoder.append(layer)
-            in_features = out_features
-        self.decoder = torch.nn.ModuleList()
-        for out_features, add_features in zip(features[::-1], features[-2::-1]+[in_channels]):
-            convolutions = ConvBlock(in_features+add_features, out_features,
-                                     kernel_size, (1, 1), activation, normalize,
-                                     residuals, n_convs_per_block, dropout)
-            layer = torch.nn.ModuleDict(
-                {"upsampling": Upsampling2d(scale_factor, method=upsampling_method) if scale_factor != (1, 1) else None,
-                 "convolutions": convolutions})
-            self.decoder.append(layer)
-            in_features = out_features
-        self.output = torch.nn.Conv2d(out_features, len(self.classes), (1, 1))
+        self.encoder = ConvolutionalEncoder(in_channels, features, kernel_size,
+                                            pooling_size, stride, activation,
+                                            n_convs_per_block, normalize,
+                                            residuals, dropout, low_memory)
+        self.intermediate = ConvBlock(
+            features[-1], features[-1], kernel_size, stride, activation,
+            normalize, residuals, n_convs_per_block, dropout)
+        self.decoder = ConvolutionalDecoder(features[-1], features[::-1], features[::-1],
+                                            kernel_size, scale_factor, upsampling_method,
+                                            activation, n_convs_per_block, normalize,
+                                            residuals, dropout, low_memory)
+        self.output = torch.nn.Conv2d(features[0], len(self.classes), (1, 1))
 
     def forward(self, X: torch.Tensor):
         X = X.to(self.device)
         encoded = []
-        for layer in self.encoder:
-            encoded.append(X)
-            convolutions, downsampling = layer["convolutions"], layer["downsampling"], 
-            X = convolutions(X)
-            if downsampling is not None:
-                X = downsampling(X)
-        for layer, feature_map in zip(self.decoder, encoded[::-1]):
-            upsampling, convolutions = layer["upsampling"], layer["convolutions"]
-            upsampled = upsampling(X) if upsampling is not None else X
-            X = torch.cat([feature_map, upsampled], dim=1)
-            X = convolutions(X)
+        X = self.encoder(X, encoded)
+        X = self.intermediate(X)
+        X = self.decoder(X, encoded[::-1])
         return self.output(X)
 
     def loss(self, x: torch.Tensor, y_target: torch.Tensor,
              weights: Optional[torch.Tensor] = None,
              class_weights: Optional[torch.Tensor] = None):
+        assert 0.0 <= self.entropy_dice_mixture <= 1.0
+        assert ((0 <= y_target) & (y_target < len(self.classes))).all()
+        alpha = self.entropy_dice_mixture
         y_pred = self(x)
-        return cross_entropy(y_pred, y_target, weights, class_weights)
-    
+        return alpha * cross_entropy(y_pred, y_target, weights, class_weights) + (1-alpha) * soft_dice_loss(y_pred, y_target, weights, class_weights)
+
     @property
     def device(self) -> torch.device:
         return self.output.weight.device
 
     def _x_to_tensor(self, x: np.ndarray,
                      device: Optional[torch.device] = None):
         return images_to_tensor(x, device=device)
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_loss_functions.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_loss_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,35 +97,39 @@
                    ) -> torch.Tensor:
     """
     A soft Dice loss for segmentation
 
     Parameters
     ----------
     y_pred : torch.Tensor
-        A Tensor of float of shape [N_observations, N_classes, ...]
-        The probability of each class for eahc observation
+        A Tensor of float of shape (n, c, *)
+        The probability (pre-softmax) of each class for each observation
     y_target : torch.Tensor
-        A Tensor of long of shape [N_observations, 1, ...]
+        A Tensor of long of shape (n, *)
         The index of the class to be predicted
     weights : None or torch.Tensor
         The individual observation weights (ignored if None)
+        a tensor of floats shape (n,)
     class_weights : None or torch.Tensor
-        If None, all classes are equally weighted
         The class-wise weights (ignored if None)
+        a tensor of shape (c)
 
     Returns
     -------
     torch.Tensor :
         the scalar value of the loss
     """
-    if (weights is not None) or (class_weights is not None):
-        raise NotImplementedError("Weighting in soft_dice_loss is not implemented yet")
+    n, c = y_pred.shape[:2]
     y_target = y_target.to(y_pred.device)
-    n_classes = y_pred.shape[1]
-    pred = F.softmax(y_pred, dim=1)
+    y_pred = F.softmax(y_pred, dim=1)
     eps = 1.0E-5
-    target = F.one_hot(y_target, num_classes=n_classes).permute(0, 3, 1, 2)
-    intersect = torch.sum(pred * target, dim=[2, 3])
-    cardinality = torch.sum(pred + target, dim=[2, 3])
+    target = F.one_hot(y_target, num_classes=c).moveaxis(-1, 1)
+    intersect = y_pred * target
+    cardinality = (y_pred + target)
     dice_coeff = (2.*intersect + eps) / (cardinality + eps)
+    dice_coeff = dice_coeff.reshape(n, c, -1).mean(dim=-1)
+    if weights is not None:
+        dice_coeff = dice_coeff * weights.unsqueeze(1)
+    if class_weights is not None:
+        dice_coeff = dice_coeff * class_weights.unsqueeze(0)
     loss = 1. - torch.mean(dice_coeff)
     return loss
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_neural_network.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_neural_network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import io
 import copy
 import pathlib
+import math
 import torch
 from typing import Union, Sequence, Optional, Callable, Iterable, List
 from ._conversions import floats_to_tensor
+from .layers import Dropout
 from pygmalion._model import Model
+from datetime import datetime
 
 
 class NeuralNetwork(torch.nn.Module, Model):
     """
     Abstract class for neural networks
     Implemented as a simple wrapper around torch.nn.Module
     with 'fit' and 'predict' methods
@@ -54,18 +57,20 @@
     def fit(self, training_data: Iterable,
             validation_data: Optional[Iterable] = None,
             optimizer: Optional[torch.optim.Optimizer] = None,
             n_steps: int = 1000,
             learning_rate: Union[float, Callable[[int], float]] = 1.0E-3,
             patience: Optional[int] = None,
             keep_best: bool = True,
-            loss: Optional[Callable] = None,
             L1: Optional[float] = None,
             L2: Optional[float] = None,
-            metric: Optional[Callable] = None,
+            gradient_cliping: Optional[float] = None,
+            backup_path: Optional[str] = None,
+            backup_prefix: str = "model",
+            backup_frequency: int = 10000,
             verbose: bool = True):
         """
         Trains a neural network model.
 
         Parameters
         ----------
         training_data : Iterable of (x, y) or (x, y, weights) data
@@ -87,17 +92,38 @@
             The number of steps before early stopping
             (if no improvement for 'patience' steps, stops training early)
             If None, no early stoping is performed
         keep_best : bool
             If True, the model is checkpointed at each step if there was
             improvement,
             and the best model is loaded back at the end of training
+        L1 : float or None
+            L1 regularization factor
+        L2 : float
+            L2 regularization factor
+        gradient_cliping : float or None
+            if provided, the gradient vector is cliped in the (-gradient_clipping, gradient_clipping) range
+        backup_path : str or path like or None
+            if provided, path where to backup the model (and optimizer) on disk
+        backup_prefix : str
+            prefix of the backup filename (the suffix is the current number step)
+        backup_frequency : int
+            number of steps before each on-disk backup
         verbose : bool
             If True the loss are displayed at each epoch
+        
+        Returns
+        -------
+        tuple :
+            (train_losses, val_losses, grad_norms, best_step)
         """
+        if backup_path is not None:
+            backup_path = pathlib.Path(backup_path)
+            if not backup_path.is_dir():
+                raise NotADirectoryError(f"Backup path is not a valid directory: '{backup_path}'")
         best_step = 0
         best_state = copy.deepcopy(self.state_dict())
         best_metric = None
         train_losses = []
         val_losses = []
         grad_norms = []
         if optimizer is None:
@@ -130,16 +156,21 @@
                 train_loss = sum(train_loss) / max(1, n_batches)
                 train_losses.append(train_loss)
                 # averaging gradient over batches
                 if n_batches > 1:
                     for p in self.parameters():
                         if p.grad is not None:
                             p.grad /= n_batches
+                # gradient cliping
+                if gradient_cliping is not None:
+                    for p in self.parameters():
+                        if p.grad is not None:
+                            p.grad = torch.clip(p.grad, -gradient_cliping, gradient_cliping)
                 # gradient norm
-                grad_norms.append(self._norm((p.grad for p in self.parameters()), 1, average=False).item())
+                grad_norms.append(self._norm((p.grad for p in self.parameters() if p.grad is not None), 1).item())
                 # validation data
                 self.eval()
                 if validation_data is not None:
                     val_loss = []
                     with torch.no_grad():
                         for batch in validation_data:
                             val_loss.append(self.loss(*batch).item())
@@ -155,18 +186,27 @@
                     if keep_best:
                         best_state = copy.deepcopy(self.state_dict())
                 # early stoping
                 if patience is not None and (step - best_step) > patience:
                     break
                 # message printing
                 if verbose:
+                    time = datetime.now().strftime("[%Y/%m/%d-%H:%M:%S]")
                     if val_loss is not None:
-                        print(f"Step {step}: train loss = {train_loss:.3g}, val loss = {val_loss:.3g}, grad = {grad_norms[-1]:.3g}")
+                        print(f"{time} Step {step}: train loss = {train_loss:.3g}, val loss = {val_loss:.3g}, grad = {grad_norms[-1]:.3e}")
                     else:
-                        print(f"Step {step}: train loss = {train_loss:.3g}, grad = {grad_norms[-1]:.3g}")
+                        print(f"{time} Step {step}: train loss = {train_loss:.3g}, grad = {grad_norms[-1]:.3e}")
+                # backup on disk
+                if (backup_path is not None) and (step % backup_frequency == 0) and (step > 0):
+                    dec = math.floor(math.log10(n_steps)) + 1
+                    torch.save(self, backup_path / f"{backup_prefix}_{step:0{dec}}.pth")
+                    torch.save(optimizer, backup_path / f"optimizer_{backup_prefix}_{step:0{dec}}.pth")
+                    if verbose:
+                        print(f"Backed up on disk '{backup_prefix}_{step:0{dec}}.pth'")
+
         except KeyboardInterrupt:
             if verbose:
                 print("Training interrupted by the user")
         finally:
             # load the best state
             if keep_best:
                 self.load_state_dict(best_state)
@@ -190,14 +230,27 @@
         x = self._x_to_tensor(*args)
         with torch.no_grad():
             y_pred = self(x)
         return self._tensor_to_y(y_pred)
     
     def loss(x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError()
+    
+    @property
+    def dropout(self) -> Optional[float]:
+        for m in self.modules():
+            if isinstance(m, Dropout):
+                return m.p
+        return None
+
+    @dropout.setter
+    def dropout(self, other: Optional[float]):
+        for m in self.modules():
+            if isinstance(m, Dropout):
+                m.p = other
 
     def _x_to_tensor(self, x: object) -> torch.Tensor:
         raise NotImplementedError()
 
     def _y_to_tensor(self, y: object) -> torch.Tensor:
         raise NotImplementedError()
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_text_classifier.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_text_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import pandas as pd
 from typing import Union, List, Optional, Literal
 from .layers.transformers import TransformerEncoder, ATTENTION_TYPE
-from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding
+from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding, Dropout
 from ._conversions import strings_to_tensor, tensor_to_classes, tensor_to_probabilities
 from ._conversions import classes_to_tensor
 from ._neural_network import NeuralNetworkClassifier
 from ._loss_functions import cross_entropy
 from pygmalion.tokenizers._utilities import Tokenizer
 
 
@@ -59,15 +59,15 @@
         super().__init__(classes)
         self.mask_padding = mask_padding
         self.sequence_length = sequence_length
         embedding_dim = projection_dim*n_heads
         self.tokenizer = tokenizer
         self.embedding = torch.nn.Embedding(self.tokenizer.n_tokens,
                                                   embedding_dim)
-        self.dropout_input = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.dropout_input = Dropout(dropout)
         if positional_encoding_type == "sinusoidal":
             self.positional_encoding = SinusoidalPositionalEncoding()
         elif positional_encoding_type == "learned":
             assert sequence_length is not None
             self.positional_encoding = LearnedPositionalEncoding(sequence_length, embedding_dim)
         elif positional_encoding_type is None:
             self.positional_encoding = None
@@ -97,16 +97,15 @@
         """
         X = X.to(self.device)
         padding_mask = (X == self.tokenizer.PAD) if self.mask_padding else None
         N, L = X.shape
         X = self.embedding(X)
         if self.positional_encoding is not None:
             X = self.positional_encoding(X)
-        if self.dropout_input is not None:
-            X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
+        X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
         X = self.transformer_encoder(X, padding_mask)
         return self.head(X.mean(dim=1))
 
     def loss(self, x, y_target, weights=None, class_weights=None):
         """
         Parameters
         ----------
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_text_segmenter.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_text_segmenter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import pandas as pd
 from typing import Union, List, Optional, Literal, Iterable
 from .layers.transformers import TransformerEncoder, ATTENTION_TYPE
-from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding
+from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding, Dropout
 from ._conversions import strings_to_tensor, tensor_to_classes, tensor_to_probabilities
 from ._conversions import classes_to_tensor
 from ._neural_network import NeuralNetworkClassifier
 from ._loss_functions import cross_entropy
 from pygmalion.tokenizers._utilities import Tokenizer
 
 
@@ -59,15 +59,15 @@
         super().__init__(classes)
         self.mask_padding = mask_padding
         self.sequence_length = sequence_length
         embedding_dim = projection_dim*n_heads
         self.tokenizer = tokenizer
         self.embedding = torch.nn.Embedding(self.tokenizer.n_tokens,
                                                   embedding_dim)
-        self.dropout_input = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.dropout_input = Dropout(dropout)
         if positional_encoding_type == "sinusoidal":
             self.positional_encoding = SinusoidalPositionalEncoding()
         elif positional_encoding_type == "learned":
             assert sequence_length is not None
             self.positional_encoding = LearnedPositionalEncoding(sequence_length, embedding_dim)
         elif positional_encoding_type is None:
             self.positional_encoding = None
@@ -99,16 +99,15 @@
         """
         X = X.to(self.device)
         padding_mask = (X == self.tokenizer.PAD) if self.mask_padding else None
         N, L = X.shape
         X = self.embedding(X)
         if self.positional_encoding is not None:
             X = self.positional_encoding(X)
-        if self.dropout_input is not None:
-            X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
+        X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
         X = self.transformer_encoder(X, padding_mask)
         return self.head(X)
 
     def loss(self, x, y_target, weights=None, class_weights=None):
         """
         Parameters
         ----------
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/_text_translator.py` & `pygmalion-0.1.5/pygmalion/neural_networks/_text_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import numpy as np
 from typing import Union, List, Sequence, Optional, Literal
 from itertools import count
 from warnings import warn
 from .layers.transformers import TransformerEncoder, TransformerDecoder, ATTENTION_TYPE
-from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding
+from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding, Dropout
 from ._conversions import strings_to_tensor, tensor_to_strings
 from ._conversions import floats_to_tensor
 from ._neural_network import NeuralNetwork
 from ._loss_functions import cross_entropy
 from pygmalion.tokenizers._utilities import Tokenizer, SpecialToken
 
 
@@ -73,16 +73,16 @@
         embedding_dim = projection_dim*n_heads
         self.tokenizer_input = tokenizer_input
         self.tokenizer_output = tokenizer_output
         self.embedding_input = torch.nn.Embedding(self.tokenizer_input.n_tokens,
                                                   embedding_dim)
         self.embedding_output = torch.nn.Embedding(self.tokenizer_output.n_tokens,
                                                 embedding_dim)
-        self.dropout_input = torch.nn.Dropout(dropout) if dropout is not None else None
-        self.dropout_output = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.dropout_input = Dropout(dropout)
+        self.dropout_output = Dropout(dropout)
         if positional_encoding_type == "sinusoidal":
             self.positional_encoding_input = SinusoidalPositionalEncoding()
             self.positional_encoding_output = SinusoidalPositionalEncoding()
         elif positional_encoding_type == "learned":
             assert input_sequence_length is not None and output_sequence_length is not None
             self.positional_encoding_input = LearnedPositionalEncoding(input_sequence_length, embedding_dim)
             self.positional_encoding_output = LearnedPositionalEncoding(output_sequence_length, embedding_dim)
@@ -125,16 +125,15 @@
         X = X.to(self.device)
         if padding_mask is not None:
             padding_mask = padding_mask.to(self.device)
         N, L = X.shape
         X = self.embedding_input(X)
         if self.positional_encoding_input is not None:
             X = self.positional_encoding_input(X)
-        if self.dropout_input is not None:
-            X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
+        X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
         X = self.transformer_encoder(X, padding_mask)
         return X
 
     def decode(self, Y: torch.Tensor, encoded: torch.Tensor, encoded_padding_mask: Optional[torch.Tensor]):
         """
         performs the decoding part of the network
 
@@ -157,16 +156,15 @@
         torch.Tensor :
             tensor of floats of shape (N, Ly, D)
         """
         N, L = Y.shape
         Y = self.embedding_output(Y)
         if self.positional_encoding_output is not None:
             Y = self.positional_encoding_output(Y)
-        if self.dropout_output is not None:
-            Y = self.dropout_output(Y.reshape(N*L, -1)).reshape(N, L, -1)
+        Y = self.dropout_output(Y.reshape(N*L, -1)).reshape(N, L, -1)
         Y = self.transformer_decoder(Y, encoded, encoded_padding_mask)
         return self.head(Y)
 
     def loss(self, x, y_target, weights=None):
         """
         Parameters
         ----------
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/_activation.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/_activation.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/_padded_conv.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_padded_conv.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,23 @@
         See torch.nn.Conv2d for parameters documentation
         """
         super().__init__()
         conv = torch.nn.Conv2d(in_channels, out_channels, kernel_size,
             stride=stride, dilation=dilation, groups=groups, bias=bias,
             device=device, dtype=dtype)
         kernel_size = tuple(k + (k-1)*(d-1) for k, d in zip(conv.kernel_size, conv.dilation))
-        padding = [p for dim in kernel_size[::-1] for p in (dim//2, dim//2)]
+        padding = [p for dim in kernel_size[::-1] for p in ((dim-1)//2, (dim-1) - (dim-1)//2)]
         self.padding = torch.nn.ConstantPad2d(padding, 0.)
         self.conv = conv
 
     def _forward(self, X):
         return self.conv(self.padding(X))
 
     def forward(self, X: torch.Tensor):
-        if self.training:
-            X.requires_grad_(True)  # To ensure that the gradient is backpropagated in the convolution parameters
+        if self.training and X.requires_grad:
             return checkpoint(self._forward, X)
         else:
             return self._forward(X)
 
 
 
 # class AdaptativePad2d(torch.nn.Module):
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/_positional_encoding.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/_upsampling.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_upsampling.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_attention.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_attention.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_multihead_attention.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_multihead_attention.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_stack.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stack.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_stages.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 from typing import Optional
 from ._multihead_attention import MultiHeadAttention, ATTENTION_TYPE
+from pygmalion.neural_networks.layers._dropout import Dropout
 from torch.utils.checkpoint import checkpoint
 
 
 class TransformerEncoderStage(torch.nn.Module):
 
     def __init__(self, projection_dim: int, n_heads: int,
                  dropout: Optional[float] = None,
@@ -15,18 +16,18 @@
         dim = projection_dim * n_heads
         self.activation = getattr(torch, activation)
         self.self_attention = MultiHeadAttention(projection_dim, n_heads, False,
                                                  RPE_radius=RPE_radius,
                                                  attention_type=attention_type,
                                                  **kwargs)
         self.intermediate_norm = torch.nn.LayerNorm(dim)
-        self.intermediate_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.intermediate_dropout = Dropout(dropout)
         self.expand = torch.nn.Linear(dim, dim * 4)
         self.contract = torch.nn.Linear(dim * 4, dim)
-        self.out_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.out_dropout = Dropout(dropout)
         self.out_norm = torch.nn.LayerNorm(dim)
 
     def forward(self, X: torch.Tensor,
                 padding_mask: Optional[torch.Tensor] = None):
         """
         Parameter
         ---------
@@ -44,21 +45,19 @@
         torch.Tensor
             tensor of shape (N, L, D)
         """
         X = X.to(self.device)
         N, L, _ = X.shape
         input = X.reshape(N * L, -1)
         X = self.self_attention(X, X, padding_mask, padding_mask).reshape(N * L, -1)
-        if self.intermediate_dropout is not None:
-            X = self.intermediate_dropout(X) + input
+        X = self.intermediate_dropout(X) + input
         X = self.intermediate_norm(X)
         input = X
         X = self.contract(self.activation(self.expand(X)))
-        if self.out_dropout is not None:
-            X = self.out_dropout(X)
+        X = self.out_dropout(X)
         X = self.out_norm(X + input)
         return X.reshape(N, L, -1)
 
     @property
     def device(self) -> torch.device:
         return self.self_attention.key.weight.device
 
@@ -73,24 +72,24 @@
         super().__init__()
         dim = projection_dim * n_heads
         self.activation = getattr(torch, activation)
         self.masked_self_attention = MultiHeadAttention(projection_dim, n_heads, True,
                                                         RPE_radius=RPE_radius,
                                                         attention_type=attention_type,
                                                         **kwargs)
-        self.first_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.first_dropout = Dropout(dropout)
         self.first_norm = torch.nn.LayerNorm(dim)
         self.attention = MultiHeadAttention(projection_dim, n_heads, False,
                                             RPE_radius=RPE_radius,
                                             attention_type=attention_type)
-        self.second_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.second_dropout = Dropout(dropout)
         self.second_norm = torch.nn.LayerNorm(dim)
         self.expand = torch.nn.Linear(dim, 4 * dim)
         self.contract = torch.nn.Linear(4 * dim, dim)
-        self.out_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.out_dropout = Dropout(dropout)
         self.out_norm = torch.nn.LayerNorm(dim)
 
     def forward(self, Y, encoded,
                 encoded_padding_mask: Optional[torch.Tensor] = None):
         """
         Parameter
         ---------
@@ -107,27 +106,24 @@
             tensor of shape (N, L, D)
         """
         encoded = encoded.to(self.device)
         Y = Y.to(self.device)
         N, L, _ = Y.shape
         input = Y.reshape(N * L, -1)
         Y = self.masked_self_attention(Y, Y).reshape(N * L, -1)
-        if self.first_dropout is not None:
-            Y = self.first_dropout(Y)
+        Y = self.first_dropout(Y)
         Y = self.first_norm(Y + input).reshape(N, L, -1)
         input = Y.reshape(N * L, -1)
         Y = self.attention(Y, encoded, query_padding_mask=None,
                            key_padding_mask=encoded_padding_mask).reshape(N * L, -1)
-        if self.second_dropout is not None:
-            Y = self.second_dropout(Y)
+        Y = self.second_dropout(Y)
         Y = self.second_norm(Y + input)
         input = Y
         Y = self.contract(self.activation(self.expand(Y)))
-        if self.out_dropout is not None:
-            Y = self.out_dropout(Y)
+        Y = self.out_dropout(Y)
         Y = self.out_norm(Y + input)
         return Y.reshape(N, L, -1)
 
     def predict(self, Y, encoded,
                 encoded_padding_mask: Optional[torch.Tensor]):
         """
         Efficiently predict the next representation
```

### Comparing `pygmalion-0.1.4/pygmalion/neural_networks/layers/transformers/_utilities.py` & `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_utilities.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/tokenizers/_ascii_char_tokenizer.py` & `pygmalion-0.1.5/pygmalion/tokenizers/_ascii_char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/tokenizers/_byte_pair_encoder.py` & `pygmalion-0.1.5/pygmalion/tokenizers/_byte_pair_encoder.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/tokenizers/_utilities/_bytes_tree.py` & `pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_bytes_tree.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/tokenizers/_utilities/_functions.py` & `pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_functions.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/tokenizers/_utilities/_tokenizer.py` & `pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/tokenizers/_words_tokenizer.py` & `pygmalion-0.1.5/pygmalion/tokenizers/_words_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/unsupervised/pca.py` & `pygmalion-0.1.5/pygmalion/unsupervised/pca.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/utilities/_cross_validation.py` & `pygmalion-0.1.5/pygmalion/utilities/_cross_validation.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/utilities/_decorators.py` & `pygmalion-0.1.5/pygmalion/utilities/_decorators.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/utilities/_download.py` & `pygmalion-0.1.5/pygmalion/utilities/_download.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/utilities/_load_model.py` & `pygmalion-0.1.5/pygmalion/utilities/_load_model.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/utilities/_metrics.py` & `pygmalion-0.1.5/pygmalion/utilities/_metrics.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion/utilities/_ploting.py` & `pygmalion-0.1.5/pygmalion/utilities/_ploting.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/pygmalion.egg-info/PKG-INFO` & `pygmalion-0.1.5/pygmalion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmalion
-Version: 0.1.4
+Version: 0.1.5
 Summary: A machine learning package
 Home-page: https://github.com/BFavier/Pygmalion
 Author: Benoit Favier
 Author-email: benoitfamillefavier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmalion-0.1.4/pygmalion.egg-info/SOURCES.txt` & `pygmalion-0.1.5/pygmalion.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pygmalion/datasets/_aquarium.py
 pygmalion/datasets/_boston_housing.py
 pygmalion/datasets/_cityscapes.py
 pygmalion/datasets/_fashion_mnist.py
 pygmalion/datasets/_iris.py
 pygmalion/datasets/_sentence_pairs.py
 pygmalion/datasets/_titanic.py
+pygmalion/datasets/_usa_economy.py
 pygmalion/datasets/generators/__init__.py
 pygmalion/datasets/generators/_circles_generator.py
 pygmalion/datasets/generators/_roman_numerals_generator.py
 pygmalion/datasets/generators/_shapes_generator.py
 pygmalion/neural_networks/__init__.py
 pygmalion/neural_networks/_conversions.py
 pygmalion/neural_networks/_dense_classifier.py
@@ -32,19 +33,23 @@
 pygmalion/neural_networks/_loss_functions.py
 pygmalion/neural_networks/_neural_network.py
 pygmalion/neural_networks/_text_classifier.py
 pygmalion/neural_networks/_text_segmenter.py
 pygmalion/neural_networks/_text_translator.py
 pygmalion/neural_networks/layers/__init__.py
 pygmalion/neural_networks/layers/_activation.py
-pygmalion/neural_networks/layers/_conv_block.py
-pygmalion/neural_networks/layers/_normalizer.py
-pygmalion/neural_networks/layers/_padded_conv.py
+pygmalion/neural_networks/layers/_dropout.py
+pygmalion/neural_networks/layers/_normalization.py
 pygmalion/neural_networks/layers/_positional_encoding.py
-pygmalion/neural_networks/layers/_upsampling.py
+pygmalion/neural_networks/layers/convolutions/__init__.py
+pygmalion/neural_networks/layers/convolutions/_conv_block.py
+pygmalion/neural_networks/layers/convolutions/_padded_conv.py
+pygmalion/neural_networks/layers/convolutions/_stack.py
+pygmalion/neural_networks/layers/convolutions/_stages.py
+pygmalion/neural_networks/layers/convolutions/_upsampling.py
 pygmalion/neural_networks/layers/transformers/__init__.py
 pygmalion/neural_networks/layers/transformers/_attention.py
 pygmalion/neural_networks/layers/transformers/_multihead_attention.py
 pygmalion/neural_networks/layers/transformers/_stack.py
 pygmalion/neural_networks/layers/transformers/_stages.py
 pygmalion/neural_networks/layers/transformers/_utilities.py
 pygmalion/tokenizers/__init__.py
```

### Comparing `pygmalion-0.1.4/setup.py` & `pygmalion-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/test/test_decoder_stage.py` & `pygmalion-0.1.5/test/test_decoder_stage.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.4/test/test_kernelized_attention.py` & `pygmalion-0.1.5/test/test_kernelized_attention.py`

 * *Files identical despite different names*

