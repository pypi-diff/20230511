# Comparing `tmp/eznlp-0.2.3rc1.tar.gz` & `tmp/eznlp-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\eznlp-0.2.3rc1.tar", last modified: Thu Nov 11 03:09:55 2021, max compression
+gzip compressed data, was "dist\eznlp-0.2.4.tar", last modified: Thu May 11 01:04:38 2023, max compression
```

## Comparing `eznlp-0.2.3rc1.tar` & `eznlp-0.2.4.tar`

### file list

```diff
@@ -1,92 +1,101 @@
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.651531 eznlp-0.2.3rc1/
--rw-rw-rw-   0        0        0    11637 2021-08-27 08:08:40.000000 eznlp-0.2.3rc1/LICENSE
--rw-rw-rw-   0        0        0       73 2021-08-27 08:08:40.000000 eznlp-0.2.3rc1/MANIFEST.in
--rw-rw-rw-   0        0        0     4491 2021-11-11 03:09:55.651531 eznlp-0.2.3rc1/PKG-INFO
--rw-rw-rw-   0        0        0     3317 2021-11-11 02:52:20.000000 eznlp-0.2.3rc1/README.md
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.475942 eznlp-0.2.3rc1/eznlp/
--rw-rw-rw-   0        0        0      278 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/__init__.py
--rw-rw-rw-   0        0        0     5419 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/config.py
--rw-rw-rw-   0        0        0     5473 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/dataset.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.526945 eznlp-0.2.3rc1/eznlp/io/
--rw-rw-rw-   0        0        0      295 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/io/__init__.py
--rw-rw-rw-   0        0        0     1010 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/io/base.py
--rw-rw-rw-   0        0        0    18539 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/io/brat.py
--rw-rw-rw-   0        0        0     1414 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/io/category_folder.py
--rw-rw-rw-   0        0        0     1923 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/io/chip.py
--rw-rw-rw-   0        0        0     7047 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/io/conll.py
--rw-rw-rw-   0        0        0    10556 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/io/json.py
--rw-rw-rw-   0        0        0     8893 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/io/processing.py
--rw-rw-rw-   0        0        0     1892 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/io/src2trg.py
--rw-rw-rw-   0        0        0     1661 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/io/tabular.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.531943 eznlp-0.2.3rc1/eznlp/language_modeling/
--rw-rw-rw-   0        0        0      163 2021-03-08 03:37:31.000000 eznlp-0.2.3rc1/eznlp/language_modeling/__init__.py
--rw-rw-rw-   0        0        0     3582 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/language_modeling/dataset.py
--rw-rw-rw-   0        0        0     3187 2021-04-20 13:48:55.000000 eznlp-0.2.3rc1/eznlp/language_modeling/model.py
--rw-rw-rw-   0        0        0      644 2021-11-10 03:32:32.000000 eznlp-0.2.3rc1/eznlp/language_modeling/trainer.py
--rw-rw-rw-   0        0        0     5052 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/metrics.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.540943 eznlp-0.2.3rc1/eznlp/model/
--rw-rw-rw-   0        0        0      391 2021-10-20 02:49:33.000000 eznlp-0.2.3rc1/eznlp/model/__init__.py
--rw-rw-rw-   0        0        0    14721 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/bert_like.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.554943 eznlp-0.2.3rc1/eznlp/model/decoder/
--rw-rw-rw-   0        0        0      609 2021-08-30 00:01:06.000000 eznlp-0.2.3rc1/eznlp/model/decoder/__init__.py
--rw-rw-rw-   0        0        0     3724 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/model/decoder/base.py
--rw-rw-rw-   0        0        0    16661 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/decoder/boundary_selection.py
--rw-rw-rw-   0        0        0    32582 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/decoder/generator.py
--rw-rw-rw-   0        0        0     6852 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/decoder/joint_extraction.py
--rw-rw-rw-   0        0        0     6592 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/model/decoder/sequence_tagging.py
--rw-rw-rw-   0        0        0    13016 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/decoder/span_attr_classification.py
--rw-rw-rw-   0        0        0     9516 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/decoder/span_classification.py
--rw-rw-rw-   0        0        0    16289 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/decoder/span_rel_classification.py
--rw-rw-rw-   0        0        0     4125 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/model/decoder/text_classification.py
--rw-rw-rw-   0        0        0     3841 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/elmo.py
--rw-rw-rw-   0        0        0     8051 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/embedder.py
--rw-rw-rw-   0        0        0    12965 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/encoder.py
--rw-rw-rw-   0        0        0     4691 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/flair.py
--rw-rw-rw-   0        0        0     4366 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/image_encoder.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.583942 eznlp-0.2.3rc1/eznlp/model/model/
--rw-rw-rw-   0        0        0      235 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/model/__init__.py
--rw-rw-rw-   0        0        0     2310 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/model/model/base.py
--rw-rw-rw-   0        0        0     8353 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/model/model/classifier.py
--rw-rw-rw-   0        0        0     9320 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/model/model/extractor.py
--rw-rw-rw-   0        0        0     2789 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/model/image2text.py
--rw-rw-rw-   0        0        0     2958 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/model/text2text.py
--rw-rw-rw-   0        0        0     9256 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/model/nested_embedder.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.591943 eznlp-0.2.3rc1/eznlp/nn/
--rw-rw-rw-   0        0        0       49 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/nn/__init__.py
--rw-rw-rw-   0        0        0    10412 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/functional.py
--rw-rw-rw-   0        0        0     6323 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/init.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.616532 eznlp-0.2.3rc1/eznlp/nn/modules/
--rw-rw-rw-   0        0        0      488 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/modules/__init__.py
--rw-rw-rw-   0        0        0     3258 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/modules/aggregation.py
--rw-rw-rw-   0        0        0    10219 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/modules/attention.py
--rw-rw-rw-   0        0        0     8266 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/modules/block.py
--rw-rw-rw-   0        0        0     7848 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/modules/crf.py
--rw-rw-rw-   0        0        0     2683 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/nn/modules/dropout.py
--rw-rw-rw-   0        0        0      952 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/modules/embedding.py
--rw-rw-rw-   0        0        0     2207 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/nn/modules/loss.py
--rw-rw-rw-   0        0        0     1713 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/nn/utils.py
--rw-rw-rw-   0        0        0    22426 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/token.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.635019 eznlp-0.2.3rc1/eznlp/training/
--rw-rw-rw-   0        0        0      511 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/training/__init__.py
--rw-rw-rw-   0        0        0     4231 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/training/evaluation.py
--rw-rw-rw-   0        0        0     3836 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/training/options.py
--rw-rw-rw-   0        0        0    15639 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/training/trainer.py
--rw-rw-rw-   0        0        0     6479 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/training/utils.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.650530 eznlp-0.2.3rc1/eznlp/utils/
--rw-rw-rw-   0        0        0      152 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/utils/__init__.py
--rw-rw-rw-   0        0        0     1478 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/utils/algorithms.py
--rw-rw-rw-   0        0        0     6245 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/utils/chunk.py
--rw-rw-rw-   0        0        0     2550 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/utils/segmentation.py
--rw-rw-rw-   0        0        0     8800 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/utils/transition.py
--rw-rw-rw-   0        0        0    16056 2021-08-27 08:08:41.000000 eznlp-0.2.3rc1/eznlp/utils/transition.xlsx
--rw-rw-rw-   0        0        0     5369 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/vectors.py
--rw-rw-rw-   0        0        0     1888 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/vocab.py
--rw-rw-rw-   0        0        0     4039 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/eznlp/wrapper.py
-drwxrwxrwx   0        0        0        0 2021-11-11 03:09:55.512942 eznlp-0.2.3rc1/eznlp.egg-info/
--rw-rw-rw-   0        0        0     4491 2021-11-11 03:09:54.000000 eznlp-0.2.3rc1/eznlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2014 2021-11-11 03:09:54.000000 eznlp-0.2.3rc1/eznlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-11 03:09:54.000000 eznlp-0.2.3rc1/eznlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      215 2021-11-11 03:09:54.000000 eznlp-0.2.3rc1/eznlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-11-11 03:09:54.000000 eznlp-0.2.3rc1/eznlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-11 03:09:55.651531 eznlp-0.2.3rc1/setup.cfg
--rw-rw-rw-   0        0        0     1582 2021-11-10 03:27:53.000000 eznlp-0.2.3rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.305938 eznlp-0.2.4/
+-rw-rw-rw-   0        0        0    11637 2022-06-22 07:04:30.000000 eznlp-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       73 2022-06-22 07:29:33.000000 eznlp-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4555 2023-05-11 01:04:38.304939 eznlp-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3376 2023-05-11 01:03:22.000000 eznlp-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.192312 eznlp-0.2.4/eznlp/
+-rw-rw-rw-   0        0        0      275 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/__init__.py
+-rw-rw-rw-   0        0        0     5419 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/config.py
+-rw-rw-rw-   0        0        0     7000 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/dataset.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.227939 eznlp-0.2.4/eznlp/io/
+-rw-rw-rw-   0        0        0      339 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/io/__init__.py
+-rw-rw-rw-   0        0        0     1010 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/io/base.py
+-rw-rw-rw-   0        0        0    18539 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/io/brat.py
+-rw-rw-rw-   0        0        0     1414 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/io/category_folder.py
+-rw-rw-rw-   0        0        0     1923 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/io/chip.py
+-rw-rw-rw-   0        0        0     6871 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/io/conll.py
+-rw-rw-rw-   0        0        0    13507 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/io/json.py
+-rw-rw-rw-   0        0        0     8893 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/io/processing.py
+-rw-rw-rw-   0        0        0     6296 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/io/raw_text.py
+-rw-rw-rw-   0        0        0     1892 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/io/src2trg.py
+-rw-rw-rw-   0        0        0     1661 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/io/tabular.py
+-rw-rw-rw-   0        0        0     5052 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.236938 eznlp-0.2.4/eznlp/model/
+-rw-rw-rw-   0        0        0      439 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/__init__.py
+-rw-rw-rw-   0        0        0    30733 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/bert_like.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.256938 eznlp-0.2.4/eznlp/model/decoder/
+-rw-rw-rw-   0        0        0      852 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/__init__.py
+-rw-rw-rw-   0        0        0     3817 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/model/decoder/base.py
+-rw-rw-rw-   0        0        0    12507 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/boundaries.py
+-rw-rw-rw-   0        0        0    12122 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/boundary_selection.py
+-rw-rw-rw-   0        0        0     9601 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/chunks.py
+-rw-rw-rw-   0        0        0    32582 2021-12-30 07:58:47.000000 eznlp-0.2.4/eznlp/model/decoder/generator.py
+-rw-rw-rw-   0        0        0     7847 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/joint_extraction.py
+-rw-rw-rw-   0        0        0     6592 2022-02-25 05:37:55.000000 eznlp-0.2.4/eznlp/model/decoder/sequence_tagging.py
+-rw-rw-rw-   0        0        0    10585 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/model/decoder/span_attr_classification.py
+-rw-rw-rw-   0        0        0    10978 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/span_classification.py
+-rw-rw-rw-   0        0        0    12483 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/span_rel_classification.py
+-rw-rw-rw-   0        0        0    10625 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/specific_span_classification.py
+-rw-rw-rw-   0        0        0    14310 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/specific_span_rel_classification.py
+-rw-rw-rw-   0        0        0    14140 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/decoder/specific_span_sparse_rel_classification.py
+-rw-rw-rw-   0        0        0     4125 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/model/decoder/text_classification.py
+-rw-rw-rw-   0        0        0     3841 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/model/elmo.py
+-rw-rw-rw-   0        0        0     8051 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/model/embedder.py
+-rw-rw-rw-   0        0        0    13161 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/model/encoder.py
+-rw-rw-rw-   0        0        0     4691 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/model/flair.py
+-rw-rw-rw-   0        0        0     4366 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/model/image_encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.265939 eznlp-0.2.4/eznlp/model/model/
+-rw-rw-rw-   0        0        0      301 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/model/__init__.py
+-rw-rw-rw-   0        0        0     2328 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/model/model/base.py
+-rw-rw-rw-   0        0        0     8353 2022-01-14 05:16:00.000000 eznlp-0.2.4/eznlp/model/model/classifier.py
+-rw-rw-rw-   0        0        0     9376 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/model/model/extractor.py
+-rw-rw-rw-   0        0        0     2789 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/model/model/image2text.py
+-rw-rw-rw-   0        0        0     5738 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/model/specific_span_extractor.py
+-rw-rw-rw-   0        0        0     2958 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/model/model/text2text.py
+-rw-rw-rw-   0        0        0     9256 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/model/nested_embedder.py
+-rw-rw-rw-   0        0        0     6013 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/model/span_bert_like.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.268938 eznlp-0.2.4/eznlp/nn/
+-rw-rw-rw-   0        0        0       49 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/nn/__init__.py
+-rw-rw-rw-   0        0        0    10412 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/nn/functional.py
+-rw-rw-rw-   0        0        0     7772 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/nn/init.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.280939 eznlp-0.2.4/eznlp/nn/modules/
+-rw-rw-rw-   0        0        0      539 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0     3258 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/nn/modules/aggregation.py
+-rw-rw-rw-   0        0        0    10264 2023-05-09 08:28:26.000000 eznlp-0.2.4/eznlp/nn/modules/attention.py
+-rw-rw-rw-   0        0        0     8266 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/nn/modules/block.py
+-rw-rw-rw-   0        0        0     7848 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/nn/modules/crf.py
+-rw-rw-rw-   0        0        0     2683 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/nn/modules/dropout.py
+-rw-rw-rw-   0        0        0      952 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/nn/modules/embedding.py
+-rw-rw-rw-   0        0        0     2207 2021-08-27 08:08:41.000000 eznlp-0.2.4/eznlp/nn/modules/loss.py
+-rw-rw-rw-   0        0        0     7421 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/nn/modules/query_bert_like.py
+-rw-rw-rw-   0        0        0     1713 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/nn/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.283939 eznlp-0.2.4/eznlp/plm/
+-rw-rw-rw-   0        0        0       95 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/plm/__init__.py
+-rw-rw-rw-   0        0        0     1063 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/plm/base.py
+-rw-rw-rw-   0        0        0     9650 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/plm/mlm.py
+-rw-rw-rw-   0        0        0    23695 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/token.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.290939 eznlp-0.2.4/eznlp/training/
+-rw-rw-rw-   0        0        0      553 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/training/__init__.py
+-rw-rw-rw-   0        0        0     5582 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/training/evaluation.py
+-rw-rw-rw-   0        0        0     3836 2023-03-24 09:23:24.000000 eznlp-0.2.4/eznlp/training/options.py
+-rw-rw-rw-   0        0        0     1020 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/training/plm_trainer.py
+-rw-rw-rw-   0        0        0    16007 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/training/trainer.py
+-rw-rw-rw-   0        0        0     6479 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/training/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.303939 eznlp-0.2.4/eznlp/utils/
+-rw-rw-rw-   0        0        0      152 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/utils/__init__.py
+-rw-rw-rw-   0        0        0     1478 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/utils/algorithms.py
+-rw-rw-rw-   0        0        0     6974 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/utils/chunk.py
+-rw-rw-rw-   0        0        0     2550 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/utils/segmentation.py
+-rw-rw-rw-   0        0        0     9635 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/utils/transition.py
+-rw-rw-rw-   0        0        0    19258 2022-03-08 06:39:08.000000 eznlp-0.2.4/eznlp/utils/transition.xlsx
+-rw-rw-rw-   0        0        0     5369 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/vectors.py
+-rw-rw-rw-   0        0        0     1888 2021-11-10 03:27:53.000000 eznlp-0.2.4/eznlp/vocab.py
+-rw-rw-rw-   0        0        0     4039 2023-05-11 01:03:22.000000 eznlp-0.2.4/eznlp/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-11 01:04:38.215937 eznlp-0.2.4/eznlp.egg-info/
+-rw-rw-rw-   0        0        0     4555 2023-05-11 01:04:36.000000 eznlp-0.2.4/eznlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2329 2023-05-11 01:04:36.000000 eznlp-0.2.4/eznlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 01:04:36.000000 eznlp-0.2.4/eznlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      215 2023-05-11 01:04:36.000000 eznlp-0.2.4/eznlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-11 01:04:36.000000 eznlp-0.2.4/eznlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 01:04:38.305938 eznlp-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-05-11 01:03:22.000000 eznlp-0.2.4/setup.py
```

### Comparing `eznlp-0.2.3rc1/LICENSE` & `eznlp-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/config.py` & `eznlp-0.2.4/eznlp/config.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/dataset.py` & `eznlp-0.2.4/eznlp/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
-from typing import List
+from typing import List, Any
+import random
 import torch
 
 from .nn.functional import seq_lens2mask
 from .wrapper import Batch
 from .model.model import ModelConfigBase
+from .plm import PreTrainingConfig
 
 
 class Dataset(torch.utils.data.Dataset):
-    def __init__(self, data: List[dict], config: ModelConfigBase=None, training: bool=True):
+    def __init__(self, data: List[dict], config: ModelConfigBase, training: bool=True):
         """
         Parameters
         ----------
         data : List[dict]
             Each entry (as a dict) follows the format of:
                 {'tokens': TokenSequence, 'label': str, 'chunks': List[tuple], 'relations': List[tuple], ...}
             where (1) `label` is a str (or int).  
@@ -124,7 +126,52 @@
             src_idx, trg_idx = self._indexing[i]
             entry = self.data[src_idx]
             # `trg_tokens` is a cache field
             entry['trg_tokens'] = entry['full_trg_tokens'][trg_idx]
             return entry
         else:
             return self.data[i]
+
+
+
+class PreTrainingDataset(torch.utils.data.Dataset):
+    """Dataset for Pre-training. 
+    """
+    def __init__(self, data: List[Any], config: PreTrainingConfig, training: bool=True, mp_rank=0, mp_world_size=0):
+        super().__init__()
+        # if mp_world_size > 0:
+        #     assert 0 <= mp_rank < mp_world_size
+            
+        #     text_paths = text_paths[_slice_chunk(mp_rank, mp_world_size, len(text_paths))]
+        # logger.info(f"Totally {len(text_paths)} text files in the {mp_rank}-th process")
+        
+        self.data = data
+        self.config = config
+        self.training = training
+        
+        
+    def __len__(self):
+        return len(self.data)
+        
+    @property
+    def summary(self):
+        summary = []
+        num_seqs = len(self.data)
+        summary.append(f"The dataset consists {num_seqs:,} sequences")
+        return "\n".join(summary)
+        
+        
+    def __getitem__(self, i):
+        entry = self.data[i]
+        
+        if getattr(self.config, 'paired_task', 'None').lower() == 'nsp':
+            paired_entry = random.choice(self.data)
+        else:
+            paired_entry = None
+        
+        example = self.config.exemplify(entry, paired_entry=paired_entry, training=self.training)
+        return example
+        
+        
+    def collate(self, batch_examples: List[str]):
+        batch = self.config.batchify(batch_examples)
+        return Batch(**batch)
```

### Comparing `eznlp-0.2.3rc1/eznlp/io/base.py` & `eznlp-0.2.4/eznlp/io/base.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/io/brat.py` & `eznlp-0.2.4/eznlp/io/brat.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/io/category_folder.py` & `eznlp-0.2.4/eznlp/io/category_folder.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/io/chip.py` & `eznlp-0.2.4/eznlp/io/chip.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/io/conll.py` & `eznlp-0.2.4/eznlp/io/conll.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,130 +4,126 @@
 from ..utils import ChunksTagsTranslator
 from .base import IO
 
 
 class ConllIO(IO):
     """An IO interface of CoNLL-format files. 
     
+    This reader will *break* the proceeding sequence and *skip* the current line starting with any of `sentence_sep_starts` and `document_sep_starts`. 
+    Hence, if you aim to ignore certain lines, you can place the corresponding "starting markers", if exist, in `sentence_sep_starts`. 
+    
     Parameters
     ----------
     sentence_sep_starts: List[str]
         * For OntoNotes (i.e., Conll2011, Conll2012), `sentence_sep_starts` should be `["#end", "pt/"]`
