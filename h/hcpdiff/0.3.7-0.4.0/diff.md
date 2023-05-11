# Comparing `tmp/hcpdiff-0.3.7.tar.gz` & `tmp/hcpdiff-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.3.7.tar", last modified: Sun May  7 12:16:10 2023, max compression
+gzip compressed data, was "hcpdiff-0.4.0.tar", last modified: Thu May 11 13:30:21 2023, max compression
```

## Comparing `hcpdiff-0.3.7.tar` & `hcpdiff-0.4.0.tar`

### file list

```diff
@@ -1,104 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/change_vae.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/euler_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/img2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/img2img_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/text2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/text2img_DA++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/infer/webui_model_infer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/plugins/plugin_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/te_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.911243 hcpdiff-0.3.7/cfgs/train/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/cfgs/train/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/CustomDiffusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/DreamArtist++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/DreamArtist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/DreamBooth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/Lion_optimizer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/TextualInversion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/fine-tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/locon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/lora_conventional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/examples/min_snr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/train_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/train/tuning_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/cfgs/unet_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/ckpt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/ckpt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_safetensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/data/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/cond_pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/cli_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loss/min_snr_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/loss/mse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/hcpdiff/models/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/cfg_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/lora_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/text_emb_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/textencoder_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/models/tokenizer_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/hcpdiff/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/convert_caption_txt2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/create_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/gen_from_ptlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/init_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/lora_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/tools/sd2diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27108 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/train_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/train_ac_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/train_colo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/hcpdiff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/caption_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/cfg_net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/colo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/img_size_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/hcpdiff/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.915243 hcpdiff-0.3.7/hcpdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 12:16:10.000000 hcpdiff-0.3.7/hcpdiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/prompt_tuning_template/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/name.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/name_2pt_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/name_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/object.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/object_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/style.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/prompt_tuning_template/style_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 12:16:10.919243 hcpdiff-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-07 12:16:00.000000 hcpdiff-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.573662 hcpdiff-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-11 13:30:21.573662 hcpdiff-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.565662 hcpdiff-0.4.0/cfgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/deepspeed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.565662 hcpdiff-0.4.0/cfgs/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/infer/change_vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/infer/euler_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/infer/img2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/infer/img2img_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/infer/text2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/infer/text2img_DA++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/infer/webui_model_infer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.565662 hcpdiff-0.4.0/cfgs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/plugins/plugin_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/te_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.565662 hcpdiff-0.4.0/cfgs/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.565662 hcpdiff-0.4.0/cfgs/train/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/CustomDiffusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/DreamArtist++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/DreamArtist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/DreamBooth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/Lion_optimizer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/TextualInversion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/fine-tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/locon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/lora_conventional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/examples/min_snr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/train_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/train/tuning_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/cfgs/unet_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.565662 hcpdiff-0.4.0/hcpdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.569662 hcpdiff-0.4.0/hcpdiff/ckpt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/ckpt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/ckpt_manager/ckpt_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/ckpt_manager/ckpt_safetensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.569662 hcpdiff-0.4.0/hcpdiff/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/data/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/data/cond_pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/data/pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.569662 hcpdiff-0.4.0/hcpdiff/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loggers/cli_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.569662 hcpdiff-0.4.0/hcpdiff/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loss/min_snr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.569662 hcpdiff-0.4.0/hcpdiff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/cfg_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/lora_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/text_emb_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/textencoder_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/models/tokenizer_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.569662 hcpdiff-0.4.0/hcpdiff/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/noise/noise_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/noise/pyramid_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.573662 hcpdiff-0.4.0/hcpdiff/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/tools/convert_caption_txt2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/tools/create_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/tools/gen_from_ptlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/tools/init_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/tools/lora_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/tools/sd2diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27596 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/train_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/train_ac_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/train_colo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/train_deepspeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.573662 hcpdiff-0.4.0/hcpdiff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/caption_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/cfg_net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/colo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/img_size_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/hcpdiff/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.569662 hcpdiff-0.4.0/hcpdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-11 13:30:21.000000 hcpdiff-0.4.0/hcpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-11 13:30:21.000000 hcpdiff-0.4.0/hcpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:30:21.000000 hcpdiff-0.4.0/hcpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 13:30:21.000000 hcpdiff-0.4.0/hcpdiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 13:30:21.000000 hcpdiff-0.4.0/hcpdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 13:30:21.000000 hcpdiff-0.4.0/hcpdiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:30:21.573662 hcpdiff-0.4.0/prompt_tuning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/name.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/name_2pt_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/name_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/object.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/object_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/prompt_tuning_template/style_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:30:21.573662 hcpdiff-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-11 13:30:09.000000 hcpdiff-0.4.0/setup.py
```

### Comparing `hcpdiff-0.3.7/LICENSE` & `hcpdiff-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/PKG-INFO` & `hcpdiff-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.7
+Version: 0.4.0
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.3.7/README.md` & `hcpdiff-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/infer/euler_a.yaml` & `hcpdiff-0.4.0/cfgs/infer/euler_a.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/infer/img2img.yaml` & `hcpdiff-0.4.0/cfgs/infer/img2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/infer/img2img_controlnet.yaml` & `hcpdiff-0.4.0/cfgs/infer/img2img_controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/infer/text2img.yaml` & `hcpdiff-0.4.0/cfgs/infer/text2img.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/infer/text2img_DA++.yaml` & `hcpdiff-0.4.0/cfgs/infer/text2img_DA++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/infer/webui_model_infer.yaml` & `hcpdiff-0.4.0/cfgs/infer/webui_model_infer.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/te_struct.txt` & `hcpdiff-0.4.0/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/DreamArtist++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/controlnet.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/controlnet.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/locon.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/locon.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 lora_unet:
   - # Linear
     lr: 1e-4
     rank: 8
     layers:
       - 're:.*\.attn.?$'
