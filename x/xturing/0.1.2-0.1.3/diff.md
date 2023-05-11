# Comparing `tmp/xturing-0.1.2.tar.gz` & `tmp/xturing-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.1.2.tar", last modified: Mon May  1 17:25:29 2023, max compression
+gzip compressed data, was "xturing-0.1.3.tar", last modified: Thu May 11 14:52:21 2023, max compression
```

## Comparing `xturing-0.1.2.tar` & `xturing-0.1.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.384961 xturing-0.1.2/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-03-20 17:06:03.000000 xturing-0.1.2/LICENSE
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-03-29 09:39:04.000000 xturing-0.1.2/MANIFEST.in
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21624 2023-05-01 17:25:29.384961 xturing-0.1.2/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7162 2023-05-01 17:21:49.000000 xturing-0.1.2/README.md
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2203 2023-05-01 17:21:49.000000 xturing-0.1.2/pyproject.toml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-05-01 17:25:29.384961 xturing-0.1.2/setup.cfg
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.352961 xturing-0.1.2/src/
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.356961 xturing-0.1.2/src/xturing/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/__about__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/__init__.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.356961 xturing-0.1.2/src/xturing/cli/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/cli/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/cli/api.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/cli/chat.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/cli/ui.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.360961 xturing-0.1.2/src/xturing/config/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/config/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/config/config_data_classes.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2701 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/config/finetuning_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2517 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/config/generation_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1862 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/config/read_config.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.360961 xturing-0.1.2/src/xturing/datasets/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/datasets/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/datasets/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8179 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/datasets/instruction_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/datasets/text2image_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/datasets/text_dataset.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.364961 xturing-0.1.2/src/xturing/engines/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3182 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/engines/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/bloom_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6742 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/cerebras_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/distilgpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/galactica_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/gpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/gptj_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.364961 xturing-0.1.2/src/xturing/engines/gptj_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/engines/gptj_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/gptj_utils/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6438 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/llama_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.364961 xturing-0.1.2/src/xturing/engines/llama_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/engines/llama_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    44486 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/engines/llama_utils/llama.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.368961 xturing-0.1.2/src/xturing/engines/lora_engine/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/lora.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/save_and_load.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/lora_engine/test.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/opt_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.368961 xturing-0.1.2/src/xturing/engines/quant_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/quant_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6803 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/quant_utils/custom_autotune.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/engines/quant_utils/quant.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.372961 xturing-0.1.2/src/xturing/model_apis/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/ai21.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/cohere.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/model_apis/openai.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.376961 xturing-0.1.2/src/xturing/models/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2566 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/models/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/models/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/bloom.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7132 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/cerebras.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/distilgpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/galactica.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/gpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2100 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/models/llama.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/models/opt.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      542 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/models/stable_diffusion.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.376961 xturing-0.1.2/src/xturing/preprocessors/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/preprocessors/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/preprocessors/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/preprocessors/instruction_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/preprocessors/text_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/registry.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/self_instruct/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/bootstrap_instructions.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/generate_instances.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/identify_if_classification.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/self_instruct/templates/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/templates/clf_task_template.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/trainers/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-03-24 15:40:08.000000 xturing-0.1.2/src/xturing/trainers/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/trainers/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6049 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/trainers/lightning_trainer.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.380961 xturing-0.1.2/src/xturing/ui/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/ui/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    13646 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/ui/playground.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.384961 xturing-0.1.2/src/xturing/utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/utils/external_loggers.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3135 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/utils/hub.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-03-29 09:39:04.000000 xturing-0.1.2/src/xturing/utils/interactive.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/utils/logging.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-03-23 21:03:53.000000 xturing-0.1.2/src/xturing/utils/loss_fns.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-03-30 13:31:50.000000 xturing-0.1.2/src/xturing/utils/notebooks.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-05-01 17:21:49.000000 xturing-0.1.2/src/xturing/utils/text_splitter.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3803 2023-04-06 13:04:39.000000 xturing-0.1.2/src/xturing/utils/utils.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:25:29.356961 xturing-0.1.2/src/xturing.egg-info/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21624 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3201 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/SOURCES.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/dependency_links.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/entry_points.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      237 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/requires.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-05-01 17:25:29.000000 xturing-0.1.2/src/xturing.egg-info/top_level.txt
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.955321 xturing-0.1.3/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-03-20 17:06:03.000000 xturing-0.1.3/LICENSE
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-03-29 09:39:04.000000 xturing-0.1.3/MANIFEST.in
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21623 2023-05-11 14:52:21.955321 xturing-0.1.3/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7161 2023-05-11 14:51:34.000000 xturing-0.1.3/README.md
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-05-11 14:51:34.000000 xturing-0.1.3/pyproject.toml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-05-11 14:52:21.955321 xturing-0.1.3/setup.cfg
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.915321 xturing-0.1.3/src/
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.923321 xturing-0.1.3/src/xturing/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/__about__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/__init__.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.927321 xturing-0.1.3/src/xturing/cli/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/cli/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/cli/api.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/cli/chat.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/cli/ui.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.927321 xturing-0.1.3/src/xturing/config/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/config/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/config/config_data_classes.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2701 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/config/finetuning_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2517 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/config/generation_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1862 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/config/read_config.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.931321 xturing-0.1.3/src/xturing/datasets/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/datasets/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/datasets/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8187 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/datasets/instruction_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/datasets/text2image_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/datasets/text_dataset.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.935321 xturing-0.1.3/src/xturing/engines/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3182 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/engines/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/bloom_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6866 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/engines/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/cerebras_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/distilgpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/galactica_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/gpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/gptj_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.935321 xturing-0.1.3/src/xturing/engines/gptj_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/engines/gptj_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/gptj_utils/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6306 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/engines/llama_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.935321 xturing-0.1.3/src/xturing/engines/llama_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/engines/llama_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    44486 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/engines/llama_utils/llama.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.939321 xturing-0.1.3/src/xturing/engines/lora_engine/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/lora.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/save_and_load.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/lora_engine/test.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/opt_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.939321 xturing-0.1.3/src/xturing/engines/quant_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/quant_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6803 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/engines/quant_utils/quant.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.943321 xturing-0.1.3/src/xturing/model_apis/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/ai21.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/cohere.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/model_apis/openai.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.947321 xturing-0.1.3/src/xturing/models/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2566 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/models/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/models/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/bloom.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7471 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/models/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/cerebras.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/distilgpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/galactica.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/gpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2259 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/models/llama.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/models/opt.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/models/stable_diffusion.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.947321 xturing-0.1.3/src/xturing/preprocessors/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/preprocessors/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/preprocessors/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/preprocessors/instruction_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/preprocessors/text_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/registry.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/self_instruct/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/generate_instances.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/identify_if_classification.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/self_instruct/templates/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/trainers/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-03-24 15:40:08.000000 xturing-0.1.3/src/xturing/trainers/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/trainers/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/trainers/lightning_trainer.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.951321 xturing-0.1.3/src/xturing/ui/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/ui/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    13646 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/ui/playground.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.955321 xturing-0.1.3/src/xturing/utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/utils/external_loggers.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-05-11 14:51:34.000000 xturing-0.1.3/src/xturing/utils/hub.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-03-29 09:39:04.000000 xturing-0.1.3/src/xturing/utils/interactive.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/utils/logging.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-03-23 21:03:53.000000 xturing-0.1.3/src/xturing/utils/loss_fns.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-03-30 13:31:50.000000 xturing-0.1.3/src/xturing/utils/notebooks.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-05-01 17:21:49.000000 xturing-0.1.3/src/xturing/utils/text_splitter.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3803 2023-04-06 13:04:39.000000 xturing-0.1.3/src/xturing/utils/utils.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-05-11 14:52:21.923321 xturing-0.1.3/src/xturing.egg-info/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21623 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3201 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/entry_points.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/requires.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-05-11 14:52:21.000000 xturing-0.1.3/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.1.2/LICENSE` & `xturing-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/PKG-INFO` & `xturing-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -243,20 +243,20 @@
     <img src="https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-the-badge"/>
   </a>
 </p>
 <br>
 
 ___
 