-        If `document_level` is False, it will *break* the proceeding sequence and *skip* the current line starting with any of `sentence_sep_starts`; 
-        else, it will *skip* the current line. 
     document_sep_starts: List[str]
         * For Conll2003, `document_sep_starts` should be `["-DOCSTART-"]`
         * For OntoNotes (i.e., Conll2011, Conll2012), `document_sep_starts` should be `["#begin"]`
-        Whether `document_level` is False or True, it will *break* the proceeding sequence and *skip* the current line starting with any of `sentence_sep_starts`.
     """
     def __init__(self, 
                  text_col_id=0, 
                  tag_col_id=1, 
                  sep=None, 
                  scheme='BIO1', 
-                 tag_sep='-',
+                 tag_sep='-', 
                  breaking_for_types=True, 
                  additional_col_id2name=None, 
                  sentence_sep_starts=None, 
-                 document_sep_starts=None,
-                 document_level: bool=False,
+                 document_sep_starts=None, 
                  encoding=None, 
                  verbose: bool=True, 
                  **token_kwargs):
         self.text_col_id = text_col_id
         self.tag_col_id = tag_col_id
         self.sep = sep
         
         self.tags_translator = ChunksTagsTranslator(scheme=scheme, sep=tag_sep, breaking_for_types=breaking_for_types)
         if additional_col_id2name is None:
             self.additional_col_id2name = {}
         else:
             assert all(isinstance(col_id, int) for col_id in additional_col_id2name.keys())
             assert all(isinstance(col_name, str) for col_name in additional_col_id2name.values())
             self.additional_col_id2name = additional_col_id2name
-            
+        
         assert sentence_sep_starts is None or all(isinstance(start, str) for start in sentence_sep_starts)
-        self.sentence_sep_starts = [] if sentence_sep_starts is None else sentence_sep_starts
+        self.sentence_sep_starts = sentence_sep_starts
         assert document_sep_starts is None or all(isinstance(start, str) for start in document_sep_starts)
-        self.document_sep_starts = [] if document_sep_starts is None else document_sep_starts
-        self.document_level = document_level
+        self.document_sep_starts = document_sep_starts
         super().__init__(is_tokenized=True, encoding=encoding, verbose=verbose, **token_kwargs)
         
         
     def read(self, file_path):
+        doc_idx = 0
         data = []
         with open(file_path, 'r', encoding=self.encoding) as f:
             text, tags = [], []
             additional = {col_id: [] for col_id in self.additional_col_id2name.keys()}
             
             _is_skipping_last = True
             for line in f:
                 line = line.strip()
                 
-                if self._is_breaking(line):
+                if self._is_document_seperator(line) or self._is_sentence_seperator(line):
                     if len(text) > 0:
                         additional_tags = {self.additional_col_id2name[col_id]: atags for col_id, atags in additional.items()}
                         tokens = self._build_tokens(text, additional_tags=additional_tags)
                         chunks = self.tags_translator.tags2chunks(tags)
-                        data.append({'tokens': tokens, 'chunks': chunks})
+                        data.append({'tokens': tokens, 'chunks': chunks, 'doc_idx': str(doc_idx)})
                         
                         text, tags = [], []
                         additional = {col_id: [] for col_id in self.additional_col_id2name.keys()}
+                    
+                    if self._is_document_seperator(line):
+                        # Empty documents will result in skipped indexes
+                        doc_idx += 1
+                    
                     _is_skipping_last = True
-                elif self._is_skipping(line):
-                    _is_skipping_last = True
+                    
                 else:
                     line_seperated = line.split(self.sep)
                     text.append(line_seperated[self.text_col_id])
                     tags.append(line_seperated[self.tag_col_id])
                     for col_id in self.additional_col_id2name.keys():
                         additional[col_id].append(line_seperated[col_id])
                     
                     # Fix for cases like ['I-ORG', '', 'I-ORG'], where the second is skipped. 
                     if (self.tags_translator.scheme == 'BIO1' 
                         and len(tags) >= 2 and tags[-1].startswith('I') and tags[-1][1:] == tags[-2][1:]
                         and _is_skipping_last):
                         tags[-1] = tags[-1].replace('I', 'B', 1)
-
+                    
                     _is_skipping_last = False
-                        
+            
             if len(text) > 0:
                 additional_tags = {self.additional_col_id2name[col_id]: atags for col_id, atags in additional.items()}
                 tokens = self._build_tokens(text, additional_tags=additional_tags)
                 chunks = self.tags_translator.tags2chunks(tags)
-                data.append({'tokens': tokens, 'chunks': chunks})
-            
+                data.append({'tokens': tokens, 'chunks': chunks, 'doc_idx': str(doc_idx)})
+        
         return data
-    
-    
+        
+        
     def _is_sentence_seperator(self, line: str):
         if line.strip() == "":
             return True
+        if self.sentence_sep_starts is None:
+            return False
         for start in self.sentence_sep_starts:
             if line.startswith(start):
                 return True
         return False
-
+        
     def _is_document_seperator(self, line: str):
+        if self.document_sep_starts is None:
+            return False
         for start in self.document_sep_starts:
             if line.startswith(start):
                 return True
         return False
-
-    def _is_breaking(self, line: str):
-        if self._is_document_seperator(line):
-            return True
-        if (not self.document_level) and self._is_sentence_seperator(line):
-            return True
-        return False
-
-    def _is_skipping(self, line: str):
-        return self._is_document_seperator(line) or self._is_sentence_seperator(line)
-
-
+        
     def flatten_to_characters(self, data: list):
         additional_keys = [key for key in data[0]['tokens'][0].__dict__.keys() if key not in ('text', 'raw_text')]
         
         new_data = []
         for entry in data:
             tokenized_raw_text = entry['tokens'].raw_text
             char_seq_lens = [len(tok) for tok in tokenized_raw_text]
```

### Comparing `eznlp-0.2.3rc1/eznlp/io/json.py` & `eznlp-0.2.4/eznlp/io/json.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     filtered_tuples = []
     for tp in tuples:
         if tp not in filtered_tuples:
             filtered_tuples.append(tp)
     return filtered_tuples
 
 
+# TODO: rename as InfoExIO?
 class JsonIO(IO):
     """An IO Interface of Json files. 
     
     """
     def __init__(self, 
                  is_tokenized: bool=True, 
                  tokenize_callback=None, 
@@ -36,41 +37,44 @@
                  attribute_chunk_key=None, 
                  relation_key=None, 
                  relation_type_key=None, 
                  relation_head_key=None, 
                  relation_tail_key=None, 
                  drop_duplicated=True, 
                  is_whole_piece: bool=True, 
+                 retain_keys: list=None, 
                  encoding=None, 
                  verbose: bool=True, 
                  **token_kwargs):
         self.text_key = text_key
         self.chunk_key = chunk_key
         self.chunk_type_key = chunk_type_key
         self.chunk_start_key = chunk_start_key
         self.chunk_end_key = chunk_end_key
         self.chunk_text_key = chunk_text_key
-
+        
         if all(key is not None for key in [attribute_key, attribute_type_key, attribute_chunk_key]):
             self.attribute_key = attribute_key
             self.attribute_type_key = attribute_type_key
             self.attribute_chunk_key = attribute_chunk_key
         else:
             self.attribute_key = None
-
+        
         if all(key is not None for key in [relation_key, relation_type_key, relation_head_key, relation_tail_key]):
             self.relation_key = relation_key
             self.relation_type_key = relation_type_key
             self.relation_head_key = relation_head_key
             self.relation_tail_key = relation_tail_key
         else:
             self.relation_key = None
         
         self.drop_duplicated = drop_duplicated
         self.is_whole_piece = is_whole_piece
+        self.retain_keys = [] if retain_keys is None else retain_keys
+        assert all(key not in self.retain_keys for key in [self.text_key, self.chunk_key, self.relation_key, self.attribute_key])
         
         super().__init__(is_tokenized=is_tokenized, tokenize_callback=tokenize_callback, encoding=encoding, verbose=verbose, **token_kwargs)
         if not self.is_tokenized:
             self.text_translator = TextChunksTranslator()
         
         
     def read(self, file_path, return_errors: bool=False):
@@ -98,39 +102,40 @@
             
             entry = {'tokens': tokens, 'chunks': [ck for ck in chunks if ck is not None]}
             
             if self.attribute_key is not None:
                 attributes = [(attr[self.attribute_type_key], 
                                chunks[attr[self.attribute_chunk_key]]) for attr in raw_entry[self.attribute_key]]
                 entry.update({'attributes': [(attr_type, ck) for attr_type, ck in attributes if ck is not None]})
-
+            
             if self.relation_key is not None:
                 relations = [(rel[self.relation_type_key], 
                               chunks[rel[self.relation_head_key]], 
                               chunks[rel[self.relation_tail_key]]) for rel in raw_entry[self.relation_key]]
                 entry.update({'relations': [(rel_type, head, tail) for rel_type, head, tail in relations if head is not None and tail is not None]})
-                
+            
             if self.drop_duplicated:
                 entry['chunks'] = _filter_duplicated(entry['chunks'])
                 if self.attribute_key is not None:
                     entry['attributes'] = _filter_duplicated(entry['attributes'])
                 if self.relation_key is not None:
                     entry['relations'] = _filter_duplicated(entry['relations'])
-
-            data.append(entry)
             
+            entry.update({k:v for k, v in raw_entry.items() if k in self.retain_keys})
+            data.append(entry)
+        
         if len(errors) > 0 or len(mismatches) > 0:
             logger.warning(f"{len(errors)} errors and {len(mismatches)} mismatches detected during parsing {file_path}")
         
         if return_errors:
             return data, errors, mismatches
         else:
             return data
-
-
+        
+        
     def write(self, data: List[dict], file_path):
         raw_data = []
         for entry in data:
             raw_entry = {self.text_key: entry['tokens'].raw_text}
             
             chunk2idx = {ck: k for k, ck in enumerate(entry['chunks'])}
             raw_entry[self.chunk_key] = [{self.chunk_type_key: chunk_type, 
@@ -139,22 +144,24 @@
             if self.attribute_key is not None:
                 raw_entry[self.attribute_key] = [{self.attribute_type_key: attr_type, 
                                                   self.attribute_chunk_key: chunk2idx[ck]} for attr_type, ck in entry['attributes']]
             if self.relation_key is not None:
                 raw_entry[self.relation_key] = [{self.relation_type_key: rel_type, 
                                                  self.relation_head_key: chunk2idx[head], 
                                                  self.relation_tail_key: chunk2idx[tail]} for rel_type, head, tail in entry['relations']]
+            
+            raw_entry.update({k: v for k, v in entry.items() if k in self.retain_keys})
             raw_data.append(raw_entry)
-
+        
         with open(file_path, 'w', encoding=self.encoding) as f:
             if self.is_whole_piece:
-                json.dump(raw_data, f)
+                json.dump(raw_data, f, ensure_ascii=False)
             else:
                 for raw_entry in raw_data:
-                    f.write(json.dumps(raw_entry))
+                    f.write(json.dumps(raw_entry, ensure_ascii=False))
                     f.write("\n")
 
 
 
 class SQuADIO(IO):
     """An IO Interface of SQuAD files. 
     
@@ -229,7 +236,63 @@
                 dev_data.append(entry)
             elif raw_entry['split'].lower().startswith('test'):
                 test_data.append(entry)
             else:
                 train_data.append(entry)
         
         return train_data, dev_data, test_data
+
+
+
+class TextClsIO(IO):
+    """An IO interface of (single or paired) text classification dataset in json files. 
+    
+    """
+    def __init__(self, 
+                 is_tokenized: bool=False, 
+                 tokenize_callback=None, 
+                 text_key: str='text', 
+                 paired_text_key: str=None, 
+                 label_key='label', 
+                 is_whole_piece: bool=True, 
+                 retain_keys: list=None, 
+                 mapping=None, 
+                 encoding=None, 
+                 verbose: bool=True, 
+                 **token_kwargs):
+        self.text_key = text_key
+        self.paired_text_key = paired_text_key
+        self.label_key = label_key
+        self.is_whole_piece = is_whole_piece
+        self.retain_keys = [] if retain_keys is None else retain_keys
+        assert all(key not in self.retain_keys for key in [self.text_key, self.paired_text_key, self.label_key])
+        self.mapping = {} if mapping is None else mapping
+        super().__init__(is_tokenized=is_tokenized, tokenize_callback=tokenize_callback, encoding=encoding, verbose=verbose, **token_kwargs)
+        
+        
+    def read(self, file_path):
+        with open(file_path, 'r', encoding=self.encoding) as f:
+            if self.is_whole_piece:
+                raw_data = json.load(f)
+            else:
+                raw_data = [json.loads(line) for line in f if len(line.strip()) > 0]
+        
+        data = []
+        for raw_entry in raw_data:
+            raw_text = raw_entry[self.text_key]
+            for pattern, repl in self.mapping.items():
+                raw_text = raw_text.replace(pattern, repl)
+            entry = {'tokens': self._build_tokens(raw_text)}
+            
+            if self.paired_text_key is not None:
+                paired_raw_text = raw_entry[self.paired_text_key]
+                for pattern, repl in self.mapping.items():
+                    paired_raw_text = paired_raw_text.replace(pattern, repl)
+                entry.update({'paired_tokens': self._build_tokens(paired_raw_text)})
+            
+            if self.label_key in raw_entry:
+                entry.update({'label': raw_entry[self.label_key]})
+            
+            entry.update({k:v for k, v in raw_entry.items() if k in self.retain_keys})
+            data.append(entry)
+        
+        return data
```

### Comparing `eznlp-0.2.3rc1/eznlp/io/processing.py` & `eznlp-0.2.4/eznlp/io/processing.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/io/src2trg.py` & `eznlp-0.2.4/eznlp/io/src2trg.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/io/tabular.py` & `eznlp-0.2.4/eznlp/io/tabular.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/metrics.py` & `eznlp-0.2.4/eznlp/metrics.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/__init__.py` & `eznlp-0.2.4/eznlp/model/decoder/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,9 +5,12 @@
 
 from .sequence_tagging import SequenceTaggingDecoderConfig
 from .span_classification import SpanClassificationDecoderConfig
 from .span_attr_classification import SpanAttrClassificationDecoderConfig
 from .span_rel_classification import SpanRelClassificationDecoderConfig
 from .boundary_selection import BoundarySelectionDecoderConfig
 from .joint_extraction import JointExtractionDecoderConfig
+from .specific_span_classification import SpecificSpanClsDecoderConfig
+from .specific_span_rel_classification import SpecificSpanRelClsDecoderConfig
+from .specific_span_sparse_rel_classification import SpecificSpanSparseRelClsDecoderConfig
 
 from .generator import GeneratorConfig
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/base.py` & `eznlp-0.2.4/eznlp/model/decoder/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 
 
 class SingleDecoderConfigBase(Config):
     def __init__(self, **kwargs):
         self.in_dim = kwargs.pop('in_dim', None)
         
-        # gamma set as 0 for cross entropy loss, 2.0 for focal loss by default
+        # focal loss `gamma`: 0 fallback to cross entropy
         self.fl_gamma = kwargs.pop('fl_gamma', 0.0) 
-        # epsilon set as 0 for cross entropy loss, 0.1 for label smoothing loss by default
+        # label smoothing `epsilon`: 0 fallback to cross entropy
         self.sl_epsilon = kwargs.pop('sl_epsilon', 0.0)
         super().__init__(**kwargs)
         
     @property
     def criterion(self):
         if getattr(self, 'multihot', False):
             return "BCE"
@@ -85,14 +85,18 @@
         
     def forward(self, batch: Batch, **states):
         raise NotImplementedError("Not Implemented `forward`")
         
     def decode(self, batch: Batch, **states):
         raise NotImplementedError("Not Implemented `decode`")
         
+    # TODO: Loosely decoding
+    def loosely_decode(self, batch: Batch, **states):
+        return self.decode(batch, **states)
+        
     def _unsqueezed_decode(self, batch: Batch, **states):
         if self.num_metrics == 0:
             raise RuntimeError("`_unsqueezed` method does not applies if `num_metrics` is 0")
         elif self.num_metrics == 1:
             return (self.decode(batch, **states), )
         else:
             return self.decode(batch, **states)
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/boundary_selection.py` & `eznlp-0.2.4/eznlp/model/decoder/specific_span_rel_classification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # -*- coding: utf-8 -*-
-from typing import List, Tuple
+from typing import List, Dict
 from collections import Counter
 import logging
+import math
+import numpy
 import torch
 
-from ...wrapper import TargetWrapper, Batch
-from ...utils.chunk import detect_nested, filter_clashed_by_priority
-from ...nn.modules import CombinedDropout, SoftLabelCrossEntropyLoss
+from ...wrapper import Batch
+from ...nn.modules import CombinedDropout
 from ...nn.init import reinit_embedding_, reinit_layer_
 from ...metrics import precision_recall_f1_report
 from ..encoder import EncoderConfig
 from .base import DecoderMixinBase, SingleDecoderConfigBase, DecoderBase
+from .boundaries import DiagBoundariesPairs, MAX_SIZE_ID_COV_RATE, _span_pairs_from_diagonals
 
 logger = logging.getLogger(__name__)
 
 
-class BoundarySelectionDecoderMixin(DecoderMixinBase):
+
+class DiagBoundariesPairsDecoderMixin(DecoderMixinBase):
+    """A `Mixin` for relation extraction. 
+    """
     @property
     def idx2label(self):
         return self._idx2label
         
     @idx2label.setter
     def idx2label(self, idx2label: List[str]):
         self._idx2label = idx2label
@@ -29,306 +34,255 @@
     def voc_dim(self):
         return len(self.label2idx)
         
     @property
     def none_idx(self):
         return self.label2idx[self.none_label]
         
-    def exemplify(self, data_entry: dict, training: bool=True):
-        return {'boundaries_obj': Boundaries(data_entry, self, training=training)}
+    @property
+    def idx2ck_label(self):
+        return self._idx2ck_label
+        
+    @idx2ck_label.setter
+    def idx2ck_label(self, idx2ck_label: List[str]):
+        self._idx2ck_label = idx2ck_label
+        self.ck_label2idx = {l: i for i, l in enumerate(idx2ck_label)} if idx2ck_label is not None else None
+        
+    @property
+    def ck_voc_dim(self):
+        return len(self.ck_label2idx)
+        
+    @property
+    def ck_none_idx(self):
+        return self.ck_label2idx[self.ck_none_label]
+        
+    def exemplify(self, entry: dict, training: bool=True):
+        return {'dbp_obj': DiagBoundariesPairs(entry, self, training=training)}
         
     def batchify(self, batch_examples: List[dict]):
-        return {'boundaries_objs': [ex['boundaries_obj'] for ex in batch_examples]}
+        return {'dbp_objs': [ex['dbp_obj'] for ex in batch_examples]}
         
     def retrieve(self, batch: Batch):
-        return [boundaries_obj.chunks for boundaries_obj in batch.boundaries_objs]
+        return [dbp_obj.relations for dbp_obj in batch.dbp_objs]
         
     def evaluate(self, y_gold: List[List[tuple]], y_pred: List[List[tuple]]):
-        """Micro-F1 for entity recognition. 
-        
-        References
-        ----------
-        https://www.clips.uantwerpen.be/conll2000/chunking/output.html
-        """
         scores, ave_scores = precision_recall_f1_report(y_gold, y_pred)
         return ave_scores['micro']['f1']
 
 
