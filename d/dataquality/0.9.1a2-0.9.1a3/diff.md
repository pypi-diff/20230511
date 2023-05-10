# Comparing `tmp/dataquality-0.9.1a2.tar.gz` & `tmp/dataquality-0.9.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.9.1a2.tar", last modified: Thu May  4 22:23:35 2023, max compression
+gzip compressed data, was "dataquality-0.9.1a3.tar", last modified: Thu May  4 22:29:03 2023, max compression
```

## Comparing `dataquality-0.9.1a2.tar` & `dataquality-0.9.1a3.tar`

### file list

```diff
@@ -1,237 +1,237 @@
--rw-r--r--   0        0        0       99 2023-02-16 18:20:37.484786 dataquality-0.9.1a2/.coveragerc
--rw-r--r--   0        0        0      131 2023-02-16 18:20:37.484963 dataquality-0.9.1a2/.editorconfig
--rw-r--r--   0        0        0      179 2023-03-06 18:27:08.322809 dataquality-0.9.1a2/.flake8
--rw-r--r--   0        0        0       19 2023-04-28 02:34:07.405536 dataquality-0.9.1a2/.github/CODEOWNERS
--rw-r--r--   0        0        0      924 2023-02-16 18:20:37.485592 dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      590 2023-02-16 18:20:37.485749 dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/doc.md
--rw-r--r--   0        0        0      700 2023-02-16 18:20:37.485896 dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      542 2023-02-16 18:20:37.486033 dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1169 2023-02-16 18:20:37.486183 dataquality-0.9.1a2/.github/pull_request_template.md
--rw-r--r--   0        0        0      950 2023-04-14 09:39:59.465229 dataquality-0.9.1a2/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      525 2023-04-14 09:39:59.466024 dataquality-0.9.1a2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      890 2023-04-14 09:39:59.467112 dataquality-0.9.1a2/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2418 2023-05-03 22:49:30.076353 dataquality-0.9.1a2/.gitignore
--rw-r--r--   0        0        0        6 2023-02-16 18:20:37.487014 dataquality-0.9.1a2/.python-version
--rw-r--r--   0        0        0     8078 2023-02-16 18:20:37.487229 dataquality-0.9.1a2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1066 2023-02-16 18:20:37.487400 dataquality-0.9.1a2/LICENSE
--rw-r--r--   0        0        0     4437 2023-02-16 18:20:37.487564 dataquality-0.9.1a2/README.md
--rw-r--r--   0        0        0     6012 2023-05-04 22:23:33.346011 dataquality-0.9.1a2/dataquality/__init__.py
--rw-r--r--   0        0        0     8461 2023-05-04 02:23:06.506407 dataquality-0.9.1a2/dataquality/analytics.py
--rw-r--r--   0        0        0        0 2023-04-07 07:52:09.639242 dataquality-0.9.1a2/dataquality/clients/__init__.py
--rw-r--r--   0        0        0    33867 2023-05-04 02:23:06.529362 dataquality-0.9.1a2/dataquality/clients/api.py
--rw-r--r--   0        0        0     8187 2023-05-04 02:23:06.516492 dataquality-0.9.1a2/dataquality/clients/objectstore.py
--rw-r--r--   0        0        0     1848 2023-04-07 07:52:09.644595 dataquality-0.9.1a2/dataquality/core/__init__.py
--rw-r--r--   0        0        0     8843 2023-05-04 02:23:06.793133 dataquality-0.9.1a2/dataquality/core/_config.py
--rw-r--r--   0        0        0     3104 2023-05-04 02:23:06.759652 dataquality-0.9.1a2/dataquality/core/auth.py
--rw-r--r--   0        0        0     6499 2023-05-04 22:17:22.621387 dataquality-0.9.1a2/dataquality/core/finish.py
--rw-r--r--   0        0        0     7026 2023-05-04 02:23:06.783167 dataquality-0.9.1a2/dataquality/core/init.py
--rw-r--r--   0        0        0    21161 2023-05-04 02:23:06.771183 dataquality-0.9.1a2/dataquality/core/log.py
--rw-r--r--   0        0        0     7039 2023-05-04 02:23:06.799371 dataquality-0.9.1a2/dataquality/core/report.py
--rw-r--r--   0        0        0        0 2023-04-07 07:52:09.650876 dataquality-0.9.1a2/dataquality/dq_auto/__init__.py
--rw-r--r--   0        0        0    10473 2023-05-04 22:23:21.461937 dataquality-0.9.1a2/dataquality/dq_auto/auto.py
--rw-r--r--   0        0        0     4158 2023-05-04 02:23:07.126817 dataquality-0.9.1a2/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0        0        0     7710 2023-05-04 22:10:32.335211 dataquality-0.9.1a2/dataquality/dq_auto/ner.py
--rw-r--r--   0        0        0     4265 2023-05-04 02:23:07.123093 dataquality-0.9.1a2/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0        0        0     1594 2023-05-04 02:23:07.142858 dataquality-0.9.1a2/dataquality/dq_auto/notebook.py
--rw-r--r--   0        0        0     3559 2023-05-04 02:23:07.146263 dataquality-0.9.1a2/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0        0        0    11797 2023-05-04 22:10:43.269244 dataquality-0.9.1a2/dataquality/dq_auto/text_classification.py
--rw-r--r--   0        0        0    13139 2023-05-04 02:23:06.545657 dataquality-0.9.1a2/dataquality/dq_start/__init__.py
--rw-r--r--   0        0        0     4498 2023-05-04 02:23:06.465858 dataquality-0.9.1a2/dataquality/dqyolo.py
--rw-r--r--   0        0        0      293 2023-04-07 07:52:09.656391 dataquality-0.9.1a2/dataquality/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-07 07:52:09.656535 dataquality-0.9.1a2/dataquality/integrations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 22:49:30.079624 dataquality-0.9.1a2/dataquality/integrations/cv/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 22:49:30.079930 dataquality-0.9.1a2/dataquality/integrations/cv/torch/__init__.py
--rw-r--r--   0        0        0    20077 2023-05-04 22:17:22.622375 dataquality-0.9.1a2/dataquality/integrations/cv/torch/semantic_segmentation.py
--rw-r--r--   0        0        0    15575 2023-05-04 02:23:07.110977 dataquality-0.9.1a2/dataquality/integrations/experimental/keras.py
--rw-r--r--   0        0        0    14914 2023-05-04 02:23:07.045645 dataquality-0.9.1a2/dataquality/integrations/fastai.py
--rw-r--r--   0        0        0    10024 2023-05-04 02:23:07.102392 dataquality-0.9.1a2/dataquality/integrations/hf.py
--rw-r--r--   0        0        0     4375 2023-05-04 02:23:07.050094 dataquality-0.9.1a2/dataquality/integrations/keras.py
--rw-r--r--   0        0        0    26831 2023-05-04 02:23:07.079437 dataquality-0.9.1a2/dataquality/integrations/spacy.py
--rw-r--r--   0        0        0    12787 2023-05-04 02:23:07.084631 dataquality-0.9.1a2/dataquality/integrations/torch.py
--rw-r--r--   0        0        0    12375 2023-05-04 22:06:55.080834 dataquality-0.9.1a2/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0        0        0    16907 2023-05-04 02:23:07.095450 dataquality-0.9.1a2/dataquality/integrations/ultralytics.py
--rw-r--r--   0        0        0       95 2023-04-07 07:52:09.664245 dataquality-0.9.1a2/dataquality/loggers/__init__.py
--rw-r--r--   0        0        0    13292 2023-05-04 02:23:06.570857 dataquality-0.9.1a2/dataquality/loggers/base_logger.py
--rw-r--r--   0        0        0      517 2023-05-04 02:23:06.665914 dataquality-0.9.1a2/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0        0        0    26263 2023-05-04 22:17:22.623202 dataquality-0.9.1a2/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0        0        0    10393 2023-05-04 02:23:06.662586 dataquality-0.9.1a2/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0        0        0     9368 2023-05-04 02:23:06.719013 dataquality-0.9.1a2/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0        0        0     2768 2023-05-04 22:17:22.623829 dataquality-0.9.1a2/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0        0        0     9864 2023-05-04 02:23:06.651100 dataquality-0.9.1a2/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0        0        0    20661 2023-05-04 02:23:06.678041 dataquality-0.9.1a2/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0        0        0    14941 2023-05-04 02:23:06.687072 dataquality-0.9.1a2/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0        0        0    31885 2023-05-04 02:23:06.699619 dataquality-0.9.1a2/dataquality/loggers/data_logger/text_ner.py
--rw-r--r--   0        0        0        0 2023-04-07 07:52:09.669046 dataquality-0.9.1a2/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0        0        0     1910 2023-05-04 22:17:22.624592 dataquality-0.9.1a2/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0        0        0      473 2023-04-07 07:52:09.669969 dataquality-0.9.1a2/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0        0        0      537 2023-04-14 09:39:59.476862 dataquality-0.9.1a2/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0        0        0      226 2023-05-03 22:49:30.083124 dataquality-0.9.1a2/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0        0        0      398 2023-05-03 22:49:30.083397 dataquality-0.9.1a2/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0        0        0      958 2023-05-04 02:23:06.738772 dataquality-0.9.1a2/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0        0        0     1510 2023-05-04 02:23:06.741859 dataquality-0.9.1a2/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0        0        0     1608 2023-05-04 02:23:06.745185 dataquality-0.9.1a2/dataquality/loggers/logger_config/text_ner.py
--rw-r--r--   0        0        0      420 2023-05-04 02:23:06.588494 dataquality-0.9.1a2/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0        0        0     7510 2023-05-04 02:23:06.637489 dataquality-0.9.1a2/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0        0        0     3309 2023-05-04 02:23:06.583977 dataquality-0.9.1a2/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0        0        0     8975 2023-05-04 02:23:06.627055 dataquality-0.9.1a2/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0        0        0     6463 2023-05-04 22:17:22.624998 dataquality-0.9.1a2/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0        0        0      519 2023-05-03 22:49:30.084436 dataquality-0.9.1a2/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0        0        0     7555 2023-05-04 02:23:06.598643 dataquality-0.9.1a2/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0        0        0     9120 2023-05-04 02:23:06.605413 dataquality-0.9.1a2/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0        0        0    32052 2023-05-04 02:23:06.616819 dataquality-0.9.1a2/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0        0        0    28673 2023-05-04 02:23:06.482946 dataquality-0.9.1a2/dataquality/metrics.py
--rw-r--r--   0        0        0      165 2023-04-07 07:52:09.676633 dataquality-0.9.1a2/dataquality/schemas/__init__.py
--rw-r--r--   0        0        0     8361 2023-05-04 02:23:07.012740 dataquality-0.9.1a2/dataquality/schemas/condition.py
--rw-r--r--   0        0        0      569 2023-05-04 02:23:06.968028 dataquality-0.9.1a2/dataquality/schemas/dataframe.py
--rw-r--r--   0        0        0     4382 2023-05-04 02:23:07.004539 dataquality-0.9.1a2/dataquality/schemas/edit.py
--rw-r--r--   0        0        0      662 2023-04-07 07:52:09.677611 dataquality-0.9.1a2/dataquality/schemas/hf.py
--rw-r--r--   0        0        0      118 2023-05-04 02:23:06.970328 dataquality-0.9.1a2/dataquality/schemas/job.py
--rw-r--r--   0        0        0     5241 2023-05-04 02:23:06.964247 dataquality-0.9.1a2/dataquality/schemas/metrics.py
--rw-r--r--   0        0        0      165 2023-05-04 02:23:07.006560 dataquality-0.9.1a2/dataquality/schemas/model.py
--rw-r--r--   0        0        0      992 2023-05-04 02:23:07.015866 dataquality-0.9.1a2/dataquality/schemas/ner.py
--rw-r--r--   0        0        0      617 2023-05-04 02:23:07.027724 dataquality-0.9.1a2/dataquality/schemas/report.py
--rw-r--r--   0        0        0      287 2023-04-07 07:52:09.678943 dataquality-0.9.1a2/dataquality/schemas/request_type.py
--rw-r--r--   0        0        0     1491 2023-05-04 02:23:06.973737 dataquality-0.9.1a2/dataquality/schemas/route.py
--rw-r--r--   0        0        0     2550 2023-05-04 22:17:22.626499 dataquality-0.9.1a2/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0        0        0      992 2023-05-04 02:23:07.018585 dataquality-0.9.1a2/dataquality/schemas/split.py
--rw-r--r--   0        0        0     1055 2023-05-04 02:23:07.021496 dataquality-0.9.1a2/dataquality/schemas/task_type.py
--rw-r--r--   0        0        0      740 2023-05-04 22:17:22.627338 dataquality-0.9.1a2/dataquality/schemas/torch.py
--rw-r--r--   0        0        0      222 2023-04-07 07:52:09.680124 dataquality-0.9.1a2/dataquality/utils/__init__.py
--rw-r--r--   0        0        0      674 2023-04-07 07:52:09.680377 dataquality-0.9.1a2/dataquality/utils/ampli.py
--rw-r--r--   0        0        0      401 2023-05-04 02:23:06.815569 dataquality-0.9.1a2/dataquality/utils/auth.py
--rw-r--r--   0        0        0     6824 2023-05-04 02:23:06.955706 dataquality-0.9.1a2/dataquality/utils/auto.py
--rw-r--r--   0        0        0      928 2023-05-04 21:34:44.817254 dataquality-0.9.1a2/dataquality/utils/auto_trainer.py
--rw-r--r--   0        0        0      154 2023-05-04 02:23:06.840003 dataquality-0.9.1a2/dataquality/utils/cloud.py
--rw-r--r--   0        0        0      885 2023-04-20 17:03:51.060491 dataquality-0.9.1a2/dataquality/utils/cuda.py
--rw-r--r--   0        0        0     2082 2023-05-04 02:23:06.900954 dataquality-0.9.1a2/dataquality/utils/cv.py
--rw-r--r--   0        0        0     3369 2023-05-04 02:23:06.908329 dataquality-0.9.1a2/dataquality/utils/dq_logger.py
--rw-r--r--   0        0        0     3514 2023-05-04 02:23:06.813427 dataquality-0.9.1a2/dataquality/utils/dqyolo.py
--rw-r--r--   0        0        0     4548 2023-05-04 02:23:06.896679 dataquality-0.9.1a2/dataquality/utils/emb.py
--rw-r--r--   0        0        0     3591 2023-05-04 02:23:06.888460 dataquality-0.9.1a2/dataquality/utils/file.py
--rw-r--r--   0        0        0     5685 2023-05-04 02:23:06.870438 dataquality-0.9.1a2/dataquality/utils/hdf5_store.py
--rw-r--r--   0        0        0     3362 2023-05-04 02:23:06.951619 dataquality-0.9.1a2/dataquality/utils/helpers.py
--rw-r--r--   0        0        0     2163 2023-05-04 02:23:06.828834 dataquality-0.9.1a2/dataquality/utils/hf_images.py
--rw-r--r--   0        0        0    10182 2023-05-04 02:23:06.821861 dataquality-0.9.1a2/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0        0        0      429 2023-04-07 07:52:09.684739 dataquality-0.9.1a2/dataquality/utils/imports.py
--rw-r--r--   0        0        0     8023 2023-05-04 02:23:06.846683 dataquality-0.9.1a2/dataquality/utils/keras.py
--rw-r--r--   0        0        0     2408 2023-05-04 02:23:06.884881 dataquality-0.9.1a2/dataquality/utils/ml.py
--rw-r--r--   0        0        0    24708 2023-04-07 07:52:09.685790 dataquality-0.9.1a2/dataquality/utils/name.py
--rw-r--r--   0        0        0     1184 2023-04-14 09:39:59.480342 dataquality-0.9.1a2/dataquality/utils/od.py
--rw-r--r--   0        0        0     5923 2023-05-04 02:23:06.929368 dataquality-0.9.1a2/dataquality/utils/profiler.py
--rw-r--r--   0        0        0        0 2023-05-03 22:49:30.085612 dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0        0        0     4148 2023-05-04 22:17:22.627633 dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0        0        0    14942 2023-05-04 22:17:22.627930 dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0        0        0     5479 2023-05-04 22:17:22.628295 dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0        0        0     5243 2023-05-04 22:17:22.628632 dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0        0        0     1914 2023-05-04 22:17:22.628890 dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0        0        0     4070 2023-05-04 02:23:06.861802 dataquality-0.9.1a2/dataquality/utils/spacy_integration.py
--rw-r--r--   0        0        0      260 2023-04-07 07:52:09.688175 dataquality-0.9.1a2/dataquality/utils/tf.py
--rw-r--r--   0        0        0     1987 2023-05-04 02:23:06.850275 dataquality-0.9.1a2/dataquality/utils/thread_pool.py
--rw-r--r--   0        0        0    18173 2023-05-04 02:23:06.939291 dataquality-0.9.1a2/dataquality/utils/torch.py
--rw-r--r--   0        0        0     2739 2023-05-04 02:23:06.842731 dataquality-0.9.1a2/dataquality/utils/transformers.py
--rw-r--r--   0        0        0    11924 2023-05-04 02:23:06.947607 dataquality-0.9.1a2/dataquality/utils/ultralytics.py
--rw-r--r--   0        0        0     5207 2023-05-04 02:23:06.837592 dataquality-0.9.1a2/dataquality/utils/upload.py
--rw-r--r--   0        0        0     8781 2023-05-04 02:23:06.878484 dataquality-0.9.1a2/dataquality/utils/vaex.py
--rw-r--r--   0        0        0     1087 2023-04-07 07:52:09.690283 dataquality-0.9.1a2/dataquality/utils/version.py
--rw-r--r--   0        0        0      634 2023-03-06 18:27:08.340955 dataquality-0.9.1a2/docs/autodocs/Makefile
--rw-r--r--   0        0        0      120 2023-03-06 18:27:08.341186 dataquality-0.9.1a2/docs/autodocs/Readme.md
--rw-r--r--   0        0        0   312552 2023-03-06 18:27:08.344287 dataquality-0.9.1a2/docs/autodocs/_build/doctrees/api/dataquality.doctree
--rw-r--r--   0        0        0    49162 2023-03-06 18:27:08.345328 dataquality-0.9.1a2/docs/autodocs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     2703 2023-03-06 18:27:08.345810 dataquality-0.9.1a2/docs/autodocs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0    33107 2023-04-10 07:35:51.793733 dataquality-0.9.1a2/docs/autodocs/_build/markdown/api/dataquality.md
--rw-r--r--   0        0        0     3191 2023-03-06 18:27:08.348392 dataquality-0.9.1a2/docs/autodocs/_build/markdown/index.md
--rw-r--r--   0        0        0     1485 2023-03-06 18:27:08.349296 dataquality-0.9.1a2/docs/autodocs/api/dataquality.rst
--rw-r--r--   0        0        0     2537 2023-03-06 18:27:08.349828 dataquality-0.9.1a2/docs/autodocs/conf.py
--rw-r--r--   0        0        0       86 2023-03-06 18:27:08.350033 dataquality-0.9.1a2/docs/autodocs/index.rst
--rw-r--r--   0        0        0      765 2023-03-06 18:27:08.350253 dataquality-0.9.1a2/docs/autodocs/make.bat
--rw-r--r--   0        0        0      165 2023-03-06 18:27:08.350468 dataquality-0.9.1a2/docs/autodocs/requirements.txt
--rw-r--r--   0        0        0      172 2023-02-16 18:20:37.512360 dataquality-0.9.1a2/docs/cv/README.md
--rw-r--r--   0        0        0   122204 2023-05-04 22:17:22.629812 dataquality-0.9.1a2/docs/cv/coco_deeplab_hooks.ipynb
--rw-r--r--   0        0        0     4245 2023-02-16 18:20:37.512548 dataquality-0.9.1a2/docs/cv/cv-demo-hf.py
--rw-r--r--   0        0        0     1893 2023-02-16 18:20:37.512698 dataquality-0.9.1a2/docs/cv/cv-testing-benchmark.py
--rw-r--r--   0        0        0    18832 2023-03-06 18:27:08.351257 dataquality-0.9.1a2/docs/notebooks/Dataquality-Client-Demo.ipynb
--rw-r--r--   0        0        0    10352 2023-03-06 18:27:08.352178 dataquality-0.9.1a2/docs/notebooks/End to End runs per task type.ipynb
--rw-r--r--   0        0        0    12031 2023-03-06 18:27:08.352622 dataquality-0.9.1a2/docs/notebooks/Inference-Demo.ipynb
--rw-r--r--   0        0        0     6893 2023-03-06 18:27:08.353238 dataquality-0.9.1a2/docs/notebooks/NER Inference.ipynb
--rw-r--r--   0        0        0     6378 2023-05-03 22:49:30.086339 dataquality-0.9.1a2/docs/notebooks/Tabular-Data.ipynb
--rw-r--r--   0        0        0      121 2023-05-04 21:27:09.407392 dataquality-0.9.1a2/mypy.ini
--rw-r--r--   0        0        0     2361 2023-05-04 21:27:05.391041 dataquality-0.9.1a2/pyproject.toml
--rw-r--r--   0        0        0       61 2023-02-16 18:20:37.515251 dataquality-0.9.1a2/pytest.ini
--rwxr-xr-x   0        0        0      247 2023-02-16 18:20:37.515473 dataquality-0.9.1a2/scripts/bump-version.sh
--rwxr-xr-x   0        0        0      100 2023-02-16 18:20:37.515600 dataquality-0.9.1a2/scripts/clean.sh
--rwxr-xr-x   0        0        0       53 2023-03-06 18:27:08.354433 dataquality-0.9.1a2/scripts/docs-build.sh
--rwxr-xr-x   0        0        0      311 2023-02-16 18:20:37.515862 dataquality-0.9.1a2/scripts/format.sh
--rwxr-xr-x   0        0        0      100 2023-04-14 09:39:59.483561 dataquality-0.9.1a2/scripts/install.sh
--rwxr-xr-x   0        0        0      126 2023-02-16 18:20:37.516123 dataquality-0.9.1a2/scripts/lint.sh
--rwxr-xr-x   0        0        0       29 2023-02-16 18:20:37.516245 dataquality-0.9.1a2/scripts/publish.sh
--rwxr-xr-x   0        0        0       66 2023-02-16 18:20:37.516369 dataquality-0.9.1a2/scripts/set-local-env.sh
--rwxr-xr-x   0        0        0       56 2023-02-16 18:20:37.516487 dataquality-0.9.1a2/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      216 2023-04-10 07:35:51.794690 dataquality-0.9.1a2/scripts/test.sh
--rw-r--r--   0        0        0        0 2023-02-16 18:20:37.516882 dataquality-0.9.1a2/tests/__init__.py
--rw-r--r--   0        0        0       16 2023-05-03 22:49:30.086944 dataquality-0.9.1a2/tests/assets/constants.py
--rw-r--r--   0        0        0     6688 2023-03-08 21:36:54.587556 dataquality-0.9.1a2/tests/assets/images/Abyssinian_83.jpg
--rw-r--r--   0        0        0     1977 2023-03-08 21:36:54.588075 dataquality-0.9.1a2/tests/assets/images/pug_198.jpg
--rw-r--r--   0        0        0     3477 2023-05-04 02:23:07.287309 dataquality-0.9.1a2/tests/auto/test_ner_auto.py
--rw-r--r--   0        0        0    16171 2023-05-04 02:23:07.284129 dataquality-0.9.1a2/tests/auto/test_tc_auto.py
--rw-r--r--   0        0        0    11188 2023-05-04 02:23:07.200376 dataquality-0.9.1a2/tests/clients/test_api.py
--rw-r--r--   0        0        0     6206 2023-05-04 02:23:07.176590 dataquality-0.9.1a2/tests/conftest.py
--rw-r--r--   0        0        0     1409 2023-05-04 02:23:07.251253 dataquality-0.9.1a2/tests/core/test_auth.py
--rw-r--r--   0        0        0      418 2023-02-16 18:20:37.518225 dataquality-0.9.1a2/tests/core/test_cloud.py
--rw-r--r--   0        0        0     6719 2023-05-04 02:23:07.263635 dataquality-0.9.1a2/tests/core/test_config.py
--rw-r--r--   0        0        0     6122 2023-05-04 02:23:07.259460 dataquality-0.9.1a2/tests/core/test_finish.py
--rw-r--r--   0        0        0    24970 2023-05-04 02:23:07.275502 dataquality-0.9.1a2/tests/core/test_init.py
--rw-r--r--   0        0        0     6907 2023-05-04 02:23:07.255690 dataquality-0.9.1a2/tests/core/test_report.py
--rw-r--r--   0        0        0       40 2023-02-16 18:20:37.519164 dataquality-0.9.1a2/tests/exceptions.py
--rw-r--r--   0        0        0     4991 2023-05-04 02:23:07.602654 dataquality-0.9.1a2/tests/inference/test_inference.py
--rw-r--r--   0        0        0     3342 2023-04-10 07:35:51.795608 dataquality-0.9.1a2/tests/inference/test_text_classification_inf.py
--rw-r--r--   0        0        0     3900 2023-04-10 07:35:51.795833 dataquality-0.9.1a2/tests/inference/test_text_ner_inf.py
--rw-r--r--   0        0        0     3862 2023-02-16 18:20:37.519849 dataquality-0.9.1a2/tests/integration/mock_training_run.py
--rw-r--r--   0        0        0     7624 2023-05-04 02:23:07.527584 dataquality-0.9.1a2/tests/integrations/fastai/test_cv_fai.py
--rw-r--r--   0        0        0    10933 2023-05-04 02:23:07.547862 dataquality-0.9.1a2/tests/integrations/hf/test_hf_integration.py
--rw-r--r--   0        0        0    13693 2023-05-04 22:09:08.118319 dataquality-0.9.1a2/tests/integrations/hf/test_text_classification_hf.py
--rw-r--r--   0        0        0     9269 2023-05-04 02:23:07.487410 dataquality-0.9.1a2/tests/integrations/keras/test_experimental.py
--rw-r--r--   0        0        0      514 2023-02-16 18:20:37.520738 dataquality-0.9.1a2/tests/integrations/keras/test_utils.py
--rw-r--r--   0        0        0     1346 2023-05-04 02:23:07.555929 dataquality-0.9.1a2/tests/integrations/spacy/conftest.py
--rw-r--r--   0        0        0      760 2023-04-07 02:45:30.770291 dataquality-0.9.1a2/tests/integrations/spacy/test_spacy_integration.py
--rw-r--r--   0        0        0    17759 2023-05-04 02:23:07.564774 dataquality-0.9.1a2/tests/integrations/spacy/test_spacy_ner.py
--rw-r--r--   0        0        0     5900 2023-05-04 02:23:07.499263 dataquality-0.9.1a2/tests/integrations/torch/test_dataloader_patching.py
--rw-r--r--   0        0        0     9298 2023-05-04 02:23:07.505356 dataquality-0.9.1a2/tests/integrations/torch/test_pt_text_classification.py
--rw-r--r--   0        0        0      904 2023-05-04 02:23:07.494930 dataquality-0.9.1a2/tests/integrations/torch/test_pt_utils.py
--rw-r--r--   0        0        0     1490 2023-04-28 02:34:07.411121 dataquality-0.9.1a2/tests/integrations/ultralytics/coco128.yaml
--rw-r--r--   0        0        0     4796 2023-05-04 02:23:07.595738 dataquality-0.9.1a2/tests/integrations/ultralytics/test_cv_yolo.py
--rw-r--r--   0        0        0     2023 2023-05-04 02:23:07.213395 dataquality-0.9.1a2/tests/loggers/conftest.py
--rw-r--r--   0        0        0    10010 2023-03-07 23:33:01.397781 dataquality-0.9.1a2/tests/loggers/test_image_classification.py
--rw-r--r--   0        0        0    11728 2023-05-04 02:23:07.208952 dataquality-0.9.1a2/tests/loggers/test_multi_label.py
--rw-r--r--   0        0        0    23505 2023-05-04 02:23:07.246089 dataquality-0.9.1a2/tests/loggers/test_ner.py
--rw-r--r--   0        0        0    28799 2023-05-04 02:23:07.228543 dataquality-0.9.1a2/tests/loggers/test_tabular_classification.py
--rw-r--r--   0        0        0    14066 2023-05-04 02:23:07.236161 dataquality-0.9.1a2/tests/loggers/test_text_classification.py
--rw-r--r--   0        0        0     7226 2023-05-04 02:23:07.447407 dataquality-0.9.1a2/tests/schemas/test_conditions.py
--rw-r--r--   0        0        0      402 2023-02-16 18:20:37.524191 dataquality-0.9.1a2/tests/schemas/test_metrics.py
--rw-r--r--   0        0        0     2892 2023-05-04 02:23:07.385253 dataquality-0.9.1a2/tests/start/test_start_auto.py
--rw-r--r--   0        0        0     4378 2023-05-04 02:23:07.380885 dataquality-0.9.1a2/tests/start/test_start_hf.py
--rw-r--r--   0        0        0     4400 2023-05-04 02:23:07.389501 dataquality-0.9.1a2/tests/start/test_start_keras.py
--rw-r--r--   0        0        0     8440 2023-05-04 02:23:07.398877 dataquality-0.9.1a2/tests/start/test_start_pt.py
--rw-r--r--   0        0        0     2995 2023-03-08 21:36:54.589817 dataquality-0.9.1a2/tests/start/test_start_spacy.md
--rw-r--r--   0        0        0    30343 2023-05-04 02:23:07.191886 dataquality-0.9.1a2/tests/test_dataquality.py
--rw-r--r--   0        0        0     1783 2023-02-16 18:20:37.524712 dataquality-0.9.1a2/tests/test_telemetrics.py
--rw-r--r--   0        0        0        0 2023-02-16 18:20:37.524869 dataquality-0.9.1a2/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     5910 2023-05-04 02:23:07.345615 dataquality-0.9.1a2/tests/test_utils/data_utils.py
--rw-r--r--   0        0        0     1692 2023-05-04 02:23:07.294017 dataquality-0.9.1a2/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0        0        0    11616 2023-04-14 09:39:59.489879 dataquality-0.9.1a2/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0        0        0     8122 2023-02-16 18:20:37.525814 dataquality-0.9.1a2/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0        0        0     3695 2023-02-16 18:20:37.526020 dataquality-0.9.1a2/tests/test_utils/lightning_model.py
--rw-r--r--   0        0        0     2057 2023-02-16 18:20:37.526167 dataquality-0.9.1a2/tests/test_utils/mock_data.py
--rw-r--r--   0        0        0     5594 2023-05-04 02:23:07.311166 dataquality-0.9.1a2/tests/test_utils/mock_request.py
--rw-r--r--   0        0        0     2840 2023-02-16 18:20:37.526602 dataquality-0.9.1a2/tests/test_utils/ner_constants.py
--rw-r--r--   0        0        0      863 2023-02-16 18:20:37.526747 dataquality-0.9.1a2/tests/test_utils/pt_datasets_mock.py
--rw-r--r--   0        0        0     4299 2023-05-04 02:23:07.315210 dataquality-0.9.1a2/tests/test_utils/spacy_integration.py
--rw-r--r--   0        0        0    22786 2023-04-14 09:39:59.490526 dataquality-0.9.1a2/tests/test_utils/spacy_integration_constants.py
--rw-r--r--   0        0        0    23021 2023-02-16 18:20:37.527473 dataquality-0.9.1a2/tests/test_utils/spacy_integration_constants_inference.py
--rw-r--r--   0        0        0     7910 2023-04-14 09:39:59.490924 dataquality-0.9.1a2/tests/test_utils/tc_constants.py
--rw-r--r--   0        0        0     4614 2023-05-04 02:23:07.417591 dataquality-0.9.1a2/tests/utils/test_auto.py
--rw-r--r--   0        0        0     1977 2023-04-10 07:35:51.802860 dataquality-0.9.1a2/tests/utils/test_dq_logger.py
--rw-r--r--   0        0        0     1522 2023-05-04 02:23:07.427111 dataquality-0.9.1a2/tests/utils/test_name.py
--rw-r--r--   0        0        0      288 2023-02-16 18:20:37.528250 dataquality-0.9.1a2/tests/utils/test_tf_version.py
--rw-r--r--   0        0        0     1003 2023-05-04 02:23:07.408449 dataquality-0.9.1a2/tests/utils/test_vaex_utils.py
--rw-r--r--   0        0        0     1098 2023-05-04 02:23:07.404632 dataquality-0.9.1a2/tests/utils/test_version.py
--rw-r--r--   0        0        0     8002 1970-01-01 00:00:00.000000 dataquality-0.9.1a2/PKG-INFO
+-rw-r--r--   0        0        0       99 2023-02-16 18:20:37.484786 dataquality-0.9.1a3/.coveragerc
+-rw-r--r--   0        0        0      131 2023-02-16 18:20:37.484963 dataquality-0.9.1a3/.editorconfig
+-rw-r--r--   0        0        0      179 2023-03-06 18:27:08.322809 dataquality-0.9.1a3/.flake8
+-rw-r--r--   0        0        0       19 2023-04-28 02:34:07.405536 dataquality-0.9.1a3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      924 2023-02-16 18:20:37.485592 dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      590 2023-02-16 18:20:37.485749 dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/doc.md
+-rw-r--r--   0        0        0      700 2023-02-16 18:20:37.485896 dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0        0        0      542 2023-02-16 18:20:37.486033 dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1169 2023-02-16 18:20:37.486183 dataquality-0.9.1a3/.github/pull_request_template.md
+-rw-r--r--   0        0        0      950 2023-04-14 09:39:59.465229 dataquality-0.9.1a3/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      525 2023-04-14 09:39:59.466024 dataquality-0.9.1a3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      890 2023-04-14 09:39:59.467112 dataquality-0.9.1a3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     2418 2023-05-03 22:49:30.076353 dataquality-0.9.1a3/.gitignore
+-rw-r--r--   0        0        0        6 2023-02-16 18:20:37.487014 dataquality-0.9.1a3/.python-version
+-rw-r--r--   0        0        0     8078 2023-02-16 18:20:37.487229 dataquality-0.9.1a3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1066 2023-02-16 18:20:37.487400 dataquality-0.9.1a3/LICENSE
+-rw-r--r--   0        0        0     4437 2023-02-16 18:20:37.487564 dataquality-0.9.1a3/README.md
+-rw-r--r--   0        0        0     6012 2023-05-04 22:28:26.956565 dataquality-0.9.1a3/dataquality/__init__.py
+-rw-r--r--   0        0        0     8461 2023-05-04 02:23:06.506407 dataquality-0.9.1a3/dataquality/analytics.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.639242 dataquality-0.9.1a3/dataquality/clients/__init__.py
+-rw-r--r--   0        0        0    33867 2023-05-04 02:23:06.529362 dataquality-0.9.1a3/dataquality/clients/api.py
+-rw-r--r--   0        0        0     8187 2023-05-04 02:23:06.516492 dataquality-0.9.1a3/dataquality/clients/objectstore.py
+-rw-r--r--   0        0        0     1848 2023-04-07 07:52:09.644595 dataquality-0.9.1a3/dataquality/core/__init__.py
+-rw-r--r--   0        0        0     8843 2023-05-04 02:23:06.793133 dataquality-0.9.1a3/dataquality/core/_config.py
+-rw-r--r--   0        0        0     3104 2023-05-04 02:23:06.759652 dataquality-0.9.1a3/dataquality/core/auth.py
+-rw-r--r--   0        0        0     6499 2023-05-04 22:17:22.621387 dataquality-0.9.1a3/dataquality/core/finish.py
+-rw-r--r--   0        0        0     7026 2023-05-04 02:23:06.783167 dataquality-0.9.1a3/dataquality/core/init.py
+-rw-r--r--   0        0        0    21161 2023-05-04 02:23:06.771183 dataquality-0.9.1a3/dataquality/core/log.py
+-rw-r--r--   0        0        0     7039 2023-05-04 02:23:06.799371 dataquality-0.9.1a3/dataquality/core/report.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.650876 dataquality-0.9.1a3/dataquality/dq_auto/__init__.py
+-rw-r--r--   0        0        0    10475 2023-05-04 22:29:00.072086 dataquality-0.9.1a3/dataquality/dq_auto/auto.py
+-rw-r--r--   0        0        0     4158 2023-05-04 02:23:07.126817 dataquality-0.9.1a3/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0        0        0     7710 2023-05-04 22:10:32.335211 dataquality-0.9.1a3/dataquality/dq_auto/ner.py
+-rw-r--r--   0        0        0     4265 2023-05-04 02:23:07.123093 dataquality-0.9.1a3/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0        0        0     1594 2023-05-04 02:23:07.142858 dataquality-0.9.1a3/dataquality/dq_auto/notebook.py
+-rw-r--r--   0        0        0     3559 2023-05-04 02:23:07.146263 dataquality-0.9.1a3/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0        0        0    11797 2023-05-04 22:10:43.269244 dataquality-0.9.1a3/dataquality/dq_auto/text_classification.py
+-rw-r--r--   0        0        0    13139 2023-05-04 02:23:06.545657 dataquality-0.9.1a3/dataquality/dq_start/__init__.py
+-rw-r--r--   0        0        0     4498 2023-05-04 02:23:06.465858 dataquality-0.9.1a3/dataquality/dqyolo.py
+-rw-r--r--   0        0        0      293 2023-04-07 07:52:09.656391 dataquality-0.9.1a3/dataquality/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.656535 dataquality-0.9.1a3/dataquality/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:49:30.079624 dataquality-0.9.1a3/dataquality/integrations/cv/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:49:30.079930 dataquality-0.9.1a3/dataquality/integrations/cv/torch/__init__.py
+-rw-r--r--   0        0        0    20077 2023-05-04 22:17:22.622375 dataquality-0.9.1a3/dataquality/integrations/cv/torch/semantic_segmentation.py
+-rw-r--r--   0        0        0    15575 2023-05-04 02:23:07.110977 dataquality-0.9.1a3/dataquality/integrations/experimental/keras.py
+-rw-r--r--   0        0        0    14914 2023-05-04 02:23:07.045645 dataquality-0.9.1a3/dataquality/integrations/fastai.py
+-rw-r--r--   0        0        0    10024 2023-05-04 02:23:07.102392 dataquality-0.9.1a3/dataquality/integrations/hf.py
+-rw-r--r--   0        0        0     4375 2023-05-04 02:23:07.050094 dataquality-0.9.1a3/dataquality/integrations/keras.py
+-rw-r--r--   0        0        0    26831 2023-05-04 02:23:07.079437 dataquality-0.9.1a3/dataquality/integrations/spacy.py
+-rw-r--r--   0        0        0    12787 2023-05-04 02:23:07.084631 dataquality-0.9.1a3/dataquality/integrations/torch.py
+-rw-r--r--   0        0        0    12375 2023-05-04 22:06:55.080834 dataquality-0.9.1a3/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0        0        0    16907 2023-05-04 02:23:07.095450 dataquality-0.9.1a3/dataquality/integrations/ultralytics.py
+-rw-r--r--   0        0        0       95 2023-04-07 07:52:09.664245 dataquality-0.9.1a3/dataquality/loggers/__init__.py
+-rw-r--r--   0        0        0    13292 2023-05-04 02:23:06.570857 dataquality-0.9.1a3/dataquality/loggers/base_logger.py
+-rw-r--r--   0        0        0      517 2023-05-04 02:23:06.665914 dataquality-0.9.1a3/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0        0        0    26263 2023-05-04 22:17:22.623202 dataquality-0.9.1a3/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0        0        0    10393 2023-05-04 02:23:06.662586 dataquality-0.9.1a3/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0        0        0     9368 2023-05-04 02:23:06.719013 dataquality-0.9.1a3/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0        0        0     2768 2023-05-04 22:17:22.623829 dataquality-0.9.1a3/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0     9864 2023-05-04 02:23:06.651100 dataquality-0.9.1a3/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0        0        0    20661 2023-05-04 02:23:06.678041 dataquality-0.9.1a3/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0        0        0    14941 2023-05-04 02:23:06.687072 dataquality-0.9.1a3/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0        0        0    31885 2023-05-04 02:23:06.699619 dataquality-0.9.1a3/dataquality/loggers/data_logger/text_ner.py
+-rw-r--r--   0        0        0        0 2023-04-07 07:52:09.669046 dataquality-0.9.1a3/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0        0        0     1910 2023-05-04 22:17:22.624592 dataquality-0.9.1a3/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0        0        0      473 2023-04-07 07:52:09.669969 dataquality-0.9.1a3/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0        0        0      537 2023-04-14 09:39:59.476862 dataquality-0.9.1a3/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0        0        0      226 2023-05-03 22:49:30.083124 dataquality-0.9.1a3/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0        0        0      398 2023-05-03 22:49:30.083397 dataquality-0.9.1a3/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0        0        0      958 2023-05-04 02:23:06.738772 dataquality-0.9.1a3/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0        0        0     1510 2023-05-04 02:23:06.741859 dataquality-0.9.1a3/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0        0        0     1608 2023-05-04 02:23:06.745185 dataquality-0.9.1a3/dataquality/loggers/logger_config/text_ner.py
+-rw-r--r--   0        0        0      420 2023-05-04 02:23:06.588494 dataquality-0.9.1a3/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0        0        0     7510 2023-05-04 02:23:06.637489 dataquality-0.9.1a3/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0        0        0     3309 2023-05-04 02:23:06.583977 dataquality-0.9.1a3/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0        0        0     8975 2023-05-04 02:23:06.627055 dataquality-0.9.1a3/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0        0        0     6463 2023-05-04 22:17:22.624998 dataquality-0.9.1a3/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0        0        0      519 2023-05-03 22:49:30.084436 dataquality-0.9.1a3/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0        0        0     7555 2023-05-04 02:23:06.598643 dataquality-0.9.1a3/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0        0        0     9120 2023-05-04 02:23:06.605413 dataquality-0.9.1a3/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0        0        0    32052 2023-05-04 02:23:06.616819 dataquality-0.9.1a3/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0        0        0    28673 2023-05-04 02:23:06.482946 dataquality-0.9.1a3/dataquality/metrics.py
+-rw-r--r--   0        0        0      165 2023-04-07 07:52:09.676633 dataquality-0.9.1a3/dataquality/schemas/__init__.py
+-rw-r--r--   0        0        0     8361 2023-05-04 02:23:07.012740 dataquality-0.9.1a3/dataquality/schemas/condition.py
+-rw-r--r--   0        0        0      569 2023-05-04 02:23:06.968028 dataquality-0.9.1a3/dataquality/schemas/dataframe.py
+-rw-r--r--   0        0        0     4382 2023-05-04 02:23:07.004539 dataquality-0.9.1a3/dataquality/schemas/edit.py
+-rw-r--r--   0        0        0      662 2023-04-07 07:52:09.677611 dataquality-0.9.1a3/dataquality/schemas/hf.py
+-rw-r--r--   0        0        0      118 2023-05-04 02:23:06.970328 dataquality-0.9.1a3/dataquality/schemas/job.py
+-rw-r--r--   0        0        0     5241 2023-05-04 02:23:06.964247 dataquality-0.9.1a3/dataquality/schemas/metrics.py
+-rw-r--r--   0        0        0      165 2023-05-04 02:23:07.006560 dataquality-0.9.1a3/dataquality/schemas/model.py
+-rw-r--r--   0        0        0      992 2023-05-04 02:23:07.015866 dataquality-0.9.1a3/dataquality/schemas/ner.py
+-rw-r--r--   0        0        0      617 2023-05-04 02:23:07.027724 dataquality-0.9.1a3/dataquality/schemas/report.py
+-rw-r--r--   0        0        0      287 2023-04-07 07:52:09.678943 dataquality-0.9.1a3/dataquality/schemas/request_type.py
+-rw-r--r--   0        0        0     1491 2023-05-04 02:23:06.973737 dataquality-0.9.1a3/dataquality/schemas/route.py
+-rw-r--r--   0        0        0     2550 2023-05-04 22:17:22.626499 dataquality-0.9.1a3/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0        0        0      992 2023-05-04 02:23:07.018585 dataquality-0.9.1a3/dataquality/schemas/split.py
+-rw-r--r--   0        0        0     1055 2023-05-04 02:23:07.021496 dataquality-0.9.1a3/dataquality/schemas/task_type.py
+-rw-r--r--   0        0        0      740 2023-05-04 22:17:22.627338 dataquality-0.9.1a3/dataquality/schemas/torch.py
+-rw-r--r--   0        0        0      222 2023-04-07 07:52:09.680124 dataquality-0.9.1a3/dataquality/utils/__init__.py
+-rw-r--r--   0        0        0      674 2023-04-07 07:52:09.680377 dataquality-0.9.1a3/dataquality/utils/ampli.py
+-rw-r--r--   0        0        0      401 2023-05-04 02:23:06.815569 dataquality-0.9.1a3/dataquality/utils/auth.py
+-rw-r--r--   0        0        0     6824 2023-05-04 02:23:06.955706 dataquality-0.9.1a3/dataquality/utils/auto.py
+-rw-r--r--   0        0        0      928 2023-05-04 21:34:44.817254 dataquality-0.9.1a3/dataquality/utils/auto_trainer.py
+-rw-r--r--   0        0        0      154 2023-05-04 02:23:06.840003 dataquality-0.9.1a3/dataquality/utils/cloud.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:03:51.060491 dataquality-0.9.1a3/dataquality/utils/cuda.py
+-rw-r--r--   0        0        0     2082 2023-05-04 02:23:06.900954 dataquality-0.9.1a3/dataquality/utils/cv.py
+-rw-r--r--   0        0        0     3369 2023-05-04 02:23:06.908329 dataquality-0.9.1a3/dataquality/utils/dq_logger.py
+-rw-r--r--   0        0        0     3514 2023-05-04 02:23:06.813427 dataquality-0.9.1a3/dataquality/utils/dqyolo.py
+-rw-r--r--   0        0        0     4548 2023-05-04 02:23:06.896679 dataquality-0.9.1a3/dataquality/utils/emb.py
+-rw-r--r--   0        0        0     3591 2023-05-04 02:23:06.888460 dataquality-0.9.1a3/dataquality/utils/file.py
+-rw-r--r--   0        0        0     5685 2023-05-04 02:23:06.870438 dataquality-0.9.1a3/dataquality/utils/hdf5_store.py
+-rw-r--r--   0        0        0     3362 2023-05-04 02:23:06.951619 dataquality-0.9.1a3/dataquality/utils/helpers.py
+-rw-r--r--   0        0        0     2163 2023-05-04 02:23:06.828834 dataquality-0.9.1a3/dataquality/utils/hf_images.py
+-rw-r--r--   0        0        0    10182 2023-05-04 02:23:06.821861 dataquality-0.9.1a3/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0        0        0      429 2023-04-07 07:52:09.684739 dataquality-0.9.1a3/dataquality/utils/imports.py
+-rw-r--r--   0        0        0     8023 2023-05-04 02:23:06.846683 dataquality-0.9.1a3/dataquality/utils/keras.py
+-rw-r--r--   0        0        0     2408 2023-05-04 02:23:06.884881 dataquality-0.9.1a3/dataquality/utils/ml.py
+-rw-r--r--   0        0        0    24708 2023-04-07 07:52:09.685790 dataquality-0.9.1a3/dataquality/utils/name.py
+-rw-r--r--   0        0        0     1184 2023-04-14 09:39:59.480342 dataquality-0.9.1a3/dataquality/utils/od.py
+-rw-r--r--   0        0        0     5923 2023-05-04 02:23:06.929368 dataquality-0.9.1a3/dataquality/utils/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:49:30.085612 dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0        0        0     4148 2023-05-04 22:17:22.627633 dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0        0        0    14942 2023-05-04 22:17:22.627930 dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0        0        0     5479 2023-05-04 22:17:22.628295 dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0        0        0     5243 2023-05-04 22:17:22.628632 dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0        0        0     1914 2023-05-04 22:17:22.628890 dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0        0        0     4070 2023-05-04 02:23:06.861802 dataquality-0.9.1a3/dataquality/utils/spacy_integration.py
+-rw-r--r--   0        0        0      260 2023-04-07 07:52:09.688175 dataquality-0.9.1a3/dataquality/utils/tf.py
+-rw-r--r--   0        0        0     1987 2023-05-04 02:23:06.850275 dataquality-0.9.1a3/dataquality/utils/thread_pool.py
+-rw-r--r--   0        0        0    18173 2023-05-04 02:23:06.939291 dataquality-0.9.1a3/dataquality/utils/torch.py
+-rw-r--r--   0        0        0     2739 2023-05-04 02:23:06.842731 dataquality-0.9.1a3/dataquality/utils/transformers.py
+-rw-r--r--   0        0        0    11924 2023-05-04 02:23:06.947607 dataquality-0.9.1a3/dataquality/utils/ultralytics.py
+-rw-r--r--   0        0        0     5207 2023-05-04 02:23:06.837592 dataquality-0.9.1a3/dataquality/utils/upload.py
+-rw-r--r--   0        0        0     8781 2023-05-04 02:23:06.878484 dataquality-0.9.1a3/dataquality/utils/vaex.py
+-rw-r--r--   0        0        0     1087 2023-04-07 07:52:09.690283 dataquality-0.9.1a3/dataquality/utils/version.py
+-rw-r--r--   0        0        0      634 2023-03-06 18:27:08.340955 dataquality-0.9.1a3/docs/autodocs/Makefile
+-rw-r--r--   0        0        0      120 2023-03-06 18:27:08.341186 dataquality-0.9.1a3/docs/autodocs/Readme.md
+-rw-r--r--   0        0        0   312552 2023-03-06 18:27:08.344287 dataquality-0.9.1a3/docs/autodocs/_build/doctrees/api/dataquality.doctree
+-rw-r--r--   0        0        0    49162 2023-03-06 18:27:08.345328 dataquality-0.9.1a3/docs/autodocs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     2703 2023-03-06 18:27:08.345810 dataquality-0.9.1a3/docs/autodocs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0    33107 2023-04-10 07:35:51.793733 dataquality-0.9.1a3/docs/autodocs/_build/markdown/api/dataquality.md
+-rw-r--r--   0        0        0     3191 2023-03-06 18:27:08.348392 dataquality-0.9.1a3/docs/autodocs/_build/markdown/index.md
+-rw-r--r--   0        0        0     1485 2023-03-06 18:27:08.349296 dataquality-0.9.1a3/docs/autodocs/api/dataquality.rst
+-rw-r--r--   0        0        0     2537 2023-03-06 18:27:08.349828 dataquality-0.9.1a3/docs/autodocs/conf.py
+-rw-r--r--   0        0        0       86 2023-03-06 18:27:08.350033 dataquality-0.9.1a3/docs/autodocs/index.rst
+-rw-r--r--   0        0        0      765 2023-03-06 18:27:08.350253 dataquality-0.9.1a3/docs/autodocs/make.bat
+-rw-r--r--   0        0        0      165 2023-03-06 18:27:08.350468 dataquality-0.9.1a3/docs/autodocs/requirements.txt
+-rw-r--r--   0        0        0      172 2023-02-16 18:20:37.512360 dataquality-0.9.1a3/docs/cv/README.md
+-rw-r--r--   0        0        0   122204 2023-05-04 22:17:22.629812 dataquality-0.9.1a3/docs/cv/coco_deeplab_hooks.ipynb
+-rw-r--r--   0        0        0     4245 2023-02-16 18:20:37.512548 dataquality-0.9.1a3/docs/cv/cv-demo-hf.py
+-rw-r--r--   0        0        0     1893 2023-02-16 18:20:37.512698 dataquality-0.9.1a3/docs/cv/cv-testing-benchmark.py
+-rw-r--r--   0        0        0    18832 2023-03-06 18:27:08.351257 dataquality-0.9.1a3/docs/notebooks/Dataquality-Client-Demo.ipynb
+-rw-r--r--   0        0        0    10352 2023-03-06 18:27:08.352178 dataquality-0.9.1a3/docs/notebooks/End to End runs per task type.ipynb
+-rw-r--r--   0        0        0    12031 2023-03-06 18:27:08.352622 dataquality-0.9.1a3/docs/notebooks/Inference-Demo.ipynb
+-rw-r--r--   0        0        0     6893 2023-03-06 18:27:08.353238 dataquality-0.9.1a3/docs/notebooks/NER Inference.ipynb
+-rw-r--r--   0        0        0     6378 2023-05-03 22:49:30.086339 dataquality-0.9.1a3/docs/notebooks/Tabular-Data.ipynb
+-rw-r--r--   0        0        0      121 2023-05-04 21:27:09.407392 dataquality-0.9.1a3/mypy.ini
+-rw-r--r--   0        0        0     2361 2023-05-04 21:27:05.391041 dataquality-0.9.1a3/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-02-16 18:20:37.515251 dataquality-0.9.1a3/pytest.ini
+-rwxr-xr-x   0        0        0      247 2023-02-16 18:20:37.515473 dataquality-0.9.1a3/scripts/bump-version.sh
+-rwxr-xr-x   0        0        0      100 2023-02-16 18:20:37.515600 dataquality-0.9.1a3/scripts/clean.sh
+-rwxr-xr-x   0        0        0       53 2023-03-06 18:27:08.354433 dataquality-0.9.1a3/scripts/docs-build.sh
+-rwxr-xr-x   0        0        0      311 2023-02-16 18:20:37.515862 dataquality-0.9.1a3/scripts/format.sh
+-rwxr-xr-x   0        0        0      100 2023-04-14 09:39:59.483561 dataquality-0.9.1a3/scripts/install.sh
+-rwxr-xr-x   0        0        0      126 2023-02-16 18:20:37.516123 dataquality-0.9.1a3/scripts/lint.sh
+-rwxr-xr-x   0        0        0       29 2023-02-16 18:20:37.516245 dataquality-0.9.1a3/scripts/publish.sh
+-rwxr-xr-x   0        0        0       66 2023-02-16 18:20:37.516369 dataquality-0.9.1a3/scripts/set-local-env.sh
+-rwxr-xr-x   0        0        0       56 2023-02-16 18:20:37.516487 dataquality-0.9.1a3/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      216 2023-04-10 07:35:51.794690 dataquality-0.9.1a3/scripts/test.sh
+-rw-r--r--   0        0        0        0 2023-02-16 18:20:37.516882 dataquality-0.9.1a3/tests/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-03 22:49:30.086944 dataquality-0.9.1a3/tests/assets/constants.py
+-rw-r--r--   0        0        0     6688 2023-03-08 21:36:54.587556 dataquality-0.9.1a3/tests/assets/images/Abyssinian_83.jpg
+-rw-r--r--   0        0        0     1977 2023-03-08 21:36:54.588075 dataquality-0.9.1a3/tests/assets/images/pug_198.jpg
+-rw-r--r--   0        0        0     3477 2023-05-04 02:23:07.287309 dataquality-0.9.1a3/tests/auto/test_ner_auto.py
+-rw-r--r--   0        0        0    16171 2023-05-04 02:23:07.284129 dataquality-0.9.1a3/tests/auto/test_tc_auto.py
+-rw-r--r--   0        0        0    11188 2023-05-04 02:23:07.200376 dataquality-0.9.1a3/tests/clients/test_api.py
+-rw-r--r--   0        0        0     6206 2023-05-04 02:23:07.176590 dataquality-0.9.1a3/tests/conftest.py
+-rw-r--r--   0        0        0     1409 2023-05-04 02:23:07.251253 dataquality-0.9.1a3/tests/core/test_auth.py
+-rw-r--r--   0        0        0      418 2023-02-16 18:20:37.518225 dataquality-0.9.1a3/tests/core/test_cloud.py
+-rw-r--r--   0        0        0     6719 2023-05-04 02:23:07.263635 dataquality-0.9.1a3/tests/core/test_config.py
+-rw-r--r--   0        0        0     6122 2023-05-04 02:23:07.259460 dataquality-0.9.1a3/tests/core/test_finish.py
+-rw-r--r--   0        0        0    24970 2023-05-04 02:23:07.275502 dataquality-0.9.1a3/tests/core/test_init.py
+-rw-r--r--   0        0        0     6907 2023-05-04 02:23:07.255690 dataquality-0.9.1a3/tests/core/test_report.py
+-rw-r--r--   0        0        0       40 2023-02-16 18:20:37.519164 dataquality-0.9.1a3/tests/exceptions.py
+-rw-r--r--   0        0        0     4991 2023-05-04 02:23:07.602654 dataquality-0.9.1a3/tests/inference/test_inference.py
+-rw-r--r--   0        0        0     3342 2023-04-10 07:35:51.795608 dataquality-0.9.1a3/tests/inference/test_text_classification_inf.py
+-rw-r--r--   0        0        0     3900 2023-04-10 07:35:51.795833 dataquality-0.9.1a3/tests/inference/test_text_ner_inf.py
+-rw-r--r--   0        0        0     3862 2023-02-16 18:20:37.519849 dataquality-0.9.1a3/tests/integration/mock_training_run.py
+-rw-r--r--   0        0        0     7624 2023-05-04 02:23:07.527584 dataquality-0.9.1a3/tests/integrations/fastai/test_cv_fai.py
+-rw-r--r--   0        0        0    10933 2023-05-04 02:23:07.547862 dataquality-0.9.1a3/tests/integrations/hf/test_hf_integration.py
+-rw-r--r--   0        0        0    13693 2023-05-04 22:09:08.118319 dataquality-0.9.1a3/tests/integrations/hf/test_text_classification_hf.py
+-rw-r--r--   0        0        0     9269 2023-05-04 02:23:07.487410 dataquality-0.9.1a3/tests/integrations/keras/test_experimental.py
+-rw-r--r--   0        0        0      514 2023-02-16 18:20:37.520738 dataquality-0.9.1a3/tests/integrations/keras/test_utils.py
+-rw-r--r--   0        0        0     1346 2023-05-04 02:23:07.555929 dataquality-0.9.1a3/tests/integrations/spacy/conftest.py
+-rw-r--r--   0        0        0      760 2023-04-07 02:45:30.770291 dataquality-0.9.1a3/tests/integrations/spacy/test_spacy_integration.py
+-rw-r--r--   0        0        0    17759 2023-05-04 02:23:07.564774 dataquality-0.9.1a3/tests/integrations/spacy/test_spacy_ner.py
+-rw-r--r--   0        0        0     5900 2023-05-04 02:23:07.499263 dataquality-0.9.1a3/tests/integrations/torch/test_dataloader_patching.py
+-rw-r--r--   0        0        0     9298 2023-05-04 02:23:07.505356 dataquality-0.9.1a3/tests/integrations/torch/test_pt_text_classification.py
+-rw-r--r--   0        0        0      904 2023-05-04 02:23:07.494930 dataquality-0.9.1a3/tests/integrations/torch/test_pt_utils.py
+-rw-r--r--   0        0        0     1490 2023-04-28 02:34:07.411121 dataquality-0.9.1a3/tests/integrations/ultralytics/coco128.yaml
+-rw-r--r--   0        0        0     4796 2023-05-04 02:23:07.595738 dataquality-0.9.1a3/tests/integrations/ultralytics/test_cv_yolo.py
+-rw-r--r--   0        0        0     2023 2023-05-04 02:23:07.213395 dataquality-0.9.1a3/tests/loggers/conftest.py
+-rw-r--r--   0        0        0    10010 2023-03-07 23:33:01.397781 dataquality-0.9.1a3/tests/loggers/test_image_classification.py
+-rw-r--r--   0        0        0    11728 2023-05-04 02:23:07.208952 dataquality-0.9.1a3/tests/loggers/test_multi_label.py
+-rw-r--r--   0        0        0    23505 2023-05-04 02:23:07.246089 dataquality-0.9.1a3/tests/loggers/test_ner.py
+-rw-r--r--   0        0        0    28799 2023-05-04 02:23:07.228543 dataquality-0.9.1a3/tests/loggers/test_tabular_classification.py
+-rw-r--r--   0        0        0    14066 2023-05-04 02:23:07.236161 dataquality-0.9.1a3/tests/loggers/test_text_classification.py
+-rw-r--r--   0        0        0     7226 2023-05-04 02:23:07.447407 dataquality-0.9.1a3/tests/schemas/test_conditions.py
+-rw-r--r--   0        0        0      402 2023-02-16 18:20:37.524191 dataquality-0.9.1a3/tests/schemas/test_metrics.py
+-rw-r--r--   0        0        0     2892 2023-05-04 02:23:07.385253 dataquality-0.9.1a3/tests/start/test_start_auto.py
+-rw-r--r--   0        0        0     4378 2023-05-04 02:23:07.380885 dataquality-0.9.1a3/tests/start/test_start_hf.py
+-rw-r--r--   0        0        0     4400 2023-05-04 02:23:07.389501 dataquality-0.9.1a3/tests/start/test_start_keras.py
+-rw-r--r--   0        0        0     8440 2023-05-04 02:23:07.398877 dataquality-0.9.1a3/tests/start/test_start_pt.py
+-rw-r--r--   0        0        0     2995 2023-03-08 21:36:54.589817 dataquality-0.9.1a3/tests/start/test_start_spacy.md
+-rw-r--r--   0        0        0    30343 2023-05-04 02:23:07.191886 dataquality-0.9.1a3/tests/test_dataquality.py
+-rw-r--r--   0        0        0     1783 2023-02-16 18:20:37.524712 dataquality-0.9.1a3/tests/test_telemetrics.py
+-rw-r--r--   0        0        0        0 2023-02-16 18:20:37.524869 dataquality-0.9.1a3/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     5910 2023-05-04 02:23:07.345615 dataquality-0.9.1a3/tests/test_utils/data_utils.py
+-rw-r--r--   0        0        0     1692 2023-05-04 02:23:07.294017 dataquality-0.9.1a3/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0        0        0    11616 2023-04-14 09:39:59.489879 dataquality-0.9.1a3/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0        0        0     8122 2023-02-16 18:20:37.525814 dataquality-0.9.1a3/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0        0        0     3695 2023-02-16 18:20:37.526020 dataquality-0.9.1a3/tests/test_utils/lightning_model.py
+-rw-r--r--   0        0        0     2057 2023-02-16 18:20:37.526167 dataquality-0.9.1a3/tests/test_utils/mock_data.py
+-rw-r--r--   0        0        0     5594 2023-05-04 02:23:07.311166 dataquality-0.9.1a3/tests/test_utils/mock_request.py
+-rw-r--r--   0        0        0     2840 2023-02-16 18:20:37.526602 dataquality-0.9.1a3/tests/test_utils/ner_constants.py
+-rw-r--r--   0        0        0      863 2023-02-16 18:20:37.526747 dataquality-0.9.1a3/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0        0        0     4299 2023-05-04 02:23:07.315210 dataquality-0.9.1a3/tests/test_utils/spacy_integration.py
+-rw-r--r--   0        0        0    22786 2023-04-14 09:39:59.490526 dataquality-0.9.1a3/tests/test_utils/spacy_integration_constants.py
+-rw-r--r--   0        0        0    23021 2023-02-16 18:20:37.527473 dataquality-0.9.1a3/tests/test_utils/spacy_integration_constants_inference.py
+-rw-r--r--   0        0        0     7910 2023-04-14 09:39:59.490924 dataquality-0.9.1a3/tests/test_utils/tc_constants.py
+-rw-r--r--   0        0        0     4614 2023-05-04 02:23:07.417591 dataquality-0.9.1a3/tests/utils/test_auto.py
+-rw-r--r--   0        0        0     1977 2023-04-10 07:35:51.802860 dataquality-0.9.1a3/tests/utils/test_dq_logger.py
+-rw-r--r--   0        0        0     1522 2023-05-04 02:23:07.427111 dataquality-0.9.1a3/tests/utils/test_name.py
+-rw-r--r--   0        0        0      288 2023-02-16 18:20:37.528250 dataquality-0.9.1a3/tests/utils/test_tf_version.py
+-rw-r--r--   0        0        0     1003 2023-05-04 02:23:07.408449 dataquality-0.9.1a3/tests/utils/test_vaex_utils.py
+-rw-r--r--   0        0        0     1098 2023-05-04 02:23:07.404632 dataquality-0.9.1a3/tests/utils/test_version.py
+-rw-r--r--   0        0        0     8002 1970-01-01 00:00:00.000000 dataquality-0.9.1a3/PKG-INFO
```

### Comparing `dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/bug.md` & `dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/doc.md` & `dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/doc.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/feature.md` & `dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.github/ISSUE_TEMPLATE/question.md` & `dataquality-0.9.1a3/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.github/pull_request_template.md` & `dataquality-0.9.1a3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.github/workflows/docs.yaml` & `dataquality-0.9.1a3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.github/workflows/publish.yaml` & `dataquality-0.9.1a3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.github/workflows/test.yaml` & `dataquality-0.9.1a3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/.gitignore` & `dataquality-0.9.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/CONTRIBUTING.md` & `dataquality-0.9.1a3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/LICENSE` & `dataquality-0.9.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/README.md` & `dataquality-0.9.1a3/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/__init__.py` & `dataquality-0.9.1a3/dataquality/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .. code-block:: python
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
-__version__ = "v0.9.1a2"
+__version__ = "v0.9.1a3"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.core._config
 import dataquality.integrations
