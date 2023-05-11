# Comparing `tmp/scdiffeq-0.0.46rc1.tar.gz` & `tmp/scdiffeq-0.0.46rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdiffeq-0.0.46rc1.tar", last modified: Thu May  4 21:39:42 2023, max compression
+gzip compressed data, was "scdiffeq-0.0.46rc3.tar", last modified: Thu May 11 20:09:20 2023, max compression
```

## Comparing `scdiffeq-0.0.46rc1.tar` & `scdiffeq-0.0.46rc3.tar`

### file list

```diff
@@ -1,117 +1,107 @@
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.640339 scdiffeq-0.0.46rc1/
--rw-r--r--   0 mvinyard   (503) staff       (20)    34523 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/LICENSE
--rw-r--r--   0 mvinyard   (503) staff       (20)     2299 2023-05-04 21:39:42.639987 scdiffeq-0.0.46rc1/PKG-INFO
--rw-r--r--   0 mvinyard   (503) staff       (20)     1627 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/README.md
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.619005 scdiffeq-0.0.46rc1/scdiffeq/
--rw-r--r--   0 mvinyard   (503) staff       (20)      665 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/__init__.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.620626 scdiffeq-0.0.46rc1/scdiffeq/core/
--rw-r--r--   0 mvinyard   (503) staff       (20)      950 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/__init__.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.622944 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/
--rw-r--r--   0 mvinyard   (503) staff       (20)      567 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1864 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_batch_processor.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1894 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_drift_net.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1787 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_ode.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      568 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_potential_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2340 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3139 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_sde_latent_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3118 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_vae_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      751 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_sinkhorn_divergence.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.624384 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/
--rw-r--r--   0 mvinyard   (503) staff       (20)      267 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1816 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_diffeq.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1000 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_drift_net.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      606 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_ode.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      675 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_lightning_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1876 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/base_models/_base_velocity_diffeq.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.625735 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/
--rw-r--r--   0 mvinyard   (503) staff       (20)      213 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      123 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_base_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      488 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_potential_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1282 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_pre_train_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1139 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_vae_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      968 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/mix_ins/_vae_pre_train_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)    18660 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/_scdiffeq.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.626797 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/
--rw-r--r--   0 mvinyard   (503) staff       (20)      593 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      271 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_gradient_potential_callback.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      834 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_intermittent_saves.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     4853 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_loss_accounting.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      806 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_testing.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.628134 scdiffeq-0.0.46rc1/scdiffeq/core/configs/
--rw-r--r--   0 mvinyard   (503) staff       (20)      488 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2178 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_function_credentialling.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1455 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_callbacks_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1594 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_data_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     5708 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1606 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration_v2.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     5672 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_trainer_configuration.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     6074 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/configs/_time_configuration.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.631183 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/
--rw-r--r--   0 mvinyard   (503) staff       (20)     1079 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1554 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1057 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2351 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2456 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2277 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3052 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1768 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1595 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2550 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2838 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3044 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2909 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.631851 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/
--rw-r--r--   0 mvinyard   (503) staff       (20)      154 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3415 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2458 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_batch_processor.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      752 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.633345 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/
--rw-r--r--   0 mvinyard   (503) staff       (20)      282 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      624 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2557 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      318 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      868 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2264 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     8342 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.636524 scdiffeq-0.0.46rc1/scdiffeq/core/utils/
--rw-r--r--   0 mvinyard   (503) staff       (20)     1070 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      611 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_abc_parse.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      931 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_anndata_inspector.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2802 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_autoparse_base_class.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1040 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_default_neural_sde.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1126 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_fast_graph.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      333 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_fetch_format.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1652 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_fetch.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     3402 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_kwargs.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      341 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_info_message.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      892 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_logging_learnable_hparams.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      395 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_normalize_time_to_range.py
--rw-r--r--   0 mvinyard   (503) staff       (20)       83 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_not_none_type.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     2339 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_scdiffeq_logger.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      346 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/core/utils/_sum_normalize.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.637024 scdiffeq-0.0.46rc1/scdiffeq/io/
--rw-r--r--   0 mvinyard   (503) staff       (20)      541 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/io/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      744 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/io/_pickle_io.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1258 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/io/_read_h5ad.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.637189 scdiffeq-0.0.46rc1/scdiffeq/plotting/
--rw-r--r--   0 mvinyard   (503) staff       (20)      462 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/plotting/__init__.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.639676 scdiffeq-0.0.46rc1/scdiffeq/tools/
--rw-r--r--   0 mvinyard   (503) staff       (20)      924 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/__init__.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1482 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_annotate_cells.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     4607 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_dimension_reduction.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1546 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_drift_diffusion_state_characterization.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      202 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_fetch.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1292 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_func_from_version.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1019 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_hyperparams.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     5462 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_reconstruct_function.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1470 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_time_free_sampling.py
--rw-r--r--   0 mvinyard   (503) staff       (20)      853 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_umap.py
--rw-r--r--   0 mvinyard   (503) staff       (20)     1242 2023-05-04 21:33:36.000000 scdiffeq-0.0.46rc1/scdiffeq/tools/_versions.py
-drwxr-xr-x   0 mvinyard   (503) staff       (20)        0 2023-05-04 21:39:42.620266 scdiffeq-0.0.46rc1/scdiffeq.egg-info/
--rw-r--r--   0 mvinyard   (503) staff       (20)     2299 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/PKG-INFO
--rw-r--r--   0 mvinyard   (503) staff       (20)     4634 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/SOURCES.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)        1 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/dependency_links.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)      272 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/requires.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)        9 2023-05-04 21:39:42.000000 scdiffeq-0.0.46rc1/scdiffeq.egg-info/top_level.txt
--rw-r--r--   0 mvinyard   (503) staff       (20)       38 2023-05-04 21:39:42.640426 scdiffeq-0.0.46rc1/setup.cfg
--rw-r--r--   0 mvinyard   (503) staff       (20)     1348 2023-05-04 21:39:40.000000 scdiffeq-0.0.46rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.114814 scdiffeq-0.0.46rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-11 20:09:20.114814 scdiffeq-0.0.46rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.106814 scdiffeq-0.0.46rc3/scdiffeq/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.106814 scdiffeq-0.0.46rc3/scdiffeq/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/_scdiffeq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.106814 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_gradient_potential_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_intermittent_saves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_loss_accounting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_visualize_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_visualize_tracked_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.106814 scdiffeq-0.0.46rc3/scdiffeq/core/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/_function_credentialling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_callbacks_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_data_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_model_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_model_configuration_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_trainer_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/configs/_time_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.110814 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_fate_bias_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae_fate_bias_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.110814 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/_batch_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.110814 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_fate_bias_drift_prior_vae_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_fate_bias_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_fate_bias_vae_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_potential_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.110814 scdiffeq-0.0.46rc3/scdiffeq/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_anndata_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_autoparse_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_default_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_display_tracked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_fast_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_fetch_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_filter_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_function_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_function_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_idx_to_int_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_info_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_knn_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_logging_learnable_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_normalize_time_to_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_not_none_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_scdiffeq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/core/utils/_sum_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.110814 scdiffeq-0.0.46rc3/scdiffeq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/io/_pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/io/_read_h5ad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.110814 scdiffeq-0.0.46rc3/scdiffeq/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.114814 scdiffeq-0.0.46rc3/scdiffeq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_annotate_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_drift_diffusion_state_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_func_from_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_hyperparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_reconstruct_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_time_free_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/scdiffeq/tools/_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:09:20.106814 scdiffeq-0.0.46rc3/scdiffeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-11 20:09:20.000000 scdiffeq-0.0.46rc3/scdiffeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-11 20:09:20.000000 scdiffeq-0.0.46rc3/scdiffeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:09:20.000000 scdiffeq-0.0.46rc3/scdiffeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-11 20:09:20.000000 scdiffeq-0.0.46rc3/scdiffeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 20:09:20.000000 scdiffeq-0.0.46rc3/scdiffeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:09:20.114814 scdiffeq-0.0.46rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-11 20:09:09.000000 scdiffeq-0.0.46rc3/setup.py
```

### Comparing `scdiffeq-0.0.46rc1/LICENSE` & `scdiffeq-0.0.46rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/PKG-INFO` & `scdiffeq-0.0.46rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.46rc1
+Version: 0.0.46rc3
 Summary: scDiffEq: modelling single-cell dynamics using neural differential equations.
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <a href=""><img src=docs/images/scdiffeq.logo.png alt="scdiffeq-logo" width="320"/>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc1 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc3 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
-:: 3.7 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
+:: 3.9 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
 Content-Type: text/markdown License-File: LICENSE # [scdiffeq-logo] [![PyPI
 pyversions](https://img.shields.io/pypi/pyversions/scdiffeq.svg)](https://
 pypi.python.org/pypi/scdiffeq/) [![PyPI version](https://badge.fury.io/py/
 scdiffeq.svg)](https://badge.fury.io/py/scdiffeq) [![Code style: black](https:/
 /img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) An analysis framework for modeling dynamical single-cell data with