-def _spans_from_surrounding(span: Tuple[int], distance: int, num_tokens: int):
-    """Spans from the surrounding area of the given `span`.
-    """
-    for k in range(distance):
-        for start_offset, end_offset in [(-k, -distance+k), 
-                                         (-distance+k, k), 
-                                         (k, distance-k), 
-                                         (distance-k, -k)]:
-            start, end = span[0]+start_offset, span[1]+end_offset
-            if 0 <= start < end <= num_tokens:
-                yield (start, end)
-
-
-def _spans_from_upper_triangular(seq_len: int):
-    """Spans from the upper triangular area. 
-    """
-    for start in range(seq_len):
-        for end in range(start+1, seq_len+1):
-            yield (start, end)
-
-
-class Boundaries(TargetWrapper):
-    """A wrapper of boundaries with underlying chunks. 
-    
-    Parameters
-    ----------
-    data_entry: dict
-        {'tokens': TokenSequence, 
-         'chunks': List[tuple]}
-    """
-    def __init__(self, data_entry: dict, config: BoundarySelectionDecoderMixin, training: bool=True):
-        super().__init__(training)
-        
-        self.chunks = data_entry.get('chunks', None)
-        num_tokens = len(data_entry['tokens'])
-        
-        if training and config.neg_sampling_rate < 1:
-            non_mask = (torch.arange(num_tokens) - torch.arange(num_tokens).unsqueeze(-1) >= 0)
-            pos_non_mask = torch.zeros_like(non_mask)
-            for label, start, end in self.chunks:
-                pos_non_mask[start, end-1] = True
-            
-            neg_sampled = torch.empty_like(non_mask).bernoulli(p=config.neg_sampling_rate)
-            
-            if config.hard_neg_sampling_rate > config.neg_sampling_rate:
-                hard_neg_non_mask = torch.zeros_like(non_mask)
-                for label, start, end in self.chunks:
-                    for dist in range(1, config.hard_neg_sampling_size+1):
-                        for sur_start, sur_end in _spans_from_surrounding((start, end), dist, num_tokens):
-                            hard_neg_non_mask[sur_start, sur_end-1] = True
-                
-                if config.hard_neg_sampling_rate < 1:
-                    # Solve: 1 - (1 - p_{neg})(1 - p_{comp}) = p_{hard}
-                    # Get: p_{comp} = (p_{hard} - p_{neg}) / (1 - p_{neg})
-                    comp_sampling_rate = (config.hard_neg_sampling_rate - config.neg_sampling_rate) / (1 - config.neg_sampling_rate)
-                    comp_sampled = torch.empty_like(non_mask).bernoulli(p=comp_sampling_rate)
-                    neg_sampled = neg_sampled | (comp_sampled & hard_neg_non_mask)
-                else:
-                    neg_sampled = neg_sampled | hard_neg_non_mask
-            
-            self.non_mask = pos_non_mask | (neg_sampled & non_mask)
-        
-        if self.chunks is not None:
-            if config.sb_epsilon <= 0 and config.sl_epsilon <= 0:
-                # Cross entropy loss
-                self.boundary2label_id = torch.full((num_tokens, num_tokens), config.none_idx, dtype=torch.long)
-                for label, start, end in self.chunks:
-                    self.boundary2label_id[start, end-1] = config.label2idx[label]
-            else:
-                # Soft label loss for either boundary or label smoothing 
-                self.boundary2label_id = torch.zeros(num_tokens, num_tokens, config.voc_dim, dtype=torch.float)
-                for label, start, end in self.chunks:
-                    label_id = config.label2idx[label]
-                    self.boundary2label_id[start, end-1, label_id] += (1 - config.sb_epsilon)
-                    
-                    for dist in range(1, config.sb_size+1):
-                        eps_per_span = config.sb_epsilon / (config.sb_size * dist * 4)
-                        sur_spans = list(_spans_from_surrounding((start, end), dist, num_tokens))
-                        for sur_start, sur_end in sur_spans:
-                            self.boundary2label_id[sur_start, sur_end-1, label_id] += (eps_per_span*config.sb_adj_factor)
-                        # Absorb the probabilities assigned to illegal positions
-                        self.boundary2label_id[start, end-1, label_id] += eps_per_span * (dist * 4 - len(sur_spans))
-                
-                # In very rare cases (e.g., ACE 2005), multiple entities may have the same span but different types
-                overflow_indic = (self.boundary2label_id.sum(dim=-1) > 1)
-                if overflow_indic.any().item():
-                    self.boundary2label_id[overflow_indic] = torch.nn.functional.normalize(self.boundary2label_id[overflow_indic], p=1, dim=-1)
-                self.boundary2label_id[:, :, config.none_idx] = 1 - self.boundary2label_id.sum(dim=-1)
-                
-                if config.sl_epsilon > 0:
-                    # Do not smooth to `<none>` label
-                    pos_indic = (torch.arange(config.voc_dim) != config.none_idx)
-                    self.boundary2label_id[:, :, pos_indic] = (self.boundary2label_id[:, :, pos_indic] * (1-config.sl_epsilon) + 
-                                                               self.boundary2label_id[:, :, pos_indic].sum(dim=-1, keepdim=True)*config.sl_epsilon / (config.voc_dim-1))
 
-
-
-class BoundarySelectionDecoderConfig(SingleDecoderConfigBase, BoundarySelectionDecoderMixin):
+class SpecificSpanRelClsDecoderConfig(SingleDecoderConfigBase, DiagBoundariesPairsDecoderMixin):
     def __init__(self, **kwargs):
         self.use_biaffine = kwargs.pop('use_biaffine', True)
         self.affine = kwargs.pop('affine', EncoderConfig(arch='FFN', hid_dim=150, num_layers=1, in_drop_rates=(0.4, 0.0, 0.0), hid_drop_rate=0.2))
         
+        self.max_span_size_ceiling = kwargs.pop('max_span_size_ceiling', 20)
+        self.max_span_size_cov_rate = kwargs.pop('max_span_size_cov_rate', 0.995)
+        self.max_span_size = kwargs.pop('max_span_size', None)
         self.max_len = kwargs.pop('max_len', None)
-        self.max_span_size = kwargs.pop('max_span_size', 50)
         self.size_emb_dim = kwargs.pop('size_emb_dim', 25)
         self.hid_drop_rates = kwargs.pop('hid_drop_rates', (0.2, 0.0, 0.0))
         
         self.neg_sampling_rate = kwargs.pop('neg_sampling_rate', 1.0)
-        self.hard_neg_sampling_rate = kwargs.pop('hard_neg_sampling_rate', 1.0)
-        self.hard_neg_sampling_rate = max(self.hard_neg_sampling_rate, self.neg_sampling_rate)
-        self.hard_neg_sampling_size = kwargs.pop('hard_neg_sampling_size', 5)
+        # self.neg_sampling_power_decay = kwargs.pop('neg_sampling_power_decay', 0.0)  # decay = 0.5, 1.0
+        # self.neg_sampling_surr_rate = kwargs.pop('neg_sampling_surr_rate', 0.0)
+        # self.neg_sampling_surr_size = kwargs.pop('neg_sampling_surr_size', 5)
         
         self.none_label = kwargs.pop('none_label', '<none>')
         self.idx2label = kwargs.pop('idx2label', None)
-        # Note: non-nested overlapping chunks are never allowed
-        self.allow_nested = kwargs.pop('allow_nested', None)
-        
-        # Boundary smoothing epsilon
-        self.sb_epsilon = kwargs.pop('sb_epsilon', 0.0)
-        self.sb_size = kwargs.pop('sb_size', 1)
-        self.sb_adj_factor = kwargs.pop('sb_adj_factor', 1.0)
+        self.ck_none_label = kwargs.pop('ck_none_label', '<none>')
+        self.idx2ck_label = kwargs.pop('idx2ck_label', None)
+        self.filter_by_labels = kwargs.pop('filter_by_labels', True)
+        self.filter_self_relation = kwargs.pop('filter_self_relation', True)
         super().__init__(**kwargs)
         
-        
     @property
     def name(self):
-        return self._name_sep.join([self.affine.arch, self.criterion])
+        return self.criterion
         
     def __repr__(self):
         repr_attr_dict = {key: getattr(self, key) for key in ['in_dim', 'hid_drop_rates', 'criterion']}
         return self._repr_non_config_attrs(repr_attr_dict)
         
     @property
     def in_dim(self):
-        return self.affine.in_dim
+        return self.affine.in_dim - self.size_emb_dim
         
     @in_dim.setter
     def in_dim(self, dim: int):
-        self.affine.in_dim = dim
-        
-    @property
-    def criterion(self):
-        if self.sb_epsilon > 0:
-            return f"SB({self.sb_epsilon:.2f}, {self.sb_size})"
-        else:
-            return super().criterion
-        
-    def instantiate_criterion(self, **kwargs):
-        if self.criterion.lower().startswith(('sb', 'sl')):
-            # For boundary/label smoothing, the `Boundaries` object has been accordingly changed; 
-            # hence, do not use `SmoothLabelCrossEntropyLoss`
-            return SoftLabelCrossEntropyLoss(**kwargs)
-        else:
-            return super().instantiate_criterion(**kwargs)
-        
+        if dim is not None:
+            self.affine.in_dim = dim + self.size_emb_dim
         
     def build_vocab(self, *partitions):
         counter = Counter(label for data in partitions for entry in data for label, start, end in entry['chunks'])
-        self.idx2label = [self.none_label] + list(counter.keys())
+        self.idx2ck_label = [self.ck_none_label] + list(counter.keys())
         
-        self.allow_nested = any(detect_nested(entry['chunks']) for data in partitions for entry in data)
-        if self.allow_nested:
-            logger.info("Nested chunks detected, nested chunks are allowed in decoding...")
-        else:
-            logger.info("No nested chunks detected, only flat chunks are allowed in decoding...")
+        # Calculate `max_span_size` according to data
+        span_sizes = [end-start for data in partitions for entry in data for label, start, end in entry['chunks']]
+        # Allow directly setting `max_span_size`
+        if self.max_span_size is None:
+            if self.max_span_size_cov_rate >= 1:
+                span_size_cov = max(span_sizes)
+            else:
+                span_size_cov = math.ceil(numpy.quantile(span_sizes, self.max_span_size_cov_rate))
+            self.max_span_size = min(span_size_cov, self.max_span_size_ceiling)
+        self.max_size_id = min(math.ceil(numpy.quantile(span_sizes, MAX_SIZE_ID_COV_RATE)), self.max_span_size) - 1
+        logger.warning(f"The `max_span_size` is set to {self.max_span_size}")
+        
+        size_counter = Counter(end-start for data in partitions for entry in data for label, start, end in entry['chunks'])
+        num_spans = sum(size_counter.values())
+        num_oov_spans = sum(num for size, num in size_counter.items() if size > self.max_span_size)
+        if num_oov_spans > 0:
+            logger.warning(f"OOV positive spans: {num_oov_spans} ({num_oov_spans/num_spans*100:.2f}%)")
         
         self.max_len = max(len(data_entry['tokens']) for data in partitions for data_entry in data)
         
+        counter = Counter(label for data in partitions for entry in data for label, head, tail in entry['relations'])
+        self.idx2label = [self.none_label] + list(counter.keys())
+        
+        counter = Counter((label, head[0], tail[0]) for data in partitions for entry in data for label, head, tail in entry['relations'])
+        self.existing_rht_labels = set(list(counter.keys()))
+        self.existing_self_relation = any(head[1:]==tail[1:] for data in partitions for entry in data for label, head, tail in entry['relations'])
+        
         
     def instantiate(self):
-        return BoundarySelectionDecoder(self)
-
+        return SpecificSpanRelClsDecoder(self)
 
 
 
-class BoundarySelectionDecoder(DecoderBase, BoundarySelectionDecoderMixin):
-    def __init__(self, config: BoundarySelectionDecoderConfig):
+class SpecificSpanRelClsDecoder(DecoderBase, DiagBoundariesPairsDecoderMixin):
+    def __init__(self, config: SpecificSpanRelClsDecoderConfig):
         super().__init__()
+        self.max_span_size = config.max_span_size
+        self.neg_sampling_rate = config.neg_sampling_rate
         self.none_label = config.none_label
         self.idx2label = config.idx2label
-        self.allow_nested = config.allow_nested
+        self.ck_none_label = config.ck_none_label
+        self.idx2ck_label = config.idx2ck_label
+        self.filter_by_labels = config.filter_by_labels
+        self.existing_rht_labels = config.existing_rht_labels
+        self.filter_self_relation = config.filter_self_relation
+        self.existing_self_relation = config.existing_self_relation
         
         if config.use_biaffine:
-            self.affine_start = config.affine.instantiate()
-            self.affine_end = config.affine.instantiate()
+            self.affine_head = config.affine.instantiate()
+            self.affine_tail = config.affine.instantiate()
         else:
             self.affine = config.affine.instantiate()
         
+        # TODO: Representations of context between head/tail entities
+        # TODO: Chunk type embedding, only for positive (entity) spans? 
         if config.size_emb_dim > 0:
-            self.size_embedding = torch.nn.Embedding(config.max_span_size, config.size_emb_dim)
+            self.size_embedding = torch.nn.Embedding(config.max_size_id+1, config.size_emb_dim)
             reinit_embedding_(self.size_embedding)
         
-        # Use buffer to accelerate computation
-        # Note: size_id = size - 1
         self.register_buffer('_span_size_ids', torch.arange(config.max_len) - torch.arange(config.max_len).unsqueeze(-1))
-        # Create `_span_non_mask` before changing values of `_span_size_ids`
-        self.register_buffer('_span_non_mask', self._span_size_ids >= 0)
         self._span_size_ids.masked_fill_(self._span_size_ids < 0, 0)
-        self._span_size_ids.masked_fill_(self._span_size_ids >= config.max_span_size, config.max_span_size-1)
+        self._span_size_ids.masked_fill_(self._span_size_ids > config.max_size_id, config.max_size_id)
         
         self.dropout = CombinedDropout(*config.hid_drop_rates)
         
         self.U = torch.nn.Parameter(torch.empty(config.voc_dim, config.affine.out_dim, config.affine.out_dim))
-        self.W = torch.nn.Parameter(torch.empty(config.voc_dim, config.affine.out_dim*2 + config.size_emb_dim))
+        self.W = torch.nn.Parameter(torch.empty(config.voc_dim, config.affine.out_dim*2))
         self.b = torch.nn.Parameter(torch.empty(config.voc_dim))
         torch.nn.init.orthogonal_(self.U.data)
         torch.nn.init.orthogonal_(self.W.data)
         torch.nn.init.zeros_(self.b.data)
         
         self.criterion = config.instantiate_criterion(reduction='sum')
         
         