-      - 're:.*\.ff\.net\.0$'
+      - 're:.*\.ff$'
   - # Conv2d
     lr: 1e-4
     rank: 8
     layers:
       - 're:.*\.resnets$'
       - 're:.*\.proj_in$'
       - 're:.*\.proj_out$'
```

### Comparing `hcpdiff-0.3.7/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.4.0/cfgs/train/examples/lora_conventional.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 lora_unet:
   -
     lr: 1e-4
     rank: 8
     layers:
       - 're:.*\.attn.?$'
-      - 're:.*\.ff\.net\.0$'
+      - 're:.*\.ff$'
 
 lora_text_encoder:
   - lr: 1e-5
     rank: 4
     layers:
       - 're:.*self_attn$'
       - 're:.*mlp$'
```

### Comparing `hcpdiff-0.3.7/cfgs/train/train_base.yaml` & `hcpdiff-0.4.0/cfgs/train/train_base.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -64,15 +64,17 @@
   tokenizer_name: null
   tokenizer_repeats: 2
   enable_xformers: True
   gradient_checkpointing: True
   ema_unet: 0 # 0 to disable
   ema_text_encoder: 0 # 0 to disable
   clip_skip: 0
-  noise_scheduler: DDPMScheduler
+  noise_scheduler:
+    _target_: diffusers.DDPMScheduler.from_pretrained
+    _partial_: True
 
 data:
   dataset1:
     _target_: hcpdiff.data.TextImagePairDataset
     _partial_: True # Not directly instantiate the object here. There are other parameters to be added in the runtime.
     batch_size: 4
     cache_latents: True
```

### Comparing `hcpdiff-0.3.7/cfgs/train/tuning_base.yaml` & `hcpdiff-0.4.0/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/cfgs/unet_struct.txt` & `hcpdiff-0.4.0/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.4.0/hcpdiff/ckpt_manager/ckpt_pkl.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.4.0/hcpdiff/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/data/__init__.py` & `hcpdiff-0.4.0/hcpdiff/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/data/bucket.py` & `hcpdiff-0.4.0/hcpdiff/data/bucket.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/data/cond_pair_dataset.py` & `hcpdiff-0.4.0/hcpdiff/data/cond_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.4.0/hcpdiff/data/pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/data/utils.py` & `hcpdiff-0.4.0/hcpdiff/data/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from PIL import Image
 import torch
 import cv2
+import numpy as np
 
 from torchvision import transforms as T
 from torchvision.transforms import functional as F
 
 
 class DualRandomCrop(object):
     def __init__(self, size):
         self.size = size
 
     def __call__(self, img):
         crop_params = T.RandomCrop.get_params(img['img'], self.size)
         img['img'] = F.crop(img['img'], *crop_params)
         if "mask" in img:
-            img['mask'] = F.crop(img['mask'], *crop_params)
+            img['mask'] = self.crop(img['mask'], *crop_params)
         if "cond" in img:
             img['cond'] = F.crop(img['cond'], *crop_params)
         return img
 
+    @staticmethod
+    def crop(img: np.ndarray, top: int, left: int, height: int, width: int) -> np.ndarray:
+        right = left + width
+        bottom = top + height
+        return img[..., top:bottom, left:right]
+
 def resize_crop_fix(img, target_size):
     w,h=img['img'].size
     if w==target_size[0] and h==target_size[1]:
         return img
 
     ratio_img=w/h
     if ratio_img > target_size[0]/target_size[1]:
```

### Comparing `hcpdiff-0.3.7/hcpdiff/loggers/base_logger.py` & `hcpdiff-0.4.0/hcpdiff/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/loggers/cli_logger.py` & `hcpdiff-0.4.0/hcpdiff/loggers/cli_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/loggers/tensorboard_logger.py` & `hcpdiff-0.4.0/hcpdiff/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/loggers/wandb_logger.py` & `hcpdiff-0.4.0/hcpdiff/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/loss/min_snr_loss.py` & `hcpdiff-0.4.0/hcpdiff/loss/min_snr_loss.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/cfg_context.py` & `hcpdiff-0.4.0/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/controlnet.py` & `hcpdiff-0.4.0/hcpdiff/models/controlnet.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/layers.py` & `hcpdiff-0.4.0/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/lora_base.py` & `hcpdiff-0.4.0/hcpdiff/models/lora_base.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/lora_layers.py` & `hcpdiff-0.4.0/hcpdiff/models/lora_layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/plugin.py` & `hcpdiff-0.4.0/hcpdiff/models/plugin.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.4.0/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.4.0/hcpdiff/models/textencoder_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.4.0/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.4.0/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.4.0/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.4.0/hcpdiff/tools/gen_from_ptlist.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/tools/init_proj.py` & `hcpdiff-0.4.0/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/tools/lora_convert.py` & `hcpdiff-0.4.0/hcpdiff/tools/lora_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument("--lora_path", default=None, type=str, required=True, help="Path to the lora to convert.")
     parser.add_argument("--lora_path_TE", default=None, type=str, help="Path to the hcp text encoder lora to convert.")
     parser.add_argument("--dump_path", default=None, type=str, required=True, help="Path to save the converted state dict.")
     parser.add_argument("--from_webui", default=None, action="store_true")
     parser.add_argument("--to_webui", default=None, action="store_true")
+    parser.add_argument("--auto_scale_alpha", default=None, action="store_true")
     args = parser.parse_args()
 
     converter = LoraConverter()
     lora_name = os.path.basename(args.lora_path)
 
     # load lora model
     print('convert lora model')
@@ -79,9 +80,11 @@
         ckpt_manager._save_ckpt(sd_unet, save_path=unet_path)
         print('save text encoder lora to:', TE_path)
         print('save unet lora to:', unet_path)
     elif args.to_webui:
         sd_unet = ckpt_manager.load_ckpt(args.lora_path)
         sd_TE = ckpt_manager.load_ckpt(args.lora_path_TE)
         state = converter.convert_to_webui(sd_unet['lora'], sd_TE['lora'])
-        ckpt_manager._save_ckpt(sd_TE, save_path=args.dump_path)
-        print('save lora to:', args.dump_path)
+        if args.auto_scale_alpha:
+            state = {k:(v*v.shape[1] if 'lora_up' in k else v) for k,v in state.items()}
+        ckpt_manager._save_ckpt(state, save_path=args.dump_path)
+        print('save lora to:', args.dump_path)
```

### Comparing `hcpdiff-0.3.7/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.4.0/hcpdiff/tools/sd2diffusers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/train_ac.py` & `hcpdiff-0.4.0/hcpdiff/train_ac.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,34 +15,36 @@
 import time
 from functools import partial
 
 import diffusers
 import hydra
 import numpy as np
 import torch
