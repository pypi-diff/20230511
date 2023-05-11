# Comparing `tmp/osl-dynamics-1.2.2.tar.gz` & `tmp/osl-dynamics-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osl-dynamics-1.2.2.tar", last modified: Mon Apr 17 12:40:43 2023, max compression
+gzip compressed data, was "osl-dynamics-1.2.3.tar", last modified: Thu May 11 16:43:18 2023, max compression
```

## Comparing `osl-dynamics-1.2.2.tar` & `osl-dynamics-1.2.3.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.897807 osl-dynamics-1.2.2/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-17 12:40:43.897995 osl-dynamics-1.2.2/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4128 2023-04-17 08:41:13.000000 osl-dynamics-1.2.2/README.rst
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.051322 osl-dynamics-1.2.2/osl_dynamics/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/__init__.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.130385 osl-dynamics-1.2.2/osl_dynamics/analysis/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      231 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    27101 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/connectivity.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6323 2023-04-14 14:48:30.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/fisher_kernel.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6165 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/gmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22485 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    18679 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/power.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-02-19 13:57:27.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/regression.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    44293 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/spectral.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7487 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/static.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7333 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/statistics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5688 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/workbench.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8199 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/array_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.144033 osl-dynamics-1.2.2/osl_dynamics/config_api/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      222 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      751 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/cli.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4477 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/pipeline.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    50523 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/wrappers.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.181753 osl-dynamics-1.2.2/osl_dynamics/data/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      185 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/data/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    36748 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/data/osl.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6757 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/processing.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8574 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/rw.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2809 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/spm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2447 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/task.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4726 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/data/tf.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.204462 osl-dynamics-1.2.2/osl_dynamics/files/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      883 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      434 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/functions.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.461814 osl-dynamics-1.2.2/osl_dynamics/files/mask/
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1649 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/__init__.py
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.517260 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      669 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.520824 osl-dynamics-1.2.2/osl_dynamics/files/scanner/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/ctf275_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.684049 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D148.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi160.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi256.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi32.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/neuromag306_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.686730 osl-dynamics-1.2.2/osl_dynamics/files/scene/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scene/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scene/mode_scene.scene
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.781106 osl-dynamics-1.2.2/osl_dynamics/inference/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/inference/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/inference/callbacks.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7410 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/inference/initializers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42087 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/inference/layers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11394 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/inference/metrics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15547 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/inference/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-02-13 15:05:52.000000 osl-dynamics-1.2.2/osl_dynamics/inference/regularizers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-02-19 13:57:27.000000 osl-dynamics-1.2.2/osl_dynamics/inference/tf_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.826545 osl-dynamics-1.2.2/osl_dynamics/models/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1426 2023-02-28 15:36:39.000000 osl-dynamics-1.2.2/osl_dynamics/models/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    16781 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/dynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11105 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/dynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    41033 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15849 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/inf_mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    23641 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/mage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20241 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/mdynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11366 2023-02-19 13:57:27.000000 osl-dynamics-1.2.2/osl_dynamics/models/mdynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    16639 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19196 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/sage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    28468 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/models/sedynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    29860 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/sedynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13439 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/state_dynemo.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.877875 osl-dynamics-1.2.2/osl_dynamics/simulation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      566 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    30162 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12958 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/hsmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2022-10-24 10:06:46.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/mar.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    26028 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/mvn.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/sin.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    10563 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/sm.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.897102 osl-dynamics-1.2.2/osl_dynamics/utils/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2022-10-30 10:07:31.000000 osl-dynamics-1.2.2/osl_dynamics/utils/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2022-10-30 10:07:31.000000 osl-dynamics-1.2.2/osl_dynamics/utils/decorators.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13545 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/misc.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6997 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/model.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/parcellation.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    55601 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/plotting.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/topoplots.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.065381 osl-dynamics-1.2.2/osl_dynamics.egg-info/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-17 12:40:43.062030 osl-dynamics-1.2.2/osl_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8279 2023-04-17 12:40:43.062562 osl-dynamics-1.2.2/osl_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-04-17 12:40:43.063229 osl-dynamics-1.2.2/osl_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       71 2023-04-17 12:40:43.063806 osl-dynamics-1.2.2/osl_dynamics.egg-info/entry_points.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      141 2023-04-17 12:40:43.064729 osl-dynamics-1.2.2/osl_dynamics.egg-info/requires.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-04-17 12:40:43.065550 osl-dynamics-1.2.2/osl_dynamics.egg-info/top_level.txt
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1161 2023-04-17 12:40:43.898763 osl-dynamics-1.2.2/setup.cfg
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/setup.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.981915 osl-dynamics-1.2.3/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4561 2023-05-11 16:43:18.982335 osl-dynamics-1.2.3/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4248 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/README.rst
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:17.543504 osl-dynamics-1.2.3/osl_dynamics/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/__init__.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:17.652257 osl-dynamics-1.2.3/osl_dynamics/analysis/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      250 2023-05-09 14:36:05.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    27101 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/connectivity.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6437 2023-05-09 14:35:55.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/fisher_kernel.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6165 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/gmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    23992 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19627 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/power.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/regression.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    44348 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/spectral.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7487 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/static.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8486 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/statistics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    29697 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/tinda.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5688 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/analysis/workbench.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    10899 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/array_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:17.660911 osl-dynamics-1.2.3/osl_dynamics/config_api/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      909 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/config_api/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5911 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/config_api/pipeline.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    50607 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/config_api/wrappers.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:17.730284 osl-dynamics-1.2.3/osl_dynamics/data/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      185 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/data/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36748 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/data/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/data/osl.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6757 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/data/processing.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8574 2023-05-10 09:37:57.000000 osl-dynamics-1.2.3/osl_dynamics/data/rw.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2809 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/data/spm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2447 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/data/task.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4726 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/data/tf.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:17.740887 osl-dynamics-1.2.3/osl_dynamics/files/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      883 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      434 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/functions.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:17.849839 osl-dynamics-1.2.3/osl_dynamics/files/mask/
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1649 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/__init__.py
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.045358 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      669 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.072484 osl-dynamics-1.2.3/osl_dynamics/files/scanner/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/ctf275_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.694018 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D148.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D248.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF151.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF275.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/EEG1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/EEG1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/EEG1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi160.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi256.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi32.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM1.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM1.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM10.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM10.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM11.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM11.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM14.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM14.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM15.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM15.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM16.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM17.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM17.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM20.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM20.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM22.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM22.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM23.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM23.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM24.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM24.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM25.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM25.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM3.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM3.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM7.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM7.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/elec1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/elec1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/elec1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/quickcap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/quickcap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scanner/neuromag306_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.703959 osl-dynamics-1.2.3/osl_dynamics/files/scene/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scene/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/files/scene/mode_scene.scene
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.791588 osl-dynamics-1.2.3/osl_dynamics/inference/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/callbacks.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7410 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/initializers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42321 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/layers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11394 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/metrics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19804 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/regularizers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/inference/tf_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.870350 osl-dynamics-1.2.3/osl_dynamics/models/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1426 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    16781 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/dynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11105 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/dynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42668 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15849 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/inf_mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    23641 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/mage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20241 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/mdynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11366 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/mdynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    16639 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19196 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/sage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    28945 2023-05-11 16:41:15.000000 osl-dynamics-1.2.3/osl_dynamics/models/sedynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    30491 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/sedynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36299 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/sehmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13439 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/models/state_dynemo.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.918348 osl-dynamics-1.2.3/osl_dynamics/simulation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      566 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    30162 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12958 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/hsmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/mar.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    26028 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/mvn.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/sin.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    10563 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/simulation/sm.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:18.973554 osl-dynamics-1.2.3/osl_dynamics/utils/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/utils/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/utils/decorators.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13545 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/utils/misc.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6997 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/utils/model.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/utils/parcellation.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    59142 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/utils/plotting.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/osl_dynamics/utils/topoplots.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-05-11 16:43:17.565668 osl-dynamics-1.2.3/osl_dynamics.egg-info/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4561 2023-05-11 16:43:17.562185 osl-dynamics-1.2.3/osl_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8308 2023-05-11 16:43:17.563420 osl-dynamics-1.2.3/osl_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-05-11 16:43:17.564129 osl-dynamics-1.2.3/osl_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       85 2023-05-11 16:43:17.564572 osl-dynamics-1.2.3/osl_dynamics.egg-info/entry_points.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      141 2023-05-11 16:43:17.565173 osl-dynamics-1.2.3/osl_dynamics.egg-info/requires.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-05-11 16:43:17.565881 osl-dynamics-1.2.3/osl_dynamics.egg-info/top_level.txt
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1175 2023-05-11 16:43:18.983535 osl-dynamics-1.2.3/setup.cfg
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2023-05-09 14:22:26.000000 osl-dynamics-1.2.3/setup.py
```

### Comparing `osl-dynamics-1.2.2/PKG-INFO` & `osl-dynamics-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.2.2
+Version: 1.2.3
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 ============
@@ -22,15 +22,15 @@
 
     git clone https://github.com/OHBA-analysis/osl-dynamics.git
     cd osl-dynamics
     conda env create -f envs/linux.yml
     conda activate osld
     pip install -e .
 
-Note, the conda environments use ``pip`` to install TensorFlow, you may need to load/install additional libraries (such as CUDA/cuDNN) if you have GPU support.
+If you're using a Mac then use the ``envs/mac.yml`` file to create the conda environment instead of ``envs/linux.yml``. Note, the conda environments use ``pip`` to install TensorFlow, you may need to load/install additional libraries (such as CUDA/cuDNN) if you have GPU support.
 
 Developers might want to clone the repo using SSH instead of HTTPS:
 
 .. code-block:: shell
 
     git clone git@github.com:OHBA-analysis/osl-dynamics.git
```

### Comparing `osl-dynamics-1.2.2/README.rst` & `osl-dynamics-1.2.3/osl_dynamics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: osl-dynamics
+Version: 1.2.3
+Summary: Models for infering dynamics in neuroimaging data
+Home-page: https://github.com/OHBA-analysis/osl-dynamics
+License: MIT
+Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
+Description-Content-Type: text/x-rst; charset=UTF-8
+
 ============
 osl-dynamics
 ============
 
 See the read the docs page for a description of this project: `https://osl-dynamics.readthedocs.io <https://osl-dynamics.readthedocs.io>`_.
 
 Installation
@@ -13,15 +22,15 @@
 
     git clone https://github.com/OHBA-analysis/osl-dynamics.git
     cd osl-dynamics
     conda env create -f envs/linux.yml
     conda activate osld
     pip install -e .
 
-Note, the conda environments use ``pip`` to install TensorFlow, you may need to load/install additional libraries (such as CUDA/cuDNN) if you have GPU support.
+If you're using a Mac then use the ``envs/mac.yml`` file to create the conda environment instead of ``envs/linux.yml``. Note, the conda environments use ``pip`` to install TensorFlow, you may need to load/install additional libraries (such as CUDA/cuDNN) if you have GPU support.
 
 Developers might want to clone the repo using SSH instead of HTTPS:
 
 .. code-block:: shell
 
     git clone git@github.com:OHBA-analysis/osl-dynamics.git
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/__init__.py` & `osl-dynamics-1.2.3/osl_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/connectivity.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/connectivity.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/fisher_kernel.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/fisher_kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+"""Implementation of the Fisher kernel for prediction studies.
+
+"""
+
 import numpy as np
-import tensorflow as tf
 import logging
 from tqdm.auto import trange
 
 _logger = logging.getLogger("osl-dynamics")
 
 
 class FisherKernel:
@@ -12,14 +15,16 @@
     Parameters
     ----------
     model : osl_dynamics.models.Model
         Model.
     """
 
     def __init__(self, model):
+        import tensorflow as tf  # moved here to avoid slow imports
+
         compatible_models = ["HMM", "DyNeMo", "M-DyNeMo"]
         if model.config.model_name not in compatible_models:
             raise NotImplementedError(
                 f"{model.config.model_name} was not found."
                 + f"Options are {compatible_models}."
             )
         self.model = model
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/gmm.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/gmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/modes.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/modes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Functions to manipulate and analyse inferred mode/state data.
 
 """
 
+import itertools
 import logging
 
 import numpy as np
 
 from osl_dynamics import array_ops, inference
 
 _logger = logging.getLogger("osl-dynamics")