-    def _get_span_size_ids(self, seq_len: int):
-        return self._span_size_ids[:seq_len, :seq_len]
-        
-    def _get_span_non_mask(self, seq_len: int):
-        return self._span_non_mask[:seq_len, :seq_len]
-        
-        
-    def compute_scores(self, batch: Batch, full_hidden: torch.Tensor):
-        if hasattr(self, 'affine_start'):
-            affined_start = self.affine_start(full_hidden, batch.mask)
-            affined_end = self.affine_end(full_hidden, batch.mask)
-        else:
-            affined_start = self.affine(full_hidden, batch.mask)
-            affined_end = self.affine(full_hidden, batch.mask)
+    def assign_chunks_pred(self, batch: Batch, batch_chunks_pred: List[List[tuple]]):
+        """This method should be called on-the-fly for joint modeling. 
+        """
+        for dbp_obj, chunks_pred in zip(batch.dbp_objs, batch_chunks_pred):
+            if dbp_obj.chunks_pred is None:
+                dbp_obj.chunks_pred = chunks_pred
+                dbp_obj.build(self)
+                dbp_obj.to(self.W.device)
+        
+        
+    def _get_diagonal_span_size_ids(self, seq_len: int, max_span_size: int):
+        span_size_ids = self._span_size_ids[:seq_len, :seq_len]
+        return torch.cat([span_size_ids.diagonal(offset=k-1) for k in range(1, max_span_size+1)], dim=-1)
+        
+        
+    def compute_scores(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
+        # full_hidden: (batch, step, hid_dim)
+        # query_hidden: (batch, step-k+1, hid_dim)
+        all_hidden = [full_hidden] + list(all_query_hidden.values())
+        
+        batch_scores = []
+        for i, curr_len in enumerate(batch.seq_lens.cpu().tolist()):
+            curr_max_span_size = min(self.max_span_size, curr_len)
+            
+            # (curr_len-k+1, hid_dim) -> (num_spans = \sum_k curr_len-k+1, hid_dim)
+            span_hidden = torch.cat([all_hidden[k-1][i, :curr_len-k+1] for k in range(1, curr_max_span_size+1)], dim=0)
+            
+            if hasattr(self, 'size_embedding'):
+                # size_embedded: (num_spans, emb_dim)
+                size_embedded = self.size_embedding(self._get_diagonal_span_size_ids(curr_len, curr_max_span_size))
+                span_hidden = torch.cat([span_hidden, size_embedded], dim=-1)
+            
+            if hasattr(self, 'affine_head'):
+                # No mask input needed here
+                affined_head = self.affine_head(span_hidden)
+                affined_tail = self.affine_tail(span_hidden)
+            else:
+                affined_head = self.affine(span_hidden)
+                affined_tail = self.affine(span_hidden)
+            
+            # scores1: (head_spans, affine_dim) * (voc_dim, affine_dim, affine_dim) * (affine_dim, tail_spans) -> (voc_dim, head_spans, tail_spans)
+            scores1 = self.dropout(affined_head).matmul(self.U).matmul(self.dropout(affined_tail.permute(1, 0)))
+            
+            # affined_cat: (head_spans, tail_spans, affine_dim*2)
+            affined_cat = torch.cat([self.dropout(affined_head).unsqueeze(1).expand(-1, affined_tail.size(0), -1), 
+                                     self.dropout(affined_tail).unsqueeze(0).expand(affined_head.size(0), -1, -1)], dim=-1)
+            
+            # scores2: (voc_dim, affine_dim*2) * (head_spans, tail_spans, affine_dim*2, 1) -> (head_spans, tail_spans, voc_dim, 1) 
+            scores2 = self.W.matmul(affined_cat.unsqueeze(-1))
+            # scores: (head_spans, tail_spans, voc_dim)
+            scores = scores1.permute(1, 2, 0) + scores2.squeeze(-1) + self.b
+            batch_scores.append(scores)
         
-        # affined_start: (batch, start_step, affine_dim) -> (batch, 1, start_step, affine_dim)
-        # affined_end: (batch, end_step, affine_dim) -> (batch, 1, affine_dim, end_step)
-        # scores1: (batch, 1, start_step, affine_dim) * (voc_dim, affine_dim, affine_dim) * (batch, 1, affine_dim, end_step) -> (batch, voc_dim, start_step, end_step)
-        scores1 = self.dropout(affined_start).unsqueeze(1).matmul(self.U).matmul(self.dropout(affined_end).permute(0, 2, 1).unsqueeze(1))
-        
-        # affined_cat: (batch, start_step, end_step, affine_dim*2)
-        affined_cat = torch.cat([self.dropout(affined_start).unsqueeze(2).expand(-1, -1, affined_end.size(1), -1), 
-                                 self.dropout(affined_end).unsqueeze(1).expand(-1, affined_start.size(1), -1, -1)], dim=-1)
-        
-        if hasattr(self, 'size_embedding'):
-            # size_embedded: (start_step, end_step, emb_dim)
-            size_embedded = self.size_embedding(self._get_span_size_ids(full_hidden.size(1)))
-            # affined_cat: (batch, start_step, end_step, affine_dim*2 + emb_dim)
-            affined_cat = torch.cat([affined_cat, self.dropout(size_embedded).unsqueeze(0).expand(full_hidden.size(0), -1, -1, -1)], dim=-1)
-        
-        # scores2: (voc_dim, affine_dim*2 + emb_dim) * (batch, start_step, end_step, affine_dim*2 + emb_dim, 1) -> (batch, start_step, end_step, voc_dim, 1)
-        scores2 = self.W.matmul(affined_cat.unsqueeze(-1))
-        # scores: (batch, start_step, end_step, voc_dim)
-        return scores1.permute(0, 2, 3, 1) + scores2.squeeze(-1) + self.b
+        return batch_scores
         
         
-    def forward(self, batch: Batch, full_hidden: torch.Tensor):
-        batch_scores = self.compute_scores(batch, full_hidden)
+    def forward(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
+        batch_scores = self.compute_scores(batch, full_hidden, all_query_hidden)
         
         losses = []
-        for curr_scores, boundaries_obj, curr_len in zip(batch_scores, batch.boundaries_objs, batch.seq_lens.cpu().tolist()):
-            curr_non_mask = getattr(boundaries_obj, 'non_mask', self._get_span_non_mask(curr_len))
+        for scores, dbp_obj in zip(batch_scores, batch.dbp_objs):
+            # label_ids: (num_spans, num_spans) or (num_spans, num_spans, voc_dim)
+            label_ids = dbp_obj.dbp2label_id
+            if hasattr(dbp_obj, 'non_mask'):
+                non_mask = dbp_obj.non_mask
+                scores, label_ids = scores[non_mask], label_ids[non_mask]
+            else:
+                scores, label_ids = scores.flatten(end_dim=1), label_ids.flatten(end_dim=1)
             
-            loss = self.criterion(curr_scores[:curr_len, :curr_len][curr_non_mask], boundaries_obj.boundary2label_id[curr_non_mask])
+            loss = self.criterion(scores, label_ids)
             losses.append(loss)
         return torch.stack(losses)
         
         
-    def decode(self, batch: Batch, full_hidden: torch.Tensor):
-        batch_scores = self.compute_scores(batch, full_hidden)
+    def decode(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
+        batch_scores = self.compute_scores(batch, full_hidden, all_query_hidden)
         
-        batch_chunks = []
-        for curr_scores, curr_len in zip(batch_scores, batch.seq_lens.cpu().tolist()):
-            curr_non_mask = self._get_span_non_mask(curr_len)
-            
-            confidences, label_ids = curr_scores[:curr_len, :curr_len][curr_non_mask].softmax(dim=-1).max(dim=-1)
-            labels = [self.idx2label[i] for i in label_ids.cpu().tolist()]
-            chunks = [(label, start, end) for label, (start, end) in zip(labels, _spans_from_upper_triangular(curr_len)) if label != self.none_label]
-            confidences = [conf for label, conf in zip(labels, confidences.cpu().tolist()) if label != self.none_label]
-            assert len(confidences) == len(chunks)
+        batch_relations = []
+        for scores, dbp_obj, curr_len in zip(batch_scores, batch.dbp_objs, batch.seq_lens.cpu().tolist()):
+            curr_max_span_size = min(self.max_span_size, curr_len)
             
-            # Sort chunks from high to low confidences
-            chunks = [ck for _, ck in sorted(zip(confidences, chunks), reverse=True)]
-            chunks = filter_clashed_by_priority(chunks, allow_nested=self.allow_nested)
+            confidences, label_ids = scores.softmax(dim=-1).max(dim=-1)
+            labels = [self.idx2label[i] for i in label_ids.flatten().cpu().tolist()]
             
-            batch_chunks.append(chunks)
-        return batch_chunks
+            relations = []
+            for label, ((h_start, h_end), (t_start, t_end)) in zip(labels, _span_pairs_from_diagonals(curr_len, curr_max_span_size)):
+                head = (dbp_obj.span2ck_label.get((h_start, h_end), self.ck_none_label), h_start, h_end)
+                tail = (dbp_obj.span2ck_label.get((t_start, t_end), self.ck_none_label), t_start, t_end)
+                if label != self.none_label and head[0] != self.ck_none_label and tail[0] != self.ck_none_label:
+                    relations.append((label, head, tail))
+            relations = [(label, head, tail) for label, head, tail in relations 
+                             if  (not self.filter_by_labels or ((label, head[0], tail[0]) in self.existing_rht_labels)) 
+                             and (not self.filter_self_relation or self.existing_self_relation or (head[1:] != tail[1:]))]
+            batch_relations.append(relations)
+        return batch_relations
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/generator.py` & `eznlp-0.2.4/eznlp/model/decoder/generator.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/joint_extraction.py` & `eznlp-0.2.4/eznlp/model/decoder/joint_extraction.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from ...config import Config
 from .base import DecoderMixinBase, SingleDecoderConfigBase, DecoderBase
 from .sequence_tagging import SequenceTaggingDecoderConfig
 from .span_classification import SpanClassificationDecoderConfig
 from .span_attr_classification import SpanAttrClassificationDecoderConfig
 from .span_rel_classification import SpanRelClassificationDecoderConfig
 from .boundary_selection import BoundarySelectionDecoderConfig
+from .specific_span_classification import SpecificSpanClsDecoderConfig
+from .specific_span_rel_classification import SpecificSpanRelClsDecoderConfig
+from .specific_span_sparse_rel_classification import SpecificSpanSparseRelClsDecoderConfig
 
 
 class JointExtractionDecoderMixin(DecoderMixinBase):
     @property
     def has_attr_decoder(self):
         return hasattr(self, 'attr_decoder') and self.attr_decoder is not None
         
@@ -33,17 +36,17 @@
         if self.has_rel_decoder:
             yield self.rel_decoder
         
         
     def exemplify(self, data_entry: dict, training: bool=True):
         example = self.ck_decoder.exemplify(data_entry, training=training)
         if self.has_attr_decoder:
-            example.update(self.attr_decoder.exemplify(data_entry, training=training, building=False))
+            example.update(self.attr_decoder.exemplify(data_entry, training=training))
         if self.has_rel_decoder:
-            example.update(self.rel_decoder.exemplify(data_entry, training=training, building=False))
+            example.update(self.rel_decoder.exemplify(data_entry, training=training))
         return example
         
     def batchify(self, batch_examples: List[dict]):
         batch = self.ck_decoder.batchify(batch_examples)
         if self.has_attr_decoder:
             batch.update(self.attr_decoder.batchify(batch_examples))
         if self.has_rel_decoder:
@@ -59,35 +62,45 @@
                          in zip(self.decoders, y_gold, y_pred))
 
 
 
 class JointExtractionDecoderConfig(Config, JointExtractionDecoderMixin):
     def __init__(self, 
                  ck_decoder: Union[SingleDecoderConfigBase, str]='span_classification', 
-                 attr_decoder: Union[SingleDecoderConfigBase, str]='span_attr_classification', 
+                 attr_decoder: Union[SingleDecoderConfigBase, str]=None, 
                  rel_decoder: Union[SingleDecoderConfigBase, str]='span_rel_classification',
                  **kwargs):
         if isinstance(ck_decoder, SingleDecoderConfigBase):
             self.ck_decoder = ck_decoder
         elif ck_decoder.lower().startswith('sequence_tagging'):
             self.ck_decoder = SequenceTaggingDecoderConfig()
         elif ck_decoder.lower().startswith('span_classification'):
             self.ck_decoder = SpanClassificationDecoderConfig()
         elif ck_decoder.lower().startswith('boundary'):
             self.ck_decoder = BoundarySelectionDecoderConfig()
+        elif ck_decoder.lower().startswith('specific_span_cls'):
+            self.ck_decoder = SpecificSpanClsDecoderConfig()
         
         if isinstance(attr_decoder, SingleDecoderConfigBase) or attr_decoder is None:
             self.attr_decoder = attr_decoder
         elif attr_decoder.lower().startswith('span_attr'):
             self.attr_decoder = SpanAttrClassificationDecoderConfig()
         
         if isinstance(rel_decoder, SingleDecoderConfigBase) or rel_decoder is None:
             self.rel_decoder = rel_decoder
         elif rel_decoder.lower().startswith('span_rel'):
             self.rel_decoder = SpanRelClassificationDecoderConfig()
+        elif rel_decoder.lower().startswith('specific_span_rel'):
+            self.rel_decoder = SpecificSpanRelClsDecoderConfig()
+        elif rel_decoder.lower().startswith('specific_span_sparse_rel'):
+            self.rel_decoder = SpecificSpanSparseRelClsDecoderConfig()
+        
+        self.ck_loss_weight = kwargs.pop('ck_loss_weight', 1.0)
+        self.attr_loss_weight = kwargs.pop('attr_loss_weight', 1.0)
+        self.rel_loss_weight = kwargs.pop('rel_loss_weight', 1.0)
         
         # It seems that pytorch does not recommend to share weights outside two modules. 
         # See https://discuss.pytorch.org/t/how-to-create-model-with-sharing-weight/398/2
         # TODO: Refer to transformers/modeling_utils/PreTrainedModel/_tie_or_clone_weights
         self.share_embeddings = kwargs.pop('share_embeddings', False)
         super().__init__(**kwargs)
         
@@ -107,54 +120,61 @@
         return self.ck_decoder.in_dim
         
     @in_dim.setter
     def in_dim(self, dim: int):
         for decoder in self.decoders:
             decoder.in_dim = dim
         
+    @property
+    def max_span_size(self):
+        return self.ck_decoder.max_span_size
+        
     def build_vocab(self, *partitions):
         for decoder in self.decoders:
             decoder.build_vocab(*partitions)
         
     def instantiate(self):
         return JointExtractionDecoder(self)
 
 
 
 class JointExtractionDecoder(DecoderBase, JointExtractionDecoderMixin):
     def __init__(self, config: JointExtractionDecoderConfig):
         super().__init__()
         self.ck_decoder = config.ck_decoder.instantiate()
+        self.ck_loss_weight = config.ck_loss_weight
         if config.has_attr_decoder:
             self.attr_decoder = config.attr_decoder.instantiate()
+            self.attr_loss_weight = config.attr_loss_weight
         if config.has_rel_decoder:
             self.rel_decoder = config.rel_decoder.instantiate()
+            self.rel_loss_weight = config.rel_loss_weight
         
         
-    def forward(self, batch: Batch, full_hidden: torch.Tensor):
-        losses = self.ck_decoder(batch, full_hidden)
-        batch_chunks_pred = self.ck_decoder.decode(batch, full_hidden)
+    def forward(self, batch: Batch, **states):
+        losses = self.ck_decoder(batch, **states) * self.ck_loss_weight
+        batch_chunks_pred = self.ck_decoder.decode(batch, **states)
         
         if self.has_attr_decoder:
-            self.attr_decoder.inject_chunks_and_build(batch, batch_chunks_pred, full_hidden.device)
-            losses += self.attr_decoder(batch, full_hidden)
+            self.attr_decoder.assign_chunks_pred(batch, batch_chunks_pred)
+            losses += self.attr_decoder(batch, **states) * self.attr_loss_weight
         
         if self.has_rel_decoder:
-            self.rel_decoder.inject_chunks_and_build(batch, batch_chunks_pred, full_hidden.device)
-            losses += self.rel_decoder(batch, full_hidden)
+            self.rel_decoder.assign_chunks_pred(batch, batch_chunks_pred)
+            losses += self.rel_decoder(batch, **states) * self.rel_loss_weight
         
         return losses
         
         
-    def decode(self, batch: Batch, full_hidden: torch.Tensor):
-        batch_chunks_pred = self.ck_decoder.decode(batch, full_hidden)
+    def decode(self, batch: Batch, **states):
+        batch_chunks_pred = self.ck_decoder.decode(batch, **states)
         y_pred = (batch_chunks_pred, )
         
         if self.has_attr_decoder:
-            self.attr_decoder.inject_chunks_and_build(batch, batch_chunks_pred, full_hidden.device)
-            y_pred = (*y_pred, self.attr_decoder.decode(batch, full_hidden))
+            self.attr_decoder.assign_chunks_pred(batch, batch_chunks_pred)
+            y_pred = (*y_pred, self.attr_decoder.decode(batch, **states))
         
         if self.has_rel_decoder:
-            self.rel_decoder.inject_chunks_and_build(batch, batch_chunks_pred, full_hidden.device)
-            y_pred = (*y_pred, self.rel_decoder.decode(batch, full_hidden))
+            self.rel_decoder.assign_chunks_pred(batch, batch_chunks_pred)
+            y_pred = (*y_pred, self.rel_decoder.decode(batch, **states))
         
         return y_pred
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/sequence_tagging.py` & `eznlp-0.2.4/eznlp/model/decoder/sequence_tagging.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/span_attr_classification.py` & `eznlp-0.2.4/eznlp/model/decoder/specific_span_sparse_rel_classification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,274 +1,271 @@
 # -*- coding: utf-8 -*-
-from typing import List
+from typing import List, Dict
 from collections import Counter
+import itertools
 import logging
+import copy
+import math
+import numpy
 import torch
 
-from ...wrapper import TargetWrapper, Batch
-from ...nn.modules import SequencePooling, SequenceAttention, CombinedDropout
-from ...nn.functional import seq_lens2mask
-from ...nn.init import reinit_embedding_, reinit_layer_
-from ...metrics import precision_recall_f1_report
-from .base import DecoderMixinBase, SingleDecoderConfigBase, DecoderBase
+from ...wrapper import Batch
+from ...nn.modules import CombinedDropout
+from ...nn.init import reinit_embedding_, reinit_layer_, reinit_vector_parameter_
+from ..encoder import EncoderConfig
+from .base import SingleDecoderConfigBase, DecoderBase
+from .boundaries import MAX_SIZE_ID_COV_RATE
+from .chunks import ChunkPairs
+from .span_rel_classification import ChunkPairsDecoderMixin
 
 logger = logging.getLogger(__name__)
 
 
-class SpanAttrClassificationDecoderMixin(DecoderMixinBase):
-    @property
-    def idx2ck_label(self):
-        return self._idx2ck_label
-        
-    @idx2ck_label.setter
-    def idx2ck_label(self, idx2ck_label: List[str]):
-        self._idx2ck_label = idx2ck_label
-        self.ck_label2idx = {l: i for i, l in enumerate(idx2ck_label)} if idx2ck_label is not None else None
-        
-    @property
-    def idx2attr_label(self):
-        return self._idx2attr_label
-        
-    @idx2attr_label.setter
-    def idx2attr_label(self, idx2attr_label: List[str]):
-        self._idx2attr_label = idx2attr_label
-        self.attr_label2idx = {l: i for i, l in enumerate(idx2attr_label)} if idx2attr_label is not None else None
-        
-    @property
-    def ck_voc_dim(self):
-        return len(self.ck_label2idx)
-        
-    @property
-    def ck_none_idx(self):
-        return self.ck_label2idx[self.ck_none_label]
-        
-    @property
-    def attr_voc_dim(self):
-        return len(self.attr_label2idx)
-        
-    @property
-    def attr_none_idx(self):
-        return self.attr_label2idx[self.attr_none_label]
-        
-    def exemplify(self, data_entry: dict, training: bool=True, building: bool=True):
-        return {'chunks_obj': Chunks(data_entry, self, training=training, building=building)}
-        
-    def batchify(self, batch_examples: List[dict]):
-        return {'chunks_objs': [ex['chunks_obj'] for ex in batch_examples]}
-        
-    def retrieve(self, batch: Batch):
-        return [chunks_obj.attributes for chunks_obj in batch.chunks_objs]
-        
-    def evaluate(self, y_gold: List[List[tuple]], y_pred: List[List[tuple]]):
-        scores, ave_scores = precision_recall_f1_report(y_gold, y_pred)
-        return ave_scores['micro']['f1']
-        
-    def inject_chunks_and_build(self, batch: Batch, batch_chunks_pred: List[List[tuple]], device=None):
-        """This method is to be invoked outside, as the outside invoker is assumed not to know the structure of `batch`. 
-        """
-        for chunks_obj, chunks_pred in zip(batch.chunks_objs, batch_chunks_pred):
-            if not chunks_obj.is_built:
-                chunks_obj.inject_chunks(chunks_pred)
-                chunks_obj.build(self)
-                if device is not None:
-                    chunks_obj.to(device)
-
-
-
-class Chunks(TargetWrapper):
-    """A wrapper of chunks with underlying attributes. 
-    
-    Parameters
-    ----------
-    data_entry: dict
-        {'tokens': TokenSequence, 
-         'chunks': List[tuple], 
-         'attributes': List[tuple]}
-    
-    Notes
-    -----
-    (1) If `building` is `True`, `data_entry['chunks']` is assumed to be known for both training and evaluation (e.g., pipeline modeling).
-        In this case, the negative samples are generated from `data_entry['chunks']`. 
-    (2) If `building` is `False`, `data_entry['chunks']` is known for training but not for evaluation (e.g., joint modeling).
-        In this case, `inject_chunks` and `build` should be successively invoked, and the negative samples are generated from injected chunks. 
-    """
-    def __init__(self, data_entry: dict, config: SpanAttrClassificationDecoderMixin, training: bool=True, building: bool=True):
-        super().__init__(training)
-        
-        self.chunks = data_entry['chunks'] if training or building else []
-        self.attributes = data_entry.get('attributes', None)
-        
-        self.is_built = False
-        if building:
-            self.build(config)
-        
-        
-    def inject_chunks(self, chunks: List[tuple]):
-        """Inject chunks from outside, typically from on-the-fly decoding. 
-        
-        Notes
-        -----
-        In merged chunks, there may exist two chunks with same spans but different chunk-types. 
-        In this case, `ck_label_ids` is crucial as input. 
-        """
-        assert not self.is_built
-        # Do not use ```self.chunks = list(set(self.chunks + chunks))```,
-        # which may return non-deterministic order?
-        self.chunks = self.chunks + [ck for ck in chunks if ck not in self.chunks]
-        
-        
-    def build(self, config: SpanAttrClassificationDecoderMixin):
-        """Generate negative samples from `self.chunks` and build up tensors. 
-        """
-        assert not self.is_built
-        self.is_built = True
-        
-        if self.training:
-            assert all(ck in self.chunks for attr_label, ck in self.attributes)
-        
-        # span_size_ids / ck_label_ids: (num_chunks, )
-        # Note: size_id = size - 1
-        self.span_size_ids = torch.tensor([end-start-1 for ck_label, start, end in self.chunks], dtype=torch.long)
-        self.span_size_ids.masked_fill_(self.span_size_ids>=config.max_span_size, config.max_span_size-1)
-        self.ck_label_ids = torch.tensor([config.ck_label2idx[ck_label] for ck_label, start, end in self.chunks], dtype=torch.long)
-        
-        if self.attributes is not None:
-            chunk2idx = {ck: k for k, ck in enumerate(self.chunks)}
-            # Note: `torch.nn.BCEWithLogitsLoss` uses `float` tensor as target
-            self.attr_label_ids = torch.zeros(len(self.chunks), config.attr_voc_dim, dtype=torch.float)
-            for attr_label, chunk in self.attributes:
-                # Note: `chunk` does not appear in `self.chunks` only if in evaluation (i.e., gold chunks missing). 
-                # In this case, `attr_label_ids` is only for forward to loss, but not for backward. 
-                if chunk in chunk2idx:
-                    self.attr_label_ids[chunk2idx[chunk], config.attr_label2idx[attr_label]] = 1
-            self.attr_label_ids[:, 0] = (self.attr_label_ids == 0).all(dim=1)
-
-
-
-
-class SpanAttrClassificationDecoderConfig(SingleDecoderConfigBase, SpanAttrClassificationDecoderMixin):
+class SpecificSpanSparseRelClsDecoderConfig(SingleDecoderConfigBase, ChunkPairsDecoderMixin):
     def __init__(self, **kwargs):
-        self.in_drop_rates = kwargs.pop('in_drop_rates', (0.5, 0.0, 0.0))
-        
-        self.max_span_size = kwargs.pop('max_span_size', 10)
-        self.ck_size_emb_dim = kwargs.pop('ck_size_emb_dim', 25)
-        self.ck_label_emb_dim = kwargs.pop('ck_label_emb_dim', 25)
-        
-        self.agg_mode = kwargs.pop('agg_mode', 'max_pooling')
+        self.use_biaffine = kwargs.pop('use_biaffine', True)
+        self.affine = kwargs.pop('affine', EncoderConfig(arch='FFN', hid_dim=150, num_layers=1, in_drop_rates=(0.4, 0.0, 0.0), hid_drop_rate=0.2))
+        self.use_context = kwargs.pop('use_context', True)
+        
+        self.max_span_size_ceiling = kwargs.pop('max_span_size_ceiling', 20)
+        self.max_span_size_cov_rate = kwargs.pop('max_span_size_cov_rate', 0.995)
+        self.max_span_size = kwargs.pop('max_span_size', None)
+        self.size_emb_dim = kwargs.pop('size_emb_dim', 25)
+        self.label_emb_dim = kwargs.pop('label_emb_dim', 25)
+        self.hid_drop_rates = kwargs.pop('hid_drop_rates', (0.2, 0.0, 0.0))
+        
+        self.neg_sampling_rate = kwargs.pop('neg_sampling_rate', 1.0)
+        # self.neg_sampling_power_decay = kwargs.pop('neg_sampling_power_decay', 0.0)  # decay = 0.5, 1.0
+        # self.neg_sampling_surr_rate = kwargs.pop('neg_sampling_surr_rate', 0.0)
+        # self.neg_sampling_surr_size = kwargs.pop('neg_sampling_surr_size', 5)
         
+        self.none_label = kwargs.pop('none_label', '<none>')
+        self.idx2label = kwargs.pop('idx2label', None)
         self.ck_none_label = kwargs.pop('ck_none_label', '<none>')
         self.idx2ck_label = kwargs.pop('idx2ck_label', None)
-        self.attr_none_label = kwargs.pop('attr_none_label', '<none>')
-        self.idx2attr_label = kwargs.pop('idx2attr_label', None)
-        
-        self.multihot = True
-        self.confidence_threshold = kwargs.pop('confidence_threshold', 0.5)
+        self.filter_by_labels = kwargs.pop('filter_by_labels', True)
+        self.filter_self_relation = kwargs.pop('filter_self_relation', True)
         super().__init__(**kwargs)
         
-        
     @property
     def name(self):
-        return self._name_sep.join([self.agg_mode, self.criterion])
+        return self.criterion
         
     def __repr__(self):
-        repr_attr_dict = {key: getattr(self, key) for key in ['in_dim', 'in_drop_rates', 'agg_mode', 'criterion']}
+        repr_attr_dict = {key: getattr(self, key) for key in ['in_dim', 'hid_drop_rates', 'criterion']}
         return self._repr_non_config_attrs(repr_attr_dict)
         
+    @property
+    def in_dim(self):
+        return self.affine.in_dim - self.size_emb_dim - self.label_emb_dim
+        
+    @in_dim.setter
+    def in_dim(self, dim: int):
+        if dim is not None:
+            self.affine.in_dim = dim + self.size_emb_dim + self.label_emb_dim
+        
+    @property
+    def affine_ctx(self):
+        affine_ctx = copy.deepcopy(self.affine)
+        affine_ctx.in_dim = self.in_dim
+        return affine_ctx
+        
     def build_vocab(self, *partitions):
-        ck_counter = Counter(label for data in partitions for entry in data for label, start, end in entry['chunks'])
-        self.idx2ck_label = [self.ck_none_label] + list(ck_counter.keys())
-        attr_counter = Counter(label for data in partitions for entry in data for label, chunk in entry['attributes'])
-        self.idx2attr_label = [self.attr_none_label] + list(attr_counter.keys())
-        legal_ck_counter = Counter(chunk[0] for data in partitions for entry in data for label, chunk in entry['attributes'])
-        self.legal_chunk_types = set(list(legal_ck_counter.keys()))
+        counter = Counter(label for data in partitions for entry in data for label, start, end in entry['chunks'])
+        self.idx2ck_label = [self.ck_none_label] + list(counter.keys())
+        
+        # Calculate `max_span_size` according to data
+        span_sizes = [end-start for data in partitions for entry in data for label, start, end in entry['chunks']]
+        # Allow directly setting `max_span_size`
+        if self.max_span_size is None:
+            if self.max_span_size_cov_rate >= 1:
+                span_size_cov = max(span_sizes)
+            else:
+                span_size_cov = math.ceil(numpy.quantile(span_sizes, self.max_span_size_cov_rate))
+            self.max_span_size = min(span_size_cov, self.max_span_size_ceiling)
+        self.max_size_id = min(math.ceil(numpy.quantile(span_sizes, MAX_SIZE_ID_COV_RATE)), self.max_span_size) - 1
+        logger.warning(f"The `max_span_size` is set to {self.max_span_size}")
+        
+        size_counter = Counter(end-start for data in partitions for entry in data for label, start, end in entry['chunks'])
+        num_spans = sum(size_counter.values())
+        num_oov_spans = sum(num for size, num in size_counter.items() if size > self.max_span_size)
+        if num_oov_spans > 0:
+            logger.warning(f"OOV positive spans: {num_oov_spans} ({num_oov_spans/num_spans*100:.2f}%)")
+        
+        counter = Counter(label for data in partitions for entry in data for label, head, tail in entry['relations'])
+        self.idx2label = [self.none_label] + list(counter.keys())
+        
+        counter = Counter((label, head[0], tail[0]) for data in partitions for entry in data for label, head, tail in entry['relations'])
+        self.existing_rht_labels = set(list(counter.keys()))
+        self.existing_self_relation = any(head[1:]==tail[1:] for data in partitions for entry in data for label, head, tail in entry['relations'])
+        
         
     def instantiate(self):
-        return SpanAttrClassificationDecoder(self)
+        return SpecificSpanSparseRelClsDecoder(self)
 
 
 
-
-class SpanAttrClassificationDecoder(DecoderBase, SpanAttrClassificationDecoderMixin):
-    def __init__(self, config: SpanAttrClassificationDecoderConfig):
+class SpecificSpanSparseRelClsDecoder(DecoderBase, ChunkPairsDecoderMixin):
+    def __init__(self, config: SpecificSpanSparseRelClsDecoderConfig):
         super().__init__()
         self.max_span_size = config.max_span_size
+        self.max_size_id = config.max_size_id
+        self.neg_sampling_rate = config.neg_sampling_rate
+        self.none_label = config.none_label
+        self.idx2label = config.idx2label
         self.ck_none_label = config.ck_none_label
         self.idx2ck_label = config.idx2ck_label
-        self.attr_none_label = config.attr_none_label
-        self.idx2attr_label = config.idx2attr_label
-        self.legal_chunk_types = config.legal_chunk_types
-        
-        if config.agg_mode.lower().endswith('_pooling'):
-            self.aggregating = SequencePooling(mode=config.agg_mode.replace('_pooling', ''))
-        elif config.agg_mode.lower().endswith('_attention'):
-            self.aggregating = SequenceAttention(config.in_dim, scoring=config.agg_mode.replace('_attention', ''))
-        
-        if config.ck_size_emb_dim > 0:
-            self.ck_size_embedding = torch.nn.Embedding(config.max_span_size, config.ck_size_emb_dim)
-            reinit_embedding_(self.ck_size_embedding)
-        if config.ck_label_emb_dim > 0:
-            self.ck_label_embedding = torch.nn.Embedding(config.ck_voc_dim, config.ck_label_emb_dim)
-            reinit_embedding_(self.ck_label_embedding)
-        
-        self.dropout = CombinedDropout(*config.in_drop_rates)
-        self.hid2logit = torch.nn.Linear(config.in_dim+config.ck_size_emb_dim+config.ck_label_emb_dim, config.attr_voc_dim)
-        reinit_layer_(self.hid2logit, 'sigmoid')
+        self.filter_by_labels = config.filter_by_labels
+        self.existing_rht_labels = config.existing_rht_labels
+        self.filter_self_relation = config.filter_self_relation
+        self.existing_self_relation = config.existing_self_relation
+        
+        if config.use_biaffine:
+            self.affine_head = config.affine.instantiate()
+            self.affine_tail = config.affine.instantiate()
+        else:
+            self.affine = config.affine.instantiate()
+        
+        if config.use_context:
+            self.affine_ctx = config.affine_ctx.instantiate()
+            # Trainable context vector for overlapping chunks
+            self.zero_context = torch.nn.Parameter(torch.empty(config.in_dim))
+            reinit_vector_parameter_(self.zero_context)
+        
+        if config.size_emb_dim > 0:
+            self.size_embedding = torch.nn.Embedding(config.max_size_id+1, config.size_emb_dim)
+            reinit_embedding_(self.size_embedding)
+        
+        if config.label_emb_dim > 0:
+            self.label_embedding = torch.nn.Embedding(config.ck_voc_dim, config.label_emb_dim)
+            reinit_embedding_(self.label_embedding)
+        
+        self.dropout = CombinedDropout(*config.hid_drop_rates)
+        
+        self.U = torch.nn.Parameter(torch.empty(config.voc_dim, config.affine.out_dim, config.affine.out_dim))
+        self.W = torch.nn.Parameter(torch.empty(config.voc_dim, config.affine.out_dim*(3 if config.use_context else 2)))
+        self.b = torch.nn.Parameter(torch.empty(config.voc_dim))
+        torch.nn.init.orthogonal_(self.U.data)
+        torch.nn.init.orthogonal_(self.W.data)
+        torch.nn.init.zeros_(self.b.data)
         
         self.criterion = config.instantiate_criterion(reduction='sum')
-        self.confidence_threshold = config.confidence_threshold
         
         
-    def get_logits(self, batch: Batch, full_hidden: torch.Tensor):
+    def assign_chunks_pred(self, batch: Batch, batch_chunks_pred: List[List[tuple]]):
+        """This method should be called on-the-fly for joint modeling. 
+        """
+        for cp_obj, chunks_pred in zip(batch.cp_objs, batch_chunks_pred):
+            if cp_obj.chunks_pred is None:
+                cp_obj.chunks_pred = chunks_pred
+                cp_obj.build(self)
+                cp_obj.to(self.W.device)
+        
+        
+    def compute_scores(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
         # full_hidden: (batch, step, hid_dim)
-        batch_logits = []
-        for k in range(full_hidden.size(0)):
-            if len(batch.chunks_objs[k].chunks) == 0:
-                logits = torch.empty(0, self.hid2logit.out_features, device=full_hidden.device)
-                
+        # query_hidden: (batch, step-k+1, hid_dim)
+        all_hidden = [full_hidden] + list(all_query_hidden.values())
+        
+        batch_scores = []
+        for i, cp_obj in enumerate(batch.cp_objs):
+            num_chunks = len(cp_obj.chunks)
+            if num_chunks == 0:
+                scores = torch.empty(0, 0, self.W.size(0), device=full_hidden.device)
             else:
-                # span_hidden: (num_spans, span_size, hid_dim) -> (num_spans, hid_dim)
-                span_hidden = [full_hidden[k, start:end] for ck_label, start, end in batch.chunks_objs[k].chunks]
-                span_mask = seq_lens2mask(torch.tensor([h.size(0) for h in span_hidden], dtype=torch.long, device=full_hidden.device))
-                span_hidden = torch.nn.utils.rnn.pad_sequence(span_hidden, batch_first=True, padding_value=0.0)
-                span_hidden = self.aggregating(self.dropout(span_hidden), mask=span_mask)
+                # (num_chunks, hid_dim)
+                span_hidden = torch.stack([all_hidden[end-start-1][i, start] for label, start, end in cp_obj.chunks])
                 
-                if hasattr(self, 'ck_size_embedding'):
-                    # ck_size_embedded: (num_spans, emb_dim)
-                    ck_size_embedded = self.ck_size_embedding(batch.chunks_objs[k].span_size_ids)
-                    span_hidden = torch.cat([span_hidden, self.dropout(ck_size_embedded)], dim=-1)
+                if hasattr(self, 'size_embedding'):
+                    # size_embedded: (num_chunks, emb_dim)
+                    size_embedded = self.size_embedding(cp_obj.span_size_ids)
+                    span_hidden = torch.cat([span_hidden, size_embedded], dim=-1)
                 
-                if hasattr(self, 'ck_label_embedding'):
-                    # ck_label_embedded: (num_spans, emb_dim)
-                    ck_label_embedded = self.ck_label_embedding(batch.chunks_objs[k].ck_label_ids)
-                    span_hidden = torch.cat([span_hidden, self.dropout(ck_label_embedded)], dim=-1)
+                if hasattr(self, 'label_embedding'):
+                    # label_embedded: (num_chunks, emb_dim)
+                    label_embedded = self.label_embedding(cp_obj.ck_label_ids)
+                    span_hidden = torch.cat([span_hidden, label_embedded], dim=-1)
                 
-                logits = self.hid2logit(span_hidden)
-            
-            batch_logits.append(logits)
-        
-        return batch_logits
-        
-        
-    def forward(self, batch: Batch, full_hidden: torch.Tensor):
-        batch_logits = self.get_logits(batch, full_hidden)
-        
-        losses = [self.criterion(batch_logits[k], batch.chunks_objs[k].attr_label_ids) 
-                      if len(batch.chunks_objs[k].chunks) > 0
-                      else torch.tensor(0.0, device=full_hidden.device)
-                      for k in range(full_hidden.size(0))]
+                if hasattr(self, 'affine_head'):
+                    # No mask input needed here
+                    affined_head = self.affine_head(span_hidden)
+                    affined_tail = self.affine_tail(span_hidden)
+                else:
+                    affined_head = self.affine(span_hidden)
+                    affined_tail = self.affine(span_hidden)
+                
+                # scores1: (head_chunks, affine_dim) * (voc_dim, affine_dim, affine_dim) * (affine_dim, tail_chunks) -> (voc_dim, head_chunks, tail_chunks)
+                scores1 = self.dropout(affined_head).matmul(self.U).matmul(self.dropout(affined_tail.permute(1, 0)))
+                
+                # affined_cat: (head_chunks, tail_chunks, affine_dim*2)
+                affined_cat = torch.cat([self.dropout(affined_head).unsqueeze(1).expand(-1, affined_tail.size(0), -1), 
+                                         self.dropout(affined_tail).unsqueeze(0).expand(affined_head.size(0), -1, -1)], dim=-1)
+                
+                if hasattr(self, 'affine_ctx'):
+                    # contexts: (num_chunks^2, hid_dim)
+                    contexts = []
+                    for (h_label, h_start, h_end), (t_label, t_start, t_end) in itertools.product(cp_obj.chunks, cp_obj.chunks):
+                        if h_end < t_start:
+                            contexts.append(_collect_context_from_specific_span_hidden(i, h_end, t_start, all_hidden))
+                        elif t_end < h_start:
+                            contexts.append(_collect_context_from_specific_span_hidden(i, t_end, h_start, all_hidden))
+                        else:
+                            contexts.append(self.zero_context)
+                    contexts = torch.stack(contexts)
+                    # affined_ctx: (num_chunks^2, affine_dim) -> (num_chunks, num_chunks, affine_dim)
+                    affined_ctx = self.affine_ctx(contexts).view(num_chunks, num_chunks, -1)
+                    affined_cat = torch.cat([affined_cat, self.dropout(affined_ctx)], dim=-1)
+                
+                # scores2: (voc_dim, affine_dim*2) * (head_chunks, tail_chunks, affine_dim*2, 1) -> (head_chunks, tail_chunks, voc_dim, 1) 
+                scores2 = self.W.matmul(affined_cat.unsqueeze(-1))
+                # scores: (head_chunks, tail_chunks, voc_dim)
+                scores = scores1.permute(1, 2, 0) + scores2.squeeze(-1) + self.b
+            batch_scores.append(scores)
+        
+        return batch_scores
+        
+        
+    def forward(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
+        batch_scores = self.compute_scores(batch, full_hidden, all_query_hidden)
+        
+        losses = []
+        for scores, cp_obj in zip(batch_scores, batch.cp_objs):
+            if len(cp_obj.chunks) == 0:
+                loss = torch.tensor(0.0, device=full_hidden.device)
+            else:
+                label_ids = cp_obj.cp2label_id
+                if hasattr(cp_obj, 'non_mask'):
+                    non_mask = cp_obj.non_mask
+                    scores, label_ids = scores[non_mask], label_ids[non_mask]
+                else:
+                    scores, label_ids = scores.flatten(end_dim=1), label_ids.flatten(end_dim=1)
+                loss = self.criterion(scores, label_ids)
+            losses.append(loss)
         return torch.stack(losses)
         
         
-    def decode(self, batch: Batch, full_hidden: torch.Tensor):
-        batch_logits = self.get_logits(batch, full_hidden)
-        
-        batch_attributes = []
-        for k in range(full_hidden.size(0)):
-            attributes = []
-            if len(batch.chunks_objs[k].chunks) > 0:
-                for chunk, ck_sigmoids in zip(batch.chunks_objs[k].chunks, batch_logits[k].sigmoid()):
-                    attr_labels = [self.idx2attr_label[i] for i, s in enumerate(ck_sigmoids.cpu().tolist()) if s >= self.confidence_threshold]
-                    if self.attr_none_label not in attr_labels:
-                        attributes.extend([(attr_label, chunk) for attr_label in attr_labels])
-            batch_attributes.append(attributes)
+    def decode(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
+        batch_scores = self.compute_scores(batch, full_hidden, all_query_hidden)
         
-        return batch_attributes
+        batch_relations = []
+        for scores, cp_obj in zip(batch_scores, batch.cp_objs):
+            if len(cp_obj.chunks) == 0:
+                relations = []
+            else:
+                confidences, label_ids = scores.softmax(dim=-1).max(dim=-1)
+                labels = [self.idx2label[i] for i in label_ids.flatten().cpu().tolist()]
+                relations = [(label, head, tail) for label, (head, tail) in zip(labels, itertools.product(cp_obj.chunks, cp_obj.chunks)) if label != self.none_label]
+                relations = [(label, head, tail) for label, head, tail in relations 
+                                if  (not self.filter_by_labels or ((label, head[0], tail[0]) in self.existing_rht_labels)) 
+                                and (not self.filter_self_relation or self.existing_self_relation or (head[1:] != tail[1:]))]
+            batch_relations.append(relations)
+        return batch_relations
+
+
+
+# TODO: Aggregation?
+def _collect_context_from_specific_span_hidden(i: int, start: int, end: int, all_hidden: List[torch.Tensor]):
+    max_span_size = len(all_hidden)
+    if end - start <= max_span_size:
+        return all_hidden[end-start-1][i, start]
+    else:
+        return (all_hidden[max_span_size-1][i, start] + all_hidden[max_span_size-1][i, end-max_span_size]) / 2
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/span_classification.py` & `eznlp-0.2.4/eznlp/model/decoder/specific_span_classification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,212 +1,212 @@
 # -*- coding: utf-8 -*-
-from typing import List
+from typing import Dict
 from collections import Counter
-import random
 import logging
+import math
+import numpy
 import torch
 
-from ...wrapper import TargetWrapper, Batch
-from ...utils.chunk import detect_nested, filter_clashed_by_priority
-from ...nn.modules import SequencePooling, SequenceAttention, CombinedDropout
-from ...nn.functional import seq_lens2mask
+from ...wrapper import Batch
+from ...utils.chunk import detect_overlapping_level, filter_clashed_by_priority
+from ...nn.modules import CombinedDropout, SoftLabelCrossEntropyLoss
 from ...nn.init import reinit_embedding_, reinit_layer_
-from ...metrics import precision_recall_f1_report
-from .base import DecoderMixinBase, SingleDecoderConfigBase, DecoderBase
+from ..encoder import EncoderConfig
+from .base import SingleDecoderConfigBase, DecoderBase
+from .boundaries import Boundaries, MAX_SIZE_ID_COV_RATE, _spans_from_diagonals
+from .boundary_selection import BoundariesDecoderMixin
 
 logger = logging.getLogger(__name__)
 
 
-class SpanClassificationDecoderMixin(DecoderMixinBase):
-    @property
-    def idx2label(self):
-        return self._idx2label
-        
-    @idx2label.setter
-    def idx2label(self, idx2label: List[str]):
-        self._idx2label = idx2label
-        self.label2idx = {l: i for i, l in enumerate(idx2label)} if idx2label is not None else None
-        
-    @property
-    def voc_dim(self):
-        return len(self.label2idx)
-        
-    @property
-    def none_idx(self):
-        return self.label2idx[self.none_label]
-        
-    def exemplify(self, data_entry: dict, training: bool=True):
-        return {'spans_obj': Spans(data_entry, self, training=training)}
-        
-    def batchify(self, batch_examples: List[dict]):
-        return {'spans_objs': [ex['spans_obj'] for ex in batch_examples]}
-        
-    def retrieve(self, batch: Batch):
-        return [spans_obj.chunks for spans_obj in batch.spans_objs]
-        
-    def evaluate(self, y_gold: List[List[tuple]], y_pred: List[List[tuple]]):
-        """Micro-F1 for entity recognition. 
-        
-        References
-        ----------
-        https://www.clips.uantwerpen.be/conll2000/chunking/output.html
-        """
-        scores, ave_scores = precision_recall_f1_report(y_gold, y_pred)
-        return ave_scores['micro']['f1']
 
-
-
-class Spans(TargetWrapper):
-    """A wrapper of spans with underlying chunks. 
-    
-    Parameters
-    ----------
-    data_entry: dict
-        {'tokens': TokenSequence, 
-         'chunks': List[tuple]}
-    """
-    def __init__(self, data_entry: dict, config: SpanClassificationDecoderMixin, training: bool=True):
-        super().__init__(training)
-        
-        self.chunks = data_entry.get('chunks', None)
-        if training:
-            pos_spans = [(start, end) for label, start, end in self.chunks]
-        else:
-            pos_spans = []
-        
-        neg_spans = [(start, end) 
-                         for start in range(len(data_entry['tokens'])) 
-                         for end in range(start+1, min(start+1+config.max_span_size, len(data_entry['tokens']) + 1))
-                         if (start, end) not in pos_spans]
-        
-        if training and len(neg_spans) > config.num_neg_chunks:
-            neg_spans = random.sample(neg_spans, config.num_neg_chunks)
-        
-        self.spans = pos_spans + neg_spans
-        # Note: size_id = size - 1
-        self.span_size_ids = torch.tensor([end-start-1 for start, end in self.spans], dtype=torch.long)
-        self.span_size_ids.masked_fill_(self.span_size_ids>=config.max_span_size, config.max_span_size-1)
-        
-        # TODO: boundary/label smoothing
-        # Do not smooth to `<none>` label
-        if self.chunks is not None:
-            span2label = {(start, end): label for label, start, end in self.chunks}
-            labels = [span2label.get(span, config.none_label) for span in self.spans]
-            self.label_ids = torch.tensor([config.label2idx[label] for label in labels], dtype=torch.long)
-
-
-
-class SpanClassificationDecoderConfig(SingleDecoderConfigBase, SpanClassificationDecoderMixin):
+class SpecificSpanClsDecoderConfig(SingleDecoderConfigBase, BoundariesDecoderMixin):
     def __init__(self, **kwargs):
-        self.in_drop_rates = kwargs.pop('in_drop_rates', (0.5, 0.0, 0.0))
+        self.affine = kwargs.pop('affine', EncoderConfig(arch='FFN', hid_dim=300, num_layers=1, in_drop_rates=(0.4, 0.0, 0.0), hid_drop_rate=0.2))
         
-        self.num_neg_chunks = kwargs.pop('num_neg_chunks', 100)
-        self.max_span_size = kwargs.pop('max_span_size', 10)
+        self.max_span_size_ceiling = kwargs.pop('max_span_size_ceiling', 20)
+        self.max_span_size_cov_rate = kwargs.pop('max_span_size_cov_rate', 0.995)
+        self.max_span_size = kwargs.pop('max_span_size', None)
+        self.max_len = kwargs.pop('max_len', None)
         self.size_emb_dim = kwargs.pop('size_emb_dim', 25)
+        self.hid_drop_rates = kwargs.pop('hid_drop_rates', (0.2, 0.0, 0.0))
         
-        self.agg_mode = kwargs.pop('agg_mode', 'max_pooling')
+        self.neg_sampling_rate = kwargs.pop('neg_sampling_rate', 1.0)
+        self.neg_sampling_power_decay = kwargs.pop('neg_sampling_power_decay', 0.0)  # decay = 0.5, 1.0
+        self.neg_sampling_surr_rate = kwargs.pop('neg_sampling_surr_rate', 0.0)
+        self.neg_sampling_surr_size = kwargs.pop('neg_sampling_surr_size', 5)
         
         self.none_label = kwargs.pop('none_label', '<none>')
         self.idx2label = kwargs.pop('idx2label', None)
-        # Note: non-nested overlapping chunks are never allowed
-        self.allow_nested = kwargs.pop('allow_nested', None)
-        super().__init__(**kwargs)
+        self.overlapping_level = kwargs.pop('overlapping_level', None)
         
+        # Boundary smoothing epsilon
+        self.sb_epsilon = kwargs.pop('sb_epsilon', 0.0)
+        self.sb_size = kwargs.pop('sb_size', 1)
+        self.sb_adj_factor = kwargs.pop('sb_adj_factor', 1.0)
+        super().__init__(**kwargs)
         
     @property
     def name(self):
-        return self._name_sep.join([self.agg_mode, self.criterion])
+        return self._name_sep.join([self.affine.arch, self.criterion])
         
     def __repr__(self):
-        repr_attr_dict = {key: getattr(self, key) for key in ['in_dim', 'in_drop_rates', 'agg_mode', 'criterion']}
+        repr_attr_dict = {key: getattr(self, key) for key in ['in_dim', 'hid_drop_rates', 'criterion']}
         return self._repr_non_config_attrs(repr_attr_dict)
         
+    @property
+    def in_dim(self):
+        return self.affine.in_dim - self.size_emb_dim
+        
+    @in_dim.setter
+    def in_dim(self, dim: int):
+        if dim is not None:
+            self.affine.in_dim = dim + self.size_emb_dim
+        
+    @property
+    def criterion(self):
+        if self.sb_epsilon > 0:
+            return f"SB({self.sb_epsilon:.2f}, {self.sb_size})"
+        else:
+            return super().criterion
+        
+    def instantiate_criterion(self, **kwargs):
+        if self.criterion.lower().startswith(('sb', 'sl')):
+            # For boundary/label smoothing, the `Boundaries` object has been accordingly changed; 
+            # hence, do not use `SmoothLabelCrossEntropyLoss`
+            return SoftLabelCrossEntropyLoss(**kwargs)
+        else:
+            return super().instantiate_criterion(**kwargs)
+        
+        
     def build_vocab(self, *partitions):
         counter = Counter(label for data in partitions for entry in data for label, start, end in entry['chunks'])
         self.idx2label = [self.none_label] + list(counter.keys())
         
-        self.allow_nested = any(detect_nested(entry['chunks']) for data in partitions for entry in data)
-        if self.allow_nested:
-            logger.info("Nested chunks detected, nested chunks are allowed in decoding...")
-        else:
-            logger.info("No nested chunks detected, only flat chunks are allowed in decoding...")
+        self.overlapping_level = max(detect_overlapping_level(entry['chunks']) for data in partitions for entry in data)
+        logger.info(f"Overlapping level: {self.overlapping_level}")
+        
+        # Calculate `max_span_size` according to data
+        span_sizes = [end-start for data in partitions for entry in data for label, start, end in entry['chunks']]
+        # Allow directly setting `max_span_size`
+        if self.max_span_size is None:
+            if self.max_span_size_cov_rate >= 1:
+                span_size_cov = max(span_sizes)
+            else:
+                span_size_cov = math.ceil(numpy.quantile(span_sizes, self.max_span_size_cov_rate))
+            self.max_span_size = min(span_size_cov, self.max_span_size_ceiling)
+        self.max_size_id = min(math.ceil(numpy.quantile(span_sizes, MAX_SIZE_ID_COV_RATE)), self.max_span_size) - 1
+        logger.warning(f"The `max_span_size` is set to {self.max_span_size}")
         
         size_counter = Counter(end-start for data in partitions for entry in data for label, start, end in entry['chunks'])
         num_spans = sum(size_counter.values())
         num_oov_spans = sum(num for size, num in size_counter.items() if size > self.max_span_size)
         if num_oov_spans > 0:
             logger.warning(f"OOV positive spans: {num_oov_spans} ({num_oov_spans/num_spans*100:.2f}%)")
         
+        self.max_len = max(len(data_entry['tokens']) for data in partitions for data_entry in data)
+        
         
     def instantiate(self):
-        return SpanClassificationDecoder(self)
+        return SpecificSpanClsDecoder(self)
 
 
 
-class SpanClassificationDecoder(DecoderBase, SpanClassificationDecoderMixin):
-    def __init__(self, config: SpanClassificationDecoderConfig):
+class SpecificSpanClsDecoder(DecoderBase, BoundariesDecoderMixin):
+    def __init__(self, config: SpecificSpanClsDecoderConfig):
         super().__init__()
+        self.max_span_size = config.max_span_size
         self.none_label = config.none_label
         self.idx2label = config.idx2label
-        self.allow_nested = config.allow_nested
+        self.overlapping_level = config.overlapping_level
         
-        if config.agg_mode.lower().endswith('_pooling'):
-            self.aggregating = SequencePooling(mode=config.agg_mode.replace('_pooling', ''))
-        elif config.agg_mode.lower().endswith('_attention'):
-            self.aggregating = SequenceAttention(config.in_dim, scoring=config.agg_mode.replace('_attention', ''))
+        self.affine = config.affine.instantiate()
         
         if config.size_emb_dim > 0:
-            self.size_embedding = torch.nn.Embedding(config.max_span_size, config.size_emb_dim)
+            self.size_embedding = torch.nn.Embedding(config.max_size_id+1, config.size_emb_dim)
             reinit_embedding_(self.size_embedding)
         
-        self.dropout = CombinedDropout(*config.in_drop_rates)
-        self.hid2logit = torch.nn.Linear(config.in_dim+config.size_emb_dim, config.voc_dim)
+        self.register_buffer('_span_size_ids', torch.arange(config.max_len) - torch.arange(config.max_len).unsqueeze(-1))
+        self._span_size_ids.masked_fill_(self._span_size_ids < 0, 0)
+        self._span_size_ids.masked_fill_(self._span_size_ids > config.max_size_id, config.max_size_id)
+        
+        self.dropout = CombinedDropout(*config.hid_drop_rates)
+        self.hid2logit = torch.nn.Linear(config.affine.out_dim, config.voc_dim)
         reinit_layer_(self.hid2logit, 'sigmoid')
         
         self.criterion = config.instantiate_criterion(reduction='sum')
         
         
-    def get_logits(self, batch: Batch, full_hidden: torch.Tensor):
+    def _get_diagonal_span_size_ids(self, seq_len: int, max_span_size: int):
+        span_size_ids = self._span_size_ids[:seq_len, :seq_len]
+        return torch.cat([span_size_ids.diagonal(offset=k-1) for k in range(1, max_span_size+1)], dim=-1)
+        
+        
+    def get_logits(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
         # full_hidden: (batch, step, hid_dim)
+        # query_hidden: (batch, step-k+1, hid_dim)
+        all_hidden = [full_hidden] + list(all_query_hidden.values())
+        
         batch_logits = []
-        for k in range(full_hidden.size(0)):
-            # span_hidden: (num_spans, span_size, hid_dim) -> (num_spans, hid_dim)
-            span_hidden = [full_hidden[k, start:end] for start, end in batch.spans_objs[k].spans]
-            span_mask = seq_lens2mask(torch.tensor([h.size(0) for h in span_hidden], dtype=torch.long, device=full_hidden.device))
-            span_hidden = torch.nn.utils.rnn.pad_sequence(span_hidden, batch_first=True, padding_value=0.0)
-            span_hidden = self.aggregating(self.dropout(span_hidden), mask=span_mask)
+        for i, curr_len in enumerate(batch.seq_lens.cpu().tolist()):
+            curr_max_span_size = min(self.max_span_size, curr_len)
+            
+            # (curr_len-k+1, hid_dim) -> (num_spans = \sum_k curr_len-k+1, hid_dim)
+            span_hidden = torch.cat([all_hidden[k-1][i, :curr_len-k+1] for k in range(1, curr_max_span_size+1)], dim=0)
             
             if hasattr(self, 'size_embedding'):
-                # size_embedded: (num_spans, emb_dim)
-                size_embedded = self.size_embedding(batch.spans_objs[k].span_size_ids)
-                span_hidden = torch.cat([span_hidden, self.dropout(size_embedded)], dim=-1)
-                
-            logits = self.hid2logit(span_hidden)
-            batch_logits.append(logits)
+                # size_embedded: (num_spans = \sum_k curr_len-k+1, emb_dim)
+                size_embedded = self.size_embedding(self._get_diagonal_span_size_ids(curr_len, curr_max_span_size))
+                span_hidden = torch.cat([span_hidden, size_embedded], dim=-1)
+            
+            # No mask input needed here
+            affined = self.affine(span_hidden)
             
+            # (num_spans, logit_dim)
+            logits = self.hid2logit(self.dropout(affined))
+            batch_logits.append(logits)
+        
         return batch_logits
         
         
-    def forward(self, batch: Batch, full_hidden: torch.Tensor):
-        batch_logits = self.get_logits(batch, full_hidden)
+    def forward(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
+        batch_logits = self.get_logits(batch, full_hidden, all_query_hidden)
         
-        losses = [self.criterion(batch_logits[k], batch.spans_objs[k].label_ids) for k in range(full_hidden.size(0))]
+        losses = []
+        for logits, boundaries_obj, curr_len in zip(batch_logits, batch.boundaries_objs, batch.seq_lens.cpu().tolist()):
+            curr_max_span_size = min(self.max_span_size, curr_len)
+            
+            # label_ids: (num_spans = \sum_k curr_len-k+1, ) or (num_spans = \sum_k curr_len-k+1, logit_dim)
+            label_ids = boundaries_obj.diagonal_label_ids(curr_max_span_size)
+            if hasattr(boundaries_obj, 'non_mask'):
+                non_mask = boundaries_obj.diagonal_non_mask(curr_max_span_size)
+                logits, label_ids = logits[non_mask], label_ids[non_mask]
+            
+            loss = self.criterion(logits, label_ids)
+            losses.append(loss)
         return torch.stack(losses)
         
         
-    def decode(self, batch: Batch, full_hidden: torch.Tensor):
-        batch_logits = self.get_logits(batch, full_hidden)
+    def decode(self, batch: Batch, full_hidden: torch.Tensor, all_query_hidden: Dict[int, torch.Tensor]):
+        batch_logits = self.get_logits(batch, full_hidden, all_query_hidden)
         
         batch_chunks = []
-        for k in range(full_hidden.size(0)):
-            confidences, label_ids = batch_logits[k].softmax(dim=-1).max(dim=-1)
+        for logits, boundaries_obj, curr_len in zip(batch_logits, batch.boundaries_objs, batch.seq_lens.cpu().tolist()):
+            curr_max_span_size = min(self.max_span_size, curr_len)
+            
+            confidences, label_ids = logits.softmax(dim=-1).max(dim=-1)
             labels = [self.idx2label[i] for i in label_ids.cpu().tolist()]
-            chunks = [(label, start, end) for label, (start, end) in zip(labels, batch.spans_objs[k].spans) if label != self.none_label]
+            chunks = [(label, start, end) for label, (start, end) in zip(labels, _spans_from_diagonals(curr_len, curr_max_span_size)) if label != self.none_label]
             confidences = [conf for label, conf in zip(labels, confidences.cpu().tolist()) if label != self.none_label]
             assert len(confidences) == len(chunks)
             
+            if hasattr(boundaries_obj, 'sub2ori_idx'):
+                is_valid = [isinstance(boundaries_obj.sub2ori_idx[start], int) and isinstance(boundaries_obj.sub2ori_idx[end], int) for label, start, end in chunks]
+                confidences = [conf for conf, is_v in zip(confidences, is_valid) if is_v]
+                chunks = [ck for ck, is_v in zip(chunks, is_valid) if is_v]
+            
             # Sort chunks from high to low confidences
             chunks = [ck for _, ck in sorted(zip(confidences, chunks), reverse=True)]
-            chunks = filter_clashed_by_priority(chunks, allow_nested=self.allow_nested)
+            chunks = filter_clashed_by_priority(chunks, allow_level=self.overlapping_level)
             
             batch_chunks.append(chunks)
         return batch_chunks
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/decoder/text_classification.py` & `eznlp-0.2.4/eznlp/model/decoder/text_classification.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/elmo.py` & `eznlp-0.2.4/eznlp/model/elmo.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/embedder.py` & `eznlp-0.2.4/eznlp/model/embedder.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/encoder.py` & `eznlp-0.2.4/eznlp/model/encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,52 +95,52 @@
         super().__init__()
         self.dropout = CombinedDropout(*config.in_drop_rates)
         if config.in_proj:
             self.in_proj_layer = torch.nn.Linear(config.in_dim, config.in_dim)
             reinit_layer_(self.in_proj_layer, 'linear')
         self.shortcut = config.shortcut
         
-    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor):
+    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None):
         raise NotImplementedError("Not Implemented `embedded2hidden`")
         
-    def forward(self, embedded: torch.FloatTensor, mask: torch.BoolTensor):
+    def forward(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None):
         # embedded: (batch, step, emb_dim)
         # hidden: (batch, step, hid_dim)
         if hasattr(self, 'in_proj_layer'):
-            hidden = self.embedded2hidden(self.in_proj_layer(self.dropout(embedded)), mask)
+            hidden = self.embedded2hidden(self.in_proj_layer(self.dropout(embedded)), mask=mask)
         else:
-            hidden = self.embedded2hidden(self.dropout(embedded), mask)
+            hidden = self.embedded2hidden(self.dropout(embedded), mask=mask)
         
         if self.shortcut:
             return torch.cat([hidden, embedded], dim=-1)
         else:
             return hidden
 
 
 
 class IdentityEncoder(Encoder):
     def __init__(self, config: EncoderConfig):
         super().__init__(config)
         
-    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor):
+    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None):
         return embedded
 
 
 
 class FFNEncoder(Encoder):
     def __init__(self, config: EncoderConfig):
         super().__init__(config)
         # NOTE: Only the first layer is differently configured, consistent to `torch.nn.RNN` modules
         self.ff_blocks = torch.nn.ModuleList(
             [FeedForwardBlock(in_dim=(config.in_dim if k==0 else config.hid_dim), 
                               out_dim=config.hid_dim, 
                               drop_rate=(0.0 if k==0 else config.hid_drop_rate)) for k in range(config.num_layers)]
         )
         
-    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor):
+    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None):
         hidden = embedded
         for ff_block in self.ff_blocks:
             hidden = ff_block(hidden)
         
         return hidden
 
 
@@ -165,49 +165,52 @@
         # h_0/c_0: (layers*directions, batch, hid_dim/2)
         if config.train_init_hidden:
             self.h_0 = torch.nn.Parameter(torch.zeros(config.num_layers*2, 1, config.hid_dim//2))
             if isinstance(self.rnn, torch.nn.LSTM):
                 self.c_0 = torch.nn.Parameter(torch.zeros(config.num_layers*2, 1, config.hid_dim//2))
         
         
-    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor, return_last_hidden: bool=False):
-        packed_embedded = torch.nn.utils.rnn.pack_padded_sequence(embedded, 
-                                                                  lengths=mask2seq_lens(mask).cpu(), 
-                                                                  batch_first=True, 
-                                                                  enforce_sorted=False)
+    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None, return_last_hidden: bool=False):
         if hasattr(self, 'h_0'):
             h_0 = self.h_0.expand(-1, embedded.size(0), -1)
             if hasattr(self, 'c_0'):
                 c_0 = self.c_0.expand(-1, embedded.size(0), -1)
                 h_0 = (h_0, c_0)
         else:
             h_0 = None
         
+        if mask is not None:
+            embedded = torch.nn.utils.rnn.pack_padded_sequence(embedded, 
+                                                               lengths=mask2seq_lens(mask).cpu(), 
+                                                               batch_first=True, 
+                                                               enforce_sorted=False)
+        
+        # rnn_outs: (batch, step, hid_dim)
         if isinstance(self.rnn, torch.nn.LSTM):
-            packed_rnn_outs, (h_T, _) = self.rnn(packed_embedded, h_0)
+            rnn_outs, (h_T, _) = self.rnn(embedded, h_0)
         else:
-            packed_rnn_outs, h_T = self.rnn(packed_embedded, h_0)
+            rnn_outs, h_T = self.rnn(embedded, h_0)
         
-        # rnn_outs: (batch, step, hid_dim)
-        rnn_outs, _ = torch.nn.utils.rnn.pad_packed_sequence(packed_rnn_outs, batch_first=True, padding_value=0)
+        if mask is not None:
+            rnn_outs, _ = torch.nn.utils.rnn.pad_packed_sequence(rnn_outs, batch_first=True, padding_value=0)
         
         if return_last_hidden:
             # h_T: (layers*directions, batch, hid_dim/2)
             return rnn_outs, h_T
         else:
             return rnn_outs
         
         
-    def forward(self, embedded: torch.FloatTensor, mask: torch.BoolTensor, return_last_hidden: bool=False):
+    def forward(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None, return_last_hidden: bool=False):
         # embedded: (batch, step, emb_dim)
         # hidden: (batch, step, hid_dim)
         if hasattr(self, 'in_proj_layer'):
-            hidden = self.embedded2hidden(self.in_proj_layer(self.dropout(embedded)), mask, return_last_hidden=return_last_hidden)
+            hidden = self.embedded2hidden(self.in_proj_layer(self.dropout(embedded)), mask=mask, return_last_hidden=return_last_hidden)
         else:
-            hidden = self.embedded2hidden(self.dropout(embedded), mask, return_last_hidden=return_last_hidden)
+            hidden = self.embedded2hidden(self.dropout(embedded), mask=mask, return_last_hidden=return_last_hidden)
         
         if self.shortcut:
             if return_last_hidden:
                 return torch.cat([hidden[0], embedded], dim=-1), hidden[1]
             else:
                 return torch.cat([hidden, embedded], dim=-1)
         else:
@@ -223,19 +226,19 @@
             [ConvBlock(in_dim=(config.in_dim if k==0 else config.hid_dim), 
                        out_dim=config.hid_dim, 
                        kernel_size=config.kernel_size, 
                        drop_rate=(0.0 if k==0 else config.hid_drop_rate), 
                        nonlinearity='relu') for k in range(config.num_layers)]
         )
         
-    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor):
+    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None):
         # embedded: (batch, step, emb_dim) -> (batch, emb_dim, step)
         hidden = embedded.permute(0, 2, 1)
         for conv_block in self.conv_blocks:
-            hidden = conv_block(hidden, mask)
+            hidden = conv_block(hidden, mask=mask)
         
         # hidden: (batch, hid_dim, step) -> (batch, step, hid_dim)
         return hidden.permute(0, 2, 1)
 
 
 
 class GehringConvEncoder(Encoder):
@@ -257,30 +260,31 @@
                        kernel_size=config.kernel_size, 
                        drop_rate=config.hid_drop_rate, # Note to apply dropout to `init_hidden`
                        nonlinearity='glu') for k in range(config.num_layers)]
         )
         self.scale = config.scale
         
         
-    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor):
+    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None):
         init_hidden = self.glu(self.emb2init_hid(embedded))
         
         # hidden: (batch, step, hid_dim/channels) -> (batch, hid_dim/channels, step)
         hidden = init_hidden.permute(0, 2, 1)
         for conv_block in self.conv_blocks:
-            conved = conv_block(hidden, mask)
+            conved = conv_block(hidden, mask=mask)
             hidden = (hidden + conved) * self.scale
         
         # hidden: (batch, hid_dim/channels, step) -> (batch, step, hid_dim/channels) 
         final_hidden = hidden.permute(0, 2, 1)
         # Residual connection
         return (init_hidden + final_hidden) * self.scale
 
 
 
+# TODO: Initialization with (truncated) normal distribution with standard deviation of 0.02?
 class TransformerEncoder(Encoder):
     """Transformer encoder by Vaswani et al. (2017). 
     
     References
     ----------
     Vaswani, A., et al. 2017. Attention is All You Need. 
     """