+from torch import nn
 import torch.utils.checkpoint
 import torch.utils.data
 import transformers
 from accelerate import Accelerator, DistributedDataParallelKwargs
 from accelerate.utils import set_seed
 from diffusers import AutoencoderKL, UNet2DConditionModel
 from diffusers.utils.import_utils import is_xformers_available
 from omegaconf import OmegaConf
 from transformers import AutoTokenizer
-from  functools import partial
+from functools import partial
 
 from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
 from hcpdiff.data import RatioBucket, DataGroup, collate_fn_ft
 from hcpdiff.loggers import LoggerGroup
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
 from hcpdiff.utils.cfg_net_tools import make_hcpdiff, make_plugin
 from hcpdiff.utils.ema import ModelEMA
 from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper, load_emb
 from hcpdiff.utils.utils import load_config_with_cli, get_cfg_range, mgcd
 from hcpdiff.visualizer import Visualizer
+from hcpdiff.noise import NoiseBase
 
 class Trainer:
     def __init__(self, cfgs_raw):
         cfgs = hydra.utils.instantiate(cfgs_raw)
         self.cfgs = cfgs
 
         self.init_context(cfgs_raw)
@@ -97,14 +99,15 @@
             self.build_ema()
 
         self.load_resume()
 
         if cfgs.allow_tf32:
             torch.backends.cuda.matmul.allow_tf32 = True
 
+        self.freeze_model()
         self.prepare()
 
     @property
     def device(self):
         return self.accelerator.device
 
     @property
@@ -124,43 +127,47 @@
         self.world_size = self.accelerator.num_processes
 
         set_seed(self.cfgs.seed+self.local_rank)
 
     def prepare(self):
         # Prepare everything with accelerator.
         if self.train_TE:
-            # try:
-            #     self.TE_unet = torch.compile(self.TE_unet)
-            # except:
-            #     print('cannot compile model')
             prepare_obj_list = [self.TE_unet]
             prepare_name_list = ['TE_unet']
         else:
-            # try:
-            #     self.unet = torch.compile(self.unet)
-            #     self.text_encoder = torch.compile(self.text_encoder)
-            # except:
-            #     print('cannot compile model')
             prepare_obj_list = [self.unet]
             prepare_name_list = ['unet']
         if hasattr(self, 'optimizer'):
             prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
             prepare_name_list.extend(['optimizer', 'lr_scheduler'])
         if hasattr(self, 'optimizer_pt'):
             prepare_obj_list.extend([self.optimizer_pt, self.lr_scheduler_pt])
             prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
 
+        prepare_obj_list.extend(self.train_loader_group.loader_list)
         prepared_obj = self.accelerator.prepare(*prepare_obj_list)
+
+        ds_num = len(self.train_loader_group.loader_list)
+        self.train_loader_group.loader_list = prepared_obj[-ds_num:]
+        prepared_obj = prepared_obj[:-ds_num]
+
         for name, obj in zip(prepare_name_list, prepared_obj):
             setattr(self, name, obj)
 
-        if len(self.train_loader_group) > 1:
-            self.train_loader_group.loader_list = list(self.accelerator.prepare(*self.train_loader_group.loader_list))
+    def freeze_model(self):
+        if self.train_TE:
+            for name, m in self.TE_unet.named_modules():
+                if isinstance(m, nn.Dropout) and not m.training:
+                    m.p = 0.
+            self.TE_unet.train()
         else:
-            self.train_loader_group.loader_list = [self.accelerator.prepare(*self.train_loader_group.loader_list)]
+            for name, m in self.unet.named_modules():
+                if isinstance(m, nn.Dropout) and not m.training:
+                    m.p = 0.
+            self.unet.train()
 
     def scale_lr(self, parameters):
         bs = sum(self.batch_size_list)
         scale_factor = bs*self.world_size*self.cfgs.train.gradient_accumulation_steps
         for param in parameters:
             if 'lr' in param:
                 param['lr'] *= scale_factor
@@ -172,16 +179,22 @@
         elif self.cfgs.model.pretrained_model_name_or_path:
             self.tokenizer = AutoTokenizer.from_pretrained(
                 self.cfgs.model.pretrained_model_name_or_path, subfolder="tokenizer",
                 revision=self.cfgs.model.revision, use_fast=False,
             )
 
         # Load scheduler and models