```

### Comparing `dataquality-0.9.1a2/dataquality/analytics.py` & `dataquality-0.9.1a3/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/clients/api.py` & `dataquality-0.9.1a3/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/clients/objectstore.py` & `dataquality-0.9.1a3/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/core/__init__.py` & `dataquality-0.9.1a3/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/core/_config.py` & `dataquality-0.9.1a3/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/core/auth.py` & `dataquality-0.9.1a3/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/core/finish.py` & `dataquality-0.9.1a3/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/core/init.py` & `dataquality-0.9.1a3/dataquality/core/init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/core/log.py` & `dataquality-0.9.1a3/dataquality/core/log.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/core/report.py` & `dataquality-0.9.1a3/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dq_auto/auto.py` & `dataquality-0.9.1a3/dataquality/dq_auto/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,17 @@
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
             create_data_embs=create_data_embs,
             num_train_epochs=num_train_epochs,
-            call_finish=call_finish)
+            call_finish=call_finish,
         )
+
     elif task_type == TaskType.text_ner:
         from dataquality.dq_auto.ner import auto as auto_ner
 
         return auto_ner(
             hf_data=hf_data,
             hf_inference_names=hf_inference_names,
             train_data=train_data,
@@ -239,11 +240,12 @@
             inference_data=inference_data,
             hf_model=hf_model,
             labels=labels,
             project_name=project_name or AUTO_PROJECT_NAME[task_type],
             run_name=run_name,
             wait=wait,
             num_train_epochs=num_train_epochs,
-            call_finish=call_finish)
+            call_finish=call_finish,
         )