-`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
+`xTuring` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
 By providing an easy-to-use interface for fine-tuning LLMs to your own data and application, xTuring makes it
 simple to build, customize and control LLMs. The entire process can be done inside your computer or in your
 private cloud, ensuring data privacy and security.
 
-With `xturing` you can,
+With `xTuring` you can,
 - Ingest data from different sources and preprocess them to a format LLMs can understand
 - Scale from single to multiple GPUs for faster fine-tuning
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
@@ -370,15 +370,15 @@
 - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
-- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation 
+- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.2/README.md` & `xturing-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     <img src="https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-the-badge"/>
   </a>
 </p>
 <br>
 
 ___
 
-`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
+`xTuring` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
 By providing an easy-to-use interface for fine-tuning LLMs to your own data and application, xTuring makes it
 simple to build, customize and control LLMs. The entire process can be done inside your computer or in your
 private cloud, ensuring data privacy and security.
 
-With `xturing` you can,
+With `xTuring` you can,
 - Ingest data from different sources and preprocess them to a format LLMs can understand
 - Scale from single to multiple GPUs for faster fine-tuning
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
@@ -142,15 +142,15 @@
 - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
-- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation 
+- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
                         [Stochastic.ai] [Stochastic.ai]
          **** Build, customize and control your own personal LLMs ****
      [https://img.shields.io/pypi/v/xturing?style=for-the-badge] [https://
 img.shields.io/badge/Documentation-blue?logo=GitBook&logoColor=white&style=for-
  the-badge] [https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-
                                   the-badge]
 