@@ -28,15 +29,14 @@
         PCA components used for dimensionality reduction.
 
     Returns
     -------
     acfs : np.ndarray
         Auto/cross-correlation functions.
     """
-
     # Validation
     error_message = (
         "mode_covariances must be of shape (n_channels, n_channels) or "
         + "(n_modes, n_channels, n_channels) or "
         + "(n_subjects, n_modes, n_channels, n_channels)."
     )
     mode_covariances = array_ops.validate(
@@ -54,20 +54,26 @@
     n_modes = te_covs.shape[1]
     n_parcels = te_covs.shape[-1] // n_embeddings
     n_acf = 2 * n_embeddings - 1
 
     # Take mean of elements from the time embedded covariances that
     # correspond to the auto/cross-correlation function
     blocks = te_covs.reshape(
-        n_subjects, n_modes, n_parcels, n_embeddings, n_parcels, n_embeddings
+        n_subjects,
+        n_modes,
+        n_parcels,
+        n_embeddings,
+        n_parcels,
+        n_embeddings,
     )
     acfs = np.empty([n_subjects, n_modes, n_parcels, n_parcels, n_acf])
     for i in range(n_acf):
         acfs[:, :, :, :, i] = np.mean(
-            np.diagonal(blocks, offset=i - n_embeddings + 1, axis1=3, axis2=5), axis=-1
+            np.diagonal(blocks, offset=i - n_embeddings + 1, axis1=3, axis2=5),
+            axis=-1,
         )
 
     return np.squeeze(acfs)
 
 
 def raw_covariances(
     mode_covariances,
@@ -93,15 +99,14 @@
         the mean over time lags.
 
     Returns
     -------
     raw_covs : np.ndarray
         Covariance matrix for raw channels.
     """
-
     # Validation
     error_message = (
         "mode_covariances must be of shape (n_channels, n_channels) or "
         + "(n_modes, n_channels, n_channels) or "
         + "(n_subjects, n_modes, n_channels, n_channels)."
     )
     mode_covariances = array_ops.validate(
@@ -113,26 +118,34 @@
 
     # Get covariance of time embedded data
     te_covs = reverse_pca(mode_covariances, pca_components)
 
     if zero_lag:
         # Return the zero-lag elements only
         raw_covs = te_covs[
-            :, :, n_embeddings // 2 :: n_embeddings, n_embeddings // 2 :: n_embeddings
+            :,
+            :,
+            n_embeddings // 2 :: n_embeddings,
+            n_embeddings // 2 :: n_embeddings,
         ]
 
     else:
         # Return block means
         n_subjects = te_covs.shape[0]
         n_modes = te_covs.shape[1]
         n_parcels = te_covs.shape[-1] // n_embeddings
 
         n_parcels = te_covs.shape[-1] // n_embeddings
         blocks = te_covs.reshape(
-            n_subjects, n_modes, n_parcels, n_embeddings, n_parcels, n_embeddings
+            n_subjects,
+            n_modes,
+            n_parcels,
+            n_embeddings,
+            n_parcels,
+            n_embeddings,
         )
         block_diagonal = blocks.diagonal(0, 2, 4)
         diagonal_means = block_diagonal.diagonal(0, 2, 3).mean(3)
 
         raw_covs = blocks.mean((3, 5))
         raw_covs[:, :, np.arange(n_parcels), np.arange(n_parcels)] = diagonal_means
 
@@ -160,97 +173,123 @@
             + f"covariances.shape={covariances.shape}, "
             + f"pca_components.shape={pca_components.shape}."
         )
 
     return pca_components @ covariances @ pca_components.T
 
 
-def state_activation(state_time_course):
+def state_activations(state_time_course):
     """Calculate state activations from a state time course.
 
     Given a state time course (strictly binary), calculate the beginning and
-    end of each activation of each state.
+    end of each activation of each state. Accepts a 1D or 2D array. If a 1D
+    array is passed, it is assumed to be a single state time course.
+
+    Either an array of ints or an array of bools is accepted, but if ints are passed
+    they should be explicitly zero or one.
 
     Parameters
     ----------
-    state_time_course : numpy.ndarray
+    state_time_course : numpy.ndarray or list of numpy.ndarray
         State time course (strictly binary).
 
     Returns
     -------
-    ons : list of numpy.ndarray
-        List containing state beginnings (index) in the order they occur for
+    slices: list of list of slice
+        List containing state activations (index) in the order they occur for
         each state. This cannot necessarily be converted into an array as an
         equal number of elements in each array is not guaranteed.
-    offs : list of numpy.ndarray
-        List containing state ends (index) in the order they occur for each state.
-        This cannot necessarily be converted into an array as an equal number of
-        elements in each array is not guaranteed.
-    """
-    state_on = []
-    state_off = []
-
-    diffs = np.diff(state_time_course, axis=0)
-    for i, diff in enumerate(diffs.T):
-        on = (diff == 1).nonzero()[0]
-        off = (diff == -1).nonzero()[0]
-        try:
-            if on[-1] > off[-1]:
-                off = np.append(off, len(diff))
-
-            if off[0] < on[0]:
-                on = np.insert(on, 0, -1)
-
-            state_on.append(on)
-            state_off.append(off)
-        except IndexError:
-            _logger.info(f"No activation in state {i}.")
-            state_on.append(np.array([]))
-            state_off.append(np.array([]))
-
-    state_on = np.array(state_on, dtype=object)
-    state_off = np.array(state_off, dtype=object)
-
-    return state_on, state_off
+    """
+    # Make sure we have a list of numpy arrays
+    shape_error_message = (
+        "State time course must be a 1D, 2D or 3D array or list of 2D arrays."
+    )
+    if isinstance(state_time_course, np.ndarray):
+        if state_time_course.ndim == 3 or state_time_course.dtype == object:
+            state_time_course = list(state_time_course)
+        if state_time_course.ndim == 2:
+            state_time_course = [state_time_course]
+        elif state_time_course.ndim == 1:
+            state_time_course = [state_time_course[:, np.newaxis]]
+        else:
+            raise ValueError(shape_error_message)
+    elif isinstance(state_time_course, list):
+        if not all(isinstance(stc, np.ndarray) for stc in state_time_course):
+            raise ValueError(shape_error_message)
+        if not all(stc.ndim == 2 for stc in state_time_course):
+            raise ValueError(shape_error_message)
+
+    # Make sure the list of arrays is of type bool
+    type_error_message = (
+        "State time course must be strictly binary. "
+        "This can either be np.bools or np.ints with values 0 and 1."
+    )
+    bool_state_time_course = []
+    for stc in state_time_course:
+        if np.issubdtype(stc.dtype, np.integer):
+            if np.all(np.isin(stc, [0, 1])):
+                bool_state_time_course.append(stc.astype(bool))
+        elif np.issubdtype(stc.dtype, np.bool_):
+            bool_state_time_course.append(stc)
+        else:
+            raise ValueError(type_error_message)
+
+    # Get the slices where each state is True
+    slices = [
+        [array_ops.ezclump(column) for column in stc.T]
+        for stc in bool_state_time_course
+    ]
+    return slices
 
 
-def lifetimes(state_time_course, sampling_frequency=None):
+def lifetimes(state_time_course, sampling_frequency=None, squeeze=True):
     """Calculate state lifetimes from a state time course.
 
     Given a state time course (one-hot encoded), calculate the lifetime of each
     activation of each state.
 
     Parameters
     ----------
     state_time_course : numpy.ndarray
         State time course (strictly binary). Shape must be (n_subjects,
         n_samples, n_states) or (n_samples, or n_states).
     sampling_frequency : float
         Sampling frequency in Hz. If passed returns the lifetimes in seconds.
+    squeeze : bool
+        If True, squeeze the output to remove singleton dimensions.
 
     Returns
     -------
     lts : list of numpy.ndarray
         List containing an array of lifetimes in the order they occur for each
         state. This cannot necessarily be converted into an array as an equal
         number of elements in each array is not guaranteed. Shape is (n_subjects,
         n_states, n_activations) or (n_states, n_activations).
     """
-    if isinstance(state_time_course, np.ndarray):
-        state_time_course = [state_time_course]
-    lts = []
-    for stc in state_time_course:
-        ons, offs = state_activation(stc)
-        lt = offs - ons
-        if sampling_frequency is not None:
-            lt = [lt_ / sampling_frequency for lt_ in lt]
-        lts.append(lt)
-    if len(lts) == 1:
-        lts = lts[0]
-    return lts
+    sampling_frequency = sampling_frequency or 1
+    slices = state_activations(state_time_course)
+
+    result = [
+        [
+            np.array([array_ops.slice_length(slice_) for slice_ in state_slices])
+            / sampling_frequency
+            for state_slices in subject_slices
+        ]
+        for subject_slices in slices
+    ]
+
+    if not squeeze:
+        return result
+
+    if len(result) == 1:
+        result = result[0]
+        if len(result) == 1:
+            result = result[0]
+
+    return result
 
 
 def lifetime_statistics(state_time_course, sampling_frequency=None):
     """Calculate statistics of the lifetime distribution of each state.
 
     Parameters
     ----------
@@ -265,27 +304,22 @@
     means : np.ndarray
         Mean lifetime of each state. Shape is (n_subjects, n_states) or
         (n_states,).
     std : np.ndarray
         Standard deviation of each state. Shape is (n_subjects, n_states) or
         (n_states,).
     """
-    lts = lifetimes(state_time_course, sampling_frequency)
-    if np.array(lts, dtype=object).ndim == 2:
-        # lts.shape = (n_subjects, n_states, n_activations)
-        mean = []
-        std = []
-        for i in range(len(lts)):
-            mean.append([np.mean(lt) for lt in lts[i]])
-            std.append([np.std(lt) for lt in lts[i]])
-    else:
-        # lts.shape = (n_states, n_activations)
-        mean = [np.mean(lt) for lt in lts]
-        std = [np.std(lt) for lt in lts]
-    return np.array(mean), np.array(std)
+    lifetimes_ = lifetimes(
+        state_time_course,
+        sampling_frequency=sampling_frequency,
+        squeeze=False,
+    )
+    means = np.squeeze(array_ops.list_means(lifetimes_))
+    stds = np.squeeze(array_ops.list_stds(lifetimes_))
+    return means, stds
 
 
 def mean_lifetimes(state_time_course, sampling_frequency=None):
     """Calculate the mean lifetime of each state.
 
     Parameters
     ----------
@@ -300,49 +334,62 @@
     mlt : np.ndarray
         Mean lifetime of each state. Shape is (n_subjects, n_states) or
         (n_states,).
     """
     return lifetime_statistics(state_time_course, sampling_frequency)[0]
 
 
-def intervals(state_time_course, sampling_frequency=None):
+def intervals(state_time_course, sampling_frequency=None, squeeze=True):
     """Calculate state intervals from a state time course.
 
     An interval is the duration between successive visits for a particular state.
 
     Parameters
     ----------
     state_time_course : list or numpy.ndarray
         State time course (strictly binary). Shape must be (n_subjects, n_samples,
         n_states) or (n_samples, n_states).
     sampling_frequency : float
         Sampling frequency in Hz. If passed returns the intervals in seconds.
+    squeeze : bool
+        If True, squeeze the output to remove singleton dimensions.
 
     Returns
     -------
     intvs : list of numpy.ndarray
         List containing an array of intervals in the order they occur for each
         state. This cannot necessarily be converted into an array as an equal
         number of elements in each array is not guaranteed. Shape is (n_subjects,
         n_states, n_activations) or (n_states, n_activations).
     """
-    if isinstance(state_time_course, np.ndarray):
-        state_time_course = [state_time_course]
-    intvs = []
-    for stc in state_time_course:
-        intv = []
-        ons, offs = state_activation(stc)
-        for on, off in zip(ons, offs):
-            intv.append(on[1:] - off[:-1])
-        if sampling_frequency is not None:
-            intv = [i / sampling_frequency for i in intv]
-        intvs.append(intv)
-    if len(intvs) == 1:
-        intvs = intvs[0]
-    return intvs
+    sampling_frequency = sampling_frequency or 1
+    slices = state_activations(state_time_course)
+    result = [
+        [
+            np.array(
+                [
+                    slice_1.start - slice_0.stop
+                    for slice_0, slice_1 in itertools.pairwise(state_slices)
+                ],
+            )
+            / sampling_frequency
+            for state_slices in subject_slice
+        ]
+        for subject_slice in slices
+    ]
+
+    if not squeeze:
+        return result
+
+    if len(result) == 1:
+        result = result[0]
+        if len(result) == 1:
+            result = result[0]
+
+    return result
 
 
 def interval_statistics(state_time_course, sampling_frequency=None):
     """Calculate statistics of the interval distribution of each state.
 
     Parameters
     ----------
