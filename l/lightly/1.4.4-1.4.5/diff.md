# Comparing `tmp/lightly-1.4.4.tar.gz` & `tmp/lightly-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightly-1.4.4.tar", last modified: Wed May  3 08:37:35 2023, max compression
+gzip compressed data, was "lightly-1.4.5.tar", last modified: Thu May 11 16:27:59 2023, max compression
```

## Comparing `lightly-1.4.4.tar` & `lightly-1.4.5.tar`

### file list

```diff
@@ -1,409 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.071134 lightly-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 08:37:23.000000 lightly-1.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 08:37:23.000000 lightly-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-03 08:37:35.071134 lightly-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-05-03 08:37:23.000000 lightly-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.011133 lightly-1.4.4/lightly/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.011133 lightly-1.4.4/lightly/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.011133 lightly-1.4.4/lightly/active_learning/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/agents/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.011133 lightly-1.4.4/lightly/active_learning/config/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/config/selection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.015133 lightly-1.4.4/lightly/active_learning/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/scorers/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/scorers/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/scorers/keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/scorers/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.015133 lightly-1.4.4/lightly/active_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/utils/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/utils/keypoint_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/active_learning/utils/object_detection_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.019133 lightly-1.4.4/lightly/api/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_compute_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_upload_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/api_workflow_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/bitmask.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/swagger_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/swagger_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/api/version_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.023133 lightly-1.4.4/lightly/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/_cli_simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.023133 lightly-1.4.4/lightly/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/config/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/crop_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/embed_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/lightly_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/train_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/upload_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/cli/version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.027133 lightly-1.4.4/lightly/data/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/_image_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/_video.py
--rw-r--r--   0 runner    (1001) docker     (123)    49756 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/lightly_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/data/multi_view_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.027133 lightly-1.4.4/lightly/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/embedding/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/embedding/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/embedding/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.031133 lightly-1.4.4/lightly/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/dcl_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/dino_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/hypersphere_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/msn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/negative_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/ntx_ent_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/pmsn_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.031133 lightly-1.4.4/lightly/loss/regularizer/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/regularizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/regularizer/co2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/swav_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/sym_neg_cos_sim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/tico_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/vicreg_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/loss/vicregl_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.031133 lightly-1.4.4/lightly/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/byol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/moco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.031133 lightly-1.4.4/lightly/models/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/modules/heads.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/modules/masked_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/modules/nn_memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/nnclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)    17107 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.007133 lightly-1.4.4/lightly/openapi_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.035133 lightly-1.4.4/lightly/openapi_generated/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    25019 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.035133 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/collaboration_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    76297 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/datasources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/docker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/embeddings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/predictions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/quota_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47328 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/samples_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/samplings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/scores_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api/versioning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.067134 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    23388 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/access_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/api_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/api_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/async_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/category_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/category_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/create_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_license_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/file_name_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/file_output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/general_job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/jobs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_studio_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/path_safe_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/s3_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sama_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sama_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sama_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_input_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/shared_access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/task_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/team_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/team_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/version_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/video_frame_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/openapi_generated/swagger_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.071134 lightly-1.4.4/lightly/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/dino_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/fast_siam_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/image_grid_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/mae_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/moco_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/msn_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/multi_crop_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/multi_view_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/pirl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/random_crop_and_flip_with_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/simclr_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/simsiam_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/smog_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/swav_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/vicreg_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/transforms/vicregl_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.071134 lightly-1.4.4/lightly/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/benchmarking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.071134 lightly-1.4.4/lightly/utils/cropping/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/cropping/crop_image_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/cropping/read_yolo_label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/embeddings_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/hipify.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/reordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-03 08:37:23.000000 lightly-1.4.4/lightly/utils/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:37:35.011133 lightly-1.4.4/lightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-03 08:37:34.000000 lightly-1.4.4/lightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-05-03 08:37:34.000000 lightly-1.4.4/lightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:37:34.000000 lightly-1.4.4/lightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 08:37:34.000000 lightly-1.4.4/lightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-03 08:37:34.000000 lightly-1.4.4/lightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 08:37:34.000000 lightly-1.4.4/lightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 08:37:23.000000 lightly-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-03 08:37:35.071134 lightly-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-03 08:37:23.000000 lightly-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 16:27:51.000000 lightly-1.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 16:27:51.000000 lightly-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 16:27:59.601920 lightly-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-05-11 16:27:51.000000 lightly-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/agents/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/config/selection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/keypoint_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/object_detection_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.569920 lightly-1.4.5/lightly/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_compute_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29042 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_upload_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/swagger_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/swagger_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/version_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.569920 lightly-1.4.5/lightly/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/_cli_simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.569920 lightly-1.4.5/lightly/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/config/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/crop_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/download_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/embed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/lightly_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/train_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/upload_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_image_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49756 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/lightly_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/multi_view_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/dcl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/dino_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/hypersphere_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/msn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/negative_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/ntx_ent_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/pmsn_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/loss/regularizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/regularizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/regularizer/co2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/swav_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/sym_neg_cos_sim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/tico_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/vicreg_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/vicregl_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/byol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/moco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/models/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/masked_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/nn_memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/nnclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18480 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/openapi_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/openapi_generated/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    25152 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.577920 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/collaboration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78621 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/docker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/mappings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/predictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/quota_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52413 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samples_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samplings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/scores_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/versioning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.597920 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    23521 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/access_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/async_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_license_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_name_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/general_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/jobs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/path_safe_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/version_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/video_frame_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/lightly/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/dino_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/fast_siam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/image_grid_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/mae_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/moco_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/msn_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/multi_crop_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/multi_view_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/pirl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/random_crop_and_flip_with_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/simclr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/simsiam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/smog_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/swav_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/vicreg_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/vicregl_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/lightly/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/lightly/utils/cropping/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/cropping/crop_image_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/cropping/read_yolo_label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/embeddings_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/hipify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/reordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 16:27:51.000000 lightly-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 16:27:59.601920 lightly-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-11 16:27:51.000000 lightly-1.4.5/setup.py
```

### Comparing `lightly-1.4.4/LICENSE.txt` & `lightly-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/PKG-INFO` & `lightly-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.4
+Version: 1.4.5
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.4/README.md` & `lightly-1.4.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,360 +1,433 @@
 
 ![Lightly Logo](docs/logos/lightly_logo_crop.png)
 