@@ -297,15 +301,15 @@
             [TransformerEncoderBlock(hid_dim=config.hid_dim, 
                                      ff_dim=config.ff_dim, 
                                      num_heads=config.num_heads, 
                                      drop_rate=(0.0 if (k==0 and not config.use_emb2init_hid) else config.hid_drop_rate), 
                                      nonlinearity='relu') for k in range(config.num_layers)]
         )
         
-    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor):
+    def embedded2hidden(self, embedded: torch.FloatTensor, mask: torch.BoolTensor=None):
         if hasattr(self, 'emb2init_hid'):
             hidden = self.relu(self.emb2init_hid(embedded))
         else:
             hidden = embedded
         
         for tf_block in self.tf_blocks:
             hidden = tf_block(hidden, mask=mask)
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/flair.py` & `eznlp-0.2.4/eznlp/model/flair.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/image_encoder.py` & `eznlp-0.2.4/eznlp/model/image_encoder.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/model/base.py` & `eznlp-0.2.4/eznlp/model/model/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         raise NotImplementedError("Not Implemented `instantiate`")
 
 
 
 class ModelBase(torch.nn.Module):
     def __init__(self, config: ModelConfigBase):
         super().__init__()
-        for name, c in config.__dict__.items():
-            if c is not None:
+        for name in config._all_names:
+            if (c := getattr(config, name)) is not None:
                 setattr(self, name, c.instantiate())
         
     def pretrained_parameters(self):
         raise NotImplementedError("Not Implemented `pretrained_parameters`")
         
     def forward2states(self, batch: Batch):
         raise NotImplementedError("Not Implemented `forward2states`")
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/model/classifier.py` & `eznlp-0.2.4/eznlp/model/model/classifier.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/model/extractor.py` & `eznlp-0.2.4/eznlp/model/model/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             elif decoder.lower().startswith('span_attr'):
                 self.decoder = SpanAttrClassificationDecoderConfig()
             elif decoder.lower().startswith('span_rel'):
                 self.decoder = SpanRelClassificationDecoderConfig()
             elif decoder.lower().startswith('boundary'):
                 self.decoder = BoundarySelectionDecoderConfig()
             elif decoder.lower().startswith('joint_extraction'):