@@ -357,27 +404,20 @@
     means : np.ndarray
         Mean interval of each state. Shape is (n_subjects, n_states) or
         (n_states,).
     std : np.ndarray
         Standard deviation of each state. Shape is (n_subjects, n_states) or
         (n_states,).
     """
-    intvs = intervals(state_time_course, sampling_frequency)
-    if np.array(intvs, dtype=object).ndim == 2:
-        # intvs.shape = (n_subjects, n_states, n_activations)
-        mean = []
-        std = []
-        for i in range(len(intvs)):
-            mean.append([np.mean(lt) for lt in intvs[i]])
-            std.append([np.std(lt) for lt in intvs[i]])
-    else:
-        # intvs.shape = (n_states, n_activations)
-        mean = [np.mean(lt) for lt in intvs]
-        std = [np.std(lt) for lt in intvs]
-    return np.array(mean), np.array(std)
+    intervals_ = intervals(
+        state_time_course, sampling_frequency=sampling_frequency, squeeze=False
+    )
+    means = np.squeeze(array_ops.list_means(intervals_))
+    stds = np.squeeze(array_ops.list_stds(intervals_))
+    return means, stds
 
 
 def mean_intervals(state_time_course, sampling_frequency=None):
     """Calculate the mean interval of each state.
 
     Parameters
     ----------
@@ -393,37 +433,42 @@
         Mean interval of each state. Shape is (n_subjects, n_states) or
         (n_states,).
     """
     return interval_statistics(state_time_course, sampling_frequency)[0]
 
 
 def fractional_occupancies(state_time_course):
-    """Calculates the fractional occupancy.
+    """Calculate the fractional occupancy.
 
     Parameters
     ----------
     state_time_course : list or np.ndarray
         State time course (strictly binary). Shape must be (n_subjects,
         n_samples, n_states) or (n_samples, n_states).
 
     Returns
     -------
     fo : np.ndarray
         The fractional occupancy of each state. Shape is (n_subjects, n_states)
         or (n_states,).
     """
-    if isinstance(state_time_course, list):
-        fo = [np.sum(stc, axis=0) / stc.shape[0] for stc in state_time_course]
-    else:
-        fo = np.sum(state_time_course, axis=0) / state_time_course.shape[0]
-    return np.array(fo, dtype=np.float32)
+    if isinstance(state_time_course, np.ndarray):
+        if state_time_course.ndim == 2:
+            state_time_course = [state_time_course]
+        elif state_time_course.ndim != 3:
+            raise ValueError(
+                "A (n_subjects, n_samples, n_states) or "
+                "(n_samples, n_states) array must be passed."
+            )
+    fo = [np.sum(stc, axis=0) / stc.shape[0] for stc in state_time_course]
+    return np.squeeze(fo)
 
 
 def switching_rates(state_time_course, sampling_frequency=None):
-    """Calculates the switching rate.
+    """Calculate the switching rate.
 
     This is defined as the number of state activations per second.
 
     Parameters
     ----------
     state_time_course : list or np.ndarray
         State time course (strictly binary). Shape must be (n_subjects,
@@ -434,15 +479,21 @@
     Returns
     -------
     sr : np.ndarray
         The switching rate of each state. Shape is (n_subjects, n_states)
         or (n_states,).
     """
     if isinstance(state_time_course, np.ndarray):
-        state_time_course = [state_time_course]
+        if state_time_course.ndim == 2:
+            state_time_course = [state_time_course]
+        elif state_time_course.ndim == 3:
+            state_time_course = list(state_time_course)
+
+    # Set sampling frequency
+    sampling_frequency = sampling_frequency or 1
 
     # Loop through subjects
     sr = []
     for subject in state_time_course:
         n_samples, n_states = subject.shape
 
         # Number of activations for each state
@@ -456,15 +507,15 @@
 
 
 def fano_factor(
     state_time_course,
     window_lengths,
     sampling_frequency=1.0,
 ):
-    """Calculates the Fano factor.
+    """Calculate the Fano factor.
 
     Parameters
     ----------
     state_time_course : list or np.ndarray
         State time course (strictly binary). Shape must be (n_subjects,
         n_samples, n_states) or (n_samples, n_states).
     window_lengths : list or np.ndarray
@@ -529,32 +580,32 @@
         Subject-specific transition probability matrices.
         Shape is (n_subjects, n_states, n_states).
     """
     if isinstance(state_time_course, np.ndarray):
         state_time_course = [state_time_course]
     trans_prob = []
     for stc in state_time_course:
-        stc = stc.argmax(axis=1)
+        stc_argmax = stc.argmax(axis=1)
         vals, counts = np.unique(
-            stc[np.arange(2)[None, :] + np.arange(len(stc) - 1)[:, None]],
+            stc_argmax[np.arange(2)[None, :] + np.arange(len(stc_argmax) - 1)[:, None]],
             axis=0,
             return_counts=True,
         )
         if n_states is None:
-            n_states = stc.max() + 1
+            n_states = stc_argmax.max() + 1
         tp = np.zeros((n_states, n_states))
         tp[vals[:, 0], vals[:, 1]] = counts
         with np.errstate(divide="ignore", invalid="ignore"):
             tp /= tp.sum(axis=1)[:, None]
         trans_prob.append(np.nan_to_num(tp))
     return np.squeeze(trans_prob)
 
 
 def simple_moving_average(data, window_length, step_size):
-    """Simple moving average.
+    """Calculate imple moving average.
 
     Calculates moving averages by computing the unweighted mean of n
     observations over the current time window. Can be used to smooth
     the fractional occupancy time courses as in Baker et al. (2014).
 
     Parameters
     ----------
@@ -572,15 +623,16 @@
     """
     # Get number of samples and modes
     n_samples = data.shape[0]
     n_modes = data.shape[1]
 
     # Pad the data
     data = np.pad(data, window_length // 2)[
-        :, window_length // 2 : window_length // 2 + n_modes
+        :,
+        window_length // 2 : window_length // 2 + n_modes,
     ]
 
     # Define indices of time points to calculate a moving average
     time_idx = range(0, n_samples, step_size)
     n_windows = n_samples // step_size
 
     # Preallocate an array to hold moving average values
@@ -639,18 +691,18 @@
     for i in range(len(data)):
         if data[i].shape[0] != alpha[i].shape[0]:
             raise ValueError("Difference number of samples in data and alpha.")
 
     pcovs = []
     for X, a in zip(data, alpha):
         # Variance normalise state/mode time courses
-        a /= np.std(a, axis=0, keepdims=True)
+        a_normed = a / np.std(a, axis=0, keepdims=True)
 
         # Do multiple regression of alpha onto data
-        pcovs.append(np.linalg.pinv(a) @ X)
+        pcovs.append(np.linalg.pinv(a_normed) @ X)
 
     return np.squeeze(pcovs)
 
 
 def ae_hmm_networks(data, alpha):
     """Calculate subject-specific AE-HMM networks.
 
@@ -667,15 +719,15 @@
     means : np.ndarray
         Subject-specific mean activity maps. Shape is (n_subjects, n_states, n_channels).
     aecs : np.ndarray
         Subject-specific amplitude envelope correlation maps.
         Shape is (n_subjects, n_states, n_channels, n_channels).
     """
     if type(data) != type(alpha):
-        raise ValueError(
+        raise TypeError(
             "data and alpha must be the same type: numpy arrays or lists of numpy arrays."
         )
     if isinstance(data, np.ndarray):
         data = [data]
         alpha = [alpha]
 
     # Hard classify the state probabilties
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/power.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/power.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Functions to calculate and save network power maps.
 
 """
 
-import os
 import logging
+import os
 from pathlib import Path
 
+import matplotlib.pyplot as plt
 import nibabel as nib
 import numpy as np
 from nilearn import plotting
 from tqdm.auto import trange
 
 from osl_dynamics import array_ops, files, utils
 from osl_dynamics.analysis.spectral import get_frequency_args_range
@@ -250,14 +251,15 @@
     power_map,
     mask_file,
     parcellation_file,
     filename=None,
     component=0,
     subtract_mean=False,
     mean_weights=None,
+    asymmetric_data=False,
     plot_kwargs=None,
 ):
     """Saves power maps.
 
     Parameters
     ----------
     power_map : np.ndarray
@@ -277,14 +279,18 @@
     component : int
         Spectral component to save.
     subtract_mean : bool
         Should we subtract the mean power across modes?
     mean_weights: np.ndarray
         Numpy array with weightings for each mode to use to calculate the mean.
         Default is equal weighting.
+    asymmetric_data : bool
+        If True, the power map is scaled to the range [-1, 1] before plotting.
+        The colorbar is rescaled to show the correct values. Useful for plotting
+        maps of statistics such as lifetimes.
     plot_kwargs : dict
         Keyword arguments to pass to `nilearn.plotting.plot_img_on_surf
         <https://nilearn.github.io/stable/modules/generated/nilearn.plotting.plot_img_on_surf.html>`_.
         By default we pass:
 
         - views=["lateral", "medial"]
         - hemispheres=["left", "right"]
@@ -350,14 +356,24 @@
         power_map -= np.average(power_map, axis=1, weights=mean_weights)[
             :, np.newaxis, ...
         ]
 
     # Select the component to plot
     power_map = power_map[component]
 
+    original_max = power_map.max()
+    original_min = power_map.min()
+
+    if asymmetric_data:
+        # Scale power map to be between -1 and 1
+        power_map -= power_map.min()
+        power_map /= power_map.max()
+        power_map *= 2
+        power_map -= 1
+
     # Calculate power map grid
     power_map = power_map_grid(mask_file, parcellation_file, power_map)
 
     # Load the mask
     mask = nib.load(mask_file)
 
     # Number of modes
@@ -366,23 +382,33 @@
     # Keyword arguments to pass to nilearn.plotting.plot_img_on_surf
     default_plot_kwargs = {
         "views": ["lateral", "medial"],
         "hemisphere": ["left", "right"],
         "colorbar": True,
     }
     plot_kwargs = utils.misc.override_dict_defaults(default_plot_kwargs, plot_kwargs)
+    cmap = plot_kwargs.get("cmap", "cold_hot")
 
     # Just display the power map
     if filename is None:
         figures, axes = [], []
         for i in trange(n_modes, desc="Saving images"):
             nii = nib.Nifti1Image(power_map[:, :, :, i], mask.affine, mask.header)
             fig, ax = plotting.plot_img_on_surf(nii, output_file=None, **plot_kwargs)
             figures.append(fig)
             axes.append(ax)
+            if asymmetric_data:
+                plt.colorbar(
+                    plt.cm.ScalarMappable(
+                        plt.matplotlib.colors.Normalize(original_min, original_max),
+                        cmap=cmap,
+                    ),
+                    cax=ax[-1],
+                    orientation="horizontal",
+                )
         return figures, axes
 
     else:
         # Save as nii file
         if ".nii" in filename:
             _logger.info(f"Saving {filename}")
             nii = nib.Nifti1Image(power_map, mask.affine, mask.header)
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/regression.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/regression.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/spectral.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/spectral.py`

 * *Files 0% similar despite different names*

```diff
@@ -1369,14 +1369,17 @@
             + f"len(alpha)={len(alpha)}."
         )
 
     for i in range(len(alpha)):
         if alpha[i].shape[1] != psd[i].shape[1]:
             raise ValueError("psd and alpha must have same number of modes.")
 
+    # Prevent in-place operation
+    psd = psd.copy()
+
     # Number of subjects
     n_subjects = len(alpha)
 
     # Window alphas to match the windowing of STFT
     for i, a in enumerate(alpha):
         alpha[i] = window_mean(
             a, window_length, step_size=step_size, n_sub_windows=n_sub_windows
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/static.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/static.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/statistics.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/statistics.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,25 +20,32 @@
     for k, v in covariates.items():
         if v.shape[0] != n_subjects:
             raise ValueError(
                 f"Got covariates['{k}'].shape[0]={v.shape[0]}, "
                 + f"but was expecting {n_subjects}."
             )
 
+    # Convert covariates to a numpy array
+    if len(covariates) > 0:
+        covariates_data = np.array(list(covariates.values())).T
+
     # Remove subjects with a nan in either array
     remove = []
-    glm_data = np.array(list(covariates.values()))
-    glm_data = np.concatenate([glm_data.T, data], axis=-1)
     for i in range(n_subjects):
-        if np.isnan(glm_data[i]).any():
-            _logger.warn(f"Removing subject {i} from GLM.")
+        if np.isnan(data[i]).any():
             remove.append(i)
+        if len(covariates) > 0:
+            if np.isnan(covariates_data[i]).any():
+                remove.append(i)
         if assignments is not None:
             if np.isnan(assignments[i]):
                 remove.append(i)
+    remove = np.unique(remove)
+    if len(remove) > 0:
+        _logger.warn(f"The following subjects were removed from the GLM: {remove}")
 
     # Keep subjects without nans
     keep = [i for i in range(n_subjects) if i not in remove]
     data = np.copy(data)[keep]
     covariates_ = {}
     for key in covariates:
         covariates_[key] = covariates[key][keep]
@@ -51,15 +58,17 @@
 
     if assignments is not None:
         return data, covariates_, assignments
     else:
         return data, covariates_
 
 
-def evoked_response_max_stat_perm(data, n_perm, covariates={}, n_jobs=1):
+def evoked_response_max_stat_perm(
+    data, n_perm, covariates={}, metric="copes", n_jobs=1
+):
     """Statistical significant testing for evoked responses.
 
     This function fits a General Linear Model (GLM) with ordinary least squares
     and performs a sign flip permutations test with the maximum statistic to
     determine a p-value for evoked responses.
 
     Parameters
