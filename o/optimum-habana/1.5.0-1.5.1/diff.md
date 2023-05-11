# Comparing `tmp/optimum-habana-1.5.0.tar.gz` & `tmp/optimum-habana-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-habana-1.5.0.tar", last modified: Mon Apr 17 17:31:30 2023, max compression
+gzip compressed data, was "optimum-habana-1.5.1.tar", last modified: Thu May 11 09:04:14 2023, max compression
```

## Comparing `optimum-habana-1.5.0.tar` & `optimum-habana-1.5.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11641 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      974 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/diffusers/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12732 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/pipeline_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39462 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/distributed/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/distributed/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10759 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/distributed/distributed_runner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/transformers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8435 2023-04-10 08:19:40.000000 optimum-habana-1.5.0/optimum/habana/transformers/deepspeed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2696 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/gaudi_configuration.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/generation/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/generation/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   113660 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/generation/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8675 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/gradient_checkpointing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/modeling_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/albert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/albert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/albert/modeling_albert.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/bloom/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/bloom/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20630 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/bloom/modeling_bloom.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10396 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4914 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/modeling_all_models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/vit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/vit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2572 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/vit/modeling_vit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11639 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84175 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/optimum/habana/transformers/trainer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17409 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/trainer_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2675 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/trainer_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23777 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/optimum/habana/transformers/training_args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4082 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/training_args_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4725 2023-04-12 07:37:50.000000 optimum-habana-1.5.0/optimum/habana/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-04-17 17:25:45.000000 optimum-habana-1.5.0/optimum/habana/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum_habana.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2165 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 17:31:25.000000 optimum-habana-1.5.0/optimum_habana.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2957 2023-04-17 17:31:03.000000 optimum-habana-1.5.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19824 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/tests/test_diffusers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17839 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/tests/test_examples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3251 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/tests/test_examples_match_transformers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2774 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/tests/test_gaudi_configuration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85824 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/tests/test_trainer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5354 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/tests/test_trainer_distributed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4733 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/tests/test_trainer_seq2seq.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11641 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.249275 optimum-habana-1.5.1/optimum/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      974 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/diffusers/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12732 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/pipeline_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39462 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/scheduling_ddim.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/distributed/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-28 10:18:20.000000 optimum-habana-1.5.1/optimum/habana/distributed/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10759 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/distributed/distributed_runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8435 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/deepspeed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2696 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/gaudi_configuration.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/generation/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/generation/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   113660 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/generation/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8675 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/gradient_checkpointing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/modeling_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/albert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/albert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/albert/modeling_albert.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20630 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/modeling_bloom.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/gpt2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/gpt2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10396 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4914 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/modeling_all_models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/vit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/vit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2572 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/vit/modeling_vit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11639 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84175 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17409 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/trainer_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2675 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/trainer_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23777 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/training_args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4082 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/training_args_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4725 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-05-11 08:57:48.000000 optimum-habana-1.5.1/optimum/habana/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/optimum_habana.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2165 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 09:04:07.000000 optimum-habana-1.5.1/optimum_habana.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2967 2023-05-11 08:57:55.000000 optimum-habana-1.5.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19824 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/tests/test_diffusers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17839 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/tests/test_examples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3251 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2774 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/tests/test_gaudi_configuration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85824 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/tests/test_trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5354 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/tests/test_trainer_distributed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4733 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/tests/test_trainer_seq2seq.py
```

### Comparing `optimum-habana-1.5.0/LICENSE` & `optimum-habana-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/MANIFEST.in` & `optimum-habana-1.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/PKG-INFO` & `optimum-habana-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.5.0
+Version: 1.5.1
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-habana-1.5.0/README.md` & `optimum-habana-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/__init__.py` & `optimum-habana-1.5.1/optimum/habana/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/pipeline_utils.py` & `optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py` & `optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/scheduling_ddim.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/distributed/distributed_runner.py` & `optimum-habana-1.5.1/optimum/habana/distributed/distributed_runner.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/__init__.py` & `optimum-habana-1.5.1/optimum/habana/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/deepspeed.py` & `optimum-habana-1.5.1/optimum/habana/transformers/deepspeed.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/gaudi_configuration.py` & `optimum-habana-1.5.1/optimum/habana/transformers/gaudi_configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/generation/utils.py` & `optimum-habana-1.5.1/optimum/habana/transformers/generation/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/gradient_checkpointing.py` & `optimum-habana-1.5.1/optimum/habana/transformers/gradient_checkpointing.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/modeling_utils.py` & `optimum-habana-1.5.1/optimum/habana/transformers/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/models/__init__.py` & `optimum-habana-1.5.1/optimum/habana/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/models/albert/modeling_albert.py` & `optimum-habana-1.5.1/optimum/habana/transformers/models/albert/modeling_albert.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/models/bloom/modeling_bloom.py` & `optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/modeling_bloom.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py` & `optimum-habana-1.5.1/optimum/habana/transformers/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/models/modeling_all_models.py` & `optimum-habana-1.5.1/optimum/habana/transformers/models/modeling_all_models.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/models/vit/modeling_vit.py` & `optimum-habana-1.5.1/optimum/habana/transformers/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py` & `optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/trainer.py` & `optimum-habana-1.5.1/optimum/habana/transformers/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/trainer_seq2seq.py` & `optimum-habana-1.5.1/optimum/habana/transformers/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/trainer_utils.py` & `optimum-habana-1.5.1/optimum/habana/transformers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/training_args.py` & `optimum-habana-1.5.1/optimum/habana/transformers/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/transformers/training_args_seq2seq.py` & `optimum-habana-1.5.1/optimum/habana/transformers/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/utils.py` & `optimum-habana-1.5.1/optimum/habana/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/optimum/habana/version.py` & `optimum-habana-1.5.1/optimum/habana/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
```

### Comparing `optimum-habana-1.5.0/optimum_habana.egg-info/PKG-INFO` & `optimum-habana-1.5.1/optimum_habana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.5.0
+Version: 1.5.1
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-habana-1.5.0/optimum_habana.egg-info/SOURCES.txt` & `optimum-habana-1.5.1/optimum_habana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/pyproject.toml` & `optimum-habana-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/setup.py` & `optimum-habana-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     with open(filepath) as version_file:
         (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
-    "transformers >= 4.26.0",
+    "transformers >= 4.26.0, < 4.29.0",
     "optimum",
     "torch",
     "accelerate",
     "diffusers >= 0.12.0",
 ]
 
 TESTS_REQUIRE = [
```

### Comparing `optimum-habana-1.5.0/tests/test_diffusers.py` & `optimum-habana-1.5.1/tests/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/tests/test_examples.py` & `optimum-habana-1.5.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/tests/test_examples_match_transformers.py` & `optimum-habana-1.5.1/tests/test_examples_match_transformers.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/tests/test_gaudi_configuration.py` & `optimum-habana-1.5.1/tests/test_gaudi_configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/tests/test_trainer.py` & `optimum-habana-1.5.1/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/tests/test_trainer_distributed.py` & `optimum-habana-1.5.1/tests/test_trainer_distributed.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.0/tests/test_trainer_seq2seq.py` & `optimum-habana-1.5.1/tests/test_trainer_seq2seq.py`

 * *Files identical despite different names*

