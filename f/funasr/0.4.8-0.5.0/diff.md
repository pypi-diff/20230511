# Comparing `tmp/funasr-0.4.8.tar.gz` & `tmp/funasr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.4.8.tar", last modified: Mon May  8 08:57:38 2023, max compression
+gzip compressed data, was "funasr-0.5.0.tar", last modified: Thu May 11 11:37:25 2023, max compression
```

## Comparing `funasr-0.4.8.tar` & `funasr-0.5.0.tar`

### file list

```diff
@@ -1,422 +1,425 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.449194 funasr-0.4.8/
--rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.4.8/LICENSE
--rw-r--r--   0 zhifu      (502) staff       (20)     8180 2023-05-08 08:57:38.448993 funasr-0.4.8/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7158 2023-05-07 09:22:42.000000 funasr-0.4.8/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.291400 funasr-0.4.8/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.308567 funasr-0.4.8/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21327 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/asr_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11203 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/asr_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/asr_inference_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37897 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/bin/asr_inference_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26713 2023-05-08 02:37:47.000000 funasr-0.4.8/funasr/bin/asr_inference_paraformer_streaming.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19242 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/asr_inference_paraformer_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32974 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/asr_inference_paraformer_vad_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25051 2023-04-25 05:58:46.000000 funasr-0.4.8/funasr/bin/asr_inference_rnnt.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/asr_inference_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23931 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/bin/asr_inference_uniasr_vad.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1006 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/bin/asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/bin/asr_train_paraformer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/asr_train_transducer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/bin/asr_train_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5382 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-03-10 07:21:13.000000 funasr-0.4.8/funasr/bin/diar_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/eend_ola_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-02-11 09:29:33.000000 funasr-0.4.8/funasr/bin/lm_calc_perplexity.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/lm_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-02-11 09:29:33.000000 funasr-0.4.8/funasr/bin/lm_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/bin/modelscope_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-03-10 07:21:13.000000 funasr-0.4.8/funasr/bin/punc_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/punctuation_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11101 2023-05-08 08:08:13.000000 funasr-0.4.8/funasr/bin/punctuation_infer_vadrealtime.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/sond_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/sv_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.4.8/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-04-25 07:21:40.000000 funasr-0.4.8/funasr/bin/tp_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/tp_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19910 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/bin/vad_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/bin/vad_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11688 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/bin/vad_inference_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.310716 funasr-0.4.8/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.4.8/funasr/datasets/iterable_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/iterable_dataset_modelscope.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.311680 funasr-0.4.8/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.312793 funasr-0.4.8/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9294 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.315105 funasr-0.4.8/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2583 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.4.8/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.315571 funasr-0.4.8/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10833 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.316625 funasr-0.4.8/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.317321 funasr-0.4.8/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.4.8/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.4.8/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.318584 funasr-0.4.8/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.4.8/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.4.8/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.321231 funasr-0.4.8/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.4.8/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.4.8/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.321741 funasr-0.4.8/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.4.8/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.324056 funasr-0.4.8/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-05-05 07:04:25.000000 funasr-0.4.8/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.324554 funasr-0.4.8/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.4.8/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.327235 funasr-0.4.8/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3479 2023-03-29 08:06:18.000000 funasr-0.4.8/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.328533 funasr-0.4.8/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.331865 funasr-0.4.8/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.4.8/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.332608 funasr-0.4.8/funasr/lm/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/lm/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/lm/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/lm/seq_rnn_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/lm/transformer_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.332976 funasr-0.4.8/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2804 2023-03-02 10:32:58.000000 funasr-0.4.8/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.334610 funasr-0.4.8/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.342319 funasr-0.4.8/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.4.8/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.345537 funasr-0.4.8/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7917 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    28528 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-04-27 09:38:10.000000 funasr-0.4.8/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34815 2023-04-27 08:40:56.000000 funasr-0.4.8/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.357052 funasr-0.4.8/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43611 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.4.8/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.4.8/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.4.8/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-02-16 09:30:51.000000 funasr-0.4.8/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.358665 funasr-0.4.8/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.4.8/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.4.8/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.4.8/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    54458 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.361652 funasr-0.4.8/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8895 2023-02-16 09:30:51.000000 funasr-0.4.8/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-02-23 03:32:15.000000 funasr-0.4.8/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.362345 funasr-0.4.8/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.362762 funasr-0.4.8/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3546 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.363440 funasr-0.4.8/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.363772 funasr-0.4.8/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-04-27 09:38:10.000000 funasr-0.4.8/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.365232 funasr-0.4.8/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/preencoder/sinc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.365935 funasr-0.4.8/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.373975 funasr-0.4.8/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    36791 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.375360 funasr-0.4.8/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/beam_search/beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.378015 funasr-0.4.8/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.4.8/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.379282 funasr-0.4.8/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.4.8/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.4.8/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.381067 funasr-0.4.8/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.4.8/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.4.8/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22114 2023-04-25 05:58:46.000000 funasr-0.4.8/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3649 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.382770 funasr-0.4.8/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.383884 funasr-0.4.8/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.386463 funasr-0.4.8/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.387606 funasr-0.4.8/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.387946 funasr-0.4.8/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.8/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.388155 funasr-0.4.8/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.8/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.389145 funasr-0.4.8/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.4.8/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.389896 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.391760 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.394411 funasr-0.4.8/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      617 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/demo.py
--rw-r--r--   0 zhifu      (502) staff       (20)      740 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      932 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      383 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      969 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.395917 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8145 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12285 2023-05-08 05:20:27.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.398716 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-05-07 16:24:45.000000 funasr-0.4.8/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.400976 funasr-0.4.8/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.402444 funasr-0.4.8/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.405574 funasr-0.4.8/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74081 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    60767 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.411867 funasr-0.4.8/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.415610 funasr-0.4.8/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.438659 funasr-0.4.8/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/train/abs_espnet_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.4.8/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37188 2023-05-07 09:22:42.000000 funasr-0.4.8/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.446179 funasr-0.4.8/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.4.8/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.4.8/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.4.8/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.4.8/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.4.8/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7735 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13178 2023-04-12 07:23:40.000000 funasr-0.4.8/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.4.8/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.4.8/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-08 08:57:08.000000 funasr-0.4.8/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.292353 funasr-0.4.8/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8180 2023-05-08 08:57:38.000000 funasr-0.4.8/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13306 2023-05-08 08:57:38.000000 funasr-0.4.8/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-08 08:57:38.000000 funasr-0.4.8/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      838 2023-05-08 08:57:38.000000 funasr-0.4.8/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-08 08:57:38.000000 funasr-0.4.8/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-08 08:57:38.449249 funasr-0.4.8/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4573 2023-04-25 05:58:46.000000 funasr-0.4.8/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-08 08:57:38.448527 funasr-0.4.8/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.4.8/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.4.8/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.4.8/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.4.8/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.4.8/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.4.8/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.324266 funasr-0.5.0/
+-rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.5.0/LICENSE
+-rw-r--r--   0 zhifu      (502) staff       (20)     8239 2023-05-11 11:37:25.324040 funasr-0.5.0/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7217 2023-05-11 11:36:41.000000 funasr-0.5.0/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.127685 funasr-0.5.0/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.184609 funasr-0.5.0/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21913 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/bin/asr_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11106 2023-05-11 11:22:48.000000 funasr-0.5.0/funasr/bin/asr_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/asr_inference_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40504 2023-05-11 11:28:45.000000 funasr-0.5.0/funasr/bin/asr_inference_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26713 2023-05-08 02:37:47.000000 funasr-0.5.0/funasr/bin/asr_inference_paraformer_streaming.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    24956 2023-05-09 09:17:41.000000 funasr-0.5.0/funasr/bin/asr_inference_rnnt.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/asr_inference_uniasr.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1068 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/bin/asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/bin/asr_train_paraformer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/asr_train_transducer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/bin/asr_train_uniasr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5382 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-03-10 07:21:13.000000 funasr-0.5.0/funasr/bin/diar_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/eend_ola_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-02-11 09:29:33.000000 funasr-0.5.0/funasr/bin/lm_calc_perplexity.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/lm_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-02-11 09:29:33.000000 funasr-0.5.0/funasr/bin/lm_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/bin/modelscope_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-03-10 07:21:13.000000 funasr-0.5.0/funasr/bin/punc_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/punctuation_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11101 2023-05-08 08:08:13.000000 funasr-0.5.0/funasr/bin/punctuation_infer_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23328 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/bin/sa_asr_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1071 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/sond_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/sv_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.0/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-04-25 07:21:40.000000 funasr-0.5.0/funasr/bin/tp_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/tp_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19679 2023-05-08 14:05:34.000000 funasr-0.5.0/funasr/bin/vad_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/bin/vad_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11618 2023-05-08 14:05:34.000000 funasr-0.5.0/funasr/bin/vad_inference_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.187613 funasr-0.5.0/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.0/funasr/datasets/iterable_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/iterable_dataset_modelscope.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.188792 funasr-0.5.0/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.190102 funasr-0.5.0/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9294 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.192863 funasr-0.5.0/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2583 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.0/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.193425 funasr-0.5.0/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10833 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.194509 funasr-0.5.0/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.195257 funasr-0.5.0/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.0/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.0/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.196388 funasr-0.5.0/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.0/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.0/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.198078 funasr-0.5.0/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.0/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.0/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.198650 funasr-0.5.0/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.0/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.200756 funasr-0.5.0/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-05-05 07:04:25.000000 funasr-0.5.0/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.201293 funasr-0.5.0/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.0/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.203012 funasr-0.5.0/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3539 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.204232 funasr-0.5.0/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.207578 funasr-0.5.0/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.0/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.208443 funasr-0.5.0/funasr/lm/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/lm/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/lm/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/lm/seq_rnn_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/lm/transformer_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.208945 funasr-0.5.0/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.210221 funasr-0.5.0/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.219345 funasr-0.5.0/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.0/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.221771 funasr-0.5.0/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.0/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-04-27 09:38:10.000000 funasr-0.5.0/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34796 2023-05-09 09:17:41.000000 funasr-0.5.0/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19501 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.228415 funasr-0.5.0/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43608 2023-05-09 09:17:41.000000 funasr-0.5.0/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.0/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.0/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.0/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-02-16 09:30:51.000000 funasr-0.5.0/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.230354 funasr-0.5.0/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.0/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    54458 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.233148 funasr-0.5.0/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9106 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-02-23 03:32:15.000000 funasr-0.5.0/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.233871 funasr-0.5.0/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.234270 funasr-0.5.0/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.237215 funasr-0.5.0/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.239611 funasr-0.5.0/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-04-27 09:38:10.000000 funasr-0.5.0/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.241400 funasr-0.5.0/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/preencoder/sinc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.242256 funasr-0.5.0/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.251372 funasr-0.5.0/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.254832 funasr-0.5.0/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.262425 funasr-0.5.0/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.0/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.271879 funasr-0.5.0/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.0/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.0/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.276611 funasr-0.5.0/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.0/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.0/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.0/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.0/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.278387 funasr-0.5.0/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.279669 funasr-0.5.0/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.280873 funasr-0.5.0/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.281585 funasr-0.5.0/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.281892 funasr-0.5.0/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.0/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.282061 funasr-0.5.0/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.0/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.282848 funasr-0.5.0/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.0/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.283488 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.285722 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.288197 funasr-0.5.0/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      617 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/demo.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      740 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      932 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      383 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      969 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.289628 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8145 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12299 2023-05-08 10:59:00.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.292369 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-05-08 10:59:26.000000 funasr-0.5.0/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.294806 funasr-0.5.0/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.295779 funasr-0.5.0/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.301412 funasr-0.5.0/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74340 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    60814 2023-05-09 09:17:41.000000 funasr-0.5.0/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21378 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.304092 funasr-0.5.0/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.306812 funasr-0.5.0/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.311098 funasr-0.5.0/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/train/abs_espnet_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.0/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    37188 2023-05-07 09:22:42.000000 funasr-0.5.0/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.320633 funasr-0.5.0/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.0/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.0/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.0/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.0/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.0/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.0/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.0/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-11 08:34:48.000000 funasr-0.5.0/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.0/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.0/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-11 11:36:41.000000 funasr-0.5.0/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.128872 funasr-0.5.0/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8239 2023-05-11 11:37:25.000000 funasr-0.5.0/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13360 2023-05-11 11:37:25.000000 funasr-0.5.0/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-11 11:37:25.000000 funasr-0.5.0/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      864 2023-05-11 11:37:25.000000 funasr-0.5.0/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-11 11:37:25.000000 funasr-0.5.0/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-11 11:37:25.324513 funasr-0.5.0/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4641 2023-05-09 03:02:42.000000 funasr-0.5.0/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-11 11:37:25.323060 funasr-0.5.0/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.0/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.0/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.0/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.0/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.0/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.0/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.4.8/LICENSE` & `funasr-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/PKG-INFO` & `funasr-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.4.8
+Version: 0.5.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -44,16 +44,16 @@
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
-### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
-We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge
+We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.4.8 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.0 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -30,52 +30,52 @@
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
 Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
 modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
 (https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
 meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
-Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
-announce that the M2MeT2.0 challenge will be held in the near future. The
-baseline system is conducted on FunASR and is provided as a receipe of
-AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
-notes For the release notes, please ref to [news](https://github.com/alibaba-
-damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
-recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
-Restoration, Language Models, Speaker Verification and Speaker diarization. -
-We have released large number of academic and industrial pretrained models on
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/
-FunASR/blob/main/docs/model_zoo/modelscope_models.md) - The pretrained model
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
-performance on many tasks in [SpeechIO leaderboard](https://github.com/
-SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
-pretrained models from [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
-github.com/espnet/espnet) framework, the training speed of large-scale datasets
-in FunASR is much faster owning to the optimized dataloader. ## Installation
-Install from pip ```shell pip install -U funasr # For the users in China, you
-could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
-have any questions about FunASR, please contact us by - email:
-[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
-Wechat group | |:---:|:-----------------------------------------------------:
-| |
+Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We are pleased to
+announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023
+challenge special session. The registration is now open. The baseline system is
+conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more
+details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-
+academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-
+academy.github.io/FunASR/m2met2/index.html)). ### Release notes For the release
+notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/
+releases) ## Highlights - FunASR supports speech recognition(ASR), Multi-talker
+ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models,
+Speaker Verification and Speaker diarization. - We have released large number
+of academic and industrial pretrained models on [ModelScope](https://
+www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model
+Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md) - The pretrained model [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) obtains the best performance on many tasks in
+[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
+supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
+(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
+Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
+speed of large-scale datasets in FunASR is much faster owning to the optimized
+dataloader. ## Installation Install from pip ```shell pip install -U funasr #
+For the users in China, you could install with the command: # pip install -
+U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
+source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
+pip install -e ./ # For the users in China, you could install with the command:
+# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
+want to use the pretrained models in ModelScope, you should install the
+modelscope: ```shell pip install -U modelscope # For the users in China, you
+could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Contact If you have any questions about FunASR, please
+contact us by - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-
+inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
+------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.4.8/README.md` & `funasr-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
-### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
-We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge
+We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
```

#### html2text {}

```diff
@@ -17,52 +17,52 @@
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
 Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
 modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
 (https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
 meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
-Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
-announce that the M2MeT2.0 challenge will be held in the near future. The
-baseline system is conducted on FunASR and is provided as a receipe of
-AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
-notes For the release notes, please ref to [news](https://github.com/alibaba-
-damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
-recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
-Restoration, Language Models, Speaker Verification and Speaker diarization. -
-We have released large number of academic and industrial pretrained models on
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/
-FunASR/blob/main/docs/model_zoo/modelscope_models.md) - The pretrained model
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
-performance on many tasks in [SpeechIO leaderboard](https://github.com/
-SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
-pretrained models from [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
-github.com/espnet/espnet) framework, the training speed of large-scale datasets
-in FunASR is much faster owning to the optimized dataloader. ## Installation
-Install from pip ```shell pip install -U funasr # For the users in China, you
-could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
-have any questions about FunASR, please contact us by - email:
-[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
-Wechat group | |:---:|:-----------------------------------------------------:
-| |
+Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We are pleased to
+announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023
+challenge special session. The registration is now open. The baseline system is
+conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more
+details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-
+academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-
+academy.github.io/FunASR/m2met2/index.html)). ### Release notes For the release
+notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/
+releases) ## Highlights - FunASR supports speech recognition(ASR), Multi-talker
+ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models,
+Speaker Verification and Speaker diarization. - We have released large number
+of academic and industrial pretrained models on [ModelScope](https://
+www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model
+Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md) - The pretrained model [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) obtains the best performance on many tasks in
+[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
+supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
+(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
+Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
+speed of large-scale datasets in FunASR is much faster owning to the optimized
+dataloader. ## Installation Install from pip ```shell pip install -U funasr #
+For the users in China, you could install with the command: # pip install -
+U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
+source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
+pip install -e ./ # For the users in China, you could install with the command:
+# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
+want to use the pretrained models in ModelScope, you should install the
+modelscope: ```shell pip install -U modelscope # For the users in China, you
+could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Contact If you have any questions about FunASR, please
+contact us by - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-
+inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
+------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.4.8/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.5.0/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/asr_inference.py` & `funasr-0.5.0/funasr/bin/asr_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
+from funasr.tasks.asr import frontend_choices
 
 
 header_colors = '\033[95m'
 end_colors = '\033[0m'
 
 
 class Speech2Text:
@@ -88,15 +89,19 @@
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = ASRTask.build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
+            if asr_train_args.frontend=='wav_frontend':
+                frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
+            else:
+                frontend_class=frontend_choices.get_class(asr_train_args.frontend)
+                frontend = frontend_class(**asr_train_args.frontend_conf).eval()
 
         logging.info("asr_model: {}".format(asr_model))
         logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
 
         decoder = asr_model.decoder
 
@@ -107,15 +112,15 @@
             ctc=ctc,
             length_bonus=LengthBonus(len(token_list)),
         )
 
         # 2. Build Language model
         if lm_train_config is not None:
             lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
+                lm_train_config, lm_file, None, device
             )
             scorers["lm"] = lm.lm
 
         # 3. Build ngram model
         # ngram is not supported now
         ngram = None
         scorers["ngram"] = ngram
@@ -189,15 +194,15 @@
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
         assert check_argument_types()
-
+        
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
@@ -276,14 +281,15 @@
         streaming: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
+        mc: bool = False,
         **kwargs,
 ):
     inference_pipeline = inference_modelscope(
         maxlenratio=maxlenratio,
         minlenratio=minlenratio,
         batch_size=batch_size,
         beam_size=beam_size,
@@ -306,14 +312,15 @@
         streaming=streaming,
         output_dir=output_dir,
         dtype=dtype,
         seed=seed,
         ngram_weight=ngram_weight,
         nbest=nbest,
         num_workers=num_workers,
+        mc=mc,
         **kwargs,
     )
     return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
 def inference_modelscope(
     maxlenratio: float,
     minlenratio: float,
@@ -338,27 +345,31 @@
     streaming: bool = False,
     output_dir: Optional[str] = None,
     dtype: str = "float32",
     seed: int = 0,
     ngram_weight: float = 0.9,
     nbest: int = 1,
     num_workers: int = 1,
+    mc: bool = False,
     param_dict: dict = None,
     **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
     
+    for handler in logging.root.handlers[:]:
+        logging.root.removeHandler(handler)
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
     
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
@@ -404,23 +415,24 @@
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
         loader = ASRTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
+            mc=mc,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
             preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
             collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-        
+
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
@@ -448,25 +460,28 @@
             for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
                 # Create a directory: outdir/{n}best_recog
                 if writer is not None:
                     ibest_writer = writer[f"{n}best_recog"]
                     
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
-                    # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
+                    ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
                 
                 if text is not None:
                     text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
                     item = {'key': key, 'value': text_postprocessed}
                     asr_result_list.append(item)
                     finish_count += 1
                     asr_utils.print_progress(finish_count / file_count)
                     if writer is not None:
                         ibest_writer["text"][key] = text
+
+                logging.info("uttid: {}".format(key))
+                logging.info("text predictions: {}\n".format(text))
         return asr_result_list
     
     return _forward
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="ASR Decoding",
@@ -633,8 +648,8 @@
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
     inference(**kwargs)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_launch.py` & `funasr-0.5.0/funasr/bin/asr_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,21 @@
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=True,
         action="append",
     )
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
+    group.add_argument(
+            "--mc",
+            type=bool,
+            default=False,
+            help="MultiChannel input",
+        )
+        
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
         "--vad_infer_config",
         type=str,
         help="VAD infer configuration",
     )
     group.add_argument(
@@ -244,35 +250,23 @@
         return None
     if mode == "asr":
         from funasr.bin.asr_inference import inference_modelscope
         return inference_modelscope(**kwargs)
     elif mode == "uniasr":
         from funasr.bin.asr_inference_uniasr import inference_modelscope
         return inference_modelscope(**kwargs)
-    elif mode == "uniasr_vad":
-        from funasr.bin.asr_inference_uniasr_vad import inference_modelscope
-        return inference_modelscope(**kwargs)
     elif mode == "paraformer":
         from funasr.bin.asr_inference_paraformer import inference_modelscope
         return inference_modelscope(**kwargs)
     elif mode == "paraformer_streaming":
         from funasr.bin.asr_inference_paraformer_streaming import inference_modelscope
         return inference_modelscope(**kwargs)
-    elif mode == "paraformer_vad":
-        from funasr.bin.asr_inference_paraformer_vad import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "paraformer_punc":
-        logging.info("Unknown decoding mode: {}".format(mode))
-        return None
-    elif mode == "paraformer_vad_punc":
-        from funasr.bin.asr_inference_paraformer_vad_punc import inference_modelscope
-        return inference_modelscope(**kwargs)
-    elif mode == "vad":
-        from funasr.bin.vad_inference import inference_modelscope
-        return inference_modelscope(**kwargs)
+    elif mode.startswith("paraformer_vad"):
+        from funasr.bin.asr_inference_paraformer import inference_modelscope_vad_punc
+        return inference_modelscope_vad_punc(**kwargs)
     elif mode == "mfcca":
         from funasr.bin.asr_inference_mfcca import inference_modelscope
         return inference_modelscope(**kwargs)
     elif mode == "rnnt":
         from funasr.bin.asr_inference_rnnt import inference_modelscope
         return inference_modelscope(**kwargs)
     else:
@@ -284,26 +278,28 @@
         mode = kwargs['mode']
     else:
         logging.info("Unknown decoding mode.")
         return None
     if mode == "asr":
         from funasr.bin.asr_inference import inference
         return inference(**kwargs)
+    elif mode == "sa_asr":
+        from funasr.bin.sa_asr_inference import inference
+        return inference(**kwargs)
     elif mode == "uniasr":
         from funasr.bin.asr_inference_uniasr import inference
         return inference(**kwargs)
     elif mode == "paraformer":
-        from funasr.bin.asr_inference_paraformer import inference
-        return inference(**kwargs)
-    elif mode == "paraformer_vad_punc":
-        from funasr.bin.asr_inference_paraformer_vad_punc import inference
-        return inference(**kwargs)
-    elif mode == "vad":
-        from funasr.bin.vad_inference import inference
-        return inference(**kwargs)
+        from funasr.bin.asr_inference_paraformer import inference_modelscope
+        inference_pipeline = inference_modelscope(**kwargs)
+        return inference_pipeline(kwargs["data_path_and_name_and_type"], hotword=kwargs.get("hotword", None))
+    elif mode.startswith("paraformer_vad"):
+        from funasr.bin.asr_inference_paraformer import inference_modelscope_vad_punc
+        inference_pipeline = inference_modelscope_vad_punc(**kwargs)
+        return inference_pipeline(kwargs["data_path_and_name_and_type"], hotword=kwargs.get("hotword", None))
     elif mode == "mfcca":
         from funasr.bin.asr_inference_mfcca import inference_modelscope
         return inference_modelscope(**kwargs)
     elif mode == "rnnt":
         from funasr.bin.asr_inference_rnnt import inference
         return inference(**kwargs)
     else:
@@ -338,8 +334,8 @@
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
 
     inference_launch_funasr(**kwargs)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_mfcca.py` & `funasr-0.5.0/funasr/bin/asr_inference_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_paraformer.py` & `funasr-0.5.0/funasr/bin/asr_inference_paraformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
 from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
 from funasr.bin.tp_inference import SpeechText2Timestamp
-
+from funasr.bin.vad_inference import Speech2VadSegment
+from funasr.bin.punctuation_infer import Text2Punc
+from funasr.utils.vad_utils import slice_padding_fbank
+from funasr.tasks.vad import VADTask
+from funasr.utils.timestamp_tools import time_stamp_sentence, ts_prediction_lfr6_standard
 
 class Speech2Text:
     """Speech2Text class
 
     Examples:
             >>> import soundfile
             >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
@@ -287,23 +291,22 @@
                 # Change integer-ids to tokens
                 token = self.converter.ids2tokens(token_int)
 
                 if self.tokenizer is not None:
                     text = self.tokenizer.tokens2text(token)
                 else:
                     text = None
-
+                timestamp = []
                 if isinstance(self.asr_model, BiCifParaformer):
-                    _, timestamp = ts_prediction_lfr6_standard(us_alphas[i], 
-                                                            us_peaks[i], 
+                    _, timestamp = ts_prediction_lfr6_standard(us_alphas[i][:enc_len[i]*3], 
+                                                            us_peaks[i][:enc_len[i]*3], 
                                                             copy.copy(token), 
                                                             vad_offset=begin_time)
-                    results.append((text, token, token_int, hyp, timestamp, enc_len_batch_total, lfr_factor))
-                else:
-                    results.append((text, token, token_int, hyp, enc_len_batch_total, lfr_factor))
+                results.append((text, token, token_int, hyp, timestamp, enc_len_batch_total, lfr_factor))
+
 
         # assert check_return_type(results)
         return results
 
     def generate_hotwords_list(self, hotword_list_or_file):
         # for None
         if hotword_list_or_file is None:
@@ -354,234 +357,14 @@
             hotword_list.append([self.asr_model.sos])
             hotword_str_list.append('<s>')
             logging.info("Hotword list: {}.".format(hotword_str_list))
         else:
             hotword_list = None
         return hotword_list
 
-class Speech2TextExport:
-    """Speech2TextExport class
-
-    """
-
-    def __init__(
-            self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
-            dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            frontend_conf: dict = None,
-            hotword_list_or_file: str = None,
-            **kwargs,
-    ):
-
-        # 1. Build ASR model
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
-        )
-        frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-
-        token_list = asr_model.token_list
-
-
-
-        logging.info(f"Decoding device={device}, dtype={dtype}")
-
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
-        else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        # self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-
-        self.device = device
-        self.dtype = dtype
-        self.nbest = nbest
-        self.frontend = frontend
-
-        model = Paraformer_export(asr_model, onnx=False)
-        self.asr_model = model
-        
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
-    ):
-        """Inference
-
-        Args:
-                speech: Input speech data
-        Returns:
-                text, token, token_int, hyp
-
-        """
-        assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.asr_model.frontend = None
-        else:
-            feats = speech
-            feats_len = speech_lengths
-
-        enc_len_batch_total = feats_len.sum()
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-
-        decoder_outs = self.asr_model(**batch)
-        decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
-        
-        results = []
-        b, n, d = decoder_out.size()
-        for i in range(b):
-            am_scores = decoder_out[i, :ys_pad_lens[i], :]
-
-            yseq = am_scores.argmax(dim=-1)
-            score = am_scores.max(dim=-1)[0]
-            score = torch.sum(score, dim=-1)
-            # pad with mask tokens to ensure compatibility with sos/eos tokens
-            yseq = torch.tensor(
-                yseq.tolist(), device=yseq.device
-            )
-            nbest_hyps = [Hypothesis(yseq=yseq, score=score)]
-
-            for hyp in nbest_hyps:
-                assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-                # remove sos/eos and get results
-                last_pos = -1
-                if isinstance(hyp.yseq, list):
-                    token_int = hyp.yseq[1:last_pos]
-                else:
-                    token_int = hyp.yseq[1:last_pos].tolist()
-
-                # remove blank symbol id, which is assumed to be 0
-                token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
-
-                # Change integer-ids to tokens
-                token = self.converter.ids2tokens(token_int)
-
-                if self.tokenizer is not None:
-                    text = self.tokenizer.tokens2text(token)
-                else:
-                    text = None
-
-                results.append((text, token, token_int, hyp, enc_len_batch_total, lfr_factor))
-
-        return results
-
-
-def inference(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        streaming: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-        timestamp_infer_config: Union[Path, str] = None,
-        timestamp_model_file: Union[Path, str] = None,
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        batch_size=batch_size,
-        beam_size=beam_size,
-        ngpu=ngpu,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        penalty=penalty,
-        log_level=log_level,
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        raw_inputs=raw_inputs,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        key_file=key_file,
-        word_lm_train_config=word_lm_train_config,
-        bpemodel=bpemodel,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        ngram_weight=ngram_weight,
-        nbest=nbest,
-        num_workers=num_workers,
-
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
 
 def inference_modelscope(
         maxlenratio: float,
         minlenratio: float,
         batch_size: int,
         beam_size: int,
@@ -661,18 +444,16 @@
         ctc_weight=ctc_weight,
         lm_weight=lm_weight,
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
         hotword_list_or_file=hotword_list_or_file,
     )
-    if export_mode:
-        speech2text = Speech2TextExport(**speech2text_kwargs)
-    else:
-        speech2text = Speech2Text(**speech2text_kwargs)
+
+    speech2text = Speech2Text(**speech2text_kwargs)
 
     if timestamp_model_file is not None:
         speechtext2timestamp = SpeechText2Timestamp(
             timestamp_cmvn_file=cmvn_file,
             timestamp_model_file=timestamp_model_file,
             timestamp_infer_config=timestamp_infer_config,
         )
@@ -687,15 +468,15 @@
             param_dict: dict = None,
             **kwargs,
     ):
 
         hotword_list_or_file = None
         if param_dict is not None:
             hotword_list_or_file = param_dict.get('hotword')
-        if 'hotword' in kwargs:
+        if 'hotword' in kwargs and kwargs['hotword'] is not None:
             hotword_list_or_file = kwargs['hotword']
         if hotword_list_or_file is not None or 'hotword' in kwargs:
             speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
 
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
@@ -758,15 +539,15 @@
 
             for batch_id in range(_bs):
                 result = [results[batch_id][:-2]]
 
                 key = keys[batch_id]
                 for n, result in zip(range(1, nbest + 1), result):
                     text, token, token_int, hyp = result[0], result[1], result[2], result[3]
-                    timestamp = None if len(result) < 5 else result[4]
+                    timestamp = result[4] if len(result[4]) > 0 else None
                     # conduct timestamp prediction here
                     # timestamp inference requires token length
                     # thus following inference cannot be conducted in batch
                     if timestamp is None and speechtext2timestamp:
                         ts_batch = {}
                         ts_batch['speech'] = batch['speech'][batch_id].unsqueeze(0)
                         ts_batch['speech_lengths'] = torch.tensor([batch['speech_lengths'][batch_id]])
@@ -810,14 +591,265 @@
         if writer is not None:
             ibest_writer["rtf"]["rtf_avf"] = rtf_avg
         return asr_result_list
 
     return _forward
 
 
+def inference_modelscope_vad_punc(
+    maxlenratio: float,
+    minlenratio: float,
+    batch_size: int,
+    beam_size: int,
+    ngpu: int,
+    ctc_weight: float,
+    lm_weight: float,
+    penalty: float,
+    log_level: Union[int, str],
+    # data_path_and_name_and_type,
+    asr_train_config: Optional[str],
+    asr_model_file: Optional[str],
+    cmvn_file: Optional[str] = None,
+    lm_train_config: Optional[str] = None,
+    lm_file: Optional[str] = None,
+    token_type: Optional[str] = None,
+    key_file: Optional[str] = None,
+    word_lm_train_config: Optional[str] = None,
+    bpemodel: Optional[str] = None,
+    allow_variable_data_keys: bool = False,
+    output_dir: Optional[str] = None,
+    dtype: str = "float32",
+    seed: int = 0,
+    ngram_weight: float = 0.9,
+    nbest: int = 1,
+    num_workers: int = 1,
+    vad_infer_config: Optional[str] = None,
+    vad_model_file: Optional[str] = None,
+    vad_cmvn_file: Optional[str] = None,
+    time_stamp_writer: bool = True,
+    punc_infer_config: Optional[str] = None,
+    punc_model_file: Optional[str] = None,
+    outputs_dict: Optional[bool] = True,
+    param_dict: dict = None,
+    **kwargs,
+):
+    assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+    
+    if word_lm_train_config is not None:
+        raise NotImplementedError("Word LM is not implemented")
+    if ngpu > 1:
+        raise NotImplementedError("only single GPU decoding is supported")
+    
+    logging.basicConfig(
+        level=log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+    
+    if param_dict is not None:
+        hotword_list_or_file = param_dict.get('hotword')
+    else:
+        hotword_list_or_file = None
+    
+    if ngpu >= 1 and torch.cuda.is_available():
+        device = "cuda"
+    else:
+        device = "cpu"
+    
+    # 1. Set random-seed
+    set_all_random_seed(seed)
+    
+    # 2. Build speech2vadsegment
+    speech2vadsegment_kwargs = dict(
+        vad_infer_config=vad_infer_config,
+        vad_model_file=vad_model_file,
+        vad_cmvn_file=vad_cmvn_file,
+        device=device,
+        dtype=dtype,
+    )
+    # logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
+    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
+    
+    # 3. Build speech2text
+    speech2text_kwargs = dict(
+        asr_train_config=asr_train_config,
+        asr_model_file=asr_model_file,
+        cmvn_file=cmvn_file,
+        lm_train_config=lm_train_config,
+        lm_file=lm_file,
+        token_type=token_type,
+        bpemodel=bpemodel,
+        device=device,
+        maxlenratio=maxlenratio,
+        minlenratio=minlenratio,
+        dtype=dtype,
+        beam_size=beam_size,
+        ctc_weight=ctc_weight,
+        lm_weight=lm_weight,
+        ngram_weight=ngram_weight,
+        penalty=penalty,
+        nbest=nbest,
+        hotword_list_or_file=hotword_list_or_file,
+    )
+    speech2text = Speech2Text(**speech2text_kwargs)
+    text2punc = None
+    if punc_model_file is not None:
+        text2punc = Text2Punc(punc_infer_config, punc_model_file, device=device, dtype=dtype)
+    
+    if output_dir is not None:
+        writer = DatadirWriter(output_dir)
+        ibest_writer = writer[f"1best_recog"]
+        ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
+    
+    def _forward(data_path_and_name_and_type,
+                 raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+                 output_dir_v2: Optional[str] = None,
+                 fs: dict = None,
+                 param_dict: dict = None,
+                 **kwargs,
+                 ):
+        
+        hotword_list_or_file = None
+        if param_dict is not None:
+            hotword_list_or_file = param_dict.get('hotword')
+        
+        if 'hotword' in kwargs:
+            hotword_list_or_file = kwargs['hotword']
+        
+        if speech2text.hotword_list is None:
+            speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
+        
+        # 3. Build data-iterator
+        if data_path_and_name_and_type is None and raw_inputs is not None:
+            if isinstance(raw_inputs, torch.Tensor):
+                raw_inputs = raw_inputs.numpy()
+            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
+        loader = ASRTask.build_streaming_iterator(
+            data_path_and_name_and_type,
+            dtype=dtype,
+            fs=fs,
+            batch_size=1,
+            key_file=key_file,
+            num_workers=num_workers,
+            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
+            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
+            allow_variable_data_keys=allow_variable_data_keys,
+            inference=True,
+        )
+        
+        if param_dict is not None:
+            use_timestamp = param_dict.get('use_timestamp', True)
+        else:
+            use_timestamp = True
+        
+        finish_count = 0
+        file_count = 1
+        lfr_factor = 6
+        # 7 .Start for-loop
+        asr_result_list = []
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        writer = None
+        if output_path is not None:
+            writer = DatadirWriter(output_path)
+            ibest_writer = writer[f"1best_recog"]
+        
+        for keys, batch in loader:
+            assert isinstance(batch, dict), type(batch)
+            assert all(isinstance(s, str) for s in keys), keys
+            _bs = len(next(iter(batch.values())))
+            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+            
+            vad_results = speech2vadsegment(**batch)
+            _, vadsegments = vad_results[0], vad_results[1][0]
+            
+            speech, speech_lengths = batch["speech"], batch["speech_lengths"]
+            
+            n = len(vadsegments)
+            data_with_index = [(vadsegments[i], i) for i in range(n)]
+            sorted_data = sorted(data_with_index, key=lambda x: x[0][1] - x[0][0])
+            results_sorted = []
+            for j, beg_idx in enumerate(range(0, n, batch_size)):
+                end_idx = min(n, beg_idx + batch_size)
+                speech_j, speech_lengths_j = slice_padding_fbank(speech, speech_lengths, sorted_data[beg_idx:end_idx])
+                
+                batch = {"speech": speech_j, "speech_lengths": speech_lengths_j}
+                batch = to_device(batch, device=device)
+                results = speech2text(**batch)
+                
+                if len(results) < 1:
+                    results = [["", [], [], [], [], [], []]]
+                results_sorted.extend(results)
+            restored_data = [0] * n
+            for j in range(n):
+                index = sorted_data[j][1]
+                restored_data[index] = results_sorted[j]
+            result = ["", [], [], [], [], [], []]
+            for j in range(n):
+                result[0] += restored_data[j][0]
+                result[1] += restored_data[j][1]
+                result[2] += restored_data[j][2]
+                if len(restored_data[j][4]) > 0:
+                    for t in restored_data[j][4]:
+                        t[0] += vadsegments[j][0]
+                        t[1] += vadsegments[j][0]
+                    result[4] += restored_data[j][4]
+                # result = [result[k]+restored_data[j][k] for k in range(len(result[:-2]))]
+            
+            key = keys[0]
+            # result = result_segments[0]
+            text, token, token_int = result[0], result[1], result[2]
+            time_stamp = result[4] if len(result[4]) > 0 else None
+            
+            if use_timestamp and time_stamp is not None:
+                postprocessed_result = postprocess_utils.sentence_postprocess(token, time_stamp)
+            else:
+                postprocessed_result = postprocess_utils.sentence_postprocess(token)
+            text_postprocessed = ""
+            time_stamp_postprocessed = ""
+            text_postprocessed_punc = postprocessed_result
+            if len(postprocessed_result) == 3:
+                text_postprocessed, time_stamp_postprocessed, word_lists = postprocessed_result[0], \
+                                                                           postprocessed_result[1], \
+                                                                           postprocessed_result[2]
+            else:
+                text_postprocessed, word_lists = postprocessed_result[0], postprocessed_result[1]
+            
+            text_postprocessed_punc = text_postprocessed
+            punc_id_list = []
+            if len(word_lists) > 0 and text2punc is not None:
+                text_postprocessed_punc, punc_id_list = text2punc(word_lists, 20)
+            
+            item = {'key': key, 'value': text_postprocessed_punc}
+            if text_postprocessed != "":
+                item['text_postprocessed'] = text_postprocessed
+            if time_stamp_postprocessed != "":
+                item['time_stamp'] = time_stamp_postprocessed
+            
+            item['sentences'] = time_stamp_sentence(punc_id_list, time_stamp_postprocessed, text_postprocessed)
+            
+            asr_result_list.append(item)
+            finish_count += 1
+            # asr_utils.print_progress(finish_count / file_count)
+            if writer is not None:
+                # Write the result to each file
+                ibest_writer["token"][key] = " ".join(token)
+                ibest_writer["token_int"][key] = " ".join(map(str, token_int))
+                ibest_writer["vad"][key] = "{}".format(vadsegments)
+                ibest_writer["text"][key] = " ".join(word_lists)
+                ibest_writer["text_with_punc"][key] = text_postprocessed_punc
+                if time_stamp_postprocessed is not None:
+                    ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
+            
+            logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
+        return asr_result_list
+    
+    return _forward
+
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="ASR Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
@@ -983,22 +1015,13 @@
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     args = parser.parse_args(cmd)
     param_dict = {'hotword': args.hotword}
     kwargs = vars(args)
     kwargs.pop("config", None)
     kwargs['param_dict'] = param_dict
-    inference(**kwargs)
+    inference_pipeline = inference_modelscope(**kwargs)
+    return inference_pipeline(kwargs["data_path_and_name_and_type"], param_dict=param_dict)
 
 
 if __name__ == "__main__":
     main()
-
-    # from modelscope.pipelines import pipeline
-    # from modelscope.utils.constant import Tasks
-    #
-    # inference_16k_pipline = pipeline(
-    #     task=Tasks.auto_speech_recognition,
-    #     model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch')
-    #
-    # rec_result = inference_16k_pipline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
-    # print(rec_result)
```

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_paraformer_streaming.py` & `funasr-0.5.0/funasr/bin/asr_inference_paraformer_streaming.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_paraformer_vad.py` & `funasr-0.5.0/funasr/bin/sa_asr_inference.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,330 @@
-#!/usr/bin/env python3
-
-import json
 import argparse
 import logging
 import sys
-import time
 from pathlib import Path
+from typing import Any
+from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
-from typing import Any
-from typing import List
-import math
+
 import numpy as np
 import torch
 from typeguard import check_argument_types
+from typeguard import check_return_type
 
 from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
-from funasr.modules.beam_search.beam_search import Hypothesis
+from funasr.modules.beam_search.batch_beam_search_online_sim import BatchBeamSearchOnlineSim
+from funasr.modules.beam_search.beam_search_sa_asr import BeamSearch
+from funasr.modules.beam_search.beam_search_sa_asr import Hypothesis
 from funasr.modules.scorers.ctc import CTCPrefixScorer
 from funasr.modules.scorers.length_bonus import LengthBonus
+from funasr.modules.scorers.scorer_interface import BatchScorerInterface
 from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTaskParaformer as ASRTask
+from funasr.tasks.sa_asr import ASRTask
 from funasr.tasks.lm import LMTask
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.token_id_converter import TokenIDConverter
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.tasks.vad import VADTask
-from funasr.bin.punctuation_infer import Text2Punc
-from funasr.bin.asr_inference_paraformer_vad_punc import Speech2Text
-from funasr.bin.asr_inference_paraformer_vad_punc import Speech2VadSegment
+from funasr.tasks.asr import frontend_choices
+
+
+header_colors = '\033[95m'
+end_colors = '\033[0m'
+
+
+class Speech2Text:
+    """Speech2Text class
+
+    Examples:
+        >>> import soundfile
+        >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
+        >>> audio, rate = soundfile.read("speech.wav")
+        >>> speech2text(audio)
+        [(text, token, token_int, hypothesis object), ...]
+
+    """
+
+    def __init__(
+            self,
+            asr_train_config: Union[Path, str] = None,
+            asr_model_file: Union[Path, str] = None,
+            cmvn_file: Union[Path, str] = None,
+            lm_train_config: Union[Path, str] = None,
+            lm_file: Union[Path, str] = None,
+            token_type: str = None,
+            bpemodel: str = None,
+            device: str = "cpu",
+            maxlenratio: float = 0.0,
+            minlenratio: float = 0.0,
+            batch_size: int = 1,
+            dtype: str = "float32",
+            beam_size: int = 20,
+            ctc_weight: float = 0.5,
+            lm_weight: float = 1.0,
+            ngram_weight: float = 0.9,
+            penalty: float = 0.0,
+            nbest: int = 1,
+            streaming: bool = False,
+            frontend_conf: dict = None,
+            **kwargs,
+    ):
+        assert check_argument_types()
+
+        # 1. Build ASR model
+        scorers = {}
+        asr_model, asr_train_args = ASRTask.build_model_from_file(
+            asr_train_config, asr_model_file, cmvn_file, device
+        )
+        frontend = None
+        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
+            if asr_train_args.frontend=='wav_frontend':
+                frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
+            else:
+                frontend_class=frontend_choices.get_class(asr_train_args.frontend)
+                frontend = frontend_class(**asr_train_args.frontend_conf).eval()
+
+        logging.info("asr_model: {}".format(asr_model))
+        logging.info("asr_train_args: {}".format(asr_train_args))
+        asr_model.to(dtype=getattr(torch, dtype)).eval()
+
+        decoder = asr_model.decoder
+
+        ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
+        token_list = asr_model.token_list
+        scorers.update(
+            decoder=decoder,
+            ctc=ctc,
+            length_bonus=LengthBonus(len(token_list)),
+        )
+
+        # 2. Build Language model
+        if lm_train_config is not None:
+            lm, lm_train_args = LMTask.build_model_from_file(
+                lm_train_config, lm_file, None, device
+            )
+            scorers["lm"] = lm.lm
+
+        # 3. Build ngram model
+        # ngram is not supported now
+        ngram = None
+        scorers["ngram"] = ngram
+
+        # 4. Build BeamSearch object
+        # transducer is not supported now
+        beam_search_transducer = None
+
+        weights = dict(
+            decoder=1.0 - ctc_weight,
+            ctc=ctc_weight,
+            lm=lm_weight,
+            ngram=ngram_weight,
+            length_bonus=penalty,
+        )
+        beam_search = BeamSearch(
+            beam_size=beam_size,
+            weights=weights,
+            scorers=scorers,
+            sos=asr_model.sos,
+            eos=asr_model.eos,
+            vocab_size=len(token_list),
+            token_list=token_list,
+            pre_beam_score_key=None if ctc_weight == 1.0 else "full",
+        )
+
+        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
+        if token_type is None:
+            token_type = asr_train_args.token_type
+        if bpemodel is None:
+            bpemodel = asr_train_args.bpemodel
+
+        if token_type is None:
+            tokenizer = None
+        elif token_type == "bpe":
+            if bpemodel is not None:
+                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
+            else:
+                tokenizer = None
+        else:
+            tokenizer = build_tokenizer(token_type=token_type)
+        converter = TokenIDConverter(token_list=token_list)
+        logging.info(f"Text tokenizer: {tokenizer}")
+
+        self.asr_model = asr_model
+        self.asr_train_args = asr_train_args
+        self.converter = converter
+        self.tokenizer = tokenizer
+        self.beam_search = beam_search
+        self.beam_search_transducer = beam_search_transducer
+        self.maxlenratio = maxlenratio
+        self.minlenratio = minlenratio
+        self.device = device
+        self.dtype = dtype
+        self.nbest = nbest
+        self.frontend = frontend
+
+    @torch.no_grad()
+    def __call__(
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray], profile: Union[torch.Tensor, np.ndarray], profile_lengths: Union[torch.Tensor, np.ndarray]
+    ) -> List[
+        Tuple[
+            Optional[str],
+            Optional[str],
+            List[str],
+            List[int],
+            Union[Hypothesis],
+        ]
+    ]:
+        """Inference
+
+        Args:
+            speech: Input speech data
+        Returns:
+            text, text_id, token, token_int, hyp
+
+        """
+        assert check_argument_types()
+
+        # Input as audio signal
+        if isinstance(speech, np.ndarray):
+            speech = torch.tensor(speech)
+
+        if isinstance(profile, np.ndarray):
+            profile = torch.tensor(profile)
+
+        if self.frontend is not None:
+            feats, feats_len = self.frontend.forward(speech, speech_lengths)
+            feats = to_device(feats, device=self.device)
+            feats_len = feats_len.int()
+            self.asr_model.frontend = None
+        else:
+            feats = speech
+            feats_len = speech_lengths
+        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
+        batch = {"speech": feats, "speech_lengths": feats_len}
+
+        # a. To device
+        batch = to_device(batch, device=self.device)
+
+        # b. Forward Encoder
+        asr_enc, _, spk_enc = self.asr_model.encode(**batch)
+        if isinstance(asr_enc, tuple):
+            asr_enc = asr_enc[0]
+        if isinstance(spk_enc, tuple):
+            spk_enc = spk_enc[0]
+        assert len(asr_enc) == 1, len(asr_enc)
+        assert len(spk_enc) == 1, len(spk_enc)
+
+        # c. Passed the encoder result and the beam search
+        nbest_hyps = self.beam_search(
+            asr_enc[0], spk_enc[0], profile[0], maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
+        )
+
+        nbest_hyps = nbest_hyps[: self.nbest]
 
+        results = []
+        for hyp in nbest_hyps:
+            assert isinstance(hyp, (Hypothesis)), type(hyp)
+
+            # remove sos/eos and get results
+            last_pos = -1
+            if isinstance(hyp.yseq, list):
+                token_int = hyp.yseq[1: last_pos]
+            else:
+                token_int = hyp.yseq[1: last_pos].tolist()
+
+            spk_weigths=torch.stack(hyp.spk_weigths, dim=0)
+
+            token_ori = self.converter.ids2tokens(token_int)
+            text_ori = self.tokenizer.tokens2text(token_ori)
+
+            text_ori_spklist = text_ori.split('$')
+            cur_index = 0
+            spk_choose = []
+            for i in range(len(text_ori_spklist)):
+                text_ori_split = text_ori_spklist[i]
+                n = len(text_ori_split)
+                spk_weights_local = spk_weigths[cur_index: cur_index + n]
+                cur_index = cur_index + n + 1
+                spk_weights_local = spk_weights_local.mean(dim=0)
+                spk_choose_local = spk_weights_local.argmax(-1)
+                spk_choose.append(spk_choose_local.item() + 1)
+
+            # remove blank symbol id, which is assumed to be 0
+            token_int = list(filter(lambda x: x != 0, token_int))
+
+            # Change integer-ids to tokens
+            token = self.converter.ids2tokens(token_int)
+
+            if self.tokenizer is not None:
+                text = self.tokenizer.tokens2text(token)
+            else:
+                text = None
+
+            text_spklist = text.split('$')
+            assert len(spk_choose) == len(text_spklist)
+
+            spk_list=[]
+            for i in range(len(text_spklist)):
+                text_split = text_spklist[i]
+                n = len(text_split)
+                spk_list.append(str(spk_choose[i]) * n)
+            
+            text_id = '$'.join(spk_list)
+            
+            assert len(text) == len(text_id)
+
+            results.append((text, text_id, token, token_int, hyp))
+
+        assert check_return_type(results)
+        return results
 
 def inference(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    streaming: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    vad_infer_config: Optional[str] = None,
-    vad_model_file: Optional[str] = None,
-    vad_cmvn_file: Optional[str] = None,
-    time_stamp_writer: bool = False,
-    punc_infer_config: Optional[str] = None,
-    punc_model_file: Optional[str] = None,
-    **kwargs,
+        maxlenratio: float,
+        minlenratio: float,
+        batch_size: int,
+        beam_size: int,
+        ngpu: int,
+        ctc_weight: float,
+        lm_weight: float,
+        penalty: float,
+        log_level: Union[int, str],
+        data_path_and_name_and_type,
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        cmvn_file: Optional[str] = None,
+        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        token_type: Optional[str] = None,
+        key_file: Optional[str] = None,
+        word_lm_train_config: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        streaming: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        ngram_weight: float = 0.9,
+        nbest: int = 1,
+        num_workers: int = 1,
+        mc: bool = False,
+        **kwargs,
 ):
-
     inference_pipeline = inference_modelscope(
         maxlenratio=maxlenratio,
         minlenratio=minlenratio,
         batch_size=batch_size,
         beam_size=beam_size,
         ngpu=ngpu,
         ctc_weight=ctc_weight,
@@ -105,20 +345,15 @@
         streaming=streaming,
         output_dir=output_dir,
         dtype=dtype,
         seed=seed,
         ngram_weight=ngram_weight,
         nbest=nbest,
         num_workers=num_workers,
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        time_stamp_writer=time_stamp_writer,
-        punc_infer_config=punc_infer_config,
-        punc_model_file=punc_model_file,
+        mc=mc,
         **kwargs,
     )
     return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
 def inference_modelscope(
     maxlenratio: float,
     minlenratio: float,
@@ -136,69 +371,50 @@
     lm_train_config: Optional[str] = None,
     lm_file: Optional[str] = None,
     token_type: Optional[str] = None,
     key_file: Optional[str] = None,
     word_lm_train_config: Optional[str] = None,
     bpemodel: Optional[str] = None,
     allow_variable_data_keys: bool = False,
+    streaming: bool = False,
     output_dir: Optional[str] = None,
     dtype: str = "float32",
     seed: int = 0,
     ngram_weight: float = 0.9,
     nbest: int = 1,
     num_workers: int = 1,
-    vad_infer_config: Optional[str] = None,
-    vad_model_file: Optional[str] = None,
-    vad_cmvn_file: Optional[str] = None,
-    time_stamp_writer: bool = True,
-    punc_infer_config: Optional[str] = None,
-    punc_model_file: Optional[str] = None,
-    outputs_dict: Optional[bool] = True,
+    mc: bool = False,
     param_dict: dict = None,
     **kwargs,
 ):
     assert check_argument_types()
-    ncpu = kwargs.get("ncpu", 1)
-    torch.set_num_threads(ncpu)
-    
+    if batch_size > 1:
+        raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
+
+    for handler in logging.root.handlers[:]:
+        logging.root.removeHandler(handler)
     
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-
-    if param_dict is not None:
-        hotword_list_or_file = param_dict.get('hotword')
-    else:
-        hotword_list_or_file = None
     
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
     
     # 1. Set random-seed
     set_all_random_seed(seed)
     
-    # 2. Build speech2vadsegment
-    speech2vadsegment_kwargs = dict(
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        device=device,
-        dtype=dtype,
-    )
-    # logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
-    
-    # 3. Build speech2text
+    # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
         token_type=token_type,
@@ -209,150 +425,97 @@
         dtype=dtype,
         beam_size=beam_size,
         ctc_weight=ctc_weight,
         lm_weight=lm_weight,
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
-        hotword_list_or_file=hotword_list_or_file,
+        streaming=streaming,
     )