@@ -67,22 +76,27 @@
     data : np.ndarray
         Baseline corrected evoked responses. This will be the target data for the GLM.
         Must be shape (n_subjects, n_samples, n_modes).
     n_perm : int
         Number of permutations.
     covariates : dict
         Covariates (extra regressors) to add to the GLM fit. These will be z-transformed.
+    metric : str
+        Metric to use to build the null distribution. Can be 'tstats' or 'copes'.
     n_jobs : int
         Number of processes to run in parallel.
 
     Returns
     -------
     pvalues : np.ndarray
         P-values for the evoked response. Shape is (n_subjects, n_samples, n_modes).
     """
+    if metric not in ["tstats", "copes"]:
+        raise ValueError("metric must be 'tstats' or 'copes'.")
+
     if not isinstance(data, np.ndarray):
         raise ValueError("data must be a numpy array.")
     if data.ndim != 3:
         raise ValueError("data must be (n_subjects, n_samples, n_modes).")
 
     data, covariates = _check_glm_data(data, covariates)
 
@@ -99,43 +113,51 @@
         DC.add_regressor(name=name, rtype="Parametric", datainfo=name, preproc="z")
     DC.add_regressor(name="Mean", rtype="Constant")
     DC.add_contrast(name="Mean", values=[1] + [0] * len(covariates))
     design = DC.design_from_datainfo(data.info)
 
     # Fit model and get t-statistics
     model = glm.fit.OLSModel(design, data)
-    tstats = abs(model.tstats[0])
 
     # Run permutations and get null distribution
     perm = glm.permutations.MaxStatPermutation(
         design,
         data,
         contrast_idx=0,  # selects the Mean contrast
         nperms=n_perm,
-        metric="tstats",
+        metric=metric,
         tail=0,  # two-sided test
         pooled_dims=(1, 2),  # pool over samples and modes dimension
         nprocesses=n_jobs,
     )
     null_dist = perm.nulls
 
     # Get p-values
-    percentiles = stats.percentileofscore(null_dist, tstats)
+    if metric == "tstats":
+        print("Using tstats as metric")
+        tstats = abs(model.tstats[0])
+        percentiles = stats.percentileofscore(null_dist, tstats)
+    elif metric == "copes":
+        print("Using copes as metric")
+        copes = abs(model.copes[0])
+        percentiles = stats.percentileofscore(null_dist, copes)
     pvalues = 1 - percentiles / 100
 
     if np.all(pvalues < 0.05):
         _logger.warn(
             "All time points for all modes are significant with p-value<0.05. "
             + "Did you remember to baseline correct the evoked responses?"
         )
 
     return pvalues
 
 
-def group_diff_max_stat_perm(data, assignments, n_perm, covariates={}, n_jobs=1):
+def group_diff_max_stat_perm(
+    data, assignments, n_perm, covariates={}, metric="tstats", n_jobs=1
+):
     """Statistical significant testing for the difference between two groups.
 
     This function fits a General Linear Model (GLM) with ordinary least squares
     and performs a row shuffle permutations test with the maximum statistic to
     determine a p-value for differences between two groups.
 
     Parameters
@@ -147,14 +169,16 @@
         1D numpy array containing group assignments. A value of 1 indicates
         Group1 and a value of 2 indicates Group2. Note, we test the contrast
         abs(Group1 - Group2) > 0.
     n_perm : int
         Number of permutations.
     covariates : dict
         Covariates (extra regressors) to add to the GLM fit. These will be z-transformed.
+    metric : str
+        Metric to use to build the null distribution. Can be 'tstats' or 'copes'.
     n_jobs : int
         Number of processes to run in parallel.
 
     Returns
     -------
     group_diff : np.ndarray
         Group difference: Group1 - Group2. Shape is (features1, features2, ...).
@@ -163,14 +187,17 @@
     """
     if not isinstance(data, np.ndarray):
         raise ValueError("data must be a numpy array.")
     ndim = data.ndim
     if ndim == 1:
         raise ValueError("data must be 2D or greater.")
 
+    if metric not in ["tstats", "copes"]:
+        raise ValueError("metric must be 'tstats' or 'copes'.")
+
     data, covariates, assignments = _check_glm_data(data, covariates, assignments)
 
     # Calculate group difference
     group1_mean = np.mean(data[assignments == 1], axis=0)
     group2_mean = np.mean(data[assignments == 2], axis=0)
     group_diff = group1_mean - group2_mean
 
@@ -189,33 +216,39 @@
     for name in covariates:
         DC.add_regressor(name=name, rtype="Parametric", datainfo=name, preproc="z")
     DC.add_contrast(name="GroupDiff", values=[1, -1] + [0] * len(covariates))
     design = DC.design_from_datainfo(data.info)
 
     # Fit model and get t-statistics
     model = glm.fit.OLSModel(design, data)
-    tstats = abs(model.tstats[0])
 
     # Which dimensions are we pooling over?
     if ndim == 2:
         pooled_dims = 1
     else:
         pooled_dims = tuple(range(1, ndim))
 
     # Run permutations and get null distribution
     perm = glm.permutations.MaxStatPermutation(
         design,
         data,
         contrast_idx=0,  # selects GroupDiff
         nperms=n_perm,
-        metric="tstats",
+        metric=metric,
         tail=0,  # two-sided test
         pooled_dims=pooled_dims,
         nprocesses=n_jobs,
     )
     null_dist = perm.nulls
 
     # Get p-values
-    percentiles = stats.percentileofscore(null_dist, tstats)
+    if metric == "tstats":
+        print("Using tstats as metric")
+        tstats = abs(model.tstats[0])
+        percentiles = stats.percentileofscore(null_dist, tstats)
+    elif metric == "copes":
+        print("Using copes as metric")
+        copes = abs(model.copes[0])
+        percentiles = stats.percentileofscore(null_dist, copes)
     pvalues = 1 - percentiles / 100
 
     return group_diff, pvalues
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/analysis/workbench.py` & `osl-dynamics-1.2.3/osl_dynamics/analysis/workbench.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/array_ops.py` & `osl-dynamics-1.2.3/osl_dynamics/array_ops.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     """
     if values.ndim == 2:
         values = values.argmax(axis=1)
     if n_states is None:
         n_states = values.max() + 1
     res = np.eye(n_states)[np.array(values).reshape(-1)]
-    return res.reshape(list(values.shape) + [n_states])
+    return res.reshape([*list(values.shape), n_states]).astype(int)
 
 
 def align_arrays(*sequences, alignment="left"):
     """Given a list of sequences, return the sequences trimmed to equal length.
 
     Given a list of sequences of unequal length, remove either the start, end or a
     portion of both the start and end of the arrays such that their lengths are equal
@@ -261,7 +261,119 @@
             rtol=0,
             atol=precision,
             equal_nan=True,
         ),
         axis=(-1, -2),
     )
     return symmetry
+
+
+def ezclump(binary_array):
+    """Find the clumps (groups of data with the same values) for a 1D bool array.
+
+    Returns a series of slices.
+    Taken wholesale from numpy.ma.extras.ezclump.
+    """
+    if binary_array.ndim > 1:
+        binary_array = binary_array.ravel()
+    idx = (binary_array[1:] ^ binary_array[:-1]).nonzero()
+    idx = idx[0] + 1
+
+    if binary_array[0]:
+        if len(idx) == 0:
+            return [slice(0, binary_array.size)]
+
+        r = [slice(0, idx[0])]
+        r.extend((slice(left, right) for left, right in zip(idx[1:-1:2], idx[2::2])))
+    else:
+        if len(idx) == 0:
+            return []
+
+        r = [slice(left, right) for left, right in zip(idx[:-1:2], idx[1::2])]
+
+    if binary_array[-1]:
+        r.append(slice(idx[-1], binary_array.size))
+    return r
+
+
+def slice_length(slice_):
+    """Return the length of a slice.
+
+    Parameters
+    ----------
+    slice_ : slice
+        Slice.
+
+    Returns
+    -------
+    length : int
+    """
+    return slice_.stop - slice_.start
+
+
+def apply_to_lists(list_of_lists, func, check_empty=True):
+    """Apply a function to each list in a list of lists.
+
+    Parameters
+    ----------
+    list_of_lists : list of list
+        List of lists.
+    func : callable
+        Function to apply to each list.
+    check_empty : bool
+        Return 0 for empty lists if set as True. If False, the function
+        will be applied to an empty list.
+
+    Returns
+    -------
+    result : np.ndarray
+        Numpy array with the function applied to each list.
+    """
+    if check_empty:
+        return np.array(
+            [
+                [
+                    func(inner_list) if np.any(inner_list) else 0
+                    for inner_list in subject_list
+                ]
+                for subject_list in list_of_lists
+            ],
+        )
+
+    return np.array(
+        [
+            [func(inner_list) for inner_list in subject_list]
+            for subject_list in list_of_lists
+        ],
+    )
+
+
+def list_means(list_of_lists):
+    """Calculate the mean of each list in a list of lists.
+
+    Parameters
+    ----------
+    list_of_lists : list of list
+        List of lists.
+
+    Returns
+    -------
+    result : np.ndarray
+        Numpy array with the mean of each list.
+    """
+    return apply_to_lists(list_of_lists, func=np.mean)
+
+
+def list_stds(list_of_lists):
+    """Calculate the standard deviation of each list in a list of lists.
+
+    Parameters
+    ----------
+    list_of_lists : list of list
+        List of lists.
+
+    Returns
+    -------
+    result : np.ndarray
+        Numpy array with the standard deviation of each list.
+    """
+    return apply_to_lists(list_of_lists, func=np.std)
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/config_api/wrappers.py` & `osl-dynamics-1.2.3/osl_dynamics/config_api/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """Wrapper functions for use in the config API.
 
-See the `toolbox examples
-<https://github.com/OHBA-analysis/osl-dynamics/tree/main/examples/toolbox_paper>`_
-for scripts that use the config API.
-
 All of the functions in this module can be listed in the config passed to
 :code:`osl_dynamics.run_pipeline`.
 
 All wrapper functions have the structure::
 
     func(data, output_dir, **kwargs)
 
 where:
 