-___ `xturing` provides fast, efficient and simple fine-tuning of LLMs, such as
+___ `xTuring` provides fast, efficient and simple fine-tuning of LLMs, such as
 LLaMA, GPT-J, Galactica, and more. By providing an easy-to-use interface for
 fine-tuning LLMs to your own data and application, xTuring makes it simple to
 build, customize and control LLMs. The entire process can be done inside your
 computer or in your private cloud, ensuring data privacy and security. With
-`xturing` you can, - Ingest data from different sources and preprocess them to
+`xTuring` you can, - Ingest data from different sources and preprocess them to
 a format LLMs can understand - Scale from single to multiple GPUs for faster
 fine-tuning - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning)
 to reduce hardware costs by up to 90% - Explore different fine-tuning methods
 and benchmark them to find the best performing model - Evaluate fine-tuned
 models on well-defined metrics for in-depth analysis
 ## ð INT4 fine-tuning and generation with LLaMA LoRA We are excited to
 announce the latest enhancement to our `xTuring` library: INT4 fine-tuning and
```

### Comparing `xturing-0.1.2/pyproject.toml` & `xturing-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.1.2"
+version = "0.1.3"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
@@ -55,14 +55,15 @@
     "ai21",
     "cohere",
     "ipywidgets",
     "openai >= 0.27.0",
     "pydantic >= 1.10.0",
     "rouge-score >= 0.1.2",
     "accelerate",
+    "wandb",
 ]
 
 [project.scripts]
 xturing = "xturing.cli:xturing"
 
 [project.optional-dependencies]
 int4 = [
```

### Comparing `xturing-0.1.2/src/xturing/cli/__init__.py` & `xturing-0.1.3/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/cli/api.py` & `xturing-0.1.3/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/cli/chat.py` & `xturing-0.1.3/src/xturing/cli/chat.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/config/__init__.py` & `xturing-0.1.3/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/config/config_data_classes.py` & `xturing-0.1.3/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.3/src/xturing/config/finetuning_config.yaml`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/config/generation_config.yaml` & `xturing-0.1.3/src/xturing/config/generation_config.yaml`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/config/read_config.py` & `xturing-0.1.3/src/xturing/config/read_config.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.3/src/xturing/datasets/instruction_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         if isinstance(path, HFDataset) or isinstance(path, DatasetDict):
             self.data = path
         elif isinstance(path, dict):
             self.data = {"train": HFDataset.from_dict(path)}
         else:
             path = Path(path)
             assert Path(path).exists(), "path does not exist"
-
             if path.is_dir():
                 self.data = load_from_disk(str(path))
             elif path.suffix == ".jsonl":
                 self.data = {"train": HFDataset.from_dict(self.from_jsonl(path))}
 
         self._validate()
 
@@ -119,15 +118,15 @@
     def __iter__(self):
         return iter(self.data["train"])
 
     def __getitem__(self, idx):
         return self.data["train"][idx]
 
     def save(self, path):
-        return self.data.save_to_disk(path)
+        return self.data["train"].save_to_disk(path)
 
     @classmethod
     def generate_dataset(
         cls,
         path: str,
         engine: TextGenerationAPI,
         num_instructions: int = 10,
```

### Comparing `xturing-0.1.2/src/xturing/datasets/text_dataset.py` & `xturing-0.1.3/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/__init__.py` & `xturing-0.1.3/src/xturing/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/bloom_engine.py` & `xturing-0.1.3/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/causal.py` & `xturing-0.1.3/src/xturing/engines/causal.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,17 @@
             )
         else:
             self.model = LoraModel(lora_config, self.model)
             self.model.print_trainable_parameters()
 
         self.loss_fct = CrossEntropyLoss()
 
+    def set_from_state_dict(self, state_dict, strict=False):
+        self.model.load_state_dict(state_dict, strict=strict)
+
     def save(self, saving_path: Union[str, Path]):
         # Save HF config file
         self.model.config.save_pretrained(str(saving_path))
         # Save model weights
         model_weights = str(Path(saving_path).resolve() / "pytorch_model.bin")
 
         torch.save(self.model.state_dict(), model_weights)
```

### Comparing `xturing-0.1.2/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.3/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.3/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/galactica_engine.py` & `xturing-0.1.3/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.3/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/gptj_engine.py` & `xturing-0.1.3/src/xturing/engines/gptj_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.3/src/xturing/engines/gptj_utils/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/llama_engine.py` & `xturing-0.1.3/src/xturing/engines/llama_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,18 +157,14 @@
         warmup_autotune = True
 
         make_quant(model, layers, wbits, groupsize)
 
         state_dict = torch.load(
             weights_path / Path("pytorch_model.bin"), map_location="cpu"
         )
-        new_state_dict = {}
-        for key, value in state_dict.items():
-            new_state_dict[key[6:]] = value
-        model.load_state_dict(new_state_dict, strict=False)
 
         if warmup_autotune:
             autotune_warmup(model)
 
         model.seqlen = 2048
 
         model.gptq = True
@@ -188,7 +184,9 @@
                 "v_proj",
             ],
         )
 
         torch.nn.init.kaiming_uniform_ = saved_kaiming_uniform_
         torch.nn.init.uniform_ = saved_uniform_
         torch.nn.init.normal_ = saved_normal_