-                self.decoder = JointExtractionDecoderConfig()
+                self.decoder = JointExtractionDecoderConfig(ck_decoder='span_classification', rel_decoder='span_rel')
             else:
                 raise ValueError(f"Invalid `decoder`: {decoder}")
         
         super().__init__(**kwargs)
         
         
     @property
```

### Comparing `eznlp-0.2.3rc1/eznlp/model/model/image2text.py` & `eznlp-0.2.4/eznlp/model/model/image2text.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/model/text2text.py` & `eznlp-0.2.4/eznlp/model/model/text2text.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/model/nested_embedder.py` & `eznlp-0.2.4/eznlp/model/nested_embedder.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/functional.py` & `eznlp-0.2.4/eznlp/nn/functional.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/init.py` & `eznlp-0.2.4/eznlp/nn/init.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 from typing import List
+import functools
 import logging
 import torch
+import transformers
 
 logger = logging.getLogger(__name__)
 
 
 
 def reinit_embedding_(embedding: torch.nn.Embedding):
     uniform_range = (3 / embedding.weight.size(1)) ** 0.5
@@ -149,7 +151,41 @@
         elif name.startswith('weight'):
             hid_size = param.size(0) // 3
             for i, nonlinearity in enumerate(['sigmoid', 'sigmoid', 'tanh']):
                 torch.nn.init.xavier_uniform_(param.data[(hid_size*i):(hid_size*(i+1))], 
                                               gain=torch.nn.init.calculate_gain(nonlinearity))
         else:
             raise TypeError(f"Invalid GRU {gru}")
+
+
+
+def _reinit_bert_like_module(module: torch.nn.Module, std: float=0.02):
+    """Initializes each BERT module. 
+    The original Google-implemented BERT uses truncated_normal for initialization
+    cf https://github.com/pytorch/pytorch/pull/5617
+    cf https://github.com/tensorflow/tensorflow/blob/r1.8/tensorflow/python/ops/init_ops.py
+    
+    Implementation follows: `transformers/models/bert/modeling_bert.py/BertPreTrainedModel`
+    """
+    if isinstance(module, (torch.nn.Linear, torch.nn.Embedding)):
+        torch.nn.init.trunc_normal_(module.weight.data, std=std, a=-2*std, b=2*std)
+    elif isinstance(module, torch.nn.LayerNorm):
+        module.bias.data.zero_()
+        module.weight.data.fill_(1.0)
+    if isinstance(module, torch.nn.Linear) and module.bias is not None:
+        module.bias.data.zero_()
+
+
+def reinit_bert_like_(bert_like: transformers.modeling_utils.PreTrainedModel):
+    """Initializes BERT weights and prunes weights if needed. 
+    
+    Implementation follows: `transformers/modeling_utils.py/PreTrainedModel`
+    """
+    # Initialize weights
+    bert_like.apply(functools.partial(_reinit_bert_like_module, std=bert_like.config.initializer_range))
+    
+    # Prune heads if needed
+    if bert_like.config.pruned_heads:
+        bert_like.prune_heads(bert_like.config.pruned_heads)
+    
+    # Tie weights if needed
+    bert_like.tie_weights()
```

### Comparing `eznlp-0.2.3rc1/eznlp/nn/modules/aggregation.py` & `eznlp-0.2.4/eznlp/nn/modules/aggregation.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/modules/attention.py` & `eznlp-0.2.4/eznlp/nn/modules/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 import torch
 
 from ..init import reinit_layer_, reinit_vector_parameter_
 from ..utils import _nonlinearity2activation
 
 
+# TODO: Scaling factor for other scoring?
+
 class SequenceAttention(torch.nn.Module):
     """Attention over steps. 
     
     Notes
     -----
     * If `external_query` is True, the query vector is an inside parameter of this module, 
     and this module works as an aggregating layer.
```

### Comparing `eznlp-0.2.3rc1/eznlp/nn/modules/block.py` & `eznlp-0.2.4/eznlp/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/modules/crf.py` & `eznlp-0.2.4/eznlp/nn/modules/crf.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/modules/dropout.py` & `eznlp-0.2.4/eznlp/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/modules/embedding.py` & `eznlp-0.2.4/eznlp/nn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/modules/loss.py` & `eznlp-0.2.4/eznlp/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/nn/utils.py` & `eznlp-0.2.4/eznlp/nn/utils.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/token.py` & `eznlp-0.2.4/eznlp/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,48 @@
 import re
 import hanziconv
 import spacy
 import jieba
 import numpy
 
 
-zh_punctuation = "！？｡。＂＃＄％＆＇（）＊＋，－——／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏"
+# "".join([chr(i) for i in range(8211, 8232)])
+# "".join([chr(i) for i in range(12289, 12352)])
+# "".join([chr(i) for i in range(65091, 65511)])
+zh_punctuation = ("–—―‖‗‘’‚‛“”„‟†‡•‣․‥…‧" + 
+                  "、。〃〄々〆〇〈〉《》「」『』【】〒〓〔〕〖〗〘〙〚〛〜〝〞〟〠〡〢〣〤〥〦〧〨〩〪〭〮〯〫〬〰〱〲〳〴〵〶〷〸〹〺〻〼〽〾〿" + 
+                  "﹃﹄﹅﹆﹇﹈﹉﹊﹋﹌﹍﹎﹏﹐﹑﹒﹔﹕﹖﹗﹘﹙﹚﹛﹜﹝﹞﹟﹠﹡﹢﹣﹤﹥﹦﹨﹩﹪﹫" + 
+                  "！＂＃＄％＆＇（）＊＋，－．／：；＜＝＞？＠［＼］＾＿｀｛｜｝～｟｠｡｢｣､･" + 
+                  "￥￦")
+
+# Full-width characters
+fw_digits = "０１２３４５６７８９"
+fw_uppercase = "ＡＢＣＤＥＦＧＨＩＪＫＬＭＮＯＰＱＲＳＴＵＶＷＸＹＺ"
+fw_lowercase = "ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ"
+
+assert not any(c.isascii() for c in zh_punctuation + fw_digits + fw_uppercase + fw_lowercase)
+
 
 ascii_re = re.compile('[\x00-\xff]')
 lower_re = re.compile('[a-z]')
 upper_re = re.compile('[A-Z]')
 digit_re = re.compile('\d')
 punct_re = re.compile('[' + ''.join("\\" + p for p in string.punctuation) + ']')
 non_ascii_re = re.compile('[^\x00-\xff]')
+
+# CJK Unified Ideographs
+# https://zh.wikipedia.org/wiki/%E4%B8%AD%E6%97%A5%E9%9F%93%E7%B5%B1%E4%B8%80%E8%A1%A8%E6%84%8F%E6%96%87%E5%AD%97
+unihan93_re = re.compile('[\u4e00-\u9fa5〇﨎﨏﨑﨓﨔﨟﨡﨣﨤﨧﨨﨩]')
+
+zh_char_re = re.compile('[\u4e00-\u9fa5]')
 zh_punct_re = re.compile('[' + zh_punctuation + ']')
+fw_lower_re = re.compile('[' + fw_lowercase + ']')
+fw_upper_re = re.compile('[' + fw_uppercase + ']')
+fw_digit_re = re.compile('[' + fw_digits + ']')
+
 
 en_title_word_re = re.compile('[A-Z]{1}[a-z]{1,}')
 en_upper_word_re = re.compile('[A-Z]{2,}')
 en_lower_word_re = re.compile('[a-z]{2,}')
 
 en_shape2criterion = [('any_ascii', lambda x: ascii_re.search(x) is not None), 
                       ('any_non_ascii', lambda x: non_ascii_re.search(x) is not None), 
@@ -80,16 +105,16 @@
     @staticmethod
     def full2half(text):
         return text.translate(Full2Half._f2h)
     
     @staticmethod
     def half2full(text):
         return text.translate(Full2Half._h2f)
-    
-    
+
+
 
 SHORT_LEN = 3
 def _adaptive_lower(text: str):
     if len(text) <= 1 or text.islower():
         return text
     
     lowered = text.lower()
@@ -114,43 +139,43 @@
 def _text_to_num_mark(text: str, return_nan_mark: bool=True):
     if text.endswith('%'):
         text4num = text[:-1]
         is_percent = True
     else:
         text4num = text
         is_percent = False
-        
+    
     try:
         possible_value = float(text4num)
     except:
         if return_nan_mark:
             return '<nan>'
         else:
             return text
     else:
         if abs(possible_value) < 1:
             digits = 0
         else:
             digits = min(MAX_DIGITS, int(numpy.log10(abs(possible_value))) + 1)
-            
+        
         if is_percent:
             num_type = 'percent'
         elif '.' in text4num:
             num_type = 'real'
         else:
             num_type = 'int'
-            
+        
         if possible_value < 0:
             num_sign = '-'
         else:
             num_sign = ''
-            
+        
         return f"<{num_sign}{num_type}{digits}>"
-    
-    
+
+
 _number_normalizers = {'none': lambda x: x, 
                        'marks': lambda x: _text_to_num_mark(x, return_nan_mark=False), 
                        'zeros': lambda x: digit_re.sub('0', x)}
 
 
 def _pipeline(*normalizers):
     def pipeline_normalizer(x):
@@ -176,79 +201,79 @@
     
     def __init__(self, raw_text: str, pre_text_normalizer=None, 
                  case_mode='None', number_mode='None', to_half=True, to_zh_simplified=False, 
                  post_text_normalizer=None, **kwargs):
         self.raw_text = raw_text
         if callable(pre_text_normalizer):
             self.raw_text = pre_text_normalizer(self.raw_text)
-            
+        
         pipeline_normalizer = _pipeline(_case_normalizers[case_mode.lower()], 
                                         _number_normalizers[number_mode.lower()], 
                                         lambda x: Full2Half.full2half(x) if to_half else x, 
                                         lambda x: hanziconv.HanziConv.toSimplified(x) if to_zh_simplified else x)
         self.text = pipeline_normalizer(self.raw_text)
         if callable(post_text_normalizer):
             self.text = post_text_normalizer(self.text)
         
         for k, v in kwargs.items():
             setattr(self, k, v)
         
-
+        
     def __eq__(self, other):
         return isinstance(other, Token) and self.raw_text == other.raw_text and self.text == other.text
         
     def __len__(self):
         return len(self.raw_text)
-    
+        
     def __repr__(self):
         return self.raw_text
-    
+        
     @property    
     def prefix_2(self):
         return self.raw_text[:2]
-    
+        
     @property
     def prefix_3(self):
         return self.raw_text[:3]
-    
+        
     @property
     def prefix_4(self):
         return self.raw_text[:4]
-    
+        
     @property
     def prefix_5(self):
         return self.raw_text[:5]
-    
+        
     @property
     def suffix_2(self):
         return self.raw_text[-2:]
-    
+        
     @property
     def suffix_3(self):
         return self.raw_text[-3:]
-    
+        
     @property
     def suffix_4(self):
         return self.raw_text[-4:]
-    
+        
     @property
     def suffix_5(self):
         return self.raw_text[-5:]
-    
+        
     @property
     def num_mark(self):
         return _text_to_num_mark(self.raw_text, return_nan_mark=True)
         
     @property
     def en_pattern(self):
         feature = upper_re.sub('A', self.raw_text)
         feature = lower_re.sub('a', feature)
         feature = digit_re.sub('0', feature)
         return feature
-    
+        
     @property
     def en_pattern_sum(self):
         feature = self.en_pattern
         feature = re.sub('A+', 'A', feature)
         feature = re.sub('a+', 'a', feature)
         feature = re.sub('0+', '0', feature)
         return feature
@@ -256,17 +281,17 @@
     @property
     def en_shape_features(self):
         return numpy.array([criterion(self.raw_text) for criterion in en_shape2criterion.values()])
         
     @property
     def zh_shape_features(self):
         return None
-    
-    
-    
+
+
+
 class TokenSequence(object):
     """A wrapper of token list, providing sequential attribute access to all tokens. 
     
     """
     _softword_idx2tag = ['B', 'M', 'E', 'S']
     _softword_tag2idx = {t: i for i, t in enumerate(_softword_idx2tag)}
     
@@ -277,57 +302,59 @@
         self.none_token = none_token
         
     def __getattr__(self, name):
         # NOTE: `__attr__` method is only invoked if the attribute wasn't found the usual ways, so 
         # it is good for implementing a fallback for missing attributes. While, `__getattribute__`
         # is invoked before looking at the actual attributes on the object. 
         # See: https://stackoverflow.com/questions/3278077/difference-between-getattr-vs-getattribute
-        if hasattr(self.token_list[0], name):
+        if len(self.token_list) == 0: 
+            # Unable to check attribute existence, return an empty list anyway
+            return []
+        elif hasattr(self.token_list[0], name):
             return [getattr(tok, name) for tok in self.token_list]
         else:
             raise AttributeError(f"{self.__class__.__name__} has no attribute {name}")
         
         
     def __eq__(self, other):
         return isinstance(other, TokenSequence) and self.__getstate__() == other.__getstate__()
-    
+        
     def __len__(self):
         return len(self.token_list)
-    
+        
     def __repr__(self):
         return repr(self.token_list)
-    
-    def __getstate__(self):
-        return {'token_list': self.token_list, 
-                'token_sep': self.token_sep, 
+        
+    @property
+    def _tokens_kwargs(self):
+        return {'token_sep': self.token_sep, 
                 'pad_token': self.pad_token, 
                 'none_token': self.none_token}
         
+    def __getstate__(self):
+        return {'token_list': self.token_list, **self._tokens_kwargs}
+        
     def __setstate__(self, state: dict):
         self.__dict__.update(state)
         
         
     def __getitem__(self, i):
         if isinstance(i, int):
             return self.token_list[i]
         elif isinstance(i, slice):
-            return TokenSequence(self.token_list[i], 
-                                 token_sep=self.token_sep, 
-                                 pad_token=self.pad_token, 
-                                 none_token=self.none_token)
+            return TokenSequence(self.token_list[i], **self._tokens_kwargs)
         else:
             raise TypeError(f"Invalid subscript type of {i}")
-            
+        
     def __add__(self, other):
-        return TokenSequence(self.token_list + other.token_list, 
-                             token_sep=self.token_sep, 
-                             pad_token=self.pad_token, 
-                             none_token=self.none_token)
-    
-    
+        assert isinstance(other, TokenSequence)
+        assert other._tokens_kwargs == self._tokens_kwargs
+        return TokenSequence(self.token_list + other.token_list, **self._tokens_kwargs)
+        
+        
     def build_pseudo_boundaries(self, sep_width: int=None):
         if sep_width is None:
             sep_width = len(self.token_sep)
         
         token_lens = numpy.array([len(tok) for tok in self.token_list])
         self.end = numpy.cumsum(token_lens + sep_width) - sep_width
         self.start = self.end - token_lens
@@ -349,48 +376,48 @@
             if word_end - word_start == 1:
                 self.softword[word_start][self._softword_tag2idx['S']] = True
             else:
                 self.softword[word_start][self._softword_tag2idx['B']] = True
                 self.softword[word_end-1][self._softword_tag2idx['E']] = True
                 for k in range(word_start+1, word_end-1):
                     self.softword[k][self._softword_tag2idx['M']] = True
-                    
-                    
+        
+        
     def build_softlexicons(self, tokenize_callback, **kwargs):
         self._assert_for_softwords(tokenize_callback)
         
         self.softlexicon = [[[] for t in self._softword_idx2tag] for tok in self.token_list]
         
         for word_text, word_start, word_end in tokenize_callback(self.token_sep.join(self.raw_text), **kwargs):
             if word_end - word_start == 1:
                 self.softlexicon[word_start][self._softword_tag2idx['S']].append(word_text)
             else:
                 self.softlexicon[word_start][self._softword_tag2idx['B']].append(word_text)
                 self.softlexicon[word_end-1][self._softword_tag2idx['E']].append(word_text)
                 for k in range(word_start+1, word_end-1):
                     self.softlexicon[k][self._softword_tag2idx['M']].append(word_text)
-                    
+        
         # Add a special token to empty word sets
         for word_sets in self.softlexicon:
             for word_set in word_sets:
                 if len(word_set) == 0:
                     word_set.append(self.none_token)
-                    
-                    
+        
+        
     @cached_property
     def bigram(self):
         unigram = self.text
         return [self.token_sep.join(gram) for gram in zip(unigram, unigram[1:]+[self.pad_token])]
-    
+        
     @cached_property
     def trigram(self):
         unigram = self.text
         return [self.token_sep.join(gram) for gram in zip(unigram, unigram[1:]+[self.pad_token], unigram[2:]+[self.pad_token, self.pad_token])]
         
-    
+        
     def spans_within_max_length(self, max_len: int):
         total_len = len(self.token_list)
         slice_start = 0
         
         while True:
             if total_len - slice_start <= max_len:
                 yield slice(slice_start, total_len)
@@ -399,55 +426,55 @@
                 slice_end = slice_start + max_len
                 while not self.token_list[slice_end-1].text in ('.', '?', '!', ';'):
                     slice_end -= 1
                     if slice_end <= slice_start:
                         raise ValueError(f"Cannot find proper slices in {self.token_list[slice_start:slice_start+max_len]}")
                 yield slice(slice_start, slice_end)
                 slice_start = slice_end
-                
-                
+        
+        
     def attach_additional_tags(self, additional_tags: dict=None, additional_tok2tags: list=None):
         """
         
         Parameters
         ----------
         additional_tags : dict of lists, optional
             {tag_name: tags, ...}. 
         additional_tok2tags : list of tuples, optional
             [(tag_name: str, tok2tag: dict), ...]. 
         """
         if additional_tags is not None:
             for tag_name, tags in additional_tags.items():
                 for tok, tag in zip(self.token_list, tags):
                     setattr(tok, tag_name, tag)
-                    
+        
         if additional_tok2tags is not None:
             for tag_name, tok2tag in additional_tok2tags:
                 for tok in self.token_list:
                     setattr(tok, tag_name, tok2tag.get(tok.text, tok2tag['<unk>']))
-                    
+        
         return self
-    
-    
+        
+        
     @classmethod
     def from_tokenized_text(cls, tokenized_text: List[str], additional_tags=None, additional_tok2tags=None, 
                             token_sep=" ", pad_token="<pad>", none_token="<none>", **kwargs):
         """Build `TokenSequence` from tokenized text. 
         
         Parameters
         ----------
         tokenized_text: List[str]
             A list of tokenized text. 
         """
         token_list = [Token(tok_text, **kwargs) for tok_text in tokenized_text]
         tokens = cls(token_list, token_sep=token_sep, pad_token=pad_token, none_token=none_token)
         tokens.attach_additional_tags(additional_tags=additional_tags, additional_tok2tags=additional_tok2tags)
         return tokens
-    
-    
+        
+        
     @classmethod
     def from_raw_text(cls, raw_text: str, tokenize_callback=None, additional_tok2tags=None, 
                       token_sep=" ", pad_token="<pad>", none_token="<none>", **kwargs):
         """Build `TokenSequence` from raw text. 
         
         Parameters
         ----------