-
 ![GitHub](https://img.shields.io/github/license/lightly-ai/lightly)
 ![Unit Tests](https://github.com/lightly-ai/lightly/workflows/Unit%20Tests/badge.svg)
-![codecov](https://codecov.io/gh/lightly-ai/lightly/branch/master/graph/badge.svg?token=1NEAVROK3W)
+[![PyPI](https://img.shields.io/pypi/v/lightly)](https://pypi.org/project/lightly/)
+[![Downloads](https://pepy.tech/badge/lightly)](https://pepy.tech/project/lightly)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Lightly is a computer vision framework for self-supervised learning.
 
-> We, at [Lightly](https://www.lightly.ai), are passionate engineers who want to make deep learning more efficient. That's why - together with our community - we want to popularize the use of self-supervised methods to understand and curate raw image data. Our solution can be applied before any data annotation step and the learned representations can be used to visualize and analyze datasets. This allows to select the best core set of samples for model training through advanced filtering.
+> We, at [Lightly](https://www.lightly.ai), are passionate engineers who want to make deep learning more efficient. That's why - together with our community - we want to popularize the use of self-supervised methods to understand and curate raw image data. Our solution can be applied before any data annotation step and the learned representations can be used to visualize and analyze datasets. This allows to select the best set of samples for model training through advanced filtering.
 
 - [Homepage](https://www.lightly.ai)
 - [Web-App](https://app.lightly.ai)
 - [Documentation](https://docs.lightly.ai/self-supervised-learning/)
+- [Lightly Solution Documentation (Lightly Worker & API)](https://docs.lightly.ai/)
 - [Github](https://github.com/lightly-ai/lightly)
-- [Discord](https://discord.gg/xvNJW94)
+- [Discord](https://discord.gg/xvNJW94) (We have weekly paper sessions!)
+
 
-### Features
+## Features
 
 Lightly offers features like
 
-- modular framework which exposes low-level building blocks such as loss functions
-- support for multi-gpu training using PyTorch Lightning
-- easy to use and written in a PyTorch like style
-- supports custom backbone models for self-supervised pre-training
-
-#### Supported Models
-
-You can [find sample code for all the supported models here.](https://docs.lightly.ai/self-supervised-learning/examples/models.html)
-We provide PyTorch, PyTorch Lightning and PyTorch Lightning distributed examples for each of the models
-to kickstart your project.
-
-Some of our supported models:
-
-- [Barlow Twins, 2021](https://arxiv.org/abs/2103.03230)
-- [BYOL, 2020](https://arxiv.org/abs/2006.07733)
-- [DCL & DCLW, 2021](https://arxiv.org/abs/2110.06848)
-- [DINO, 2021](https://arxiv.org/abs/2104.14294)
-- [MAE, 2021](https://arxiv.org/abs/2111.06377)
-- [MSN, 2022](https://arxiv.org/abs/2204.07141)
-- [MoCo, 2019](https://arxiv.org/abs/1911.05722)
-- [NNCLR, 2021](https://arxiv.org/abs/2104.14548)
-- [PMSN, 2022](https://arxiv.org/abs/2210.07277)
-- [SimCLR, 2020](https://arxiv.org/abs/2002.05709)
-- [SimMIM, 2021](https://arxiv.org/abs/2111.09886)
-- [SimSiam, 2021](https://arxiv.org/abs/2011.10566)
-- [SMoG, 2022](https://arxiv.org/abs/2207.06167)
-- [SwaV, 2020](https://arxiv.org/abs/2006.09882)
-- [TiCo, 2022](https://arxiv.org/abs/2206.10698)
-- [VICReg, 2022](https://arxiv.org/abs/2105.04906)
-- [VICRegL, 2022](https://arxiv.org/abs/2210.01571)
+- Modular framework which exposes low-level building blocks such as loss functions and
+  model heads.
+- Easy to use and written in a PyTorch like style.
+- Supports custom backbone models for self-supervised pre-training.
+- Support for distributed training using PyTorch Lightning.
+
+
+### Supported Models
+
+You can [find sample code for all the supported models here.](https://docs.lightly.ai/self-supervised-learning/examples/models.html) We provide PyTorch, PyTorch Lightning,
+and PyTorch Lightning distributed examples for all models to kickstart your project.
+
+**Models**:
+
+- Barlow Twins, 2021 [paper](https://arxiv.org/abs/2103.03230) [docs](https://docs.lightly.ai/self-supervised-learning/examples/barlowtwins.html)
+- BYOL, 2020 [paper](https://arxiv.org/abs/2006.07733) [docs](https://docs.lightly.ai/self-supervised-learning/examples/byol.html)
+- DCL & DCLW, 2021 [paper](https://arxiv.org/abs/2110.06848) [docs](https://docs.lightly.ai/self-supervised-learning/examples/dcl.html)
+- DINO, 2021 [paper](https://arxiv.org/abs/2104.14294) [docs](https://docs.lightly.ai/self-supervised-learning/examples/dino.html)
+- MAE, 2021 [paper](https://arxiv.org/abs/2111.06377) [docs](https://docs.lightly.ai/self-supervised-learning/examples/mae.html)
+- MSN, 2022 [paper](https://arxiv.org/abs/2204.07141) [docs](https://docs.lightly.ai/self-supervised-learning/examples/msn.html)
+- MoCo, 2019 [paper](https://arxiv.org/abs/1911.05722) [docs](https://docs.lightly.ai/self-supervised-learning/examples/moco.html)
+- NNCLR, 2021 [paper](https://arxiv.org/abs/2104.14548) [docs](https://docs.lightly.ai/self-supervised-learning/examples/nnclr.html)
+- PMSN, 2022 [paper](https://arxiv.org/abs/2210.07277) [docs](https://docs.lightly.ai/self-supervised-learning/examples/pmsn.html)
+- SimCLR, 2020 [paper](https://arxiv.org/abs/2002.05709) [docs](https://docs.lightly.ai/self-supervised-learning/examples/simclr.html)
+- SimMIM, 2021 [paper](https://arxiv.org/abs/2111.09886) [docs](https://docs.lightly.ai/self-supervised-learning/examples/simmim.html)
+- SimSiam, 2021 [paper](https://arxiv.org/abs/2011.10566) [docs](https://docs.lightly.ai/self-supervised-learning/examples/simsiam.html)
+- SMoG, 2022 [paper](https://arxiv.org/abs/2207.06167) [docs](https://docs.lightly.ai/self-supervised-learning/examples/smog.html)
+- SwaV, 2020 [paper](https://arxiv.org/abs/2006.09882) [docs](https://docs.lightly.ai/self-supervised-learning/examples/swav.html)
+- TiCo, 2022 [paper](https://arxiv.org/abs/2206.10698) [docs](https://docs.lightly.ai/self-supervised-learning/examples/tico.html)
+- VICReg, 2022 [paper](https://arxiv.org/abs/2105.04906) [docs](https://docs.lightly.ai/self-supervised-learning/examples/vicreg.html)
+- VICRegL, 2022 [paper](https://arxiv.org/abs/2210.01571) [docs](https://docs.lightly.ai/self-supervised-learning/examples/vicregl.html)
 
 
-### Tutorials
+## Tutorials
 
-Want to jump to the tutorials and see lightly in action?
+Want to jump to the tutorials and see Lightly in action?
 
 - [Train MoCo on CIFAR-10](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_moco_memory_bank.html)
-- [Train SimCLR on clothing data](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_simclr_clothing.html)
-- [Train SimSiam on satellite images](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_simsiam_esa.html)
-- [Use lightly with custom augmentations](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_custom_augmentations.html)
+- [Train SimCLR on Clothing Data](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_simclr_clothing.html)
+- [Train SimSiam on Satellite Images](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_simsiam_esa.html)
+- [Use Lightly with Custom Augmentations](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_custom_augmentations.html)
 - [Pre-train a Detectron2 Backbone with Lightly](https://docs.lightly.ai/self-supervised-learning/tutorials/package/tutorial_pretrain_detectron2.html)
 
-Documentation and tutorials of using the Lightly Solution:
+Tutorials for the Lightly Solution (Lightly Worker & API):
 
 - [General Docs of Lightly Solution](https://docs.lightly.ai)
 - [Active Learning Using YOLOv7 and Comma10k](https://docs.lightly.ai/docs/active-learning-yolov7)
 - [Active Learning for Driveable Area Segmentation Using Cityscapes](https://docs.lightly.ai/docs/active-learning-for-driveable-area-segmentation-using-cityscapes)
 - [Active Learning for Transactions of Images](https://docs.lightly.ai/docs/active-learning-for-transactions-of-images)
 - [Improving YOLOv8 using Active Learning on Videos](https://docs.lightly.ai/docs/active-learning-yolov8-video)
 - [Assertion-based Active Learning with YOLOv8](https://docs.lightly.ai/docs/assertion-based-active-learning-tutorial)
 - and more ...
 
 
 Community and partner projects:
 
 - [On-Device Deep Learning with Lightly on an ARM microcontroller](https://github.com/ARM-software/EndpointAI/tree/master/ProofOfConcepts/Vision/OpenMvMaskDefaults)
 
+
 ## Quick Start
 
-Lightly requires **Python 3.6+** but we recommend using **Python 3.7+**.
-We recommend installing Lightly in a **Linux** or **OSX** environment.
+Lightly requires **Python 3.6+** but we recommend using **Python 3.7+**. We recommend installing Lightly in a **Linux** or **OSX** environment.
 
 ### Dependencies
 
-- hydra-core>=1.0.0
-- numpy>=1.18.1
-- pytorch_lightning>=1.5
-- requests>=2.23.0
-- torchvision
-- tqdm
+- [PyTorch](https://pytorch.org/)
+- [Torchvision](https://pytorch.org/vision/stable/index.html)
+- [PyTorch Lightning](https://www.pytorchlightning.ai/index.html) v1.5+
+
+Lightly is compatible with PyTorch and PyTorch Lightning v2.0+!
+
+Vision transformer based models require Torchvision v0.12+.
 
 ### Installation
 You can install Lightly and its dependencies from PyPI with:
 ```
 pip3 install lightly
 ```
 
-We strongly recommend that you install Lightly in a dedicated virtualenv, to avoid conflicting with your system packages.
+We strongly recommend that you install Lightly in a dedicated virtualenv, to avoid
+conflicting with your system packages.
+
+If you only want to install the API client without torch and torchvision dependencies
+follow the docs on [how to install the Lightly Python Client](https://docs.lightly.ai/docs/install-lightly#install-the-lightly-python-client).
 
 
 ### Lightly in Action
 
-With lightly, you can use the latest self-supervised learning methods in a modular
+With Lightly, you can use the latest self-supervised learning methods in a modular
 way using the full power of PyTorch. Experiment with different backbones,
 models, and loss functions. The framework has been designed to be easy to use
 from the ground up. [Find more examples in our docs](https://docs.lightly.ai/self-supervised-learning/examples/models.html).
 
 ```python
 import torch
 import torchvision
-import lightly.models as models
-import lightly.loss as loss
-import lightly.data as data
-
-# the collate function applies random transforms to the input images
-collate_fn = data.ImageCollateFunction(input_size=32, cj_prob=0.5)
 
-# create a dataset from your image folder
-dataset = data.LightlyDataset(input_dir='./my/cute/cats/dataset/')
+from lightly import loss
+from lightly import transforms
+from lightly.data import LightlyDataset
+from lightly.data.multi_view_collate import MultiViewCollate
+from lightly.models.modules import heads
 
-# build a PyTorch dataloader
-dataloader = torch.utils.data.DataLoader(
-    dataset,                # pass the dataset to the dataloader
-    batch_size=128,         # a large batch size helps with the learning
-    shuffle=True,           # shuffling is important!
-    collate_fn=collate_fn)  # apply transformations to the input images
 
-
-# create a PyTorch module for the SimCLR model
-class SimCLR(nn.Module):
+# Create a PyTorch module for the SimCLR model.
+class SimCLR(torch.nn.Module):
     def __init__(self, backbone):
         super().__init__()
         self.backbone = backbone
-        self.projection_head = models.modules.SimCLRProjectionHead(
-          input_dim=512, 
-          hidden_dim=512,
-          output_dim=128
+        self.projection_head = heads.SimCLRProjectionHead(
+            input_dim=512,  # Resnet18 features have 512 dimensions.
+            hidden_dim=512,
+            output_dim=128,
         )
 
     def forward(self, x):
-        x = self.backbone(x).flatten(start_dim=1)
-        z = self.projection_head(x)
+        features = self.backbone(x).flatten(start_dim=1)
+        z = self.projection_head(features)
         return z
 
-# use a resnet backbone
-resnet = torchvision.models.resnet18()
-backbone = nn.Sequential(*list(resnet.children())[:-1])
 
-# build the simclr model
+# Use a resnet backbone.
+backbone = torchvision.models.resnet18()
+# Ignore the classification head as we only want the features.
+backbone.fc = torch.nn.Identity()
+
+# Build the SimCLR model.
 model = SimCLR(backbone)
 
-# lightly exposes building blocks such as loss functions
+# Prepare transform that creates multiple random views for every image.
+transform = transforms.SimCLRTransform(input_size=32, cj_prob=0.5)
+
+# Combine views from multiple images into a batch.
+collate_fn = MultiViewCollate()
+
+# Create a dataset from your image folder.
+dataset = data.LightlyDataset(input_dir="./my/cute/cats/dataset/", transform=transform)
+
+# Build a PyTorch dataloader.
+dataloader = torch.utils.data.DataLoader(
+    dataset,  # Pass the dataset to the dataloader.
+    batch_size=128,  # A large batch size helps with the learning.
+    shuffle=True,  # Shuffling is important!
+    collate_fn=collate_fn,
+)
+
+# Lightly exposes building blocks such as loss functions.
 criterion = loss.NTXentLoss(temperature=0.5)
 
-# get a PyTorch optimizer
-optimizer = torch.optim.SGD(model.parameters(), lr=1e-0, weight_decay=1e-5)
+# Get a PyTorch optimizer.
+optimizer = torch.optim.SGD(model.parameters(), lr=0.1, weight_decay=1e-6)
+
+# Train the model.
+for epoch in range(10):
+    for (view0, view1), targets, filenames in dataloader:
+        z0 = model(view0)
+        z1 = model(view1)
+        loss = criterion(z0, z1)
+        loss.backward()
+        optimizer.step()
+        optimizer.zero_grad()
+        print(f"loss: {loss.item():.5f}")
 ```
 
 You can easily use another model like SimSiam by swapping the model and the
 loss function.
+
 ```python
-# PyTorch module for the SimSiam model
-class SimSiam(nn.Module):
+# PyTorch module for the SimSiam model.
+class SimSiam(torch.nn.Module):
     def __init__(self, backbone):
         super().__init__()
         self.backbone = backbone
-        self.projection_head = SimSiamProjectionHead(512, 512, 128)
-        self.prediction_head = SimSiamPredictionHead(128, 64, 128)
+        self.projection_head = heads.SimSiamProjectionHead(512, 512, 128)
+        self.prediction_head = heads.SimSiamPredictionHead(128, 64, 128)
 
     def forward(self, x):
-        f = self.backbone(x).flatten(start_dim=1)
-        z = self.projection_head(f)
+        features = self.backbone(x).flatten(start_dim=1)
+        z = self.projection_head(features)
         p = self.prediction_head(z)
         z = z.detach()
         return z, p
 
+
 model = SimSiam(backbone)
 
-# use the SimSiam loss function
+# Use the SimSiam loss function.
 criterion = loss.NegativeCosineSimilarity()
 ```
+
 You can [find a more complete example for SimSiam here.](https://docs.lightly.ai/self-supervised-learning/examples/simsiam.html)
 
 
 Use PyTorch Lightning to train the model:
 
 ```python
-trainer = pl.Trainer(max_epochs=max_epochs, devices=1, accelerator="gpu")
-trainer.fit(
-    model,
-    dataloader
-)
+from pytorch_lightning import LightningModule, Trainer
+
+class SimCLR(LightningModule):
+    def __init__(self):
+        super().__init__()
+        resnet = torchvision.models.resnet18()
+        resnet.fc = torch.nn.Identity()
+        self.backbone = resnet
+        self.projection_head = heads.SimCLRProjectionHead(512, 512, 128)
+        self.criterion = loss.NTXentLoss()
+
+    def forward(self, x):
+        features = self.backbone(x).flatten(start_dim=1)
+        z = self.projection_head(features)
+        return z
+
+    def training_step(self, batch, batch_index):
+        (view0, view1), _, _ = batch
+        z0 = self.forward(view0)
+        z1 = self.forward(view1)
+        loss = self.criterion(z0, z1)
+        return loss
+
+    def configure_optimizers(self):
+        optim = torch.optim.SGD(self.parameters(), lr=0.06)
+        return optim
+
+
+model = SimCLR()
+trainer = Trainer(max_epochs=10, devices=1, accelerator="gpu")
+trainer.fit(model, dataloader)
 ```
 
+See [our docs for a full PyTorch Lightning example.](https://docs.lightly.ai/self-supervised-learning/examples/simclr.html)
+
 Or train the model on 4 GPUs:
 ```python
 
-# use distributed version of loss functions
-criterion = NTXentLoss(gather_distributed=True)
+# Use distributed version of loss functions.
+criterion = loss.NTXentLoss(gather_distributed=True)
 
-trainer = pl.Trainer(
-    max_epochs=max_epochs, 
+trainer = Trainer(
+    max_epochs=10,
     devices=4,
     accelerator="gpu",
     strategy="ddp",
+    sync_batchnorm=True,
+    use_distributed_sampler=True,  # or replace_sampler_ddp=True for PyTorch Lightning <2.0
 )
-trainer.fit(
-    model,
-    dataloader
-)
+trainer.fit(model, dataloader)
 ```
 
-We provide proper multi-GPU training with distributed gather and synchronized BatchNorm.
-
-[Have a look at our docs regarding distributed training](https://docs.lightly.ai/self-supervised-learning/getting_started/distributed_training.html)
+We provide multi-GPU training examples with distributed gather and synchronized BatchNorm.
+[Have a look at our docs regarding distributed training.](https://docs.lightly.ai/self-supervised-learning/getting_started/distributed_training.html)
 
 
+## Benchmarks
 
-### Benchmarks
+Implemented models and their performance on various datasets. Hyperparameters are not
+tuned for maximum accuracy. For detailed results and more info about the benchmarks click
+[here](https://docs.lightly.ai/self-supervised-learning/getting_started/benchmarks.html).
+
+
+### Imagenet
+
+| Model       | Backbone | Batch Size | Epochs | Linear Top1 | Linear Top1 Online | KNN Top1 | Tensorboard | Checkpoint |
+|-------------|----------|------------|--------|-------------|--------------------|----------|-------------|------------|
+| SimCLR      | Res50    |        256 |    100 |        63.2 |               63.1 |     44.9 |      [link](https://tensorboard.dev/experiment/JwNs9E02TeeQkS7aljh8dA) |       [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-05-04_09-02-54/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
+
+
+### ImageNette
+
+| Model       | Backbone | Batch Size | Epochs | KNN Top1 |
+|-------------|----------|------------|--------|----------|
+| BarlowTwins | Res18    |        256 |    800 |    0.852 |
+| BYOL        | Res18    |        256 |    800 |    0.887 |
+| DCL         | Res18    |        256 |    800 |    0.861 |
+| DCLW        | Res18    |        256 |    800 |    0.865 |
+| DINO        | Res18    |        256 |    800 |    0.888 |
+| FastSiam    | Res18    |        256 |    800 |    0.873 |
+| MAE         | ViT-S    |        256 |    800 |    0.610 |
+| MSN         | ViT-S    |        256 |    800 |    0.828 |
+| Moco        | Res18    |        256 |    800 |    0.874 |
+| NNCLR       | Res18    |        256 |    800 |    0.884 |
+| PMSN        | ViT-S    |        256 |    800 |    0.822 |
+| SimCLR      | Res18    |        256 |    800 |    0.889 |
+| SimMIM      | ViT-B32  |        256 |    800 |    0.343 |
+| SimSiam     | Res18    |        256 |    800 |    0.872 |
+| SwaV        | Res18    |        256 |    800 |    0.902 |
+| SwaVQueue   | Res18    |        256 |    800 |    0.890 |
+| SMoG        | Res18    |        256 |    800 |    0.788 |
+| TiCo        | Res18    |        256 |    800 |    0.856 |
+| VICReg      | Res18    |        256 |    800 |    0.845 |
+| VICRegL     | Res18    |        256 |    800 |    0.778 |
+
+
+### Cifar10
+
+| Model       | Backbone | Batch Size | Epochs | KNN Top1 |
+|-------------|----------|------------|--------|----------|
+| BarlowTwins | Res18    |        512 |    800 |    0.859 |
+| BYOL        | Res18    |        512 |    800 |    0.910 |
+| DCL         | Res18    |        512 |    800 |    0.874 |
+| DCLW        | Res18    |        512 |    800 |    0.871 |
+| DINO        | Res18    |        512 |    800 |    0.848 |
+| FastSiam    | Res18    |        512 |    800 |    0.902 |
+| Moco        | Res18    |        512 |    800 |    0.899 |
+| NNCLR       | Res18    |        512 |    800 |    0.892 |
+| SimCLR      | Res18    |        512 |    800 |    0.879 |
+| SimSiam     | Res18    |        512 |    800 |    0.904 |
+| SwaV        | Res18    |        512 |    800 |    0.884 |
+| SMoG        | Res18    |        512 |    800 |    0.800 |
 
-Currently implemented models and their accuracy on cifar10 and imagenette. All models have been evaluated using kNN. We report the max test accuracy over the epochs as well as the maximum GPU memory consumption. All models in this benchmark use the same augmentations as well as the same ResNet-18 backbone. Training precision is set to FP32 and SGD is used as an optimizer with cosineLR.
-One epoch on cifar10 takes ~35 seconds on a V100 GPU. [Learn more about the cifar10 and imagenette benchmark here](https://docs.lightly.ai/self-supervised-learning/getting_started/benchmarks.html)
-
-#### ImageNette
-
-| Model            | Batch Size | Epochs | KNN Test Accuracy |
-|------------------|------------|--------|-------------------|
-| BarlowTwins      |        256 |    800 |             0.850 |
-| BYOL             |        256 |    800 |             0.887 |
-| DCL              |        256 |    800 |             0.864 |
-| DCLW             |        256 |    800 |             0.861 |
-| DINO (Res18)     |        256 |    800 |             0.887 |
-| FastSiam         |        256 |    800 |             0.865 |
-| MAE (ViT-S)      |        256 |    800 |             0.620 |
-| MSN (ViT-S)      |        256 |    800 |             0.833 |
-| Moco             |        256 |    800 |             0.874 |
-| NNCLR            |        256 |    800 |             0.885 |
-| PMSN (ViT-S)     |        256 |    800 |             0.830 |
-| SimCLR           |        256 |    800 |             0.889 |
-| SimMIM (ViT-B32) |        256 |    800 |             0.351 |
-| SimSiam          |        256 |    800 |             0.871 |
-| SwaV             |        256 |    800 |             0.899 |
-| SwaVQueue        |        256 |    800 |             0.898 |
-| SMoG             |        256 |    800 |             0.782 |
-| TiCo             |        256 |    800 |             0.857 |
-| VICReg           |        256 |    800 |             0.843 |
-| VICRegL          |        256 |    800 |             0.781 |
-
-
-#### Cifar10
-
-| Model         | Batch Size | Epochs | KNN Test Accuracy |
-|---------------|------------|--------|-------------------|
-| BarlowTwins   |        512 |    800 |             0.859 |
-| BYOL          |        512 |    800 |             0.910 |
-| DCL           |        512 |    800 |             0.874 |
-| DCLW          |        512 |    800 |             0.871 |
-| DINO          |        512 |    800 |             0.848 |
-| FastSiam      |        512 |    800 |             0.902 |
-| Moco (*)      |        512 |    800 |             0.899 |
-| NNCLR (*)     |        512 |    800 |             0.892 |
-| SimCLR        |        512 |    800 |             0.879 |
-| SimSiam       |        512 |    800 |             0.904 |
-| SwaV          |        512 |    800 |             0.884 |
-| SMoG          |        512 |    800 |             0.800 |
 
 ## Terminology
 
-Below you can see a schematic overview of the different concepts present in the lightly Python package. The terms in bold are explained in more detail in our [documentation](https://docs.lightly.ai/self-supervised-learning/).
+Below you can see a schematic overview of the different concepts in the package.
+The terms in bold are explained in more detail in our [documentation](https://docs.lightly.ai/self-supervised-learning/).
 
-<img src="/docs/source/getting_started/images/lightly_overview.png" alt="Overview of the lightly pip package"/></a>
+<img src="/docs/source/getting_started/images/lightly_overview.png" alt="Overview of the Lightly pip package"/></a>
 
 
 ### Next Steps
-Head to the [documentation](https://docs.lightly.ai) and see the things you can achieve with lightly!
+
+Head to the [documentation](https://docs.lightly.ai) and see the things you can achieve with Lightly!
 
 
 ## Development
 
-To install dev dependencies (for example to contribute to the framework)
-you can use the following command:
+To install dev dependencies (for example to contribute to the framework) you can use the following command:
 ```
 pip3 install -e ".[dev]"
 ```
 
 For more information about how to contribute have a look [here](CONTRIBUTING.md).
 
+
 ### Running Tests
 
-Unit tests are within the [tests folder](tests/) and we recommend running them using 
-[pytest](https://docs.pytest.org/en/stable/).
-There are two test configurations available. By default, only a subset will be run.
-This is faster and should take less than a minute. You can run it using
+Unit tests are within the [tests directory](tests/) and we recommend running them using 
+[pytest](https://docs.pytest.org/en/stable/). There are two test configurations
+available. By default, only a subset will be run:
 ```
-python -m pytest -s -v
+make test-fast
 ```
 
-To run all tests (including the slow ones) you can use the following command.
+To run all tests (including the slow ones) you can use the following command:
 ```
-python -m pytest -s -v --runslow
+make test
 ```
 
-### Code Linting
-We provide a [Pylint](https://github.com/PyCQA/pylint) config following the
-[Google Python Style Guide](https://github.com/google/styleguide/blob/gh-pages/pyguide.md).
-
-You can run the linter from your terminal either on a folder
+To test a specific file or directory use:
 ```
-pylint lightly/
+pytest <path to file or directory>
 ```
-or on a specific file
+
+
+### Code Formatting
+
+To format code with [black](https://black.readthedocs.io/en/stable/) and [isort](https://docs.pytest.org) run:
 ```
-pylint lightly/core.py
+make format
 ```
 
 
 ## Further Reading
 
-**Self-supervised Learning:**
-- [A Simple Framework for Contrastive Learning of Visual Representations (2020)](https://arxiv.org/abs/2002.05709)
-- [Momentum Contrast for Unsupervised Visual Representation Learning (2020)](https://arxiv.org/abs/1911.05722)
-- [Unsupervised Learning of Visual Features by Contrasting Cluster Assignments (2020)](https://arxiv.org/abs/2006.09882)
-- [What Should Not Be Contrastive in Contrastive Learning (2020)](https://arxiv.org/abs/2008.05659)
+**Self-Supervised Learning**:
+- Have a look at our [#papers channel on discord](https://discord.com/channels/752876370337726585/815153188487299083)
+  for the newest self-supervised learning papers.
+- [A Cookbook of Self-Supervised Learning, 2023](https://arxiv.org/abs/2304.12210)
+- [Masked Autoencoders Are Scalable Vision Learners, 2021](https://arxiv.org/abs/2111.06377)
+- [Emerging Properties in Self-Supervised Vision Transformers, 2021](https://arxiv.org/abs/2104.14294)
+- [Unsupervised Learning of Visual Features by Contrasting Cluster Assignments, 2021](https://arxiv.org/abs/2006.09882)
+- [What Should Not Be Contrastive in Contrastive Learning, 2020](https://arxiv.org/abs/2008.05659)
+- [A Simple Framework for Contrastive Learning of Visual Representations, 2020](https://arxiv.org/abs/2002.05709)
+- [Momentum Contrast for Unsupervised Visual Representation Learning, 2020](https://arxiv.org/abs/1911.05722)
+
 
 ## FAQ
 
 - Why should I care about self-supervised learning? Aren't pre-trained models from ImageNet much better for transfer learning?
-  - Self-supervised learning has become increasingly popular among scientists over the last year because the learned representations perform extraordinarily well on downstream tasks. This means that they capture the important information in an image better than other types of pre-trained models. By training a self-supervised model on *your* dataset, you can make sure that the representations have all the necessary information about your images.
+  - Self-supervised learning has become increasingly popular among scientists over the last years because the learned representations perform extraordinarily well on downstream tasks. This means that they capture the important information in an image better than other types of pre-trained models. By training a self-supervised model on *your* dataset, you can make sure that the representations have all the necessary information about your images.
 
 - How can I contribute?
   - Create an issue if you encounter bugs or have ideas for features we should implement. You can also add your own code by forking this repository and creating a PR. More details about how to contribute with code is in our [contribution guide](CONTRIBUTING.md).
 
 - Is this framework for free?
-  - Yes, this framework is completely free to use and we provide the source code. We believe that
-  we need to make training deep learning models more data efficient to achieve widespread adoption. One step to achieve this goal is by leveraging self-supervised learning. The company behind Lightly is committed to keep this framework open-source.
+  - Yes, this framework is completely free to use and we provide the source code. We believe that we need to make training deep learning models more data efficient to achieve widespread adoption. One step to achieve this goal is by leveraging self-supervised learning. The company behind Lightly is committed to keep this framework open-source.
 
-- If this framework is free, how is the company behind lightly making money?
+- If this framework is free, how is the company behind Lightly making money?
   - Training self-supervised models is only one part of our solution. 
-  [The company behind lightly](https://lightly.ai/) focuses on processing and analyzing embeddings created by self-supervised models. 
+  [The company behind Lightly](https://lightly.ai/) focuses on processing and analyzing embeddings created by self-supervised models. 
   By building, what we call a self-supervised active learning loop we help companies understand and work with their data more efficiently. 
   As the [Lightly Solution](https://docs.lightly.ai) is a freemium product, you can try it out for free. However, we will charge for some features.
   - In any case this framework will always be free to use, even for commercial purposes.
 
 
 ## Lightly in Research
 
-- [Learning Visual Representations via Language-Guided Sampling](https://arxiv.org/pdf/2302.12248.pdf)
-- [Decoupled Contrastive Learning](https://arxiv.org/abs/2110.06848)
-- [DPCL: Constrative Representation Learning with Differential Privacy](https://assets.researchsquare.com/files/rs-1516950/v1_covered.pdf?c=1654486158)
-- [Self-Supervised Learning Methods for Label-Efficient Dental Caries Classification](https://www.mdpi.com/2075-4418/12/5/1237)
-- [solo-learn: A Library of Self-supervised Methods for Visual Representation Learning](https://www.jmlr.org/papers/volume23/21-1155/21-1155.pdf)
+- [Learning Visual Representations via Language-Guided Sampling, 2023](https://arxiv.org/pdf/2302.12248.pdf)
+- [Self-Supervised Learning Methods for Label-Efficient Dental Caries Classification, 2022](https://www.mdpi.com/2075-4418/12/5/1237)
+- [DPCL: Constrative Representation Learning with Differential Privacy, 2022](https://assets.researchsquare.com/files/rs-1516950/v1_covered.pdf?c=1654486158)
+- [Decoupled Contrastive Learning, 2021](https://arxiv.org/abs/2110.06848)
+- [solo-learn: A Library of Self-supervised Methods for Visual Representation Learning, 2021](https://www.jmlr.org/papers/volume23/21-1155/21-1155.pdf)
 
 
 ## BibTeX
 If you want to cite the framework feel free to use this:
 
 ```bibtex
 @article{susmelj2020lightly,
```

### Comparing `lightly-1.4.4/lightly/__init__.py` & `lightly-1.4.5/lightly/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 __name__ = "lightly"
-__version__ = "1.4.4"
+__version__ = "1.4.5"
 
 import os
 
 try:
     # See (https://github.com/PyTorchLightning/pytorch-lightning)
     # This variable is injected in the __builtins__ by the build
     # process. It used to enable importing subpackages of skimage when
```

### Comparing `lightly-1.4.4/lightly/active_learning/agents/agent.py` & `lightly-1.4.5/lightly/active_learning/agents/agent.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/config/selection_config.py` & `lightly-1.4.5/lightly/active_learning/config/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/scorers/classification.py` & `lightly-1.4.5/lightly/active_learning/scorers/classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/scorers/detection.py` & `lightly-1.4.5/lightly/active_learning/scorers/detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/scorers/keypoint_detection.py` & `lightly-1.4.5/lightly/active_learning/scorers/keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/scorers/semantic_segmentation.py` & `lightly-1.4.5/lightly/active_learning/scorers/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/utils/bounding_box.py` & `lightly-1.4.5/lightly/active_learning/utils/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/utils/keypoint_predictions.py` & `lightly-1.4.5/lightly/active_learning/utils/keypoint_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/active_learning/utils/object_detection_output.py` & `lightly-1.4.5/lightly/active_learning/utils/object_detection_output.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/__init__.py` & `lightly-1.4.5/lightly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_artifacts.py` & `lightly-1.4.5/lightly/api/api_workflow_artifacts.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_client.py` & `lightly-1.4.5/lightly/api/api_workflow_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_collaboration.py` & `lightly-1.4.5/lightly/api/api_workflow_collaboration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_compute_worker.py` & `lightly-1.4.5/lightly/api/api_workflow_compute_worker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_datasets.py` & `lightly-1.4.5/lightly/api/api_workflow_datasets.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_datasources.py` & `lightly-1.4.5/lightly/api/api_workflow_datasources.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,16 @@
 
     def download_raw_predictions(
         self,
         task_name: str,
         from_: int = 0,
         to: Optional[int] = None,
         relevant_filenames_file_name: Optional[str] = None,
+        run_id: Optional[str] = None,
+        relevant_filenames_artifact_id: Optional[str] = None,
         use_redirected_read_url: Optional[bool] = False,
         progress_bar: Optional[tqdm.tqdm] = None,
     ) -> List[Tuple[str, str]]:
         """Downloads all prediction filenames and read urls from the datasource between `from_` and `to`.
 
         Samples which have timestamp == `from_` or timestamp == `to` will also be included.
 
@@ -158,42 +160,69 @@
             from_:
                 Unix timestamp from which on samples are downloaded.
             to:
                 Unix timestamp up to and including which samples are downloaded.
             relevant_filenames_file_name:
                 The path to the relevant filenames text file in the cloud bucket.
                 The path is relative to the datasource root.
+            run_id:
+                Run ID. Should be given along with `relevant_filenames_artifact_id` to
+                download relevant files only.
+            relevant_filenames_artifact_id:
+                ID of the relevant filename artifact. Should be given along with
+                `run_id` to download relevant files only. Note that this is different
+                from `relevant_filenames_file_name`.
             use_redirected_read_url:
                 By default this is set to false unless a S3DelegatedAccess is configured in which
                 case its always true and this param has no effect.
                 When true this will return RedirectedReadUrls instead of ReadUrls meaning that
                 returned URLs allow for unlimited access to the file
             progress_bar:
                 Tqdm progress bar to show how many prediction files have already been
                 retrieved.
 
         Returns:
            A list of (filename, url) tuples, where each tuple represents a sample
 
         """
+        if run_id is not None and relevant_filenames_artifact_id is None:
+            raise ValueError(
+                "'relevant_filenames_artifact_id' should not be `None` when 'run_id' "
+                "is specified."
+            )
+        if run_id is None and relevant_filenames_artifact_id is not None:
+            raise ValueError(
+                "'run_id' should not be `None` when 'relevant_filenames_artifact_id' "
+                "is specified."
+            )
+        relevant_filenames_kwargs = {}
+        if run_id is not None and relevant_filenames_artifact_id is not None:
+            relevant_filenames_kwargs["relevant_filenames_run_id"] = run_id
+            relevant_filenames_kwargs[
+                "relevant_filenames_artifact_id"
+            ] = relevant_filenames_artifact_id
+
         samples = self._download_raw_files(
             download_function=self._datasources_api.get_list_of_raw_samples_predictions_from_datasource_by_dataset_id,
             from_=from_,
             to=to,
             relevant_filenames_file_name=relevant_filenames_file_name,
             use_redirected_read_url=use_redirected_read_url,
             task_name=task_name,
             progress_bar=progress_bar,
+            **relevant_filenames_kwargs,
         )
         return samples
 
     def download_raw_metadata(
         self,
         from_: int = 0,
         to: Optional[int] = None,
+        run_id: Optional[str] = None,
+        relevant_filenames_artifact_id: Optional[str] = None,
         relevant_filenames_file_name: Optional[str] = None,
         use_redirected_read_url: Optional[bool] = False,
         progress_bar: Optional[tqdm.tqdm] = None,
     ) -> List[Tuple[str, str]]:
         """Downloads all metadata filenames and read urls from the datasource between `from_` and `to`.
 
         Samples which have timestamp == `from_` or timestamp == `to` will also be included.
@@ -202,34 +231,59 @@
             from_:
                 Unix timestamp from which on samples are downloaded.
             to:
                 Unix timestamp up to and including which samples are downloaded.
             relevant_filenames_file_name:
                 The path to the relevant filenames text file in the cloud bucket.
                 The path is relative to the datasource root.
+            run_id:
+                Run ID. Should be given along with `relevant_filenames_artifact_id` to
+                download relevant files only.
+            relevant_filenames_artifact_id:
+                ID of the relevant filename artifact. Should be given along with
+                `run_id` to download relevant files only. Note that this is different
+                from `relevant_filenames_file_name`.
             use_redirected_read_url:
                 By default this is set to false unless a S3DelegatedAccess is configured in which
                 case its always true and this param has no effect.
                 When true this will return RedirectedReadUrls instead of ReadUrls meaning that
                 returned URLs allow for unlimited access to the file
             progress_bar:
                 Tqdm progress bar to show how many metadata files have already been
                 retrieved.
 
         Returns:
            A list of (filename, url) tuples, where each tuple represents a sample
 
         """
+        if run_id is not None and relevant_filenames_artifact_id is None:
+            raise ValueError(
+                "'relevant_filenames_artifact_id' should not be `None` when 'run_id' "
+                "is specified."
+            )
+        if run_id is None and relevant_filenames_artifact_id is not None:
+            raise ValueError(
+                "'run_id' should not be `None` when 'relevant_filenames_artifact_id' "
+                "is specified."
+            )
+        relevant_filenames_kwargs = {}
+        if run_id is not None and relevant_filenames_artifact_id is not None:
+            relevant_filenames_kwargs["relevant_filenames_run_id"] = run_id
+            relevant_filenames_kwargs[
+                "relevant_filenames_artifact_id"
+            ] = relevant_filenames_artifact_id
+
         samples = self._download_raw_files(
             self._datasources_api.get_list_of_raw_samples_metadata_from_datasource_by_dataset_id,
             from_=from_,
             to=to,
             relevant_filenames_file_name=relevant_filenames_file_name,
             use_redirected_read_url=use_redirected_read_url,
             progress_bar=progress_bar,
+            **relevant_filenames_kwargs,
         )
         return samples
 
     def download_new_raw_samples(
         self,
         use_redirected_read_url: Optional[bool] = False,
     ) -> List[Tuple[str, str]]:
```

### Comparing `lightly-1.4.4/lightly/api/api_workflow_download_dataset.py` & `lightly-1.4.5/lightly/api/api_workflow_download_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_export.py` & `lightly-1.4.5/lightly/api/api_workflow_export.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_predictions.py` & `lightly-1.4.5/lightly/api/api_workflow_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_selection.py` & `lightly-1.4.5/lightly/api/api_workflow_selection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_tags.py` & `lightly-1.4.5/lightly/api/api_workflow_tags.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_upload_dataset.py` & `lightly-1.4.5/lightly/api/api_workflow_upload_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_upload_embeddings.py` & `lightly-1.4.5/lightly/api/api_workflow_upload_embeddings.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/api_workflow_upload_metadata.py` & `lightly-1.4.5/lightly/api/api_workflow_upload_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/bitmask.py` & `lightly-1.4.5/lightly/api/bitmask.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/download.py` & `lightly-1.4.5/lightly/api/download.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/patch.py` & `lightly-1.4.5/lightly/api/patch.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/prediction_singletons.py` & `lightly-1.4.5/lightly/api/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/swagger_api_client.py` & `lightly-1.4.5/lightly/api/swagger_api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/swagger_rest_client.py` & `lightly-1.4.5/lightly/api/swagger_rest_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/utils.py` & `lightly-1.4.5/lightly/api/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/api/version_checking.py` & `lightly-1.4.5/lightly/api/version_checking.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/_cli_simclr.py` & `lightly-1.4.5/lightly/cli/_cli_simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/_helpers.py` & `lightly-1.4.5/lightly/cli/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/config/config.yaml` & `lightly-1.4.5/lightly/cli/config/config.yaml`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/crop_cli.py` & `lightly-1.4.5/lightly/cli/crop_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/download_cli.py` & `lightly-1.4.5/lightly/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/embed_cli.py` & `lightly-1.4.5/lightly/cli/embed_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/lightly_cli.py` & `lightly-1.4.5/lightly/cli/lightly_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/train_cli.py` & `lightly-1.4.5/lightly/cli/train_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/upload_cli.py` & `lightly-1.4.5/lightly/cli/upload_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/cli/version_cli.py` & `lightly-1.4.5/lightly/cli/version_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/core.py` & `lightly-1.4.5/lightly/core.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/__init__.py` & `lightly-1.4.5/lightly/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/_helpers.py` & `lightly-1.4.5/lightly/data/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/_image.py` & `lightly-1.4.5/lightly/data/_image.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/_image_loaders.py` & `lightly-1.4.5/lightly/data/_image_loaders.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/_utils.py` & `lightly-1.4.5/lightly/data/_utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/_video.py` & `lightly-1.4.5/lightly/data/_video.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/collate.py` & `lightly-1.4.5/lightly/data/collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/dataset.py` & `lightly-1.4.5/lightly/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/lightly_subset.py` & `lightly-1.4.5/lightly/data/lightly_subset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/data/multi_view_collate.py` & `lightly-1.4.5/lightly/data/multi_view_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/embedding/_base.py` & `lightly-1.4.5/lightly/embedding/_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/embedding/callbacks.py` & `lightly-1.4.5/lightly/embedding/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/embedding/embedding.py` & `lightly-1.4.5/lightly/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/__init__.py` & `lightly-1.4.5/lightly/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/barlow_twins_loss.py` & `lightly-1.4.5/lightly/loss/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/dcl_loss.py` & `lightly-1.4.5/lightly/loss/dcl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/dino_loss.py` & `lightly-1.4.5/lightly/loss/dino_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/hypersphere_loss.py` & `lightly-1.4.5/lightly/loss/hypersphere_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/memory_bank.py` & `lightly-1.4.5/lightly/loss/memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/msn_loss.py` & `lightly-1.4.5/lightly/loss/msn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/negative_cosine_similarity.py` & `lightly-1.4.5/lightly/loss/negative_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/ntx_ent_loss.py` & `lightly-1.4.5/lightly/loss/ntx_ent_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/pmsn_loss.py` & `lightly-1.4.5/lightly/loss/pmsn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/regularizer/co2.py` & `lightly-1.4.5/lightly/loss/regularizer/co2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/swav_loss.py` & `lightly-1.4.5/lightly/loss/swav_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/sym_neg_cos_sim_loss.py` & `lightly-1.4.5/lightly/loss/sym_neg_cos_sim_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/tico_loss.py` & `lightly-1.4.5/lightly/loss/tico_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/vicreg_loss.py` & `lightly-1.4.5/lightly/loss/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/loss/vicregl_loss.py` & `lightly-1.4.5/lightly/loss/vicregl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/__init__.py` & `lightly-1.4.5/lightly/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/_momentum.py` & `lightly-1.4.5/lightly/models/_momentum.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/barlowtwins.py` & `lightly-1.4.5/lightly/models/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/batchnorm.py` & `lightly-1.4.5/lightly/models/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/byol.py` & `lightly-1.4.5/lightly/models/byol.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/moco.py` & `lightly-1.4.5/lightly/models/moco.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/modules/__init__.py` & `lightly-1.4.5/lightly/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/modules/heads.py` & `lightly-1.4.5/lightly/models/modules/heads.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/modules/masked_autoencoder.py` & `lightly-1.4.5/lightly/models/modules/masked_autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/modules/nn_memory_bank.py` & `lightly-1.4.5/lightly/models/modules/nn_memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/nnclr.py` & `lightly-1.4.5/lightly/models/nnclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/resnet.py` & `lightly-1.4.5/lightly/models/resnet.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/simclr.py` & `lightly-1.4.5/lightly/models/simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/simsiam.py` & `lightly-1.4.5/lightly/models/simsiam.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/models/utils.py` & `lightly-1.4.5/lightly/models/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """ Utils for working with SSL models """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 import math
 import warnings
-from typing import Optional, Tuple, Union
+from typing import Iterable, List, Optional, Tuple, Union
 
-import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn as nn
+from torch.nn import Module
+from torch.nn.modules.batchnorm import _BatchNorm
+from torch.nn.parameter import Parameter
 
 
 @torch.no_grad()
 def batch_shuffle(
     batch: torch.Tensor, distributed: bool = False
 ) -> Tuple[torch.Tensor, torch.Tensor]:
     """Randomly shuffles all tensors in the batch.
@@ -525,7 +527,43 @@
     filtered_candidate_maps = torch.gather(
         selected_candidate_maps,
         1,
         min_indices.unsqueeze(-1).expand(-1, -1, feature_dimension),
     )  # [bsz, num_matches, feature_dimension]
 
     return filtered_input_maps, filtered_candidate_maps
+
+
+def get_weight_decay_parameters(
+    modules: Iterable[Module],
+    decay_batch_norm: bool = False,
+    decay_bias: bool = False,
+) -> Tuple[List[Parameter], List[Parameter]]:
+    """Returns all parameters of the modules that should be decayed and not decayed.
+
+    Args:
+        modules:
+            List of modules to get the parameters from.
+        no_batch_norm:
+            If True, batch norm parameters are decayed.
+        no_bias:
+            If True, bias parameters are decayed.
+
+    Returns:
+        (params, params_no_weight_decay) tuple.
+    """
+    params = []
+    params_no_weight_decay = []
+    for module in modules:
+        for mod in module.modules():
+            if isinstance(mod, _BatchNorm):
+                if not decay_batch_norm:
+                    params_no_weight_decay.extend(mod.parameters(recurse=False))
+                else:
+                    params.extend(mod.parameters(recurse=False))
+            else:
+                for name, param in mod.named_parameters(recurse=False):
+                    if not decay_bias and name.endswith("bias"):
+                        params_no_weight_decay.append(param)
+                    else:
+                        params.append(param)
+    return params, params_no_weight_decay
```

### Comparing `lightly-1.4.4/lightly/models/zoo.py` & `lightly-1.4.5/lightly/models/zoo.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/__init__.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from lightly.openapi_generated.swagger_client.models.category_name import CategoryName
 from lightly.openapi_generated.swagger_client.models.configuration_data import ConfigurationData
 from lightly.openapi_generated.swagger_client.models.configuration_entry import ConfigurationEntry
 from lightly.openapi_generated.swagger_client.models.configuration_set_request import ConfigurationSetRequest
 from lightly.openapi_generated.swagger_client.models.configuration_value_data_type import ConfigurationValueDataType
 from lightly.openapi_generated.swagger_client.models.create_docker_worker_registry_entry_request import CreateDockerWorkerRegistryEntryRequest
 from lightly.openapi_generated.swagger_client.models.create_entity_response import CreateEntityResponse
+from lightly.openapi_generated.swagger_client.models.create_sample_with_write_urls_response import CreateSampleWithWriteUrlsResponse
 from lightly.openapi_generated.swagger_client.models.creator import Creator
 from lightly.openapi_generated.swagger_client.models.crop_data import CropData
 from lightly.openapi_generated.swagger_client.models.custom_sample_meta_data import CustomSampleMetaData
 from lightly.openapi_generated.swagger_client.models.dataset_create_request import DatasetCreateRequest
 from lightly.openapi_generated.swagger_client.models.dataset_creator import DatasetCreator
 from lightly.openapi_generated.swagger_client.models.dataset_data import DatasetData
 from lightly.openapi_generated.swagger_client.models.dataset_data_enriched import DatasetDataEnriched
```

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/__init__.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/collaboration_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/collaboration_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/datasets_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/datasources_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasources_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,14 +552,16 @@
         :param async_req bool
         :param MongoObjectID dataset_id: ObjectId of the dataset (required)
         :param Timestamp _from: Unix timestamp, only samples with a creation date after `from` will be returned. This parameter is ignored if `cursor` is specified. 
         :param Timestamp to: Unix timestamp, only samples with a creation date before `to` will be returned. This parameter is ignored if `cursor` is specified. 
         :param str cursor: Cursor from previous request, encodes `from` and `to` parameters. Specify to continue reading samples from the list. 
         :param bool use_redirected_read_url: By default this is set to false unless a S3DelegatedAccess is configured in which case its always true and this param has no effect. When true this will return RedirectedReadUrls instead of ReadUrls meaning that  returned URLs allow for unlimited access to the file 
         :param str relevant_filenames_file_name: The name of the file within your datasource which contains a list of relevant filenames to list. See https://docs.lightly.ai/docker/getting_started/first_steps.html#specify-relevant-files for more details  
+        :param MongoObjectID relevant_filenames_run_id: The run id of the run which generated an artifact to be used as the relevant filenames file. (see DatasourceRelevantFilenamesArtifactIdParam) 
+        :param MongoObjectID relevant_filenames_artifact_id: The artifact id of the run provided by DatasourceRelevantFilenamesRunIdParam to be used as the relevant filenames file. 
         :return: DatasourceRawSamplesMetadataData
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_list_of_raw_samples_metadata_from_datasource_by_dataset_id_with_http_info(dataset_id, **kwargs)  # noqa: E501
@@ -579,20 +581,22 @@
         :param async_req bool
         :param MongoObjectID dataset_id: ObjectId of the dataset (required)
         :param Timestamp _from: Unix timestamp, only samples with a creation date after `from` will be returned. This parameter is ignored if `cursor` is specified. 
         :param Timestamp to: Unix timestamp, only samples with a creation date before `to` will be returned. This parameter is ignored if `cursor` is specified. 
         :param str cursor: Cursor from previous request, encodes `from` and `to` parameters. Specify to continue reading samples from the list. 
         :param bool use_redirected_read_url: By default this is set to false unless a S3DelegatedAccess is configured in which case its always true and this param has no effect. When true this will return RedirectedReadUrls instead of ReadUrls meaning that  returned URLs allow for unlimited access to the file 
         :param str relevant_filenames_file_name: The name of the file within your datasource which contains a list of relevant filenames to list. See https://docs.lightly.ai/docker/getting_started/first_steps.html#specify-relevant-files for more details  
+        :param MongoObjectID relevant_filenames_run_id: The run id of the run which generated an artifact to be used as the relevant filenames file. (see DatasourceRelevantFilenamesArtifactIdParam) 
+        :param MongoObjectID relevant_filenames_artifact_id: The artifact id of the run provided by DatasourceRelevantFilenamesRunIdParam to be used as the relevant filenames file. 
         :return: DatasourceRawSamplesMetadataData
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['dataset_id', '_from', 'to', 'cursor', 'use_redirected_read_url', 'relevant_filenames_file_name']  # noqa: E501
+        all_params = ['dataset_id', '_from', 'to', 'cursor', 'use_redirected_read_url', 'relevant_filenames_file_name', 'relevant_filenames_run_id', 'relevant_filenames_artifact_id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -621,14 +625,18 @@
             query_params.append(('to', params['to']))  # noqa: E501
         if 'cursor' in params:
             query_params.append(('cursor', params['cursor']))  # noqa: E501
         if 'use_redirected_read_url' in params:
             query_params.append(('useRedirectedReadUrl', params['use_redirected_read_url']))  # noqa: E501
         if 'relevant_filenames_file_name' in params:
             query_params.append(('relevantFilenamesFileName', params['relevant_filenames_file_name']))  # noqa: E501
+        if 'relevant_filenames_run_id' in params:
+            query_params.append(('relevantFilenamesRunId', params['relevant_filenames_run_id']))  # noqa: E501
+        if 'relevant_filenames_artifact_id' in params:
+            query_params.append(('relevantFilenamesArtifactId', params['relevant_filenames_artifact_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -668,14 +676,16 @@
         :param MongoObjectID dataset_id: ObjectId of the dataset (required)
         :param TaskName task_name: The prediction task name for which one wants to list the predictions (required)
         :param Timestamp _from: Unix timestamp, only samples with a creation date after `from` will be returned. This parameter is ignored if `cursor` is specified. 
         :param Timestamp to: Unix timestamp, only samples with a creation date before `to` will be returned. This parameter is ignored if `cursor` is specified. 
         :param str cursor: Cursor from previous request, encodes `from` and `to` parameters. Specify to continue reading samples from the list. 
         :param bool use_redirected_read_url: By default this is set to false unless a S3DelegatedAccess is configured in which case its always true and this param has no effect. When true this will return RedirectedReadUrls instead of ReadUrls meaning that  returned URLs allow for unlimited access to the file 
         :param str relevant_filenames_file_name: The name of the file within your datasource which contains a list of relevant filenames to list. See https://docs.lightly.ai/docker/getting_started/first_steps.html#specify-relevant-files for more details  
+        :param MongoObjectID relevant_filenames_run_id: The run id of the run which generated an artifact to be used as the relevant filenames file. (see DatasourceRelevantFilenamesArtifactIdParam) 
+        :param MongoObjectID relevant_filenames_artifact_id: The artifact id of the run provided by DatasourceRelevantFilenamesRunIdParam to be used as the relevant filenames file. 
         :return: DatasourceRawSamplesPredictionsData
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_list_of_raw_samples_predictions_from_datasource_by_dataset_id_with_http_info(dataset_id, task_name, **kwargs)  # noqa: E501
@@ -696,20 +706,22 @@
         :param MongoObjectID dataset_id: ObjectId of the dataset (required)
         :param TaskName task_name: The prediction task name for which one wants to list the predictions (required)
         :param Timestamp _from: Unix timestamp, only samples with a creation date after `from` will be returned. This parameter is ignored if `cursor` is specified. 
         :param Timestamp to: Unix timestamp, only samples with a creation date before `to` will be returned. This parameter is ignored if `cursor` is specified. 
         :param str cursor: Cursor from previous request, encodes `from` and `to` parameters. Specify to continue reading samples from the list. 
         :param bool use_redirected_read_url: By default this is set to false unless a S3DelegatedAccess is configured in which case its always true and this param has no effect. When true this will return RedirectedReadUrls instead of ReadUrls meaning that  returned URLs allow for unlimited access to the file 
         :param str relevant_filenames_file_name: The name of the file within your datasource which contains a list of relevant filenames to list. See https://docs.lightly.ai/docker/getting_started/first_steps.html#specify-relevant-files for more details  
+        :param MongoObjectID relevant_filenames_run_id: The run id of the run which generated an artifact to be used as the relevant filenames file. (see DatasourceRelevantFilenamesArtifactIdParam) 
+        :param MongoObjectID relevant_filenames_artifact_id: The artifact id of the run provided by DatasourceRelevantFilenamesRunIdParam to be used as the relevant filenames file. 
         :return: DatasourceRawSamplesPredictionsData
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['dataset_id', 'task_name', '_from', 'to', 'cursor', 'use_redirected_read_url', 'relevant_filenames_file_name']  # noqa: E501
+        all_params = ['dataset_id', 'task_name', '_from', 'to', 'cursor', 'use_redirected_read_url', 'relevant_filenames_file_name', 'relevant_filenames_run_id', 'relevant_filenames_artifact_id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -744,14 +756,18 @@
             query_params.append(('to', params['to']))  # noqa: E501
         if 'cursor' in params:
             query_params.append(('cursor', params['cursor']))  # noqa: E501
         if 'use_redirected_read_url' in params:
             query_params.append(('useRedirectedReadUrl', params['use_redirected_read_url']))  # noqa: E501
         if 'relevant_filenames_file_name' in params:
             query_params.append(('relevantFilenamesFileName', params['relevant_filenames_file_name']))  # noqa: E501
+        if 'relevant_filenames_run_id' in params:
+            query_params.append(('relevantFilenamesRunId', params['relevant_filenames_run_id']))  # noqa: E501
+        if 'relevant_filenames_artifact_id' in params:
+            query_params.append(('relevantFilenamesArtifactId', params['relevant_filenames_artifact_id']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/docker_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/docker_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/embeddings_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/jobs_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/mappings_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/mappings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/predictions_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/predictions_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/quota_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/quota_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/samples_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samples_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,121 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def create_sample_with_write_urls_by_dataset_id(self, body, dataset_id, **kwargs):  # noqa: E501
+        """create_sample_with_write_urls_by_dataset_id  # noqa: E501
+
+        Create a sample and immediately receive write URLs (full image and thumbnail) to upload images  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_sample_with_write_urls_by_dataset_id(body, dataset_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param SampleCreateRequest body: (required)
+        :param MongoObjectID dataset_id: ObjectId of the dataset (required)
+        :return: CreateSampleWithWriteUrlsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.create_sample_with_write_urls_by_dataset_id_with_http_info(body, dataset_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.create_sample_with_write_urls_by_dataset_id_with_http_info(body, dataset_id, **kwargs)  # noqa: E501
+            return data
+
+    def create_sample_with_write_urls_by_dataset_id_with_http_info(self, body, dataset_id, **kwargs):  # noqa: E501
+        """create_sample_with_write_urls_by_dataset_id  # noqa: E501
+
+        Create a sample and immediately receive write URLs (full image and thumbnail) to upload images  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_sample_with_write_urls_by_dataset_id_with_http_info(body, dataset_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param SampleCreateRequest body: (required)
+        :param MongoObjectID dataset_id: ObjectId of the dataset (required)
+        :return: CreateSampleWithWriteUrlsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body', 'dataset_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_sample_with_write_urls_by_dataset_id" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if self.api_client.client_side_validation and ('body' not in params or
+                                                       params['body'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `create_sample_with_write_urls_by_dataset_id`")  # noqa: E501
+        # verify the required parameter 'dataset_id' is set
+        if self.api_client.client_side_validation and ('dataset_id' not in params or
+                                                       params['dataset_id'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `dataset_id` when calling `create_sample_with_write_urls_by_dataset_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'dataset_id' in params:
+            path_params['datasetId'] = params['dataset_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['ApiKeyAuth', 'auth0Bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/datasets/{datasetId}/samples/withWriteUrls', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='CreateSampleWithWriteUrlsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_sample_by_id(self, dataset_id, sample_id, **kwargs):  # noqa: E501
         """get_sample_by_id  # noqa: E501
 
         Get a specific sample of a dataset  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_sample_by_id(dataset_id, sample_id, async_req=True)
```

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/samplings_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samplings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/scores_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/scores_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/tags_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/teams_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api/versioning_api.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/versioning_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/api_client.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/configuration.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/__init__.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from lightly.openapi_generated.swagger_client.models.category_name import CategoryName
 from lightly.openapi_generated.swagger_client.models.configuration_data import ConfigurationData
 from lightly.openapi_generated.swagger_client.models.configuration_entry import ConfigurationEntry
 from lightly.openapi_generated.swagger_client.models.configuration_set_request import ConfigurationSetRequest
 from lightly.openapi_generated.swagger_client.models.configuration_value_data_type import ConfigurationValueDataType
 from lightly.openapi_generated.swagger_client.models.create_docker_worker_registry_entry_request import CreateDockerWorkerRegistryEntryRequest
 from lightly.openapi_generated.swagger_client.models.create_entity_response import CreateEntityResponse
+from lightly.openapi_generated.swagger_client.models.create_sample_with_write_urls_response import CreateSampleWithWriteUrlsResponse
 from lightly.openapi_generated.swagger_client.models.creator import Creator
 from lightly.openapi_generated.swagger_client.models.crop_data import CropData
 from lightly.openapi_generated.swagger_client.models.custom_sample_meta_data import CustomSampleMetaData
 from lightly.openapi_generated.swagger_client.models.dataset_create_request import DatasetCreateRequest
 from lightly.openapi_generated.swagger_client.models.dataset_creator import DatasetCreator
 from lightly.openapi_generated.swagger_client.models.dataset_data import DatasetData
 from lightly.openapi_generated.swagger_client.models.dataset_data_enriched import DatasetDataEnriched
```

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/access_role.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/access_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/active_learning_scores.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_scores.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/api_error_code.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_code.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/api_error_response.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/async_task_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/async_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/bounding_box.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/category_id.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/category_name.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_entry.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_set_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_set_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/create_entity_response.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_entity_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/creator.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/crop_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/crop_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_creator.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_name.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_name_query.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name_query.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dataset_update_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_base.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_local.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_local.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_purpose.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_purpose.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_license_information.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_license_information.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_state.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_task_description.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_task_description.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_user_stats.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_user_stats.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         'checkpoint': 'str',
         'corruptness_check': 'DockerWorkerConfigV3DockerCorruptnessCheck',
         'datasource': 'DockerWorkerConfigV3DockerDatasource',
         'embeddings': 'str',
         'enable_training': 'bool',
         'training': 'DockerWorkerConfigV3DockerTraining',
         'normalize_embeddings': 'bool',
+        'num_processes': 'int',
+        'num_threads': 'int',
         'output_image_format': 'str',
         'pretagging': 'bool',
         'pretagging_upload': 'bool',
         'relevant_filenames_file': 'str',
         'selected_sequence_length': 'int',
         'upload_report': 'bool'
     }
@@ -52,35 +54,39 @@
         'checkpoint': 'checkpoint',
         'corruptness_check': 'corruptnessCheck',
         'datasource': 'datasource',
         'embeddings': 'embeddings',
         'enable_training': 'enableTraining',
         'training': 'training',
         'normalize_embeddings': 'normalizeEmbeddings',
+        'num_processes': 'numProcesses',
+        'num_threads': 'numThreads',
         'output_image_format': 'outputImageFormat',
         'pretagging': 'pretagging',
         'pretagging_upload': 'pretaggingUpload',
         'relevant_filenames_file': 'relevantFilenamesFile',
         'selected_sequence_length': 'selectedSequenceLength',
         'upload_report': 'uploadReport'
     }
 
-    def __init__(self, checkpoint=None, corruptness_check=None, datasource=None, embeddings=None, enable_training=None, training=None, normalize_embeddings=None, output_image_format=None, pretagging=None, pretagging_upload=None, relevant_filenames_file=None, selected_sequence_length=None, upload_report=None, _configuration=None):  # noqa: E501
+    def __init__(self, checkpoint=None, corruptness_check=None, datasource=None, embeddings=None, enable_training=None, training=None, normalize_embeddings=None, num_processes=None, num_threads=None, output_image_format=None, pretagging=None, pretagging_upload=None, relevant_filenames_file=None, selected_sequence_length=None, upload_report=None, _configuration=None):  # noqa: E501
         """DockerWorkerConfigV3Docker - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._checkpoint = None
         self._corruptness_check = None
         self._datasource = None
         self._embeddings = None
         self._enable_training = None
         self._training = None
         self._normalize_embeddings = None
+        self._num_processes = None
+        self._num_threads = None
         self._output_image_format = None
         self._pretagging = None
         self._pretagging_upload = None
         self._relevant_filenames_file = None
         self._selected_sequence_length = None
         self._upload_report = None
         self.discriminator = None
@@ -95,14 +101,18 @@
             self.embeddings = embeddings
         if enable_training is not None:
             self.enable_training = enable_training
         if training is not None:
             self.training = training
         if normalize_embeddings is not None:
             self.normalize_embeddings = normalize_embeddings
+        if num_processes is not None:
+            self.num_processes = num_processes
+        if num_threads is not None:
+            self.num_threads = num_threads
         if output_image_format is not None:
             self.output_image_format = output_image_format
         if pretagging is not None:
             self.pretagging = pretagging
         if pretagging_upload is not None:
             self.pretagging_upload = pretagging_upload
         if relevant_filenames_file is not None:
@@ -256,14 +266,56 @@
         :param normalize_embeddings: The normalize_embeddings of this DockerWorkerConfigV3Docker.  # noqa: E501
         :type: bool
         """
 
         self._normalize_embeddings = normalize_embeddings
 
     @property
+    def num_processes(self):
+        """Gets the num_processes of this DockerWorkerConfigV3Docker.  # noqa: E501
+
+
+        :return: The num_processes of this DockerWorkerConfigV3Docker.  # noqa: E501
+        :rtype: int
+        """
+        return self._num_processes
+
+    @num_processes.setter
+    def num_processes(self, num_processes):
+        """Sets the num_processes of this DockerWorkerConfigV3Docker.
+
+
+        :param num_processes: The num_processes of this DockerWorkerConfigV3Docker.  # noqa: E501
+        :type: int
+        """
+
+        self._num_processes = num_processes
+
+    @property
+    def num_threads(self):
+        """Gets the num_threads of this DockerWorkerConfigV3Docker.  # noqa: E501
+
+
+        :return: The num_threads of this DockerWorkerConfigV3Docker.  # noqa: E501
+        :rtype: int
+        """
+        return self._num_threads
+
+    @num_threads.setter
+    def num_threads(self, num_threads):
+        """Sets the num_threads of this DockerWorkerConfigV3Docker.
+
+
+        :param num_threads: The num_threads of this DockerWorkerConfigV3Docker.  # noqa: E501
+        :type: int
+        """
+
+        self._num_threads = num_threads
+
+    @property
     def output_image_format(self):
         """Gets the output_image_format of this DockerWorkerConfigV3Docker.  # noqa: E501
 
 
         :return: The output_image_format of this DockerWorkerConfigV3Docker.  # noqa: E501
         :rtype: str
         """
```

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_name.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_state.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/docker_worker_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding2d_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/embedding_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/file_name_format.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_name_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/file_output_format.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_output_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/general_job_result.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/general_job_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/image_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/image_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_result_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_result_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_state.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_data_result.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_meta.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_meta.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/jobs_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/jobs_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_data_row.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_studio_task.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/mongo_object_id.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/mongo_object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/object_id.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/path_safe_name.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/path_safe_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_singletons.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/probabilities.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/probabilities.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/questionnaire_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/questionnaire_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/read_url.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/redirected_read_url.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/redirected_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/s3_region.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_region.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sama_task.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sama_task_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sama_tasks.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_data_modes.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data_modes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_meta_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_sort_by.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_sort_by.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_update_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sample_write_urls.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_write_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_config.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sampling_method.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/score.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/score.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/sector.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sector.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config_entry.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_input_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,49 +33,49 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'MongoObjectID',
         'owner': 'str',
         'access_type': 'SharedAccessType',
         'users': 'list[str]',
-        'organizations': 'list[str]',
+        'teams': 'list[str]',
         'created_at': 'Timestamp',
         'last_modified_at': 'Timestamp'
     }
 
     attribute_map = {
         'id': 'id',
         'owner': 'owner',
         'access_type': 'accessType',
         'users': 'users',
-        'organizations': 'organizations',
+        'teams': 'teams',
         'created_at': 'createdAt',
         'last_modified_at': 'lastModifiedAt'
     }
 
-    def __init__(self, id=None, owner=None, access_type=None, users=None, organizations=None, created_at=None, last_modified_at=None, _configuration=None):  # noqa: E501
+    def __init__(self, id=None, owner=None, access_type=None, users=None, teams=None, created_at=None, last_modified_at=None, _configuration=None):  # noqa: E501
         """SharedAccessConfigData - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._id = None
         self._owner = None
         self._access_type = None
         self._users = None
-        self._organizations = None
+        self._teams = None
         self._created_at = None
         self._last_modified_at = None
         self.discriminator = None
 
         self.id = id
         self.owner = owner
         self.access_type = access_type
         self.users = users
-        self.organizations = organizations
+        self.teams = teams
         self.created_at = created_at
         self.last_modified_at = last_modified_at
 
     @property
     def id(self):
         """Gets the id of this SharedAccessConfigData.  # noqa: E501
 
@@ -168,37 +168,37 @@
         """
         if self._configuration.client_side_validation and users is None:
             raise ValueError("Invalid value for `users`, must not be `None`")  # noqa: E501
 
         self._users = users
 
     @property
-    def organizations(self):
-        """Gets the organizations of this SharedAccessConfigData.  # noqa: E501
+    def teams(self):
+        """Gets the teams of this SharedAccessConfigData.  # noqa: E501
 
-        List of organizations with access to the dataset  # noqa: E501
+        List of teams with access to the dataset  # noqa: E501
 
-        :return: The organizations of this SharedAccessConfigData.  # noqa: E501
+        :return: The teams of this SharedAccessConfigData.  # noqa: E501
         :rtype: list[str]
         """
-        return self._organizations
+        return self._teams
 
-    @organizations.setter
-    def organizations(self, organizations):
-        """Sets the organizations of this SharedAccessConfigData.
+    @teams.setter
+    def teams(self, teams):
+        """Sets the teams of this SharedAccessConfigData.
 
-        List of organizations with access to the dataset  # noqa: E501
+        List of teams with access to the dataset  # noqa: E501
 
-        :param organizations: The organizations of this SharedAccessConfigData.  # noqa: E501
+        :param teams: The teams of this SharedAccessConfigData.  # noqa: E501
         :type: list[str]
         """
-        if self._configuration.client_side_validation and organizations is None:
-            raise ValueError("Invalid value for `organizations`, must not be `None`")  # noqa: E501
+        if self._configuration.client_side_validation and teams is None:
+            raise ValueError("Invalid value for `teams`, must not be `None`")  # noqa: E501
 
-        self._organizations = organizations
+        self._teams = teams
 
     @property
     def created_at(self):
         """Gets the created_at of this SharedAccessConfigData.  # noqa: E501
 
 
         :return: The created_at of this SharedAccessConfigData.  # noqa: E501
```

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/shared_access_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_change_entry.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_create_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_creator.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_name.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_update_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/task_name.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/task_type.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/team_basic_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/team_role.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/timestamp.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/version_number.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/version_number.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/video_frame_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/video_frame_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/openapi_generated/swagger_client/rest.py` & `lightly-1.4.5/lightly/openapi_generated/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/__init__.py` & `lightly-1.4.5/lightly/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/dino_transform.py` & `lightly-1.4.5/lightly/transforms/dino_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/fast_siam_transform.py` & `lightly-1.4.5/lightly/transforms/fast_siam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/gaussian_blur.py` & `lightly-1.4.5/lightly/transforms/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/image_grid_transform.py` & `lightly-1.4.5/lightly/transforms/image_grid_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/jigsaw.py` & `lightly-1.4.5/lightly/transforms/jigsaw.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/mae_transform.py` & `lightly-1.4.5/lightly/transforms/mae_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/moco_transform.py` & `lightly-1.4.5/lightly/transforms/moco_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/msn_transform.py` & `lightly-1.4.5/lightly/transforms/msn_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/multi_crop_transform.py` & `lightly-1.4.5/lightly/transforms/multi_crop_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/multi_view_transform.py` & `lightly-1.4.5/lightly/transforms/multi_view_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/pirl_transform.py` & `lightly-1.4.5/lightly/transforms/pirl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/random_crop_and_flip_with_grid.py` & `lightly-1.4.5/lightly/transforms/random_crop_and_flip_with_grid.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/rotation.py` & `lightly-1.4.5/lightly/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/simclr_transform.py` & `lightly-1.4.5/lightly/transforms/simclr_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/simsiam_transform.py` & `lightly-1.4.5/lightly/transforms/simsiam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/smog_transform.py` & `lightly-1.4.5/lightly/transforms/smog_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/solarize.py` & `lightly-1.4.5/lightly/transforms/solarize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/swav_transform.py` & `lightly-1.4.5/lightly/transforms/swav_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/vicreg_transform.py` & `lightly-1.4.5/lightly/transforms/vicreg_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/transforms/vicregl_transform.py` & `lightly-1.4.5/lightly/transforms/vicregl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/cropping/crop_image_by_bounding_boxes.py` & `lightly-1.4.5/lightly/utils/cropping/crop_image_by_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/cropping/read_yolo_label_file.py` & `lightly-1.4.5/lightly/utils/cropping/read_yolo_label_file.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/debug.py` & `lightly-1.4.5/lightly/utils/debug.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/dist.py` & `lightly-1.4.5/lightly/utils/dist.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/embeddings_2d.py` & `lightly-1.4.5/lightly/utils/embeddings_2d.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/hipify.py` & `lightly-1.4.5/lightly/utils/hipify.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/io.py` & `lightly-1.4.5/lightly/utils/io.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/reordering.py` & `lightly-1.4.5/lightly/utils/reordering.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly/utils/version_compare.py` & `lightly-1.4.5/lightly/utils/version_compare.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.4/lightly.egg-info/PKG-INFO` & `lightly-1.4.5/lightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.4
+Version: 1.4.5
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.4/lightly.egg-info/SOURCES.txt` & `lightly-1.4.5/lightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 lightly/openapi_generated/swagger_client/models/category_name.py
 lightly/openapi_generated/swagger_client/models/configuration_data.py
 lightly/openapi_generated/swagger_client/models/configuration_entry.py
 lightly/openapi_generated/swagger_client/models/configuration_set_request.py
 lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
 lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
 lightly/openapi_generated/swagger_client/models/create_entity_response.py
+lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
 lightly/openapi_generated/swagger_client/models/creator.py
 lightly/openapi_generated/swagger_client/models/crop_data.py
 lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
 lightly/openapi_generated/swagger_client/models/dataset_create_request.py
 lightly/openapi_generated/swagger_client/models/dataset_creator.py
 lightly/openapi_generated/swagger_client/models/dataset_data.py
 lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
@@ -367,18 +368,18 @@
 lightly/transforms/smog_transform.py
 lightly/transforms/solarize.py
 lightly/transforms/swav_transform.py
 lightly/transforms/utils.py
 lightly/transforms/vicreg_transform.py
 lightly/transforms/vicregl_transform.py
 lightly/utils/__init__.py
-lightly/utils/benchmarking.py
 lightly/utils/debug.py
 lightly/utils/dist.py
 lightly/utils/embeddings_2d.py
 lightly/utils/hipify.py
 lightly/utils/io.py
+lightly/utils/lars.py
 lightly/utils/reordering.py
 lightly/utils/scheduler.py
 lightly/utils/version_compare.py
 lightly/utils/cropping/crop_image_by_bounding_boxes.py
 lightly/utils/cropping/read_yolo_label_file.py
```

### Comparing `lightly-1.4.4/lightly.egg-info/requires.txt` & `lightly-1.4.5/lightly.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 torch
 torchvision
 pytorch_lightning>=1.0.4
 
 [all]
 tox
 sphinx
+pylint
 pytest
 pytest-forked
 pytest-xdist
 pytest-mock
 responses
 docutils<=0.16
 sphinx-copybutton
@@ -37,14 +38,15 @@
 isort==5.11.5
 torchvision>=0.8.0
 av>=8.0.2
 
 [dev]
 tox
 sphinx
+pylint
 pytest
 pytest-forked
 pytest-xdist
 pytest-mock
 responses
 docutils<=0.16
 sphinx-copybutton
```

### Comparing `lightly-1.4.4/setup.py` & `lightly-1.4.5/setup.py`

 * *Files identical despite different names*