+
+        self.set_from_state_dict(state_dict)
```

### Comparing `xturing-0.1.2/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.3/src/xturing/engines/llama_utils/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.3/src/xturing/engines/lora_engine/lora.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/lora_engine/save_and_load.py` & `xturing-0.1.3/src/xturing/engines/lora_engine/save_and_load.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/opt_engine.py` & `xturing-0.1.3/src/xturing/engines/opt_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/quant_utils/custom_autotune.py` & `xturing-0.1.3/src/xturing/engines/quant_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/engines/quant_utils/quant.py` & `xturing-0.1.3/src/xturing/engines/quant_utils/quant.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/model_apis/__init__.py` & `xturing-0.1.3/src/xturing/model_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/model_apis/ai21.py` & `xturing-0.1.3/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/model_apis/base.py` & `xturing-0.1.3/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/model_apis/cohere.py` & `xturing-0.1.3/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/model_apis/openai.py` & `xturing-0.1.3/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/__init__.py` & `xturing-0.1.3/src/xturing/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/base.py` & `xturing-0.1.3/src/xturing/models/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/bloom.py` & `xturing-0.1.3/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/causal.py` & `xturing-0.1.3/src/xturing/models/causal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from pathlib import Path
-from typing import Iterable, List, Optional, Union
+from typing import Iterable, List, Optional, Union, Type
 
 import torch
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from xturing.config import DEFAULT_DEVICE, assert_not_cpu_int8
 from xturing.config.config_data_classes import FinetuningConfig, GenerationConfig
@@ -14,14 +14,15 @@
 from xturing.engines.base import BaseEngine
 from xturing.engines.causal import CausalLoraEngine
 from xturing.models import BaseModel
 from xturing.preprocessors.base import BasePreprocessor
 from xturing.trainers.base import BaseTrainer
 from xturing.trainers.lightning_trainer import LightningTrainer
 from xturing.utils.logging import configure_logger
+from pytorch_lightning.loggers import Logger
 
 logger = configure_logger(__name__)
 
 
 class CausalModel(BaseModel):
     def __init__(self, engine: str, weights_path: Optional[str] = None):
         self.engine = BaseEngine.create(engine, weights_path)
@@ -59,32 +60,35 @@
         return BasePreprocessor.create(
             dataset.config_name,
             self.engine.tokenizer,
             int(self.finetuning_args.max_length),
             dataset.meta,
         )
 
-    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset]):
+    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset], 
+                      logger: Union[Logger, Iterable[Logger], bool] = True):
         return BaseTrainer.create(
             LightningTrainer.config_name,
             self.engine,
             dataset,
             self._make_collate_fn(dataset),
             int(self.finetuning_args.num_train_epochs),
             int(self.finetuning_args.batch_size),
             float(self.finetuning_args.learning_rate),
             self.finetuning_args.optimizer_name,
+            logger=logger,
         )
 