```

### Comparing `scdiffeq-0.0.46rc1/README.md` & `scdiffeq-0.0.46rc3/README.md`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/__init__.py` & `scdiffeq-0.0.46rc3/scdiffeq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 __module_name__ = "__init__.py"
-__version__ = "0.0.45"
+__version__ = "0.0.46rc3"
 __doc__ = """Top-level __init__ for the scdiffeq package."""
 __author__ = ", ".join(["Michael E. Vinyard", "Anders Rasmussen", "Ruitong Li"])
 __email__ = ", ".join(
     [
         "mvinyard@broadinstitute.org",
         "arasmuss@broadinstitute.org",
         "ruitong@broadinstitute.org",
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_batch_processor.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/_batch_processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import ABCParse
 from typing import List
 import torch
 
-from .. import utils
+from ... import utils
+
+NoneType = type(None)
 
 class BatchRepr:
     def __init__(self, batch):
 
         self.header = "🍪 LitDataBatch"
         self.X = f"- X: {list(batch.X.shape)}"
         self.W = f"- W: {list(batch.W.shape)}"
-        self.W_hat = f"W_hat: {list(batch.W_hat.shape)}"
+        self.W_hat = f"- W_hat: {list(batch.W_hat.shape)}"
+        if not isinstance(batch.F_idx, NoneType):
+            self.F_idx = f"- F_idx: {list(batch.F_idx.shape)}"
+        else:
+            self.F_idx = ""
 
     def __call__(self):
-        return "\n".join([self.header, self.X, self.W])
+        return "\n".join([self.header, self.X, self.W, self.W_hat, self.F_idx])
     
 
 class BatchProcessor(ABCParse.ABCParse):
     """
     Batch Items:
     ------------
-    1. t - time. always required
-    2. X - data. tensor of size: [batch_size, len(t), n_dim]. always required.
-    3. W - weight. tensor of size: [batch_size, len(t), 1]
+    0. t - time. always required
+    1. X - data. tensor of size: [batch_size, len(t), n_dim]. always required.
+    2. W - weight. tensor of size: [batch_size, len(t), 1]
+    3. F_idx - fate_idx. tensor of size: [batch_Size, len(t), 1]
     """
     def __init__(self, batch: List[torch.Tensor], batch_idx: int)->None:
         
         self.__parse__(locals(), private=['batch'])
         
     @property
     def device(self):
@@ -59,10 +66,23 @@
             return utils.sum_normalize(W, sample_axis=1).contiguous()
         return utils.sum_normalize(torch.ones([len(self.t), self.batch_size, 1], device=self.device)).contiguous()
         
     @property
     def W(self)->torch.Tensor:
         return utils.sum_normalize(torch.ones_like(self.W_hat)).contiguous()
     
-        
+    @property
+    def F_idx(self):
+        if self.n_batch_items >= 4:
+            return (
+                self._batch[3]
+                .transpose(1, 0)[0]
+                .detach()
+                .cpu()
+                .numpy()
+                .flatten()
+                .astype(int)
+                .astype(str)
+            )
+
     def __repr__(self)->str:
         return BatchRepr(self)()
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_lightning_vae_sde.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 
 # -- import packages: ----------------------------------------------------------
+from neural_diffeqs import LatentPotentialODE
+import torch_nets
 import torch
 
 
 # -- import local dependencies: ------------------------------------------------
-from .base_models import BaseLightningSDE
-from .mix_ins import VAEPreTrainMixIn, VAEMixIn
-from ._sinkhorn_divergence import SinkhornDivergence
-from ..utils import sum_normalize
+from . import mix_ins
+from . import base
 
 
-NoneType = type(None)
+from typing import Union, List
 
-
-class LightningVAESDE(VAEPreTrainMixIn, VAEMixIn, BaseLightningSDE):
+# -- lightning model: ----------------------------------------------------------
+class LightningODE_VAE_PriorPotential(
+    mix_ins.DriftPriorMixIn,
+    mix_ins.PotentialMixIn,
+    mix_ins.VAEMixIn,
+    mix_ins.PreTrainMixIn,
+    base.BaseLightningDiffEq,
+):
     def __init__(
         self,
-        func,
-        pretrain_epochs=20,
-        dt=0.1,
-        pretrain_lr=1e-2,
+        data_dim,
+        latent_dim,
         train_lr=1e-5,
+        pretrain_lr=1e-3,
+        pretrain_epochs=100,
+        pretrain_optimizer=torch.optim.Adam,
+        train_optimizer=torch.optim.RMSprop,
+        pretrain_scheduler=torch.optim.lr_scheduler.StepLR,
+        train_scheduler=torch.optim.lr_scheduler.StepLR,
         pretrain_step_size=200,
-        train_step_size=50,
-        optimizers=[torch.optim.RMSprop, torch.optim.RMSprop],
-        lr_schedulers=[
-            torch.optim.lr_scheduler.StepLR,
-            torch.optim.lr_scheduler.StepLR,
-        ],
+        train_step_size=10,
+        dt=0.1,
+        adjoint=False,
+        
+        # -- encoder parameters: -------
+        encoder_n_hidden: int = 4,
+        encoder_power: float = 2,
+        encoder_activation: Union[str, List[str]] = 'LeakyReLU',
+        encoder_dropout: Union[float, List[float]] = 0.2,
+        encoder_bias: bool = True,
+        encoder_output_bias: bool = True,
+
+        # -- decoder parameters: -------
+        decoder_n_hidden: int = 4,
+        decoder_power: float = 2,
+        decoder_activation: Union[str, List[str]] = 'LeakyReLU',
+        decoder_dropout: Union[float, List[float]] = 0.2,
+        decoder_bias: bool = True,
+        decoder_output_bias: bool = True,
+        
+        *args,
+        **kwargs,
     ):
-        super(LightningVAESDE, self).__init__()
-
-        self.__parse__(kwargs=locals())
-
-        self.func = func
+        super().__init__()
 
-        self.SinkhornLoss = SinkhornDivergence(backend="auto")
-        self.MSELoss = torch.nn.MSELoss(reduction="sum")
+        self.save_hyperparameters()
+        
+        # -- torch modules: ----------------------------------------------------
+        self._configure_torch_modules(func = LatentPotentialODE, kwargs=locals())
+        self._configure_optimizers_schedulers()
+
+    def log_computed_loss(self, sinkhorn_loss, t, kl_div_loss, stage):
+        
+        sinkhorn_loss = self.log_sinkhorn_divergence(sinkhorn_loss).sum()
+        self.log(f"kl_div_{stage}", kl_div_loss.sum())
+
+        return sinkhorn_loss + kl_div_loss.sum()
+
+    def step(self, batch, batch_idx, stage=None):
+
+        batch = self.process_batch(batch, batch_idx)
+        X_hat, kl_div_loss = self.forward(batch.X0, batch.t)
+        sinkhorn_loss = self.compute_sinkhorn_divergence(
+            batch.X, X_hat, batch.W, batch.W_hat
+        )
+        return self.log_computed_loss(
+            sinkhorn_loss, t=batch.t, kl_div_loss=kl_div_loss, stage=stage
+        )
+
+    def pretrain_step(self, batch, batch_idx, stage=None):
+
+        batch = self.process_batch(batch, batch_idx)
+        X0_hat = self.Decoder(self.Encoder(batch.X0))
+        recon_loss = self.reconstruction_loss(X0_hat, batch.X0).sum()
+        self.log("pretrain_rl_mse", recon_loss.item())
+        return recon_loss
 
-        VAE_params = list(self.Encoder.parameters()) + list(self.Decoder.parameters())
-        self.optimizers = [
-            optimizers[0](VAE_params, lr=pretrain_lr),
-            optimizers[1](self.parameters(), lr=train_lr),
-        ]
-        self.lr_schedulers = [
-            lr_schedulers[0](self.optimizers[0], step_size=pretrain_step_size),
-            lr_schedulers[1](self.optimizers[1], step_size=train_step_size),
-        ]
-        self.hparams["func_type"] = "NeuralSDE"
-        self.hparams["func_description"] = str(self.func)
-        self.save_hyperparameters(ignore=["func", "optimizer", "lr_scheduler"])
-
-    def process_batch(self, batch):
-        """called in step"""
-
-        t = batch[0].unique()
-        X = batch[1].transpose(1, 0)
-        X0 = X[0]
-
-        return X, X0, t
-
-    def loss(self, X, X_hat):
-        return self.SinkhornLoss(X.contiguous(), X_hat.contiguous())
-
-    def record_loss(self, loss, stage):
-        """Record loss. called in step"""
-
-        log_msg = "{}"
-        if not isinstance(stage, NoneType):
-            log_msg = f"{stage}_" + "{}"
-        for i, l in enumerate(loss):
-            self.log(log_msg.format(i), l.item())
-
-    def step(self, batch, batch_idx, stage):
-
-        X, X0, t = self.process_batch(batch)
-        X_hat = self.forward(X0, t)
-        loss = self.loss(X, X_hat)
-        self.record_loss(loss, stage)
-        return loss.sum()
-
-    def training_step(self, batch, batch_idx, optimizer_idx):
-
-        if self.pretrain_criteria(optimizer_idx):
-            return self.pretrain_step(batch, batch_idx, stage="pretraining_train")
-        elif self.train_criteria(optimizer_idx):
-            return self.step(batch, batch_idx, stage="training")
-
-    def validation_step(self, batch, batch_idx, optimizer_idx):
-
-        if self.pretrain_criteria(optimizer_idx):
-            return self.pretrain_step(batch, batch_idx, stage="pretraining_validation")
-        elif self.train_criteria(optimizer_idx):
-            return self.step(batch, batch_idx, stage="validation")
+    def __repr__(self):
+        return "LightningODE-VAE-PriorPotential"
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/_lightning_models/_sinkhorn_divergence.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/_sinkhorn_divergence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # -- import packages: ----------------------------------------------------------
 from geomloss import SamplesLoss
 from autodevice import AutoDevice
 
 
 # -- import local dependencies: ------------------------------------------------
-from ..utils import AutoParseBase
+from ...utils import AutoParseBase
 
 
 # -- API-facing class: ---------------------------------------------------------
 class SinkhornDivergence(SamplesLoss, AutoParseBase):
     def __init__(
         self,
         device=AutoDevice(),
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/__init__.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 )
 
 
 # -- import: -----------------------------------------------------------------------------
 from ._loss_accounting import LossAccounting
 from ._intermittent_saves import IntermittentSaves
 from ._gradient_potential_callback import GradientPotentialTest
-from ._testing import Testing
+from ._testing import Testing
+
+from ._visualize_tracked_loss import VisualizeTrackedLoss
+from ._visualize_predictions import VisualizePredictions
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_intermittent_saves.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_intermittent_saves.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_loss_accounting.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_loss_accounting.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/callbacks/_testing.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/callbacks/_testing.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_function_credentialling.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/configs/_function_credentialling.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_model_configuration.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_model_configuration_v2.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_model_configuration_v2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import ABCParse
+import os
 
 from .. import lightning_models, utils
 
+NoneType = type(None)
+
 # -- import packages: ----------------------------------------------------------
 class LightningModelConfiguration(ABCParse.ABCParse):
     _potential_types = {
         "fixed": "FixedPotential",
         "prior": "PriorPotential",
     }
 
     def __init__(
         self,
         data_dim,
         latent_dim: int = 20,
         DiffEq_type: str = "SDE",
         potential_type="prior",
+        fate_bias_csv_path = None,
     ):
 
         self.__parse__(locals(), public=[None])
 
     @property
     def available_lightning_models(self):
         return [
@@ -35,25 +39,38 @@
     def use_vae(self):
         return self._data_dim > self._latent_dim
 
     @property
     def potential_type(self):
         if self._potential_type:
             return self._potential_types[self._potential_type]
+        
+    @property
+    def fate_bias_aware(self):
+        if isinstance(self._fate_bias_csv_path, NoneType):
+            return False
+        else:
+            if os.path.exists(self._fate_bias_csv_path):
+                return True
+            else:
+                raise ValueError("Path to fate_bias.csv was passed though not found.")
 
     def __call__(self, kwargs):
 
         _model = [self.DiffEq_type]
 
         if self.use_vae:
             _model.append("VAE")
 
         if self.potential_type:
             _model.append(self.potential_type)
+            
+        if self.fate_bias_aware:
+            _model.append("FateBiasAware")
 
         _model = "_".join(_model)
 
         if _model in self.available_lightning_models:
             lit_model = getattr(lightning_models, _model)
             model_kwargs = utils.function_kwargs(func=lit_model.__init__, kwargs=kwargs)
-            # data_dim=self._data_dim, latent_dim=self._latent_dim, 
             return lit_model(data_dim = self._data_dim, **model_kwargs)
+        raise ValueError(f"Configuration tried: {_model} - this does not exist as an available model.")
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_lightning_trainer_configuration.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/configs/_lightning_trainer_configuration.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,44 +20,63 @@
 
 # -- define typing: ------------------------------------------------------------
 from typing import Union, Dict, List
 NoneType = type(None)
 
 
 # -- Main class: ---------------------------------------------------------------
-class LightningTrainerConfiguration(utils.AutoParseBase):
+class LightningTrainerConfiguration(utils.ABCParse):
     def __init__(
         self,
         save_dir: str = "scDiffEq_Model",
     ):
+        super().__init__()
+        
         self.__parse__(locals())
         if not os.path.exists(save_dir):
             os.mkdir(save_dir)
 
     # -- kwargs: ---------------------------------------------------------------
     @property
     def _CSVLogger_kwargs(self):
-        return utils.extract_func_kwargs(func=loggers.CSVLogger, kwargs=self._KWARGS)
+        return utils.extract_func_kwargs(func=loggers.CSVLogger, kwargs=self._PARAMS, ignore=['version'])
 
     @property
     def _Trainer_kwargs(self):
-        return utils.extract_func_kwargs(func=Trainer, kwargs=self._KWARGS)
+        return utils.extract_func_kwargs(func=Trainer, kwargs=self._PARAMS, ignore=["accelerator", "callbacks"])
 
     @property
     def Callbacks(self):
         callback_config = LightningCallbacksConfiguration()
+        
         return callback_config(
+            version = self.version,
+            model_name=self.model_name,
+            working_dir=self.working_dir,
+            train_version=self.train_version,
+            pretrain_version=self.pretrain_version,
             callbacks=self._callbacks,
             ckpt_frequency=self.ckpt_frequency,
             keep_ckpts=self.keep_ckpts,
+            monitor=self.monitor,
             retain_test_gradients=self.retain_test_gradients,
-            monitor = self.monitor,
-#             swa_lrs = self.swa_lrs,
-            save_last = self.save_last_ckpt,
+            save_last=self.save_last_ckpt,
+            # swa_lrs=1e-5,
         )
+
+#         return callback_config(
+#             callbacks=self._callbacks,
+#             ckpt_frequency=self.ckpt_frequency,
+#             keep_ckpts=self.keep_ckpts,
+#             retain_test_gradients=self.retain_test_gradients,
+#             monitor = self.monitor,
+# #             swa_lrs = self.swa_lrs,
+#             save_last = self.save_last_ckpt,
+#             version = self.version,
+#         )
     
     @property
     def accelerator(self):
         if not isinstance(self._accelerator, NoneType):
             return self._accelerator
         if torch.cuda.is_available():
             return "gpu"
@@ -71,14 +90,15 @@
     # -- trainers: -------------------------------------------------------------
     @property
     def Trainer(self):
         """
         Main Lightning Trainer used for fitting / testing.
         If pre-train routine was used, Trainer loads from ckpt path.
         """
+
         return Trainer(
             accelerator=self.accelerator,
             logger=loggers.CSVLogger(**self._CSVLogger_kwargs),
             callbacks=self.Callbacks,
             **self._Trainer_kwargs,
         )
 
@@ -99,29 +119,38 @@
             enable_progress_bar=False,
             **self._Trainer_kwargs,
         )
 
     def __call__(
         self,
         lr: float = None,
+        model_name="scDiffEq_model",
+        working_dir=os.getcwd(),
+        train_version=0,
+        pretrain_version=0,
         stage=None,
         max_epochs=500,
         monitor=None,
         accelerator=None,
         devices=None,
         prefix: str = "",
         log_every_n_steps=1,
         flush_logs_every_n_steps: int = 1,
         ckpt_frequency: int = 25,
         save_last_ckpt: bool = True,
         keep_ckpts: int = -1,
         version: Union[int, str, NoneType] = None,
         callbacks: list = [],
         potential_model: bool = False,
+        check_val_every_n_epoch = 1,
+        limit_val_batches = None,
+        num_sanity_val_steps = None,
+        val_check_interval = None,
 #         swa_lrs: float = None,
+        reload_dataloaders_every_n_epochs = 1,
         **kwargs
     ):
         
         """
         Return trainer upon call.
         
         Parameters:
@@ -181,16 +210,17 @@
 #         if isinstance(swa_lrs, NoneType):
 #             swa_lrs = lr
             
         if torch.cuda.device_count() > 0:
             devices = torch.cuda.device_count()
 
         self.__parse__(locals(), private=['accelerator', 'callbacks'])
-        self._KWARGS["name"] = "{}_logs".format(stage)
-        log_save_dir = os.path.join(self.save_dir, self._KWARGS["name"])
+        
+        self._PARAMS["name"] = "{}_logs".format(stage)
+        log_save_dir = os.path.join(self.save_dir, self._PARAMS["name"])
         if not os.path.exists(log_save_dir):
             os.mkdir(log_save_dir)
 
         if (potential_model) and (stage in ["test", "predict"]):
             self.retain_test_gradients = True
             return self.GradientsRetainedTestTrainer
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/configs/_time_configuration.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/configs/_time_configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,198 +1,360 @@
 
 # -- import packages: --------------------------------------------------------------------
-from anndata import AnnData
+import anndata
 import pandas as pd
+import numpy as np
 import torch
 
 
 # -- import local dependencies: ----------------------------------------------------------
 from .. import utils
-from ...tools import time_free_sampling
+from ... import tools
 
 
 # -- define types: -----------------------------------------------------------------------
 NoneType = type(None)
 
 
-# -- main class: -------------------------------------------------------------------------
-class TimeConfiguration(utils.AutoParseBase):
+class TimeConfiguration(utils.ABCParse):
     def __init__(
         self,
-        adata: AnnData,
+        adata: anndata.AnnData,
         time_key: str = None,
-        t0_idx: pd.Index = None,
-        t: torch.Tensor = None,
-        dt: float = None,
-        n_steps: int = 40,
-        t_min: float = 0,
-        t_max: float = 1,
+        t_min=0,
+        t_max=1,
+        dt=0.1,
+        t0_idx=None,
+        t0_cluster=None,
+        time_cluster_key=None,
     ):
-        """
-        Must provide t0_idx or time_key. if both are provided,
-        time_key overrules t0_idx.
-        """
-        self._check_passed_time_args(t0_idx, time_key)
-        self.__parse__(locals(), public=[None])
-
-    # -- utility funcs: ------------------------------------------------------------------
-    def _check_passed_time_args(self, t0_idx, time_key):
-        """If time_key is passed"""
-        if utils.not_none(t0_idx):
-            time_key = None
-        elif sum([utils.not_none(time_key), utils.not_none(t0_idx)]) < 1:
-            "Must provide t0_idx or time_key. If both are provided, t0_idx overrules time_key"
-            
-    
-#     def _value_pass_check(self, time_key, t0_idx):
-#         assert any(
-#             [not isinstance(time_key, NoneType), not isinstance(t0_idx, NoneType)]
-#         ), "Must provide t0_idx or time_key. If both are provided, time_key overrules t0_idx"
-
-    def _time_from_adata(self):
-        return torch.Tensor(sorted(self._adata.obs[self.time_key].unique()))
-
-    # -- time_key: -----------------------------------------------------------------------
-    def _configure_time_key(self):
-        if isinstance(self._time_key, NoneType):
-            try:
-
-                time_free_sampling(
-                    self._adata,
-                    self.t0_idx,
-                    n_steps=self.n_steps,
-                    t0_key="t0",
-                    t_key="t",
-                )
-                utils.normalize_time(
-                    self._adata,
-                    time_key="t",
-                    t_min=self._t_min,
-                    t_max=self._t_max,
-                )
-                self._time_key = "t"
-
-            except:
-                raise ValueError("Pass `t0_idx` or `time_key`")
+        super().__init__()
+        self.__parse__(kwargs=locals(), public=["adata"])
+        
+## WE DONT NEED THIS B/C WE CAN GENERATE T0_IDX FROM OTHER KEY:VAL PAIRS
+#         self._check_passed_time_args(self._t0_idx, self._time_key)
+        
+#     def _check_passed_time_args(self, t0_idx, time_key):
+#         """If time_key is passed"""
+        
+#         if sum([utils.not_none(time_key), utils.not_none(t0_idx)]) < 1:
+#             raise ValueError("Must provide `t0_idx` and/or `time_key`.")
 
     @property
-    def time_key(self):
-        self._configure_time_key()
-        return self._time_key
+    def t0_idx(self):
 
-    # -- t: ------------------------------------------------------------------------------
-    def _configure_t(self):
         """
-        we are here because we don't have t
-        we can use 0-1 in place of a real time and throw in n_steps
+        If t0_idx is provided, returns that.
+        If t0_idx is not provided, but a cluster key and t0 cluster
+        value-pair is provided, this can isolate the t0_idx.
         """
 
-        if isinstance(self._t, NoneType):
-            self._t = self._time_from_adata()
+        if self.has_time_key:
+            
+            return self.adata.obs[
+                self.adata.obs[self._time_key] == self.adata.obs[self._time_key].min()
+            ].index
+
+        if not isinstance(self._t0_idx, NoneType):
+            return self._t0_idx
+
+        if (not isinstance(self._time_cluster_key, NoneType)) and (
+            not isinstance(self._t0_cluster, NoneType)
+        ):
+            return self.adata.obs[
+                self.adata.obs[self._time_cluster_key] == self._t0_cluster
+            ].index
+
+    def time_sampling(self):
+        if not self.has_time_key:
+            self.adata.obs["t0"] = self.adata.obs.index.isin(self.t0_idx)
+#         else:
+        tools.time_free_sampling(
+            adata=self.adata,
+            t0_idx=self.t0_idx,
+            n_steps=self.n_steps,
+            t0_key="t0",
+            t_key="t",
+        )
 
     @property
-    def t(self):
-        self._configure_t()
-        return self._t
-
-    # -- t0_idx: -------------------------------------------------------------------------
-    def _configure_t0_idx(self):
-        if isinstance(self._t0_idx, NoneType):
-            raise ValueError("Must provide t0_idx")
+    def has_time_key(self):
+        return (not isinstance(self._time_key, NoneType)) and (
+            self._time_key in self.adata.obs_keys()
+        )
 
     @property
-    def t0_idx(self):
-        self._configure_t0_idx()
-        return self._t0_idx
-
-    # -- t_min: --------------------------------------------------------------------------
-    def _configure_t_min(self):
-        if not isinstance(self.t, NoneType):
-            self._t_min = min(self.t).item()
+    def time_key(self):
+        if self.has_time_key:
+            return self._time_key
+        return "t"
 
     @property
-    def t_min(self) -> float:
-        self._configure_t_min()
+    def t_min(self):
+        if self.has_time_key:
+            self._t_min = self.adata.obs[self._time_key].min()
         return self._t_min
 
-    # -- t_max: --------------------------------------------------------------------------
-    def _configure_t_max(self):
-        if not isinstance(self.t, NoneType):
-            self._t_max = max(self.t).item()
-
     @property
-    def t_max(self) -> float:
-        self._configure_t_max()
+    def t_max(self):
+        if self.has_time_key:
+            self._t_max = self.adata.obs[self._time_key].max()
         return self._t_max
 
-    # -- t_span: -------------------------------------------------------------------------
-    def _configure_t_span(self):
-        if not hasattr(self, "_t_span"):
-            self._t_span = abs(self.t_max - self.t_min)
-
     @property
-    def t_span(self):
-        self._configure_t_span()
-        return self._t_span
+    def t_diff(self):
+        return self._t_max - self._t_min
 
-    # -- dt: -----------------------------------------------------------------------------
-    def _configure_dt(self):
-        """
-        we are here because we don't have dt.
-        to get dt, de novo, we need t and n_steps.
-        """
-        if isinstance(self._dt, NoneType):
-            self._dt = self.t_span / self._n_steps
-
-    @property
-    def dt(self):
-        self._configure_dt()
-        return self._dt
+    def _IS_CONTIGUOUS(self, n_steps):
+        return n_steps % 1 == 0
 
-    # -- n_steps: ------------------------------------------------------------------------
     @property
     def n_steps(self):
-        return int(self._n_steps + 1)
+        _n_steps = self.t_diff / self._dt + 1
+        if self._IS_CONTIGUOUS(_n_steps):
+            return int(_n_steps)
+        raise ValueError("Time is non-contiguous")
 
-    # -- collect attributes: -------------------------------------------------------------
+    @property
+    def dt(self):
+        return self._dt
 
-    def __attributes__(self):
+    def _t_from_time_key(self):
+        return torch.Tensor(sorted(self.adata.obs[self._time_key].unique()))
 
-        self._attrs = {}
+    def _t_from_bounds(self):
+        return torch.linspace(self._t_min, self._t_max, self.n_steps)
 
-        for attr in self.__dir__():
-            if (not attr == "attributes") and (not attr.startswith("_")):
-                if attr == "t0_idx":
-                    if self._t0_idx is None:
-                        continue
-                self._attrs[attr] = getattr(self, attr)
+    def __call__(self):
 
-        return self._attrs
+        if self.has_time_key:
+            return self._t_from_time_key()
+        self.time_sampling()
+        return self._t_from_bounds()
 
     @property
     def attributes(self):
-        return self.__attributes__()
-    
+        self._ATTR_KEYS = sorted(
+            ["time_key", "t0_idx", "t_min", "t_max", "t_diff", "dt", "n_steps"]
+        )
+        return {attr: getattr(self, attr) for attr in self._ATTR_KEYS}
+
+    def __repr__(self):
+
+        header = "Time Attributes:\n\n  "
+
+        _attrs = [
+            "{:<9} :  {}".format(attr, val) for attr, val in self.attributes.items()
+        ]
+        return header + "\n  ".join(_attrs)
+
+
 def configure_time(
-    adata: AnnData,
+    adata: anndata.AnnData,
     time_key: str = None,
-    t0_idx: pd.Index = None,
-    t: torch.Tensor = None,
-    dt: float = None,
-    n_steps: int = 40,
     t_min: float = 0,
     t_max: float = 1,
+    t0_idx: pd.Index = None,
+    dt: float = 0.1,
+    t0_cluster=None,
+    time_cluster_key=None,
 ) -> dict:
 
     """Updates time for AnnData. Returns time_attributes dictionary."""
 
     time_config = TimeConfiguration(
         adata=adata,
         time_key=time_key,
-        t0_idx=t0_idx,
-        t=t,
-        dt=dt,
-        n_steps=n_steps,
         t_min=t_min,
         t_max=t_max,
+        t0_idx=t0_idx,
+        dt=dt,
+        t0_cluster=t0_cluster,
+        time_cluster_key=time_cluster_key,
     )
-    return time_config.attributes
+    
+    t = time_config()
+    
+    return t, time_config
+
+# # -- main class: -------------------------------------------------------------------------
+# class TimeConfiguration(utils.AutoParseBase):
+#     def __init__(
+#         self,
+#         adata: AnnData,
+#         time_key: str = None,
+#         t0_idx: pd.Index = None,
+#         t: torch.Tensor = None,
+#         dt: float = None,
+#         n_steps: int = 40,
+#         t_min: float = 0,
+#         t_max: float = 1,
+#     ):
+#         """
+#         Must provide t0_idx or time_key. if both are provided,
+#         time_key overrules t0_idx.
+#         """
+#         self._check_passed_time_args(t0_idx, time_key)
+#         self.__parse__(locals(), public=[None])
+
+#     # -- utility funcs: ------------------------------------------------------------------
+#     def _check_passed_time_args(self, t0_idx, time_key):
+#         """If time_key is passed"""
+#         if utils.not_none(t0_idx):
+#             time_key = None
+#         elif sum([utils.not_none(time_key), utils.not_none(t0_idx)]) < 1:
+#             "Must provide t0_idx and/or time_key. If both are provided, t0_idx overrules time_key"
+            
+    
+# #     def _value_pass_check(self, time_key, t0_idx):
+# #         assert any(
+# #             [not isinstance(time_key, NoneType), not isinstance(t0_idx, NoneType)]
+# #         ), "Must provide t0_idx or time_key. If both are provided, time_key overrules t0_idx"
+
+#     def _time_from_adata(self):
+#         return torch.Tensor(sorted(self._adata.obs[self.time_key].unique()))
+
+#     # -- time_key: -----------------------------------------------------------------------
+#     def _configure_time_key(self):
+#         if isinstance(self._time_key, NoneType):
+#             try:
+
+#                 time_free_sampling(
+#                     self._adata,
+#                     self.t0_idx,
+#                     n_steps=self.n_steps,
+#                     t0_key="t0",
+#                     t_key="t",
+#                 )
+#                 utils.normalize_time(
+#                     self._adata,
+#                     time_key="t",
+#                     t_min=self._t_min,
+#                     t_max=self._t_max,
+#                 )
+#                 self._time_key = "t"
+
+#             except:
+#                 raise ValueError("Pass `t0_idx` or `time_key`")
+
+#     @property
+#     def time_key(self):
+#         self._configure_time_key()
+#         return self._time_key
+
+#     # -- t: ------------------------------------------------------------------------------
+#     def _configure_t(self):
+#         """
+#         we are here because we don't have t
+#         we can use 0-1 in place of a real time and throw in n_steps
+#         """
+
+#         if isinstance(self._t, NoneType):
+#             self._t = self._time_from_adata()
+
+#     @property
+#     def t(self):
+#         self._configure_t()
+#         return self._t
+
+#     # -- t0_idx: -------------------------------------------------------------------------
+#     def _configure_t0_idx(self):
+#         if isinstance(self._t0_idx, NoneType):
+#             raise ValueError("Must provide t0_idx")
+
+#     @property
+#     def t0_idx(self):
+#         self._configure_t0_idx()
+#         return self._t0_idx
+
+#     # -- t_min: --------------------------------------------------------------------------
+#     def _configure_t_min(self):
+#         if not isinstance(self.t, NoneType):
+#             self._t_min = min(self.t).item()
+
+#     @property
+#     def t_min(self) -> float:
+#         self._configure_t_min()
+#         return self._t_min
+
+#     # -- t_max: --------------------------------------------------------------------------
+#     def _configure_t_max(self):
+#         if not isinstance(self.t, NoneType):
+#             self._t_max = max(self.t).item()
+
+#     @property
+#     def t_max(self) -> float:
+#         self._configure_t_max()
+#         return self._t_max
+
+#     # -- t_span: -------------------------------------------------------------------------
+#     def _configure_t_span(self):
+#         if not hasattr(self, "_t_span"):
+#             self._t_span = abs(self.t_max - self.t_min)
+
+#     @property
+#     def t_span(self):
+#         self._configure_t_span()
+#         return self._t_span
+
+#     # -- dt: -----------------------------------------------------------------------------
+#     def _configure_dt(self):
+#         """
+#         we are here because we don't have dt.
+#         to get dt, de novo, we need t and n_steps.
+#         """
+#         if isinstance(self._dt, NoneType):
+#             self._dt = self.t_span / self._n_steps
+
+#     @property
+#     def dt(self):
+#         self._configure_dt()
+#         return self._dt
+
+#     # -- n_steps: ------------------------------------------------------------------------
+#     @property
+#     def n_steps(self):
+#         return int(self._n_steps + 1)
+
+#     # -- collect attributes: -------------------------------------------------------------
+
+#     def __attributes__(self):
+
+#         self._attrs = {}
+
+#         for attr in self.__dir__():
+#             if (not attr == "attributes") and (not attr.startswith("_")):
+#                 if attr == "t0_idx":
+#                     if self._t0_idx is None:
+#                         continue
+#                 self._attrs[attr] = getattr(self, attr)
+
+#         return self._attrs
+
+#     @property
+#     def attributes(self):
+#         return self.__attributes__()
+    
+# def configure_time(
+#     adata: AnnData,
+#     time_key: str = None,
+#     t0_idx: pd.Index = None,
+#     t: torch.Tensor = None,
+#     dt: float = None,
+#     n_steps: int = 40,
+#     t_min: float = 0,
+#     t_max: float = 1,
+# ) -> dict:
+
+#     """Updates time for AnnData. Returns time_attributes dictionary."""
+
+#     time_config = TimeConfiguration(
+#         adata=adata,
+#         time_key=time_key,
+#         t0_idx=t0_idx,
+#         t=t,
+#         dt=dt,
+#         n_steps=n_steps,
+#         t_min=t_min,
+#         t_max=t_max,
+#     )
+#     return time_config.attributes
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/__init__.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,7 +18,10 @@
 from ._lightning_sde_vae_fixed_potential import LightningSDE_VAE_FixedPotential
 
 
 from ._lightning_ode_prior_potential import LightningODE_PriorPotential
 from ._lightning_sde_prior_potential import LightningSDE_PriorPotential
 from ._lightning_ode_vae_prior_potential import LightningODE_VAE_PriorPotential
 from ._lightning_sde_vae_prior_potential import LightningSDE_VAE_PriorPotential
+
+from ._lightning_sde_fate_bias_aware import LightningSDE_FateBiasAware
+from ._lightning_sde_vae_fate_bias_aware import LightningSDE_VAE_FateBiasAware
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_vae.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_ode_vae_fixed_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_ode_vae_prior_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,66 @@
 
-# -- import packages: ----------------------------------------------------------
-from neural_diffeqs import LatentPotentialODE
-import torch_nets
+from neural_diffeqs import LatentPotentialSDE
 import torch
 
+from . import base, mix_ins
 
-# -- import local dependencies: ------------------------------------------------
-from . import mix_ins
-from . import base
-
+from .. import utils
 
 from typing import Union, List
 
-# -- lightning model: ----------------------------------------------------------
-class LightningODE_VAE_PriorPotential(
-    mix_ins.DriftPriorMixIn,
-    mix_ins.PotentialMixIn,
-    mix_ins.VAEMixIn,
-    mix_ins.PreTrainMixIn,
+class LightningSDE_PriorPotential(
     base.BaseLightningDiffEq,
+    mix_ins.PotentialMixIn,
 ):
     def __init__(
         self,
-        data_dim,
         latent_dim,
-        train_lr=1e-5,
-        pretrain_lr=1e-3,
-        pretrain_epochs=100,
-        pretrain_optimizer=torch.optim.Adam,
+        train_lr=1e-4,
         train_optimizer=torch.optim.RMSprop,
-        pretrain_scheduler=torch.optim.lr_scheduler.StepLR,
         train_scheduler=torch.optim.lr_scheduler.StepLR,
-        pretrain_step_size=200,
         train_step_size=10,
         dt=0.1,
         adjoint=False,
-        
-        # -- encoder parameters: -------
-        encoder_n_hidden: int = 4,
-        encoder_power: float = 2,
-        encoder_activation: Union[str, List[str]] = 'LeakyReLU',
-        encoder_dropout: Union[float, List[float]] = 0.2,
-        encoder_bias: bool = True,
-        encoder_output_bias: bool = True,
-
-        # -- decoder parameters: -------
-        decoder_n_hidden: int = 4,
-        decoder_power: float = 2,
-        decoder_activation: Union[str, List[str]] = 'LeakyReLU',
-        decoder_dropout: Union[float, List[float]] = 0.2,
-        decoder_bias: bool = True,
-        decoder_output_bias: bool = True,
-        
+        mu_hidden: Union[List[int], int] = [400, 400, 400],
+        sigma_hidden: Union[List[int], int] = [400, 400, 400],
+        mu_activation: Union[str, List[str]] = 'LeakyReLU',
+        sigma_activation: Union[str, List[str]] = 'LeakyReLU',
+        mu_dropout: Union[float, List[float]] = 0.2,
+        sigma_dropout: Union[float, List[float]] = 0.2,
+        mu_bias: bool = True,
+        sigma_bias: List[bool] = True,
+        mu_output_bias: bool = True,
+        sigma_output_bias: bool = True,
+        mu_n_augment: int = 0,
+        sigma_n_augment: int = 0,
+        sde_type='ito',
+        noise_type='general',
+        brownian_dim=1,
+        coef_drift: float = 1.0,
+        coef_diffusion: float = 1.0,
+        coef_prior_drift: float = 1.0,
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
         
         # -- torch modules: ----------------------------------------------------
-        self._configure_torch_modules(func = LatentPotentialODE, kwargs=locals())
+        self._configure_torch_modules(func=LatentPotentialSDE, kwargs=locals())
         self._configure_optimizers_schedulers()
 
+    def forward(self, X0, t, **kwargs):
+        """Forward step: (0) integrate in latent space"""
+        Z_hat, KL_div = self.integrate(
+            Z0=X0, t=t, dt=self.hparams["dt"], logqp=True, **kwargs
+        )
+        return Z_hat, KL_div
+
     def log_computed_loss(self, sinkhorn_loss, t, kl_div_loss, stage):
         
         sinkhorn_loss = self.log_sinkhorn_divergence(sinkhorn_loss).sum()
         self.log(f"kl_div_{stage}", kl_div_loss.sum())
 
         return sinkhorn_loss + kl_div_loss.sum()
 
@@ -77,17 +71,10 @@
         sinkhorn_loss = self.compute_sinkhorn_divergence(
             batch.X, X_hat, batch.W, batch.W_hat
         )
         return self.log_computed_loss(
             sinkhorn_loss, t=batch.t, kl_div_loss=kl_div_loss, stage=stage
         )
 
-    def pretrain_step(self, batch, batch_idx, stage=None):
-
-        batch = self.process_batch(batch, batch_idx)
-        X0_hat = self.Decoder(self.Encoder(batch.X0))
-        recon_loss = self.reconstruction_loss(X0_hat, batch.X0).sum()
-        self.log("pretrain_rl_mse", recon_loss.item())
-        return recon_loss
-
+        
     def __repr__(self):
-        return "LightningODE-VAE-PriorPotential"
+        return "LightningSDE-PriorPotential"
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_fixed_potential.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from neural_diffeqs import PotentialSDE
 import torch
 
 
 from . import base, mix_ins
 from typing import Union, List
 
+
+# -- lightning model: -----------------------------------
 class LightningSDE_FixedPotential(
-    base.BaseLightningDiffEq,
     mix_ins.PotentialMixIn,
     mix_ins.BaseForwardMixIn,
+    base.BaseLightningDiffEq,
 ):
     def __init__(
         self,
         latent_dim,
         mu_hidden: Union[List[int], int] = [400, 400, 400],
         sigma_hidden: Union[List[int], int] = [400, 400, 400],
         mu_activation: Union[str, List[str]] = 'LeakyReLU',
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_prior_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,93 @@
 
-from neural_diffeqs import LatentPotentialSDE
-import torch
+from . import mix_ins, base
 
-from . import base, mix_ins
 
-from .. import utils
+from neural_diffeqs import PotentialSDE
+import torch_nets
+import torch
 
 from typing import Union, List
 
-class LightningSDE_PriorPotential(
-    base.BaseLightningDiffEq,
+class LightningSDE_VAE_FixedPotential(
+    mix_ins.PreTrainMixIn,
     mix_ins.PotentialMixIn,
+    mix_ins.VAEMixIn,
+    base.BaseLightningDiffEq,
 ):
     def __init__(
         self,
+        data_dim,
         latent_dim,
-        train_lr=1e-4,
-        train_optimizer=torch.optim.RMSprop,
-        train_scheduler=torch.optim.lr_scheduler.StepLR,
-        train_step_size=10,
-        dt=0.1,
-        adjoint=False,
-        mu_hidden: Union[List[int], int] = [400, 400, 400],
-        sigma_hidden: Union[List[int], int] = [400, 400, 400],
+        mu_hidden: Union[List[int], int] = [400, 400],
         mu_activation: Union[str, List[str]] = 'LeakyReLU',
-        sigma_activation: Union[str, List[str]] = 'LeakyReLU',
         mu_dropout: Union[float, List[float]] = 0.2,
-        sigma_dropout: Union[float, List[float]] = 0.2,
         mu_bias: bool = True,
-        sigma_bias: List[bool] = True,
         mu_output_bias: bool = True,
-        sigma_output_bias: bool = True,
         mu_n_augment: int = 0,
+        sigma_hidden: Union[List[int], int] = [400, 400],
+        sigma_activation: Union[str, List[str]] = 'LeakyReLU',
+        sigma_dropout: Union[float, List[float]] = 0.2,
+        sigma_bias: List[bool] = True,
+        sigma_output_bias: bool = True,
         sigma_n_augment: int = 0,
         sde_type='ito',
         noise_type='general',
         brownian_dim=1,
         coef_drift: float = 1.0,
         coef_diffusion: float = 1.0,
-        coef_prior_drift: float = 1.0,
+        
+        train_lr=1e-5,
+        train_optimizer=torch.optim.RMSprop,
+        train_scheduler=torch.optim.lr_scheduler.StepLR,
+        train_step_size=10,
+        
+        pretrain_lr=1e-3,
+        pretrain_epochs=100,
+        pretrain_optimizer=torch.optim.Adam,
+        pretrain_scheduler=torch.optim.lr_scheduler.StepLR,
+        pretrain_step_size=200,
+        
+        # -- encoder parameters: -------
+        encoder_n_hidden: int = 4,
+        encoder_power: float = 2,
+        encoder_activation: Union[str, List[str]] = 'LeakyReLU',
+        encoder_dropout: Union[float, List[float]] = 0.2,
+        encoder_bias: bool = True,
+        encoder_output_bias: bool = True,
+        
+        # -- decoder parameters: -------
+        decoder_n_hidden: int = 4,
+        decoder_power: float = 2,
+        decoder_activation: Union[str, List[str]] = 'LeakyReLU',
+        decoder_dropout: Union[float, List[float]] = 0.2,
+        decoder_bias: bool = True,
+        decoder_output_bias: bool = True,
+        
+        dt=0.1,
+        adjoint=False,
         *args,
         **kwargs,
     ):
         super().__init__()
 
         self.save_hyperparameters()
         
         # -- torch modules: ----------------------------------------------------
-        self._configure_torch_modules(func=LatentPotentialSDE, kwargs=locals())
+        self._configure_torch_modules(func = PotentialSDE, kwargs=locals())
         self._configure_optimizers_schedulers()
 
-    def forward(self, X0, t, **kwargs):
-        """Forward step: (0) integrate in latent space"""
-        Z_hat, KL_div = self.integrate(
-            Z0=X0, t=t, dt=self.hparams["dt"], logqp=True, **kwargs
-        )
-        return Z_hat, KL_div
-
-    def log_computed_loss(self, sinkhorn_loss, t, kl_div_loss, stage):
-        
-        sinkhorn_loss = self.log_sinkhorn_divergence(sinkhorn_loss).sum()
-        self.log(f"kl_div_{stage}", kl_div_loss.sum())
-
-        return sinkhorn_loss + kl_div_loss.sum()
-
-    def step(self, batch, batch_idx, stage=None):
+    def pretrain_step(self, batch, batch_idx, stage=None):
 
         batch = self.process_batch(batch, batch_idx)
-        X_hat, kl_div_loss = self.forward(batch.X0, batch.t)
-        sinkhorn_loss = self.compute_sinkhorn_divergence(
-            batch.X, X_hat, batch.W, batch.W_hat
-        )
-        return self.log_computed_loss(
-            sinkhorn_loss, t=batch.t, kl_div_loss=kl_div_loss, stage=stage
-        )
+        X0_hat = self.Decoder(self.Encoder(batch.X0))
+        recon_loss = self.reconstruction_loss(X0_hat, batch.X0).sum()
+        self.log("pretrain_rl_mse", recon_loss.item())
+        return recon_loss
+
+    def training_step(self, batch, batch_idx, *args, **kwargs):
+        if self.PRETRAIN:
+            return self.pretrain_step(batch, batch_idx, stage="pretrain")
+        return self.step(batch, batch_idx, stage="training")
 
-        
     def __repr__(self):
-        return "LightningSDE-PriorPotential"
+        return "LightningSDE-VAE-FixedPotential"
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from . import mix_ins, base
 
 from typing import Union, List
 
 # -- lightning model: ----------------------------------------------------------
 class LightningSDE_VAE(
     mix_ins.VAEMixIn, 
-    mix_ins.PreTrainMixIn, 
+    mix_ins.PreTrainMixIn,
     base.BaseLightningDiffEq,
 ):
     def __init__(
         self,
         data_dim,
         latent_dim,
         train_lr=1e-5,
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_fixed_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential_fate_bias_aware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 
-from . import mix_ins, base
-
-
-from neural_diffeqs import PotentialSDE
+# -- import packages: ----------------------------------------------------------
+from neural_diffeqs import LatentPotentialSDE
 import torch_nets
 import torch
 
+
+# -- import local dependencies: ------------------------------------------------
+from . import mix_ins
+from . import base
+from .. import utils
+
 from typing import Union, List
 
-class LightningSDE_VAE_FixedPotential(
-    mix_ins.PreTrainMixIn,
+
+# -- lightning model: ----------------------------------------------------------
+class LightningSDE_VAE_PriorPotential_FateBiasAware(
+    mix_ins.FateBiasVAEMixIn,
+    mix_ins.DriftPriorVAEMixIn,
     mix_ins.PotentialMixIn,
     mix_ins.VAEMixIn,
+    mix_ins.PreTrainMixIn,
     base.BaseLightningDiffEq,
 ):
     def __init__(
         self,
         data_dim,
         latent_dim,
-        mu_hidden: Union[List[int], int] = [400, 400],
+        train_lr=1e-5,
+        pretrain_lr=1e-3,
+        pretrain_epochs=100,
+        pretrain_optimizer=torch.optim.Adam,
+        train_optimizer=torch.optim.RMSprop,
+        pretrain_scheduler=torch.optim.lr_scheduler.StepLR,
+        train_scheduler=torch.optim.lr_scheduler.StepLR,
+        pretrain_step_size=200,
+        train_step_size=10,
+        dt=0.1,
+        adjoint=False,
+        
+        # -- sde params: -----
+        
+        mu_hidden: Union[List[int], int] = [400, 400, 400],
+        sigma_hidden: Union[List[int], int] = [400, 400, 400],
         mu_activation: Union[str, List[str]] = 'LeakyReLU',
-        mu_dropout: Union[float, List[float]] = 0.2,
-        mu_bias: bool = True,
-        mu_output_bias: bool = True,
-        mu_n_augment: int = 0,
-        sigma_hidden: Union[List[int], int] = [400, 400],
         sigma_activation: Union[str, List[str]] = 'LeakyReLU',
-        sigma_dropout: Union[float, List[float]] = 0.2,
+        mu_dropout: Union[float, List[float]] = 0.1,
+        sigma_dropout: Union[float, List[float]] = 0.1,
+        mu_bias: bool = True,
         sigma_bias: List[bool] = True,
+        mu_output_bias: bool = True,
         sigma_output_bias: bool = True,
+        mu_n_augment: int = 0,
         sigma_n_augment: int = 0,
         sde_type='ito',
         noise_type='general',
         brownian_dim=1,
         coef_drift: float = 1.0,
         coef_diffusion: float = 1.0,
-        
-        train_lr=1e-5,
-        train_optimizer=torch.optim.RMSprop,
-        train_scheduler=torch.optim.lr_scheduler.StepLR,
-        train_step_size=10,
-        
-        pretrain_lr=1e-3,
-        pretrain_epochs=100,
-        pretrain_optimizer=torch.optim.Adam,
-        pretrain_scheduler=torch.optim.lr_scheduler.StepLR,
-        pretrain_step_size=200,
+        coef_prior_drift: float = 1.0,
         
         # -- encoder parameters: -------
         encoder_n_hidden: int = 4,
         encoder_power: float = 2,
         encoder_activation: Union[str, List[str]] = 'LeakyReLU',
         encoder_dropout: Union[float, List[float]] = 0.2,
         encoder_bias: bool = True,
@@ -59,35 +71,30 @@
         decoder_n_hidden: int = 4,
         decoder_power: float = 2,
         decoder_activation: Union[str, List[str]] = 'LeakyReLU',
         decoder_dropout: Union[float, List[float]] = 0.2,
         decoder_bias: bool = True,
         decoder_output_bias: bool = True,
         
-        dt=0.1,
-        adjoint=False,
+        PCA = None,
+        
         *args,
         **kwargs,
     ):
         super().__init__()
-
+        
         self.save_hyperparameters()
         
         # -- torch modules: ----------------------------------------------------
-        self._configure_torch_modules(func = PotentialSDE, kwargs=locals())
+        self._configure_torch_modules(func = LatentPotentialSDE, kwargs=locals())
         self._configure_optimizers_schedulers()
-
-    def pretrain_step(self, batch, batch_idx, stage=None):
-
-        batch = self.process_batch(batch, batch_idx)
-        X0_hat = self.Decoder(self.Encoder(batch.X0))
-        recon_loss = self.reconstruction_loss(X0_hat, batch.X0).sum()
-        self.log("pretrain_rl_mse", recon_loss.item())
-        return recon_loss
-
-    def training_step(self, batch, batch_idx, *args, **kwargs):
-        if self.PRETRAIN:
-            return self.pretrain_step(batch, batch_idx, stage="pretrain")
-        return self.step(batch, batch_idx, stage="training")
+        
+        self._configure_fate(
+            graph=kNN_Graph,
+            csv_path = fate_bias_csv_path,
+            t0_idx = t0_idx,
+            fate_bias_multiplier = fate_bias_multiplier,
+            PCA = PCA,
+        )
 
     def __repr__(self):
-        return "LightningSDE-VAE-FixedPotential"
+        return "LightningSDE-VAE-PriorPotential-FateBiasAware"
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/_lightning_sde_vae_prior_potential.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/base/_base_lightning_diffeq.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 # -- DiffEq class: -------------------------------------------------------------
 class BaseLightningDiffEq(lightning.LightningModule):
     def __init__(self, *args, **kwargs):
         super().__init__()
 
         self.sinkhorn_divergence = SinkhornDivergence(backend="auto", **kwargs)
         self.process_batch = BatchProcessor
+        self.COMPLETED_EPOCHS = 0
+        
+    def _update_lit_diffeq_hparams(self, model_params):
+        for key, val in self.hparams.items():
+            if key in model_params.keys():
+                if val != model_params[key]:
+                    self.hparams.update({key: model_params[key]})
         
     # -- setup: ----------------------------------------------------------------
     def _configure_optimizers_schedulers(self):
         """Assumes no pre-train - i.e., a single optimizer, scheduler"""
         optimizer = self.hparams['train_optimizer']
         scheduler = self.hparams['train_scheduler']
 
@@ -35,14 +42,18 @@
         ]
 
     def _configure_torch_modules(self, func, kwargs):
         
         kwargs['state_size'] = self.hparams['latent_dim']
         self.func = func(**utils.function_kwargs(func, kwargs))
         
+    @property
+    def PRETRAIN(self):
+        return False
+    
     # -- integrator stuff: -----------------------------------------------------
     @property
     def _INTEGRATOR(self):
         if self.hparams["adjoint"]:
             return torchsde.sdeint_adjoint
         return torchsde.sdeint
 
@@ -60,23 +71,24 @@
     def compute_sinkhorn_divergence(self, X, X_hat, W, W_hat):
         return self.sinkhorn_divergence(
             W.contiguous(), X.contiguous(), W_hat.contiguous(), X_hat.contiguous()
         )
 
     def log_sinkhorn_divergence(self, sinkhorn_loss, t, stage):
         for i in range(len(t)):
-            msg = f"sinkhorn_{t[i].item()}_{stage}"
+            _t = round(t[i].item(), 3)
+            msg = f"sinkhorn_{_t}_{stage}"
             val = sinkhorn_loss[i]
             self.log(msg, val)
 
         return sinkhorn_loss.sum()
 
     # -- custom steps: -------------------------------------------------------------
     @abstractmethod
-    def forward(self, X0, t, **kwargs):
+    def forward(self, Z0, t, **kwargs):
         """most likely over-written in another class"""
         ...
 
     @abstractmethod
     def step(self, batch, batch_idx, stage=None):
         ...
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_base_forward_mix_in.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     def step(self, batch, batch_idx, stage=None):
 
         batch = self.process_batch(batch, batch_idx)
         X_hat = self.forward(batch.X0, batch.t)
         sinkhorn_loss = self.compute_sinkhorn_divergence(
             batch.X, X_hat, batch.W, batch.W_hat
         )
-        return self.log_sinkhorn_divergence(sinkhorn_loss, t=batch.t, stage=stage)
+        return self.log_sinkhorn_divergence(sinkhorn_loss, t=batch.t, stage=stage)
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_drift_prior_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_pre_train_mix_in.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 
     def validation_step(self, batch, batch_idx, *args, **kwargs):
         if not self.PRETRAIN:
             return self.step(batch, batch_idx, stage="validation")
 
     @property
     def PRETRAIN(self):
-        return self.current_epoch < self.hparams["pretrain_epochs"]
+        return self.COMPLETED_EPOCHS < self.hparams["pretrain_epochs"]
+#         return self.current_epoch < self.hparams["pretrain_epochs"]
 
     @abstractmethod
     def pretrain_step(self):
         ...
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_sde_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/lightning_models/mix_ins/_vae_mix_in.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/__init__.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,8 +27,18 @@
 from ._function_fetch import FunctionFetch, fetch_optimizer, fetch_lr_scheduler
 
 
 from ._anndata_inspector import AnnDataInspector
 from ._info_message import InfoMessage
 from ._abc_parse import ABCParse
 from ._fast_graph import FastGraph
-from ._fetch_format import fetch_format
+from ._fetch_format import fetch_format
+
+from ._idx_to_int_str import idx_to_int_str
+
+from ._logs import Logs, PretrainLogs, TrainLogs
+
+from ._filter_df import filter_df
+
+from ._display_tracked_loss import display_tracked_loss
+
+from ._knn_graph_query import kNNGraphQuery
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_anndata_inspector.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_anndata_inspector.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_autoparse_base_class.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_autoparse_base_class.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_default_neural_sde.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_default_neural_sde.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_fast_graph.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_fast_graph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 
 from ._info_message import InfoMessage
 from ._anndata_inspector import AnnDataInspector
 
 import annoyance
 import pandas as pd
+import torch
+import numpy as np
+
+NoneType = type(None)
 
 class FastGraph:
     def __init__(self, adata, use_key, annot_key="Cell type annotation"):
 
         self._INFO = InfoMessage()
 
         self.adata = adata
@@ -24,15 +28,36 @@
         return (
             self.adata[X_nn.flatten().astype(str)]
             .obs[self.annot_key]
             .values.reshape(-1, self.Graph._n_neighbors)
         )
 
     def _query(self, X_fin):
-        return self._fast_count(self.Graph.query(X_fin.detach().cpu().numpy()))
+        return self._fast_count(self.Graph.query(X_fin))
 
     def _fate_df(self, x_lab):
         return pd.DataFrame([x_lab[0].value_counts() for i in range(len(x_lab))])
-
-    def __call__(self, X_hat):
-        x_lab = self._query(X_hat[-1])
-        return self._fate_df(x_lab)
+    
+    def _DETACH(self, X_hat: torch.Tensor)->np.ndarray:
+        return X_hat.detach().cpu().numpy()
+    
+    def _DETACH_FINAL(self, X_hat: torch.Tensor)->np.ndarray:
+        return X_hat[-1].detach().cpu().numpy()
+    
+    def _TRANSFORM(self, dimension_reduction_model, X_fin):
+        return dimension_reduction_model.transform(X_fin)
+        
+
+    def __call__(self, X_hat, dimension_reduction_model = None, final_timepoint_only=True):
+        
+        if X_hat.device != "cpu" and (final_timepoint_only):
+            X_hat_ = self._DETACH_FINAL(X_hat)
+        elif X_hat.device != "cpu":
+            X_hat_ = self._DETACH(X_hat)
+        elif final_timepoint_only:
+            X_hat_ = X_hat[-1].numpy()
+        else:
+            X_hat_ = X_hat.numpy()
+            
+        if not isinstance(dimension_reduction_model, NoneType):
+            X_hat_ = self._TRANSFORM(dimension_reduction_model, X_hat_)
+        return self._fate_df(self._query(X_fin))
```

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_fetch.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_function_fetch.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_function_kwargs.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_logging_learnable_hparams.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_logging_learnable_hparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/core/utils/_scdiffeq_logger.py` & `scdiffeq-0.0.46rc3/scdiffeq/core/utils/_scdiffeq_logger.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/io/__init__.py` & `scdiffeq-0.0.46rc3/scdiffeq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/io/_pickle_io.py` & `scdiffeq-0.0.46rc3/scdiffeq/io/_pickle_io.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/io/_read_h5ad.py` & `scdiffeq-0.0.46rc3/scdiffeq/io/_read_h5ad.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/__init__.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_annotate_cells.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_annotate_cells.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_dimension_reduction.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_drift_diffusion_state_characterization.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_drift_diffusion_state_characterization.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_func_from_version.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_func_from_version.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_hyperparams.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_hyperparams.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_reconstruct_function.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_reconstruct_function.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_time_free_sampling.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_time_free_sampling.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_umap.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq/tools/_versions.py` & `scdiffeq-0.0.46rc3/scdiffeq/tools/_versions.py`

 * *Files identical despite different names*

### Comparing `scdiffeq-0.0.46rc1/scdiffeq.egg-info/PKG-INFO` & `scdiffeq-0.0.46rc3/scdiffeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: scdiffeq
-Version: 0.0.46rc1
+Version: 0.0.46rc3
 Summary: scDiffEq: modelling single-cell dynamics using neural differential equations.
 Home-page: https://github.com/mvinyard/sc-neural-diffeqs
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <a href=""><img src=docs/images/scdiffeq.logo.png alt="scdiffeq-logo" width="320"/>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc1 Summary: scDiffEq:
+Metadata-Version: 2.1 Name: scdiffeq Version: 0.0.46rc3 Summary: scDiffEq:
 modelling single-cell dynamics using neural differential equations. Home-page:
 https://github.com/mvinyard/sc-neural-diffeqs Author: Michael E. Vinyard -
 Harvard University - Massachussetts General Hospital - Broad Institute of MIT
 and Harvard Author-email: mvinyard@broadinstitute.org License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python