-- :code:`data` is an :code:`osl_dynamics.data.Data` object
+- :code:`data` is an :code:`osl_dynamics.data.Data` object.
 - :code:`output_dir` is the path to save output to.
 - :code:`kwargs` are keyword arguments for function specific options.
 """
 
 import os
 import logging
 from pathlib import Path
@@ -1213,19 +1209,19 @@
             kwargs["filename"] = f"{alphas_dir}/alpha_{i}.png"
             plotting.plot_alpha(alp[i], **kwargs)
     else:
         kwargs["filename"] = f"{alphas_dir}/alpha_{subject}.png"
         plotting.plot_alpha(alp[subject], **kwargs)
 
     if normalize:
+        from osl_dynamics.inference import modes
+
         # Calculate normalised alphas
         covs = load(f"{inf_params_dir}/covs.npy")
-        traces = np.trace(covs, axis1=1, axis2=2)
-        norm_alp = [a * traces[np.newaxis, :] for a in alp]
-        norm_alp = [na / np.sum(na, axis=1, keepdims=True) for na in norm_alp]
+        norm_alp = modes.reweight_alphas(alp)
 
         # Plot
         if subject == "all":
             for i in range(len(alp)):
                 kwargs["filename"] = f"{alphas_dir}/norm_alpha_{i}.png"
                 plotting.plot_alpha(norm_alp[i], **kwargs)
         else:
@@ -1285,14 +1281,17 @@
 
     - :code:`<output_dir>/inf_params`, which contains the inferred parameters.
 
     This function will create:
 
     - :code:`<output_dir>/summary_stats`, which contains plots of the summary statistics.
 
+    The :code:`<output_dir>/summary_stats` directory will also contain numpy files
+    with the summary statistics.
+
     Parameters
     ----------
     data : osl_dynamics.data.Data
         Data object.
     output_dir : str
         Path to output directory.
     use_gmm_alpha : bool
@@ -1337,14 +1336,20 @@
 
     # Calculate summary stats
     fo = modes.fractional_occupancies(stc)
     lt = modes.mean_lifetimes(stc, sampling_frequency)
     intv = modes.mean_intervals(stc, sampling_frequency)
     sr = modes.switching_rates(stc, sampling_frequency)
 
+    # Save summary stats
+    save(f"{summary_stats_dir}/fo.npy", fo)
+    save(f"{summary_stats_dir}/lt.npy", lt)
+    save(f"{summary_stats_dir}/intv.npy", intv)
+    save(f"{summary_stats_dir}/sr.npy", sr)
+
     # Plot
     from osl_dynamics.utils import plotting
 
     n_states = fo.shape[1]
     x = range(1, n_states + 1)
     plotting.plot_violin(
         fo.T,
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/data/base.py` & `osl-dynamics-1.2.3/osl_dynamics/data/base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/data/osl.py` & `osl-dynamics-1.2.3/osl_dynamics/data/osl.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/data/processing.py` & `osl-dynamics-1.2.3/osl_dynamics/data/processing.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/data/rw.py` & `osl-dynamics-1.2.3/osl_dynamics/data/rw.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/data/spm.py` & `osl-dynamics-1.2.3/osl_dynamics/data/spm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/data/task.py` & `osl-dynamics-1.2.3/osl_dynamics/data/task.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/data/tf.py` & `osl-dynamics-1.2.3/osl_dynamics/data/tf.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/__init__.py` & `osl-dynamics-1.2.3/osl_dynamics/files/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/__init__.py` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/__init__.py` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/giles_39_binary.nii.gz` & `osl-dynamics-1.2.3/osl_dynamics/files/parcellation/giles_39_binary.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/ctf275_channel_names.npy` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/ctf275_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D148.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D148.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D248.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D248_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/4D248_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF151.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF275.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1005.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/EEG1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1010.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/EEG1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1020.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/EEG1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi128.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi16.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi160.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi256.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi32.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi64.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM1.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM1.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM10.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM10.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM11.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM11.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM14.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM14.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM15.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM15.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM16.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM17.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM17.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM20.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM20.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM22.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM22.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM23.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM23.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM24.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM24.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM25.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM25.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM3.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM3.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM7.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/easycapM7.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1005.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/elec1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1010.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/elec1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1020.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/elec1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122planar.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag122planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306mag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/quickcap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.outline` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/quickcap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440all.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scanner/neuromag306_channel_names.npy` & `osl-dynamics-1.2.3/osl_dynamics/files/scanner/neuromag306_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/files/scene/mode_scene.scene` & `osl-dynamics-1.2.3/osl_dynamics/files/scene/mode_scene.scene`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/inference/callbacks.py` & `osl-dynamics-1.2.3/osl_dynamics/inference/callbacks.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/inference/initializers.py` & `osl-dynamics-1.2.3/osl_dynamics/inference/initializers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/inference/layers.py` & `osl-dynamics-1.2.3/osl_dynamics/inference/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1156,28 +1156,33 @@
 
     def __init__(self, n_states, epsilon, **kwargs):
         super().__init__(**kwargs)
         self.n_states = n_states
         self.epsilon = epsilon
 
     def call(self, inputs, **kwargs):
-        x, mu, sigma, probs = inputs
-
+        x, mu, sigma, probs, subj_id = inputs
         # Add a small error for numerical stability
         sigma = add_epsilon(sigma, self.epsilon, diag=True)
 
+        if subj_id is not None:
+            subj_id = tf.cast(subj_id, tf.int32)
+            mu = tf.gather(mu, subj_id)
+            sigma = tf.gather(sigma, subj_id)
+
         # Log-likelihood for each state
         ll_loss = tf.zeros(shape=tf.shape(x)[:-1])
         for i in range(self.n_states):
             mvn = tfp.distributions.MultivariateNormalTriL(
-                loc=mu[i],
-                scale_tril=tf.linalg.cholesky(sigma[i]),
+                loc=tf.gather(mu, i, axis=-2),
+                scale_tril=tf.linalg.cholesky(tf.gather(sigma, i, axis=-3)),
                 allow_nan_stats=False,
             )
-            ll_loss += probs[:, :, i] * mvn.log_prob(x)
+            a = mvn.log_prob(x)
+            ll_loss += probs[:, :, i] * a
 
         # Sum over time dimension and average over the batch dimension
         ll_loss = tf.reduce_sum(ll_loss, axis=1)
         ll_loss = tf.reduce_mean(ll_loss, axis=0)
 
         # Add the negative log-likelihood to the loss
         nll_loss = -ll_loss
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/inference/metrics.py` & `osl-dynamics-1.2.3/osl_dynamics/inference/metrics.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/inference/modes.py` & `osl-dynamics-1.2.3/osl_dynamics/inference/modes.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from pathlib import Path
 
 import mne
 import numpy as np
 import matplotlib.pyplot as plt
 from tqdm.auto import trange
 from scipy.optimize import linear_sum_assignment
+from scipy.cluster import hierarchy
+from sklearn.cluster import AgglomerativeClustering
 
 from osl_dynamics import analysis, array_ops
 from osl_dynamics.inference import metrics
 from osl_dynamics.utils import plotting
 from osl_dynamics.utils.misc import override_dict_defaults
 
 
@@ -448,7 +450,127 @@
                 raw.info["sfreq"],
                 [extra_chan] * chan_data.shape[0],
             )
             chan_raw = mne.io.RawArray(chan_data, chan_info, verbose=verbose)
             alpha_raw.add_channels([chan_raw], force_update_info=True)
 
     return alpha_raw
+
+
+def reweight_alphas(alpha, covs):
+    """Re-weight DyNeMo mixing coefficients to account for the magnitude of
+    the mode covariances.
+
+    Parameters
+    ----------
+    alpha : list of np.ndarray or np.ndarray
+        Raw alphas from DyNeMo. Shape must be (n_subjects, n_samples, n_modes)
+        or (n_samples, n_modes).
+    covs : np.ndarray
+        Mode covariances. Shape must be (n_modes, n_channels, n_channels).
+
+    Returns
+    -------
+    reweighted_alpha : list of np.ndarray or np.ndarray
+        Re-weighted alphas. Shape is the same as alpha.
+    """
+    if isinstance(alpha, np.ndarray):
+        alpha = [alpha]
+
+    # Calculate normalised alphas
+    traces = np.trace(covs, axis1=1, axis2=2)
+    reweighted_alpha = [a * traces[np.newaxis, :] for a in alpha]
+    reweighted_alpha = [
+        na / np.sum(na, axis=1, keepdims=True) for na in reweighted_alpha
+    ]
+
+    if len(reweighted_alpha) == 1:
+        reweighted_alpha = reweighted_alpha[0]
+
+    return reweighted_alpha
+
+
+def average_runs(alpha, n_clusters=None, return_cluster_info=False):
+    """Average the state probabilities from different runs using hierarchical
+    clustering.
+
+    The hierarchical clustering used in this function is described `here
+    <https://www.biorxiv.org/content/10.1101/2023.01.18.524539v2>`_.
+
+    Parameters
+    ----------
+    alpha : list of list of np.ndarray or list of np.ndarray
+        State probabilities. Shape must be (n_runs, n_subjects, n_samples, n_states)
+        or (n_runs, n_samples, n_states).
+    n_clusters : int
+        Number of clusters to fit. Optional. Defaults to the largest number of
+        states in alpha.
+    return_cluster_info : bool
+        Should we return information describing the clustering?
+
+    Returns
+    -------
+    average_alpha : list of np.ndarray or np.ndarray
+        State probabilities averaged over runs. Shape is (n_subjects, n_states).
+    cluster_info : dict
+        Clustering info. Only returned if return_cluster_info=True.
+        This is a dictionary with keys 'correlation', 'dissimiarity', 'ids' and
+        'linkage'.
+    """
+    if not isinstance(alpha, list):
+        raise ValueError(
+            "alpha must be a list of lists (of numpy arrays) or list of numpy arrays."
+        )
+    if isinstance(alpha[0], np.ndarray):
+        alpha = [[a] for a in alpha]
+
+    # Number of runs and length of each subject's data
+    n_runs = len(alpha)
+    n_subject_samples = [a.shape[0] for a in alpha[0]]
+
+    # Use the largest number of states as the number of clusters to find
+    if n_clusters is None:
+        n_clusters = max([a.shape[-1] for a in alpha[0]])
+
+    # Concatenate over subjects, gives (n_runs, n_samples, n_states) array
+    alpha = [np.concatenate(a, axis=0) for a in alpha]
+
+    # Turn into a (n_runs * n_states, n_samples) array
+    alpha_ = []
+    for i in range(n_runs):
+        for j in range(alpha[i].shape[-1]):
+            alpha_.append(alpha[i][:, j])
+    alpha = np.array(alpha_, dtype=np.float32).T
+
+    # Calculate correlation between all pairwise state probability time courses
+    corr = np.corrcoef(alpha, rowvar=False)
+
+    # Convert correlation to a dis-similarity measure
+    dissimilarity = 1 - corr
+
+    # Hierarchical clustering
+    clustering = AgglomerativeClustering(n_clusters, linkage="ward")
+    cluster_ids = clustering.fit_predict(dissimilarity)
+
+    # Average alphas in each cluster
+    average_alpha = []
+    for i in range(n_clusters):
+        a = np.mean(alpha[:, cluster_ids == i], axis=-1)
+        average_alpha.append(a)
+    average_alpha = np.array(average_alpha, dtype=np.float32).T
+
+    # Split average alphas back into subject-specific time courses
+    average_alpha = np.split(average_alpha, np.cumsum(n_subject_samples[:-1]))
+
+    if return_cluster_info:
+        # Create a dictionary containing the clustering info
+        linkage = hierarchy.linkage(dissimilarity, method="ward")
+        cluster_info = {
+            "correlation": corr,
+            "dissimilarity": dissimilarity,
+            "ids": cluster_ids,
+            "linkage": linkage,
+        }
+        return average_alpha, cluster_info
+
+    else:
+        return average_alpha
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/inference/regularizers.py` & `osl-dynamics-1.2.3/osl_dynamics/inference/regularizers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/inference/tf_ops.py` & `osl-dynamics-1.2.3/osl_dynamics/inference/tf_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/__init__.py` & `osl-dynamics-1.2.3/osl_dynamics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/dynemo.py` & `osl-dynamics-1.2.3/osl_dynamics/models/dynemo.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/dynemo_obs.py` & `osl-dynamics-1.2.3/osl_dynamics/models/dynemo_obs.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/hmm.py` & `osl-dynamics-1.2.3/osl_dynamics/models/hmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,16 @@
     # Observation model parameters
     learn_means: bool = None
     learn_covariances: bool = None
     initial_means: np.ndarray = None
     initial_covariances: np.ndarray = None
     diagonal_covariances: bool = False
     covariances_epsilon: float = None
+    means_regularizer: tf.keras.regularizers.Regularizer = None
+    covariances_regularizer: tf.keras.regularizers.Regularizer = None
 
     initial_trans_prob: np.ndarray = None
     learn_trans_prob: bool = True
     state_probs_t0: np.ndarray = None
 
     # Learning rate schedule parameters
     trans_prob_update_delay: float = 5  # alpha
@@ -381,34 +383,37 @@
             return
 
         _logger.info(f"Using initialization {best_initialization}")
         self.set_weights(best_weights, best_trans_prob)
 
         return best_history
 
-    def _get_state_probs(self, x):
+    def _get_state_probs(self, x, subj_id=None):
         """Get state probabilities.
 
         Parameters
         ----------
         x : np.ndarray
             Observed data. Shape is (batch_size, sequence_length, n_channels).
+        subj_id : np.ndarray
+            Subject ID. Shape is (batch_size, sequence_length).
+            Only used in osl_dynamics.models.sehmm.
 
         Returns
         -------
         gamma : np.ndarray
             Marginal posterior distribution of hidden states given the data, q(s_t).
             Shape is (batch_size*sequence_length, n_states).
         xi : np.ndarray
             Joint posterior distribution of hidden states at two consecutive time points,
             q(s_t, s_t+1). Shape is (batch_size*sequence_length-1, n_states*n_states).
         """
 
         # Use Baum-Welch algorithm to calculate gamma, xi
-        B = self._get_likelihood(x)
+        B = self._get_likelihood(x, subj_id)
         Pi_0 = self.state_probs_t0
         P = self.trans_prob
 
         gamma, xi = self._baum_welch(B, Pi_0, P)
 
         return gamma, xi
 
@@ -466,41 +471,51 @@
         b = beta[1:] * B[:, 1:].T
         t = P * np.expand_dims(alpha[:-1], axis=2) * np.expand_dims(b, axis=1)
         xi = t.reshape(n_samples - 1, -1, order="F")
         xi /= np.expand_dims(np.sum(xi, axis=1), axis=1) + EPS
 
         return gamma, xi
 
-    def _get_likelihood(self, x):
+    def _get_likelihood(self, x, subj_id=None):
         """Get the likelihood, p(x_t | s_t).
 
         Parameters
         ----------
         x : np.ndarray
             Observed data. Shape is (batch_size, sequence_length, n_channels).
