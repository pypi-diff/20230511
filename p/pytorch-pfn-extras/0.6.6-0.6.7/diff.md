# Comparing `tmp/pytorch-pfn-extras-0.6.6.tar.gz` & `tmp/pytorch-pfn-extras-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-pfn-extras-0.6.6.tar", last modified: Thu Apr  6 09:18:57 2023, max compression
+gzip compressed data, was "pytorch-pfn-extras-0.6.7.tar", last modified: Thu May 11 07:42:00 2023, max compression
```

## Comparing `pytorch-pfn-extras-0.6.6.tar` & `pytorch-pfn-extras-0.6.7.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1068 2021-03-09 06:27:52.000000 pytorch-pfn-extras-0.6.6/LICENSE
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      337 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/PKG-INFO
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2354 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/README.md
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      294 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pyproject.toml
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1327 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/__init__.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/_cupy/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      410 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/_cupy/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       24 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/_cupy/_cupy_stub.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5181 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/_tensor.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      259 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/_torch_version.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       22 2023-04-06 09:18:27.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/_version.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     9286 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/config.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1128 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/config_types.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/cuda/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      226 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/cuda/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2159 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/cuda/_allocator.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataloaders/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      130 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataloaders/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       84 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataloaders/dataloader.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1081 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataloaders/utils.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      246 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1896 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/shared_dataset.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      550 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1058 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_asmode.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3901 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_concat.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2150 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_join.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2071 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_slice.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    10171 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_transform.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2677 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_utils.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      809 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_with_converter.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1735 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5345 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/from_data.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    11172 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      302 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1688 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/_dataset_util.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2343 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2518 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/_initialize.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8371 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/engine.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      401 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3917 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/_code_block.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    16860 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/_handler.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    19078 2023-04-06 09:09:10.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/_logic.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1712 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/logging.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      747 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/__init__.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4622 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/ensure_shape.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3928 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/extended_sequential.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8081 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3109 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2139 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy_conv.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1355 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy_linear.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/parallel/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       87 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/parallel/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    13350 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/parallel/distributed.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.963830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      989 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4392 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_as_output.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1021 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_constants.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      951 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_globals.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3568 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_grad.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      659 2023-03-06 02:09:36.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_helper.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    21962 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_lax.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14777 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/annotate.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    17459 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/export_testcase.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1231 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/load.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.963830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/pfto_exporter/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       60 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/pfto_exporter/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    42905 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/pfto_exporter/export.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3470 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/strip_large_tensor.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1129 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/symbolic_registry.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4784 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/unstrip_tensor.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.963830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/profiler/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      360 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/profiler/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2963 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/profiler/_record.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    11611 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/profiler/_time_summary.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/py.typed
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    15212 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/reporting.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.963830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      267 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1739 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_autocast.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      380 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_map.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      846 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_registry.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    17535 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_runtime.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2572 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_to.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      504 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/torchscript.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.963830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1026 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     6564 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_evaluator.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1531 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_manager_protocol.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14943 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_trainer.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      458 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_transform_model.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2929 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_trigger_util.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      716 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_util.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    10472 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extension.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2520 2023-03-06 02:09:36.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    19200 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/_snapshot.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4490 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/best_value.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    17521 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/evaluator.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1393 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/fail_on_non_number.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    10517 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/log_report.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2579 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/lr_scheduler.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3666 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/micro_average.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     7484 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/parameter_statistics.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8454 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/plot_report.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     6878 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/print_report.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2167 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/print_report_notebook.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     6041 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/profile_report.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4062 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/progress_bar.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5494 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14630 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/slack.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       81 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/snapshot_writers.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4372 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/util.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2023 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/value_observation.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    15270 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    27923 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/manager.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1146 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/metrics.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      493 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/trigger.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      772 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5064 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2876 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/interval_trigger.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2399 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5041 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1654 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/once_trigger.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      965 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/time_trigger.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/utils/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      110 2023-04-03 06:31:42.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/utils/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2022-03-04 05:54:25.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/utils/_is_notebook.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2015 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/utils/checkpoint.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    28023 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/utils/comparer.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      689 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3068 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_parallel_writer.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5454 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_queue_writer.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1591 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_simple_writer.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2828 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_tensorboard_writer.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    12856 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_writer_base.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.959830 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras.egg-info/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      337 2023-04-06 09:18:57.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras.egg-info/PKG-INFO
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8076 2023-04-06 09:18:57.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        1 2023-04-06 09:18:57.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       98 2023-04-06 09:18:57.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras.egg-info/requires.txt
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       19 2023-04-06 09:18:57.000000 pytorch-pfn-extras-0.6.6/pytorch_pfn_extras.egg-info/top_level.txt
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      709 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/setup.cfg
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      802 2022-12-27 05:10:31.000000 pytorch-pfn-extras-0.6.6/setup.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.955830 pytorch-pfn-extras-0.6.6/tests/
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/__init__.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/cuda_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/cuda_tests/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2869 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/cuda_tests/test_allocator.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataloader_test/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataloader_test/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1147 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataloader_test/test_dataloader.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.967830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/__init__.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1288 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/dummy_dataset.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1104 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_asmode.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3022 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_concat.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      650 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_delegate_dataset.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    11731 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_from_data.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2972 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_join.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     7949 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_slice.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2997 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_tabular_dataset.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     7563 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_transform.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1125 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_converter.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      986 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_torch_dataloader.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      863 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/test_shared_dataset.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/__init__.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8094 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_extended_sequential.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5685 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      963 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_batchnorm.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      926 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_conv.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      405 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_linear.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     9362 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/test_distributed.py
-drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-04-06 09:18:57.971830 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/profiler_tests/
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/profiler_tests/__init__.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2816 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/profiler_tests/test_time_summary.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     9794 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_config.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3386 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_config_types.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    19653 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_handler.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      695 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_logging.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14959 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_reporter.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3002 2023-01-26 08:06:57.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_tensor.py
--rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      615 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_writing.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.567586 pytorch-pfn-extras-0.6.7/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1068 2021-03-09 06:27:52.000000 pytorch-pfn-extras-0.6.7/LICENSE
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      318 2023-05-11 07:42:00.567586 pytorch-pfn-extras-0.6.7/PKG-INFO
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2354 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/README.md
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      294 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pyproject.toml
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1327 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/__init__.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/_cupy/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      410 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/_cupy/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       24 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/_cupy/_cupy_stub.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5181 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/_tensor.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      259 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/_torch_version.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       22 2023-05-11 07:41:55.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/_version.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     9286 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/config.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1128 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/config_types.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/cuda/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      226 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/cuda/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2159 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/cuda/_allocator.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataloaders/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      130 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataloaders/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       84 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataloaders/dataloader.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1081 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataloaders/utils.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      246 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1896 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/shared_dataset.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      550 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1058 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_asmode.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3901 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_concat.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2150 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_join.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2071 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_slice.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    10171 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_transform.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2677 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_utils.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      809 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_with_converter.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1735 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5345 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/from_data.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    11172 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      302 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1688 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/_dataset_util.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2343 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2518 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/_initialize.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8371 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/engine.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      401 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3917 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/_code_block.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    16860 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/_handler.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    19078 2023-05-11 07:18:31.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/_logic.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1712 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/logging.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      747 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/__init__.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4622 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/ensure_shape.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3928 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/extended_sequential.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8081 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3109 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2139 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy_conv.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1355 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy_linear.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/parallel/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       87 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/parallel/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    13350 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/parallel/distributed.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.559586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      989 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4392 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_as_output.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1021 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_constants.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      951 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_globals.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3568 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_grad.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      659 2023-03-06 02:09:36.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_helper.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    21962 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_lax.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14777 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/annotate.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    17459 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/export_testcase.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1231 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/load.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.559586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/pfto_exporter/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       60 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/pfto_exporter/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    47261 2023-05-11 07:18:31.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/pfto_exporter/export.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3470 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/strip_large_tensor.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1129 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/symbolic_registry.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4784 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/unstrip_tensor.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.559586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/profiler/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      360 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/profiler/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2963 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/profiler/_record.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    11611 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/profiler/_time_summary.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/py.typed
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    15212 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/reporting.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.559586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      267 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1739 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_autocast.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      380 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_map.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      846 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_registry.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    17535 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_runtime.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2572 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_to.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      504 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/torchscript.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.559586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1026 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     6564 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_evaluator.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1531 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_manager_protocol.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14943 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_trainer.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      458 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_transform_model.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2929 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_trigger_util.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      716 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_util.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    10472 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extension.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2520 2023-03-06 02:09:36.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    19200 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/_snapshot.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4490 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/best_value.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    17521 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/evaluator.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1393 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/fail_on_non_number.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    10517 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/log_report.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2579 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/lr_scheduler.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3666 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/micro_average.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     7484 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/parameter_statistics.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8454 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/plot_report.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     6878 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/print_report.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2167 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/print_report_notebook.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     6041 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/profile_report.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4062 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/progress_bar.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5494 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14630 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/slack.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       81 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/snapshot_writers.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     4372 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/util.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2023 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/value_observation.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    15270 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    27923 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/manager.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1146 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/metrics.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      493 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/trigger.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      772 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5064 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2876 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/interval_trigger.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2399 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5041 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1654 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/once_trigger.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      965 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/time_trigger.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/utils/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      110 2023-04-03 06:31:42.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/utils/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2022-03-04 05:54:25.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/utils/_is_notebook.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2015 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/utils/checkpoint.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    28023 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/utils/comparer.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      689 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3068 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_parallel_writer.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5454 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_queue_writer.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1591 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_simple_writer.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2828 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_tensorboard_writer.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    12856 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_writer_base.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.555586 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras.egg-info/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      318 2023-05-11 07:41:59.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8076 2023-05-11 07:42:00.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        1 2023-05-11 07:42:00.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       98 2023-05-11 07:42:00.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras.egg-info/requires.txt
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)       19 2023-05-11 07:42:00.000000 pytorch-pfn-extras-0.6.7/pytorch_pfn_extras.egg-info/top_level.txt
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      709 2023-05-11 07:42:00.567586 pytorch-pfn-extras-0.6.7/setup.cfg
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      802 2022-12-27 05:10:31.000000 pytorch-pfn-extras-0.6.7/setup.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.551586 pytorch-pfn-extras-0.6.7/tests/
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/__init__.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/cuda_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/cuda_tests/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2869 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/cuda_tests/test_allocator.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataloader_test/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataloader_test/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1147 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataloader_test/test_dataloader.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/__init__.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1288 2020-09-04 02:31:31.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/dummy_dataset.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1104 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_asmode.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3022 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_concat.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      650 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_delegate_dataset.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    11731 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_from_data.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2972 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_join.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     7949 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_slice.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2997 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_tabular_dataset.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     7563 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_transform.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     1125 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_converter.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      986 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_torch_dataloader.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      863 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/test_shared_dataset.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.563586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/__init__.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.567586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2020-05-12 06:46:24.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     8094 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_extended_sequential.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     5685 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      963 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_batchnorm.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      926 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_conv.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      405 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_linear.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.567586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     9362 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/test_distributed.py
+drwxrwxr-x   0 ecastill  (2428) ecastill  (2428)        0 2023-05-11 07:42:00.567586 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/profiler_tests/
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)        0 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/profiler_tests/__init__.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     2816 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/profiler_tests/test_time_summary.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     9794 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_config.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3386 2021-07-29 07:52:35.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_config_types.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    19653 2023-04-06 07:19:19.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_handler.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      695 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_logging.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)    14959 2022-11-01 08:10:34.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_reporter.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)     3002 2023-01-26 08:06:57.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_tensor.py
+-rw-rw-r--   0 ecastill  (2428) ecastill  (2428)      615 2023-01-26 08:07:04.000000 pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_writing.py
```

### Comparing `pytorch-pfn-extras-0.6.6/LICENSE` & `pytorch-pfn-extras-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/README.md` & `pytorch-pfn-extras-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/_tensor.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/config.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/config.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/config_types.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/config_types.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/cuda/_allocator.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/cuda/_allocator.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataloaders/utils.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataloaders/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/shared_dataset.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/shared_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_asmode.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_asmode.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_concat.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_concat.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_join.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_join.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_slice.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_slice.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_transform.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_transform.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_utils.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/_with_converter.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/_with_converter.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/delegate_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/from_data.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/from_data.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/dataset/tabular/tabular_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/_dataset_util.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/_dataset_util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/_distributed_validation_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/distributed/_initialize.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/distributed/_initialize.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/engine.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/_code_block.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/_code_block.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/_handler.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/handler/_logic.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/handler/_logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     def consume_options(self, options: Dict[str, Any]) -> None:
         super().consume_options(options)
 
         self.backward_outputs = options.pop('backward_outputs', None)
         self._grad_scaler = options.pop('grad_scaler', None)
 
         self._backward_fn = options.pop('backward_function', None)