+    logging.info("speech2text_kwargs: {}".format(speech2text_kwargs))
     speech2text = Speech2Text(**speech2text_kwargs)
-    text2punc = None
-    if punc_model_file is not None:
-        text2punc = Text2Punc(punc_infer_config, punc_model_file, device=device, dtype=dtype)
-
-    if output_dir is not None:
-        writer = DatadirWriter(output_dir)
-        ibest_writer = writer[f"1best_recog"]
-        ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
     
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
-
-        hotword_list_or_file = None
-        if param_dict is not None:
-            hotword_list_or_file = param_dict.get('hotword')
-
-        if 'hotword' in kwargs:
-            hotword_list_or_file = kwargs['hotword']
-
-        if speech2text.hotword_list is None:
-            speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
-
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
         loader = ASRTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
-            batch_size=1,
+            mc=mc,
+            batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
+            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
+            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-
-        if param_dict is not None:
-            use_timestamp = param_dict.get('use_timestamp', True)
-        else:
-            use_timestamp = True
         
         finish_count = 0
         file_count = 1
-        lfr_factor = 6
         # 7 .Start for-loop
+        # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        writer = None
         if output_path is not None:
             writer = DatadirWriter(output_path)
-            ibest_writer = writer[f"1best_recog"]
-         
+        else:
+            writer = None
+        
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-
-            vad_results = speech2vadsegment(**batch)
-            fbanks, vadsegments = vad_results[0], vad_results[1]
-            for i, segments in enumerate(vadsegments):
-                result_segments = [["", [], [], ]]
-                for j, segment_idx in enumerate(segments):
-                    bed_idx, end_idx = int(segment_idx[0] / 10), int(segment_idx[1] / 10)
-                    segment = fbanks[:, bed_idx:end_idx, :].to(device)
-                    speech_lengths = torch.Tensor([end_idx - bed_idx]).int().to(device)
-                    batch = {"speech": segment, "speech_lengths": speech_lengths, "begin_time": vadsegments[i][j][0],
-                             "end_time": vadsegments[i][j][1]}
-                    results = speech2text(**batch)
-                    if len(results) < 1:
-                        continue
-
-                    result_cur = [results[0][:-2]]
-                    if j == 0:
-                        result_segments = result_cur
-                    else:
-                        result_segments = [[result_segments[0][i] + result_cur[0][i] for i in range(len(result_cur[0]))]]
-                
-                key = keys[0]
-                result = result_segments[0]
-                text, token, token_int = result[0], result[1], result[2]
-                time_stamp = None if len(result) < 4 else result[3]
-               
-                if use_timestamp and time_stamp is not None:
-                    postprocessed_result = postprocess_utils.sentence_postprocess(token, time_stamp)
-                else:
-                    postprocessed_result = postprocess_utils.sentence_postprocess(token)
-                text_postprocessed = ""
-                time_stamp_postprocessed = ""
-                text_postprocessed_punc = postprocessed_result
-                if len(postprocessed_result) == 3:
-                    text_postprocessed, time_stamp_postprocessed, word_lists = postprocessed_result[0], \
-                                                                               postprocessed_result[1], \
-                                                                               postprocessed_result[2]
-                else:
-                    text_postprocessed, word_lists = postprocessed_result[0], postprocessed_result[1]
-                text_postprocessed_punc = text_postprocessed
-                if len(word_lists) > 0 and text2punc is not None:
-                    text_postprocessed_punc, punc_id_list = text2punc(word_lists, 20)
-
-                
-                item = {'key': key, 'value': text_postprocessed_punc}
-                if text_postprocessed != "":
-                    item['text_postprocessed'] = text_postprocessed
-                if time_stamp_postprocessed != "":
-                    item['time_stamp'] = time_stamp_postprocessed
-
-                asr_result_list.append(item)
-                finish_count += 1
-                # asr_utils.print_progress(finish_count / file_count)
+            # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
+            # N-best list of (text, token, token_int, hyp_object)
+            try:
+                results = speech2text(**batch)
+            except TooShortUttError as e:
+                logging.warning(f"Utterance {keys} {e}")
+                hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
+                results = [[" ", ["sil"], [2], hyp]] * nbest
+            
+            # Only supporting batch_size==1
+            key = keys[0]
+            for n, (text, text_id, token, token_int, hyp) in zip(range(1, nbest + 1), results):
+                # Create a directory: outdir/{n}best_recog
                 if writer is not None:
+                    ibest_writer = writer[f"{n}best_recog"]
+                    
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                    ibest_writer["vad"][key] = "{}".format(vadsegments)
-                    ibest_writer["text"][key] = " ".join(word_lists)
-                    ibest_writer["text_with_punc"][key] = text_postprocessed_punc
-                    if time_stamp_postprocessed is not None:
-                        ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
+                    ibest_writer["score"][key] = str(hyp.score)
+                    ibest_writer["text_id"][key] = text_id
                 
-                logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
-
-
+                if text is not None:
+                    text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
+                    item = {'key': key, 'value': text_postprocessed}
+                    asr_result_list.append(item)
+                    finish_count += 1
+                    asr_utils.print_progress(finish_count / file_count)
+                    if writer is not None:
+                        ibest_writer["text"][key] = text
+
+                logging.info("uttid: {}".format(key))
+                logging.info("text predictions: {}".format(text))
+                logging.info("text_id predictions: {}\n".format(text_id))
         return asr_result_list