-:: 3.7 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
+:: 3.9 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-
 Content-Type: text/markdown License-File: LICENSE # [scdiffeq-logo] [![PyPI
 pyversions](https://img.shields.io/pypi/pyversions/scdiffeq.svg)](https://
 pypi.python.org/pypi/scdiffeq/) [![PyPI version](https://badge.fury.io/py/
 scdiffeq.svg)](https://badge.fury.io/py/scdiffeq) [![Code style: black](https:/
 /img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) An analysis framework for modeling dynamical single-cell data with
```

### Comparing `scdiffeq-0.0.46rc1/setup.py` & `scdiffeq-0.0.46rc3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import re
 import os
 import sys
 
 setuptools.setup(
     name="scdiffeq",
-    version="0.0.46rc1",
+    version="0.0.46rc3",
     python_requires=">3.9.0",
     author="Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     author_email="mvinyard@broadinstitute.org",
     url="https://github.com/mvinyard/sc-neural-diffeqs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="scDiffEq: modelling single-cell dynamics using neural differential equations.",
@@ -22,20 +22,22 @@
         "licorice_font>=0.0.3",
         "torchsde>=0.2.5",
         "scikit-learn>=1.0.2",
         "umap-learn>=0.5.3",
         "lightning>=2.0.1",
         "neural-diffeqs==0.3.1rc0",
         "torch-nets>=0.0.4",
-        "torch-adata>=0.0.20",
+        "torch-adata>=0.0.23",
         "autodevice>=0.0.2",
         "brownian-diffuser>=0.0.2",
         "vinplots>=0.0.75",
+        "annoyance==0.0.18",
+        "ABCParse==0.0.3",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     license="MIT",
 )
```