-        self.noise_scheduler = getattr(diffusers, self.cfgs.model.noise_scheduler) \
-            .from_pretrained(self.cfgs.model.pretrained_model_name_or_path, subfolder="scheduler")
+        noise_scheduler=self.cfgs.model.noise_scheduler
+        noise_class = getattr(noise_scheduler.func, '__self__', noise_scheduler.func)  # support static or class method
+        if issubclass(noise_class, NoiseBase):
+            base_scheduler = noise_scheduler.keywords.pop('base_scheduler')(self.cfgs.model.pretrained_model_name_or_path, subfolder="scheduler")
+            self.noise_scheduler = noise_scheduler(base_scheduler)
+        else:
+            self.noise_scheduler = noise_scheduler(self.cfgs.model.pretrained_model_name_or_path, subfolder="scheduler")
+
         self.num_train_timesteps = len(self.noise_scheduler.timesteps)
         self.vae: AutoencoderKL = AutoencoderKL.from_pretrained(self.cfgs.model.pretrained_model_name_or_path, subfolder="vae",
                                                                 revision=self.cfgs.model.revision)
         self.build_unet_and_TE()
 
     def build_unet_and_TE(self):  # for easy to use colossalAI
         self.unet = UNet2DConditionModel.from_pretrained(
```

### Comparing `hcpdiff-0.3.7/hcpdiff/train_ac_single.py` & `hcpdiff-0.4.0/hcpdiff/train_ac_single.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,42 +18,37 @@
 
         self.local_rank = 0
         self.world_size = self.accelerator.num_processes
 
         set_seed(self.cfgs.seed + self.local_rank)
 
     def prepare(self):
-        # try:
-        #     self.unet = torch.compile(self.unet)
-        #     self.text_encoder = torch.compile(self.text_encoder)
-        # except:
-        #     print('cannot compile model')
-
         # Prepare everything with accelerator.
         prepare_obj_list = [self.unet]
         prepare_name_list = ['unet']
         if hasattr(self, 'optimizer'):
             prepare_obj_list.extend([self.optimizer, self.lr_scheduler])
             prepare_name_list.extend(['optimizer', 'lr_scheduler'])
         if hasattr(self, 'optimizer_pt'):
             prepare_obj_list.extend([self.optimizer_pt, self.lr_scheduler_pt])
             prepare_name_list.extend(['optimizer_pt', 'lr_scheduler_pt'])
         if self.train_TE:
             prepare_obj_list.append(self.text_encoder)
             prepare_name_list.append('text_encoder')
 
+        prepare_obj_list.extend(self.train_loader_group.loader_list)
         prepared_obj = self.accelerator.prepare(*prepare_obj_list)
+
+        ds_num = len(self.train_loader_group.loader_list)
+        self.train_loader_group.loader_list = list(prepared_obj[-ds_num:])
+        prepared_obj = prepared_obj[:-ds_num]
+
         for name, obj in zip(prepare_name_list, prepared_obj):
             setattr(self, name, obj)
 
-        if len(self.train_loader_group)>1:
-            self.train_loader_group.loader_list = list(self.accelerator.prepare(*self.train_loader_group.loader_list))
-        else:
-            self.train_loader_group.loader_list = [self.accelerator.prepare(*self.train_loader_group.loader_list)]
-
     def build_data(self, data_builder:partial) -> torch.utils.data.DataLoader:
         batch_size = data_builder.keywords.pop('batch_size')
         cache_latents = data_builder.keywords.pop('cache_latents')
         self.batch_size_list.append(batch_size)
 
         train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
         train_dataset.bucket.build(batch_size * self.world_size,
```

### Comparing `hcpdiff-0.3.7/hcpdiff/train_colo.py` & `hcpdiff-0.4.0/hcpdiff/train_colo.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.4.0/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.4.0/hcpdiff/utils/cfg_net_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.4.0/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/utils/ema.py` & `hcpdiff-0.4.0/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.4.0/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/utils/net_utils.py` & `hcpdiff-0.4.0/hcpdiff/utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/hcpdiff/utils/utils.py` & `hcpdiff-0.4.0/hcpdiff/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,26 +61,29 @@
         return float(l), float(h), dy_cfg_f
     else:
         return float(cfg_text), float(cfg_text), dy_cfg_f
 
 def to_validate_file(name):
     rstr = r"[\/\\\:\*\?\"\<\>\|]"  # '/ \ : * ? " < > |'
     new_title = re.sub(rstr, "_", name)  # 替换为下划线
-    return new_title
+    return new_title[:50]
 
 def make_mask(start, end, length):
     mask=torch.zeros(length)
     mask[int(length*start):int(length*end)]=1
     return mask.bool()
 
 def get_file_name(file: str):
     return file.rsplit('.',1)[0]
 
 def get_file_ext(file: str):
-    return file.rsplit('.',1)[1].lower()
+    try:
+        return file.rsplit('.',1)[1].lower()
+    except:
+        return ''
 
 def factorization(dimension: int, factor:int=-1) -> Tuple[int, int]:
     find_one = lambda x: len(x) - (x.rfind('1') + 1)
     dim_bin = bin(dimension)
     num = find_one(dim_bin)
     f_max = (len(dim_bin)-3)>>1 if factor<0 else find_one(bin(factor))
     num = min(num, f_max)
```

### Comparing `hcpdiff-0.3.7/hcpdiff/visualizer.py` & `hcpdiff-0.4.0/hcpdiff/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                     feeder(ex_input_dict)
 
             images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
         return images
 
     def save_images(self, images, root, prompt, negative_prompt='', save_cfg=True):
         os.makedirs(root, exist_ok=True)
-        num_img_exist = max([int(x.split('-', 1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support]) + 1
+        num_img_exist = max([0]+[int(x.split('-', 1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support]) + 1
 
         for p, pn, img in zip(prompt, negative_prompt, images):
             img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.{self.cfgs.save.image_type}"), quality=self.cfgs.save.quality)
 
             if save_cfg:
                 with open(os.path.join(root, f"{num_img_exist}-info.yaml"), 'w', encoding='utf-8') as f:
                     f.write(OmegaConf.to_yaml(self.cfgs_raw))
```

### Comparing `hcpdiff-0.3.7/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.4.0/hcpdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.3.7
+Version: 0.4.0
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.3.7/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.4.0/hcpdiff.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+cfgs/deepspeed.json
 cfgs/te_struct.txt
 cfgs/unet_struct.txt
 cfgs/infer/change_vae.yaml
 cfgs/infer/euler_a.yaml
 cfgs/infer/img2img.yaml
 cfgs/infer/img2img_controlnet.yaml
 cfgs/infer/text2img.yaml
@@ -24,14 +25,15 @@
 cfgs/train/examples/locon.yaml
 cfgs/train/examples/lora_conventional.yaml
 cfgs/train/examples/min_snr.yaml
 hcpdiff/__init__.py
 hcpdiff/train_ac.py
 hcpdiff/train_ac_single.py
 hcpdiff/train_colo.py
+hcpdiff/train_deepspeed.py
 hcpdiff/visualizer.py
 hcpdiff.egg-info/PKG-INFO
 hcpdiff.egg-info/SOURCES.txt
 hcpdiff.egg-info/dependency_links.txt
 hcpdiff.egg-info/entry_points.txt
 hcpdiff.egg-info/requires.txt
 hcpdiff.egg-info/top_level.txt
@@ -57,14 +59,17 @@
 hcpdiff/models/layers.py
 hcpdiff/models/lora_base.py
 hcpdiff/models/lora_layers.py
 hcpdiff/models/plugin.py
 hcpdiff/models/text_emb_ex.py
 hcpdiff/models/textencoder_ex.py
 hcpdiff/models/tokenizer_ex.py
+hcpdiff/noise/__init__.py
+hcpdiff/noise/noise_base.py
+hcpdiff/noise/pyramid_noise.py
 hcpdiff/tools/__init__.py
 hcpdiff/tools/convert_caption_txt2json.py
 hcpdiff/tools/create_embedding.py
 hcpdiff/tools/gen_from_ptlist.py
 hcpdiff/tools/init_proj.py
 hcpdiff/tools/lora_convert.py
 hcpdiff/tools/sd2diffusers.py
```

### Comparing `hcpdiff-0.3.7/prompt_tuning_template/object.txt` & `hcpdiff-0.4.0/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.4.0/prompt_tuning_template/object_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/prompt_tuning_template/style.txt` & `hcpdiff-0.4.0/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.4.0/prompt_tuning_template/style_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.3.7/setup.py` & `hcpdiff-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.3.7",
+    version="0.4.0",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