+
     else:
         raise Exception("auto is only supported for text classification and NER!")
```

### Comparing `dataquality-0.9.1a2/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.1a3/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dq_auto/ner.py` & `dataquality-0.9.1a3/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.1a3/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dq_auto/notebook.py` & `dataquality-0.9.1a3/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.1a3/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.1a3/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dq_start/__init__.py` & `dataquality-0.9.1a3/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/dqyolo.py` & `dataquality-0.9.1a3/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/cv/torch/semantic_segmentation.py` & `dataquality-0.9.1a3/dataquality/integrations/cv/torch/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/experimental/keras.py` & `dataquality-0.9.1a3/dataquality/integrations/experimental/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/fastai.py` & `dataquality-0.9.1a3/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/hf.py` & `dataquality-0.9.1a3/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/keras.py` & `dataquality-0.9.1a3/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/spacy.py` & `dataquality-0.9.1a3/dataquality/integrations/spacy.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/torch.py` & `dataquality-0.9.1a3/dataquality/integrations/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/transformers_trainer.py` & `dataquality-0.9.1a3/dataquality/integrations/transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/integrations/ultralytics.py` & `dataquality-0.9.1a3/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/base_logger.py` & `dataquality-0.9.1a3/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/__init__.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/image_classification.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/object_detection.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.1a3/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.1a3/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/logger_config/object_detection.py` & `dataquality-0.9.1a3/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.1a3/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.1a3/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.1a3/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/image_classification.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/object_detection.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.1a3/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/metrics.py` & `dataquality-0.9.1a3/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/condition.py` & `dataquality-0.9.1a3/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/dataframe.py` & `dataquality-0.9.1a3/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/edit.py` & `dataquality-0.9.1a3/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/hf.py` & `dataquality-0.9.1a3/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/metrics.py` & `dataquality-0.9.1a3/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/ner.py` & `dataquality-0.9.1a3/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/report.py` & `dataquality-0.9.1a3/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/route.py` & `dataquality-0.9.1a3/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/semantic_segmentation.py` & `dataquality-0.9.1a3/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/split.py` & `dataquality-0.9.1a3/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/task_type.py` & `dataquality-0.9.1a3/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/schemas/torch.py` & `dataquality-0.9.1a3/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/ampli.py` & `dataquality-0.9.1a3/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/auto.py` & `dataquality-0.9.1a3/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/auto_trainer.py` & `dataquality-0.9.1a3/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/cuda.py` & `dataquality-0.9.1a3/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/cv.py` & `dataquality-0.9.1a3/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/dq_logger.py` & `dataquality-0.9.1a3/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/dqyolo.py` & `dataquality-0.9.1a3/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/emb.py` & `dataquality-0.9.1a3/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/file.py` & `dataquality-0.9.1a3/dataquality/utils/file.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/hdf5_store.py` & `dataquality-0.9.1a3/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/helpers.py` & `dataquality-0.9.1a3/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/hf_images.py` & `dataquality-0.9.1a3/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.1a3/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/keras.py` & `dataquality-0.9.1a3/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/ml.py` & `dataquality-0.9.1a3/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/name.py` & `dataquality-0.9.1a3/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/od.py` & `dataquality-0.9.1a3/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/profiler.py` & `dataquality-0.9.1a3/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-0.9.1a3/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/spacy_integration.py` & `dataquality-0.9.1a3/dataquality/utils/spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/thread_pool.py` & `dataquality-0.9.1a3/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/torch.py` & `dataquality-0.9.1a3/dataquality/utils/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/transformers.py` & `dataquality-0.9.1a3/dataquality/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/ultralytics.py` & `dataquality-0.9.1a3/dataquality/utils/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/upload.py` & `dataquality-0.9.1a3/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/vaex.py` & `dataquality-0.9.1a3/dataquality/utils/vaex.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/dataquality/utils/version.py` & `dataquality-0.9.1a3/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/Makefile` & `dataquality-0.9.1a3/docs/autodocs/Makefile`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/_build/doctrees/api/dataquality.doctree` & `dataquality-0.9.1a3/docs/autodocs/_build/doctrees/api/dataquality.doctree`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/_build/doctrees/environment.pickle` & `dataquality-0.9.1a3/docs/autodocs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/_build/doctrees/index.doctree` & `dataquality-0.9.1a3/docs/autodocs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/_build/markdown/api/dataquality.md` & `dataquality-0.9.1a3/docs/autodocs/_build/markdown/api/dataquality.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/_build/markdown/index.md` & `dataquality-0.9.1a3/docs/autodocs/_build/markdown/index.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/api/dataquality.rst` & `dataquality-0.9.1a3/docs/autodocs/api/dataquality.rst`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/conf.py` & `dataquality-0.9.1a3/docs/autodocs/conf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/autodocs/make.bat` & `dataquality-0.9.1a3/docs/autodocs/make.bat`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/cv/coco_deeplab_hooks.ipynb` & `dataquality-0.9.1a3/docs/cv/coco_deeplab_hooks.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/cv/cv-demo-hf.py` & `dataquality-0.9.1a3/docs/cv/cv-demo-hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/cv/cv-testing-benchmark.py` & `dataquality-0.9.1a3/docs/cv/cv-testing-benchmark.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/notebooks/Dataquality-Client-Demo.ipynb` & `dataquality-0.9.1a3/docs/notebooks/Dataquality-Client-Demo.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/notebooks/End to End runs per task type.ipynb` & `dataquality-0.9.1a3/docs/notebooks/End to End runs per task type.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/notebooks/Inference-Demo.ipynb` & `dataquality-0.9.1a3/docs/notebooks/Inference-Demo.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/notebooks/NER Inference.ipynb` & `dataquality-0.9.1a3/docs/notebooks/NER Inference.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/docs/notebooks/Tabular-Data.ipynb` & `dataquality-0.9.1a3/docs/notebooks/Tabular-Data.ipynb`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/pyproject.toml` & `dataquality-0.9.1a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/assets/images/Abyssinian_83.jpg` & `dataquality-0.9.1a3/tests/assets/images/Abyssinian_83.jpg`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/assets/images/pug_198.jpg` & `dataquality-0.9.1a3/tests/assets/images/pug_198.jpg`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/auto/test_ner_auto.py` & `dataquality-0.9.1a3/tests/auto/test_ner_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/auto/test_tc_auto.py` & `dataquality-0.9.1a3/tests/auto/test_tc_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/clients/test_api.py` & `dataquality-0.9.1a3/tests/clients/test_api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/conftest.py` & `dataquality-0.9.1a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/core/test_auth.py` & `dataquality-0.9.1a3/tests/core/test_auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/core/test_config.py` & `dataquality-0.9.1a3/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/core/test_finish.py` & `dataquality-0.9.1a3/tests/core/test_finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/core/test_init.py` & `dataquality-0.9.1a3/tests/core/test_init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/core/test_report.py` & `dataquality-0.9.1a3/tests/core/test_report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/inference/test_inference.py` & `dataquality-0.9.1a3/tests/inference/test_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/inference/test_text_classification_inf.py` & `dataquality-0.9.1a3/tests/inference/test_text_classification_inf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/inference/test_text_ner_inf.py` & `dataquality-0.9.1a3/tests/inference/test_text_ner_inf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integration/mock_training_run.py` & `dataquality-0.9.1a3/tests/integration/mock_training_run.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/fastai/test_cv_fai.py` & `dataquality-0.9.1a3/tests/integrations/fastai/test_cv_fai.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/hf/test_hf_integration.py` & `dataquality-0.9.1a3/tests/integrations/hf/test_hf_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/hf/test_text_classification_hf.py` & `dataquality-0.9.1a3/tests/integrations/hf/test_text_classification_hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/keras/test_experimental.py` & `dataquality-0.9.1a3/tests/integrations/keras/test_experimental.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/keras/test_utils.py` & `dataquality-0.9.1a3/tests/integrations/keras/test_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/spacy/conftest.py` & `dataquality-0.9.1a3/tests/integrations/spacy/conftest.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/spacy/test_spacy_integration.py` & `dataquality-0.9.1a3/tests/integrations/spacy/test_spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/spacy/test_spacy_ner.py` & `dataquality-0.9.1a3/tests/integrations/spacy/test_spacy_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/torch/test_dataloader_patching.py` & `dataquality-0.9.1a3/tests/integrations/torch/test_dataloader_patching.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/torch/test_pt_text_classification.py` & `dataquality-0.9.1a3/tests/integrations/torch/test_pt_text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/torch/test_pt_utils.py` & `dataquality-0.9.1a3/tests/integrations/torch/test_pt_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/ultralytics/coco128.yaml` & `dataquality-0.9.1a3/tests/integrations/ultralytics/coco128.yaml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/integrations/ultralytics/test_cv_yolo.py` & `dataquality-0.9.1a3/tests/integrations/ultralytics/test_cv_yolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/loggers/conftest.py` & `dataquality-0.9.1a3/tests/loggers/conftest.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/loggers/test_image_classification.py` & `dataquality-0.9.1a3/tests/loggers/test_image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/loggers/test_multi_label.py` & `dataquality-0.9.1a3/tests/loggers/test_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/loggers/test_ner.py` & `dataquality-0.9.1a3/tests/loggers/test_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/loggers/test_tabular_classification.py` & `dataquality-0.9.1a3/tests/loggers/test_tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/loggers/test_text_classification.py` & `dataquality-0.9.1a3/tests/loggers/test_text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/schemas/test_conditions.py` & `dataquality-0.9.1a3/tests/schemas/test_conditions.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/start/test_start_auto.py` & `dataquality-0.9.1a3/tests/start/test_start_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/start/test_start_hf.py` & `dataquality-0.9.1a3/tests/start/test_start_hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/start/test_start_keras.py` & `dataquality-0.9.1a3/tests/start/test_start_keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/start/test_start_pt.py` & `dataquality-0.9.1a3/tests/start/test_start_pt.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/start/test_start_spacy.md` & `dataquality-0.9.1a3/tests/start/test_start_spacy.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_dataquality.py` & `dataquality-0.9.1a3/tests/test_dataquality.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_telemetrics.py` & `dataquality-0.9.1a3/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/data_utils.py` & `dataquality-0.9.1a3/tests/test_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/hf_datasets_mock.py` & `dataquality-0.9.1a3/tests/test_utils/hf_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.1a3/tests/test_utils/hf_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.1a3/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/lightning_model.py` & `dataquality-0.9.1a3/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/mock_data.py` & `dataquality-0.9.1a3/tests/test_utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/mock_request.py` & `dataquality-0.9.1a3/tests/test_utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/ner_constants.py` & `dataquality-0.9.1a3/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/pt_datasets_mock.py` & `dataquality-0.9.1a3/tests/test_utils/pt_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/spacy_integration.py` & `dataquality-0.9.1a3/tests/test_utils/spacy_integration.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/spacy_integration_constants.py` & `dataquality-0.9.1a3/tests/test_utils/spacy_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/spacy_integration_constants_inference.py` & `dataquality-0.9.1a3/tests/test_utils/spacy_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/test_utils/tc_constants.py` & `dataquality-0.9.1a3/tests/test_utils/tc_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/utils/test_auto.py` & `dataquality-0.9.1a3/tests/utils/test_auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/utils/test_dq_logger.py` & `dataquality-0.9.1a3/tests/utils/test_dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/utils/test_name.py` & `dataquality-0.9.1a3/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/utils/test_vaex_utils.py` & `dataquality-0.9.1a3/tests/utils/test_vaex_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/tests/utils/test_version.py` & `dataquality-0.9.1a3/tests/utils/test_version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.1a2/PKG-INFO` & `dataquality-0.9.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.1a2
+Version: 0.9.1a3
 Summary: dataquality is a library for tracking and analyzing your machine learning models.
 Home-page: https://www.github.com/rungalileo/dataquality
 Author: Galileo Technologies, Inc
 Author-email: team@rungalileo.io
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=1.8.2
```