+    
     return _forward
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="ASR Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
@@ -370,14 +533,20 @@
     parser.add_argument("--output_dir", type=str, required=True)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
+    parser.add_argument(
+        "--gpuid_list",
+        type=str,
+        default="",
+        help="The visible gpus",
+    )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
     parser.add_argument(
         "--dtype",
         default="float32",
         choices=["float16", "float32", "float64"],
         help="Data type",
     )
@@ -391,14 +560,16 @@
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=False,
         action="append",
     )
+    group.add_argument("--raw_inputs", type=list, default=None)
+    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
         "--asr_train_config",
         type=str,
@@ -478,23 +649,14 @@
         type=float,
         default=0.5,
         help="CTC weight in joint decoding",
     )
     group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
     group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
     group.add_argument("--streaming", type=str2bool, default=False)
-    group.add_argument("--time_stamp_writer", type=str2bool, default=False)
-
-    group.add_argument(
-        "--frontend_conf",
-        default=None,
-        help="",
-    )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
 
     group = parser.add_argument_group("Text converter related")
     group.add_argument(
         "--token_type",
         type=str_or_none,
         default=None,
         choices=["char", "bpe", None],
@@ -504,39 +666,15 @@
     group.add_argument(
         "--bpemodel",
         type=str_or_none,
         default=None,
         help="The model path of sentencepiece. "
              "If not given, refers from the training args",
     )
-    group.add_argument(
-        "--vad_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--vad_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
-    group.add_argument(
-        "--vad_cmvn_file",
-        type=str,
-        help="vad, Global cmvn file",
-    )
-    group.add_argument(
-        "--punc_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--punc_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
+
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     args = parser.parse_args(cmd)
```

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_paraformer_vad_punc.py` & `funasr-0.5.0/funasr/bin/asr_inference_uniasr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,56 @@
 #!/usr/bin/env python3
-
-import json
 import argparse
 import logging
 import sys
-import time
-import os
-import codecs
-import tempfile
-import requests
 from pathlib import Path
+from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
 from typing import Any
-from typing import List
-import math
-import copy
+
 import numpy as np
 import torch
 from typeguard import check_argument_types
+from typeguard import check_return_type
 
 from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
+from funasr.modules.beam_search.beam_search import BeamSearchScama as BeamSearch
 from funasr.modules.beam_search.beam_search import Hypothesis
 from funasr.modules.scorers.ctc import CTCPrefixScorer
 from funasr.modules.scorers.length_bonus import LengthBonus
 from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTaskParaformer as ASRTask
+from funasr.tasks.asr import ASRTaskUniASR as ASRTask
 from funasr.tasks.lm import LMTask
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.token_id_converter import TokenIDConverter
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.tasks.vad import VADTask
-from funasr.bin.vad_inference import Speech2VadSegment
-from funasr.utils.timestamp_tools import time_stamp_sentence, ts_prediction_lfr6_standard
-from funasr.bin.punctuation_infer import Text2Punc
-from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
-
 
-header_colors = '\033[95m'
-end_colors = '\033[0m'
 
 
 class Speech2Text:
     """Speech2Text class
 
     Examples:
-            >>> import soundfile
-            >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
-            >>> audio, rate = soundfile.read("speech.wav")
-            >>> speech2text(audio)
-            [(text, token, token_int, hypothesis object), ...]
+        >>> import soundfile
+        >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
+        >>> audio, rate = soundfile.read("speech.wav")
+        >>> speech2text(audio)
+        [(text, token, token_int, hypothesis object), ...]
 
     """
 
     def __init__(
             self,
             asr_train_config: Union[Path, str] = None,
             asr_model_file: Union[Path, str] = None,
@@ -80,40 +65,46 @@
             dtype: str = "float32",
             beam_size: int = 20,
             ctc_weight: float = 0.5,
             lm_weight: float = 1.0,
             ngram_weight: float = 0.9,
             penalty: float = 0.0,
             nbest: int = 1,
+            token_num_relax: int = 1,
+            decoding_ind: int = 0,
+            decoding_mode: str = "model1",
             frontend_conf: dict = None,
-            hotword_list_or_file: str = None,
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file=cmvn_file, device=device
+            asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
-        if asr_model.frontend is not None and asr_train_args.frontend_conf is not None:
+        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
 
-        # logging.info("asr_model: {}".format(asr_model))
-        # logging.info("asr_train_args: {}".format(asr_train_args))
+        logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
+        if decoding_mode == "model1":
+            decoder = asr_model.decoder
+        else:
+            decoder = asr_model.decoder2
 
         if asr_model.ctc != None:
             ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
             scorers.update(
                 ctc=ctc
             )
         token_list = asr_model.token_list
         scorers.update(
+            decoder=decoder,
             length_bonus=LengthBonus(len(token_list)),
         )
 
         # 2. Build Language model
         if lm_train_config is not None:
             lm, lm_train_args = LMTask.build_model_from_file(
                 lm_train_config, lm_file, device
@@ -147,15 +138,15 @@
             pre_beam_score_key=None if ctc_weight == 1.0 else "full",
         )
 
         beam_search.to(device=device, dtype=getattr(torch, dtype)).eval()
         for scorer in scorers.values():
             if isinstance(scorer, torch.nn.Module):
                 scorer.to(device=device, dtype=getattr(torch, dtype)).eval()
-
+        # logging.info(f"Beam_search: {beam_search}")
         logging.info(f"Decoding device={device}, dtype={dtype}")
 
         # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
         if token_type is None:
             token_type = asr_train_args.token_type
         if bpemodel is None:
             bpemodel = asr_train_args.bpemodel
@@ -172,206 +163,115 @@
         converter = TokenIDConverter(token_list=token_list)
         logging.info(f"Text tokenizer: {tokenizer}")
 
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
-
-        # 6. [Optional] Build hotword list from str, local file or url
-        self.hotword_list = None
-        self.hotword_list = self.generate_hotwords_list(hotword_list_or_file)
-
-        is_use_lm = lm_weight != 0.0 and lm_file is not None
-        if (ctc_weight == 0.0 or asr_model.ctc == None) and not is_use_lm:
-            beam_search = None
         self.beam_search = beam_search
-        logging.info(f"Beam_search: {self.beam_search}")
         self.beam_search_transducer = beam_search_transducer
         self.maxlenratio = maxlenratio
         self.minlenratio = minlenratio
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
+        self.token_num_relax = token_num_relax
+        self.decoding_ind = decoding_ind
+        self.decoding_mode = decoding_mode
         self.frontend = frontend
-        self.encoder_downsampling_factor = 1
-        if asr_train_args.encoder_conf["input_layer"] == "conv2d":
-            self.encoder_downsampling_factor = 4
 
     @torch.no_grad()
     def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            begin_time: int = 0, end_time: int = None,
-    ):
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
+    ) -> List[
+        Tuple[
+            Optional[str],
+            List[str],
+            List[int],
+            Union[Hypothesis],
+        ]
+    ]:
         """Inference
 
         Args:
-                speech: Input speech data
+            speech: Input speech data
         Returns:
-                text, token, token_int, hyp
+            text, token, token_int, hyp
 
         """
         assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
-            # feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            # fbanks, fbanks_len = self.frontend.forward_fbank(speech, speech_lengths)
-            feats, feats_len = self.frontend.forward_lfr_cmvn(speech, speech_lengths)
+            feats, feats_len = self.frontend.forward(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
             feats_len = feats_len.int()
             self.asr_model.frontend = None
         else:
             feats = speech
             feats_len = speech_lengths
         lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
+        feats_raw = feats.clone().to(self.device)
         batch = {"speech": feats, "speech_lengths": feats_len}
 
         # a. To device
         batch = to_device(batch, device=self.device)
-
         # b. Forward Encoder
-        enc, enc_len = self.asr_model.encode(**batch)
+        _, enc, enc_len = self.asr_model.encode(**batch, ind=self.decoding_ind)
         if isinstance(enc, tuple):
             enc = enc[0]
-        # assert len(enc) == 1, len(enc)
-        enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
-
-        predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
-        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
-                                                                        predictor_outs[2], predictor_outs[3]
-        pre_token_length = pre_token_length.round().long()
-        if torch.max(pre_token_length) < 1:
-            return []
-
-        if not isinstance(self.asr_model, ContextualParaformer):
-            if self.hotword_list:
-                logging.warning("Hotword is given but asr model is not a ContextualParaformer.")
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length)
-            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
+        assert len(enc) == 1, len(enc)
+        if self.decoding_mode == "model1":
+            predictor_outs = self.asr_model.calc_predictor_mask(enc, enc_len)
         else:
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length, hw_list=self.hotword_list)
-            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
+            enc, enc_len = self.asr_model.encode2(enc, enc_len, feats_raw, feats_len, ind=self.decoding_ind)
+            predictor_outs = self.asr_model.calc_predictor_mask2(enc, enc_len)
+
+        scama_mask = predictor_outs[4]
+        pre_token_length = predictor_outs[1]
+        pre_acoustic_embeds = predictor_outs[0]
+        maxlen = pre_token_length.sum().item() + self.token_num_relax
+        minlen = max(0, pre_token_length.sum().item() - self.token_num_relax)
+        # c. Passed the encoder result and the beam search
+        nbest_hyps = self.beam_search(
+            x=enc[0], scama_mask=scama_mask, pre_acoustic_embeds=pre_acoustic_embeds, maxlenratio=self.maxlenratio,
+            minlenratio=self.minlenratio, maxlen=int(maxlen), minlen=int(minlen),
+        )
 
-        if isinstance(self.asr_model, BiCifParaformer):
-            _, _, us_alphas, us_peaks = self.asr_model.calc_predictor_timestamp(enc, enc_len,
-                                                                                   pre_token_length)  # test no bias cif2
+        nbest_hyps = nbest_hyps[: self.nbest]
 
         results = []
-        b, n, d = decoder_out.size()
-        for i in range(b):
-            x = enc[i, :enc_len[i], :]
-            am_scores = decoder_out[i, :pre_token_length[i], :]
-            if self.beam_search is not None:
-                nbest_hyps = self.beam_search(
-                    x=x, am_scores=am_scores, maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
-                )
+        for hyp in nbest_hyps:
+            assert isinstance(hyp, (Hypothesis)), type(hyp)
 
-                nbest_hyps = nbest_hyps[: self.nbest]
+            # remove sos/eos and get results
+            last_pos = -1
+            if isinstance(hyp.yseq, list):
+                token_int = hyp.yseq[1:last_pos]
             else:
-                yseq = am_scores.argmax(dim=-1)
-                score = am_scores.max(dim=-1)[0]
-                score = torch.sum(score, dim=-1)
-                # pad with mask tokens to ensure compatibility with sos/eos tokens
-                yseq = torch.tensor(
-                    [self.asr_model.sos] + yseq.tolist() + [self.asr_model.eos], device=yseq.device
-                )
-                nbest_hyps = [Hypothesis(yseq=yseq, score=score)]
-
-            for hyp in nbest_hyps:
-                assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-                # remove sos/eos and get results
-                last_pos = -1
-                if isinstance(hyp.yseq, list):
-                    token_int = hyp.yseq[1:last_pos]
-                else:
-                    token_int = hyp.yseq[1:last_pos].tolist()
-
-                # remove blank symbol id, which is assumed to be 0
-                token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
-                if len(token_int) == 0:
-                    continue
-
-                # Change integer-ids to tokens
-                token = self.converter.ids2tokens(token_int)
-
-                if self.tokenizer is not None:
-                    text = self.tokenizer.tokens2text(token)
-                else:
-                    text = None
-
-                if isinstance(self.asr_model, BiCifParaformer):
-                    _, timestamp = ts_prediction_lfr6_standard(us_alphas[i], 
-                                                            us_peaks[i], 
-                                                            copy.copy(token), 
-                                                            vad_offset=begin_time)
-                    results.append((text, token, token_int, timestamp, enc_len_batch_total, lfr_factor))
-                else:
-                    results.append((text, token, token_int, enc_len_batch_total, lfr_factor))
+                token_int = hyp.yseq[1:last_pos].tolist()
 
-        # assert check_return_type(results)
-        return results
+            # remove blank symbol id, which is assumed to be 0
+            token_int = list(filter(lambda x: x != 0, token_int))
 
-    def generate_hotwords_list(self, hotword_list_or_file):
-        # for None
-        if hotword_list_or_file is None:
-            hotword_list = None
-        # for local txt inputs
-        elif os.path.exists(hotword_list_or_file) and hotword_list_or_file.endswith('.txt'):
-            logging.info("Attempting to parse hotwords from local txt...")
-            hotword_list = []
-            hotword_str_list = []
-            with codecs.open(hotword_list_or_file, 'r') as fin:
-                for line in fin.readlines():
-                    hw = line.strip()
-                    hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-                hotword_list.append([self.asr_model.sos])
-                hotword_str_list.append('<s>')
-            logging.info("Initialized hotword list from file: {}, hotword list: {}."
-                         .format(hotword_list_or_file, hotword_str_list))
-        # for url, download and generate txt
-        elif hotword_list_or_file.startswith('http'):
-            logging.info("Attempting to parse hotwords from url...")
-            work_dir = tempfile.TemporaryDirectory().name
-            if not os.path.exists(work_dir):
-                os.makedirs(work_dir)
-            text_file_path = os.path.join(work_dir, os.path.basename(hotword_list_or_file))
-            local_file = requests.get(hotword_list_or_file)
-            open(text_file_path, "wb").write(local_file.content)
-            hotword_list_or_file = text_file_path
-            hotword_list = []
-            hotword_str_list = []
-            with codecs.open(hotword_list_or_file, 'r') as fin:
-                for line in fin.readlines():
-                    hw = line.strip()
-                    hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-                hotword_list.append([self.asr_model.sos])
-                hotword_str_list.append('<s>')
-            logging.info("Initialized hotword list from file: {}, hotword list: {}."
-                         .format(hotword_list_or_file, hotword_str_list))
-        # for text str input
-        elif not hotword_list_or_file.endswith('.txt'):
-            logging.info("Attempting to parse hotwords as str...")
-            hotword_list = []
-            hotword_str_list = []
-            for hw in hotword_list_or_file.strip().split():
-                hotword_str_list.append(hw)
-                hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-            hotword_list.append([self.asr_model.sos])
-            hotword_str_list.append('<s>')
-            logging.info("Hotword list: {}.".format(hotword_str_list))
-        else:
-            hotword_list = None
-        return hotword_list
+            # Change integer-ids to tokens
+            token = self.converter.ids2tokens(token_int)
+            token = list(filter(lambda x: x != "<gbg>", token))
+
+            if self.tokenizer is not None:
+                text = self.tokenizer.tokens2text(token)
+            else:
+                text = None
+            results.append((text, token, token_int, hyp))
+
+        assert check_return_type(results)
+        return results
 
 
 def inference(
         maxlenratio: float,
         minlenratio: float,
         batch_size: int,
         beam_size: int,
@@ -379,14 +279,15 @@
         ctc_weight: float,
         lm_weight: float,
         penalty: float,
         log_level: Union[int, str],
         data_path_and_name_and_type,
         asr_train_config: Optional[str],
         asr_model_file: Optional[str],
+        ngram_file: Optional[str] = None,
         cmvn_file: Optional[str] = None,
         raw_inputs: Union[np.ndarray, torch.Tensor] = None,
         lm_train_config: Optional[str] = None,
         lm_file: Optional[str] = None,
         token_type: Optional[str] = None,
         key_file: Optional[str] = None,
         word_lm_train_config: Optional[str] = None,
@@ -395,20 +296,17 @@
         streaming: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
-        vad_infer_config: Optional[str] = None,
-        vad_model_file: Optional[str] = None,
-        vad_cmvn_file: Optional[str] = None,
-        time_stamp_writer: bool = False,
-        punc_infer_config: Optional[str] = None,
-        punc_model_file: Optional[str] = None,
+        token_num_relax: int = 1,
+        decoding_ind: int = 0,
+        decoding_mode: str = "model1",
         **kwargs,
 ):
     inference_pipeline = inference_modelscope(
         maxlenratio=maxlenratio,
         minlenratio=minlenratio,
         batch_size=batch_size,
         beam_size=beam_size,
@@ -429,22 +327,20 @@
         bpemodel=bpemodel,
         allow_variable_data_keys=allow_variable_data_keys,
         streaming=streaming,
         output_dir=output_dir,
         dtype=dtype,
         seed=seed,
         ngram_weight=ngram_weight,
+        ngram_file=ngram_file,
         nbest=nbest,
         num_workers=num_workers,
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        time_stamp_writer=time_stamp_writer,
-        punc_infer_config=punc_infer_config,
-        punc_model_file=punc_model_file,
+        token_num_relax=token_num_relax,
+        decoding_ind=decoding_ind,
+        decoding_mode=decoding_mode,
         **kwargs,
     )
     return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
 
 def inference_modelscope(
         maxlenratio: float,
@@ -455,238 +351,178 @@
         ctc_weight: float,
         lm_weight: float,
         penalty: float,
         log_level: Union[int, str],
         # data_path_and_name_and_type,
         asr_train_config: Optional[str],
         asr_model_file: Optional[str],
+        ngram_file: Optional[str] = None,
         cmvn_file: Optional[str] = None,
+        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
         lm_train_config: Optional[str] = None,
         lm_file: Optional[str] = None,
         token_type: Optional[str] = None,
         key_file: Optional[str] = None,
         word_lm_train_config: Optional[str] = None,
         bpemodel: Optional[str] = None,
         allow_variable_data_keys: bool = False,
+        streaming: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
-        vad_infer_config: Optional[str] = None,
-        vad_model_file: Optional[str] = None,
-        vad_cmvn_file: Optional[str] = None,
-        time_stamp_writer: bool = True,
-        punc_infer_config: Optional[str] = None,
-        punc_model_file: Optional[str] = None,
-        outputs_dict: Optional[bool] = True,
+        token_num_relax: int = 1,
+        decoding_ind: int = 0,
+        decoding_mode: str = "model1",
         param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
-
+    if batch_size > 1:
+        raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
-    if param_dict is not None:
-        hotword_list_or_file = param_dict.get('hotword')
-    else:
-        hotword_list_or_file = None
-
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
+    
+    if param_dict is not None and "decoding_model" in param_dict:
+        if param_dict["decoding_model"] == "fast":
+            decoding_ind = 0
+            decoding_mode = "model1"
+        elif param_dict["decoding_model"] == "normal":
+            decoding_ind = 0
+            decoding_mode = "model2"
+        elif param_dict["decoding_model"] == "offline":
+            decoding_ind = 1
+            decoding_mode = "model2"
+        else:
+            raise NotImplementedError("unsupported decoding model {}".format(param_dict["decoding_model"]))
 
     # 1. Set random-seed
     set_all_random_seed(seed)
 
-    # 2. Build speech2vadsegment
-    speech2vadsegment_kwargs = dict(
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        device=device,
-        dtype=dtype,
-    )
-    # logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
-
-    # 3. Build speech2text
+    # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
+        ngram_file=ngram_file,
         token_type=token_type,
         bpemodel=bpemodel,
         device=device,
         maxlenratio=maxlenratio,
         minlenratio=minlenratio,
         dtype=dtype,
         beam_size=beam_size,
         ctc_weight=ctc_weight,
         lm_weight=lm_weight,
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
-        hotword_list_or_file=hotword_list_or_file,
+        streaming=streaming,
+        token_num_relax=token_num_relax,
+        decoding_ind=decoding_ind,
+        decoding_mode=decoding_mode,
     )
     speech2text = Speech2Text(**speech2text_kwargs)
-    text2punc = None
-    if punc_model_file is not None:
-        text2punc = Text2Punc(punc_infer_config, punc_model_file, device=device, dtype=dtype)
-
-    if output_dir is not None:
-        writer = DatadirWriter(output_dir)
-        ibest_writer = writer[f"1best_recog"]
-        ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
-
+    
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
-
-        hotword_list_or_file = None
-        if param_dict is not None:
-            hotword_list_or_file = param_dict.get('hotword')
-
-        if 'hotword' in kwargs:
-            hotword_list_or_file = kwargs['hotword']
-
-        if speech2text.hotword_list is None:
-            speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
-
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
         loader = ASRTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
-            batch_size=1,
+            batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
+            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
+            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-
-        if param_dict is not None:
-            use_timestamp = param_dict.get('use_timestamp', True)
-        else:
-            use_timestamp = True
-
+    
         finish_count = 0
         file_count = 1
-        lfr_factor = 6
         # 7 .Start for-loop
+        # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        writer = None
         if output_path is not None:
             writer = DatadirWriter(output_path)
-            ibest_writer = writer[f"1best_recog"]
-
+        else:
+            writer = None
+    
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-
-            vad_results = speech2vadsegment(**batch)
-            fbanks, vadsegments = vad_results[0], vad_results[1]
-            for i, segments in enumerate(vadsegments):
-                result_segments = [["", [], [], []]]
-                for j, segment_idx in enumerate(segments):
-                    bed_idx, end_idx = int(segment_idx[0] / 10), int(segment_idx[1] / 10)
-                    segment = fbanks[:, bed_idx:end_idx, :].to(device)
-                    speech_lengths = torch.Tensor([end_idx - bed_idx]).int().to(device)
-                    batch = {"speech": segment, "speech_lengths": speech_lengths, "begin_time": vadsegments[i][j][0],
-                             "end_time": vadsegments[i][j][1]}
-                    results = speech2text(**batch)
-                    if len(results) < 1:
-                        continue
-
-                    result_cur = [results[0][:-2]]
-                    if j == 0:
-                        result_segments = result_cur
-                    else:
-                        result_segments = [
-                            [result_segments[0][i] + result_cur[0][i] for i in range(len(result_cur[0]))]]
-
-                key = keys[0]
-                result = result_segments[0]
-                text, token, token_int = result[0], result[1], result[2]
-                time_stamp = None if len(result) < 4 else result[3]
-
-
-                if use_timestamp and time_stamp is not None: 
-                    postprocessed_result = postprocess_utils.sentence_postprocess(token, time_stamp)
-                else:
-                    postprocessed_result = postprocess_utils.sentence_postprocess(token)
-                text_postprocessed = ""
-                time_stamp_postprocessed = ""
-                text_postprocessed_punc = postprocessed_result
-                if len(postprocessed_result) == 3:
-                    text_postprocessed, time_stamp_postprocessed, word_lists = postprocessed_result[0], \
-                                                                               postprocessed_result[1], \
-                                                                               postprocessed_result[2]
-                else:
-                    text_postprocessed, word_lists = postprocessed_result[0], postprocessed_result[1]
-
-                text_postprocessed_punc = text_postprocessed
-                punc_id_list = []
-                if len(word_lists) > 0 and text2punc is not None:
-                    text_postprocessed_punc, punc_id_list = text2punc(word_lists, 20)
-
-                item = {'key': key, 'value': text_postprocessed_punc}
-                if text_postprocessed != "":
-                    item['text_postprocessed'] = text_postprocessed
-                if time_stamp_postprocessed != "":
-                    item['time_stamp'] = time_stamp_postprocessed
-
-                item['sentences'] = time_stamp_sentence(punc_id_list, time_stamp_postprocessed, text_postprocessed)
-
-                asr_result_list.append(item)
-                finish_count += 1
-                # asr_utils.print_progress(finish_count / file_count)
+            #batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
+    
+            # N-best list of (text, token, token_int, hyp_object)
+            try:
+                results = speech2text(**batch)
+            except TooShortUttError as e:
+                logging.warning(f"Utterance {keys} {e}")
+                hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
+                results = [[" ", ["sil"], [2], hyp]] * nbest
+    
+            # Only supporting batch_size==1
+            key = keys[0]
+            logging.info(f"Utterance: {key}")
+            for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
+                # Create a directory: outdir/{n}best_recog
                 if writer is not None:
+                    ibest_writer = writer[f"{n}best_recog"]
+    
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
-                    ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                    ibest_writer["vad"][key] = "{}".format(vadsegments)
-                    ibest_writer["text"][key] = " ".join(word_lists)
-                    ibest_writer["text_with_punc"][key] = text_postprocessed_punc
-                    if time_stamp_postprocessed is not None:
-                        ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
-
-                logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
+                    # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
+                    ibest_writer["score"][key] = str(hyp.score)
+    
+                if text is not None:
+                    text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
+                    item = {'key': key, 'value': text_postprocessed}
+                    asr_result_list.append(item)
+                    finish_count += 1
+                    asr_utils.print_progress(finish_count / file_count)
+                    if writer is not None:
+                        ibest_writer["text"][key] = " ".join(word_lists)
         return asr_result_list
-
+    
     return _forward
 
 
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="ASR Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
@@ -723,14 +559,16 @@
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=False,
         action="append",
     )
+    group.add_argument("--raw_inputs", type=list, default=None)
+    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
         "--asr_train_config",
         type=str,
@@ -810,23 +648,14 @@
         type=float,
         default=0.5,
         help="CTC weight in joint decoding",
     )
     group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
     group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
     group.add_argument("--streaming", type=str2bool, default=False)
-    group.add_argument("--time_stamp_writer", type=str2bool, default=False)
-
-    group.add_argument(
-        "--frontend_conf",
-        default=None,
-        help="",
-    )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
 
     group = parser.add_argument_group("Text converter related")
     group.add_argument(
         "--token_type",
         type=str_or_none,
         default=None,
         choices=["char", "bpe", None],
@@ -836,38 +665,22 @@
     group.add_argument(
         "--bpemodel",
         type=str_or_none,
         default=None,
         help="The model path of sentencepiece. "
              "If not given, refers from the training args",
     )
+    group.add_argument("--token_num_relax", type=int, default=1, help="")
+    group.add_argument("--decoding_ind", type=int, default=0, help="")
+    group.add_argument("--decoding_mode", type=str, default="model1", help="")
     group.add_argument(
-        "--vad_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--vad_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
-    group.add_argument(
-        "--vad_cmvn_file",
-        type=str,
-        help="vad, Global cmvn file",
-    )
-    group.add_argument(
-        "--punc_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--punc_model_file",
-        type=str,
-        help="VAD model parameter file",
+        "--ctc_weight2",
+        type=float,
+        default=0.0,
+        help="CTC weight in joint decoding",
     )
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
```

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_rnnt.py` & `funasr-0.5.0/funasr/bin/asr_inference_rnnt.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,26 +184,23 @@
         if not simu_streaming or chunk_size == 0:
             self.simu_streaming = False
             self.asr_model.encoder.dynamic_chunk_training = False
 
         self.frontend = frontend
         self.window_size = self.chunk_size + self.right_context
         
-        self._ctx = self.asr_model.encoder.get_encoder_input_size(
-            self.window_size
-        )
+        if self.streaming:
+            self._ctx = self.asr_model.encoder.get_encoder_input_size(
+                self.window_size
+            )
        
-        #self.last_chunk_length = (
-        #    self.asr_model.encoder.embed.min_frame_length + self.right_context + 1
-        #) * self.hop_length
-
-        self.last_chunk_length = (
-            self.asr_model.encoder.embed.min_frame_length + self.right_context + 1
-        )
-        self.reset_inference_cache()
+            self.last_chunk_length = (
+                self.asr_model.encoder.embed.min_frame_length + self.right_context + 1
+            )
+            self.reset_inference_cache()
 
     def reset_inference_cache(self) -> None:
         """Reset Speech2Text parameters."""
         self.frontend_cache = None
 
         self.asr_model.encoder.reset_streaming_cache(
             self.left_context, device=self.device
```

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_uniasr.py` & `funasr-0.5.0/funasr/bin/sond_inference.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,551 +1,497 @@
 #!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
 import argparse
 import logging
+import os
 import sys
 from pathlib import Path
+from typing import Any
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
-from typing import Dict
-from typing import Any
 
+from collections import OrderedDict
 import numpy as np
+import soundfile
 import torch
+from torch.nn import functional as F
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.beam_search import BeamSearchScama as BeamSearch
-from funasr.modules.beam_search.beam_search import Hypothesis
-from funasr.modules.scorers.ctc import CTCPrefixScorer
-from funasr.modules.scorers.length_bonus import LengthBonus
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTaskUniASR as ASRTask
-from funasr.tasks.lm import LMTask
-from funasr.text.build_tokenizer import build_tokenizer
-from funasr.text.token_id_converter import TokenIDConverter
+from funasr.utils.cli_utils import get_commandline_args
+from funasr.tasks.diar import DiarTask
+from funasr.tasks.asr import ASRTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend
+from scipy.ndimage import median_filter
+from funasr.utils.misc import statistic_model_parameters
+from funasr.datasets.iterable_dataset import load_bytes
 
 
-
-class Speech2Text:
-    """Speech2Text class
+class Speech2Diarization:
+    """Speech2Xvector class
 
     Examples:
         >>> import soundfile
-        >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
+        >>> import numpy as np
+        >>> speech2diar = Speech2Diarization("diar_sond_config.yml", "diar_sond.pb")
+        >>> profile = np.load("profiles.npy")
         >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2text(audio)
-        [(text, token, token_int, hypothesis object), ...]
+        >>> speech2diar(audio, profile)
+        {"spk1": [(int, int), ...], ...}
 
     """
 
     def __init__(
             self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
+            diar_train_config: Union[Path, str] = None,
+            diar_model_file: Union[Path, str] = None,
+            device: Union[str, torch.device] = "cpu",
+            batch_size: int = 1,
             dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            token_num_relax: int = 1,
-            decoding_ind: int = 0,
-            decoding_mode: str = "model1",
-            frontend_conf: dict = None,
-            **kwargs,
+            streaming: bool = False,
+            smooth_size: int = 83,
+            dur_threshold: float = 10,
     ):
         assert check_argument_types()
 
-        # 1. Build ASR model
-        scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
-        )
-        frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-        if decoding_mode == "model1":
-            decoder = asr_model.decoder
-        else:
-            decoder = asr_model.decoder2
-
-        if asr_model.ctc != None:
-            ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
-            scorers.update(
-                ctc=ctc
-            )
-        token_list = asr_model.token_list
-        scorers.update(
-            decoder=decoder,
-            length_bonus=LengthBonus(len(token_list)),
+        # TODO: 1. Build Diarization model
+        diar_model, diar_train_args = DiarTask.build_model_from_file(
+            config_file=diar_train_config,
+            model_file=diar_model_file,
+            device=device
         )
-
-        # 2. Build Language model
-        if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
-            )
-            scorers["lm"] = lm.lm
-
-        # 3. Build ngram model
-        # ngram is not supported now
-        ngram = None
-        scorers["ngram"] = ngram
-
-        # 4. Build BeamSearch object
-        # transducer is not supported now
-        beam_search_transducer = None
-
-        weights = dict(
-            decoder=1.0 - ctc_weight,
-            ctc=ctc_weight,
-            lm=lm_weight,
-            ngram=ngram_weight,
-            length_bonus=penalty,
-        )
-        beam_search = BeamSearch(
-            beam_size=beam_size,
-            weights=weights,
-            scorers=scorers,
-            sos=asr_model.sos,
-            eos=asr_model.eos,
-            vocab_size=len(token_list),
-            token_list=token_list,
-            pre_beam_score_key=None if ctc_weight == 1.0 else "full",
-        )
-
-        beam_search.to(device=device, dtype=getattr(torch, dtype)).eval()
-        for scorer in scorers.values():
-            if isinstance(scorer, torch.nn.Module):
-                scorer.to(device=device, dtype=getattr(torch, dtype)).eval()
-        # logging.info(f"Beam_search: {beam_search}")
-        logging.info(f"Decoding device={device}, dtype={dtype}")
-
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
-        else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-        self.beam_search = beam_search
-        self.beam_search_transducer = beam_search_transducer
-        self.maxlenratio = maxlenratio
-        self.minlenratio = minlenratio
+        logging.info("diar_model: {}".format(diar_model))
+        logging.info("model parameter number: {}".format(statistic_model_parameters(diar_model)))
+        logging.info("diar_train_args: {}".format(diar_train_args))
+        diar_model.to(dtype=getattr(torch, dtype)).eval()
+
+        self.diar_model = diar_model
+        self.diar_train_args = diar_train_args
+        self.token_list = diar_train_args.token_list
+        self.smooth_size = smooth_size
+        self.dur_threshold = dur_threshold
         self.device = device
         self.dtype = dtype
-        self.nbest = nbest
-        self.token_num_relax = token_num_relax
-        self.decoding_ind = decoding_ind
-        self.decoding_mode = decoding_mode
-        self.frontend = frontend
+
+    def smooth_multi_labels(self, multi_label):
+        multi_label = median_filter(multi_label, (self.smooth_size, 1), mode="constant", cval=0.0).astype(int)
+        return multi_label
+
+    @staticmethod
+    def calc_spk_turns(label_arr, spk_list):
+        turn_list = []
+        length = label_arr.shape[0]
+        n_spk = label_arr.shape[1]
+        for k in range(n_spk):
+            if spk_list[k] == "None":
+                continue
+            in_utt = False
+            start = 0
+            for i in range(length):
+                if label_arr[i, k] == 1 and in_utt is False:
+                    start = i
+                    in_utt = True
+                if label_arr[i, k] == 0 and in_utt is True:
+                    turn_list.append([spk_list[k], start, i - start])
+                    in_utt = False
+            if in_utt:
+                turn_list.append([spk_list[k], start, length - start])
+        return turn_list
+
+    @staticmethod
+    def seq2arr(seq, vec_dim=8):
+        def int2vec(x, vec_dim=8, dtype=np.int):
+            b = ('{:0' + str(vec_dim) + 'b}').format(x)
+            # little-endian order: lower bit first
+            return (np.array(list(b)[::-1]) == '1').astype(dtype)
+
+        # process oov
+        seq = np.array([int(x) for x in seq])
+        new_seq = []
+        for i, x in enumerate(seq):
+            if x < 2 ** vec_dim:
+                new_seq.append(x)
+            else:
+                idx_list = np.where(seq < 2 ** vec_dim)[0]
+                idx = np.abs(idx_list - i).argmin()
+                new_seq.append(seq[idx_list[idx]])
+        return np.row_stack([int2vec(x, vec_dim) for x in new_seq])
+
+    def post_processing(self, raw_logits: torch.Tensor, spk_num: int, output_format: str = "speaker_turn"):
+        logits_idx = raw_logits.argmax(-1)  # B, T, vocab_size -> B, T
+        # upsampling outputs to match inputs
+        ut = logits_idx.shape[1] * self.diar_model.encoder.time_ds_ratio
+        logits_idx = F.upsample(
+            logits_idx.unsqueeze(1).float(),
+            size=(ut, ),
+            mode="nearest",
+        ).squeeze(1).long()
+        logits_idx = logits_idx[0].tolist()
+        pse_labels = [self.token_list[x] for x in logits_idx]
+        if output_format == "pse_labels":
+            return pse_labels, None
+
+        multi_labels = self.seq2arr(pse_labels, spk_num)[:, :spk_num]  # remove padding speakers
+        multi_labels = self.smooth_multi_labels(multi_labels)
+        if output_format == "binary_labels":
+            return multi_labels, None
+
+        spk_list = ["spk{}".format(i + 1) for i in range(spk_num)]
+        spk_turns = self.calc_spk_turns(multi_labels, spk_list)
+        results = OrderedDict()
+        for spk, st, dur in spk_turns:
+            if spk not in results:
+                results[spk] = []
+            if dur > self.dur_threshold:
+                results[spk].append((st, st+dur))
+
+        # sort segments in start time ascending
+        for spk in results:
+            results[spk] = sorted(results[spk], key=lambda x: x[0])
+
+        return results, pse_labels
 
     @torch.no_grad()
     def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
-    ) -> List[
-        Tuple[
-            Optional[str],
-            List[str],
-            List[int],
-            Union[Hypothesis],
-        ]
-    ]:
+            self,
+            speech: Union[torch.Tensor, np.ndarray],
+            profile: Union[torch.Tensor, np.ndarray],
+            output_format: str = "speaker_turn"
+    ):
         """Inference
 
         Args:
             speech: Input speech data
+            profile: Speaker profiles
         Returns:
-            text, token, token_int, hyp
+            diarization results for each speaker
 
         """
         assert check_argument_types()
-
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
+        if isinstance(profile, np.ndarray):
+            profile = torch.tensor(profile)
 
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.asr_model.frontend = None
-        else:
-            feats = speech
-            feats_len = speech_lengths
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        feats_raw = feats.clone().to(self.device)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
+        # data: (Nsamples,) -> (1, Nsamples)
+        speech = speech.unsqueeze(0).to(getattr(torch, self.dtype))
+        profile = profile.unsqueeze(0).to(getattr(torch, self.dtype))
+        # lengths: (1,)
+        speech_lengths = speech.new_full([1], dtype=torch.long, fill_value=speech.size(1))
+        profile_lengths = profile.new_full([1], dtype=torch.long, fill_value=profile.size(1))
+        batch = {"speech": speech, "speech_lengths": speech_lengths,
+                 "profile": profile, "profile_lengths": profile_lengths}
         # a. To device
         batch = to_device(batch, device=self.device)
-        # b. Forward Encoder
-        _, enc, enc_len = self.asr_model.encode(**batch, ind=self.decoding_ind)
-        if isinstance(enc, tuple):
-            enc = enc[0]
-        assert len(enc) == 1, len(enc)
-        if self.decoding_mode == "model1":
-            predictor_outs = self.asr_model.calc_predictor_mask(enc, enc_len)
-        else:
-            enc, enc_len = self.asr_model.encode2(enc, enc_len, feats_raw, feats_len, ind=self.decoding_ind)
-            predictor_outs = self.asr_model.calc_predictor_mask2(enc, enc_len)
 
-        scama_mask = predictor_outs[4]
-        pre_token_length = predictor_outs[1]
-        pre_acoustic_embeds = predictor_outs[0]
-        maxlen = pre_token_length.sum().item() + self.token_num_relax
-        minlen = max(0, pre_token_length.sum().item() - self.token_num_relax)
-        # c. Passed the encoder result and the beam search
-        nbest_hyps = self.beam_search(
-            x=enc[0], scama_mask=scama_mask, pre_acoustic_embeds=pre_acoustic_embeds, maxlenratio=self.maxlenratio,
-            minlenratio=self.minlenratio, maxlen=int(maxlen), minlen=int(minlen),
-        )
+        logits = self.diar_model.prediction_forward(**batch)
+        results, pse_labels = self.post_processing(logits, profile.shape[1], output_format)
 
-        nbest_hyps = nbest_hyps[: self.nbest]
+        return results, pse_labels
 
-        results = []
-        for hyp in nbest_hyps:
-            assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-            # remove sos/eos and get results
-            last_pos = -1
-            if isinstance(hyp.yseq, list):
-                token_int = hyp.yseq[1:last_pos]
-            else:
-                token_int = hyp.yseq[1:last_pos].tolist()
+    @staticmethod
+    def from_pretrained(
+            model_tag: Optional[str] = None,
+            **kwargs: Optional[Any],
+    ):
+        """Build Speech2Xvector instance from the pretrained model.
 
-            # remove blank symbol id, which is assumed to be 0
-            token_int = list(filter(lambda x: x != 0, token_int))
+        Args:
+            model_tag (Optional[str]): Model tag of the pretrained models.
+                Currently, the tags of espnet_model_zoo are supported.
 
-            # Change integer-ids to tokens
-            token = self.converter.ids2tokens(token_int)
-            token = list(filter(lambda x: x != "<gbg>", token))
+        Returns:
+            Speech2Xvector: Speech2Xvector instance.
 
-            if self.tokenizer is not None:
-                text = self.tokenizer.tokens2text(token)
-            else:
-                text = None
-            results.append((text, token, token_int, hyp))
+        """
+        if model_tag is not None:
+            try:
+                from espnet_model_zoo.downloader import ModelDownloader
 
-        assert check_return_type(results)
-        return results
+            except ImportError:
+                logging.error(
+                    "`espnet_model_zoo` is not installed. "
+                    "Please install via `pip install -U espnet_model_zoo`."
+                )
+                raise
+            d = ModelDownloader()
+            kwargs.update(**d.download_and_unpack(model_tag))
 
-
-def inference(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        ngram_file: Optional[str] = None,
-        cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        streaming: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-        token_num_relax: int = 1,
-        decoding_ind: int = 0,
-        decoding_mode: str = "model1",
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        batch_size=batch_size,
-        beam_size=beam_size,
-        ngpu=ngpu,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        penalty=penalty,
-        log_level=log_level,
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        raw_inputs=raw_inputs,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        key_file=key_file,
-        word_lm_train_config=word_lm_train_config,
-        bpemodel=bpemodel,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        ngram_weight=ngram_weight,
-        ngram_file=ngram_file,
-        nbest=nbest,
-        num_workers=num_workers,
-        token_num_relax=token_num_relax,
-        decoding_ind=decoding_ind,
-        decoding_mode=decoding_mode,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
+        return Speech2Diarization(**kwargs)
 
 
 def inference_modelscope(
-        maxlenratio: float,
-        minlenratio: float,
-        batch_size: int,
-        beam_size: int,
-        ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        ngram_file: Optional[str] = None,
-        cmvn_file: Optional[str] = None,
-        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
-        key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        streaming: bool = False,
+        diar_train_config: str,
+        diar_model_file: str,
         output_dir: Optional[str] = None,
+        batch_size: int = 1,
         dtype: str = "float32",
+        ngpu: int = 0,
         seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
-        num_workers: int = 1,
-        token_num_relax: int = 1,
-        decoding_ind: int = 0,
-        decoding_mode: str = "model1",
-        param_dict: dict = None,
+        num_workers: int = 0,
+        log_level: Union[int, str] = "INFO",
+        key_file: Optional[str] = None,
+        model_tag: Optional[str] = None,
+        allow_variable_data_keys: bool = True,
+        streaming: bool = False,
+        smooth_size: int = 83,
+        dur_threshold: int = 10,
+        out_format: str = "vad",
+        param_dict: Optional[dict] = None,
+        mode: str = "sond",
         **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
-    if word_lm_train_config is not None:
-        raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
+    logging.info("param_dict: {}".format(param_dict))
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
-    if param_dict is not None and "decoding_model" in param_dict:
-        if param_dict["decoding_model"] == "fast":
-            decoding_ind = 0
-            decoding_mode = "model1"
-        elif param_dict["decoding_model"] == "normal":
-            decoding_ind = 0
-            decoding_mode = "model2"
-        elif param_dict["decoding_model"] == "offline":
-            decoding_ind = 1
-            decoding_mode = "model2"
-        else:
-            raise NotImplementedError("unsupported decoding model {}".format(param_dict["decoding_model"]))
 
     # 1. Set random-seed
     set_all_random_seed(seed)
 
-    # 2. Build speech2text
-    speech2text_kwargs = dict(
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        ngram_file=ngram_file,
-        token_type=token_type,
-        bpemodel=bpemodel,
+    # 2a. Build speech2xvec [Optional]
+    if mode == "sond_demo" and param_dict is not None and "extract_profile" in param_dict and param_dict["extract_profile"]:
+        assert "sv_train_config" in param_dict, "sv_train_config must be provided param_dict."
+        assert "sv_model_file" in param_dict, "sv_model_file must be provided in param_dict."
+        sv_train_config = param_dict["sv_train_config"]
+        sv_model_file = param_dict["sv_model_file"]
+        if "model_dir" in param_dict:
+            sv_train_config = os.path.join(param_dict["model_dir"], sv_train_config)
+            sv_model_file = os.path.join(param_dict["model_dir"], sv_model_file)
+        from funasr.bin.sv_inference import Speech2Xvector
+        speech2xvector_kwargs = dict(
+            sv_train_config=sv_train_config,
+            sv_model_file=sv_model_file,
+            device=device,
+            dtype=dtype,
+            streaming=streaming,
+            embedding_node="resnet1_dense"
+        )
+        logging.info("speech2xvector_kwargs: {}".format(speech2xvector_kwargs))
+        speech2xvector = Speech2Xvector.from_pretrained(
+            model_tag=model_tag,
+            **speech2xvector_kwargs,
+        )
+        speech2xvector.sv_model.eval()
+
+    # 2b. Build speech2diar
+    speech2diar_kwargs = dict(
+        diar_train_config=diar_train_config,
+        diar_model_file=diar_model_file,
         device=device,
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
         dtype=dtype,
-        beam_size=beam_size,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        ngram_weight=ngram_weight,
-        penalty=penalty,
-        nbest=nbest,
         streaming=streaming,
-        token_num_relax=token_num_relax,
-        decoding_ind=decoding_ind,
-        decoding_mode=decoding_mode,
-    )
-    speech2text = Speech2Text(**speech2text_kwargs)
-    
-    def _forward(data_path_and_name_and_type,
-                 raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-                 output_dir_v2: Optional[str] = None,
-                 fs: dict = None,
-                 param_dict: dict = None,
-                 **kwargs,
-                 ):
-        # 3. Build data-iterator
+        smooth_size=smooth_size,
+        dur_threshold=dur_threshold,
+    )
+    logging.info("speech2diarization_kwargs: {}".format(speech2diar_kwargs))
+    speech2diar = Speech2Diarization.from_pretrained(
+        model_tag=model_tag,
+        **speech2diar_kwargs,
+    )
+    speech2diar.diar_model.eval()
+
+    def output_results_str(results: dict, uttid: str):
+        rst = []
+        mid = uttid.rsplit("-", 1)[0]
+        for key in results:
+            results[key] = [(x[0]/100, x[1]/100) for x in results[key]]
+        if out_format == "vad":
+            for spk, segs in results.items():
+                rst.append("{} {}".format(spk, segs))
+        else:
+            template = "SPEAKER {} 0 {:.2f} {:.2f} <NA> <NA> {} <NA> <NA>"
+            for spk, segs in results.items():
+                rst.extend([template.format(mid, st, ed, spk) for st, ed in segs])
+
+        return "\n".join(rst)
+
+    def _forward(
+            data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
+            raw_inputs: List[List[Union[np.ndarray, torch.Tensor, str, bytes]]] = None,
+            output_dir_v2: Optional[str] = None,
+            param_dict: Optional[dict] = None,
+    ):
+        logging.info("param_dict: {}".format(param_dict))
         if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
-            dtype=dtype,
-            fs=fs,
-            batch_size=batch_size,
-            key_file=key_file,
-            num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
-        )
-    
-        finish_count = 0
-        file_count = 1
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        asr_result_list = []
+            if isinstance(raw_inputs, (list, tuple)):
+                if not isinstance(raw_inputs[0], List):
+                    raw_inputs = [raw_inputs]
+
+                assert all([len(example) >= 2 for example in raw_inputs]), \
+                    "The length of test case in raw_inputs must larger than 1 (>=2)."
+
+                def prepare_dataset():
+                    for idx, example in enumerate(raw_inputs):
+                        # read waveform file
+                        example = [load_bytes(x) if isinstance(x, bytes) else x
+                                   for x in example]
+                        example = [soundfile.read(x)[0] if isinstance(x, str) else x
+                                   for x in example]
+                        # convert torch tensor to numpy array
+                        example = [x.numpy() if isinstance(example[0], torch.Tensor) else x
+                                   for x in example]
+                        speech = example[0]
+                        logging.info("Extracting profiles for {} waveforms".format(len(example)-1))
+                        profile = [speech2xvector.calculate_embedding(x) for x in example[1:]]
+                        profile = torch.cat(profile, dim=0)
+                        yield ["test{}".format(idx)], {"speech": [speech], "profile": [profile]}
+
+                loader = prepare_dataset()
+            else:
+                raise TypeError("raw_inputs must be a list or tuple in [speech, profile1, profile2, ...] ")
+        else:
+            # 3. Build data-iterator
+            loader = ASRTask.build_streaming_iterator(
+                data_path_and_name_and_type,
+                dtype=dtype,
+                batch_size=batch_size,
+                key_file=key_file,
+                num_workers=num_workers,
+                preprocess_fn=None,
+                collate_fn=None,
+                allow_variable_data_keys=allow_variable_data_keys,
+                inference=True,
+            )
+
+        # 7. Start for-loop
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
-            writer = DatadirWriter(output_path)
-        else:
-            writer = None
-    
-        for keys, batch in loader:
+            os.makedirs(output_path, exist_ok=True)
+            output_writer = open("{}/result.txt".format(output_path), "w")
+            pse_label_writer = open("{}/labels.txt".format(output_path), "w")
+        logging.info("Start to diarize...")
+        result_list = []
+        for idx, (keys, batch) in enumerate(loader):
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            #batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-    
-            # N-best list of (text, token, token_int, hyp_object)
-            try:
-                results = speech2text(**batch)
-            except TooShortUttError as e:
-                logging.warning(f"Utterance {keys} {e}")
-                hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
-                results = [[" ", ["sil"], [2], hyp]] * nbest
-    
+            batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
+
+            results, pse_labels = speech2diar(**batch)
             # Only supporting batch_size==1
-            key = keys[0]
-            logging.info(f"Utterance: {key}")
-            for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
-                # Create a directory: outdir/{n}best_recog
-                if writer is not None:
-                    ibest_writer = writer[f"{n}best_recog"]
-    
-                    # Write the result to each file
-                    ibest_writer["token"][key] = " ".join(token)
-                    # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                    ibest_writer["score"][key] = str(hyp.score)
-    
-                if text is not None:
-                    text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
-                    item = {'key': key, 'value': text_postprocessed}
-                    asr_result_list.append(item)
-                    finish_count += 1
-                    asr_utils.print_progress(finish_count / file_count)
-                    if writer is not None:
-                        ibest_writer["text"][key] = " ".join(word_lists)
-        return asr_result_list
-    
+            key, value = keys[0], output_results_str(results, keys[0])
+            item = {"key": key, "value": value}
+            result_list.append(item)
+            if output_path is not None:
+                output_writer.write(value)
+                output_writer.flush()
+                pse_label_writer.write("{} {}\n".format(key, " ".join(pse_labels)))
+                pse_label_writer.flush()
+
+            if idx % 100 == 0:
+                logging.info("Processing {:5d}: {}".format(idx, key))
+
+        if output_path is not None:
+            output_writer.close()
+            pse_label_writer.close()
+
+        return result_list
+
     return _forward
 
 
+def inference(
+        data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
+        diar_train_config: Optional[str],
+        diar_model_file: Optional[str],
+        output_dir: Optional[str] = None,
+        batch_size: int = 1,
+        dtype: str = "float32",
+        ngpu: int = 0,
+        seed: int = 0,
+        num_workers: int = 1,
+        log_level: Union[int, str] = "INFO",
+        key_file: Optional[str] = None,
+        model_tag: Optional[str] = None,
+        allow_variable_data_keys: bool = True,
+        streaming: bool = False,
+        smooth_size: int = 83,
+        dur_threshold: int = 10,
+        out_format: str = "vad",
+        **kwargs,
+):
+    inference_pipeline = inference_modelscope(
+        diar_train_config=diar_train_config,
+        diar_model_file=diar_model_file,
+        output_dir=output_dir,
+        batch_size=batch_size,
+        dtype=dtype,
+        ngpu=ngpu,
+        seed=seed,
+        num_workers=num_workers,
+        log_level=log_level,
+        key_file=key_file,
+        model_tag=model_tag,
+        allow_variable_data_keys=allow_variable_data_keys,
+        streaming=streaming,
+        smooth_size=smooth_size,
+        dur_threshold=dur_threshold,
+        out_format=out_format,
+        **kwargs,
+    )
+
+    return inference_pipeline(data_path_and_name_and_type, raw_inputs=None)
+
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="ASR Decoding",
+        description="Speaker verification/x-vector extraction",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
     # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
 
-    parser.add_argument("--output_dir", type=str, required=True)
+    parser.add_argument("--output_dir", type=str, required=False)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
+    parser.add_argument(
+        "--gpuid_list",
+        type=str,
+        default="",
+        help="The visible gpus",
+    )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
     parser.add_argument(
         "--dtype",
         default="float32",
         choices=["float16", "float32", "float64"],
         help="Data type",
     )
@@ -559,136 +505,73 @@
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=False,
         action="append",
     )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
-        "--asr_train_config",
-        type=str,
-        help="ASR training configuration",
-    )
-    group.add_argument(
-        "--asr_model_file",
-        type=str,
-        help="ASR model parameter file",
-    )
-    group.add_argument(
-        "--cmvn_file",
+        "--diar_train_config",
         type=str,
-        help="Global cmvn file",
+        help="diarization training configuration",
     )
     group.add_argument(
-        "--lm_train_config",
+        "--diar_model_file",
         type=str,
-        help="LM training configuration",
+        help="diarization model parameter file",
     )
     group.add_argument(
-        "--lm_file",
-        type=str,
-        help="LM parameter file",
-    )
-    group.add_argument(
-        "--word_lm_train_config",
-        type=str,
-        help="Word LM training configuration",
-    )
-    group.add_argument(
-        "--word_lm_file",
-        type=str,
-        help="Word LM parameter file",
+        "--dur_threshold",
+        type=int,
+        default=10,
+        help="The threshold for short segments in number frames"
     )
-    group.add_argument(
-        "--ngram_file",
-        type=str,
-        help="N-gram parameter file",
+    parser.add_argument(
+        "--smooth_size",
+        type=int,
+        default=83,
+        help="The smoothing window length in number frames"
     )
     group.add_argument(
         "--model_tag",
         type=str,
         help="Pretrained model tag. If specify this option, *_train_config and "
              "*_file will be overwritten",
     )
-
-    group = parser.add_argument_group("Beam-search related")
-    group.add_argument(
+    parser.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
-    group.add_argument("--nbest", type=int, default=1, help="Output N-best hypotheses")
-    group.add_argument("--beam_size", type=int, default=20, help="Beam size")
-    group.add_argument("--penalty", type=float, default=0.0, help="Insertion penalty")
-    group.add_argument(
-        "--maxlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain max output length. "
-             "If maxlenratio=0.0 (default), it uses a end-detect "
-             "function "
-             "to automatically find maximum hypothesis lengths."
-             "If maxlenratio<0.0, its absolute value is interpreted"
-             "as a constant max output length",
-    )
-    group.add_argument(
-        "--minlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain min output length",
-    )
-    group.add_argument(
-        "--ctc_weight",
-        type=float,
-        default=0.5,
-        help="CTC weight in joint decoding",
-    )
-    group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
-    group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
-    group.add_argument("--streaming", type=str2bool, default=False)
+    parser.add_argument("--streaming", type=str2bool, default=False)
 
-    group = parser.add_argument_group("Text converter related")
-    group.add_argument(
-        "--token_type",
-        type=str_or_none,
-        default=None,
-        choices=["char", "bpe", None],
-        help="The token type for ASR model. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument(
-        "--bpemodel",
-        type=str_or_none,
-        default=None,
-        help="The model path of sentencepiece. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument("--token_num_relax", type=int, default=1, help="")
-    group.add_argument("--decoding_ind", type=int, default=0, help="")
-    group.add_argument("--decoding_mode", type=str, default="model1", help="")
-    group.add_argument(
-        "--ctc_weight2",
-        type=float,
-        default=0.0,
-        help="CTC weight in joint decoding",
-    )
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
-    inference(**kwargs)
+    logging.info("args: {}".format(kwargs))
+    if args.output_dir is None:
+        jobid, n_gpu = 1, 1
+        gpuid = args.gpuid_list.split(",")[jobid-1]
+    else:
+        jobid = int(args.output_dir.split(".")[-1])
+        n_gpu = len(args.gpuid_list.split(","))
+        gpuid = args.gpuid_list.split(",")[(jobid - 1) % n_gpu]
+    os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
+    os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
+    results_list = inference(**kwargs)
+    for results in results_list:
+        print("{} {}".format(results["key"], results["value"]))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.4.8/funasr/bin/asr_inference_uniasr_vad.py` & `funasr-0.5.0/funasr/bin/vad_inference.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,202 +1,99 @@
-#!/usr/bin/env python3
 import argparse
 import logging
+import os
 import sys
+import json
 from pathlib import Path
+from typing import Any
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
-from typing import Any
 
+import math
 import numpy as np
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.beam_search import BeamSearchScama as BeamSearch
-from funasr.modules.beam_search.beam_search import Hypothesis
-from funasr.modules.scorers.ctc import CTCPrefixScorer
-from funasr.modules.scorers.length_bonus import LengthBonus
+from funasr.modules.scorers.scorer_interface import BatchScorerInterface
 from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTaskUniASR as ASRTask
-from funasr.tasks.lm import LMTask
-from funasr.text.build_tokenizer import build_tokenizer
-from funasr.text.token_id_converter import TokenIDConverter
+from funasr.tasks.vad import VADTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend
-
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
 
 header_colors = '\033[95m'
 end_colors = '\033[0m'
 
+global_asr_language: str = 'zh-cn'
+global_sample_rate: Union[int, Dict[Any, int]] = {
+    'audio_fs': 16000,
+    'model_fs': 16000
+}
 
-class Speech2Text:
-    """Speech2Text class
+
+class Speech2VadSegment:
+    """Speech2VadSegment class
 
     Examples:
         >>> import soundfile
-        >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
+        >>> speech2segment = Speech2VadSegment("vad_config.yml", "vad.pt")
         >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2text(audio)
-        [(text, token, token_int, hypothesis object), ...]
+        >>> speech2segment(audio)
+        [[10, 230], [245, 450], ...]
 
     """
 
     def __init__(
             self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
+            vad_infer_config: Union[Path, str] = None,
+            vad_model_file: Union[Path, str] = None,
+            vad_cmvn_file: Union[Path, str] = None,
             device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
+            batch_size: int = 1,
             dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            token_num_relax: int = 1,
-            decoding_ind: int = 0,
-            decoding_mode: str = "model1",
-            frontend_conf: dict = None,
             **kwargs,
     ):
         assert check_argument_types()
 
-        # 1. Build ASR model
-        scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
+        # 1. Build vad model
+        vad_model, vad_infer_args = VADTask.build_model_from_file(
+            vad_infer_config, vad_model_file, device
         )
         frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
+        if vad_infer_args.frontend is not None:
+            frontend = WavFrontend(cmvn_file=vad_cmvn_file, **vad_infer_args.frontend_conf)
 
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-        if decoding_mode == "model1":
-            decoder = asr_model.decoder
-        else:
-            decoder = asr_model.decoder2
+        logging.info("vad_model: {}".format(vad_model))
+        logging.info("vad_infer_args: {}".format(vad_infer_args))
+        vad_model.to(dtype=getattr(torch, dtype)).eval()
 
-        if asr_model.ctc != None:
-            ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
-            scorers.update(
-                ctc=ctc
-            )
-        token_list = asr_model.token_list
-        scorers.update(
-            decoder=decoder,
-            length_bonus=LengthBonus(len(token_list)),
-        )
-
-        # 2. Build Language model
-        if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
-            )
-            scorers["lm"] = lm.lm
-
-        # 3. Build ngram model
-        # ngram is not supported now
-        ngram = None
-        scorers["ngram"] = ngram
-
-        # 4. Build BeamSearch object
-        # transducer is not supported now
-        beam_search_transducer = None
-
-        weights = dict(
-            decoder=1.0 - ctc_weight,
-            ctc=ctc_weight,
-            lm=lm_weight,
-            ngram=ngram_weight,
-            length_bonus=penalty,
-        )
-        beam_search = BeamSearch(
-            beam_size=beam_size,
-            weights=weights,
-            scorers=scorers,
-            sos=asr_model.sos,
-            eos=asr_model.eos,
-            vocab_size=len(token_list),
-            token_list=token_list,
-            pre_beam_score_key=None if ctc_weight == 1.0 else "full",
-        )
-
-        beam_search.to(device=device, dtype=getattr(torch, dtype)).eval()
-        for scorer in scorers.values():
-            if isinstance(scorer, torch.nn.Module):
-                scorer.to(device=device, dtype=getattr(torch, dtype)).eval()
-        # logging.info(f"Beam_search: {beam_search}")
-        logging.info(f"Decoding device={device}, dtype={dtype}")
-
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
-        else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-        self.beam_search = beam_search
-        self.beam_search_transducer = beam_search_transducer
-        self.maxlenratio = maxlenratio
-        self.minlenratio = minlenratio
+        self.vad_model = vad_model
+        self.vad_infer_args = vad_infer_args
         self.device = device
         self.dtype = dtype
-        self.nbest = nbest
-        self.token_num_relax = token_num_relax
-        self.decoding_ind = decoding_ind
-        self.decoding_mode = decoding_mode
         self.frontend = frontend
+        self.batch_size = batch_size
 
     @torch.no_grad()
     def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
-    ) -> List[
-        Tuple[
-            Optional[str],
-            List[str],
-            List[int],
-            Union[Hypothesis],
-        ]
-    ]:
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
+            in_cache: Dict[str, torch.Tensor] = dict()
+    ) -> Tuple[List[List[int]], Dict[str, torch.Tensor]]:
         """Inference
 
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
@@ -204,349 +101,406 @@
         assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
+            self.frontend.filter_length_max = math.inf
+            fbanks, fbanks_len = self.frontend.forward_fbank(speech, speech_lengths)
+            feats, feats_len = self.frontend.forward_lfr_cmvn(fbanks, fbanks_len)
+            fbanks = to_device(fbanks, device=self.device)
             feats = to_device(feats, device=self.device)
             feats_len = feats_len.int()
-            self.asr_model.frontend = None
-        else:
-            feats = speech
-            feats_len = speech_lengths
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        feats_raw = feats.clone().to(self.device)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-        # b. Forward Encoder
-        _, enc, enc_len = self.asr_model.encode(**batch, ind=self.decoding_ind)
-        if isinstance(enc, tuple):
-            enc = enc[0]
-        assert len(enc) == 1, len(enc)
-        if self.decoding_mode == "model1":
-            predictor_outs = self.asr_model.calc_predictor_mask(enc, enc_len)
         else:
-            enc, enc_len = self.asr_model.encode2(enc, enc_len, feats_raw, feats_len, ind=self.decoding_ind)
-            predictor_outs = self.asr_model.calc_predictor_mask2(enc, enc_len)
+            raise Exception("Need to extract feats first, please configure frontend configuration")
 
-        scama_mask = predictor_outs[4]
-        pre_token_length = predictor_outs[1]
-        pre_acoustic_embeds = predictor_outs[0]
-        maxlen = pre_token_length.sum().item() + self.token_num_relax
-        minlen = max(0, pre_token_length.sum().item() - self.token_num_relax)
-        # c. Passed the encoder result and the beam search
-        nbest_hyps = self.beam_search(
-            x=enc[0], scama_mask=scama_mask, pre_acoustic_embeds=pre_acoustic_embeds, maxlenratio=self.maxlenratio,
-            minlenratio=self.minlenratio, maxlen=int(maxlen), minlen=int(minlen),
-        )
+        # b. Forward Encoder streaming
+        t_offset = 0
+        step = min(feats_len.max(), 6000)
+        segments = [[]] * self.batch_size
+        for t_offset in range(0, feats_len, min(step, feats_len - t_offset)):
+            if t_offset + step >= feats_len - 1:
+                step = feats_len - t_offset
+                is_final = True
+            else:
+                is_final = False
+            batch = {
+                "feats": feats[:, t_offset:t_offset + step, :],
+                "waveform": speech[:, t_offset * 160:min(speech.shape[-1], (t_offset + step - 1) * 160 + 400)],
+                "is_final": is_final,
+                "in_cache": in_cache
+            }
+            # a. To device
+            #batch = to_device(batch, device=self.device)
+            segments_part, in_cache = self.vad_model(**batch)
+            if segments_part:
+                for batch_num in range(0, self.batch_size):
+                    segments[batch_num] += segments_part[batch_num]
+        return fbanks, segments
 
-        nbest_hyps = nbest_hyps[: self.nbest]
+class Speech2VadSegmentOnline(Speech2VadSegment):
+    """Speech2VadSegmentOnline class
 
-        results = []
-        for hyp in nbest_hyps:
-            assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-            # remove sos/eos and get results
-            last_pos = -1
-            if isinstance(hyp.yseq, list):
-                token_int = hyp.yseq[1:last_pos]
-            else:
-                token_int = hyp.yseq[1:last_pos].tolist()
+    Examples:
+        >>> import soundfile
+        >>> speech2segment = Speech2VadSegmentOnline("vad_config.yml", "vad.pt")
+        >>> audio, rate = soundfile.read("speech.wav")
+        >>> speech2segment(audio)
+        [[10, 230], [245, 450], ...]
 
-            # remove blank symbol id, which is assumed to be 0
-            token_int = list(filter(lambda x: x != 0, token_int))
+    """
+    def __init__(self, **kwargs):
+        super(Speech2VadSegmentOnline, self).__init__(**kwargs)
+        vad_cmvn_file = kwargs.get('vad_cmvn_file', None)
+        self.frontend = None
+        if self.vad_infer_args.frontend is not None:
+            self.frontend = WavFrontendOnline(cmvn_file=vad_cmvn_file, **self.vad_infer_args.frontend_conf)
 
-            # Change integer-ids to tokens
-            token = self.converter.ids2tokens(token_int)
-            token = list(filter(lambda x: x != "<gbg>", token))
 
-            if self.tokenizer is not None:
-                text = self.tokenizer.tokens2text(token)
-            else:
-                text = None
-            results.append((text, token, token_int, hyp))
+    @torch.no_grad()
+    def __call__(
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
+            in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False, max_end_sil: int = 800
+    ) -> Tuple[torch.Tensor, List[List[int]], torch.Tensor]:
+        """Inference
 
-        assert check_return_type(results)
-        return results
+        Args:
+            speech: Input speech data
+        Returns:
+            text, token, token_int, hyp
+
+        """
+        assert check_argument_types()
+
+        # Input as audio signal
+        if isinstance(speech, np.ndarray):
+            speech = torch.tensor(speech)
+        batch_size = speech.shape[0]
+        segments = [[]] * batch_size
+        if self.frontend is not None:
+            feats, feats_len = self.frontend.forward(speech, speech_lengths, is_final)
+            fbanks, _ = self.frontend.get_fbank()
+        else:
+            raise Exception("Need to extract feats first, please configure frontend configuration")
+        if feats.shape[0]:
+            feats = to_device(feats, device=self.device)
+            feats_len = feats_len.int()
+            waveforms = self.frontend.get_waveforms()
+
+            batch = {
+                "feats": feats,
+                "waveform": waveforms,
+                "in_cache": in_cache,
+                "is_final": is_final,
+                "max_end_sil": max_end_sil
+            }
+            # a. To device
+            batch = to_device(batch, device=self.device)
+            segments, in_cache = self.vad_model.forward_online(**batch)
+            # in_cache.update(batch['in_cache'])
+            # in_cache = {key: value for key, value in batch['in_cache'].items()}
+        return fbanks, segments, in_cache
 
 
 def inference(
-        maxlenratio: float,
-        minlenratio: float,
         batch_size: int,
-        beam_size: int,
         ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
         log_level: Union[int, str],
         data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        ngram_file: Optional[str] = None,
-        cmvn_file: Optional[str] = None,
+        vad_infer_config: Optional[str],
+        vad_model_file: Optional[str],
+        vad_cmvn_file: Optional[str] = None,
         raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
         key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
         allow_variable_data_keys: bool = False,
-        streaming: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
         num_workers: int = 1,
-        token_num_relax: int = 1,
-        decoding_ind: int = 0,
-        decoding_mode: str = "model1",
+        online: bool = False,
         **kwargs,
 ):
-    inference_pipeline = inference_modelscope(
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
-        batch_size=batch_size,
-        beam_size=beam_size,
-        ngpu=ngpu,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        penalty=penalty,
-        log_level=log_level,
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        raw_inputs=raw_inputs,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        token_type=token_type,
-        key_file=key_file,
-        word_lm_train_config=word_lm_train_config,
-        bpemodel=bpemodel,
-        allow_variable_data_keys=allow_variable_data_keys,
-        streaming=streaming,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        ngram_weight=ngram_weight,
-        ngram_file=ngram_file,
-        nbest=nbest,
-        num_workers=num_workers,
-        token_num_relax=token_num_relax,
-        decoding_ind=decoding_ind,
-        decoding_mode=decoding_mode,
-        **kwargs,
-    )
+    if not online:
+        inference_pipeline = inference_modelscope(
+            batch_size=batch_size,
+            ngpu=ngpu,
+            log_level=log_level,
+            vad_infer_config=vad_infer_config,
+            vad_model_file=vad_model_file,
+            vad_cmvn_file=vad_cmvn_file,
+            key_file=key_file,
+            allow_variable_data_keys=allow_variable_data_keys,
+            output_dir=output_dir,
+            dtype=dtype,
+            seed=seed,
+            num_workers=num_workers,
+            **kwargs,
+        )
+    else:
+        inference_pipeline = inference_modelscope_online(
+            batch_size=batch_size,
+            ngpu=ngpu,
+            log_level=log_level,
+            vad_infer_config=vad_infer_config,
+            vad_model_file=vad_model_file,
+            vad_cmvn_file=vad_cmvn_file,
+            key_file=key_file,
+            allow_variable_data_keys=allow_variable_data_keys,
+            output_dir=output_dir,
+            dtype=dtype,
+            seed=seed,
+            num_workers=num_workers,
+            **kwargs,
+        )
     return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
-
 def inference_modelscope(
-        maxlenratio: float,
-        minlenratio: float,
         batch_size: int,
-        beam_size: int,
         ngpu: int,
-        ctc_weight: float,
-        lm_weight: float,
-        penalty: float,
         log_level: Union[int, str],
         # data_path_and_name_and_type,
-        asr_train_config: Optional[str],
-        asr_model_file: Optional[str],
-        ngram_file: Optional[str] = None,
-        cmvn_file: Optional[str] = None,
+        vad_infer_config: Optional[str],
+        vad_model_file: Optional[str],
+        vad_cmvn_file: Optional[str] = None,
         # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        lm_train_config: Optional[str] = None,
-        lm_file: Optional[str] = None,
-        token_type: Optional[str] = None,
         key_file: Optional[str] = None,
-        word_lm_train_config: Optional[str] = None,
-        bpemodel: Optional[str] = None,
         allow_variable_data_keys: bool = False,
-        streaming: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
-        ngram_weight: float = 0.9,
-        nbest: int = 1,
         num_workers: int = 1,
-        token_num_relax: int = 1,
-        decoding_ind: int = 0,
-        decoding_mode: str = "model1",
-        param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
-    if word_lm_train_config is not None:
-        raise NotImplementedError("Word LM is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
+
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
+        batch_size = 1
+    # 1. Set random-seed
+    set_all_random_seed(seed)
 
-    if param_dict is not None and "decoding_model" in param_dict:
-        if param_dict["decoding_model"] == "fast":
-            decoding_ind = 0
-            decoding_mode = "model1"
-        elif param_dict["decoding_model"] == "normal":
-            decoding_ind = 0
-            decoding_mode = "model2"
-        elif param_dict["decoding_model"] == "offline":
-            decoding_ind = 1
-            decoding_mode = "model2"
+    # 2. Build speech2vadsegment
+    speech2vadsegment_kwargs = dict(
+        vad_infer_config=vad_infer_config,
+        vad_model_file=vad_model_file,
+        vad_cmvn_file=vad_cmvn_file,
+        device=device,
+        dtype=dtype,
+    )
+    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
+    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
+
+    def _forward(
+            data_path_and_name_and_type,
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            fs: dict = None,
+            param_dict: dict = None
+    ):
+        # 3. Build data-iterator
+        if data_path_and_name_and_type is None and raw_inputs is not None:
+            if isinstance(raw_inputs, torch.Tensor):
+                raw_inputs = raw_inputs.numpy()
+            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
+        loader = VADTask.build_streaming_iterator(
+            data_path_and_name_and_type,
+            dtype=dtype,
+            batch_size=batch_size,
+            key_file=key_file,
+            num_workers=num_workers,
+            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
+            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
+            allow_variable_data_keys=allow_variable_data_keys,
+            inference=True,
+        )
+
+        finish_count = 0
+        file_count = 1
+        # 7 .Start for-loop
+        # FIXME(kamo): The output format should be discussed about
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        if output_path is not None:
+            writer = DatadirWriter(output_path)
+            ibest_writer = writer[f"1best_recog"]
         else:
-            raise NotImplementedError("unsupported decoding model {}".format(param_dict["decoding_model"]))
+            writer = None
+            ibest_writer = None
+
+        vad_results = []
+        for keys, batch in loader:
+            assert isinstance(batch, dict), type(batch)
+            assert all(isinstance(s, str) for s in keys), keys
+            _bs = len(next(iter(batch.values())))
+            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+
+            # do vad segment
+            _, results = speech2vadsegment(**batch)
+            for i, _ in enumerate(keys):
+                if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
+                    results[i] = json.dumps(results[i])
+                item = {'key': keys[i], 'value': results[i]}
+                vad_results.append(item)
+                if writer is not None:
+                    ibest_writer["text"][keys[i]] = "{}".format(results[i])
+
+        return vad_results
+
+    return _forward
+
+def inference_modelscope_online(
+        batch_size: int,
+        ngpu: int,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        vad_infer_config: Optional[str],
+        vad_model_file: Optional[str],
+        vad_cmvn_file: Optional[str] = None,
+        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        key_file: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        num_workers: int = 1,
+        **kwargs,
+):
+    assert check_argument_types()
+
+
+    logging.basicConfig(
+        level=log_level,
+        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
+    )
+
+    if ngpu >= 1 and torch.cuda.is_available():
+        device = "cuda"
+    else:
+        device = "cpu"
+        batch_size = 1
 
     # 1. Set random-seed
     set_all_random_seed(seed)
 
-    # 2. Build speech2text
-    speech2text_kwargs = dict(
-        asr_train_config=asr_train_config,
-        asr_model_file=asr_model_file,
-        cmvn_file=cmvn_file,
-        lm_train_config=lm_train_config,
-        lm_file=lm_file,
-        ngram_file=ngram_file,
-        token_type=token_type,
-        bpemodel=bpemodel,
+    # 2. Build speech2vadsegment
+    speech2vadsegment_kwargs = dict(
+        vad_infer_config=vad_infer_config,
+        vad_model_file=vad_model_file,
+        vad_cmvn_file=vad_cmvn_file,
         device=device,
-        maxlenratio=maxlenratio,
-        minlenratio=minlenratio,
         dtype=dtype,
-        beam_size=beam_size,
-        ctc_weight=ctc_weight,
-        lm_weight=lm_weight,
-        ngram_weight=ngram_weight,
-        penalty=penalty,
-        nbest=nbest,
-        streaming=streaming,
-        token_num_relax=token_num_relax,
-        decoding_ind=decoding_ind,
-        decoding_mode=decoding_mode,
-    )
-    speech2text = Speech2Text(**speech2text_kwargs)
-    
-    def _forward(data_path_and_name_and_type,
-                 raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-                 output_dir_v2: Optional[str] = None,
-                 fs: dict = None,
-                 param_dict: dict = None,
-                 **kwargs,
-                 ):
+    )
+    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
+    speech2vadsegment = Speech2VadSegmentOnline(**speech2vadsegment_kwargs)
+
+    def _forward(
+            data_path_and_name_and_type,
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            fs: dict = None,
+            param_dict: dict = None,
+    ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
+        loader = VADTask.build_streaming_iterator(
             data_path_and_name_and_type,
             dtype=dtype,
-            fs=fs,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
+            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
+            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
             allow_variable_data_keys=allow_variable_data_keys,
             inference=True,
         )
-    
+
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
-        asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
+            ibest_writer = writer[f"1best_recog"]
         else:
             writer = None
-    
+            ibest_writer = None
+
+        vad_results = []
+        batch_in_cache = param_dict['in_cache'] if param_dict is not None else dict()
+        is_final = param_dict.get('is_final', False) if param_dict is not None else False
+        max_end_sil = param_dict.get('max_end_sil', 800) if param_dict is not None else 800
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            #batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-    
-            # N-best list of (text, token, token_int, hyp_object)
-            try:
-                results = speech2text(**batch)
-            except TooShortUttError as e:
-                logging.warning(f"Utterance {keys} {e}")
-                hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
-                results = [[" ", ["sil"], [2], hyp]] * nbest
-    
-            # Only supporting batch_size==1
-            key = keys[0]
-            logging.info(f"Utterance: {key}")
-            for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
-                # Create a directory: outdir/{n}best_recog
-                if writer is not None:
-                    ibest_writer = writer[f"{n}best_recog"]
-    
-                    # Write the result to each file
-                    ibest_writer["token"][key] = " ".join(token)
-                    # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                    ibest_writer["score"][key] = str(hyp.score)
-    
-                if text is not None:
-                    text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
-                    item = {'key': key, 'value': text_postprocessed}
-                    asr_result_list.append(item)
-                    finish_count += 1
-                    asr_utils.print_progress(finish_count / file_count)
-                    if writer is not None:
-                        ibest_writer["text"][key] = " ".join(word_lists)
-        return asr_result_list
-    
-    return _forward
+            batch['in_cache'] = batch_in_cache
+            batch['is_final'] = is_final
+            batch['max_end_sil'] = max_end_sil
+
+            # do vad segment
+            _, results, param_dict['in_cache'] = speech2vadsegment(**batch)
+            # param_dict['in_cache'] = batch['in_cache']
+            if results:
+                for i, _ in enumerate(keys):
+                    if results[i]:
+                        if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
+                            results[i] = json.dumps(results[i])
+                        item = {'key': keys[i], 'value': results[i]}
+                        vad_results.append(item)
+                        if writer is not None:
+                            ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
+        return vad_results
 
+    return _forward
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
-        description="ASR Decoding",
+        description="VAD Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
     # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
 
-    parser.add_argument("--output_dir", type=str, required=True)
+    parser.add_argument("--output_dir", type=str, required=False)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
+    parser.add_argument(
+        "--gpuid_list",
+        type=str,
+        default="",
+        help="The visible gpus",
+    )
     parser.add_argument("--seed", type=int, default=0, help="Random seed")
     parser.add_argument(
         "--dtype",
         default="float32",
         choices=["float16", "float32", "float64"],
         help="Data type",
     )
@@ -567,129 +521,50 @@
     group.add_argument("--raw_inputs", type=list, default=None)
     # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
     group.add_argument("--key_file", type=str_or_none)
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
 
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
-        "--asr_train_config",
+        "--vad_infer_config",
         type=str,
-        help="ASR training configuration",
+        help="VAD infer configuration",
     )
     group.add_argument(
-        "--asr_model_file",
+        "--vad_model_file",
         type=str,
-        help="ASR model parameter file",
+        help="VAD model parameter file",
     )
     group.add_argument(
-        "--cmvn_file",
+        "--vad_cmvn_file",
         type=str,
         help="Global cmvn file",
     )
     group.add_argument(
-        "--lm_train_config",
-        type=str,
-        help="LM training configuration",
-    )
-    group.add_argument(
-        "--lm_file",
-        type=str,
-        help="LM parameter file",
-    )
-    group.add_argument(
-        "--word_lm_train_config",
+        "--online",
         type=str,
-        help="Word LM training configuration",
-    )
-    group.add_argument(
-        "--word_lm_file",
-        type=str,
-        help="Word LM parameter file",
-    )
-    group.add_argument(
-        "--ngram_file",
-        type=str,
-        help="N-gram parameter file",
-    )
-    group.add_argument(
-        "--model_tag",
-        type=str,
-        help="Pretrained model tag. If specify this option, *_train_config and "
-             "*_file will be overwritten",
+        help="decoding mode",
     )
 
-    group = parser.add_argument_group("Beam-search related")
+    group = parser.add_argument_group("infer related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
-    group.add_argument("--nbest", type=int, default=1, help="Output N-best hypotheses")
-    group.add_argument("--beam_size", type=int, default=20, help="Beam size")
-    group.add_argument("--penalty", type=float, default=0.0, help="Insertion penalty")
-    group.add_argument(
-        "--maxlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain max output length. "
-             "If maxlenratio=0.0 (default), it uses a end-detect "
-             "function "
-             "to automatically find maximum hypothesis lengths."
-             "If maxlenratio<0.0, its absolute value is interpreted"
-             "as a constant max output length",
-    )
-    group.add_argument(
-        "--minlenratio",
-        type=float,
-        default=0.0,
-        help="Input length ratio to obtain min output length",
-    )
-    group.add_argument(
-        "--ctc_weight",
-        type=float,
-        default=0.5,
-        help="CTC weight in joint decoding",
-    )
-    group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
-    group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
-    group.add_argument("--streaming", type=str2bool, default=False)
 
-    group = parser.add_argument_group("Text converter related")
-    group.add_argument(
-        "--token_type",
-        type=str_or_none,
-        default=None,
-        choices=["char", "bpe", None],
-        help="The token type for ASR model. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument(
-        "--bpemodel",
-        type=str_or_none,
-        default=None,
-        help="The model path of sentencepiece. "
-             "If not given, refers from the training args",
-    )
-    group.add_argument("--token_num_relax", type=int, default=1, help="")
-    group.add_argument("--decoding_ind", type=int, default=0, help="")
-    group.add_argument("--decoding_mode", type=str, default="model1", help="")
-    group.add_argument(
-        "--ctc_weight2",
-        type=float,
-        default=0.0,
-        help="CTC weight in joint decoding",
-    )
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     args = parser.parse_args(cmd)
     kwargs = vars(args)
     kwargs.pop("config", None)
     inference(**kwargs)
 
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `funasr-0.4.8/funasr/bin/asr_train.py` & `funasr-0.5.0/funasr/bin/asr_train_paraformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import os
 
-from funasr.tasks.asr import ASRTask
+from funasr.tasks.asr import ASRTaskParaformer as ASRTask
 
 
 # for ASR Training
 def parse_args():
     parser = ASRTask.get_parser()
     parser.add_argument(
         "--gpu_id",
```

### Comparing `funasr-0.4.8/funasr/bin/asr_train_paraformer.py` & `funasr-0.5.0/funasr/bin/asr_train_uniasr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 
 import os
 
-from funasr.tasks.asr import ASRTaskParaformer as ASRTask
+from funasr.tasks.asr import ASRTaskUniASR
 
 
 # for ASR Training
 def parse_args():
-    parser = ASRTask.get_parser()
+    parser = ASRTaskUniASR.get_parser()
     parser.add_argument(
         "--gpu_id",
         type=int,
         default=0,
         help="local gpu id.",
     )
     args = parser.parse_args()
     return args
 
 
 def main(args=None, cmd=None):
     # for ASR Training
-    ASRTask.main(args=args, cmd=cmd)
+    ASRTaskUniASR.main(args=args, cmd=cmd)
 
 
 if __name__ == '__main__':
     args = parse_args()
 
     # setup local gpu_id
     os.environ['CUDA_VISIBLE_DEVICES'] = str(args.gpu_id)
```

### Comparing `funasr-0.4.8/funasr/bin/asr_train_transducer.py` & `funasr-0.5.0/funasr/bin/asr_train_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/asr_train_uniasr.py` & `funasr-0.5.0/funasr/bin/diar_train.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 
 import os
 
-from funasr.tasks.asr import ASRTaskUniASR
+from funasr.tasks.diar import DiarTask
 
 
 # for ASR Training
 def parse_args():
-    parser = ASRTaskUniASR.get_parser()
+    parser = DiarTask.get_parser()
     parser.add_argument(
         "--gpu_id",
         type=int,
         default=0,
         help="local gpu id.",
     )
     args = parser.parse_args()
     return args
 
 
 def main(args=None, cmd=None):
     # for ASR Training
-    ASRTaskUniASR.main(args=args, cmd=cmd)
+    DiarTask.main(args=args, cmd=cmd)
 
 
 if __name__ == '__main__':
     args = parse_args()
 
     # setup local gpu_id
     os.environ['CUDA_VISIBLE_DEVICES'] = str(args.gpu_id)
```

### Comparing `funasr-0.4.8/funasr/bin/build_trainer.py` & `funasr-0.5.0/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/data2vec_train.py` & `funasr-0.5.0/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/diar_inference_launch.py` & `funasr-0.5.0/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/diar_train.py` & `funasr-0.5.0/funasr/bin/lm_train.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 
 import os
 
-from funasr.tasks.diar import DiarTask
+from funasr.tasks.lm import LMTask
 
 
-# for ASR Training
+# for LM Training
 def parse_args():
-    parser = DiarTask.get_parser()
+    parser = LMTask.get_parser()
     parser.add_argument(
         "--gpu_id",
         type=int,
         default=0,
         help="local gpu id.",
     )
     args = parser.parse_args()
     return args
 
 
 def main(args=None, cmd=None):
-    # for ASR Training
-    DiarTask.main(args=args, cmd=cmd)
+    # for LM Training
+    LMTask.main(args=args, cmd=cmd)
 
 
 if __name__ == '__main__':
     args = parse_args()
 
     # setup local gpu_id
     os.environ['CUDA_VISIBLE_DEVICES'] = str(args.gpu_id)
@@ -33,14 +33,14 @@
     if args.ngpu > 1:
         args.distributed = True
     else:
         args.distributed = False
     assert args.num_worker_count == 1
 
     # re-compute batch size: when dataset type is small
-    if args.dataset_type == "small":
+    if args.dataset_type == "small" and args.ngpu != 0:
         if args.batch_size is not None:
             args.batch_size = args.batch_size * args.ngpu
         if args.batch_bins is not None:
             args.batch_bins = args.batch_bins * args.ngpu
 
     main(args=args)
```

### Comparing `funasr-0.4.8/funasr/bin/eend_ola_inference.py` & `funasr-0.5.0/funasr/bin/eend_ola_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/lm_calc_perplexity.py` & `funasr-0.5.0/funasr/bin/lm_calc_perplexity.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/lm_inference.py` & `funasr-0.5.0/funasr/bin/lm_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/lm_inference_launch.py` & `funasr-0.5.0/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/modelscope_infer.py` & `funasr-0.5.0/funasr/bin/modelscope_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/punc_inference_launch.py` & `funasr-0.5.0/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/punc_train.py` & `funasr-0.5.0/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/punctuation_infer.py` & `funasr-0.5.0/funasr/bin/punctuation_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/punctuation_infer_vadrealtime.py` & `funasr-0.5.0/funasr/bin/punctuation_infer_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/sv_inference.py` & `funasr-0.5.0/funasr/bin/sv_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/sv_inference_launch.py` & `funasr-0.5.0/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/tokenize_text.py` & `funasr-0.5.0/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/tp_inference.py` & `funasr-0.5.0/funasr/bin/tp_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/tp_inference_launch.py` & `funasr-0.5.0/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/vad_inference.py` & `funasr-0.5.0/funasr/bin/vad_inference_online.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,139 +8,35 @@
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
 
-import math
 import numpy as np
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
 from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.scorers.scorer_interface import BatchScorerInterface
-from funasr.modules.subsampling import TooShortUttError
 from funasr.tasks.vad import VADTask
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
+from funasr.models.frontend.wav_frontend import WavFrontendOnline
+from funasr.models.frontend.wav_frontend import WavFrontend
+from funasr.bin.vad_inference import Speech2VadSegment
 
 header_colors = '\033[95m'
 end_colors = '\033[0m'
 
-global_asr_language: str = 'zh-cn'
-global_sample_rate: Union[int, Dict[Any, int]] = {
-    'audio_fs': 16000,
-    'model_fs': 16000
-}
-
-
-class Speech2VadSegment:
-    """Speech2VadSegment class
-
-    Examples:
-        >>> import soundfile
-        >>> speech2segment = Speech2VadSegment("vad_config.yml", "vad.pt")
-        >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2segment(audio)
-        [[10, 230], [245, 450], ...]
-
-    """
-
-    def __init__(
-            self,
-            vad_infer_config: Union[Path, str] = None,
-            vad_model_file: Union[Path, str] = None,
-            vad_cmvn_file: Union[Path, str] = None,
-            device: str = "cpu",
-            batch_size: int = 1,
-            dtype: str = "float32",
-            **kwargs,
-    ):
-        assert check_argument_types()
-
-        # 1. Build vad model
-        vad_model, vad_infer_args = VADTask.build_model_from_file(
-            vad_infer_config, vad_model_file, device
-        )
-        frontend = None
-        if vad_infer_args.frontend is not None:
-            frontend = WavFrontend(cmvn_file=vad_cmvn_file, **vad_infer_args.frontend_conf)
-
-        logging.info("vad_model: {}".format(vad_model))
-        logging.info("vad_infer_args: {}".format(vad_infer_args))
-        vad_model.to(dtype=getattr(torch, dtype)).eval()
-
-        self.vad_model = vad_model
-        self.vad_infer_args = vad_infer_args
-        self.device = device
-        self.dtype = dtype
-        self.frontend = frontend
-        self.batch_size = batch_size
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            in_cache: Dict[str, torch.Tensor] = dict()
-    ) -> Tuple[List[List[int]], Dict[str, torch.Tensor]]:
-        """Inference
-
-        Args:
-            speech: Input speech data
-        Returns:
-            text, token, token_int, hyp
-
-        """
-        assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if self.frontend is not None:
-            self.frontend.filter_length_max = math.inf
-            fbanks, fbanks_len = self.frontend.forward_fbank(speech, speech_lengths)
-            feats, feats_len = self.frontend.forward_lfr_cmvn(fbanks, fbanks_len)
-            fbanks = to_device(fbanks, device=self.device)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-        else:
-            raise Exception("Need to extract feats first, please configure frontend configuration")
-
-        # b. Forward Encoder streaming
-        t_offset = 0
-        step = min(feats_len.max(), 6000)
-        segments = [[]] * self.batch_size
-        for t_offset in range(0, feats_len, min(step, feats_len - t_offset)):
-            if t_offset + step >= feats_len - 1:
-                step = feats_len - t_offset
-                is_final = True
-            else:
-                is_final = False
-            batch = {
-                "feats": feats[:, t_offset:t_offset + step, :],
-                "waveform": speech[:, t_offset * 160:min(speech.shape[-1], (t_offset + step - 1) * 160 + 400)],
-                "is_final": is_final,
-                "in_cache": in_cache
-            }
-            # a. To device
-            #batch = to_device(batch, device=self.device)
-            segments_part, in_cache = self.vad_model(**batch)
-            if segments_part:
-                for batch_num in range(0, self.batch_size):
-                    segments[batch_num] += segments_part[batch_num]
-        return fbanks, segments
 
 class Speech2VadSegmentOnline(Speech2VadSegment):
     """Speech2VadSegmentOnline class
 
     Examples:
         >>> import soundfile
         >>> speech2segment = Speech2VadSegmentOnline("vad_config.yml", "vad.pt")
@@ -213,156 +109,35 @@
         raw_inputs: Union[np.ndarray, torch.Tensor] = None,
         key_file: Optional[str] = None,
         allow_variable_data_keys: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         num_workers: int = 1,
-        online: bool = False,
-        **kwargs,
-):
-    if not online:
-        inference_pipeline = inference_modelscope(
-            batch_size=batch_size,
-            ngpu=ngpu,
-            log_level=log_level,
-            vad_infer_config=vad_infer_config,
-            vad_model_file=vad_model_file,
-            vad_cmvn_file=vad_cmvn_file,
-            key_file=key_file,
-            allow_variable_data_keys=allow_variable_data_keys,
-            output_dir=output_dir,
-            dtype=dtype,
-            seed=seed,
-            num_workers=num_workers,
-            **kwargs,
-        )
-    else:
-        inference_pipeline = inference_modelscope_online(
-            batch_size=batch_size,
-            ngpu=ngpu,
-            log_level=log_level,
-            vad_infer_config=vad_infer_config,
-            vad_model_file=vad_model_file,
-            vad_cmvn_file=vad_cmvn_file,
-            key_file=key_file,
-            allow_variable_data_keys=allow_variable_data_keys,
-            output_dir=output_dir,
-            dtype=dtype,
-            seed=seed,
-            num_workers=num_workers,
-            **kwargs,
-        )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-def inference_modelscope(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        vad_infer_config: Optional[str],
-        vad_model_file: Optional[str],
-        vad_cmvn_file: Optional[str] = None,
-        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
         **kwargs,
 ):
-    assert check_argument_types()
-    if batch_size > 1:
-        raise NotImplementedError("batch decoding is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
-
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-
-    # 2. Build speech2vadsegment
-    speech2vadsegment_kwargs = dict(
+    inference_pipeline = inference_modelscope(
+        batch_size=batch_size,
+        ngpu=ngpu,
+        log_level=log_level,
         vad_infer_config=vad_infer_config,
         vad_model_file=vad_model_file,
         vad_cmvn_file=vad_cmvn_file,
-        device=device,
+        key_file=key_file,
+        allow_variable_data_keys=allow_variable_data_keys,
+        output_dir=output_dir,
         dtype=dtype,
+        seed=seed,
+        num_workers=num_workers,
+        **kwargs,
     )
-    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
-
-    def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None
-    ):
-        # 3. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = VADTask.build_streaming_iterator(
-            data_path_and_name_and_type,
-            dtype=dtype,
-            batch_size=batch_size,
-            key_file=key_file,
-            num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
-        )
-
-        finish_count = 0
-        file_count = 1
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        if output_path is not None:
-            writer = DatadirWriter(output_path)
-            ibest_writer = writer[f"1best_recog"]
-        else:
-            writer = None
-            ibest_writer = None
-
-        vad_results = []
-        for keys, batch in loader:
-            assert isinstance(batch, dict), type(batch)
-            assert all(isinstance(s, str) for s in keys), keys
-            _bs = len(next(iter(batch.values())))
-            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-
-            # do vad segment
-            _, results = speech2vadsegment(**batch)
-            for i, _ in enumerate(keys):
-                if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
-                    results[i] = json.dumps(results[i])
-                item = {'key': keys[i], 'value': results[i]}
-                vad_results.append(item)
-                if writer is not None:
-                    ibest_writer["text"][keys[i]] = "{}".format(results[i])
-
-        return vad_results
+    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
-    return _forward
 
-def inference_modelscope_online(
+def inference_modelscope(
         batch_size: int,
         ngpu: int,
         log_level: Union[int, str],
         # data_path_and_name_and_type,
         vad_infer_config: Optional[str],
         vad_model_file: Optional[str],
         vad_cmvn_file: Optional[str] = None,
@@ -372,29 +147,30 @@
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         num_workers: int = 1,
         **kwargs,
 ):
     assert check_argument_types()
+    ncpu = kwargs.get("ncpu", 1)
+    torch.set_num_threads(ncpu)
+    
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-
+        batch_size = 1
     # 1. Set random-seed
     set_all_random_seed(seed)
 
     # 2. Build speech2vadsegment
     speech2vadsegment_kwargs = dict(
         vad_infer_config=vad_infer_config,
         vad_model_file=vad_model_file,
@@ -467,14 +243,15 @@
                         if writer is not None:
                             ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
         return vad_results
 
     return _forward
 
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="VAD Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
@@ -538,19 +315,14 @@
         help="VAD model parameter file",
     )
     group.add_argument(
         "--vad_cmvn_file",
         type=str,
         help="Global cmvn file",
     )
-    group.add_argument(
-        "--online",
-        type=str,
-        help="decoding mode",
-    )
 
     group = parser.add_argument_group("infer related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
@@ -566,8 +338,7 @@
     kwargs = vars(args)
     kwargs.pop("config", None)
     inference(**kwargs)
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `funasr-0.4.8/funasr/bin/vad_inference_launch.py` & `funasr-0.5.0/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/bin/vad_inference_online.py` & `funasr-0.5.0/funasr/tasks/vad.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,346 +1,363 @@
 import argparse
 import logging
-import os
-import sys
-import json
-from pathlib import Path
-from typing import Any
+from typing import Callable
+from typing import Collection
+from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Sequence
+from typing import Tuple
+import os
+from pathlib import Path
 from typing import Tuple
 from typing import Union
-from typing import Dict
-
+import yaml
 import numpy as np
 import torch
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.tasks.vad import VADTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
+from funasr.datasets.collate_fn import CommonCollateFn
+from funasr.datasets.preprocessor import CommonPreprocessor
+from funasr.models.ctc import CTC
+from funasr.models.decoder.abs_decoder import AbsDecoder
+from funasr.models.decoder.rnn_decoder import RNNDecoder
+from funasr.models.decoder.transformer_decoder import (
+    DynamicConvolution2DTransformerDecoder,  # noqa: H301
+)
+from funasr.models.decoder.transformer_decoder import DynamicConvolutionTransformerDecoder
+from funasr.models.decoder.transformer_decoder import (
+    LightweightConvolution2DTransformerDecoder,  # noqa: H301
+)
+from funasr.models.decoder.transformer_decoder import (
+    LightweightConvolutionTransformerDecoder,  # noqa: H301
+)
+from funasr.models.decoder.transformer_decoder import TransformerDecoder
+from funasr.models.encoder.abs_encoder import AbsEncoder
+from funasr.models.encoder.conformer_encoder import ConformerEncoder
+from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
+from funasr.models.encoder.rnn_encoder import RNNEncoder
+from funasr.models.encoder.transformer_encoder import TransformerEncoder
+from funasr.models.frontend.abs_frontend import AbsFrontend
+from funasr.models.frontend.default import DefaultFrontend
+from funasr.models.frontend.fused import FusedFrontends
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
+from funasr.models.frontend.s3prl import S3prlFrontend
+from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
+from funasr.models.postencoder.hugging_face_transformers_postencoder import (
+    HuggingFaceTransformersPostEncoder,  # noqa: H301
+)
+from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
+from funasr.models.preencoder.linear import LinearProjection
+from funasr.models.preencoder.sinc import LightweightSincConvs
+from funasr.models.specaug.abs_specaug import AbsSpecAug
+from funasr.models.specaug.specaug import SpecAug
+from funasr.layers.abs_normalize import AbsNormalize
+from funasr.layers.global_mvn import GlobalMVN
+from funasr.layers.utterance_mvn import UtteranceMVN
+from funasr.tasks.abs_task import AbsTask
+from funasr.text.phoneme_tokenizer import g2p_choices
+from funasr.train.abs_espnet_model import AbsESPnetModel
+from funasr.train.class_choices import ClassChoices
+from funasr.train.trainer import Trainer
+from funasr.utils.get_default_kwargs import get_default_kwargs
+from funasr.utils.nested_dict_action import NestedDictAction
+from funasr.utils.types import float_or_none
+from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.models.frontend.wav_frontend import WavFrontendOnline
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.bin.vad_inference import Speech2VadSegment
-
-header_colors = '\033[95m'
-end_colors = '\033[0m'
-
-
-class Speech2VadSegmentOnline(Speech2VadSegment):
-    """Speech2VadSegmentOnline class
-
-    Examples:
-        >>> import soundfile
-        >>> speech2segment = Speech2VadSegmentOnline("vad_config.yml", "vad.pt")
-        >>> audio, rate = soundfile.read("speech.wav")
-        >>> speech2segment(audio)
-        [[10, 230], [245, 450], ...]
-
-    """
-    def __init__(self, **kwargs):
-        super(Speech2VadSegmentOnline, self).__init__(**kwargs)
-        vad_cmvn_file = kwargs.get('vad_cmvn_file', None)
-        self.frontend = None
-        if self.vad_infer_args.frontend is not None:
-            self.frontend = WavFrontendOnline(cmvn_file=vad_cmvn_file, **self.vad_infer_args.frontend_conf)
-
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False, max_end_sil: int = 800
-    ) -> Tuple[torch.Tensor, List[List[int]], torch.Tensor]:
-        """Inference
 
-        Args:
-            speech: Input speech data
-        Returns:
-            text, token, token_int, hyp
+from funasr.models.specaug.specaug import SpecAugLFR
+from funasr.models.predictor.cif import CifPredictor, CifPredictorV2
+from funasr.modules.subsampling import Conv1dSubsampling
+from funasr.models.e2e_vad import E2EVadModel
+from funasr.models.encoder.fsmn_encoder import FSMN
+
+frontend_choices = ClassChoices(
+    name="frontend",
+    classes=dict(
+        default=DefaultFrontend,
+        sliding_window=SlidingWindow,
+        s3prl=S3prlFrontend,
+        fused=FusedFrontends,
+        wav_frontend=WavFrontend,
+        wav_frontend_online=WavFrontendOnline,
+    ),
+    type_check=AbsFrontend,
+    default="default",
+)
+specaug_choices = ClassChoices(
+    name="specaug",
+    classes=dict(
+        specaug=SpecAug,
+        specaug_lfr=SpecAugLFR,
+    ),
+    type_check=AbsSpecAug,
+    default=None,
+    optional=True,
+)
+normalize_choices = ClassChoices(
+    "normalize",
+    classes=dict(
+        global_mvn=GlobalMVN,
+        utterance_mvn=UtteranceMVN,
+    ),
+    type_check=AbsNormalize,
+    default=None,
+    optional=True,
+)
+model_choices = ClassChoices(
+    "model",
+    classes=dict(
+        e2evad=E2EVadModel,
+    ),
+    type_check=object,
+    default="e2evad",
+)
+
+encoder_choices = ClassChoices(
+    "encoder",
+    classes=dict(
+        fsmn=FSMN,
+    ),
+    type_check=torch.nn.Module,
+    default="fsmn",
+)
+
+
+class VADTask(AbsTask):
+    # If you need more than one optimizers, change this value
+    num_optimizers: int = 1
+
+    # Add variable objects configurations
+    class_choices_list = [
+        # --frontend and --frontend_conf
+        frontend_choices,
+        # --model and --model_conf
+        model_choices,
+    ]
+
+    # If you need to modify train() or eval() procedures, change Trainer class here
+    trainer = Trainer
+
+    @classmethod
+    def add_task_arguments(cls, parser: argparse.ArgumentParser):
+        group = parser.add_argument_group(description="Task related")
+
+        # NOTE(kamo): add_arguments(..., required=True) can't be used
+        # to provide --print_config mode. Instead of it, do as
+        # required = parser.get_default("required")
+        # required += ["token_list"]
+
+        group.add_argument(
+            "--init",
+            type=lambda x: str_or_none(x.lower()),
+            default=None,
+            help="The initialization method",
+            choices=[
+                "chainer",
+                "xavier_uniform",
+                "xavier_normal",
+                "kaiming_uniform",
+                "kaiming_normal",
+                None,
+            ],
+        )
 
-        """
+        group.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of input dimension of the feature",
+        )
+
+        group = parser.add_argument_group(description="Preprocess related")
+        parser.add_argument(
+            "--speech_volume_normalize",
+            type=float_or_none,
+            default=None,
+            help="Scale the maximum amplitude to the given value.",
+        )
+        parser.add_argument(
+            "--rir_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of rir scp file.",
+        )
+        parser.add_argument(
+            "--rir_apply_prob",
+            type=float,
+            default=1.0,
+            help="THe probability for applying RIR convolution.",
+        )
+        parser.add_argument(
+            "--cmvn_file",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_scp",
+            type=str_or_none,
+            default=None,
+            help="The file path of noise scp file.",
+        )
+        parser.add_argument(
+            "--noise_apply_prob",
+            type=float,
+            default=1.0,
+            help="The probability applying Noise adding.",
+        )
+        parser.add_argument(
+            "--noise_db_range",
+            type=str,
+            default="13_15",
+            help="The range of noise decibel level.",
+        )
+
+        for class_choices in cls.class_choices_list:
+            # Append --<name> and --<name>_conf.
+            # e.g. --encoder and --encoder_conf
+            class_choices.add_arguments(group)
+
+    @classmethod
+    def build_collate_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Callable[
+        [Collection[Tuple[str, Dict[str, np.ndarray]]]],
+        Tuple[List[str], Dict[str, torch.Tensor]],
+    ]:
         assert check_argument_types()
+        # NOTE(kamo): int value = 0 is reserved by CTC-blank symbol
+        return CommonCollateFn(float_pad_value=0.0, int_pad_value=-1)
 
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-        batch_size = speech.shape[0]
-        segments = [[]] * batch_size
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths, is_final)
-            fbanks, _ = self.frontend.get_fbank()
+    @classmethod
+    def build_preprocess_fn(
+            cls, args: argparse.Namespace, train: bool
+    ) -> Optional[Callable[[str, Dict[str, np.array]], Dict[str, np.ndarray]]]:
+        assert check_argument_types()
+        # if args.use_preprocessor:
+        #    retval = CommonPreprocessor(
+        #        train=train,
+        #        # NOTE(kamo): Check attribute existence for backward compatibility
+        #        rir_scp=args.rir_scp if hasattr(args, "rir_scp") else None,
+        #        rir_apply_prob=args.rir_apply_prob
+        #        if hasattr(args, "rir_apply_prob")
+        #        else 1.0,
+        #        noise_scp=args.noise_scp if hasattr(args, "noise_scp") else None,
+        #        noise_apply_prob=args.noise_apply_prob
+        #        if hasattr(args, "noise_apply_prob")
+        #        else 1.0,
+        #        noise_db_range=args.noise_db_range
+        #        if hasattr(args, "noise_db_range")
+        #        else "13_15",
+        #        speech_volume_normalize=args.speech_volume_normalize
+        #        if hasattr(args, "rir_scp")
+        #        else None,
+        #    )
+        # else:
+        #    retval = None
+        retval = None
+        assert check_return_type(retval)
+        return retval
+
+    @classmethod
+    def required_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        if not inference:
+            retval = ("speech", "text")
         else:
-            raise Exception("Need to extract feats first, please configure frontend configuration")
-        if feats.shape[0]:
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            waveforms = self.frontend.get_waveforms()
-
-            batch = {
-                "feats": feats,
-                "waveform": waveforms,
-                "in_cache": in_cache,
-                "is_final": is_final,
-                "max_end_sil": max_end_sil
-            }
-            # a. To device
-            batch = to_device(batch, device=self.device)
-            segments, in_cache = self.vad_model.forward_online(**batch)
-            # in_cache.update(batch['in_cache'])
-            # in_cache = {key: value for key, value in batch['in_cache'].items()}
-        return fbanks, segments, in_cache
-
-
-def inference(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        data_path_and_name_and_type,
-        vad_infer_config: Optional[str],
-        vad_model_file: Optional[str],
-        vad_cmvn_file: Optional[str] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        **kwargs,
-):
-    inference_pipeline = inference_modelscope(
-        batch_size=batch_size,
-        ngpu=ngpu,
-        log_level=log_level,
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        key_file=key_file,
-        allow_variable_data_keys=allow_variable_data_keys,
-        output_dir=output_dir,
-        dtype=dtype,
-        seed=seed,
-        num_workers=num_workers,
-        **kwargs,
-    )
-    return inference_pipeline(data_path_and_name_and_type, raw_inputs)
-
-
-def inference_modelscope(
-        batch_size: int,
-        ngpu: int,
-        log_level: Union[int, str],
-        # data_path_and_name_and_type,
-        vad_infer_config: Optional[str],
-        vad_model_file: Optional[str],
-        vad_cmvn_file: Optional[str] = None,
-        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        key_file: Optional[str] = None,
-        allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
-        dtype: str = "float32",
-        seed: int = 0,
-        num_workers: int = 1,
-        **kwargs,
-):
-    assert check_argument_types()
-    ncpu = kwargs.get("ncpu", 1)
-    torch.set_num_threads(ncpu)
-    
-    if batch_size > 1:
-        raise NotImplementedError("batch decoding is not implemented")
-    if ngpu > 1:
-        raise NotImplementedError("only single GPU decoding is supported")
-
-    logging.basicConfig(
-        level=log_level,
-        format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
-    )
-
-    if ngpu >= 1 and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    # 1. Set random-seed
-    set_all_random_seed(seed)
-
-    # 2. Build speech2vadsegment
-    speech2vadsegment_kwargs = dict(
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        device=device,
-        dtype=dtype,
-    )
-    logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegmentOnline(**speech2vadsegment_kwargs)
-
-    def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None,
-    ):
-        # 3. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = VADTask.build_streaming_iterator(
-            data_path_and_name_and_type,
-            dtype=dtype,
-            batch_size=batch_size,
-            key_file=key_file,
-            num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
-        )
+            # Recognition mode
+            retval = ("speech",)
+        return retval
+
+    @classmethod
+    def optional_data_names(
+            cls, train: bool = True, inference: bool = False
+    ) -> Tuple[str, ...]:
+        retval = ()
+        assert check_return_type(retval)
+        return retval
 
-        finish_count = 0
-        file_count = 1
-        # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        if output_path is not None:
-            writer = DatadirWriter(output_path)
-            ibest_writer = writer[f"1best_recog"]
+    @classmethod
+    def build_model(cls, args: argparse.Namespace):
+        assert check_argument_types()
+        # 4. Encoder
+        encoder_class = encoder_choices.get_class(args.encoder)
+        encoder = encoder_class(**args.encoder_conf)
+
+        # 5. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("e2evad")
+        
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            if args.frontend == 'wav_frontend':
+                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
+            else:
+                frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
         else:
-            writer = None
-            ibest_writer = None
+            # Give features from data-loader
+            args.frontend = None
+            args.frontend_conf = {}
+            frontend = None
+            input_size = args.input_size
+        
+        model = model_class(encoder=encoder, vad_post_args=args.vad_post_conf, frontend=frontend)
+
+        return model
+
+    # ~~~~~~~~~ The methods below are mainly used for inference ~~~~~~~~~
+    @classmethod
+    def build_model_from_file(
+            cls,
+            config_file: Union[Path, str] = None,
+            model_file: Union[Path, str] = None,
+            device: str = "cpu",
+            cmvn_file: Union[Path, str] = None,
+    ):
+        """Build model from the files.
+
+        This method is used for inference or fine-tuning.
+
+        Args:
+            config_file: The yaml file saved when training.
+            model_file: The model file saved when training.
+            device: Device type, "cpu", "cuda", or "cuda:N".
 
-        vad_results = []
-        batch_in_cache = param_dict['in_cache'] if param_dict is not None else dict()
-        is_final = param_dict.get('is_final', False) if param_dict is not None else False
-        max_end_sil = param_dict.get('max_end_sil', 800) if param_dict is not None else 800
-        for keys, batch in loader:
-            assert isinstance(batch, dict), type(batch)
-            assert all(isinstance(s, str) for s in keys), keys
-            _bs = len(next(iter(batch.values())))
-            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            batch['in_cache'] = batch_in_cache
-            batch['is_final'] = is_final
-            batch['max_end_sil'] = max_end_sil
-
-            # do vad segment
-            _, results, param_dict['in_cache'] = speech2vadsegment(**batch)
-            # param_dict['in_cache'] = batch['in_cache']
-            if results:
-                for i, _ in enumerate(keys):
-                    if results[i]:
-                        if "MODELSCOPE_ENVIRONMENT" in os.environ and os.environ["MODELSCOPE_ENVIRONMENT"] == "eas":
-                            results[i] = json.dumps(results[i])
-                        item = {'key': keys[i], 'value': results[i]}
-                        vad_results.append(item)
-                        if writer is not None:
-                            ibest_writer["text"][keys[i]] = "{}".format(results[i])
-
-        return vad_results
-
-    return _forward
-
-
-def get_parser():
-    parser = config_argparse.ArgumentParser(
-        description="VAD Decoding",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    # Note(kamo): Use '_' instead of '-' as separator.
-    # '-' is confusing if written in yaml.
-    parser.add_argument(
-        "--log_level",
-        type=lambda x: x.upper(),
-        default="INFO",
-        choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
-        help="The verbose level of logging",
-    )
-
-    parser.add_argument("--output_dir", type=str, required=False)
-    parser.add_argument(
-        "--ngpu",
-        type=int,
-        default=0,
-        help="The number of gpus. 0 indicates CPU mode",
-    )
-    parser.add_argument(
-        "--gpuid_list",
-        type=str,
-        default="",
-        help="The visible gpus",
-    )
-    parser.add_argument("--seed", type=int, default=0, help="Random seed")
-    parser.add_argument(
-        "--dtype",
-        default="float32",
-        choices=["float16", "float32", "float64"],
-        help="Data type",
-    )
-    parser.add_argument(
-        "--num_workers",
-        type=int,
-        default=1,
-        help="The number of workers used for DataLoader",
-    )
-
-    group = parser.add_argument_group("Input data related")
-    group.add_argument(
-        "--data_path_and_name_and_type",
-        type=str2triple_str,
-        required=False,
-        action="append",
-    )
-    group.add_argument("--raw_inputs", type=list, default=None)
-    # example=[{'key':'EdevDEWdIYQ_0021','file':'/mnt/data/jiangyu.xzy/test_data/speech_io/SPEECHIO_ASR_ZH00007_zhibodaihuo/wav/EdevDEWdIYQ_0021.wav'}])
-    group.add_argument("--key_file", type=str_or_none)
-    group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
-
-    group = parser.add_argument_group("The model configuration related")
-    group.add_argument(
-        "--vad_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--vad_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
-    group.add_argument(
-        "--vad_cmvn_file",
-        type=str,
-        help="Global cmvn file",
-    )
-
-    group = parser.add_argument_group("infer related")
-    group.add_argument(
-        "--batch_size",
-        type=int,
-        default=1,
-        help="The batch size for inference",
-    )
-
-    return parser
-
-
-def main(cmd=None):
-    print(get_commandline_args(), file=sys.stderr)
-    parser = get_parser()
-    args = parser.parse_args(cmd)
-    kwargs = vars(args)
-    kwargs.pop("config", None)
-    inference(**kwargs)
+        """
+        assert check_argument_types()
+        if config_file is None:
+            assert model_file is not None, (
+                "The argument 'model_file' must be provided "
+                "if the argument 'config_file' is not specified."
+            )
+            config_file = Path(model_file).parent / "config.yaml"
+        else:
+            config_file = Path(config_file)
 
+        with config_file.open("r", encoding="utf-8") as f:
+            args = yaml.safe_load(f)
+        #if cmvn_file is not None:
+        args["cmvn_file"] = cmvn_file
+        args = argparse.Namespace(**args)
+        model = cls.build_model(args)
+        model.to(device)
+        model_dict = dict()
+        model_name_pth = None
+        if model_file is not None:
+            logging.info("model_file is {}".format(model_file))
+            if device == "cuda":
+                device = f"cuda:{torch.cuda.current_device()}"
+            model_dir = os.path.dirname(model_file)
+            model_name = os.path.basename(model_file)
+            model_dict = torch.load(model_file, map_location=device)
+        model.encoder.load_state_dict(model_dict)
 
-if __name__ == "__main__":
-    main()
+        return model, args
```

### Comparing `funasr-0.4.8/funasr/datasets/collate_fn.py` & `funasr-0.5.0/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/dataset.py` & `funasr-0.5.0/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/iterable_dataset.py` & `funasr-0.5.0/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/iterable_dataset_modelscope.py` & `funasr-0.5.0/funasr/datasets/iterable_dataset_modelscope.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.5.0/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.5.0/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.5.0/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/dataset.py` & `funasr-0.5.0/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.5.0/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.5.0/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.5.0/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.5.0/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.5.0/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.5.0/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/ms_dataset.py` & `funasr-0.5.0/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/datasets/preprocessor.py` & `funasr-0.5.0/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/export_model.py` & `funasr-0.5.0/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/CT_Transformer.py` & `funasr-0.5.0/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/__init__.py` & `funasr-0.5.0/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.5.0/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.5.0/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.5.0/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/e2e_vad.py` & `funasr-0.5.0/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.5.0/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.5.0/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.5.0/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/modules/decoder_layer.py` & `funasr-0.5.0/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/modules/encoder_layer.py` & `funasr-0.5.0/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/modules/feedforward.py` & `funasr-0.5.0/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/modules/multihead_att.py` & `funasr-0.5.0/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/models/predictor/cif.py` & `funasr-0.5.0/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/test/test_onnx.py` & `funasr-0.5.0/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/test/test_onnx_punc.py` & `funasr-0.5.0/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.5.0/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/test/test_onnx_vad.py` & `funasr-0.5.0/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/export/utils/torch_function.py` & `funasr-0.5.0/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/fileio/datadir_writer.py` & `funasr-0.5.0/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/fileio/npy_scp.py` & `funasr-0.5.0/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/fileio/rand_gen_dataset.py` & `funasr-0.5.0/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/fileio/read_text.py` & `funasr-0.5.0/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/fileio/sound_scp.py` & `funasr-0.5.0/funasr/fileio/sound_scp.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,21 +42,23 @@
         self.dest_sample_rate = dest_sample_rate
 
     def __getitem__(self, key):
         wav = self.data[key]
         if self.normalize:
             # soundfile.read normalizes data to [-1,1] if dtype is not given
             array, rate = librosa.load(
-                wav, sr=self.dest_sample_rate, mono=not self.always_2d
+                wav, sr=self.dest_sample_rate, mono=self.always_2d
             )
         else:
             array, rate = librosa.load(
-                wav, sr=self.dest_sample_rate, mono=not self.always_2d, dtype=self.dtype
+                wav, sr=self.dest_sample_rate, mono=self.always_2d, dtype=self.dtype
             )
 
+        if array.ndim==2:
+            array=array.transpose((1, 0))
         return rate, array
 
     def get_path(self, key):
         return self.data[key]
 
     def __contains__(self, item):
         return item
```

### Comparing `funasr-0.4.8/funasr/iterators/chunk_iter_factory.py` & `funasr-0.5.0/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/iterators/multiple_iter_factory.py` & `funasr-0.5.0/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/iterators/sequence_iter_factory.py` & `funasr-0.5.0/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/complex_utils.py` & `funasr-0.5.0/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/global_mvn.py` & `funasr-0.5.0/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/label_aggregation.py` & `funasr-0.5.0/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/log_mel.py` & `funasr-0.5.0/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/mask_along_axis.py` & `funasr-0.5.0/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/sinc_conv.py` & `funasr-0.5.0/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/stft.py` & `funasr-0.5.0/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/time_warp.py` & `funasr-0.5.0/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/layers/utterance_mvn.py` & `funasr-0.5.0/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/lm/abs_model.py` & `funasr-0.5.0/funasr/lm/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/lm/seq_rnn_lm.py` & `funasr-0.5.0/funasr/lm/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/lm/transformer_lm.py` & `funasr-0.5.0/funasr/lm/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/losses/label_smoothing_loss.py` & `funasr-0.5.0/funasr/losses/label_smoothing_loss.py`

 * *Files 22% similar despite different names*

```diff
@@ -75,7 +75,53 @@
         self.criterion = criterion
 
     def forward(self, pred, label, lengths):
         pad_mask = make_pad_mask(lengths, maxlen=pred.shape[1])
         loss = self.criterion(pred, label)
         denom = (~pad_mask).sum() if self.normalize_length else pred.shape[0]
         return loss.masked_fill(pad_mask, 0).sum() / denom
+
+
+class NllLoss(nn.Module):
+    """Nll loss.
+
+    :param int size: the number of class
+    :param int padding_idx: ignored class id
+    :param bool normalize_length: normalize loss by sequence length if True
+    :param torch.nn.Module criterion: loss function
+    """
+
+    def __init__(
+        self,
+        size,
+        padding_idx,
+        normalize_length=False,
+        criterion=nn.NLLLoss(reduction='none'),
+    ):
+        """Construct an NllLoss object."""
+        super(NllLoss, self).__init__()
+        self.criterion = criterion
+        self.padding_idx = padding_idx
+        self.size = size
+        self.true_dist = None
+        self.normalize_length = normalize_length
+
+    def forward(self, x, target):
+        """Compute loss between x and target.
+
+        :param torch.Tensor x: prediction (batch, seqlen, class)
+        :param torch.Tensor target:
+            target signal masked with self.padding_id (batch, seqlen)
+        :return: scalar float value
+        :rtype torch.Tensor
+        """
+        assert x.size(2) == self.size
+        batch_size = x.size(0)
+        x = x.view(-1, self.size)
+        target = target.view(-1)
+        with torch.no_grad():
+            ignore = target == self.padding_idx  # (B,)
+            total = len(target) - ignore.sum().item()
+            target = target.masked_fill(ignore, 0)  # avoid -1 index
+        kl = self.criterion(x , target)
+        denom = total if self.normalize_length else batch_size
+        return kl.masked_fill(ignore, 0).sum() / denom
```

### Comparing `funasr-0.4.8/funasr/main_funcs/average_nbest_models.py` & `funasr-0.5.0/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.5.0/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/main_funcs/collect_stats.py` & `funasr-0.5.0/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/main_funcs/pack_funcs.py` & `funasr-0.5.0/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/ctc.py` & `funasr-0.5.0/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/data2vec.py` & `funasr-0.5.0/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/decoder/contextual_decoder.py` & `funasr-0.5.0/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/decoder/rnn_decoder.py` & `funasr-0.5.0/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.5.0/funasr/models/decoder/rnnt_decoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         embed_size: int = 256,
         hidden_size: int = 256,
         rnn_type: str = "lstm",
         num_layers: int = 1,
         dropout_rate: float = 0.0,
         embed_dropout_rate: float = 0.0,
         embed_pad: int = 0,
+        use_embed_mask: bool = False,
     ) -> None:
         """Construct a RNNDecoder object."""
         super().__init__()
 
         assert check_argument_types()
 
         if rnn_type not in ("lstm", "gru"):
@@ -62,14 +63,23 @@
         self.dtype = rnn_type
 
         self.output_size = hidden_size
         self.vocab_size = vocab_size
 
         self.device = next(self.parameters()).device
         self.score_cache = {}
+
+        self.use_embed_mask = use_embed_mask
+        if self.use_embed_mask:
+            self._embed_mask = SpecAug(
+                time_mask_width_range=3,
+                num_time_mask=4,
+                apply_freq_mask=False,
+                apply_time_warp=False
+            )
     
     def forward(
         self,
         labels: torch.Tensor,
         label_lens: torch.Tensor,
         states: Optional[Tuple[torch.Tensor, Optional[torch.Tensor]]] = None,
     ) -> torch.Tensor:
@@ -84,14 +94,16 @@
             dec_out: Decoder output sequences. (B, U, D_dec)
 
         """
         if states is None:
             states = self.init_state(labels.size(0))
 
         dec_embed = self.dropout_embed(self.embed(labels))
+        if self.use_embed_mask and self.training:
+            dec_embed = self._embed_mask(dec_embed, label_lens)[0]
         dec_out, states = self.rnn_forward(dec_embed, states)
         return dec_out
 
     def rnn_forward(
         self,
         x: torch.Tensor,
         state: Tuple[torch.Tensor, Optional[torch.Tensor]],
```

### Comparing `funasr-0.4.8/funasr/models/decoder/sanm_decoder.py` & `funasr-0.5.0/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/decoder/sv_decoder.py` & `funasr-0.5.0/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/decoder/transformer_decoder.py` & `funasr-0.5.0/funasr/models/decoder/transformer_decoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import torch
 from torch import nn
 from typeguard import check_argument_types
 
 from funasr.models.decoder.abs_decoder import AbsDecoder
 from funasr.modules.attention import MultiHeadedAttention
+from funasr.modules.attention import CosineDistanceAttention
 from funasr.modules.dynamic_conv import DynamicConvolution
 from funasr.modules.dynamic_conv2d import DynamicConvolution2D
 from funasr.modules.embedding import PositionalEncoding
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.lightconv import LightweightConvolution
 from funasr.modules.lightconv2d import LightweightConvolution2D
 from funasr.modules.mask import subsequent_mask
@@ -759,8 +760,433 @@
                     attention_heads, attention_dim, src_attention_dropout_rate
                 ),
                 PositionwiseFeedForward(attention_dim, linear_units, dropout_rate),
                 dropout_rate,
                 normalize_before,
                 concat_after,
             ),
-        )
+        )
+
+class BaseSAAsrTransformerDecoder(AbsDecoder, BatchScorerInterface):
+    
+    def __init__(
+        self,
+        vocab_size: int,
+        encoder_output_size: int,
+        spker_embedding_dim: int = 256,
+        dropout_rate: float = 0.1,
+        positional_dropout_rate: float = 0.1,
+        input_layer: str = "embed",
+        use_asr_output_layer: bool = True,
+        use_spk_output_layer: bool = True,
+        pos_enc_class=PositionalEncoding,
+        normalize_before: bool = True,
+    ):
+        assert check_argument_types()
+        super().__init__()
+        attention_dim = encoder_output_size
+
+        if input_layer == "embed":
+            self.embed = torch.nn.Sequential(
+                torch.nn.Embedding(vocab_size, attention_dim),
+                pos_enc_class(attention_dim, positional_dropout_rate),
+            )
+        elif input_layer == "linear":
+            self.embed = torch.nn.Sequential(
+                torch.nn.Linear(vocab_size, attention_dim),
+                torch.nn.LayerNorm(attention_dim),
+                torch.nn.Dropout(dropout_rate),
+                torch.nn.ReLU(),
+                pos_enc_class(attention_dim, positional_dropout_rate),
+            )
+        else:
+            raise ValueError(f"only 'embed' or 'linear' is supported: {input_layer}")
+
+        self.normalize_before = normalize_before
+        if self.normalize_before:
+            self.after_norm = LayerNorm(attention_dim)
+        if use_asr_output_layer:
+            self.asr_output_layer = torch.nn.Linear(attention_dim, vocab_size)
+        else:
+            self.asr_output_layer = None
+
+        if use_spk_output_layer:
+            self.spk_output_layer = torch.nn.Linear(attention_dim, spker_embedding_dim)
+        else:
+            self.spk_output_layer = None
+
+        self.cos_distance_att = CosineDistanceAttention()
+
+        self.decoder1 = None
+        self.decoder2 = None
+        self.decoder3 = None
+        self.decoder4 = None
+
+    def forward(
+        self,
+        asr_hs_pad: torch.Tensor,
+        spk_hs_pad: torch.Tensor,
+        hlens: torch.Tensor,
+        ys_in_pad: torch.Tensor,
+        ys_in_lens: torch.Tensor,
+        profile: torch.Tensor,
+        profile_lens: torch.Tensor,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        
+        tgt = ys_in_pad
+        # tgt_mask: (B, 1, L)
+        tgt_mask = (~make_pad_mask(ys_in_lens)[:, None, :]).to(tgt.device)
+        # m: (1, L, L)
+        m = subsequent_mask(tgt_mask.size(-1), device=tgt_mask.device).unsqueeze(0)
+        # tgt_mask: (B, L, L)
+        tgt_mask = tgt_mask & m
+
+        asr_memory = asr_hs_pad
+        spk_memory = spk_hs_pad
+        memory_mask = (~make_pad_mask(hlens))[:, None, :].to(asr_memory.device)
+        # Spk decoder
+        x = self.embed(tgt)
+
+        x, tgt_mask, asr_memory, spk_memory, memory_mask, z = self.decoder1(
+            x, tgt_mask, asr_memory, spk_memory, memory_mask
+        )
+        x, tgt_mask, spk_memory, memory_mask = self.decoder2(
+            x, tgt_mask, spk_memory, memory_mask
+        )
+        if self.normalize_before:
+            x = self.after_norm(x)
+        if self.spk_output_layer is not None:
+            x = self.spk_output_layer(x)
+        dn, weights = self.cos_distance_att(x, profile, profile_lens)
+        # Asr decoder
+        x, tgt_mask, asr_memory, memory_mask = self.decoder3(
+            z, tgt_mask, asr_memory, memory_mask, dn
+        )
+        x, tgt_mask, asr_memory, memory_mask = self.decoder4(
+            x, tgt_mask, asr_memory, memory_mask
+        )
+
+        if self.normalize_before:
+            x = self.after_norm(x)
+        if self.asr_output_layer is not None:
+            x = self.asr_output_layer(x)
+
+        olens = tgt_mask.sum(1)
+        return x, weights, olens
+
+
+    def forward_one_step(
+        self,
+        tgt: torch.Tensor,
+        tgt_mask: torch.Tensor,
+        asr_memory: torch.Tensor,
+        spk_memory: torch.Tensor,
+        profile: torch.Tensor,
+        cache: List[torch.Tensor] = None,
+    ) -> Tuple[torch.Tensor, List[torch.Tensor]]:
+        
+        x = self.embed(tgt)
+
+        if cache is None:
+            cache = [None] * (2 + len(self.decoder2) + len(self.decoder4))
+        new_cache = []
+        x, tgt_mask, asr_memory, spk_memory, _, z = self.decoder1(
+                x, tgt_mask, asr_memory, spk_memory, None, cache=cache[0]
+        )
+        new_cache.append(x)
+        for c, decoder in zip(cache[1: len(self.decoder2) + 1], self.decoder2):
+            x, tgt_mask, spk_memory, _ = decoder(
+                x, tgt_mask, spk_memory, None, cache=c
+            )
+            new_cache.append(x)
+        if self.normalize_before:
+            x = self.after_norm(x)
+        else:
+            x = x
+        if self.spk_output_layer is not None:
+            x = self.spk_output_layer(x)
+        dn, weights = self.cos_distance_att(x, profile, None)
+
+        x, tgt_mask, asr_memory, _ = self.decoder3(
+            z, tgt_mask, asr_memory, None, dn, cache=cache[len(self.decoder2) + 1]
+        )
+        new_cache.append(x)
+
+        for c, decoder in zip(cache[len(self.decoder2) + 2: ], self.decoder4):
+            x, tgt_mask, asr_memory, _ = decoder(
+                x, tgt_mask, asr_memory, None, cache=c
+            )
+            new_cache.append(x)
+
+        if self.normalize_before:
+            y = self.after_norm(x[:, -1])
+        else:
+            y = x[:, -1]
+        if self.asr_output_layer is not None:
+            y = torch.log_softmax(self.asr_output_layer(y), dim=-1)
+
+        return y, weights, new_cache
+
+    def score(self, ys, state, asr_enc, spk_enc, profile):
+        """Score."""
+        ys_mask = subsequent_mask(len(ys), device=ys.device).unsqueeze(0)
+        logp, weights, state = self.forward_one_step(
+            ys.unsqueeze(0), ys_mask, asr_enc.unsqueeze(0), spk_enc.unsqueeze(0), profile.unsqueeze(0), cache=state
+        )
+        return logp.squeeze(0), weights.squeeze(), state
+
+class SAAsrTransformerDecoder(BaseSAAsrTransformerDecoder):
+    def __init__(
+        self,
+        vocab_size: int,
+        encoder_output_size: int,
+        spker_embedding_dim: int = 256,
+        attention_heads: int = 4,
+        linear_units: int = 2048,
+        asr_num_blocks: int = 6,
+        spk_num_blocks: int = 3,
+        dropout_rate: float = 0.1,
+        positional_dropout_rate: float = 0.1,
+        self_attention_dropout_rate: float = 0.0,
+        src_attention_dropout_rate: float = 0.0,
+        input_layer: str = "embed",
+        use_asr_output_layer: bool = True,
+        use_spk_output_layer: bool = True,
+        pos_enc_class=PositionalEncoding,
+        normalize_before: bool = True,
+        concat_after: bool = False,
+    ):
+        assert check_argument_types()
+        super().__init__(
+            vocab_size=vocab_size,
+            encoder_output_size=encoder_output_size,
+            spker_embedding_dim=spker_embedding_dim,
+            dropout_rate=dropout_rate,
+            positional_dropout_rate=positional_dropout_rate,
+            input_layer=input_layer,
+            use_asr_output_layer=use_asr_output_layer,
+            use_spk_output_layer=use_spk_output_layer,
+            pos_enc_class=pos_enc_class,
+            normalize_before=normalize_before,
+        )
+
+        attention_dim = encoder_output_size
+
+        self.decoder1 = SpeakerAttributeSpkDecoderFirstLayer(
+            attention_dim,
+            MultiHeadedAttention(
+                attention_heads, attention_dim, self_attention_dropout_rate
+            ),
+            MultiHeadedAttention(
+                attention_heads, attention_dim, src_attention_dropout_rate
+            ),
+            PositionwiseFeedForward(attention_dim, linear_units, dropout_rate),
+            dropout_rate,
+            normalize_before,
+            concat_after,
+        )
+        self.decoder2 = repeat(
+            spk_num_blocks - 1,
+            lambda lnum: DecoderLayer(
+                attention_dim,
+                MultiHeadedAttention(
+                    attention_heads, attention_dim, self_attention_dropout_rate
+                ),
+                MultiHeadedAttention(
+                    attention_heads, attention_dim, src_attention_dropout_rate
+                ),
+                PositionwiseFeedForward(attention_dim, linear_units, dropout_rate),
+                dropout_rate,
+                normalize_before,
+                concat_after,
+            ),
+        )
+        
+        
+        self.decoder3 = SpeakerAttributeAsrDecoderFirstLayer(
+            attention_dim,
+            spker_embedding_dim,
+            MultiHeadedAttention(
+                attention_heads, attention_dim, src_attention_dropout_rate
+            ),
+            PositionwiseFeedForward(attention_dim, linear_units, dropout_rate),
+            dropout_rate,
+            normalize_before,
+            concat_after,
+        )
+        self.decoder4 = repeat(
+            asr_num_blocks - 1,
+            lambda lnum: DecoderLayer(
+                attention_dim,
+                MultiHeadedAttention(
+                    attention_heads, attention_dim, self_attention_dropout_rate
+                ),
+                MultiHeadedAttention(
+                    attention_heads, attention_dim, src_attention_dropout_rate
+                ),
+                PositionwiseFeedForward(attention_dim, linear_units, dropout_rate),
+                dropout_rate,
+                normalize_before,
+                concat_after,
+            ),
+        )
+
+class SpeakerAttributeSpkDecoderFirstLayer(nn.Module):
+
+    def __init__(
+        self,
+        size,
+        self_attn,
+        src_attn,
+        feed_forward,
+        dropout_rate,
+        normalize_before=True,
+        concat_after=False,
+    ):
+        """Construct an DecoderLayer object."""
+        super(SpeakerAttributeSpkDecoderFirstLayer, self).__init__()
+        self.size = size
+        self.self_attn = self_attn
+        self.src_attn = src_attn
+        self.feed_forward = feed_forward
+        self.norm1 = LayerNorm(size)
+        self.norm2 = LayerNorm(size)
+        self.dropout = nn.Dropout(dropout_rate)
+        self.normalize_before = normalize_before
+        self.concat_after = concat_after
+        if self.concat_after:
+            self.concat_linear1 = nn.Linear(size + size, size)
+            self.concat_linear2 = nn.Linear(size + size, size)
+
+    def forward(self, tgt, tgt_mask, asr_memory, spk_memory, memory_mask, cache=None):
+        
+        residual = tgt
+        if self.normalize_before:
+            tgt = self.norm1(tgt)
+
+        if cache is None:
+            tgt_q = tgt
+            tgt_q_mask = tgt_mask
+        else:
+            # compute only the last frame query keeping dim: max_time_out -> 1
+            assert cache.shape == (
+                tgt.shape[0],
+                tgt.shape[1] - 1,
+                self.size,
+            ), f"{cache.shape} == {(tgt.shape[0], tgt.shape[1] - 1, self.size)}"
+            tgt_q = tgt[:, -1:, :]
+            residual = residual[:, -1:, :]
+            tgt_q_mask = None
+            if tgt_mask is not None:
+                tgt_q_mask = tgt_mask[:, -1:, :]
+
+        if self.concat_after:
+            tgt_concat = torch.cat(
+                (tgt_q, self.self_attn(tgt_q, tgt, tgt, tgt_q_mask)), dim=-1
+            )
+            x = residual + self.concat_linear1(tgt_concat)
+        else:
+            x = residual + self.dropout(self.self_attn(tgt_q, tgt, tgt, tgt_q_mask))
+        if not self.normalize_before:
+            x = self.norm1(x)
+        z = x
+        
+        residual = x
+        if self.normalize_before:
+            x = self.norm1(x)
+
+        skip = self.src_attn(x, asr_memory, spk_memory, memory_mask)
+
+        if self.concat_after:
+            x_concat = torch.cat(
+                (x, skip), dim=-1
+            )
+            x = residual + self.concat_linear2(x_concat)
+        else:
+            x = residual + self.dropout(skip)
+        if not self.normalize_before:
+            x = self.norm1(x)
+        
+        residual = x
+        if self.normalize_before:
+            x = self.norm2(x)
+        x = residual + self.dropout(self.feed_forward(x))
+        if not self.normalize_before:
+            x = self.norm2(x)
+
+        if cache is not None:
+            x = torch.cat([cache, x], dim=1)
+            
+        return x, tgt_mask, asr_memory, spk_memory, memory_mask, z
+
+class SpeakerAttributeAsrDecoderFirstLayer(nn.Module):
+    
+    def __init__(
+        self,
+        size,
+        d_size,
+        src_attn,
+        feed_forward,
+        dropout_rate,
+        normalize_before=True,
+        concat_after=False,
+    ):
+        """Construct an DecoderLayer object."""
+        super(SpeakerAttributeAsrDecoderFirstLayer, self).__init__()
+        self.size = size
+        self.src_attn = src_attn
+        self.feed_forward = feed_forward
+        self.norm1 = LayerNorm(size)
+        self.norm2 = LayerNorm(size)
+        self.norm3 = LayerNorm(size)
+        self.dropout = nn.Dropout(dropout_rate)
+        self.normalize_before = normalize_before
+        self.concat_after = concat_after
+        self.spk_linear = nn.Linear(d_size, size, bias=False)
+        if self.concat_after:
+            self.concat_linear1 = nn.Linear(size + size, size)
+            self.concat_linear2 = nn.Linear(size + size, size)
+
+    def forward(self, tgt, tgt_mask, memory, memory_mask, dn, cache=None):
+        
+        residual = tgt
+        if self.normalize_before:
+            tgt = self.norm1(tgt)
+
+        if cache is None:
+            tgt_q = tgt
+            tgt_q_mask = tgt_mask
+        else:
+            
+            tgt_q = tgt[:, -1:, :]
+            residual = residual[:, -1:, :]
+            tgt_q_mask = None
+            if tgt_mask is not None:
+                tgt_q_mask = tgt_mask[:, -1:, :]
+
+        x = tgt_q
+        if self.normalize_before:
+            x = self.norm2(x)
+        if self.concat_after:
+            x_concat = torch.cat(
+                (x, self.src_attn(x, memory, memory, memory_mask)), dim=-1
+            )
+            x = residual + self.concat_linear2(x_concat)
+        else:
+            x = residual + self.dropout(self.src_attn(x, memory, memory, memory_mask))
+        if not self.normalize_before:
+            x = self.norm2(x)
+        residual = x
+
+        if dn!=None:
+            x = x + self.spk_linear(dn)
+        if self.normalize_before:
+            x = self.norm3(x)
+        
+        x = residual + self.dropout(self.feed_forward(x))
+        if not self.normalize_before:
+            x = self.norm3(x)
+
+        if cache is not None:
+            x = torch.cat([cache, x], dim=1)
+
+        return x, tgt_mask, memory, memory_mask
```

### Comparing `funasr-0.4.8/funasr/models/e2e_asr.py` & `funasr-0.5.0/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_asr_common.py` & `funasr-0.5.0/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.5.0/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_asr_mfcca.py` & `funasr-0.5.0/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_asr_paraformer.py` & `funasr-0.5.0/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_asr_transducer.py` & `funasr-0.5.0/funasr/models/e2e_asr_transducer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from packaging.version import parse as V
 from typeguard import check_argument_types
 
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.decoder.abs_decoder import AbsDecoder as AbsAttDecoder
-from funasr.models.encoder.conformer_encoder import ConformerChunkEncoder as Encoder
+from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.modules.nets_utils import get_transducer_task_io
 from funasr.layers.abs_normalize import AbsNormalize
 from funasr.torch_utils.device_funcs import force_gatherable
 from funasr.train.abs_espnet_model import AbsESPnetModel
 
 if V(torch.__version__) >= V("1.6.0"):
@@ -58,15 +58,15 @@
     def __init__(
         self,
         vocab_size: int,
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
         normalize: Optional[AbsNormalize],
-        encoder: Encoder,
+        encoder: AbsEncoder,
         decoder: RNNTDecoder,
         joint_network: JointNetwork,
         att_decoder: Optional[AbsAttDecoder] = None,
         transducer_weight: float = 1.0,
         fastemit_lambda: float = 0.0,
         auxiliary_ctc_weight: float = 0.0,
         auxiliary_ctc_dropout_rate: float = 0.0,
@@ -282,15 +282,15 @@
                 feats, feats_lengths = self.specaug(feats, feats_lengths)
 
             # 3. Normalization for feature: e.g. Global-CMVN, Utterance-CMVN
             if self.normalize is not None:
                 feats, feats_lengths = self.normalize(feats, feats_lengths)
 
         # 4. Forward encoder
-        encoder_out, encoder_out_lens = self.encoder(feats, feats_lengths)
+        encoder_out, encoder_out_lens, _ = self.encoder(feats, feats_lengths)
 
         assert encoder_out.size(0) == speech.size(0), (
             encoder_out.size(),
             speech.size(0),
         )
         assert encoder_out.size(1) <= encoder_out_lens.max(), (
             encoder_out.size(),
@@ -511,15 +511,15 @@
     def __init__(
         self,
         vocab_size: int,
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
         normalize: Optional[AbsNormalize],
-        encoder: Encoder,
+        encoder: AbsEncoder,
         decoder: RNNTDecoder,
         joint_network: JointNetwork,
         att_decoder: Optional[AbsAttDecoder] = None,
         transducer_weight: float = 1.0,
         fastemit_lambda: float = 0.0,
         auxiliary_ctc_weight: float = 0.0,
         auxiliary_att_weight: float = 0.0,
```

### Comparing `funasr-0.4.8/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.5.0/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_diar_sond.py` & `funasr-0.5.0/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_sv.py` & `funasr-0.5.0/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_tp.py` & `funasr-0.5.0/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_uni_asr.py` & `funasr-0.5.0/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/e2e_vad.py` & `funasr-0.5.0/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/conformer_encoder.py` & `funasr-0.5.0/funasr/models/encoder/conformer_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
     def __init__(
         self,
         block_size: int,
         self_att: torch.nn.Module,
         feed_forward: torch.nn.Module,
         feed_forward_macaron: torch.nn.Module,
         conv_mod: torch.nn.Module,
-        norm_class: torch.nn.Module = torch.nn.LayerNorm,
+        norm_class: torch.nn.Module = LayerNorm,
         norm_args: Dict = {},
         dropout_rate: float = 0.0,
     ) -> None:
         """Construct a Conformer object."""
         super().__init__()
 
         self.self_att = self_att
@@ -1141,15 +1141,15 @@
         )
 
         olens = mask.eq(0).sum(1)
         if self.time_reduction_factor > 1:
             x = x[:,::self.time_reduction_factor,:]
             olens = torch.floor_divide(olens-1, self.time_reduction_factor) + 1
 
-        return x, olens
+        return x, olens, None
 
     def simu_chunk_forward(
         self,
         x: torch.Tensor,
         x_len: torch.Tensor,
         chunk_size: int = 16,
         left_context: int = 32,
```

### Comparing `funasr-0.4.8/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.5.0/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.5.0/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.5.0/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.5.0/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.5.0/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.5.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.5.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.5.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.5.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.5.0/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/rnn_encoder.py` & `funasr-0.5.0/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/sanm_encoder.py` & `funasr-0.5.0/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/encoder/transformer_encoder.py` & `funasr-0.5.0/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/frontend/default.py` & `funasr-0.5.0/funasr/models/frontend/default.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             onesided: bool = True,
             n_mels: int = 80,
             fmin: int = None,
             fmax: int = None,
             htk: bool = False,
             frontend_conf: Optional[dict] = get_default_kwargs(Frontend),
             apply_stft: bool = True,
+            use_channel: int = None,
     ):
         assert check_argument_types()
         super().__init__()
         if isinstance(fs, str):
             fs = humanfriendly.parse_size(fs)
 
         # Deepcopy (In general, dict shouldn't be used as default arg)
@@ -73,14 +74,15 @@
             n_mels=n_mels,
             fmin=fmin,
             fmax=fmax,
             htk=htk,
         )
         self.n_mels = n_mels
         self.frontend_type = "default"
+        self.use_channel = use_channel
 
     def output_size(self) -> int:
         return self.n_mels
 
     def forward(
             self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
@@ -96,17 +98,20 @@
             # input_stft: (Batch, Length, [Channel], Freq)
             input_stft, _, mask = self.frontend(input_stft, feats_lens)
 
         # 3. [Multi channel case]: Select a channel
         if input_stft.dim() == 4:
             # h: (B, T, C, F) -> h: (B, T, F)
             if self.training:
-                # Select 1ch randomly
-                ch = np.random.randint(input_stft.size(2))
-                input_stft = input_stft[:, :, ch, :]
+                if self.use_channel == None:
+                    input_stft = input_stft[:, :, 0, :]
+                else:
+                    # Select 1ch randomly
+                    ch = np.random.randint(input_stft.size(2))
+                    input_stft = input_stft[:, :, ch, :]
             else:
                 # Use the first channel
                 input_stft = input_stft[:, :, 0, :]
 
         # 4. STFT -> Power spectrum
         # h: ComplexTensor(B, T, F) -> torch.Tensor(B, T, F)
         input_power = input_stft.real ** 2 + input_stft.imag ** 2
```

### Comparing `funasr-0.4.8/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.5.0/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/frontend/fused.py` & `funasr-0.5.0/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/frontend/s3prl.py` & `funasr-0.5.0/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/frontend/wav_frontend.py` & `funasr-0.5.0/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.5.0/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/frontend/windowing.py` & `funasr-0.5.0/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/joint_net/joint_network.py` & `funasr-0.5.0/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/pooling/statistic_pooling.py` & `funasr-0.5.0/funasr/models/pooling/statistic_pooling.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,17 @@
 ) -> Tuple[torch.Tensor, int]:
     # xs_pad in (Batch, Channel, Time, Frequency)
 
     tt = xs_pad.shape[2]
     num_chunk = int(math.ceil(tt / pooling_stride))
     pad = pooling_size // 2
     if len(xs_pad.shape) == 4:
-        features = F.pad(xs_pad, (0, 0, pad, pad), "reflect")
+        features = F.pad(xs_pad, (0, 0, pad, pad), "replicate")
     else:
-        features = F.pad(xs_pad, (pad, pad), "reflect")
+        features = F.pad(xs_pad, (pad, pad), "replicate")
     stat_list = []
 
     for i in range(num_chunk):
         # B x C
         st, ed = i*pooling_stride, i*pooling_stride+pooling_size
         stat = statistic_pooling(features[:, :, st: ed], pooling_dim=pooling_dim)
         stat_list.append(stat.unsqueeze(2))
```

### Comparing `funasr-0.4.8/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.5.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/predictor/cif.py` & `funasr-0.5.0/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/preencoder/linear.py` & `funasr-0.5.0/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/preencoder/sinc.py` & `funasr-0.5.0/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/specaug/specaug.py` & `funasr-0.5.0/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/target_delay_transformer.py` & `funasr-0.5.0/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/models/vad_realtime_transformer.py` & `funasr-0.5.0/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/add_sos_eos.py` & `funasr-0.5.0/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/attention.py` & `funasr-0.5.0/funasr/modules/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 import math
 
 import numpy
 import torch
 from torch import nn
 from typing import Optional, Tuple
 
+import torch.nn.functional as F
+from funasr.modules.nets_utils import make_pad_mask
+
 class MultiHeadedAttention(nn.Module):
     """Multi-Head Attention layer.
 
     Args:
         n_head (int): The number of heads.
         n_feat (int): The number of features.
         dropout_rate (float): Dropout rate.
@@ -955,7 +958,41 @@
             left_context: Number of frames in left context.
         Returns:
             : Output tensor. (B, T_1, H * d_k)
         """
         q, k, v = self.forward_qkv(query, key, value)
         scores = self.compute_att_score(q, k, pos_enc, left_context=left_context)
         return self.forward_attention(v, scores, mask, chunk_mask=chunk_mask)
+
+
+class CosineDistanceAttention(nn.Module):
+    """ Compute Cosine Distance between spk decoder output and speaker profile 
+    Args:
+        profile_path: speaker profile file path (.npy file)
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.softmax = nn.Softmax(dim=-1)
+
+    def forward(self, spk_decoder_out, profile, profile_lens=None):
+        """
+        Args:
+            spk_decoder_out(torch.Tensor):(B, L, D)
+            spk_profiles(torch.Tensor):(B, N, D)
+        """
+        x = spk_decoder_out.unsqueeze(2)  # (B, L, 1, D)
+        if profile_lens is not None:
+            
+            mask = (make_pad_mask(profile_lens)[:, None, :]).to(profile.device)
+            min_value = float(
+                numpy.finfo(torch.tensor(0, dtype=x.dtype).numpy().dtype).min
+            )
+            weights_not_softmax=F.cosine_similarity(x, profile.unsqueeze(1), dim=-1).masked_fill(mask, min_value)
+            weights = self.softmax(weights_not_softmax).masked_fill(mask, 0.0)  # (B, L, N)
+        else:
+            x = x[:, -1:, :, :]
+            weights_not_softmax=F.cosine_similarity(x, profile.unsqueeze(1).to(x.device), dim=-1)
+            weights = self.softmax(weights_not_softmax)  # (B, 1, N)
+        spk_embedding = torch.matmul(weights, profile.to(weights.device))  # (B, L, D)
+
+        return spk_embedding, weights
```

### Comparing `funasr-0.4.8/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.5.0/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.5.0/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/beam_search/beam_search.py` & `funasr-0.5.0/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.5.0/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/data2vec/data_utils.py` & `funasr-0.5.0/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/data2vec/ema_module.py` & `funasr-0.5.0/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.5.0/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/data2vec/quant_noise.py` & `funasr-0.5.0/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/data2vec/utils.py` & `funasr-0.5.0/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.5.0/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/dynamic_conv.py` & `funasr-0.5.0/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/dynamic_conv2d.py` & `funasr-0.5.0/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/e2e_asr_common.py` & `funasr-0.5.0/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/eend_ola/encoder.py` & `funasr-0.5.0/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.5.0/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/embedding.py` & `funasr-0.5.0/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/frontends/beamformer.py` & `funasr-0.5.0/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.5.0/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.5.0/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/frontends/feature_transform.py` & `funasr-0.5.0/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/frontends/frontend.py` & `funasr-0.5.0/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/frontends/mask_estimator.py` & `funasr-0.5.0/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/layer_norm.py` & `funasr-0.5.0/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/lightconv.py` & `funasr-0.5.0/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/lightconv2d.py` & `funasr-0.5.0/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/mask.py` & `funasr-0.5.0/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/multi_layer_conv.py` & `funasr-0.5.0/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/nets_utils.py` & `funasr-0.5.0/funasr/modules/nets_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -481,22 +481,47 @@
     if len(old_keys) > 0:
         logging.warning(f"Rename: {old_prefix} -> {new_prefix}")
     for k in old_keys:
         v = state_dict.pop(k)
         new_k = k.replace(old_prefix, new_prefix)
         state_dict[new_k] = v
 
-
 class Swish(torch.nn.Module):
-    """Construct an Swish object."""
+    """Swish activation definition.
 
-    def forward(self, x):
-        """Return Swich activation function."""
-        return x * torch.sigmoid(x)
+    Swish(x) = (beta * x) * sigmoid(x)
+                 where beta = 1 defines standard Swish activation.
 
+    References:
+        https://arxiv.org/abs/2108.12943 / https://arxiv.org/abs/1710.05941v1.
+        E-swish variant: https://arxiv.org/abs/1801.07145.
+
+    Args:
+        beta: Beta parameter for E-Swish.
+                (beta >= 1. If beta < 1, use standard Swish).
+        use_builtin: Whether to use PyTorch function if available.
+
+    """
+
+    def __init__(self, beta: float = 1.0, use_builtin: bool = False) -> None:
+        super().__init__()
+
+        self.beta = beta
+
+        if beta > 1:
+            self.swish = lambda x: (self.beta * x) * torch.sigmoid(x)
+        else:
+            if use_builtin:
+                self.swish = torch.nn.SiLU()
+            else:
+                self.swish = lambda x: x * torch.sigmoid(x)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """Forward computation."""
+        return self.swish(x)
 
 def get_activation(act):
     """Return activation function."""
 
     activation_funcs = {
         "hardtanh": torch.nn.Hardtanh,
         "tanh": torch.nn.Tanh,
```

### Comparing `funasr-0.4.8/funasr/modules/positionwise_feed_forward.py` & `funasr-0.5.0/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/repeat.py` & `funasr-0.5.0/funasr/modules/repeat.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Copyright 2019 Shigeki Karita
 #  Apache 2.0  (http://www.apache.org/licenses/LICENSE-2.0)
 
 """Repeat the same layer definition."""
 
 from typing import Dict, List, Optional
-
+from funasr.modules.layer_norm import LayerNorm
 import torch
 
 
 class MultiSequential(torch.nn.Sequential):
     """Multi-input multi-output torch.nn.Sequential."""
 
     def forward(self, *args):
@@ -44,15 +44,15 @@
         norm_args: Normalization module arguments.
     """
 
     def __init__(
         self,
         block_list: List[torch.nn.Module],
         output_size: int,
-        norm_class: torch.nn.Module = torch.nn.LayerNorm,
+        norm_class: torch.nn.Module = LayerNorm,
     ) -> None:
         """Construct a MultiBlocks object."""
         super().__init__()
 
         self.blocks = torch.nn.ModuleList(block_list)
         self.norm_blocks = norm_class(output_size)
```

### Comparing `funasr-0.4.8/funasr/modules/rnn/argument.py` & `funasr-0.5.0/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/rnn/attentions.py` & `funasr-0.5.0/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/rnn/decoders.py` & `funasr-0.5.0/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/rnn/encoders.py` & `funasr-0.5.0/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/scorers/ctc.py` & `funasr-0.5.0/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.5.0/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/scorers/length_bonus.py` & `funasr-0.5.0/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/scorers/scorer_interface.py` & `funasr-0.5.0/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.5.0/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.5.0/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/streaming_utils/utils.py` & `funasr-0.5.0/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/subsampling.py` & `funasr-0.5.0/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/modules/subsampling_without_posenc.py` & `funasr-0.5.0/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/optimizers/fairseq_adam.py` & `funasr-0.5.0/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/optimizers/sgd.py` & `funasr-0.5.0/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/demo.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/libtorch/setup.py` & `funasr-0.5.0/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/demo.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         new_mini_sentence = ""
         new_mini_sentence_punc = []
         cache_pop_trigger_limit = 200
         for mini_sentence_i in range(len(mini_sentences)):
             mini_sentence = mini_sentences[mini_sentence_i]
             mini_sentence_id = mini_sentences_id[mini_sentence_i]
             mini_sentence = cache_sent + mini_sentence
-            mini_sentence_id = np.array(cache_sent_id + mini_sentence_id, dtype='int64')
+            mini_sentence_id = np.array(cache_sent_id + mini_sentence_id, dtype='int32')
             data = {
                 "text": mini_sentence_id[None,:],
                 "text_lengths": np.array([len(mini_sentence_id)], dtype='int32'),
             }
             try:
                 outputs = self.infer(data['text'], data['text_lengths'])
                 y = outputs[0]
@@ -162,15 +162,15 @@
         sentence_words_list = []
         cache_pop_trigger_limit = 200
         skip_num = 0
         for mini_sentence_i in range(len(mini_sentences)):
             mini_sentence = mini_sentences[mini_sentence_i]
             mini_sentence_id = mini_sentences_id[mini_sentence_i]
             mini_sentence = cache_sent + mini_sentence
-            mini_sentence_id = np.concatenate((cache_sent_id, mini_sentence_id), axis=0)
+            mini_sentence_id = np.concatenate((cache_sent_id, mini_sentence_id), axis=0,dtype='int32')
             text_length = len(mini_sentence_id)
             data = {
                 "input": mini_sentence_id[None,:],
                 "text_lengths": np.array([text_length], dtype='int32'),
                 "vad_mask": self.vad_mask(text_length, len(cache))[None, None, :, :].astype(np.float32),
                 "sub_masks": np.tril(np.ones((text_length, text_length), dtype=np.float32))[None, None, :, :].astype(np.float32)
             }
```

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.5.0/funasr/runtime/python/onnxruntime/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.7'
+VERSION_NUM = '0.0.8'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab of DAMO Academy, Alibaba Group",
```

### Comparing `funasr-0.4.8/funasr/samplers/build_batch_sampler.py` & `funasr-0.5.0/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/samplers/folded_batch_sampler.py` & `funasr-0.5.0/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/samplers/length_batch_sampler.py` & `funasr-0.5.0/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.5.0/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.5.0/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.5.0/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/schedulers/abs_scheduler.py` & `funasr-0.5.0/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/schedulers/noam_lr.py` & `funasr-0.5.0/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.5.0/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/schedulers/warmup_lr.py` & `funasr-0.5.0/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/tasks/abs_task.py` & `funasr-0.5.0/funasr/tasks/abs_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,14 +441,20 @@
         group.add_argument(
             "--collect_stats",
             type=str2bool,
             default=False,
             help='Perform on "collect stats" mode',
         )
         group.add_argument(
+            "--mc",
+            type=bool,
+            default=False,
+            help="MultiChannel input",
+        )
+        group.add_argument(
             "--write_collected_feats",
             type=str2bool,
             default=False,
             help='Write the output features from the model when "collect stats" mode',
         )
 
         group = parser.add_argument_group("Trainer related")
@@ -637,16 +643,16 @@
         )
 
         group = parser.add_argument_group("Pretraining model related")
         group.add_argument("--pretrain_path", help="This option is obsoleted")
         group.add_argument(
             "--init_param",
             type=str,
+            action="append",
             default=[],
-            nargs="*",
             help="Specify the file path used for initialization of parameters. "
                  "The format is '<file_path>:<src_key>:<dst_key>:<exclude_keys>', "
                  "where file_path is the model file path, "
                  "src_key specifies the key of model states to be used in the model file, "
                  "dst_key specifies the attribute of the model to be initialized, "
                  "and exclude_keys excludes keys of model states for the initialization."
                  "e.g.\n"
@@ -664,15 +670,15 @@
             default=False,
             help="Ignore size mismatch when loading pre-trained model",
         )
         group.add_argument(
             "--freeze_param",
             type=str,
             default=[],
-            nargs="*",
+            action="append",
             help="Freeze parameters",
         )
 
         group = parser.add_argument_group("BatchSampler related")
         group.add_argument(
             "--num_iters_per_epoch",
             type=int_or_none,
@@ -1155,18 +1161,18 @@
         if args.use_pai:
             distributed_option.init_torch_distributed_pai(args)
         elif not args.simple_ddp:
             distributed_option.init_torch_distributed(args)
         elif args.distributed and args.simple_ddp:
             distributed_option.init_torch_distributed_pai(args)
             args.ngpu = dist.get_world_size()
-            if args.dataset_type == "small":
+            if args.dataset_type == "small" and args.ngpu > 0:
                 if args.batch_size is not None:
                     args.batch_size = args.batch_size * args.ngpu
-                if args.batch_bins is not None:
+                if args.batch_bins is not None and args.ngpu > 0:
                     args.batch_bins = args.batch_bins * args.ngpu
 
         # filter samples if wav.scp and text are mismatch
         if (args.train_shape_file is None and args.dataset_type == "small") or args.train_data_file is None and args.dataset_type == "large":
             if not args.simple_ddp or distributed_option.dist_rank == 0:
                 filter_wav_text(args.data_dir, args.train_set)
                 filter_wav_text(args.data_dir, args.dev_set)
@@ -1318,25 +1324,27 @@
 
             collect_stats(
                 model=model,
                 train_iter=cls.build_streaming_iterator(
                     data_path_and_name_and_type=args.train_data_path_and_name_and_type,
                     key_file=train_key_file,
                     batch_size=args.batch_size,
+                    mc=args.mc,
                     dtype=args.train_dtype,
                     num_workers=args.num_workers,
                     allow_variable_data_keys=args.allow_variable_data_keys,
                     ngpu=args.ngpu,
                     preprocess_fn=cls.build_preprocess_fn(args, train=False),
                     collate_fn=cls.build_collate_fn(args, train=False),
                 ),
                 valid_iter=cls.build_streaming_iterator(
                     data_path_and_name_and_type=args.valid_data_path_and_name_and_type,
                     key_file=valid_key_file,
                     batch_size=args.valid_batch_size,
+                    mc=args.mc,
                     dtype=args.train_dtype,
                     num_workers=args.num_workers,
                     allow_variable_data_keys=args.allow_variable_data_keys,
                     ngpu=args.ngpu,
                     preprocess_fn=cls.build_preprocess_fn(args, train=False),
                     collate_fn=cls.build_collate_fn(args, train=False),
                 ),
```

### Comparing `funasr-0.4.8/funasr/tasks/asr.py` & `funasr-0.5.0/funasr/tasks/asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1680,15 +1680,15 @@
             encoder_output_size,
             decoder_output_size,
             **args.joint_network_conf,
         )
 
         # 7. Build model
 
-        if encoder.unified_model_training:
+        if hasattr(encoder, 'unified_model_training') and encoder.unified_model_training:
             model = UnifiedTransducerModel(
                 vocab_size=vocab_size,
                 token_list=token_list,
                 frontend=frontend,
                 specaug=specaug,
                 normalize=normalize,
                 encoder=encoder,
```

### Comparing `funasr-0.4.8/funasr/tasks/data2vec.py` & `funasr-0.5.0/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/tasks/diar.py` & `funasr-0.5.0/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/tasks/lm.py` & `funasr-0.5.0/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/tasks/punctuation.py` & `funasr-0.5.0/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/tasks/sv.py` & `funasr-0.5.0/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/build_tokenizer.py` & `funasr-0.5.0/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/char_tokenizer.py` & `funasr-0.5.0/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/cleaner.py` & `funasr-0.5.0/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/korean_cleaner.py` & `funasr-0.5.0/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/phoneme_tokenizer.py` & `funasr-0.5.0/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.5.0/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/token_id_converter.py` & `funasr-0.5.0/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/text/word_tokenizer.py` & `funasr-0.5.0/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.5.0/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/torch_utils/device_funcs.py` & `funasr-0.5.0/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/torch_utils/forward_adaptor.py` & `funasr-0.5.0/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/torch_utils/initialize.py` & `funasr-0.5.0/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.5.0/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/torch_utils/model_summary.py` & `funasr-0.5.0/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/torch_utils/recursive_op.py` & `funasr-0.5.0/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/train/abs_espnet_model.py` & `funasr-0.5.0/funasr/train/abs_espnet_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/train/abs_model.py` & `funasr-0.5.0/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/train/class_choices.py` & `funasr-0.5.0/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/train/distributed_utils.py` & `funasr-0.5.0/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/train/reporter.py` & `funasr-0.5.0/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/train/trainer.py` & `funasr-0.5.0/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/asr_env_checking.py` & `funasr-0.5.0/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/asr_utils.py` & `funasr-0.5.0/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/build_dataclass.py` & `funasr-0.5.0/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/cli_utils.py` & `funasr-0.5.0/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/compute_eer.py` & `funasr-0.5.0/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/compute_min_dcf.py` & `funasr-0.5.0/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/compute_wer.py` & `funasr-0.5.0/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/config_argparse.py` & `funasr-0.5.0/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/get_default_kwargs.py` & `funasr-0.5.0/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/griffin_lim.py` & `funasr-0.5.0/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/job_runner.py` & `funasr-0.5.0/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/misc.py` & `funasr-0.5.0/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/modelscope_param.py` & `funasr-0.5.0/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/nested_dict_action.py` & `funasr-0.5.0/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/postprocess_utils.py` & `funasr-0.5.0/funasr/utils/postprocess_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -238,8 +238,8 @@
     else:
         word_lists = abbr_dispose(word_lists)
         real_word_lists = []
         for ch in word_lists:
             if ch != ' ':
                 real_word_lists.append(ch)
         sentence = ''.join(word_lists).strip()
-        return sentence, real_word_lists
+        return sentence, real_word_lists
```

### Comparing `funasr-0.4.8/funasr/utils/sized_dict.py` & `funasr-0.5.0/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/timestamp_tools.py` & `funasr-0.5.0/funasr/utils/timestamp_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,70 +76,71 @@
     for char, timestamp in zip(new_char_list, timestamp_list):
         if char != '<sil>':
             res.append([int(timestamp[0] * 1000), int(timestamp[1] * 1000)])
     return res_txt, res
 
 
 def time_stamp_sentence(punc_id_list, time_stamp_postprocessed, text_postprocessed):
+    punc_list = ['，', '。', '？', '、']
     res = []
     if text_postprocessed is None:
         return res
     if time_stamp_postprocessed is None:
         return res
     if len(time_stamp_postprocessed) == 0:
         return res
     if len(text_postprocessed) == 0:
         return res
 
     if punc_id_list is None or len(punc_id_list) == 0:
         res.append({
             'text': text_postprocessed.split(),
             "start": time_stamp_postprocessed[0][0],
-            "end": time_stamp_postprocessed[-1][1]
+            "end": time_stamp_postprocessed[-1][1],
+            'text_seg': text_postprocessed.split(),
+            "ts_list": time_stamp_postprocessed,
         })
         return res
     if len(punc_id_list) != len(time_stamp_postprocessed):
         print("  warning length mistach!!!!!!")
-    sentence_text = ''
+    sentence_text = ""
+    sentence_text_seg = ""
+    ts_list = []
     sentence_start = time_stamp_postprocessed[0][0]
     sentence_end = time_stamp_postprocessed[0][1]
     texts = text_postprocessed.split()
     punc_stamp_text_list = list(zip_longest(punc_id_list, time_stamp_postprocessed, texts, fillvalue=None))
     for punc_stamp_text in punc_stamp_text_list:
         punc_id, time_stamp, text = punc_stamp_text
-        sentence_text += text if text is not None else ''
+        # sentence_text += text if text is not None else ''
+        if text is not None:
+            if 'a' <= text[0] <= 'z' or 'A' <= text[0] <= 'Z':
+                sentence_text += ' ' + text
+            elif len(sentence_text) and ('a' <= sentence_text[-1] <= 'z' or 'A' <= sentence_text[-1] <= 'Z'):
+                sentence_text += ' ' + text
+            else:
+                sentence_text += text
+            sentence_text_seg += text + ' '
+        ts_list.append(time_stamp)
+
         punc_id = int(punc_id) if punc_id is not None else 1
         sentence_end = time_stamp[1] if time_stamp is not None else sentence_end
 
-        if punc_id == 2:
-            sentence_text += ','
-            res.append({
-                'text': sentence_text,
-                "start": sentence_start,
-                "end": sentence_end
-            })
-            sentence_text = ''
-            sentence_start = sentence_end
-        elif punc_id == 3:
-            sentence_text += '.'
-            res.append({
-                'text': sentence_text,
-                "start": sentence_start,
-                "end": sentence_end
-            })
-            sentence_text = ''
-            sentence_start = sentence_end
-        elif punc_id == 4:
-            sentence_text += '?'
+        if punc_id > 1:
+            sentence_text += punc_list[punc_id - 2]
             res.append({
                 'text': sentence_text,
                 "start": sentence_start,
-                "end": sentence_end
+                "end": sentence_end,
+                "text_seg": sentence_text_seg,
+                "ts_list": ts_list
             })
             sentence_text = ''
+            sentence_text_seg = ''
+            ts_list = []
             sentence_start = sentence_end
     return res
 
 
 class AverageShiftCalculator():
     def __init__(self):
         logging.warning("Calculating average shift.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `funasr-0.4.8/funasr/utils/types.py` & `funasr-0.5.0/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr/utils/wav_utils.py` & `funasr-0.5.0/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/funasr.egg-info/PKG-INFO` & `funasr-0.5.0/funasr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.4.8
+Version: 0.5.0
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -44,16 +44,16 @@
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
-### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
-We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge
+We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.4.8 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.0 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -30,52 +30,52 @@
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
 Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
 modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
 (https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
 meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
-Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
-announce that the M2MeT2.0 challenge will be held in the near future. The
-baseline system is conducted on FunASR and is provided as a receipe of
-AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
-notes For the release notes, please ref to [news](https://github.com/alibaba-
-damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
-recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
-Restoration, Language Models, Speaker Verification and Speaker diarization. -
-We have released large number of academic and industrial pretrained models on
-[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
-recognition), ref to [Model Zoo](https://github.com/alibaba-damo-academy/
-FunASR/blob/main/docs/model_zoo/modelscope_models.md) - The pretrained model
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
-performance on many tasks in [SpeechIO leaderboard](https://github.com/
-SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
-pretrained models from [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
-github.com/espnet/espnet) framework, the training speed of large-scale datasets
-in FunASR is much faster owning to the optimized dataloader. ## Installation
-Install from pip ```shell pip install -U funasr # For the users in China, you
-could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Contact If you
-have any questions about FunASR, please contact us by - email:
-[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
-Wechat group | |:---:|:-----------------------------------------------------:
-| |
+Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We are pleased to
+announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023
+challenge special session. The registration is now open. The baseline system is
+conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more
+details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-
+academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-
+academy.github.io/FunASR/m2met2/index.html)). ### Release notes For the release
+notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/
+releases) ## Highlights - FunASR supports speech recognition(ASR), Multi-talker
+ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models,
+Speaker Verification and Speaker diarization. - We have released large number
+of academic and industrial pretrained models on [ModelScope](https://
+www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), ref to [Model
+Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md) - The pretrained model [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) obtains the best performance on many tasks in
+[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
+supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
+(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
+Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
+speed of large-scale datasets in FunASR is much faster owning to the optimized
+dataloader. ## Installation Install from pip ```shell pip install -U funasr #
+For the users in China, you could install with the command: # pip install -
+U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
+source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
+pip install -e ./ # For the users in China, you could install with the command:
+# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
+want to use the pretrained models in ModelScope, you should install the
+modelscope: ```shell pip install -U modelscope # For the users in China, you
+could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Contact If you have any questions about FunASR, please
+contact us by - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-
+inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
+------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.4.8/funasr.egg-info/SOURCES.txt` & `funasr-0.5.0/funasr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,16 @@
 funasr/bin/__init__.py
 funasr/bin/aggregate_stats_dirs.py
 funasr/bin/asr_inference.py
 funasr/bin/asr_inference_launch.py
 funasr/bin/asr_inference_mfcca.py
 funasr/bin/asr_inference_paraformer.py
 funasr/bin/asr_inference_paraformer_streaming.py
-funasr/bin/asr_inference_paraformer_vad.py
-funasr/bin/asr_inference_paraformer_vad_punc.py
 funasr/bin/asr_inference_rnnt.py
 funasr/bin/asr_inference_uniasr.py
-funasr/bin/asr_inference_uniasr_vad.py
 funasr/bin/asr_train.py
 funasr/bin/asr_train_paraformer.py
 funasr/bin/asr_train_transducer.py
 funasr/bin/asr_train_uniasr.py
 funasr/bin/build_trainer.py
 funasr/bin/data2vec_train.py
 funasr/bin/diar_inference_launch.py
@@ -34,14 +31,16 @@
 funasr/bin/lm_inference_launch.py
 funasr/bin/lm_train.py
 funasr/bin/modelscope_infer.py
 funasr/bin/punc_inference_launch.py
 funasr/bin/punc_train.py
 funasr/bin/punctuation_infer.py
 funasr/bin/punctuation_infer_vadrealtime.py
+funasr/bin/sa_asr_inference.py
+funasr/bin/sa_asr_train.py
 funasr/bin/sond_inference.py
 funasr/bin/sv_inference.py
 funasr/bin/sv_inference_launch.py
 funasr/bin/tokenize_text.py
 funasr/bin/tp_inference.py
 funasr/bin/tp_inference_launch.py
 funasr/bin/vad_inference.py
@@ -137,14 +136,15 @@
 funasr/models/e2e_asr_common.py
 funasr/models/e2e_asr_contextual_paraformer.py
 funasr/models/e2e_asr_mfcca.py
 funasr/models/e2e_asr_paraformer.py
 funasr/models/e2e_asr_transducer.py
 funasr/models/e2e_diar_eend_ola.py
 funasr/models/e2e_diar_sond.py
+funasr/models/e2e_sa_asr.py
 funasr/models/e2e_sv.py
 funasr/models/e2e_tp.py
 funasr/models/e2e_uni_asr.py
 funasr/models/e2e_vad.py
 funasr/models/target_delay_transformer.py
 funasr/models/vad_realtime_transformer.py
 funasr/models/decoder/__init__.py
@@ -214,14 +214,15 @@
 funasr/modules/repeat.py
 funasr/modules/subsampling.py
 funasr/modules/subsampling_without_posenc.py
 funasr/modules/beam_search/__init__.py
 funasr/modules/beam_search/batch_beam_search.py
 funasr/modules/beam_search/batch_beam_search_online_sim.py
 funasr/modules/beam_search/beam_search.py
+funasr/modules/beam_search/beam_search_sa_asr.py
 funasr/modules/beam_search/beam_search_transducer.py
 funasr/modules/data2vec/__init__.py
 funasr/modules/data2vec/data_utils.py
 funasr/modules/data2vec/ema_module.py
 funasr/modules/data2vec/grad_multiply.py
 funasr/modules/data2vec/multihead_attention.py
 funasr/modules/data2vec/quant_noise.py
@@ -300,14 +301,15 @@
 funasr/tasks/__init__.py
 funasr/tasks/abs_task.py
 funasr/tasks/asr.py
 funasr/tasks/data2vec.py
 funasr/tasks/diar.py
 funasr/tasks/lm.py
 funasr/tasks/punctuation.py
+funasr/tasks/sa_asr.py
 funasr/tasks/sv.py
 funasr/tasks/vad.py
 funasr/text/__init__.py
 funasr/text/abs_tokenizer.py
 funasr/text/build_tokenizer.py
 funasr/text/char_tokenizer.py
 funasr/text/cleaner.py
@@ -348,14 +350,15 @@
 funasr/utils/misc.py
 funasr/utils/modelscope_param.py
 funasr/utils/nested_dict_action.py
 funasr/utils/postprocess_utils.py
 funasr/utils/sized_dict.py
 funasr/utils/timestamp_tools.py
 funasr/utils/types.py
+funasr/utils/vad_utils.py
 funasr/utils/wav_utils.py
 funasr/utils/yaml_no_alias_safe_dump.py
 tests/test_asr_inference_pipeline.py
 tests/test_asr_vad_punc_inference_pipeline.py
 tests/test_lm_pipeline.py
 tests/test_punctuation_pipeline.py
 tests/test_sv_inference_pipeline.py
```

### Comparing `funasr-0.4.8/funasr.egg-info/requires.txt` & `funasr-0.5.0/funasr.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 setuptools>=38.5.1
-typeguard<=2.13.3
+typeguard==2.13.3
 humanfriendly
 scipy>=1.4.1
 librosa==0.8.1
 jamo==0.4.1
 PyYAML>=5.1.2
 soundfile>=0.10.2
 h5py>=2.10.0
@@ -15,14 +15,16 @@
 espnet_tts_frontend
 pytorch_wpe
 editdistance==0.5.2
 tensorboard==1.15
 g2p
 oss2
 edit-distance
+textgrid
+protobuf==3.20.0
 
 [all]
 torch_optimizer
 fairscale
 transformers
 editdistance==0.5.2
 wandb
```

### Comparing `funasr-0.4.8/setup.py` & `funasr-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 
 requirements = {
     "install": [
         "setuptools>=38.5.1",
         # "configargparse>=1.2.1",
-        "typeguard<=2.13.3",
+        "typeguard==2.13.3",
         "humanfriendly",
         "scipy>=1.4.1",
         # "filelock",
         "librosa==0.8.1",
         "jamo==0.4.1",  # For kss
         "PyYAML>=5.1.2",
         "soundfile>=0.10.2",
@@ -38,15 +38,18 @@
         "editdistance==0.5.2",
         "tensorboard==1.15",
         "g2p",
         # PAI
         "oss2",
         # "kaldi-native-fbank",
         # timestamp
-        "edit-distance"
+        "edit-distance",
+        # textgrid
+        "textgrid",
+        "protobuf==3.20.0",
     ],
     # train: The modules invoked when training only.
     "train": [
         # "pillow>=6.1.0",
         "editdistance==0.5.2",
         "wandb",
     ],
```

### Comparing `funasr-0.4.8/tests/test_asr_inference_pipeline.py` & `funasr-0.5.0/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.5.0/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/tests/test_lm_pipeline.py` & `funasr-0.5.0/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/tests/test_punctuation_pipeline.py` & `funasr-0.5.0/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/tests/test_sv_inference_pipeline.py` & `funasr-0.5.0/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.8/tests/test_vad_inference_pipeline.py` & `funasr-0.5.0/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