-    def finetune(self, dataset: Union[TextDataset, InstructionDataset]):
+    def finetune(self, dataset: Union[TextDataset, InstructionDataset], 
+                 logger: Union[Logger, Iterable[Logger], bool] = True):
         assert dataset.config_name in [
             "text_dataset",
             "instruction_dataset",
         ], "Please make sure the dataset_type is text_dataset or instruction_dataset"
-        trainer = self._make_trainer(dataset)
+        trainer = self._make_trainer(dataset, logger)
         trainer.fit()
 
     def evaluate(self, dataset: Union[TextDataset, InstructionDataset]):
         pass
 
     def _generate_from_iterable(
         self, data_iterator: Iterable, do_tokenization=False, show_tqdm_bar=True
@@ -184,26 +188,28 @@
         super().__init__(engine, weights_path)
 
 
 class CausalLoraModel(CausalModel):
     def __init__(self, engine: str, weights_path: Optional[str] = None):
         super().__init__(engine, weights_path)
 
-    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset]):
+    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset], 
+                      logger: Union[Logger, Iterable[Logger], bool] = True):
         return BaseTrainer.create(
             LightningTrainer.config_name,
             self.engine,
             dataset,
             self._make_collate_fn(dataset),
             int(self.finetuning_args.num_train_epochs),
             int(self.finetuning_args.batch_size),
             float(self.finetuning_args.learning_rate),
             self.finetuning_args.optimizer_name,
             True,
             True,
+            logger=logger,
         )
 
 
 class CausalLoraInt8Model(CausalLoraModel):
     def __init__(self, engine: str, weights_path: Optional[str] = None):
         assert_not_cpu_int8()
         super().__init__(engine, weights_path)
```

### Comparing `xturing-0.1.2/src/xturing/models/cerebras.py` & `xturing-0.1.3/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/distilgpt2.py` & `xturing-0.1.3/src/xturing/models/distilgpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/galactica.py` & `xturing-0.1.3/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/gpt2.py` & `xturing-0.1.3/src/xturing/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/gptj.py` & `xturing-0.1.3/src/xturing/models/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/models/llama.py` & `xturing-0.1.3/src/xturing/models/llama.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List, Optional, Union
+from typing import Iterable, List, Optional, Union
+from pytorch_lightning.loggers import Logger
 
 from xturing.engines.llama_engine import (
     LLamaEngine,
     LLamaInt8Engine,
     LlamaLoraEngine,
     LlamaLoraInt8Engine,
     LlamaLoraInt4Engine,
@@ -46,24 +47,26 @@
     def __init__(self, weights_path: Optional[str] = None):
         super().__init__(LlamaLoraInt8Engine.config_name, weights_path)
 
 
 class LlamaLoraInt4(CausalLoraInt8Model):
     config_name: str = "llama_lora_int4"
 
-    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset]):
+    def _make_trainer(self, dataset: Union[TextDataset, InstructionDataset], 
+                      logger: Union[Logger, Iterable[Logger], bool] = True):
         return BaseTrainer.create(
             LightningTrainer.config_name,
             self.engine,
             dataset,
             self._make_collate_fn(dataset),
             int(self.finetuning_args.num_train_epochs),
             int(self.finetuning_args.batch_size),
             float(self.finetuning_args.learning_rate),
             self.finetuning_args.optimizer_name,
             True,
             True,
             lora_type=32,
+            logger=logger,
         )
 
     def __init__(self, weights_path: Optional[str] = None):
         super().__init__(LlamaLoraInt4Engine.config_name, weights_path)
```

### Comparing `xturing-0.1.2/src/xturing/models/opt.py` & `xturing-0.1.3/src/xturing/models/opt.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.3/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.3/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/registry.py` & `xturing-0.1.3/src/xturing/registry.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.3/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.3/src/xturing/self_instruct/generate_instances.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.3/src/xturing/self_instruct/identify_if_classification.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.3/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.3/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.3/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.3/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.3/src/xturing/trainers/lightning_trainer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import datetime
 import os
 import tempfile
 import uuid
 from pathlib import Path
-from typing import Optional, Union
+from typing import Iterable, Optional, Union, Type
 
 import pytorch_lightning as pl
 import torch
 from deepspeed.ops.adam import DeepSpeedCPUAdam
 from pytorch_lightning import callbacks
 from pytorch_lightning.trainer.trainer import Trainer