+        subj_id : np.ndarray
+            Subject ID. Shape is (batch_size, sequence_length).
+            Only used in for osl_dynamics.models.sehmm
 
         Returns
         -------
         likelihood : np.ndarray
             Likelihood. Shape is (n_states, batch_size*sequence_length).
         """
         # Get the current observation model parameters
-        means, covs = self.get_means_covariances()
+        if subj_id is None:
+            means, covs = self.get_means_covariances()
+            n_states = means.shape[0]
+        else:
+            means, covs = self.get_subject_means_covariances()
+            n_states = means.shape[1]
+            subj_id = tf.cast(subj_id, tf.int32)
+            means = tf.gather(means, subj_id)
+            covs = tf.gather(covs, subj_id)
 
-        n_states = means.shape[0]
         batch_size = x.shape[0]
         sequence_length = x.shape[1]
 
         # Calculate the log-likelihood for each state to have generated the
         # observed data
         log_likelihood = np.empty([n_states, batch_size, sequence_length])
         for state in range(n_states):
             mvn = tfp.distributions.MultivariateNormalTriL(
-                loc=means[state],
-                scale_tril=tf.linalg.cholesky(covs[state]),
+                loc=tf.gather(means, state, axis=-2),
+                scale_tril=tf.linalg.cholesky(tf.gather(covs, state, axis=-3)),
                 allow_nan_stats=False,
             )
             log_likelihood[state] = mvn.log_prob(x)
         log_likelihood = log_likelihood.reshape(n_states, batch_size * sequence_length)
 
         # We add a constant to the log-likelihood for time points where all states
         # have a negative log-likelihood. This is critical for numerical stability.
@@ -584,15 +599,15 @@
         first_term = np.sum(xlogy(xi, xi))
 
         # second_term = sum^{T-1}_t=2 int q(s_t) log q(s_t) ds_t
         second_term = np.sum(xlogy(gamma, gamma)[1:-1])
 
         return first_term - second_term
 
-    def _get_posterior_expected_log_likelihood(self, x, gamma):
+    def _get_posterior_expected_log_likelihood(self, x, gamma, subj_id=None):
         """Expected log-likelihood.
 
         Calculates the expected log-likelihood with respect to the posterior
         distribution of the states:
 
         .. math::
             LL &= \int q(s_{1:T}) \log \prod_{t=1}^T p(x_t | s_t) ds_{1:T}
@@ -602,22 +617,25 @@
         Parameters
         ----------
         x : np.ndarray
             Data. Shape is (batch_size, sequence_length, n_channels).
         gamma : np.ndarray
             Marginal posterior distribution of hidden states given the data, q(s_t).
             Shape is (batch_size*sequence_length, n_states).
+        subj_id : np.ndarray
+            Subject ID. Shape is (batch_size, sequence_length).
+            Only used in osl_dynamics.models.sehmm
 
         Returns
         -------
         log_likelihood : float
             Posterior expected log-likelihood.
         """
         gamma = np.reshape(gamma, (x.shape[0], x.shape[1], -1))
-        log_likelihood = self._get_log_likelihood(x)
+        log_likelihood = self._get_log_likelihood(x, subj_id)
         return tf.reduce_sum(log_likelihood * gamma)
 
     def _get_posterior_expected_prior(self, gamma, xi):
         """Posterior expected prior.
 
         Calculates the expected prior probability of states with respect to the
         posterior distribution of the states:
@@ -676,59 +694,72 @@
         log_trans_prob = np.expand_dims(np.log(self.trans_prob), 0)
         log_smoothing_distribution = np.expand_dims(log_smoothing_distribution, -1)
         log_prediction_distribution = logsumexp(
             log_trans_prob + log_smoothing_distribution, -2
         )
         return log_prediction_distribution
 
-    def _get_log_likelihood(self, data):
+    def _get_log_likelihood(self, data, subj_id=None):
         """Get the log-likelihood of data, log p(x_t | s_t).
 
         Parameters
         ----------
         data : np.ndarray
             Data. Shape is (batch_size, ..., n_channels).
+        subj_id : np.ndarray
+            Subject ID. Shape is (batch_size, ...).
+            Only used in osl_dynamics.models.sehmm
 
         Returns
         -------
         log_likelihood : np.ndarray
             Log-likelihood. Shape is (batch_size, ..., n_states)
         """
-        means, covs = self.get_means_covariances()
+        if subj_id is None:
+            means, covs = self.get_means_covariances()
+        else:
+            means, covs = self.get_subject_means_covariances()
+            subj_id = tf.cast(subj_id, tf.int32)
+            means = tf.gather(means, subj_id)
+            covs = tf.gather(covs, subj_id)
+
         mvn = tfp.distributions.MultivariateNormalTriL(
             loc=means,
             scale_tril=tf.linalg.cholesky(covs),
             allow_nan_stats=False,
         )
         log_likelihood = mvn.log_prob(tf.expand_dims(data, axis=-2))
         return log_likelihood.numpy()
 
-    def _evidence_update_step(self, data, log_prediction_distribution):
+    def _evidence_update_step(self, data, log_prediction_distribution, subj_id=None):
         """Update step for calculating the evidence.
 
         .. math::
             p(s_t = j | x_{1:t}) &= \displaystyle\\frac{p(x_t | s_t = j) p(s_t = j | x_{1:t-1})}{p(x_t | x_{1:t-1})}
 
             p(x_t | x_{1:t-1}) &= \displaystyle\sum_i p(x_t | s_t = j) p(s_t = i | x_{1:t-1})
 
         Parameters
         ----------
         data : np.ndarray
             Data for the update step. Shape is (batch_size, n_channels).
         log_prediction_distribution : np.ndarray
             log p(s_t | x_1:t-1). Shape is (batch_size, n_states).
+        subj_id : np.ndarray
+            Subject ID. Shape is (batch_size,).
+            Only used in osl_dynamics.models.sehmm
 
         Returns
         -------
         log_smoothing_distribution : np.ndarray
             log p(s_t | x_1:t). Shape is (batch_size, n_states).
         predictive_log_likelihood : np.ndarray
             log p(x_t | x_1:t-1). Shape is (batch_size).
         """
-        log_likelihood = self._get_log_likelihood(data)
+        log_likelihood = self._get_log_likelihood(data, subj_id)
         log_smoothing_distribution = log_likelihood + log_prediction_distribution
         predictive_log_likelihood = logsumexp(log_smoothing_distribution, -1)
 
         # Normalise the log smoothing distribution
         log_smoothing_distribution -= np.expand_dims(predictive_log_likelihood, -1)
         return log_smoothing_distribution, predictive_log_likelihood
 
@@ -1146,37 +1177,40 @@
 
     # Definition of layers
     means_layer = VectorsLayer(
         config.n_states,
         config.n_channels,
         config.learn_means,
         config.initial_means,
+        config.means_regularizer,
         name="means",
     )
     if config.diagonal_covariances:
         covs_layer = DiagonalMatricesLayer(
             config.n_states,
             config.n_channels,
             config.learn_covariances,
             config.initial_covariances,
             config.covariances_epsilon,
+            config.covariances_regularizer,
             name="covs",
         )
     else:
         covs_layer = CovarianceMatricesLayer(
             config.n_states,
             config.n_channels,
             config.learn_covariances,
             config.initial_covariances,
             config.covariances_epsilon,
+            config.covariances_regularizer,
             name="covs",
         )
     ll_loss_layer = CategoricalLogLikelihoodLossLayer(
         config.n_states, config.covariances_epsilon, name="ll_loss"
     )
 
     # Data flow
     mu = means_layer(data)  # data not used
     D = covs_layer(data)  # data not used
-    ll_loss = ll_loss_layer([data, mu, D, gamma])
+    ll_loss = ll_loss_layer([data, mu, D, gamma, None])
 
     return tf.keras.Model(inputs=inputs, outputs=[ll_loss], name="HMM-Obs")
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/inf_mod_base.py` & `osl-dynamics-1.2.3/osl_dynamics/models/inf_mod_base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/mage.py` & `osl-dynamics-1.2.3/osl_dynamics/models/mage.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/mdynemo.py` & `osl-dynamics-1.2.3/osl_dynamics/models/mdynemo.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/mdynemo_obs.py` & `osl-dynamics-1.2.3/osl_dynamics/models/mdynemo_obs.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/mod_base.py` & `osl-dynamics-1.2.3/osl_dynamics/models/mod_base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/sage.py` & `osl-dynamics-1.2.3/osl_dynamics/models/sage.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/sedynemo.py` & `osl-dynamics-1.2.3/osl_dynamics/models/sedynemo.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     ModelRNNLayer,
     NormalizationLayer,
     KLDivergenceLayer,
     KLLossLayer,
     SampleNormalDistributionLayer,
     SampleGammaDistributionLayer,
     SoftmaxLayer,
-    ConcatenateLayer,
     ConcatEmbeddingsLayer,
     SubjectMapLayer,
     MixSubjectSpecificParametersLayer,
     TFRangeLayer,
     ZeroLayer,
     InverseCholeskyLayer,
     StaticKLDivergenceLayer,
@@ -251,25 +250,50 @@
         """Builds a keras model."""
         self.model = _model_structure(self.config)
 
     def make_dataset(self, inputs, shuffle=False, concatenate=False, subj_id=True):
         """SE-DyNeMo requires subject id to be included in the dataset."""
         return super().make_dataset(inputs, shuffle, concatenate, subj_id)
 
+    def fit(self, training_data, *args, **kwargs):
+        # Set Bayesian KL scaling
+        self.set_bayesian_kl_scaling(training_data)
+        return super().fit(training_data, *args, **kwargs)
+
+    def get_group_means(self):
+        """Get the group means.
+
+        Returns
+        -------
+        means : np.ndarray
+            Group means. Shape is (n_modes, n_channels).
+        """
+        return dynemo_obs.get_means(self.model, "group_means")
+
+    def get_group_covariances(self):
+        """Get the group covariances.
+
+        Returns
+        -------
+        covariances : np.ndarray
+            Group covariances. Shape is (n_modes, n_channels, n_channels).
+        """
+        return dynemo_obs.get_covariances(self.model, "group_covs")
+
     def get_group_means_covariances(self):
         """Get the group means and covariances of each mode
 
         Returns
         -------
         means : np.ndarray
             Mode means for the group. Shape is (n_modes, n_channels).
         covariances : np.ndarray
             Mode covariances for the group. Shape is (n_modes, n_channels, n_channels).
         """
-        return sedynemo_obs.get_group_means_covs(self.model)
+        return sedynemo_obs.get_group_means_covariances(self.model)
 
     def get_observation_model_parameters(self):
         """Wrapper for get_group_means_covariances."""
         return self.get_group_means_covariances()
 
     def get_subject_embeddings(self):
         """Get the subject embedding vectors
@@ -296,15 +320,15 @@
         -------
         subject_means : np.ndarray
             Mode means for each subject. Shape is (n_subjects, n_modes, n_channels).
         subject_covs : np.ndarray
             Mode covariances for each subject.
             Shape is (n_subjects, n_modes, n_channels, n_channels).
         """
-        return sedynemo_obs.get_subject_means_covs(
+        return sedynemo_obs.get_subject_means_covariances(
             self.model,
             self.config.learn_means,
             self.config.learn_covariances,
             subject_embeddings,
             n_neighbours,
         )
 
@@ -501,15 +525,15 @@
             config.dev_activation,
             config.dev_dropout,
             name="means_dev_map_input",
         )
         means_dev_map_layer = layers.Dense(config.n_channels, name="means_dev_map")
 
         norm_means_dev_map_layer = layers.LayerNormalization(
-            axis=-1, scale=False, name="norm_means_dev_map"
+            axis=-1, name="norm_means_dev_map"
         )
 
         means_dev_mag_inf_alpha_input_layer = LearnableTensorLayer(
             shape=(config.n_subjects, config.n_modes, 1),
             learn=config.learn_means,
             initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
             name="means_dev_mag_inf_alpha_input",
@@ -587,15 +611,15 @@
             config.dev_dropout,
             name="covs_dev_map_input",
         )
         covs_dev_map_layer = layers.Dense(
             config.n_channels * (config.n_channels + 1) // 2, name="covs_dev_map"
         )
         norm_covs_dev_map_layer = layers.LayerNormalization(
-            axis=-1, scale=False, name="norm_covs_dev_map"
+            axis=-1, name="norm_covs_dev_map"
         )
 
         covs_dev_mag_inf_alpha_input_layer = LearnableTensorLayer(
             shape=(config.n_subjects, config.n_modes, 1),
             learn=config.learn_covariances,
             initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
             name="covs_dev_mag_inf_alpha_input",
@@ -697,28 +721,25 @@
         config.model_activation,
         config.model_n_layers,
         config.model_n_units,
         config.model_dropout,
         config.model_regularizer,
         name="mod_rnn",
     )
-    concatenate_layer = ConcatenateLayer(axis=2, name="model_concat")
     mod_mu_layer = layers.Dense(config.n_modes, name="mod_mu")
     mod_sigma_layer = layers.Dense(
         config.n_modes, activation="softplus", name="mod_sigma"
     )
     kl_div_layer = KLDivergenceLayer(config.theta_std_epsilon, name="kl_div")
 
     # Data flow
     model_input_dropout = model_input_dropout_layer(theta_norm)
     model_output = model_output_layer(model_input_dropout)