```

### Comparing `eznlp-0.2.3rc1/eznlp/training/options.py` & `eznlp-0.2.4/eznlp/training/options.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/training/trainer.py` & `eznlp-0.2.4/eznlp/training/trainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def __init__(self, 
                  model: ModelBase, 
                  optimizer: torch.optim.Optimizer=None, 
                  scheduler: torch.optim.lr_scheduler._LRScheduler=None, 
                  schedule_by_step: bool=False, 
                  num_grad_acc_steps: int=None, 
                  device: torch.device=None, 
+                 non_blocking: bool=False,
                  grad_clip: float=None, 
                  use_amp: bool=False):
         self.model = model
         if hasattr(self.model, 'decoder'):
             self.num_metrics = self.model.decoder.num_metrics
         else:
             self.num_metrics = 0
@@ -43,14 +44,15 @@
         self.scheduler = scheduler
         self.schedule_by_step = schedule_by_step
         self.num_grad_acc_steps = num_grad_acc_steps if isinstance(num_grad_acc_steps, int) and num_grad_acc_steps > 0 else 1
         self.num_steps = 0
         
         assert device is not None
         self.device = device
+        self.non_blocking = non_blocking
         self.grad_clip = grad_clip
         self.use_amp = use_amp
         self.scaler = torch.cuda.amp.GradScaler(enabled=use_amp)
         
         
     def forward_batch(self, batch: Batch):
         """
@@ -115,15 +117,15 @@
         
         dataloader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=False, collate_fn=dataset.collate)
         
         self.model.eval()
         set_y_pred = [[] for k in range(self.num_metrics)]
         with torch.no_grad():
             for batch in dataloader:
-                batch = batch.to(self.device)
+                batch = batch.to(self.device, non_blocking=self.non_blocking)
                 
                 # `dataset` may not have ground-truths, so avoid computing loss here 
                 if beam_size <= 1:
                     states = self.model.forward2states(batch)
                     batch_y_pred = self.model.decoder._unsqueezed_decode(batch, **states)
                     for k in range(self.num_metrics):
                         set_y_pred[k].extend(batch_y_pred[k])
@@ -146,15 +148,15 @@
         """
         self.model.train()
         
         epoch_losses = []
         epoch_y_gold = [[] for k in range(self.num_metrics)]
         epoch_y_pred = [[] for k in range(self.num_metrics)]
         for batch in dataloader:
-            batch = batch.to(self.device)
+            batch = batch.to(self.device, non_blocking=self.non_blocking)
             with torch.cuda.amp.autocast(enabled=self.use_amp):
                 loss_with_possible_y_pred = self.forward_batch(batch)
             
             if self.num_metrics == 0:
                 loss = loss_with_possible_y_pred
             else:
                 loss, *batch_y_pred = loss_with_possible_y_pred
@@ -178,15 +180,15 @@
         self.model.eval()
         
         epoch_losses = []
         epoch_y_gold = [[] for k in range(self.num_metrics)]
         epoch_y_pred = [[] for k in range(self.num_metrics)]
         with torch.no_grad():
             for batch in dataloader:
-                batch = batch.to(self.device)
+                batch = batch.to(self.device, non_blocking=self.non_blocking)
                 loss_with_possible_y_pred = self.forward_batch(batch)
                 
                 if self.num_metrics == 0:
                     loss = loss_with_possible_y_pred
                 else:
                     loss, *batch_y_pred = loss_with_possible_y_pred
                     batch_y_gold = self.model.decoder._unsqueezed_retrieve(batch)
@@ -232,15 +234,15 @@
         save_callback
             The callback function to save model.
         save_by_loss: bool
             Whether to save by loss or other metrics. The metric must hold that it is better if higher, e.g., accuracy or F1. 
         """
         max_steps = numpy.inf if max_steps is None else max_steps
         disp_every_steps = len(train_loader) if disp_every_steps is None else disp_every_steps
-        eval_every_steps = len(train_loader) if eval_every_steps is None else eval_every_steps
+        eval_every_steps = disp_every_steps  if eval_every_steps is None else eval_every_steps
         if eval_every_steps % disp_every_steps != 0:
             raise ValueError(f"`eval_every_steps` {eval_every_steps} should be multiples of `disp_every_steps` {disp_every_steps}")
         
         self.model.train()
         
         best_dev_loss = numpy.inf
         best_dev_metric = -numpy.inf
@@ -250,15 +252,15 @@
         train_y_pred = [[] for k in range(self.num_metrics)]
         eidx, sidx = 0, 0
         done_training = False
         t0 = time.time()
         
         while eidx < num_epochs:
             for batch in train_loader:
-                batch = batch.to(self.device)
+                batch = batch.to(self.device, non_blocking=self.non_blocking)
                 with torch.cuda.amp.autocast(enabled=self.use_amp):
                     loss_with_possible_y_pred = self.forward_batch(batch)
                     
                 if self.num_metrics == 0:
                     loss = loss_with_possible_y_pred
                 else:
                     loss, *batch_y_pred = loss_with_possible_y_pred
@@ -318,14 +320,16 @@
                         else:
                             self.scheduler.step()
                     
                     self.model.train()
                     t0 = time.time()
                 
                 if (sidx+1) % eval_every_steps == 0 and dev_loader is None:
+                    # Always save the model if `dev_loader` is None
+                    # Save multiple models by accordlingly defining `save_callback`
                     if save_callback is not None:
                         save_callback(self.model)
                 
                 if (sidx+1) >= max_steps:
                     done_training = True
                     break
                 sidx += 1
```

### Comparing `eznlp-0.2.3rc1/eznlp/training/utils.py` & `eznlp-0.2.4/eznlp/training/utils.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/utils/algorithms.py` & `eznlp-0.2.4/eznlp/utils/algorithms.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/utils/chunk.py` & `eznlp-0.2.4/eznlp/utils/chunk.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,58 +2,81 @@
 from typing import List
 import re
 
 from ..token import TokenSequence
 from . import find_ascending
 
 
-def is_overlapped(chunk1: tuple, chunk2: tuple):
+FLAT = 0       # Flat entities
+NESTED = 1     # Nested entities
+ARBITRARY = 2  # Arbitrarily overlapping entities
+
+
+def _is_overlapping(chunk1: tuple, chunk2: tuple):
+    # `NESTED` or `ARBITRARY`
     (_, s1, e1), (_, s2, e2) = chunk1, chunk2
     return (s1 < e2 and s2 < e1)
 
 
-def is_nested(chunk1: tuple, chunk2: tuple):
+def _is_ordered_nested(chunk1: tuple, chunk2: tuple):
+    # `chunk1` is nested in `chunk2`
+    (_, s1, e1), (_, s2, e2) = chunk1, chunk2
+    return (s2 <= s1 and e1 <= e2)
+
+
+def _is_nested(chunk1: tuple, chunk2: tuple):
+    # `NESTED`
     (_, s1, e1), (_, s2, e2) = chunk1, chunk2
     return (s1 <= s2 and e2 <= e1) or (s2 <= s1 and e1 <= e2)
 
 
-def is_clashed(chunk1: tuple, chunk2: tuple, allow_nested: bool=True):
-    if allow_nested:
-        return is_overlapped(chunk1, chunk2) and not is_nested(chunk1, chunk2)
+def _is_clashed(chunk1: tuple, chunk2: tuple, allow_level: int=NESTED):
+    if allow_level == FLAT:
+        return _is_overlapping(chunk1, chunk2)
+    elif allow_level == NESTED:
+        return _is_overlapping(chunk1, chunk2) and not _is_nested(chunk1, chunk2)
     else:
-        return is_overlapped(chunk1, chunk2)
+        return False
 
 
-def filter_clashed_by_priority(chunks: List[tuple], allow_nested: bool=True):
+def filter_clashed_by_priority(chunks: List[tuple], allow_level: int=NESTED):
     filtered_chunks = []
     for ck in chunks:
-        if all(not is_clashed(ck, ex_ck, allow_nested=allow_nested) for ex_ck in filtered_chunks):
+        if all(not _is_clashed(ck, ex_ck, allow_level=allow_level) for ex_ck in filtered_chunks):
             filtered_chunks.append(ck)
-            
     return filtered_chunks
 
 
-def detect_nested(chunks: List[tuple]):
+def detect_overlapping_level(chunks: List[tuple]):
+    level = FLAT
     for i, ck1 in enumerate(chunks):
         for ck2 in chunks[i+1:]:
-            if is_nested(ck1, ck2):
-                return True
-    return False
+            if _is_nested(ck1, ck2):
+                level = NESTED
+            elif _is_overlapping(ck1, ck2):
+                # Non-nested overlapping -> `ARBITRARY`
+                return ARBITRARY
+    return level
+
+
+def count_nested(chunks: List[tuple]):
+    return sum(any(ck1[1:] != ck2[1:] and _is_ordered_nested(ck1, ck2) for ck2 in chunks) for ck1 in chunks)
 
 
 def chunk_pair_distance(chunk1: tuple, chunk2: tuple, overlap_distance: int=-1):
     (_, s1, e1), (_, s2, e2) = chunk1, chunk2
     if e1 <= s2:
         return s2 - e1
     elif e2 <= s1:
         return s1 - e2
     else:
         return overlap_distance
 
 
+
 class TextChunksTranslator(object):
     """The translator between chunks and text-chunks. 
     
     Args
     ----
     chunks: list
         list of (chunk_type, chunk_start, chunk_end).
```

### Comparing `eznlp-0.2.3rc1/eznlp/utils/segmentation.py` & `eznlp-0.2.4/eznlp/utils/segmentation.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/utils/transition.py` & `eznlp-0.2.4/eznlp/utils/transition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 from typing import List
 import os
 import re
 from collections import Counter
 import pandas
 
+from ..token import zh_char_re, zh_punct_re
+
 
 class ChunksTagsTranslator(object):
     """The translator between chunks and tags. 
     
     Args
     ----
     chunks: list
@@ -19,15 +21,15 @@
         Token sequence object. 
         
     References
     ----------
     https://github.com/chakki-works/seqeval
     """
     def __init__(self, scheme='BIOES', sep: str='-', breaking_for_types: bool=True):
-        assert scheme in ('BIO1', 'BIO2', 'BIOES', 'BMES', 'BILOU', 'OntoNotes')
+        assert scheme in ('BIO1', 'BIO2', 'BIOES', 'BMES', 'BILOU', 'OntoNotes', 'wwm')
         self.scheme = scheme
         
         dirname = os.path.dirname(__file__)
         sheet_name = 'BIOES' if scheme in ('BMES', 'BILOU') else scheme
         trans = pandas.read_excel(f"{dirname}/transition.xlsx", sheet_name=sheet_name, 
                                   usecols=['from_tag', 'to_tag', 'legal', 'end_of_chunk', 'start_of_chunk'])
         
@@ -206,7 +208,31 @@
             prev_tag = this_tag
             
             
         if self.trans[(prev_tag, '(*')]['end_of_chunk']:
             chunks.append((chunk_type, chunk_start, len(tags)))
             
         return chunks
+
+
+
+def _token2wwm_tag(tok: str, subword_prefix: str='##'):
+    if tok.startswith('[') and tok.endswith(']'):
+        return 'SP-SP'
+    
+    # Theoretically, Chinese characters never follow `##`
+    # Chinese punctuations belong to `ETC`, and may follow `##`
+    
+    if tok.startswith(subword_prefix):
+        if tok[2:].isascii():
+            return '##EN-EN'  # The returning prefix `##` corresponds to that in `transition.xlsx`
+        elif zh_char_re.fullmatch(tok[2:]):  # zh_punct_re.fullmatch(tok[2:])
+            return '##ZH-ZH'
+        else:
+            return '##ETC-ETC'
+    else:
+        if tok.isascii():
+            return 'EN-EN'
+        elif zh_char_re.fullmatch(tok):
+            return 'ZH-ZH'
+        else:
+            return 'ETC-ETC'
```

### Comparing `eznlp-0.2.3rc1/eznlp/vectors.py` & `eznlp-0.2.4/eznlp/vectors.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/vocab.py` & `eznlp-0.2.4/eznlp/vocab.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp/wrapper.py` & `eznlp-0.2.4/eznlp/wrapper.py`

 * *Files identical despite different names*

### Comparing `eznlp-0.2.3rc1/eznlp.egg-info/SOURCES.txt` & `eznlp-0.2.4/eznlp.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,59 +19,68 @@
 eznlp/io/base.py
 eznlp/io/brat.py
 eznlp/io/category_folder.py
 eznlp/io/chip.py
 eznlp/io/conll.py
 eznlp/io/json.py
 eznlp/io/processing.py
+eznlp/io/raw_text.py
 eznlp/io/src2trg.py
 eznlp/io/tabular.py
-eznlp/language_modeling/__init__.py
-eznlp/language_modeling/dataset.py
-eznlp/language_modeling/model.py
-eznlp/language_modeling/trainer.py
 eznlp/model/__init__.py
 eznlp/model/bert_like.py
 eznlp/model/elmo.py
 eznlp/model/embedder.py
 eznlp/model/encoder.py
 eznlp/model/flair.py
 eznlp/model/image_encoder.py
 eznlp/model/nested_embedder.py
+eznlp/model/span_bert_like.py
 eznlp/model/decoder/__init__.py
 eznlp/model/decoder/base.py
+eznlp/model/decoder/boundaries.py
 eznlp/model/decoder/boundary_selection.py
+eznlp/model/decoder/chunks.py
 eznlp/model/decoder/generator.py
 eznlp/model/decoder/joint_extraction.py
 eznlp/model/decoder/sequence_tagging.py
 eznlp/model/decoder/span_attr_classification.py
 eznlp/model/decoder/span_classification.py
 eznlp/model/decoder/span_rel_classification.py
+eznlp/model/decoder/specific_span_classification.py
+eznlp/model/decoder/specific_span_rel_classification.py
+eznlp/model/decoder/specific_span_sparse_rel_classification.py
 eznlp/model/decoder/text_classification.py
 eznlp/model/model/__init__.py
 eznlp/model/model/base.py
 eznlp/model/model/classifier.py
 eznlp/model/model/extractor.py
 eznlp/model/model/image2text.py
+eznlp/model/model/specific_span_extractor.py
 eznlp/model/model/text2text.py
 eznlp/nn/__init__.py
 eznlp/nn/functional.py
 eznlp/nn/init.py
 eznlp/nn/utils.py
 eznlp/nn/modules/__init__.py
 eznlp/nn/modules/aggregation.py
 eznlp/nn/modules/attention.py
 eznlp/nn/modules/block.py
 eznlp/nn/modules/crf.py
 eznlp/nn/modules/dropout.py
 eznlp/nn/modules/embedding.py
 eznlp/nn/modules/loss.py
+eznlp/nn/modules/query_bert_like.py
+eznlp/plm/__init__.py
+eznlp/plm/base.py
+eznlp/plm/mlm.py
 eznlp/training/__init__.py
 eznlp/training/evaluation.py
 eznlp/training/options.py
+eznlp/training/plm_trainer.py
 eznlp/training/trainer.py
 eznlp/training/utils.py
 eznlp/utils/__init__.py
 eznlp/utils/algorithms.py
 eznlp/utils/chunk.py
 eznlp/utils/segmentation.py
 eznlp/utils/transition.py
```

### Comparing `eznlp-0.2.3rc1/setup.py` & `eznlp-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,22 +20,22 @@
       author_email='enwei.zhu@outlook.com',
       license='Apache',
       keywords='torch',
       packages=find_packages(include=["eznlp", "eznlp.*"]),
       include_package_data=True,
       install_requires=["torch>=1.7.1",
                         "torchvision>=0.8.2",
-                        "nltk>=3.5",
+                        "flair==0.8",
+                        "allennlp==2.1.0",
                         "transformers==4.3.2",
-                        "tokenizers==0.10.1", 
-                        "allennlp==2.0.1", 
-                        "flair==0.7",
-                        "truecase==0.0.12", 
-                        "hanziconv==0.3.2", 
+                        "tokenizers==0.10.1",
+                        "nltk>=3.5",
+                        "truecase==0.0.12",
+                        "hanziconv==0.3.2",
                         "spacy>=2.3.2",
-                        "jieba>=0.42.1", 
+                        "jieba>=0.42.1",
                         "numpy>=1.18.5",
                         "pandas>=1.0.5", 
                         "matplotlib>=3.2.2"],
-      tests_require=["torchtext>=0.8.1", 
+      tests_require=["torchtext>=0.8.1",
                      "pytorch-crf>=0.7.2"], 
       python_requires='>=3.8,<4')
```