-        autocast_options = options.get("autocast", False)
+        autocast_options = options.pop("autocast", False)
         if isinstance(autocast_options, bool):
             autocast_options = {"enabled": autocast_options, "device_type": "cuda"}
         self._autocast = _autocast._AutocastManager(
             autocast_options, self._grad_scaler is not None
         )
 
         if self._grad_scaler is not None:
```

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/logging.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/logging.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/ensure_shape.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/ensure_shape.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/extended_sequential.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/extended_sequential.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy_batchnorm.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy_conv.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy_conv.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/modules/lazy_linear.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/modules/lazy_linear.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/nn/parallel/distributed.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/nn/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_as_output.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_as_output.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_constants.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_constants.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_globals.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_globals.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_grad.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_grad.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_helper.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_helper.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/_lax.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/_lax.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/annotate.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/annotate.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/export_testcase.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/export_testcase.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/load.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/load.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/pfto_exporter/export.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/pfto_exporter/export.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import dataclasses
 import types
 import typing
 import warnings
 from typing import Any, Callable, Dict, Iterator, List, Optional, Sequence, Set, Tuple, Union, cast
+from contextlib import contextmanager
 
 import onnx
 import onnx.checker
 import onnx.helper
 import onnx.numpy_helper
 import onnx.shape_inference
 import pytorch_pfn_extras
 import pytorch_pfn_extras.onnx._constants
+from pytorch_pfn_extras.onnx import _grad as grad
 from pytorch_pfn_extras.onnx._globals import GLOBALS
 from pytorch_pfn_extras.torchscript import run_jit_pass
 import torch
 import torch.jit
 import torch.onnx.symbolic_helper as sym_hel
 import torch.onnx.utils as to_utils
 from torch.onnx import OperatorExportTypes
@@ -24,14 +26,97 @@
 
 # Alias confusing function names
 torch._C.Graph.returnNode = torch._C.Graph.return_node  # type: ignore[attr-defined]
 torch._C.Block.return_node = torch._C.Block.returnNode  # type: ignore[attr-defined]
 
 _ppe_ignore_scope: str = "_ppe_as_out_module"
 _list_create_ops: List[str] = ["prim::ListConstruct", "onnx::SequenceConstruct", "onnx::SequenceEmpty"]
+_fix_ir_version = 8
+
+# Original from https://github.com/pytorch/pytorch/blob/52a36a98d9425479f62b6e2d1a59e434b85f7f7e/torch/csrc/jit/passes/normalize_ops.cpp#L85-L162
+_op_normalize_table: Dict[str, str] = {
+    "absolute": "abs",
+    "absolute_": "abs_",
+    "clip": "clamp",
+    "clip_": "clamp_",
+    "det": "linalg_det",
+    "matrix_power": "linalg_matrix_power",
+    "matrix_exp": "linalg_matrix_exp",
+    "ger": "outer",
+    "arccos": "acos",
+    "arccos_": "acos_",
+    "arcsin": "asin",
+    "arcsin_": "asin_",
+    "arctan": "atan",
+    "arctan_": "atan_",
+    "arctan2": "atan2",
+    "arctan2_": "atan2_",
+    "arccosh": "acosh",
+    "arccosh_": "acosh_",
+    "arcsinh": "asinh",
+    "arcsinh_": "asinh_",
+    "arctanh": "atanh",
+    "arctanh_": "atanh_",
+    "fix": "trunc",
+    "fix_": "trunc_",
+    "negative": "neg",
+    "negative_": "neg_",
+    "subtract": "sub",
+    "subtract_": "sub_",
+    "greater_equal": "ge",
+    "greater_equal_": "ge_",
+    "greater": "gt",
+    "greater_": "gt_",
+    "less_equal": "le",
+    "less_equal_": "le_",
+    "less": "lt",
+    "less_": "lt_",
+    "not_equal": "ne",
+    "not_equal_": "ne_",
+    "divide": "div",
+    "divide_": "div_",
+    "multiply": "mul",
+    "multiply_": "mul_",
+    "linalg_matmul": "matmul",
+    "inverse": "linalg_inv",
+    "true_divide": "div",
+    "true_divide_": "div_",
+    "concat": "cat",
+    "concatenate": "cat",
+    "row_stack": "vstack",
+    "swapdims": "transpose",
+    "swapdims_": "transpose_",
+    "swapaxes": "transpose",
+    "swapaxes_": "transpose_",
+    "moveaxis": "movedim",
+    "special_erf": "erf",
+    "special_erfc": "erfc",
+    "special_erfinv": "erfinv",
+    "special_expit": "sigmoid",
+    "special_exp2": "exp2",
+    "special_expm1": "expm1",
+    "special_logit": "logit",
+    "special_logsumexp": "logsumexp",
+    "special_round": "round",
+    "special_log1p": "log1p",
+    "special_sinc": "sinc",
+    "special_digamma": "digamma",
+    "special_psi": "digamma",
+    "special_i0": "i0",
+    "special_xlogy": "xlogy",
+    "special_log_softmax": "log_softmax",
+    "orgqr": "linalg_householder_product",
+    "adjoint": "mH",
+    "special_multigammaln": "mvlgamma",
+    "special_polygamma": "polygamma",
+    "special_softmax": "softmax",
+    "special_gammainc": "igamma",
+    "special_gammaincc": "igammac",
+    "special_gammaln": "lgamma",
+}
 
 if pytorch_pfn_extras.requires("1.13"):
     from torch.onnx._internal import jit_utils
     GraphContext = jit_utils.GraphContext
 else:
     GraphContext = torch._C.Graph  # type: ignore
 
@@ -143,14 +228,28 @@
     v.type.tensor_type.shape.ClearField("dim")
     for i in t.shape:
         # TODO(twata): Support dynamic_axes
         a = v.type.tensor_type.shape.dim.add()
         a.dim_value = i
 
 
+@contextmanager
+def _force_tracing() -> Any:
+    old_is_tracing = torch.jit.is_tracing
+
+    def is_tracing() -> bool:
+        return True
+
+    try:
+        torch.jit.is_tracing = is_tracing
+        yield
+    finally:
+        torch.jit.is_tracing = old_is_tracing
+
+
 @dataclasses.dataclass
 class _ExporterOptions:
     opset_version: int = 12
 
     check_trace: bool = False
     strict_trace: bool = True
     force_outplace_trace: bool = False
@@ -216,35 +315,62 @@
         self._convert()
 
     def _restore_state(self) -> None:
         torch.set_rng_state(self.rng_state)
         if torch.cuda.is_available():
             torch.cuda.set_rng_state_all(self.cuda_rng_state)
 
+    # TODO(twata): Use `self.traced` instead or use traced result outputs
+    def _get_original_outputs(self) -> None:
+        self._restore_state()
+        with _force_tracing(), grad.init_grad_state():
+            self.original_outputs = self.original_model(*self.inputs)
+        self.flat_outputs = _to_tuple_if_not_sequence(torch._C._jit_flatten(self.original_outputs)[0])
+
     def _run_trace(self) -> None:
         # TODO(twata): Use `torch._C._craete_graph_by_tracing` instead.
         # So that we don't need to run heavy models multiple times
-        self.traced: torch.jit.RecursiveScriptModule = torch.jit.trace(  # type: ignore
-            self.original_model,
-            self.inputs,
-            check_trace=self.check_trace,
-            strict=self.strict_trace,
-            _force_outplace=self.force_outplace_trace,
-        )
+        self._restore_state()
+        with grad.init_grad_state():
+            self.traced: torch.jit.RecursiveScriptModule = torch.jit.trace(  # type: ignore
+                self.original_model,
+                self.inputs,
+                check_trace=self.check_trace,
+                strict=self.strict_trace,
+                _force_outplace=self.force_outplace_trace,
+            )
 
         self.graph_doc_string = f"""
 # Model: {self.traced.original_name}
 """
 
-        # TODO(twata): Use `self.traced` instead or use traced result outputs
-        self._restore_state()
-        self.original_outputs = self.original_model(*self.inputs)
-        self.flat_outputs = _to_tuple_if_not_sequence(torch._C._jit_flatten(self.original_outputs)[0])
         self.g: torch._C.Graph = self.traced.inlined_graph
-        self.vars: Dict[str, torch.IValue] = {_remove_prefix(k, f"{_ppe_ignore_scope}."): v for k, v in self.traced.state_dict().items()}
+        """
+        `self.trace` ignores the override of `state_dict` method in `self.original_model`.
+        Thus, the key name may be different between state dict of `self.trace` and `self.original_model`.
+        pfto uses the key name of `self.original_model.state_dict()` as the parameter names in ONNX.
+
+        To implement this behavior, we have to prepare mapping from name of `self.trace` state_dict to
+        the name of `self.original_model` state_dict.
+        """
+        self.name_from_trace: Dict[str, str] = {}
+        vars_in_traced: Dict[str, torch.IValue] = {
+            _remove_prefix(k, f"{_ppe_ignore_scope}."): v for k, v in self.traced.state_dict().items()
+        }
+        if isinstance(self.original_model, torch.nn.Module):
+            vars_tmp: Dict[str, Any] = {
+                _remove_prefix(k, f"{_ppe_ignore_scope}."): v for k, v in self.traced.state_dict(keep_vars=True).items()
+            }
+            v_to_name: Dict[Any, str] = {v: k for k, v in self.original_model.state_dict(keep_vars=True).items()}
+            for name, v in vars_tmp.items():
+                self.name_from_trace[name] = v_to_name[v]
+        else:
+            for name in vars_in_traced.keys():
+                self.name_from_trace[name] = name
+        self.vars: Dict[str, torch.IValue] = {self.name_from_trace[name]: v for name, v in vars_in_traced.items()}
         self.torch2onnx_var: Dict[torch._C.Value, torch._C.Value] = {
             i: i for i in self.g.inputs()
         }
         self.self_id: Optional[TorchValueID] = None
         self.self_name: Optional[str] = None
         first_arg = list(self.g.inputs())[0]
         if first_arg.type().kind() == "ClassType":
@@ -272,14 +398,16 @@
             run_jit_pass(torch._C._jit_pass_constant_propagation, graph)  # type: ignore[attr-defined]
 
         # _split_tensor_list_constants(graph, graph)
         # run dce to eliminate dead parts of the graph that might have been
         # left behind by things like symbolic_override
         run_jit_pass(torch._C._jit_pass_dce, graph)
 
+        run_jit_pass(torch._C._jit_pass_cse, graph)
+
         run_jit_pass(torch._C._jit_pass_canonicalize_graph_fuser_ops, graph)  # type: ignore[attr-defined]
         torch._C._jit_pass_peephole(graph, True)  # type: ignore[attr-defined]
         run_jit_pass(torch._C._jit_pass_fuse_addmm, graph)  # type: ignore[attr-defined]
 
         torch._C._jit_pass_peephole(graph, True)  # type: ignore[attr-defined]
         torch._C._jit_pass_lower_all_tuples(graph)  # type: ignore[attr-defined]
         # in _jit_pass_onnx, symbolic functions are called for each node for conversion.
@@ -418,27 +546,23 @@
                 c.node().copyAttributes(n)
             return c
 
         self.run_symbolic_function(g, n, gen_const)
 
     def handle_getattr(self, g: torch._C.Graph, n: torch._C.Node) -> None:
         if self.is_self(n.input()) or self.attrs[_unique_id(n.input())] == _ppe_ignore_scope:
-            self.attrs[_unique_id(n.output())] = ONNXValueID(n.s("name"))
+            var_name = n.s("name")
         else:
-            self.attrs[_unique_id(n.output())] = ONNXValueID(
-                "%s.%s"
-                % (
-                    self.attrs[_unique_id(n.input())],
-                    n.s("name"),
-                )
-            )
-        var_name = self.attrs[_unique_id(n.output())]
+            var_name = "%s.%s" % (self.attrs[_unique_id(n.input())], n.s("name"))
+        if var_name in self.name_from_trace:
+            var_name = self.name_from_trace[var_name]
         if var_name in self.vars:
             assert isinstance(self.vars[var_name], torch.Tensor)
             n.output().inferTypeFrom(cast(torch.Tensor, self.vars[var_name]))
+        self.attrs[_unique_id(n.output())] = ONNXValueID(var_name)
 
     def handle_list_construct(self, g: torch._C.Graph, n: torch._C.Node) -> None:
         # Concat if int type input
         is_integer_output: bool = cast(torch._C.TensorType, n.output().type()).getElementType().kind() == "IntType"
         if len(list(n.inputs())) > 0 and is_integer_output:
 
             def gen_concat(g: torch._C.Graph, *args: Any) -> torch._C.Value:
@@ -515,14 +639,17 @@
                 if pytorch_pfn_extras.requires('1.11'):
                     domain = "prim"
                 else:
                     op = f"prim_{op}"
 
             import pytorch_pfn_extras.onnx.symbolic_registry as sym_reg
 
+            if not sym_reg.is_registered_op(op, domain, self.opset_version) and op in _op_normalize_table:
+                op = _op_normalize_table[op]
+
             if sym_reg.is_registered_op(op, domain, self.opset_version):  # type: ignore[no-untyped-call]
                 return cast(  # type: ignore[redundant-cast]
                     Callable, sym_reg.get_registered_op(op, domain, self.opset_version)  # type: ignore[no-untyped-call]
                 )
             else:
                 return None
 
@@ -917,18 +1044,19 @@
                 if node.domain != onnx.defs.ONNX_DOMAIN:
                     opsets[node.domain] = self.custom_opsets.get(node.domain, 1)
             opset_imports = []
             for domain, version in opsets.items():
                 opset_imports.append(onnx.helper.make_opsetid(domain, version))
             return opset_imports
 
-        model: onnx.ModelProto = onnx.helper.make_model(
+        model: onnx.ModelProto = onnx.helper.make_model_gen_version(
             graph,
             opset_imports=get_model_opset_imports(graph),
             producer_name="pfto",
+            ir_version=_fix_ir_version,
         )
         model = self.check_model(model)
 
         # Applying dynamic axes after onnx shape inference since it will be erased
         for o in model.graph.output:
             apply_dynamic_axes_info(o, o.name)
 
@@ -952,14 +1080,15 @@
                 else:
                     to_utils.__IN_ONNX_EXPORT = True  # type: ignore[attr-defined]
                     sym_hel._set_opset_version(self.opset_version)  # type: ignore[no-untyped-call]
                     sym_hel._set_operator_export_type(self.operator_export_type)  # type: ignore[no-untyped-call]
                     sym_hel._set_onnx_shape_inference(  # type: ignore[no-untyped-call]
                         False  # TODO(twata): Use `self.onnx_shape_inference`
                     )
+                self._get_original_outputs()
                 self._run_trace()
                 self.model: onnx.ModelProto = self.generate_onnx()
         finally:
             if pytorch_pfn_extras.requires("1.13"):
                 GLOBALS.in_onnx_export = False  # type: ignore[attr-defined]
                 if prev_opset_version is not None:
                     GLOBALS.export_onnx_opset_version = prev_opset_version
```

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/strip_large_tensor.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/strip_large_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/symbolic_registry.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/symbolic_registry.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/onnx/unstrip_tensor.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/onnx/unstrip_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/profiler/_record.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/profiler/_record.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/profiler/_time_summary.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/profiler/_time_summary.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/reporting.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/reporting.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_autocast.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_autocast.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_registry.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_registry.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_runtime.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_runtime.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/runtime/_to.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/runtime/_to.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_evaluator.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_evaluator.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_manager_protocol.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_manager_protocol.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_trainer.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_trainer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_trigger_util.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_trigger_util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/_util.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/_util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extension.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extension.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/_snapshot.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/_snapshot.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/best_value.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/best_value.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/evaluator.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/evaluator.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/fail_on_non_number.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/fail_on_non_number.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/log_report.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/log_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/lr_scheduler.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/micro_average.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/micro_average.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/parameter_statistics.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/parameter_statistics.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/plot_report.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/plot_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/print_report.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/print_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/print_report_notebook.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/print_report_notebook.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/profile_report.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/profile_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/progress_bar.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/progress_bar_notebook.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/slack.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/slack.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/util.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/util.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/value_observation.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/value_observation.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/extensions/variable_statistics_plot.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/manager.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/manager.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/metrics.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/metrics.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/early_stopping_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/interval_trigger.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/interval_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/manual_schedule_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/minmax_value_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/once_trigger.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/once_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/training/triggers/time_trigger.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/training/triggers/time_trigger.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/utils/checkpoint.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/utils/comparer.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/utils/comparer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/__init__.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_parallel_writer.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_parallel_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_queue_writer.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_queue_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_simple_writer.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_simple_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_tensorboard_writer.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras/writing/_writer_base.py` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras/writing/_writer_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/pytorch_pfn_extras.egg-info/SOURCES.txt` & `pytorch-pfn-extras-0.6.7/pytorch_pfn_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/setup.cfg` & `pytorch-pfn-extras-0.6.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/setup.py` & `pytorch-pfn-extras-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/cuda_tests/test_allocator.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/cuda_tests/test_allocator.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataloader_test/test_dataloader.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataloader_test/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/dummy_dataset.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_asmode.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_asmode.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_concat.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_delegate_dataset.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_delegate_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_from_data.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_from_data.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_join.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_join.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_slice.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_tabular_dataset.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_tabular_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_transform.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_converter.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_converter.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_torch_dataloader.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/tabular_tests/test_with_torch_dataloader.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/dataset_tests/test_shared_dataset.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/dataset_tests/test_shared_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_extended_sequential.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_extended_sequential.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_batchnorm.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_batchnorm.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_conv.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/modules_tests/test_lazy_conv.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/test_distributed.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/nn_tests/parallel_tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/profiler_tests/test_time_summary.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/profiler_tests/test_time_summary.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_config.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_config_types.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_config_types.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_handler.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_logging.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_reporter.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_tensor.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-pfn-extras-0.6.6/tests/pytorch_pfn_extras_tests/test_writing.py` & `pytorch-pfn-extras-0.6.7/tests/pytorch_pfn_extras_tests/test_writing.py`

 * *Files identical despite different names*