+from pytorch_lightning.loggers import Logger
 
 from xturing.config import DEFAULT_DEVICE, IS_INTERACTIVE
 from xturing.datasets.base import BaseDataset
 from xturing.engines.base import BaseEngine
 from xturing.preprocessors.base import BasePreprocessor
 
 
@@ -97,14 +98,15 @@
         batch_size: int = 2,
         learning_rate: float = 1e-3,
         optimizer_name: str = "adamw",
         use_lora: bool = False,
         use_deepspeed: bool = False,
         max_training_time_in_secs: Optional[int] = None,
         lora_type: int = 16,
+        logger: Union[Logger, Iterable[Logger], bool] = True,
     ):
         self.lightning_model = TuringLightningModule(
             model_engine=model_engine,
             train_dataset=train_dataset,
             preprocessor=preprocessor,
             batch_size=batch_size,
             learning_rate=learning_rate,
@@ -141,23 +143,25 @@
             self.trainer = Trainer(
                 num_nodes=1,
                 accelerator="cpu",
                 max_epochs=max_epochs,
                 callbacks=training_callbacks,
                 enable_checkpointing=False,
                 log_every_n_steps=50,
+                logger=logger,
             )
         elif not use_lora and not use_deepspeed:
             self.trainer = Trainer(
                 num_nodes=1,
                 accelerator="gpu",
                 max_epochs=max_epochs,
                 callbacks=training_callbacks,
                 enable_checkpointing=True,
                 log_every_n_steps=50,
+                logger=logger,
             )
         else:
             training_callbacks = [
                 callbacks.ModelCheckpoint(
                     dirpath=str(checkpoints_dir_path), save_on_train_epoch_end=True
                 ),
             ]
@@ -175,14 +179,15 @@
                 accelerator="gpu",
                 strategy=strategy,
                 precision=lora_type,
                 max_epochs=max_epochs,
                 callbacks=training_callbacks,
                 enable_checkpointing=True,
                 log_every_n_steps=50,
+                logger=logger,
             )
 
     def fit(self):
         self.trainer.fit(self.lightning_model)
         if self.trainer.checkpoint_callback is not None:
             self.trainer.checkpoint_callback.best_model_path
```

### Comparing `xturing-0.1.2/src/xturing/ui/playground.py` & `xturing-0.1.3/src/xturing/ui/playground.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/utils/hub.py` & `xturing-0.1.3/src/xturing/utils/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                     current,
                     total,
                 )
                 sys.stdout.write("\r" + progress_message)
                 sys.stdout.flush()
 
             try:
-                wget.download(url, str(zip_filename), bar=bar_progress)
+                wget.download(url, str(zip_filename))
 
                 with ZipFile(zip_filename, "r") as zip_ref:
                     zip_ref.extractall(path=model_dir)
 
                 print(f"Downloaded model {model_name} from {url}")
 
                 # if zip has folder with model, move files to root
```

### Comparing `xturing-0.1.2/src/xturing/utils/logging.py` & `xturing-0.1.3/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/utils/loss_fns.py` & `xturing-0.1.3/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/utils/notebooks.py` & `xturing-0.1.3/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/utils/text_splitter.py` & `xturing-0.1.3/src/xturing/utils/text_splitter.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing/utils/utils.py` & `xturing-0.1.3/src/xturing/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.2/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.3/src/xturing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -243,20 +243,20 @@
     <img src="https://img.shields.io/badge/Chat-FFFFFF?logo=discord&style=for-the-badge"/>
   </a>
 </p>
 <br>
 
 ___
 
-`xturing` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
+`xTuring` provides fast, efficient and simple fine-tuning of LLMs, such as LLaMA, GPT-J, Galactica, and more.
 By providing an easy-to-use interface for fine-tuning LLMs to your own data and application, xTuring makes it
 simple to build, customize and control LLMs. The entire process can be done inside your computer or in your
 private cloud, ensuring data privacy and security.
 
-With `xturing` you can,
+With `xTuring` you can,
 - Ingest data from different sources and preprocess them to a format LLMs can understand
 - Scale from single to multiple GPUs for faster fine-tuning
 - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning) to reduce hardware costs by up to 90%
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
@@ -370,15 +370,15 @@
 - [x] Support for LLaMA, GPT-J, GPT-2, OPT, Cerebras-GPT, Galactica and Bloom models
 - [x] Dataset generation using self-instruction
 - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
-- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation 
+- [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
 - [ ] Evaluation of LLM models
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.2/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.3/src/xturing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