-    dynamic_subject_embeddings = subject_embeddings_layer(subj_id)
-    model_output_concat = concatenate_layer([model_output, dynamic_subject_embeddings])
-    mod_mu = mod_mu_layer(model_output_concat)
-    mod_sigma = mod_sigma_layer(model_output_concat)
+    mod_mu = mod_mu_layer(model_output)
+    mod_sigma = mod_sigma_layer(model_output)
     kl_div = kl_div_layer([inf_mu, inf_sigma, mod_mu, mod_sigma])
 
     # For the observation model (static KL loss)
     if config.learn_means:
         # Layer definitions
         means_dev_mag_mod_beta_input_layer = MultiLayerPerceptronLayer(
             config.dev_n_layers,
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/sedynemo_obs.py` & `osl-dynamics-1.2.3/osl_dynamics/models/sedynemo_obs.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,34 +149,54 @@
 
 
 class Model(ModelBase):
     """Observation model for directional SE-DyNeMo
 
     Parameters
     ----------
-    config : osl_dynamics.models.directional_sedynemo_obs.Config
+    config : osl_dynamics.models.sedynemo_obs.Config
     """
 
     config_type = Config
 
     def build_model(self):
         """Builds a keras model."""
         self.model = _model_structure(self.config)
 
-    def get_group_means_covs(self):
+    def get_group_means(self):
+        """Get the group means.
+
+        Returns
+        -------
+        means : np.ndarray
+            Group means. Shape is (n_modes, n_channels).
+        """
+        return dynemo_obs.get_means(self.model, "group_means")
+
+    def get_group_covariances(self):
+        """Get the group covariances.
+
+        Returns
+        -------
+        covariances : np.ndarray
+            Group covariances. Shape is (n_modes, n_channels, n_channels).
+        """
+        return dynemo_obs.get_covariances(self.model, "group_covs")
+
+    def get_group_means_covariances(self):
         """Get the group means and covariances of each mode.
 
         Returns
         -------
         means : np.ndarray
             Mode means for the group. Shape is (n_modes, n_channels).
         covariances : np.ndarray
             Mode covariances for the group. Shape is (n_modes, n_channels, n_channels).
         """
-        return get_group_means_covs(self.model)
+        return get_group_means_covariances(self.model)
 
     def get_subject_embeddings(self):
         """Get the subject embedding vectors.
 
         Returns
         -------
         subject_embeddings : np.ndarray
@@ -197,15 +217,15 @@
         Returns
         -------
         subject_means : np.ndarray
             Mode means for each subject. Shape is (n_subjects, n_modes, n_channels).
         subject_covs : np.ndarray
             Mode covariances for each subject. Shape is (n_subjects, n_modes, n_channels, n_channels).
         """
-        return get_subject_means_covs(
+        return get_subject_means_covariances(
             self.model,
             self.config.learn_means,
             self.config.learn_covariances,
             subject_embeddings,
             n_neighbours,
         )
 
@@ -217,14 +237,16 @@
         covariances matrices with nu=n_channels - 1 + 0.1 and psi=diag(range).
 
         Parameters
         ----------
         training_data : tensorflow.data.Dataset
             Training dataset.
         """
+        training_dataset = self.make_dataset(training_dataset, concatenate=True)
+
         if self.config.learn_means:
             dynemo_obs.set_means_regularizer(
                 self.model, training_dataset, layer_name="group_means"
             )
 
         if self.config.learn_covariances:
             dynemo_obs.set_covariances_regularizer(
@@ -525,15 +547,14 @@
             config.dev_activation,
             config.dev_dropout,
             name="means_dev_mag_mod_beta_input",
         )
         means_dev_mag_mod_beta_layer = layers.Dense(
             1,
             activation="softplus",
-            use_bias=False,
             name="means_dev_mag_mod_beta",
         )
 
         means_dev_mag_kl_loss_layer = StaticKLDivergenceLayer(
             config.covariances_epsilon, name="means_dev_mag_kl_loss"
         )
 
@@ -565,15 +586,14 @@
             config.dev_activation,
             config.dev_dropout,
             name="covs_dev_mag_mod_beta_input",
         )
         covs_dev_mag_mod_beta_layer = layers.Dense(
             1,
             activation="softplus",
-            use_bias=False,
             name="covs_dev_mag_mod_beta",
         )
 
         covs_dev_mag_kl_loss_layer = StaticKLDivergenceLayer(
             config.covariances_epsilon, name="covs_dev_mag_kl_loss"
         )
 
@@ -604,21 +624,19 @@
     return tf.keras.Model(
         inputs=[data, alpha, subj_id],
         outputs=[ll_loss, kl_loss],
         name="Se_DyNeMo-Obs",
     )
 
 
-def get_group_means_covs(model):
-    group_means_layer = model.get_layer("group_means")
-    group_covs_layer = model.get_layer("group_covs")
-
-    group_means = group_means_layer(1)
-    group_covs = group_covs_layer(1)
-    return group_means.numpy(), group_covs.numpy()
+def get_group_means_covariances(model):
+    """Wrapper for getting the group level means and covariances."""
+    group_means = dynemo_obs.get_means(model, "group_means")
+    group_covariances = dynemo_obs.get_covariances(model, "group_covs")
+    return group_means, group_covariances
 
 
 def get_subject_embeddings(model):
     subject_embeddings_layer = model.get_layer("subject_embeddings")
     n_subjects = subject_embeddings_layer.input_dim
     return subject_embeddings_layer(np.arange(n_subjects)).numpy()
 
@@ -727,40 +745,40 @@
         covs_dev = covs_dev_layer([covs_dev_mag, covs_dev_map])
     else:
         covs_dev = covs_dev_layer(1)
 
     return means_dev.numpy(), covs_dev.numpy()
 
 
-def get_subject_means_covs(
+def get_subject_means_covariances(
     model, learn_means, learn_covariances, subject_embeddings=None, n_neighbours=2
 ):
-    group_means, group_covs = get_group_means_covs(model)
+    group_means, group_covs = get_group_means_covariances(model)
     means_dev, covs_dev = get_subject_dev(
         model, learn_means, learn_covariances, subject_embeddings, n_neighbours
     )
 
     subject_means_layer = model.get_layer("subject_means")
     subject_covs_layer = model.get_layer("subject_covs")
 
     mu = subject_means_layer([group_means, means_dev])
     D = subject_covs_layer([group_covs, covs_dev])
     return mu.numpy(), D.numpy()
 
 
 def _get_means_mode_embeddings(model):
-    group_means, _ = get_group_means_covs(model)
+    group_means, _ = get_group_means_covariances(model)
     means_mode_embeddings_layer = model.get_layer("means_mode_embeddings")
     means_mode_embeddings = means_mode_embeddings_layer(group_means)
     return means_mode_embeddings.numpy()
 
 
 def _get_covs_mode_embeddings(model):
     cholesky_bijector = tfb.Chain([tfb.CholeskyOuterProduct(), tfb.FillScaleTriL()])
-    _, group_covs = get_group_means_covs(model)
+    _, group_covs = get_group_means_covariances(model)
     covs_mode_embeddings_layer = model.get_layer("covs_mode_embeddings")
     covs_mode_embeddings = covs_mode_embeddings_layer(
         cholesky_bijector.inverse(group_covs)
     )
     return covs_mode_embeddings.numpy()
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/models/state_dynemo.py` & `osl-dynamics-1.2.3/osl_dynamics/models/state_dynemo.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/__init__.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/base.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/hmm.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/hmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/hsmm.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/hsmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/mar.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/mar.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/mvn.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/mvn.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/sin.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/sin.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/simulation/sm.py` & `osl-dynamics-1.2.3/osl_dynamics/simulation/sm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/utils/decorators.py` & `osl-dynamics-1.2.3/osl_dynamics/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/utils/misc.py` & `osl-dynamics-1.2.3/osl_dynamics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/utils/model.py` & `osl-dynamics-1.2.3/osl_dynamics/utils/model.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/utils/parcellation.py` & `osl-dynamics-1.2.3/osl_dynamics/utils/parcellation.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics/utils/plotting.py` & `osl-dynamics-1.2.3/osl_dynamics/utils/plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -248,19 +248,18 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (7, 4)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (7, 4)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     if plot_kwargs is None:
         plot_kwargs = {}
 
     # Create figure
     create_fig = ax is None
     if create_fig:
@@ -398,19 +397,18 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (7, 4)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (7, 4)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     if plot_kwargs is None:
         plot_kwargs = {}
 
     if len(x) > 10:
         colors = get_colors(len(x), colormap="tab20")
     else:
@@ -491,15 +489,15 @@
     x_label : str
         Label for x-axis.
     y_label : str
         Label for y-axis.
     title : str
         Figure title.
     plot_kwargs : dict
-        Arguments to pass to the ax.hist method.
+        Arguments to pass to the ax.hist method. Defaults to {"histtype": "step"}.
     fig_kwargs : dict
         Arguments to pass to plt.subplots.
     ax : matplotlib.axes.Axes
         Axis object to plot on.
     filename : str
         Output filename.
 
@@ -537,31 +535,32 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (7, 4)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (7, 4)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     if plot_kwargs is None:
         plot_kwargs = {}
+    default_plot_kwargs = {"histtype": "step"}
+    plot_kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
 
     # Create figure
     create_fig = ax is None
     if create_fig:
         fig, ax = create_figure(**fig_kwargs)
 
     # Plot histograms
     for d, b, l in zip(data, bins, labels):
-        ax.hist(d, bins=b, label=l, histtype="step")
+        ax.hist(d, bins=b, label=l, **plot_kwargs)
 
     # Set axis range
     ax.set_xlim(x_range[0], x_range[1])
     ax.set_ylim(y_range[0], y_range[1])
 
     # Set title and axis labels
     ax.set_title(title)
@@ -646,19 +645,18 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (7, 4)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (7, 4)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     if plot_kwargs is None:
         plot_kwargs = {}
 
     # Create figure
     create_fig = ax is None
     if create_fig:
@@ -691,15 +689,14 @@
     bins=50,
     legend_loc=1,
     x_range=None,
     y_range=None,
     x_label=None,
     y_label=None,
     title=None,
-    plot_kwargs=None,
     fig_kwargs=None,
     ax=None,
     filename=None,
 ):
     """Plot a two component Gaussian mixture model.
 
     Parameters
@@ -723,16 +720,14 @@
         Minimum and maximum for y-axis.
     x_label : str
         Label for x-axis.
     y_label : str
         Label for y-axis.
     title : str
         Figure title.
-    plot_kwargs : dict
-        Arguments to pass to the ax.hist method.
     fig_kwargs : dict
         Arguments to pass to plt.subplots.
     ax : matplotlib.axes.Axes
         Axis object to plot on.
     filename : str
         Output filename.
 
@@ -756,22 +751,18 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (7, 4)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
-
-    if plot_kwargs is None:
-        plot_kwargs = {}
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (7, 4)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     # Create figure
     create_fig = ax is None
     if create_fig:
         fig, ax = create_figure(**fig_kwargs)
 
     # Plot histogram
@@ -859,26 +850,28 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (7, 4)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (7, 4)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     # Create a pandas DataFrame
-    data_dict = {}
-    for x, d in zip(x, data):
-        data_dict[x] = []
-        for y in d:
-            data_dict[x].append(y)
+    # Pad the data with NaNs to make sure all columns have the same length
+    max_len = max([d.size for d in data])
+    data_dict = {
+        k: np.pad(
+            v, pad_width=(0, max_len - v.size), mode="constant", constant_values=np.nan
+        )
+        for k, v in zip(x, data)
+    }
     df = pd.DataFrame(data_dict)
 
     # Create figure
     create_fig = ax is None
     if create_fig:
         fig, ax = create_figure(**fig_kwargs)
 
@@ -916,14 +909,15 @@
         The number of time points to be plotted.
     y_tick_values:
         Labels for the channels to be placed on the y-axis.
     fig_kwargs : dict
         Keyword arguments to be passed on to matplotlib.pyplot.subplots.
     plot_kwargs : dict
         Keyword arguments to be passed on to matplotlib.pyplot.plot.
+        Defaults to {"lw": 0.7, "color": "tab:blue"}.
     ax : matplotlib.axes.Axes
         The axis on which to plot the data. If not given, a new axis is created.
     filename : str
         Output filename.
 
     Returns
     -------
@@ -942,25 +936,23 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (12, 8)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (12, 8)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
-    default_plot_kwargs = {"lw": 0.7, "color": "tab:blue"}
     if plot_kwargs is None:
-        plot_kwargs = default_plot_kwargs
-    else:
-        plot_kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
+        plot_kwargs = {}
+    default_plot_kwargs = {"lw": 0.7, "color": "tab:blue"}
+    plot_kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
 
     # Calculate separation
     separation = (
         np.maximum(time_series[:n_samples].max(), time_series[:n_samples].min()) * 1.2
     )
     gaps = np.arange(n_channels)[::-1] * separation
 
@@ -1010,39 +1002,38 @@
         Sampling frequency of the input data, enabling us to label the x-axis.
     n_samples : int
         Number of samples to be shown on the x-axis.
     fig_kwargs : dict
         Keyword arguments to be passed on to matplotlib.pyplot.subplots.
     plot_kwargs : dict
         Keyword arguments to be passed on to matplotlib.pyplot.plot.
+        Defaults to {"lw": 0.7}.
     filename : str
         Output filename.
 
     Returns
     -------
     fig : matplotlib.pyplot.figure
         Matplotlib figure object. Only returned if filename=None.
     ax : matplotlib.pyplot.axis.
         Matplotlib axis object(s). Only returned if filename=None.
     """
     time_series = np.asarray(time_series)
     n_samples = n_samples or min([ts.shape[0] for ts in time_series])
     n_lines = time_series[0].shape[1]
 
-    default_fig_kwargs = {"figsize": (20, 10), "sharex": "all"}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (20, 10), "sharex": "all"}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
-    default_plot_kwargs = {"lw": 0.7}
     if plot_kwargs is None:
-        plot_kwargs = default_plot_kwargs
-    else:
-        plot_kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
+        plot_kwargs = {}
+    default_plot_kwargs = {"lw": 0.7}
+    plot_kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
 
     if sampling_frequency is not None:
         time_vector = np.linspace(0, n_samples / sampling_frequency, n_samples)
     else:
         time_vector = np.linspace(0, n_samples, n_samples)
 
     # Create figure
@@ -1138,19 +1129,18 @@
             raise ValueError(
                 "Please use plotting.save() to save the figure instead of the "
                 + "filename argument."
             )
         if isinstance(ax, np.ndarray):
             raise ValueError("Only pass one axis.")
 
-    default_fig_kwargs = {"figsize": (16, 3)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (16, 3)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     if plot_kwargs is None:
         plot_kwargs = {}
 
     # Create figure
     create_fig = ax is None
     if create_fig:
@@ -1663,27 +1653,25 @@
     ]:
         cmap = plt.cm.get_cmap(name=cmap)
     else:
         cmap = plt.cm.get_cmap(name=cmap, lut=n_modes)
     colors = cmap.colors
 
     # Validation
+    if fig_kwargs is None:
+        fig_kwargs = {}
     default_fig_kwargs = dict(
         figsize=(12, 2.5 * n_alphas), sharex="all", facecolor="white"
     )
-    if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
-    default_plot_kwargs = dict(colors=colors)
     if plot_kwargs is None:
-        plot_kwargs = default_plot_kwargs
-    else:
-        plot_kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
+        plot_kwargs = {}
+    default_plot_kwargs = dict(colors=colors)
+    plot_kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
 
     if y_labels is None:
         y_labels = [None] * n_alphas
     elif isinstance(y_labels, str):
         y_labels = [y_labels] * n_alphas
     elif len(y_labels) != n_alphas:
         raise ValueError("Incorrect number of y_labels passed.")
@@ -1791,19 +1779,18 @@
 
     # Validation
     if mode_time_course.ndim == 1:
         mode_time_course = get_one_hot(mode_time_course)
     if mode_time_course.ndim != 2:
         raise ValueError("mode_timecourse must be a 2D array")
 
-    default_fig_kwargs = {"figsize": (long * 2.5, short * 2.5)}
     if fig_kwargs is None:
-        fig_kwargs = default_fig_kwargs
-    else:
-        fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (long * 2.5, short * 2.5)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
 
     if plot_kwargs is None:
         plot_kwargs = {}
 
     # Calculate mode lifetimes
     channel_lifetimes = modes.lifetimes(mode_time_course)
 
@@ -1955,15 +1942,15 @@
     # Create a pandas DataFrame to hold the summary stats
     ss_dict = {name: [], "State": [], "Group": []}
     n_subjects, n_states = summary_stats.shape
     for subject in range(n_subjects):
         for state in range(n_states):
             ss_dict[name].append(summary_stats[subject, state])
             ss_dict["State"].append(state + 1)
-            ss_dict["Group"].append(int(assignments[subject]))
+            ss_dict["Group"].append(assignments[subject])
     ss_df = pd.DataFrame(ss_dict)
 
     # Plot a half violin for each group
     sns.violinplot(data=ss_df, x="State", y=name, hue="Group", split=True)
 
     # Add a star above the violin to indicate significance
     scatter_kwargs = {"c": "black", "s": 32, "marker": "*"}
@@ -1974,7 +1961,130 @@
         elif pvalues[i] < 0.05:
             plt.scatter(i, summary_stats[:, i].max() * 1.6, **scatter_kwargs)
 
     # Save
     _logger.info(f"Saving {filename}")
     plt.savefig(filename)
     plt.close()
+
+
+def plot_evoked_response(
+    t,
+    epochs,
+    pvalues,
+    significance_level=0.05,
+    offset_between_bars=0.01,
+    labels=None,
+    legend_loc=1,
+    x_label=None,
+    y_label=None,
+    title=None,
+    fig_kwargs=None,
+    ax=None,
+    filename=None,
+):
+    """Plot an evoked responses with significant time points highlighted.
+
+    Parameters
+    ----------
+    t : np.ndarray
+        Time axis. Shape must be (n_samples,).
+    epochs : np.ndarray
+        Evoked responses. Shape must be (n_samples, n_channels).
+    pvalues : np.ndarray
+        p-value for each evoked response. This can be calculated with
+        `osl_dynamics.analysis.statistics.evoked_response_max_stat_perm
+        <https://osl-dynamics.readthedocs.io/en/latest/autoapi/osl_dynamics/analysis/statistics/index.html#osl_dynamics.analysis.statistics.evoked_response_max_stat_perm>`_.
+    significance_level : float
+        Value to threshold the p-values with to consider significant. By
+        default pvalues < 0.05 are significant.
+    offset_between_bars : float
+        Vertical offset between bars that highlight significance.
+    labels : list
+        Label for each evoked response time series.
+    legend_loc : int
+        Position of the legend.
+    x_label : str
+        Label for x-axis.
+    y_label : str
+        Label for y-axis.
+    title : str
+        Figure title.
+    fig_kwargs : dict
+        Arguments to pass to plt.subplots.
+    ax : matplotlib.axes.axes
+        Axis object to plot on.
+    filename : str
+        Output filename.
+
+    Returns
+    -------
+    fig : matplotlib.pyplot.figure
+        Matplotlib figure object. Only returned if filename=None.
+    ax : matplotlib.pyplot.axis.
+        Matplotlib axis object(s). Only returned if filename=None.
+    """
+
+    # Validation
+    if labels is not None:
+        if isinstance(labels, str):
+            labels = [labels]
+        else:
+            if len(labels) != epochs.shape[1]:
+                raise ValueError("Incorrect number of lines or labels passed.")
+        add_legend = True
+    else:
+        labels = [None] * epochs.shape[1]
+        add_legend = False
+
+    if ax is not None:
+        if filename is not None:
+            raise ValueError(
+                "Please use plotting.save() to save the figure instead of the "
+                + "filename argument."
+            )
+        if isinstance(ax, np.ndarray):
+            raise ValueError("Only pass one axis.")
+
+    if fig_kwargs is None:
+        fig_kwargs = {}
+    default_fig_kwargs = {"figsize": (7, 4)}
+    fig_kwargs = override_dict_defaults(default_fig_kwargs, fig_kwargs)
+
+    # Get significant time points for each channel
+    significant = pvalues < significance_level
+
+    # Create figure
+    create_fig = ax is None
+    if create_fig:
+        fig, ax = create_figure(**fig_kwargs)
+
+    for i, e, l, s in zip(range(epochs.shape[1]), epochs.T, labels, significant.T):
+        # Plot evoked response
+        p = ax.plot(t, e, label=l)
+
+        # Highlight significant time points
+        sig_times = t[s]
+        if len(sig_times) > 0:
+            y = 1.1 * np.max(epochs) + i * offset_between_bars
+            dt = (t[1] - t[0]) / 2
+            for st in sig_times:
+                ax.plot((st - dt, st + dt), (y, y), color=p[0].get_color(), linewidth=3)
+
+    # Add a dashed line at time = 0
+    ax.axvline(0, linestyle="--", color="black")
+
+    # Set title, axis labels and range
+    ax.set_title(title)
+    ax.set_xlabel(x_label)
+    ax.set_ylabel(y_label)
+    ax.set_xlim(t[0], t[-1])
+
+    # Add a legend
+    if add_legend:
+        ax.legend(loc=legend_loc)
+
+    # Save figure
+    if filename is not None:
+        save(fig, filename)
+    elif create_fig:
+        return fig, ax
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics/utils/topoplots.py` & `osl-dynamics-1.2.3/osl_dynamics/utils/topoplots.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.2/osl_dynamics.egg-info/PKG-INFO` & `osl-dynamics-1.2.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: osl-dynamics
-Version: 1.2.2
-Summary: Models for infering dynamics in neuroimaging data
-Home-page: https://github.com/OHBA-analysis/osl-dynamics
-License: MIT
-Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
-Description-Content-Type: text/x-rst; charset=UTF-8
-
 ============
 osl-dynamics
 ============
 
 See the read the docs page for a description of this project: `https://osl-dynamics.readthedocs.io <https://osl-dynamics.readthedocs.io>`_.
 
 Installation
@@ -22,15 +13,15 @@
 
     git clone https://github.com/OHBA-analysis/osl-dynamics.git
     cd osl-dynamics
     conda env create -f envs/linux.yml
     conda activate osld
     pip install -e .
 
-Note, the conda environments use ``pip`` to install TensorFlow, you may need to load/install additional libraries (such as CUDA/cuDNN) if you have GPU support.
+If you're using a Mac then use the ``envs/mac.yml`` file to create the conda environment instead of ``envs/linux.yml``. Note, the conda environments use ``pip`` to install TensorFlow, you may need to load/install additional libraries (such as CUDA/cuDNN) if you have GPU support.
 
 Developers might want to clone the repo using SSH instead of HTTPS:
 
 .. code-block:: shell
 
     git clone git@github.com:OHBA-analysis/osl-dynamics.git
```

### Comparing `osl-dynamics-1.2.2/osl_dynamics.egg-info/SOURCES.txt` & `osl-dynamics-1.2.3/osl_dynamics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 osl_dynamics/analysis/gmm.py
 osl_dynamics/analysis/modes.py
 osl_dynamics/analysis/power.py
 osl_dynamics/analysis/regression.py
 osl_dynamics/analysis/spectral.py
 osl_dynamics/analysis/static.py
 osl_dynamics/analysis/statistics.py
+osl_dynamics/analysis/tinda.py
 osl_dynamics/analysis/workbench.py
 osl_dynamics/config_api/__init__.py
-osl_dynamics/config_api/cli.py
 osl_dynamics/config_api/pipeline.py
 osl_dynamics/config_api/wrappers.py
 osl_dynamics/data/__init__.py
 osl_dynamics/data/base.py
 osl_dynamics/data/osl.py
 osl_dynamics/data/processing.py
 osl_dynamics/data/rw.py
@@ -155,14 +155,15 @@
 osl_dynamics/models/mage.py
 osl_dynamics/models/mdynemo.py
 osl_dynamics/models/mdynemo_obs.py
 osl_dynamics/models/mod_base.py
 osl_dynamics/models/sage.py
 osl_dynamics/models/sedynemo.py
 osl_dynamics/models/sedynemo_obs.py
+osl_dynamics/models/sehmm.py
 osl_dynamics/models/state_dynemo.py
 osl_dynamics/simulation/__init__.py
 osl_dynamics/simulation/base.py
 osl_dynamics/simulation/hmm.py
 osl_dynamics/simulation/hsmm.py
 osl_dynamics/simulation/mar.py
 osl_dynamics/simulation/mvn.py
```

### Comparing `osl-dynamics-1.2.2/setup.cfg` & `osl-dynamics-1.2.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osl-dynamics
-version = 1.2.2
+version = 1.2.3
 description = Models for infering dynamics in neuroimaging data
 license = MIT
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/OHBA-analysis/osl-dynamics
 project_urls = 
 	Documentation = https://osl-dynamics.readthedocs.io/en/latest/
@@ -52,13 +52,13 @@
 
 [build_sphinx]
 source_dir = doc
 build_dir = build/sphinx
 
 [options.entry_points]
 console_scripts = 
-	osld-pipeline = osl_dynamics.config_api.cli:pipeline
+	osld-pipeline = osl_dynamics.config_api.pipeline:osld_pipeline_cli
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

