# Comparing `tmp/Vespa_Suite-1.0.2-py38-none-any.whl.zip` & `tmp/Vespa_Suite-1.1.0rc1-py37-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,32 @@
-Zip file size: 7483788 bytes, number of entries: 445
+Zip file size: 7623277 bytes, number of entries: 459
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/__init__.py
 -rw-rw-rw-  2.0 fat     8316 b- defN 21-Mar-07 21:00 vespa/check_dependencies.py
 -rw-rw-rw-  2.0 fat     6021 b- defN 21-Feb-18 17:57 vespa/create_shortcuts.py
 -rw-rw-rw-  2.0 fat     1853 b- defN 21-Feb-18 17:57 vespa/requirements.txt
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/analysis/__init__.py
 -rw-rw-rw-  2.0 fat     2824 b- defN 21-Feb-18 17:57 vespa/analysis/block.py
--rw-rw-rw-  2.0 fat    54813 b- defN 21-Mar-07 21:13 vespa/analysis/block_fit_giso.py
+-rw-rw-rw-  2.0 fat    53457 b- defN 22-Jul-31 02:17 vespa/analysis/block_fit_giso.py
+-rw-rw-rw-  2.0 fat    54813 b- defN 21-Mar-07 21:13 vespa/analysis/block_fit_giso_Last.py
 -rw-rw-rw-  2.0 fat     2948 b- defN 21-Feb-18 17:57 vespa/analysis/block_fit_identity.py
+-rw-rw-rw-  2.0 fat    40393 b- defN 21-Mar-07 21:15 vespa/analysis/block_fit_voigt - Copy.py
 -rw-rw-rw-  2.0 fat    40393 b- defN 21-Mar-07 21:15 vespa/analysis/block_fit_voigt.py
 -rw-rw-rw-  2.0 fat     1620 b- defN 21-Feb-18 17:57 vespa/analysis/block_prep_edit_fidsum.py
 -rw-rw-rw-  2.0 fat    28301 b- defN 21-Mar-09 17:27 vespa/analysis/block_prep_fidsum.py
 -rw-rw-rw-  2.0 fat     2814 b- defN 21-Feb-18 17:57 vespa/analysis/block_prep_identity.py
 -rw-rw-rw-  2.0 fat    11384 b- defN 21-Feb-18 17:57 vespa/analysis/block_prep_megalaser.py
 -rw-rw-rw-  2.0 fat    14223 b- defN 21-Feb-18 17:57 vespa/analysis/block_prep_timeseries.py
 -rw-rw-rw-  2.0 fat    14072 b- defN 21-Jul-08 17:44 vespa/analysis/block_prep_wbnaa.py
 -rw-rw-rw-  2.0 fat     2800 b- defN 21-Feb-18 17:57 vespa/analysis/block_quant_identity.py
 -rw-rw-rw-  2.0 fat    16636 b- defN 21-Feb-18 17:57 vespa/analysis/block_quant_watref.py
 -rw-rw-rw-  2.0 fat     4255 b- defN 21-Feb-18 17:57 vespa/analysis/block_raw.py
 -rw-rw-rw-  2.0 fat     9535 b- defN 21-Mar-20 01:15 vespa/analysis/block_raw_cmrr_slaser.py
--rw-rw-rw-  2.0 fat     6801 b- defN 21-Mar-20 01:15 vespa/analysis/block_raw_edit_fidsum.py
--rw-rw-rw-  2.0 fat     4246 b- defN 21-Mar-20 01:15 vespa/analysis/block_raw_probep.py
+-rw-rw-rw-  2.0 fat     9115 b- defN 23-Jan-30 01:30 vespa/analysis/block_raw_edit.py
+-rw-rw-rw-  2.0 fat     9265 b- defN 23-Jan-30 01:30 vespa/analysis/block_raw_edit_fidsum.py
+-rw-rw-rw-  2.0 fat     4265 b- defN 23-Jan-29 16:29 vespa/analysis/block_raw_probep.py
 -rw-rw-rw-  2.0 fat    39995 b- defN 21-Feb-18 17:57 vespa/analysis/block_spectral.py
 -rw-rw-rw-  2.0 fat     2844 b- defN 21-Feb-18 17:57 vespa/analysis/block_spectral_identity.py
 -rw-rw-rw-  2.0 fat     1326 b- defN 21-Feb-18 17:57 vespa/analysis/chain_base.py
 -rw-rw-rw-  2.0 fat    20823 b- defN 21-Feb-18 17:57 vespa/analysis/chain_fit_giso.py
 -rw-rw-rw-  2.0 fat      474 b- defN 21-Feb-18 17:57 vespa/analysis/chain_fit_identity.py
 -rw-rw-rw-  2.0 fat    38831 b- defN 21-Apr-11 19:56 vespa/analysis/chain_fit_voigt.py
 -rw-rw-rw-  2.0 fat     7370 b- defN 21-Apr-16 17:21 vespa/analysis/chain_prep_fidsum.py
@@ -32,65 +35,65 @@
 -rw-rw-rw-  2.0 fat     3169 b- defN 21-Feb-18 17:57 vespa/analysis/chain_prep_timeseries.py
 -rw-rw-rw-  2.0 fat     3067 b- defN 21-Jul-08 18:39 vespa/analysis/chain_prep_wbnaa.py
 -rw-rw-rw-  2.0 fat      476 b- defN 21-Feb-18 17:57 vespa/analysis/chain_quant_identity.py
 -rw-rw-rw-  2.0 fat     5660 b- defN 21-Apr-06 20:49 vespa/analysis/chain_quant_watref.py
 -rw-rw-rw-  2.0 fat      632 b- defN 21-Feb-18 17:57 vespa/analysis/chain_raw.py
 -rw-rw-rw-  2.0 fat     5420 b- defN 21-Feb-18 17:57 vespa/analysis/chain_spectral.py
 -rw-rw-rw-  2.0 fat      489 b- defN 21-Feb-18 17:57 vespa/analysis/chain_spectral_identity.py
--rw-rw-rw-  2.0 fat    26640 b- defN 21-Apr-11 19:53 vespa/analysis/constants.py
+-rw-rw-rw-  2.0 fat    26649 b- defN 22-Sep-13 00:47 vespa/analysis/constants.py
 -rw-rw-rw-  2.0 fat     6119 b- defN 21-Feb-18 17:57 vespa/analysis/deprecated_dynamic_list_user_prior.py
 -rw-rw-rw-  2.0 fat     7091 b- defN 21-Feb-18 17:57 vespa/analysis/dialog_dataset_browser.py
 -rw-rw-rw-  2.0 fat    10805 b- defN 21-Feb-18 17:57 vespa/analysis/dialog_experiment_indices.py
 -rw-rw-rw-  2.0 fat    23643 b- defN 21-Feb-18 17:57 vespa/analysis/dialog_user_defined_metabolite.py
 -rw-rw-rw-  2.0 fat    31127 b- defN 21-Feb-18 17:57 vespa/analysis/dialog_user_defined_prior.py
 -rw-rw-rw-  2.0 fat    13767 b- defN 21-Feb-18 17:57 vespa/analysis/dialog_user_metabolite_info.py
 -rw-rw-rw-  2.0 fat    19804 b- defN 21-Feb-18 17:57 vespa/analysis/dialog_user_prior.py
 -rw-rw-rw-  2.0 fat    11637 b- defN 21-Feb-18 17:57 vespa/analysis/dynamic_list_giso_metabolite.py
 -rw-rw-rw-  2.0 fat    11659 b- defN 21-Feb-18 17:57 vespa/analysis/dynamic_list_voigt_metabolite.py
 -rw-rw-rw-  2.0 fat   107792 b- defN 21-May-05 01:53 vespa/analysis/figure_layouts.py
 -rw-rw-rw-  2.0 fat     6983 b- defN 21-Feb-18 17:57 vespa/analysis/liver31p_series_sorter.py
--rw-rw-rw-  2.0 fat    32510 b- defN 21-Jul-23 13:25 vespa/analysis/main.py
--rw-rw-rw-  2.0 fat   102829 b- defN 21-Apr-06 22:14 vespa/analysis/mrs_dataset.py
+-rw-rw-rw-  2.0 fat    33195 b- defN 23-Jan-29 04:16 vespa/analysis/main.py
+-rw-rw-rw-  2.0 fat   103551 b- defN 23-Jan-29 19:24 vespa/analysis/mrs_dataset.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 21-Feb-18 17:57 vespa/analysis/mrs_macromolecule.py
 -rw-rw-rw-  2.0 fat    18240 b- defN 21-Feb-18 17:57 vespa/analysis/mrs_metinfo.py
 -rw-rw-rw-  2.0 fat     4516 b- defN 21-Feb-18 17:57 vespa/analysis/mrs_user_prior.py
 -rw-rw-rw-  2.0 fat     5345 b- defN 21-Feb-18 17:57 vespa/analysis/mrs_user_prior_spectrum.py
--rw-rw-rw-  2.0 fat    28391 b- defN 21-Mar-26 14:02 vespa/analysis/notebook_datasets.py
+-rw-rw-rw-  2.0 fat    30137 b- defN 23-Jan-30 14:22 vespa/analysis/notebook_datasets.py
 -rw-rw-rw-  2.0 fat    10386 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_giso.py
 -rw-rw-rw-  2.0 fat    14377 b- defN 21-Mar-26 16:28 vespa/analysis/plot_panel_prep_fidsum.py
 -rw-rw-rw-  2.0 fat     6691 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_prep_megalaser.py
 -rw-rw-rw-  2.0 fat     7084 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_prep_timeseries.py
 -rw-rw-rw-  2.0 fat    11940 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_prep_wbnaa.py
 -rw-rw-rw-  2.0 fat    10050 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_spectral.py
 -rw-rw-rw-  2.0 fat     9383 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_svd_filter.py
 -rw-rw-rw-  2.0 fat     4966 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_user_defined_metabolite.py
 -rw-rw-rw-  2.0 fat     5020 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_user_prior.py
 -rw-rw-rw-  2.0 fat    10463 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_voigt.py
 -rw-rw-rw-  2.0 fat     9969 b- defN 21-Feb-18 17:57 vespa/analysis/plot_panel_watref.py
 -rw-rw-rw-  2.0 fat    14386 b- defN 21-Feb-18 17:57 vespa/analysis/prefs.py
 -rw-rw-rw-  2.0 fat     4112 b- defN 21-Feb-18 17:57 vespa/analysis/svd_output.py
 -rw-rw-rw-  2.0 fat     4581 b- defN 21-Feb-18 17:57 vespa/analysis/tab_base.py
--rw-rw-rw-  2.0 fat    28549 b- defN 21-Mar-26 13:31 vespa/analysis/tab_dataset.py
+-rw-rw-rw-  2.0 fat    28792 b- defN 23-Jan-29 04:18 vespa/analysis/tab_dataset.py
 -rw-rw-rw-  2.0 fat   118580 b- defN 21-Mar-07 21:13 vespa/analysis/tab_giso.py
--rw-rw-rw-  2.0 fat    51561 b- defN 21-Mar-26 16:26 vespa/analysis/tab_prep_fidsum.py
--rw-rw-rw-  2.0 fat    24000 b- defN 21-Feb-18 17:57 vespa/analysis/tab_prep_timeseries.py
+-rw-rw-rw-  2.0 fat    51841 b- defN 23-Jan-31 02:43 vespa/analysis/tab_prep_fidsum.py
+-rw-rw-rw-  2.0 fat    24081 b- defN 23-Jan-26 22:52 vespa/analysis/tab_prep_timeseries.py
 -rw-rw-rw-  2.0 fat    27449 b- defN 21-Jul-08 18:41 vespa/analysis/tab_prep_wbnaa.py
 -rw-rw-rw-  2.0 fat     5874 b- defN 21-Feb-18 17:57 vespa/analysis/tab_raw.py
--rw-rw-rw-  2.0 fat    94724 b- defN 21-Feb-18 17:57 vespa/analysis/tab_spectral.py
+-rw-rw-rw-  2.0 fat   106352 b- defN 23-Jan-29 22:33 vespa/analysis/tab_spectral.py
 -rw-rw-rw-  2.0 fat   152487 b- defN 21-Apr-11 22:35 vespa/analysis/tab_voigt.py
 -rw-rw-rw-  2.0 fat    36691 b- defN 21-Apr-12 01:21 vespa/analysis/tab_watref.py
 -rw-rw-rw-  2.0 fat    25912 b- defN 21-Feb-18 17:57 vespa/analysis/test_multi_optimize.py
 -rw-rw-rw-  2.0 fat    30675 b- defN 21-Feb-18 17:57 vespa/analysis/test_multi_optimize_pool.py
 -rw-rw-rw-  2.0 fat     2288 b- defN 21-Feb-18 17:57 vespa/analysis/util_analysis_config.py
 -rw-rw-rw-  2.0 fat      586 b- defN 21-Feb-18 17:57 vespa/analysis/util_db.py
--rw-rw-rw-  2.0 fat    18798 b- defN 21-Jul-23 13:25 vespa/analysis/util_file_import.py
+-rw-rw-rw-  2.0 fat    21320 b- defN 23-Jan-30 15:13 vespa/analysis/util_file_import.py
 -rw-rw-rw-  2.0 fat     2518 b- defN 21-Feb-18 17:57 vespa/analysis/util_import.py
 -rw-rw-rw-  2.0 fat    70015 b- defN 21-Feb-18 17:57 vespa/analysis/util_initial_values.py
--rw-rw-rw-  2.0 fat    44104 b- defN 21-Apr-12 01:33 vespa/analysis/util_menu.py
--rw-rw-rw-  2.0 fat     1149 b- defN 21-Feb-18 17:57 vespa/analysis/utils.py
+-rw-rw-rw-  2.0 fat    46427 b- defN 23-Jan-28 03:07 vespa/analysis/util_menu.py
+-rw-rw-rw-  2.0 fat     5791 b- defN 22-Aug-30 20:09 vespa/analysis/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/analysis/algos/__init__.py
 -rw-rw-rw-  2.0 fat     1633 b- defN 21-Feb-18 17:57 vespa/analysis/algos/auto_correlate.py
 -rw-rw-rw-  2.0 fat     1683 b- defN 21-Feb-18 17:57 vespa/analysis/algos/b0_correction.py
 -rw-rw-rw-  2.0 fat    13137 b- defN 21-Jul-18 19:40 vespa/analysis/algos/constrained_levenberg_marquardt.py
 -rw-rw-rw-  2.0 fat     1564 b- defN 21-Feb-18 17:57 vespa/analysis/algos/cross_correlate.py
 -rw-rw-rw-  2.0 fat     3228 b- defN 21-Feb-18 17:57 vespa/analysis/algos/fida_ecc.py
 -rw-rw-rw-  2.0 fat     3246 b- defN 21-Feb-18 17:57 vespa/analysis/algos/fida_getcoilcombos_specReg.py
@@ -120,26 +123,28 @@
 -rw-rw-rw-  2.0 fat     3010 b- defN 21-Feb-18 17:57 vespa/analysis/auto_gui/raw.py
 -rw-rw-rw-  2.0 fat    35026 b- defN 21-Feb-18 17:57 vespa/analysis/auto_gui/spectral.py
 -rw-rw-rw-  2.0 fat    17067 b- defN 21-Feb-18 17:57 vespa/analysis/auto_gui/timeseries.py
 -rw-rw-rw-  2.0 fat    86685 b- defN 21-Apr-11 19:55 vespa/analysis/auto_gui/voigt.py
 -rw-rw-rw-  2.0 fat    17137 b- defN 21-Feb-18 17:57 vespa/analysis/auto_gui/watref.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/__init__.py
 -rw-rw-rw-  2.0 fat     4656 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/bruker.py
--rw-rw-rw-  2.0 fat    60309 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/dicom_browser_dialog.py
+-rw-rw-rw-  2.0 fat    60852 b- defN 22-Oct-03 21:30 vespa/analysis/fileio/dicom_browser_dialog.py
 -rw-rw-rw-  2.0 fat     8306 b- defN 21-Apr-30 13:12 vespa/analysis/fileio/dicom_philips.py
--rw-rw-rw-  2.0 fat    15275 b- defN 21-Apr-30 13:12 vespa/analysis/fileio/dicom_siemens.py
+-rw-rw-rw-  2.0 fat    15392 b- defN 23-Jan-26 22:52 vespa/analysis/fileio/dicom_siemens.py
+-rw-rw-rw-  2.0 fat    19729 b- defN 23-Jan-26 22:52 vespa/analysis/fileio/dicom_siemens_cmrr_mpress.py
+-rw-rw-rw-  2.0 fat    19998 b- defN 23-Jan-30 14:25 vespa/analysis/fileio/dicom_siemens_eja_svs_mpress.py
 -rw-rw-rw-  2.0 fat      720 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/dicom_siemens_timeseries.py
--rw-rw-rw-  2.0 fat     8041 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/ge_pfile.py
+-rw-rw-rw-  2.0 fat     8193 b- defN 22-May-03 02:05 vespa/analysis/fileio/ge_pfile.py
 -rw-rw-rw-  2.0 fat     1894 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/philips_fidsum.py
 -rw-rw-rw-  2.0 fat     7281 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/philips_spar.py
--rw-rw-rw-  2.0 fat     9119 b- defN 21-Jun-27 20:15 vespa/analysis/fileio/raw_reader.py
+-rw-rw-rw-  2.0 fat     9690 b- defN 23-Jan-30 15:10 vespa/analysis/fileio/raw_reader.py
 -rw-rw-rw-  2.0 fat     4381 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/siemens_rda.py
--rw-rw-rw-  2.0 fat    20784 b- defN 21-Mar-11 21:59 vespa/analysis/fileio/siemens_twix.py
+-rw-rw-rw-  2.0 fat    21064 b- defN 23-Mar-22 21:28 vespa/analysis/fileio/siemens_twix.py
 -rw-rw-rw-  2.0 fat     7395 b- defN 21-Mar-20 03:56 vespa/analysis/fileio/siemens_twix_slaser_cmrr.py
--rw-rw-rw-  2.0 fat     2993 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/siemens_twix_svs_edit.py
+-rw-rw-rw-  2.0 fat     3055 b- defN 22-Sep-12 14:15 vespa/analysis/fileio/siemens_twix_svs_edit.py
 -rw-rw-rw-  2.0 fat     1735 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/siemens_twix_svs_se.py
 -rw-rw-rw-  2.0 fat    15803 b- defN 21-Jun-27 19:22 vespa/analysis/fileio/siemens_twix_wbnaa.py
 -rw-rw-rw-  2.0 fat     7146 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/template.py
 -rw-rw-rw-  2.0 fat     2347 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/util_exceptions.py
 -rw-rw-rw-  2.0 fat     6634 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/util_parameters.py
 -rw-rw-rw-  2.0 fat     8272 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/util_philips.py
 -rw-rw-rw-  2.0 fat     4721 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/varian.py
@@ -154,71 +159,71 @@
 -rw-rw-rw-  2.0 fat     3288 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/dicom_browser/auto_gui/dicom_browser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/nmrglue/__init__.py
 -rw-rw-rw-  2.0 fat    84694 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/nmrglue/bruker_for_vespa.py
 -rw-rw-rw-  2.0 fat    20111 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/nmrglue/fileiobase.py
 -rw-rw-rw-  2.0 fat    63756 b- defN 21-Feb-18 17:57 vespa/analysis/fileio/nmrglue/proc_base.py
 -rw-rw-rw-  2.0 fat    64749 b- defN 21-Mar-07 20:50 vespa/analysis/fileio/nmrglue/varian.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/analysis/functors/__init__.py
--rw-rw-rw-  2.0 fat    22520 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_ecc.py
+-rw-rw-rw-  2.0 fat    23166 b- defN 23-Jan-26 22:52 vespa/analysis/functors/funct_ecc.py
 -rw-rw-rw-  2.0 fat     9504 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_fidsum_all.py
 -rw-rw-rw-  2.0 fat    19534 b- defN 21-Mar-09 17:42 vespa/analysis/functors/funct_fidsum_coil_combine.py
--rw-rw-rw-  2.0 fat    16331 b- defN 21-Apr-13 20:29 vespa/analysis/functors/funct_fidsum_correction.py
+-rw-rw-rw-  2.0 fat    16394 b- defN 23-Jan-19 00:13 vespa/analysis/functors/funct_fidsum_correction.py
 -rw-rw-rw-  2.0 fat     2590 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_fidsum_exclude.py
 -rw-rw-rw-  2.0 fat    11631 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_fidsum_megalaser.py
 -rw-rw-rw-  2.0 fat    12259 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_fidsum_wbnaa.py
 -rw-rw-rw-  2.0 fat    34838 b- defN 21-Mar-20 14:42 vespa/analysis/functors/funct_fit_giso.py
--rw-rw-rw-  2.0 fat    45038 b- defN 21-Apr-16 17:19 vespa/analysis/functors/funct_fit_voigt.py
+-rw-rw-rw-  2.0 fat    45412 b- defN 23-May-03 01:49 vespa/analysis/functors/funct_fit_voigt.py
 -rw-rw-rw-  2.0 fat      363 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_quant_watref_all.py
 -rw-rw-rw-  2.0 fat    15521 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_spectral_all.py
 -rw-rw-rw-  2.0 fat    10751 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_timeseries_all.py
 -rw-rw-rw-  2.0 fat    13207 b- defN 21-Feb-18 17:57 vespa/analysis/functors/funct_water_filter.py
 -rw-rw-rw-  2.0 fat     1055 b- defN 21-Feb-18 17:57 vespa/analysis/functors/functor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/common/__init__.py
 -rw-rw-rw-  2.0 fat     8785 b- defN 21-Feb-18 17:57 vespa/common/base_transform.py
 -rw-rw-rw-  2.0 fat     6970 b- defN 21-Feb-18 17:57 vespa/common/bloch_call.py
 -rw-rw-rw-  2.0 fat     1232 b- defN 21-Feb-18 17:57 vespa/common/configobj.py
--rw-rw-rw-  2.0 fat    30989 b- defN 21-Apr-15 20:34 vespa/common/constants.py
+-rw-rw-rw-  2.0 fat    30990 b- defN 23-May-09 01:18 vespa/common/constants.py
 -rw-rw-rw-  2.0 fat    11886 b- defN 21-Apr-15 20:40 vespa/common/create_database.py
 -rw-rw-rw-  2.0 fat    15836 b- defN 21-Jul-23 13:26 vespa/common/default_ini_file_content.py
 -rw-rw-rw-  2.0 fat     6615 b- defN 21-Feb-18 17:57 vespa/common/dialog_experiment_browser.py
 -rw-rw-rw-  2.0 fat     5828 b- defN 21-Feb-18 17:57 vespa/common/dialog_export.py
 -rw-rw-rw-  2.0 fat     6528 b- defN 21-Feb-18 17:57 vespa/common/dialog_pulse_design_browser.py
--rw-rw-rw-  2.0 fat    12150 b- defN 21-Feb-18 17:57 vespa/common/exception_handler.py
+-rw-rw-rw-  2.0 fat    12182 b- defN 23-May-09 01:18 vespa/common/exception_handler.py
 -rw-rw-rw-  2.0 fat     2465 b- defN 21-Feb-18 17:57 vespa/common/experiment_preview.py
--rw-rw-rw-  2.0 fat   210652 b- defN 21-Feb-18 17:57 vespa/common/ge_read_pfile.py
+-rw-rw-rw-  2.0 fat   198250 b- defN 22-May-03 02:14 vespa/common/ge_read_pfile.py
 -rw-rw-rw-  2.0 fat    36943 b- defN 21-Feb-18 17:57 vespa/common/hlsvdpropy.py
 -rw-rw-rw-  2.0 fat    10905 b- defN 21-Mar-08 20:41 vespa/common/images.py
 -rw-rw-rw-  2.0 fat    10917 b- defN 21-Feb-18 17:57 vespa/common/menu.py
 -rw-rw-rw-  2.0 fat     7261 b- defN 21-Feb-18 17:57 vespa/common/minf_parabolic_info.py
--rw-rw-rw-  2.0 fat    20366 b- defN 21-Jun-27 19:35 vespa/common/mrs_data_raw.py
+-rw-rw-rw-  2.0 fat    23597 b- defN 22-Oct-04 02:25 vespa/common/mrs_data_raw.py
 -rw-rw-rw-  2.0 fat      788 b- defN 21-Feb-18 17:57 vespa/common/mrs_data_raw_timeseries.py
 -rw-rw-rw-  2.0 fat      996 b- defN 21-Feb-18 17:57 vespa/common/mrs_data_raw_wbnaa.py
 -rw-rw-rw-  2.0 fat    17733 b- defN 21-Mar-07 21:13 vespa/common/mrs_experiment.py
 -rw-rw-rw-  2.0 fat    10811 b- defN 21-Feb-18 17:57 vespa/common/mrs_generic.py
 -rw-rw-rw-  2.0 fat    13639 b- defN 21-Feb-18 17:57 vespa/common/mrs_generic_basis.py
 -rw-rw-rw-  2.0 fat     2489 b- defN 21-Feb-18 17:57 vespa/common/mrs_j_coupling.py
 -rw-rw-rw-  2.0 fat     8055 b- defN 21-Feb-18 17:57 vespa/common/mrs_metabolite.py
 -rw-rw-rw-  2.0 fat     9319 b- defN 21-Mar-07 21:13 vespa/common/mrs_prior.py
 -rw-rw-rw-  2.0 fat     5083 b- defN 21-Feb-18 17:57 vespa/common/mrs_prior_metabolite.py
 -rw-rw-rw-  2.0 fat     9326 b- defN 21-Feb-18 17:57 vespa/common/mrs_pulse_sequence.py
 -rw-rw-rw-  2.0 fat    11755 b- defN 21-Feb-18 17:57 vespa/common/mrs_simulation.py
 -rw-rw-rw-  2.0 fat     2177 b- defN 21-Feb-18 17:57 vespa/common/mrs_spin.py
--rw-rw-rw-  2.0 fat     8707 b- defN 21-Feb-18 17:57 vespa/common/prefs.py
+-rw-rw-rw-  2.0 fat     8740 b- defN 22-Aug-30 00:47 vespa/common/prefs.py
 -rw-rw-rw-  2.0 fat     9473 b- defN 21-Feb-18 17:57 vespa/common/rfp_machine_specs.py
 -rw-rw-rw-  2.0 fat     2842 b- defN 21-Feb-18 17:57 vespa/common/rfp_master_parameters.py
--rw-rw-rw-  2.0 fat    19774 b- defN 21-Feb-18 17:57 vespa/common/rfp_pulse_design.py
+-rw-rw-rw-  2.0 fat    19777 b- defN 23-May-09 01:18 vespa/common/rfp_pulse_design.py
 -rw-rw-rw-  2.0 fat     2182 b- defN 21-Feb-18 17:57 vespa/common/rfp_pulse_design_preview.py
--rw-rw-rw-  2.0 fat    24203 b- defN 21-Feb-18 17:57 vespa/common/rfp_rf_result.py
+-rw-rw-rw-  2.0 fat    25646 b- defN 23-May-09 01:18 vespa/common/rfp_rf_result.py
 -rw-rw-rw-  2.0 fat    11262 b- defN 21-Mar-07 21:13 vespa/common/rfp_transform.py
 -rw-rw-rw-  2.0 fat    19525 b- defN 21-Feb-18 17:57 vespa/common/rfp_transform_kernel.py
 -rw-rw-rw-  2.0 fat    15742 b- defN 21-Feb-18 17:57 vespa/common/styled_text_control.py
 -rw-rw-rw-  2.0 fat     2264 b- defN 21-Feb-18 17:57 vespa/common/transform_kernel_preview.py
 -rw-rw-rw-  2.0 fat      802 b- defN 21-Feb-18 17:57 vespa/common/transform_run_exception.py
 -rw-rw-rw-  2.0 fat    42333 b- defN 21-Jun-27 17:14 vespa/common/twix_parser.py
--rw-rw-rw-  2.0 fat    67633 b- defN 21-Jun-27 17:15 vespa/common/twix_parser_multi_raid.py
+-rw-rw-rw-  2.0 fat    68433 b- defN 23-Mar-22 21:28 vespa/common/twix_parser_multi_raid.py
 -rw-rw-rw-  2.0 fat   262945 b- defN 21-Feb-18 17:57 vespa/common/wavelet_1d.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/common/auto_gui/__init__.py
 -rw-rw-rw-  2.0 fat     2203 b- defN 21-Feb-18 17:57 vespa/common/auto_gui/exception_report.py
 -rw-rw-rw-  2.0 fat     3417 b- defN 21-Feb-18 17:57 vespa/common/auto_gui/experiment_browser.py
 -rw-rw-rw-  2.0 fat     3105 b- defN 21-Feb-18 17:57 vespa/common/auto_gui/export.py
 -rw-rw-rw-  2.0 fat     3637 b- defN 21-Feb-18 17:57 vespa/common/auto_gui/pulse_design_browser.py
 -rw-rw-rw-  2.0 fat     2846 b- defN 21-Feb-18 17:57 vespa/common/auto_gui/pulse_project_browser.py
@@ -286,32 +291,32 @@
 -rw-rw-rw-  2.0 fat     6326 b- defN 21-Feb-18 17:57 vespa/common/util/ppm.py
 -rw-rw-rw-  2.0 fat     4873 b- defN 21-Feb-18 17:57 vespa/common/util/time_.py
 -rw-rw-rw-  2.0 fat    28288 b- defN 21-Feb-18 17:57 vespa/common/util/xml_.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/__init__.py
 -rw-rw-rw-  2.0 fat     7027 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/common_dialogs.py
 -rw-rw-rw-  2.0 fat    68903 b- defN 21-Mar-07 21:13 vespa/common/wx_gravy/image_panel.py
 -rw-rw-rw-  2.0 fat    98996 b- defN 21-Mar-07 21:13 vespa/common/wx_gravy/image_panel_roi.py
--rw-rw-rw-  2.0 fat    67355 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/image_panel_toolbar.py
+-rw-rw-rw-  2.0 fat    67254 b- defN 22-Jun-13 20:14 vespa/common/wx_gravy/image_panel_toolbar.py
 -rw-rw-rw-  2.0 fat    78240 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/mask_panel_toolbar.py
 -rw-rw-rw-  2.0 fat     6415 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/notebooks.py
--rw-rw-rw-  2.0 fat    59997 b- defN 21-Mar-26 16:27 vespa/common/wx_gravy/plot_panel.py
+-rw-rw-rw-  2.0 fat    59997 b- defN 23-May-09 01:18 vespa/common/wx_gravy/plot_panel.py
 -rw-rw-rw-  2.0 fat    93072 b- defN 21-Mar-07 21:14 vespa/common/wx_gravy/plot_panel_points.py
 -rw-rw-rw-  2.0 fat    94844 b- defN 21-Mar-07 21:14 vespa/common/wx_gravy/plot_panel_scatter.py
--rw-rw-rw-  2.0 fat   116167 b- defN 21-Mar-07 21:14 vespa/common/wx_gravy/plot_panel_spectrum.py
+-rw-rw-rw-  2.0 fat   116692 b- defN 23-Jan-28 03:00 vespa/common/wx_gravy/plot_panel_spectrum.py
 -rw-rw-rw-  2.0 fat    18536 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/util.py
 -rw-rw-rw-  2.0 fat     2386 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/zot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/__init__.py
 -rw-rw-rw-  2.0 fat      162 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin/__init__.py
 -rw-rw-rw-  2.0 fat     1721 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin/codegen.py
--rw-rw-rw-  2.0 fat     8725 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin/floatspin.py
+-rw-rw-rw-  2.0 fat     9243 b- defN 23-May-04 01:30 vespa/common/wx_gravy/widgets/floatspin/floatspin.py
 -rw-rw-rw-  2.0 fat     3200 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin/wconfig.py
 -rw-rw-rw-  2.0 fat      172 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier/__init__.py
 -rw-rw-rw-  2.0 fat     2206 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier/codegen.py
--rw-rw-rw-  2.0 fat     9088 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier.py
--rw-rw-rw-  2.0 fat     2514 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier_base.py
+-rw-rw-rw-  2.0 fat     9611 b- defN 23-May-04 01:30 vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier.py
+-rw-rw-rw-  2.0 fat     2508 b- defN 23-May-04 01:30 vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier_base.py
 -rw-rw-rw-  2.0 fat     3236 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier/wconfig.py
 -rw-rw-rw-  2.0 fat      172 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/__init__.py
 -rw-rw-rw-  2.0 fat     2206 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/codegen.py
 -rw-rw-rw-  2.0 fat     9611 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/floatspin_multiplier.py
 -rw-rw-rw-  2.0 fat     2508 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/floatspin_multiplier_base.py
 -rw-rw-rw-  2.0 fat     3236 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/wconfig.py
 -rw-rw-rw-  2.0 fat      162 b- defN 21-Feb-18 17:57 vespa/common/wx_gravy/widgets/floatspin_v96/__init__.py
@@ -341,14 +346,23 @@
 -rw-rw-rw-  2.0 fat   448020 b- defN 21-Feb-18 17:57 vespa/docs/datasim_user_manual.pdf
 -rw-rw-rw-  2.0 fat  1181178 b- defN 21-Feb-18 17:57 vespa/docs/pulse_user_manual.pdf
 -rw-rw-rw-  2.0 fat  1132329 b- defN 21-Feb-18 17:57 vespa/docs/simulation_user_manual.pdf
 -rw-rw-rw-  2.0 fat    19518 b- defN 21-Mar-08 20:48 vespa/icons/icon1_datasim.ico
 -rw-rw-rw-  2.0 fat    19518 b- defN 21-Mar-08 20:48 vespa/icons/icon2_simulation.ico
 -rw-rw-rw-  2.0 fat    19518 b- defN 21-Mar-08 20:48 vespa/icons/icon3_pulse.ico
 -rw-rw-rw-  2.0 fat    19518 b- defN 21-Mar-08 20:48 vespa/icons/icon4_analysis.ico
+-rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/interfaces/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/interfaces/inline/__init__.py
+-rw-rw-rw-  2.0 fat    25199 b- defN 21-May-03 13:10 vespa/interfaces/inline/vespa_inline_engine.py
+-rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/interfaces/inline/ge/__init__.py
+-rw-rw-rw-  2.0 fat   118878 b- defN 21-Feb-18 17:57 vespa/interfaces/inline/ge/inline_vespa_ge.py
+-rw-rw-rw-  2.0 fat    17884 b- defN 21-Feb-18 17:57 vespa/interfaces/inline/ge/run_inline_vespa_ge.py
+-rw-rw-rw-  2.0 fat     4880 b- defN 21-Feb-18 17:57 vespa/interfaces/inline/ge/run_inline_vespa_ge_v1.py
+-rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/interfaces/inline/philips/__init__.py
+-rw-rw-rw-  2.0 fat    20930 b- defN 21-May-05 02:36 vespa/interfaces/inline/philips/run_inline_vespa_philips.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/public/__init__.py
 -rw-rw-rw-  2.0 fat     3482 b- defN 21-Feb-18 17:57 vespa/public/annotated_coding_example.py
 -rw-rw-rw-  2.0 fat     7232 b- defN 21-Feb-18 17:57 vespa/public/convert_ascii2viff.py
 -rw-rw-rw-  2.0 fat     1819 b- defN 21-Feb-18 17:57 vespa/public/minimalist_pulse.py
 -rw-rw-rw-  2.0 fat     5589 b- defN 21-Feb-18 17:57 vespa/public/simulation_description.py
 -rw-rw-rw-  2.0 fat     1513 b- defN 21-Feb-18 17:57 vespa/public/transform_description.py
 -rw-rw-rw-  2.0 fat        2 b- defN 21-Feb-18 17:57 vespa/pulse/__init__.py
@@ -369,15 +383,15 @@
 -rw-rw-rw-  2.0 fat     2645 b- defN 21-Feb-18 17:57 vespa/pulse/plot_panel_transform.py
 -rw-rw-rw-  2.0 fat     5166 b- defN 21-Feb-18 17:57 vespa/pulse/plot_panel_transform_contour.py
 -rw-rw-rw-  2.0 fat     2363 b- defN 21-Feb-18 17:57 vespa/pulse/prefs.py
 -rw-rw-rw-  2.0 fat    26064 b- defN 21-Feb-18 17:57 vespa/pulse/run_transform_controller.py
 -rw-rw-rw-  2.0 fat    27877 b- defN 21-Feb-18 17:57 vespa/pulse/run_transform_controller_multi.py
 -rw-rw-rw-  2.0 fat    13461 b- defN 21-Mar-07 21:06 vespa/pulse/tab_basic_info.py
 -rw-rw-rw-  2.0 fat    29011 b- defN 21-Mar-07 21:14 vespa/pulse/tab_pulse_design.py
--rw-rw-rw-  2.0 fat    71252 b- defN 21-Mar-07 21:14 vespa/pulse/tab_transform.py
+-rw-rw-rw-  2.0 fat    72322 b- defN 23-May-09 01:18 vespa/pulse/tab_transform.py
 -rw-rw-rw-  2.0 fat      838 b- defN 21-Feb-18 17:57 vespa/pulse/util.py
 -rw-rw-rw-  2.0 fat    18518 b- defN 21-Feb-18 17:57 vespa/pulse/util_db.py
 -rw-rw-rw-  2.0 fat     8599 b- defN 21-Mar-08 16:23 vespa/pulse/util_menu.py
 -rw-rw-rw-  2.0 fat      745 b- defN 21-Feb-18 17:57 vespa/pulse/util_pulse_config.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/__init__.py
 -rw-rw-rw-  2.0 fat     6787 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/basic_info.py
 -rw-rw-rw-  2.0 fat    13112 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/editor_transform.py
@@ -385,15 +399,15 @@
 -rw-rw-rw-  2.0 fat     7126 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/machine_specs.py
 -rw-rw-rw-  2.0 fat     4657 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/manage_machine_specs.py
 -rw-rw-rw-  2.0 fat     5272 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/manage_pulse_designs.py
 -rw-rw-rw-  2.0 fat     5720 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/manage_transform_kernels.py
 -rw-rw-rw-  2.0 fat    14094 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/ocn.py
 -rw-rw-rw-  2.0 fat     1507 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/optional_message.py
 -rw-rw-rw-  2.0 fat     4039 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/panel_kernel_globals.py
--rw-rw-rw-  2.0 fat    11463 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/panel_tab_transform.py
+-rw-rw-rw-  2.0 fat    11940 b- defN 23-May-09 01:18 vespa/pulse/auto_gui/panel_tab_transform.py
 -rw-rw-rw-  2.0 fat     9615 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/panel_transform_editor.py
 -rw-rw-rw-  2.0 fat     1970 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/referrers.py
 -rw-rw-rw-  2.0 fat    12269 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/third_party_export.py
 -rw-rw-rw-  2.0 fat     1893 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/view_pulse_design.py
 -rw-rw-rw-  2.0 fat     1934 b- defN 21-Feb-18 17:57 vespa/pulse/auto_gui/view_transform_kernel.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Feb-18 17:57 vespa/simulation/__init__.py
 -rw-rw-rw-  2.0 fat      630 b- defN 21-Feb-18 17:57 vespa/simulation/aui_subclass.py
@@ -435,13 +449,13 @@
 -rw-rw-rw-  2.0 fat     4137 b- defN 21-Feb-18 17:57 vespa/simulation/auto_gui/mixed_metabolite_designer.py
 -rw-rw-rw-  2.0 fat    25640 b- defN 21-Feb-18 17:57 vespa/simulation/auto_gui/mixed_metabolite_output.py
 -rw-rw-rw-  2.0 fat    22576 b- defN 21-Mar-07 21:16 vespa/simulation/auto_gui/pulse_sequence_editor.py
 -rw-rw-rw-  2.0 fat     6996 b- defN 21-Feb-18 17:57 vespa/simulation/auto_gui/pulse_sequence_info.py
 -rw-rw-rw-  2.0 fat    13199 b- defN 21-Feb-18 17:57 vespa/simulation/auto_gui/simulate.py
 -rw-rw-rw-  2.0 fat    16152 b- defN 21-Feb-18 17:57 vespa/simulation/auto_gui/visualize.py
 -rw-rw-rw-  2.0 fat     3137 b- defN 21-Feb-18 17:57 vespa/simulation/auto_gui/visualize_resolution.py
--rw-rw-rw-  2.0 fat     1704 b- defN 21-Jul-23 13:41 Vespa_Suite-1.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2093 b- defN 21-Jul-23 13:41 Vespa_Suite-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       93 b- defN 21-Jul-23 13:41 Vespa_Suite-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 21-Jul-23 13:41 Vespa_Suite-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    42566 b- defN 21-Jul-23 13:41 Vespa_Suite-1.0.2.dist-info/RECORD
-445 files, 15439629 bytes uncompressed, 7415658 bytes compressed:  52.0%
+-rw-rw-rw-  2.0 fat     1704 b- defN 23-May-11 12:28 Vespa_Suite-1.1.0rc1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2096 b- defN 23-May-11 12:28 Vespa_Suite-1.1.0rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       93 b- defN 23-May-11 12:28 Vespa_Suite-1.1.0rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-11 12:28 Vespa_Suite-1.1.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    43984 b- defN 23-May-11 12:28 Vespa_Suite-1.1.0rc1.dist-info/RECORD
+459 files, 15797832 bytes uncompressed, 7552839 bytes compressed:  52.2%
```

## zipnote {}

```diff
@@ -15,17 +15,23 @@
 
 Filename: vespa/analysis/block.py
 Comment: 
 
 Filename: vespa/analysis/block_fit_giso.py
 Comment: 
 
+Filename: vespa/analysis/block_fit_giso_Last.py
+Comment: 
+
 Filename: vespa/analysis/block_fit_identity.py
 Comment: 
 
+Filename: vespa/analysis/block_fit_voigt - Copy.py
+Comment: 
+
 Filename: vespa/analysis/block_fit_voigt.py
 Comment: 
 
 Filename: vespa/analysis/block_prep_edit_fidsum.py
 Comment: 
 
 Filename: vespa/analysis/block_prep_fidsum.py
@@ -51,14 +57,17 @@
 
 Filename: vespa/analysis/block_raw.py
 Comment: 
 
 Filename: vespa/analysis/block_raw_cmrr_slaser.py
 Comment: 
 
+Filename: vespa/analysis/block_raw_edit.py
+Comment: 
+
 Filename: vespa/analysis/block_raw_edit_fidsum.py
 Comment: 
 
 Filename: vespa/analysis/block_raw_probep.py
 Comment: 
 
 Filename: vespa/analysis/block_spectral.py
@@ -378,14 +387,20 @@
 
 Filename: vespa/analysis/fileio/dicom_philips.py
 Comment: 
 
 Filename: vespa/analysis/fileio/dicom_siemens.py
 Comment: 
 
+Filename: vespa/analysis/fileio/dicom_siemens_cmrr_mpress.py
+Comment: 
+
+Filename: vespa/analysis/fileio/dicom_siemens_eja_svs_mpress.py
+Comment: 
+
 Filename: vespa/analysis/fileio/dicom_siemens_timeseries.py
 Comment: 
 
 Filename: vespa/analysis/fileio/ge_pfile.py
 Comment: 
 
 Filename: vespa/analysis/fileio/philips_fidsum.py
@@ -1032,14 +1047,41 @@
 
 Filename: vespa/icons/icon3_pulse.ico
 Comment: 
 
 Filename: vespa/icons/icon4_analysis.ico
 Comment: 
 
+Filename: vespa/interfaces/__init__.py
+Comment: 
+
+Filename: vespa/interfaces/inline/__init__.py
+Comment: 
+
+Filename: vespa/interfaces/inline/vespa_inline_engine.py
+Comment: 
+
+Filename: vespa/interfaces/inline/ge/__init__.py
+Comment: 
+
+Filename: vespa/interfaces/inline/ge/inline_vespa_ge.py
+Comment: 
+
+Filename: vespa/interfaces/inline/ge/run_inline_vespa_ge.py
+Comment: 
+
+Filename: vespa/interfaces/inline/ge/run_inline_vespa_ge_v1.py
+Comment: 
+
+Filename: vespa/interfaces/inline/philips/__init__.py
+Comment: 
+
+Filename: vespa/interfaces/inline/philips/run_inline_vespa_philips.py
+Comment: 
+
 Filename: vespa/public/__init__.py
 Comment: 
 
 Filename: vespa/public/annotated_coding_example.py
 Comment: 
 
 Filename: vespa/public/convert_ascii2viff.py
@@ -1314,23 +1356,23 @@
 
 Filename: vespa/simulation/auto_gui/visualize.py
 Comment: 
 
 Filename: vespa/simulation/auto_gui/visualize_resolution.py
 Comment: 
 
-Filename: Vespa_Suite-1.0.2.dist-info/LICENSE
+Filename: Vespa_Suite-1.1.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: Vespa_Suite-1.0.2.dist-info/METADATA
+Filename: Vespa_Suite-1.1.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: Vespa_Suite-1.0.2.dist-info/WHEEL
+Filename: Vespa_Suite-1.1.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Vespa_Suite-1.0.2.dist-info/top_level.txt
+Filename: Vespa_Suite-1.1.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Vespa_Suite-1.0.2.dist-info/RECORD
+Filename: Vespa_Suite-1.1.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vespa/analysis/block_fit_giso.py

```diff
@@ -35,3392 +35,3308 @@
 00000220: 4659 4920 4749 534f 203d 2047 726f 7570  FYI GISO = Group
 00000230: 6564 2049 6e64 6976 6964 7561 6c20 5369  ed Individual Si
 00000240: 6e67 6c65 7473 204f 7074 696d 697a 6174  nglets Optimizat
 00000250: 696f 6e0d 0a23 2020 206f 7220 6d61 7962  ion..#   or mayb
 00000260: 6520 4765 6e65 7261 6c69 7a65 6420 496e  e Generalized In
 00000270: 6469 7669 6475 616c 2053 696e 676c 6574  dividual Singlet
 00000280: 204f 7074 696d 697a 6174 696f 6e0d 0a0d   Optimization...
-00000290: 0a23 2054 6865 2048 544d 4c20 6765 6e65  .# The HTML gene
-000002a0: 7261 7465 6420 6279 2074 6869 7320 636f  rated by this co
-000002b0: 6465 2063 6f6e 7461 696e 7320 6120 636f  de contains a co
-000002c0: 6e64 6974 696f 6e61 6c20 636f 6d6d 656e  nditional commen
-000002d0: 7420 666f 7220 4945 2075 7365 7273 2e0d  t for IE users..
-000002e0: 0a23 205f 4945 5f49 4e43 4150 4142 4c45  .# _IE_INCAPABLE
-000002f0: 5f4d 5347 2069 7320 7468 6520 636f 6e74  _MSG is the cont
-00000300: 656e 7420 666f 7220 7468 6174 2063 6f6d  ent for that com
-00000310: 6d65 6e74 2e0d 0a23 2057 6520 7573 6520  ment...# We use 
-00000320: 7468 6520 6461 7461 2055 5249 2073 6368  the data URI sch
-00000330: 656d 6520 746f 2064 6973 706c 6179 206f  eme to display o
-00000340: 7572 2069 6d61 6765 2c20 616e 6420 4945  ur image, and IE
-00000350: 203c 2039 2064 6f65 7320 7375 7070 6f72   < 9 does suppor
-00000360: 7420 6974 2e0d 0a23 2054 6865 2063 6f6e  t it...# The con
-00000370: 6469 7469 6f6e 616c 636f 6d6d 656e 7420  ditionalcomment 
-00000380: 6973 2061 2076 616c 6964 2048 544d 4c20  is a valid HTML 
-00000390: 636f 6d6d 656e 742e 2049 7427 7320 6967  comment. It's ig
-000003a0: 6e6f 7265 6420 6279 2062 726f 7773 6572  nored by browser
-000003b0: 730d 0a23 2065 7863 6570 7420 4945 2077  s..# except IE w
-000003c0: 6869 6368 2069 7320 646f 6375 6d65 6e74  hich is document
-000003d0: 6564 2074 6f20 6c6f 6f6b 2066 6f72 2048  ed to look for H
-000003e0: 544d 4c20 636f 6d6d 656e 7473 2063 6f6e  TML comments con
-000003f0: 7461 696e 696e 6720 6365 7274 6169 6e20  taining certain 
-00000400: 6b65 790d 0a23 2073 7472 696e 6773 2e20  key..# strings. 
-00000410: 5468 6973 2061 6c6c 6f77 7320 7573 2074  This allows us t
-00000420: 6f20 6469 7370 6c61 7920 736c 6967 6874  o display slight
-00000430: 6c79 2064 6966 6665 7265 6e74 2063 6f6e  ly different con
-00000440: 7465 6e74 2074 6f20 7468 6f73 6520 7768  tent to those wh
-00000450: 6f0d 0a23 2063 616e 2774 2073 6565 2074  o..# can't see t
-00000460: 6865 2069 6d61 6765 2e0d 0a23 2072 6566  he image...# ref
-00000470: 3a20 6874 7470 3a2f 2f6d 7364 6e2e 6d69  : http://msdn.mi
-00000480: 6372 6f73 6f66 742e 636f 6d2f 656e 2d75  crosoft.com/en-u
-00000490: 732f 6c69 6272 6172 792f 6d73 3533 3735  s/library/ms5375
-000004a0: 3132 2532 3876 3d76 732e 3835 2532 392e  12%28v=vs.85%29.
-000004b0: 6173 7078 0d0a 2320 7265 463a 2068 7474  aspx..# reF: htt
-000004c0: 703a 2f2f 7777 772e 7175 6972 6b73 6d6f  p://www.quirksmo
-000004d0: 6465 2e6f 7267 2f63 7373 2f63 6f6e 6463  de.org/css/condc
-000004e0: 6f6d 2e68 746d 6c0d 0a5f 4945 5f49 4e43  om.html.._IE_INC
-000004f0: 4150 4142 4c45 5f4d 5347 203d 2022 2222  APABLE_MSG = """
-00000500: 5b69 6620 6c74 2049 4520 395d 3e0d 0a3c  [if lt IE 9]>..<
-00000510: 703e 3c73 7472 6f6e 673e 536f 7272 792c  p><strong>Sorry,
-00000520: 2049 6e74 6572 6e65 7420 4578 706c 6f72   Internet Explor
-00000530: 6572 2036 2c20 372c 2061 6e64 2038 2063  er 6, 7, and 8 c
-00000540: 616e 2774 2064 6973 706c 6179 2074 6865  an't display the
-00000550: 200d 0a69 6d61 6765 2062 656c 6f77 2e20   ..image below. 
-00000560: 416c 6c20 6f74 6865 7220 6d61 6a6f 7220  All other major 
-00000570: 6272 6f77 7365 7273 2028 4945 2039 2c20  browsers (IE 9, 
-00000580: 0d0a 3c61 2068 7265 663d 2268 7474 703a  ..<a href="http:
-00000590: 2f2f 7777 772e 6d6f 7a69 6c6c 612e 6f72  //www.mozilla.or
-000005a0: 672f 223e 4669 7265 666f 783c 2f61 3e2c  g/">Firefox</a>,
-000005b0: 200d 0a3c 6120 6872 6566 3d22 6874 7470   ..<a href="http
-000005c0: 3a2f 2f77 7777 2e67 6f6f 676c 652e 636f  ://www.google.co
-000005d0: 6d2f 6368 726f 6d65 2f22 3e43 6872 6f6d  m/chrome/">Chrom
-000005e0: 653c 2f61 3e2c 0d0a 3c61 2068 7265 663d  e</a>,..<a href=
-000005f0: 2268 7474 703a 2f2f 7777 772e 6f70 6572  "http://www.oper
-00000600: 612e 636f 6d2f 223e 4f70 6572 613c 2f61  a.com/">Opera</a
-00000610: 3e2c 2061 6e64 0d0a 3c61 2068 7265 663d  >, and..<a href=
-00000620: 2268 7474 703a 2f2f 7777 772e 6170 706c  "http://www.appl
-00000630: 652e 636f 6d2f 7361 6661 7269 2f22 3e53  e.com/safari/">S
-00000640: 6166 6172 693c 2f61 3e29 200d 0a63 616e  afari</a>) ..can
-00000650: 2064 6973 706c 6179 2069 742e 3c2f 7374   display it.</st
-00000660: 726f 6e67 3e0d 0a3c 2f70 3e0d 0a3c 215b  rong>..</p>..<![
-00000670: 656e 6469 665d 0d0a 2222 220d 0a0d 0a0d  endif]..""".....
-00000680: 0a23 205f 4353 5320 6973 2074 6865 2073  .# _CSS is the s
-00000690: 7479 6c65 2073 6865 6574 2066 6f72 2074  tyle sheet for t
-000006a0: 6865 2048 544d 4c20 7468 6174 2074 6869  he HTML that thi
-000006b0: 7320 636f 6465 2062 7569 6c64 732e 204e  s code builds. N
-000006c0: 6f74 6520 7468 6174 200d 0a23 2077 7850  ote that ..# wxP
-000006d0: 7974 686f 6e27 7320 4854 4d4c 2063 6f6e  ython's HTML con
-000006e0: 7472 6f6c 2064 6f65 736e 2774 2075 6e64  trol doesn't und
-000006f0: 6572 7374 616e 6420 4353 532e 2054 6869  erstand CSS. Thi
-00000700: 7320 6973 206f 6e6c 7920 666f 7220 7072  s is only for pr
-00000710: 696e 7469 6e67 0d0a 2320 6672 6f6d 2074  inting..# from t
-00000720: 6865 2062 726f 7773 6572 2e0d 0a5f 4353  he browser..._CS
-00000730: 5320 3d20 2222 220d 0a20 2020 2040 7061  S = """..    @pa
-00000740: 6765 207b 206d 6172 6769 6e3a 2032 306d  ge { margin: 20m
-00000750: 6d3b 2020 2020 2020 2020 2020 0d0a 2020  m;          ..  
-00000760: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00000770: 6c61 6e64 7363 6170 653b 2020 0d0a 2020  landscape;  ..  
-00000780: 2020 2020 2020 2020 7d0d 0a0d 0a20 2020          }....   
-00000790: 2040 6d65 6469 6120 7072 696e 7420 7b0d   @media print {.
-000007a0: 0a20 2020 2020 2020 202f 2a20 6134 203d  .        /* a4 =
-000007b0: 2032 3130 2078 2032 3937 6d6d 2c20 5553   210 x 297mm, US
-000007c0: 206c 6574 7465 7220 3d20 3231 3620 7820   letter = 216 x 
-000007d0: 3238 306d 6d2e 2054 776f 2032 306d 6d20  280mm. Two 20mm 
-000007e0: 6d61 7267 696e 7320 706c 7573 0d0a 2020  margins plus..  
-000007f0: 2020 2020 2020 7477 6f20 3131 306d 6d20        two 110mm 
-00000800: 626c 6f63 6b20 656c 656d 656e 7473 203d  block elements =
-00000810: 2034 3020 2b20 3232 3020 3d20 3236 306d   40 + 220 = 260m
-00000820: 6d20 7768 6963 6820 6669 7473 2077 6974  m which fits wit
-00000830: 6820 726f 6f6d 2074 6f0d 0a20 2020 2020  h room to..     
-00000840: 2020 2073 7061 7265 206f 6e20 626f 7468     spare on both
-00000850: 2070 6170 6572 2073 697a 6573 2061 7320   paper sizes as 
-00000860: 6c6f 6e67 2061 7320 7468 6520 276c 616e  long as the 'lan
-00000870: 6473 6361 7065 2720 6469 7265 6374 6976  dscape' directiv
-00000880: 6520 6973 0d0a 2020 2020 2020 2020 7265  e is..        re
-00000890: 7370 6563 7465 642e 0d0a 2020 2020 2020  spected...      
-000008a0: 2020 2a2f 0d0a 2020 2020 2020 2020 6469    */..        di
-000008b0: 7623 7461 626c 6520 7b20 7769 6474 683a  v#table { width:
-000008c0: 2038 306d 6d3b 207d 0d0a 2020 2020 2020   80mm; }..      
-000008d0: 2020 6469 7623 696d 6720 2020 7b20 7769    div#img   { wi
-000008e0: 6474 683a 2031 3430 6d6d 3b20 7d0d 0a20  dth: 140mm; }.. 
-000008f0: 2020 207d 0d0a 2222 220d 0a0d 0a0d 0a23     }.."""......#
-00000900: 2054 6865 2033 2066 756e 6374 696f 6e73   The 3 functions
-00000910: 2062 656c 6f77 2061 7265 2075 7365 6420   below are used 
-00000920: 666f 7220 6275 696c 6469 6e67 2048 544d  for building HTM
-00000930: 4c0d 0a64 6566 205f 666f 726d 6174 5f63  L..def _format_c
-00000940: 6f6c 756d 6e28 636f 6c75 6d6e 2c20 706c  olumn(column, pl
-00000950: 6163 6573 3d34 293a 0d0a 2020 2020 2320  aces=4):..    # 
-00000960: 4769 7665 6e20 6120 636f 6c75 6d6e 2066  Given a column f
-00000970: 726f 6d20 7468 6520 7461 626c 652c 2063  rom the table, c
-00000980: 6f6e 7665 7274 7320 6974 2074 6f20 6120  onverts it to a 
-00000990: 6e69 6365 6c79 2066 6f72 6d61 7474 6564  nicely formatted
-000009a0: 2073 7472 696e 670d 0a20 2020 2023 2061   string..    # a
-000009b0: 6e64 2072 6574 7572 6e73 2069 742e 2054  nd returns it. T
-000009c0: 6865 2063 6f6c 756d 6e20 6361 6e20 6265  he column can be
-000009d0: 2066 6c6f 6174 2c20 696e 742c 2062 6f6f   float, int, boo
-000009e0: 6c20 6f72 2061 2073 7472 696e 672e 2053  l or a string. S
-000009f0: 7472 696e 6773 0d0a 2020 2020 2320 6172  trings..    # ar
-00000a00: 6520 7265 7475 726e 6564 2075 6e74 6f75  e returned untou
-00000a10: 6368 6564 2e0d 0a20 2020 2069 6620 6973  ched...    if is
-00000a20: 696e 7374 616e 6365 2863 6f6c 756d 6e2c  instance(column,
-00000a30: 2066 6c6f 6174 293a 0d0a 2020 2020 2020   float):..      
-00000a40: 2020 636f 6c75 6d6e 203d 2028 2225 252e    column = ("%%.
-00000a50: 2564 6722 2025 2070 6c61 6365 7329 2025  %dg" % places) %
-00000a60: 2063 6f6c 756d 6e0d 0a20 2020 2065 6c69   column..    eli
-00000a70: 6620 6973 696e 7374 616e 6365 2863 6f6c  f isinstance(col
-00000a80: 756d 6e2c 2069 6e74 2920 6f72 2069 7369  umn, int) or isi
-00000a90: 6e73 7461 6e63 6528 636f 6c75 6d6e 2c20  nstance(column, 
-00000aa0: 626f 6f6c 293a 0d0a 2020 2020 2020 2020  bool):..        
-00000ab0: 636f 6c75 6d6e 203d 2073 7472 2863 6f6c  column = str(col
-00000ac0: 756d 6e29 0d0a 2020 2020 2365 6c73 653a  umn)..    #else:
-00000ad0: 0d0a 2020 2020 2020 2020 2320 4974 2773  ..        # It's
-00000ae0: 2061 2073 7472 696e 672c 206c 6561 7665   a string, leave
-00000af0: 2069 7420 616c 6f6e 652e 0d0a 0d0a 2020   it alone.....  
-00000b00: 2020 7265 7475 726e 2063 6f6c 756d 6e0d    return column.
-00000b10: 0a0d 0a0d 0a64 6566 205f 6765 745f 6d61  .....def _get_ma
-00000b20: 785f 7769 6474 6828 7461 626c 652c 2069  x_width(table, i
-00000b30: 6e64 6578 293a 0d0a 2020 2020 2222 2247  ndex):..    """G
-00000b40: 6574 2074 6865 206d 6178 696d 756d 2077  et the maximum w
-00000b50: 6964 7468 206f 6620 7468 6520 6769 7665  idth of the give
-00000b60: 6e20 636f 6c75 6d6e 2069 6e64 6578 2222  n column index""
-00000b70: 220d 0a20 2020 2072 6574 7572 6e20 6d61  "..    return ma
-00000b80: 7828 5b6c 656e 285f 666f 726d 6174 5f63  x([len(_format_c
-00000b90: 6f6c 756d 6e28 726f 775b 696e 6465 785d  olumn(row[index]
-00000ba0: 2929 2066 6f72 2072 6f77 2069 6e20 7461  )) for row in ta
-00000bb0: 626c 655d 2920 2020 200d 0a0d 0a0d 0a64  ble])    ......d
-00000bc0: 6566 205f 7072 6574 7479 5f73 7061 6365  ef _pretty_space
-00000bd0: 5f74 6162 6c65 2874 6162 6c65 2c20 706c  _table(table, pl
-00000be0: 6163 6573 293a 0d0a 2020 2020 2222 2252  aces):..    """R
-00000bf0: 6574 7572 6e73 2061 2074 6162 6c65 206f  eturns a table o
-00000c00: 6620 6461 7461 2c20 7061 6464 6564 2066  f data, padded f
-00000c10: 6f72 2061 6c69 676e 6d65 6e74 0d0a 2020  or alignment..  
-00000c20: 2020 4070 6172 616d 2074 6162 6c65 3a20    @param table: 
-00000c30: 5468 6520 7461 626c 6520 746f 2070 7269  The table to pri
-00000c40: 6e74 2e20 4120 6c69 7374 206f 6620 6c69  nt. A list of li
-00000c50: 7374 732e 0d0a 2020 2020 4561 6368 2072  sts...    Each r
-00000c60: 6f77 206d 7573 7420 6861 7665 2074 6865  ow must have the
-00000c70: 2073 616d 6520 6e75 6d62 6572 206f 6620   same number of 
-00000c80: 636f 6c75 6d6e 732e 200d 0a20 2020 2022  columns. ..    "
-00000c90: 2222 0d0a 2020 2020 636f 6c5f 7061 6464  ""..    col_padd
-00000ca0: 696e 6773 203d 205b 5d0d 0a0d 0a20 2020  ings = []....   
-00000cb0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00000cc0: 6c65 6e28 7461 626c 655b 305d 2929 3a0d  len(table[0])):.
-00000cd0: 0a20 2020 2020 2020 2063 6f6c 5f70 6164  .        col_pad
-00000ce0: 6469 6e67 732e 6170 7065 6e64 285f 6765  dings.append(_ge
-00000cf0: 745f 6d61 785f 7769 6474 6828 7461 626c  t_max_width(tabl
-00000d00: 652c 2069 2929 0d0a 0d0a 2020 2020 6c69  e, i))....    li
-00000d10: 6e65 7320 3d20 5b5d 0d0a 2020 2020 666f  nes = []..    fo
-00000d20: 7220 726f 7720 696e 2074 6162 6c65 3a0d  r row in table:.
-00000d30: 0a20 2020 2020 2020 2023 206c 6566 7420  .        # left 
-00000d40: 636f 6c0d 0a20 2020 2020 2020 2068 6472  col..        hdr
-00000d50: 203d 2072 6f77 5b30 5d2e 6365 6e74 6572   = row[0].center
-00000d60: 2863 6f6c 5f70 6164 6469 6e67 735b 305d  (col_paddings[0]
-00000d70: 202b 2032 290d 0a20 2020 2020 2020 2023   + 2)..        #
-00000d80: 2072 6573 7420 6f66 2074 6865 2063 6f6c   rest of the col
-00000d90: 730d 0a20 2020 2020 2020 2066 6f72 2069  s..        for i
-00000da0: 2069 6e20 7261 6e67 6528 312c 206c 656e   in range(1, len
-00000db0: 2872 6f77 2929 3a0d 0a20 2020 2020 2020  (row)):..       
-00000dc0: 2020 2020 2063 6f6c 203d 205f 666f 726d       col = _form
-00000dd0: 6174 5f63 6f6c 756d 6e28 726f 775b 695d  at_column(row[i]
-00000de0: 2c20 706c 6163 6573 292e 6365 6e74 6572  , places).center
-00000df0: 2863 6f6c 5f70 6164 6469 6e67 735b 695d  (col_paddings[i]
-00000e00: 202b 2032 290d 0a20 2020 2020 2020 2020   + 2)..         
-00000e10: 2020 2068 6472 202b 3d20 636f 6c0d 0a20     hdr += col.. 
-00000e20: 2020 2020 2020 206c 696e 6573 2e61 7070         lines.app
-00000e30: 656e 6428 6864 7229 0d0a 2020 2020 0d0a  end(hdr)..    ..
-00000e40: 2020 2020 7265 7475 726e 206c 696e 6573      return lines
-00000e50: 0d0a 0d0a 0d0a 6465 6620 5f70 7265 7474  ......def _prett
-00000e60: 795f 7370 6163 655f 7461 626c 655f 696e  y_space_table_in
-00000e70: 706c 6163 6528 7461 626c 652c 2070 6c61  place(table, pla
-00000e80: 6365 7329 3a0d 0a20 2020 2022 2222 5265  ces):..    """Re
-00000e90: 7475 726e 7320 6120 7461 626c 6520 6f66  turns a table of
-00000ea0: 2064 6174 612c 2070 6164 6465 6420 666f   data, padded fo
-00000eb0: 7220 616c 6967 6e6d 656e 740d 0a20 2020  r alignment..   
-00000ec0: 2040 7061 7261 6d20 7461 626c 653a 2054   @param table: T
-00000ed0: 6865 2074 6162 6c65 2074 6f20 7072 696e  he table to prin
-00000ee0: 742e 2041 206c 6973 7420 6f66 206c 6973  t. A list of lis
-00000ef0: 7473 2e0d 0a20 2020 2045 6163 6820 726f  ts...    Each ro
-00000f00: 7720 6d75 7374 2068 6176 6520 7468 6520  w must have the 
-00000f10: 7361 6d65 206e 756d 6265 7220 6f66 2063  same number of c
-00000f20: 6f6c 756d 6e73 2e20 0d0a 2020 2020 2222  olumns. ..    ""
-00000f30: 220d 0a20 2020 2063 6f6c 5f70 6164 6469  "..    col_paddi
-00000f40: 6e67 7320 3d20 5b5d 0d0a 0d0a 2020 2020  ngs = []....    
-00000f50: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00000f60: 656e 2874 6162 6c65 5b30 5d29 293a 0d0a  en(table[0])):..
-00000f70: 2020 2020 2020 2020 636f 6c5f 7061 6464          col_padd
-00000f80: 696e 6773 2e61 7070 656e 6428 5f67 6574  ings.append(_get
-00000f90: 5f6d 6178 5f77 6964 7468 2874 6162 6c65  _max_width(table
-00000fa0: 2c20 6929 290d 0a0d 0a20 2020 2066 6f72  , i))....    for
-00000fb0: 206a 2c20 726f 7720 696e 2065 6e75 6d65   j, row in enume
-00000fc0: 7261 7465 2874 6162 6c65 293a 0d0a 2020  rate(table):..  
-00000fd0: 2020 2020 2020 2320 6c65 6674 2063 6f6c        # left col
-00000fe0: 0d0a 2020 2020 2020 2020 7461 626c 655b  ..        table[
-00000ff0: 6a5d 5b30 5d20 3d20 726f 775b 305d 2e72  j][0] = row[0].r
-00001000: 6a75 7374 2863 6f6c 5f70 6164 6469 6e67  just(col_padding
-00001010: 735b 305d 202b 2032 290d 0a20 2020 2020  s[0] + 2)..     
-00001020: 2020 2023 2072 6573 7420 6f66 2074 6865     # rest of the
-00001030: 2063 6f6c 730d 0a20 2020 2020 2020 2066   cols..        f
-00001040: 6f72 2069 2069 6e20 7261 6e67 6528 312c  or i in range(1,
-00001050: 206c 656e 2872 6f77 2929 3a0d 0a20 2020   len(row)):..   
-00001060: 2020 2020 2020 2020 2074 6162 6c65 5b6a           table[j
-00001070: 5d5b 695d 203d 205f 666f 726d 6174 5f63  ][i] = _format_c
-00001080: 6f6c 756d 6e28 726f 775b 695d 2c20 706c  olumn(row[i], pl
-00001090: 6163 6573 292e 6365 6e74 6572 2863 6f6c  aces).center(col
-000010a0: 5f70 6164 6469 6e67 735b 695d 202b 2032  _paddings[i] + 2
-000010b0: 290d 0a20 2020 200d 0a20 2020 2072 6574  )..    ..    ret
-000010c0: 7572 6e20 7461 626c 650d 0a0d 0a0d 0a0d  urn table.......
-000010d0: 0a63 6c61 7373 205f 5365 7474 696e 6773  .class _Settings
-000010e0: 286f 626a 6563 7429 3a0d 0a20 2020 2022  (object):..    "
-000010f0: 2222 200d 0a20 2020 2053 6574 7469 6e67  "" ..    Setting
-00001100: 7320 6f62 6a65 6374 2063 6f6e 7461 696e  s object contain
-00001110: 7320 7468 6520 7061 7261 6d65 7465 7220  s the parameter 
-00001120: 696e 7075 7473 2075 7365 6420 666f 7220  inputs used for 
-00001130: 7072 6f63 6573 7369 6e67 2069 6e20 7468  processing in th
-00001140: 6520 0d0a 2020 2020 4368 6169 6e20 6f62  e ..    Chain ob
-00001150: 6a65 6374 2069 6e20 7468 6973 2042 6c6f  ject in this Blo
-00001160: 636b 2e20 4861 7669 6e67 2061 2073 6570  ck. Having a sep
-00001170: 6172 6174 6520 6f62 6a65 6374 2068 656c  arate object hel
-00001180: 7073 2074 6f20 6465 6c69 6e65 6174 6520  ps to delineate 
-00001190: 0d0a 2020 2020 696e 7075 7473 2f6f 7574  ..    inputs/out
-000011a0: 7075 7473 2061 6e64 2074 6f20 7369 6d70  puts and to simp
-000011b0: 6c69 6679 206c 6f61 642f 7361 7665 206f  lify load/save o
-000011c0: 6620 7072 6573 6574 2076 616c 7565 732e  f preset values.
-000011d0: 0d0a 0d0a 2020 2020 5468 6973 206f 626a  ....    This obj
-000011e0: 6563 7420 6361 6e20 616c 736f 2073 6176  ect can also sav
-000011f0: 652f 7265 6361 6c6c 2074 6865 7365 2076  e/recall these v
-00001200: 616c 7565 7320 746f 2f66 726f 6d20 616e  alues to/from an
-00001210: 2058 4d4c 206e 6f64 652e 0d0a 2020 2020   XML node...    
-00001220: 0d0a 2020 2020 2222 220d 0a20 2020 2058  ..    """..    X
-00001230: 4d4c 5f56 4552 5349 4f4e 203d 2022 312e  ML_VERSION = "1.
-00001240: 302e 3022 0d0a 2020 2020 0d0a 2020 2020  0.0"..    ..    
-00001250: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00001260: 662c 2020 6174 7472 6962 7574 6573 3d4e  f,  attributes=N
-00001270: 6f6e 6529 3a0d 0a0d 0a20 2020 2020 2020  one):....       
-00001280: 2023 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   #--------------
-00001290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000012a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-000012b0: 2020 2020 2320 4749 534f 2061 6c67 6f72      # GISO algor
-000012c0: 6974 686d 2069 6e70 7574 2073 6574 7469  ithm input setti
-000012d0: 6e67 730d 0a0d 0a20 2020 2020 2020 2073  ngs....        s
-000012e0: 656c 662e 7072 696f 725f 7070 6d5f 7374  elf.prior_ppm_st
-000012f0: 6172 7420 2020 2020 2020 2020 2020 2020  art             
-00001300: 2020 2020 2020 203d 2030 2e30 0d0a 2020         = 0.0..  
-00001310: 2020 2020 2020 7365 6c66 2e70 7269 6f72        self.prior
-00001320: 5f70 706d 5f65 6e64 2020 2020 2020 2020  _ppm_end        
-00001330: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
-00001340: 362e 310d 0a20 2020 2020 2020 2073 656c  6.1..        sel
-00001350: 662e 7072 696f 725f 6d61 736b 5f73 6f75  f.prior_mask_sou
-00001360: 7263 6520 2020 2020 2020 2020 2020 2020  rce             
-00001370: 2020 2020 203d 2063 6f6e 7374 616e 7473       = constants
-00001380: 2e46 6974 5072 696f 724d 6173 6b53 6f75  .FitPriorMaskSou
-00001390: 7263 652e 414c 4c5f 4f4e 0d0a 2020 2020  rce.ALL_ON..    
-000013a0: 2020 2020 7365 6c66 2e70 7269 6f72 5f6c      self.prior_l
-000013b0: 6973 7420 2020 2020 2020 2020 2020 2020  ist             
-000013c0: 2020 2020 2020 2020 2020 2020 3d20 5b5d              = []
-000013d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-000013e0: 7269 6f72 5f61 7265 615f 7363 616c 6520  rior_area_scale 
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2020 3d20 5b5d 0d0a 2020 2020 2020 2020    = []..        
-00001410: 7365 6c66 2e70 7269 6f72 5f70 6561 6b5f  self.prior_peak_
-00001420: 7070 6d20 2020 2020 2020 2020 2020 2020  ppm             
-00001430: 2020 2020 2020 2020 3d20 5b5d 0d0a 2020          = []..  
-00001440: 2020 2020 2020 7365 6c66 2e70 7269 6f72        self.prior
-00001450: 5f73 6561 7263 685f 7070 6d20 2020 2020  _search_ppm     
-00001460: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
-00001470: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
-00001480: 2e70 7269 6f72 5f64 625f 7070 6d20 2020  .prior_db_ppm   
-00001490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014a0: 2020 2020 3d20 5b5d 0d0a 2020 2020 2020      = []..      
-000014b0: 2020 7365 6c66 2e70 7269 6f72 5f66 6978    self.prior_fix
-000014c0: 5f74 3220 2020 2020 2020 2020 2020 2020  _t2             
-000014d0: 2020 2020 2020 2020 2020 3d20 5b5d 0d0a            = []..
-000014e0: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-000014f0: 6f72 5f73 6561 7263 685f 7068 3020 2020  or_search_ph0   
-00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001510: 3d20 5b5d 0d0a 2020 2020 2020 2020 7365  = []..        se
-00001520: 6c66 2e70 7269 6f72 5f78 7261 6e67 6520  lf.prior_xrange 
+00000290: 0a0d 0a0d 0a0d 0a0d 0a63 6c61 7373 205f  .........class _
+000002a0: 5365 7474 696e 6773 286f 626a 6563 7429  Settings(object)
+000002b0: 3a0d 0a20 2020 2022 2222 200d 0a20 2020  :..    """ ..   
+000002c0: 2053 6574 7469 6e67 7320 6f62 6a65 6374   Settings object
+000002d0: 2063 6f6e 7461 696e 7320 7468 6520 7061   contains the pa
+000002e0: 7261 6d65 7465 7220 696e 7075 7473 2075  rameter inputs u
+000002f0: 7365 6420 666f 7220 7072 6f63 6573 7369  sed for processi
+00000300: 6e67 2069 6e20 7468 6520 0d0a 2020 2020  ng in the ..    
+00000310: 4368 6169 6e20 6f62 6a65 6374 2069 6e20  Chain object in 
+00000320: 7468 6973 2042 6c6f 636b 2e20 4861 7669  this Block. Havi
+00000330: 6e67 2061 2073 6570 6172 6174 6520 6f62  ng a separate ob
+00000340: 6a65 6374 2068 656c 7073 2074 6f20 6465  ject helps to de
+00000350: 6c69 6e65 6174 6520 0d0a 2020 2020 696e  lineate ..    in
+00000360: 7075 7473 2f6f 7574 7075 7473 2061 6e64  puts/outputs and
+00000370: 2074 6f20 7369 6d70 6c69 6679 206c 6f61   to simplify loa
+00000380: 642f 7361 7665 206f 6620 7072 6573 6574  d/save of preset
+00000390: 2076 616c 7565 732e 0d0a 0d0a 2020 2020   values.....    
+000003a0: 5468 6973 206f 626a 6563 7420 6361 6e20  This object can 
+000003b0: 616c 736f 2073 6176 652f 7265 6361 6c6c  also save/recall
+000003c0: 2074 6865 7365 2076 616c 7565 7320 746f   these values to
+000003d0: 2f66 726f 6d20 616e 2058 4d4c 206e 6f64  /from an XML nod
+000003e0: 652e 0d0a 2020 2020 0d0a 2020 2020 2222  e...    ..    ""
+000003f0: 220d 0a20 2020 2058 4d4c 5f56 4552 5349  "..    XML_VERSI
+00000400: 4f4e 203d 2022 312e 302e 3022 0d0a 2020  ON = "1.0.0"..  
+00000410: 2020 0d0a 2020 2020 6465 6620 5f5f 696e    ..    def __in
+00000420: 6974 5f5f 2873 656c 662c 2020 6174 7472  it__(self,  attr
+00000430: 6962 7574 6573 3d4e 6f6e 6529 3a0d 0a0d  ibutes=None):...
+00000440: 0a20 2020 2020 2020 2023 2d2d 2d2d 2d2d  .        #------
+00000450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000470: 2d2d 0d0a 2020 2020 2020 2020 2320 4749  --..        # GI
+00000480: 534f 2061 6c67 6f72 6974 686d 2069 6e70  SO algorithm inp
+00000490: 7574 2073 6574 7469 6e67 730d 0a0d 0a20  ut settings.... 
+000004a0: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
+000004b0: 725f 7070 6d5f 7374 6172 7420 2020 2020  r_ppm_start     
+000004c0: 2020 2020 2020 2020 2020 2020 2020 203d                 =
+000004d0: 2030 2e30 0d0a 2020 2020 2020 2020 7365   0.0..        se
+000004e0: 6c66 2e70 7269 6f72 5f70 706d 5f65 6e64  lf.prior_ppm_end
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 2020 2020 2020 3d20 362e 310d 0a20 2020        = 6.1..   
+00000510: 2020 2020 2073 656c 662e 7072 696f 725f       self.prior_
+00000520: 6d61 736b 5f73 6f75 7263 6520 2020 2020  mask_source     
+00000530: 2020 2020 2020 2020 2020 2020 203d 2063               = c
+00000540: 6f6e 7374 616e 7473 2e46 6974 5072 696f  onstants.FitPrio
+00000550: 724d 6173 6b53 6f75 7263 652e 414c 4c5f  rMaskSource.ALL_
+00000560: 4f4e 0d0a 2020 2020 2020 2020 7365 6c66  ON..        self
+00000570: 2e70 7269 6f72 5f6c 6973 7420 2020 2020  .prior_list     
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 2020 2020 3d20 5b5d 0d0a 2020 2020 2020      = []..      
+000005a0: 2020 7365 6c66 2e70 7269 6f72 5f61 7265    self.prior_are
+000005b0: 615f 7363 616c 6520 2020 2020 2020 2020  a_scale         
+000005c0: 2020 2020 2020 2020 2020 3d20 5b5d 0d0a            = []..
+000005d0: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
+000005e0: 6f72 5f70 6561 6b5f 7070 6d20 2020 2020  or_peak_ppm     
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 3d20 5b5d 0d0a 2020 2020 2020 2020 7365  = []..        se
+00000610: 6c66 2e70 7269 6f72 5f73 6561 7263 685f  lf.prior_search_
+00000620: 7070 6d20 2020 2020 2020 2020 2020 2020  ppm             
+00000630: 2020 2020 2020 3d20 5b5d 0d0a 2020 2020        = []..    
+00000640: 2020 2020 7365 6c66 2e70 7269 6f72 5f64      self.prior_d
+00000650: 625f 7070 6d20 2020 2020 2020 2020 2020  b_ppm           
+00000660: 2020 2020 2020 2020 2020 2020 3d20 5b5d              = []
+00000670: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000680: 7269 6f72 5f66 6978 5f74 3220 2020 2020  rior_fix_t2     
+00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006a0: 2020 3d20 5b5d 0d0a 2020 2020 2020 2020    = []..        
+000006b0: 7365 6c66 2e70 7269 6f72 5f73 6561 7263  self.prior_searc
+000006c0: 685f 7068 3020 2020 2020 2020 2020 2020  h_ph0           
+000006d0: 2020 2020 2020 2020 3d20 5b5d 0d0a 2020          = []..  
+000006e0: 2020 2020 2020 7365 6c66 2e70 7269 6f72        self.prior
+000006f0: 5f78 7261 6e67 6520 2020 2020 2020 2020  _xrange         
+00000700: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+00000710: 5b30 2c31 5d20 2020 2020 2320 6d69 6e2f  [0,1]     # min/
+00000720: 6d61 7820 782d 7261 6e67 650d 0a20 2020  max x-range..   
+00000730: 2020 2020 2073 656c 662e 7072 696f 725f       self.prior_
+00000740: 7972 616e 6765 2020 2020 2020 2020 2020  yrange          
+00000750: 2020 2020 2020 2020 2020 2020 203d 205b               = [
+00000760: 302c 315d 2020 2020 2023 206d 696e 2f6d  0,1]     # min/m
+00000770: 6178 2079 2d72 616e 6765 0d0a 2020 2020  ax y-range..    
+00000780: 2020 2020 7365 6c66 2e70 7269 6f72 5f7a      self.prior_z
+00000790: 7261 6e67 6520 2020 2020 2020 2020 2020  range           
+000007a0: 2020 2020 2020 2020 2020 2020 3d20 5b30              = [0
+000007b0: 2c31 5d20 2020 2020 2320 6d69 6e2f 6d61  ,1]     # min/ma
+000007c0: 7820 7a2d 7261 6e67 650d 0a20 2020 2020  x z-range..     
+000007d0: 2020 2073 656c 662e 7072 696f 725f 6967     self.prior_ig
+000007e0: 6e6f 7265 5f6d 6173 6b20 2020 2020 2020  nore_mask       
+000007f0: 2020 2020 2020 2020 2020 203d 2046 616c             = Fal
+00000800: 7365 2020 2020 2020 0d0a 2020 2020 2020  se      ..      
+00000810: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00000820: 2e6c 696e 6573 6861 7065 5f6d 6f64 656c  .lineshape_model
+00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000840: 2020 2020 3d20 4669 744c 696e 6573 6861      = FitLinesha
+00000850: 7065 4d6f 6465 6c2e 4741 5553 5320 0d0a  peModel.GAUSS ..
+00000860: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
+00000870: 6e69 7469 616c 5f62 305f 7368 6966 745f  nitial_b0_shift_
+00000880: 6d65 7468 6f64 2020 2020 2020 2020 2020  method          
+00000890: 2020 3d20 636f 6e73 7461 6e74 732e 4669    = constants.Fi
+000008a0: 7449 6e69 7469 616c 4230 5368 6966 744d  tInitialB0ShiftM
+000008b0: 6574 686f 642e 4d41 4e55 414c 0d0a 2020  ethod.MANUAL..  
+000008c0: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
+000008d0: 616c 5f62 305f 7661 6c75 6520 2020 2020  al_b0_value     
+000008e0: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+000008f0: 302e 3020 2020 2020 2020 2320 696e 6974  0.0       # init
+00000900: 6961 6c20 6230 2073 6869 6674 2069 6e20  ial b0 shift in 
+00000910: 687a 0d0a 2020 2020 2020 2020 7365 6c66  hz..        self
+00000920: 2e69 6e69 7469 616c 5f62 6173 656c 696e  .initial_baselin
+00000930: 655f 6d65 7468 6f64 2020 2020 2020 2020  e_method        
+00000940: 2020 2020 3d20 636f 6e73 7461 6e74 732e      = constants.
+00000950: 4669 7449 6e69 7469 616c 4261 7365 6c69  FitInitialBaseli
+00000960: 6e65 4d65 7468 6f64 2e4e 4f4e 450d 0a20  neMethod.NONE.. 
+00000970: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+00000980: 6961 6c5f 6261 7365 6c69 6e65 5f6c 6f77  ial_baseline_low
+00000990: 6573 735f 7769 6474 6820 2020 2020 2020  ess_width       
+000009a0: 203d 2033 352e 3020 2020 2023 2048 7a0d   = 35.0    # Hz.
+000009b0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+000009c0: 6974 6961 6c5f 6261 7365 6c69 6e65 5f6c  itial_baseline_l
+000009d0: 6f77 6573 735f 6465 6c74 6120 2020 2020  owess_delta     
+000009e0: 2020 203d 2033 2e32 2020 2020 2023 200d     = 3.2     # .
+000009f0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00000a00: 6974 6961 6c5f 6261 7365 6c69 6e65 5f6c  itial_baseline_l
+00000a10: 6f77 6573 735f 6967 6e6f 7265 5f77 6964  owess_ignore_wid
+00000a20: 7468 203d 2031 352e 3020 2020 2023 2048  th = 15.0    # H
+00000a30: 7a0d 0a20 2020 2020 2020 200d 0a20 2020  z..        ..   
+00000a40: 2020 2020 2073 656c 662e 696e 6974 6961       self.initia
+00000a50: 6c5f 6372 5f63 686f 5f73 6570 6172 6174  l_cr_cho_separat
+00000a60: 696f 6e20 2020 2020 2020 2020 203d 2054  ion          = T
+00000a70: 7275 650d 0a20 2020 2020 2020 2073 656c  rue..        sel
+00000a80: 662e 696e 6974 6961 6c5f 7065 616b 5f73  f.initial_peak_s
+00000a90: 6561 7263 685f 6162 7320 2020 2020 2020  earch_abs       
+00000aa0: 2020 2020 203d 2046 616c 7365 0d0a 2020       = False..  
+00000ab0: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
+00000ac0: 616c 5f73 6d61 6c6c 5f70 6561 6b5f 6172  al_small_peak_ar
+00000ad0: 6561 7320 2020 2020 2020 2020 2020 3d20  eas           = 
+00000ae0: 636f 6e73 7461 6e74 732e 4669 7449 6e69  constants.FitIni
+00000af0: 7469 616c 536d 616c 6c50 6561 6b41 7265  tialSmallPeakAre
+00000b00: 6173 2e4e 4141 5f52 4154 494f 0d0a 2020  as.NAA_RATIO..  
+00000b10: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
+00000b20: 616c 5f73 6d61 6c6c 5f70 6561 6b5f 6672  al_small_peak_fr
+00000b30: 6571 7320 2020 2020 2020 2020 2020 3d20  eqs           = 
+00000b40: 636f 6e73 7461 6e74 732e 4669 7449 6e69  constants.FitIni
+00000b50: 7469 616c 536d 616c 6c50 6561 6b46 7265  tialSmallPeakFre
+00000b60: 7173 2e52 4546 5f50 4541 4b0d 0a20 2020  qs.REF_PEAK..   
+00000b70: 2020 2020 2073 656c 662e 696e 6974 6961       self.initia
+00000b80: 6c5f 6c69 6e65 7769 6474 685f 6d65 7468  l_linewidth_meth
+00000b90: 6f64 2020 2020 2020 2020 2020 203d 2063  od           = c
+00000ba0: 6f6e 7374 616e 7473 2e46 6974 496e 6974  onstants.FitInit
+00000bb0: 6961 6c4c 696e 6577 6964 7468 4d65 7468  ialLinewidthMeth
+00000bc0: 6f64 2e4d 414e 5541 4c20 0d0a 2020 2020  od.MANUAL ..    
+00000bd0: 2020 2020 7365 6c66 2e69 6e69 7469 616c      self.initial
+00000be0: 5f6c 696e 6577 6964 7468 5f76 616c 7565  _linewidth_value
+00000bf0: 2020 2020 2020 2020 2020 2020 3d20 382e              = 8.
+00000c00: 3020 2020 2020 2020 2320 696e 6974 6961  0       # initia
+00000c10: 6c20 6c69 6e65 7769 6474 6820 696e 2068  l linewidth in h
+00000c20: 7a0d 0a20 2020 2020 2020 2073 656c 662e  z..        self.
+00000c30: 696e 6974 6961 6c5f 6c69 6e65 7769 6474  initial_linewidt
+00000c40: 685f 7261 6e67 655f 7374 6172 7420 2020  h_range_start   
+00000c50: 2020 203d 2031 2e39 2020 2020 2020 2023     = 1.9       #
+00000c60: 204e 4220 7468 6973 2069 7320 2a4c 572a   NB this is *LW*
+00000c70: 206f 7074 696d 697a 6174 696f 6e20 7261   optimization ra
+00000c80: 6e67 650d 0a20 2020 2020 2020 2073 656c  nge..        sel
+00000c90: 662e 696e 6974 6961 6c5f 6c69 6e65 7769  f.initial_linewi
+00000ca0: 6474 685f 7261 6e67 655f 656e 6420 2020  dth_range_end   
+00000cb0: 2020 2020 203d 2034 2e31 2020 2020 2020       = 4.1      
+00000cc0: 2023 2020 7374 6172 742f 656e 6420 696e   #  start/end in
+00000cd0: 2070 706d 0d0a 2020 2020 2020 2020 7365   ppm..        se
+00000ce0: 6c66 2e69 6e69 7469 616c 5f6c 696e 6577  lf.initial_linew
+00000cf0: 6964 7468 5f66 7564 6765 2020 2020 2020  idth_fudge      
+00000d00: 2020 2020 2020 3d20 312e 3020 2020 2020        = 1.0     
+00000d10: 2020 2320 4c57 2066 7564 6765 2076 616c    # LW fudge val
+00000d20: 7565 2028 6c69 6e65 6172 2073 6361 6c65  ue (linear scale
+00000d30: 7229 0d0a 2020 2020 2020 2020 7365 6c66  r)..        self
+00000d40: 2e69 6e69 7469 616c 5f70 6861 7365 5f6d  .initial_phase_m
+00000d50: 6574 686f 6420 2020 2020 2020 2020 2020  ethod           
+00000d60: 2020 2020 3d20 636f 6e73 7461 6e74 732e      = constants.
+00000d70: 4669 7449 6e69 7469 616c 5068 6173 654d  FitInitialPhaseM
+00000d80: 6574 686f 642e 4d41 4e55 414c 2020 0d0a  ethod.MANUAL  ..
+00000d90: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
+00000da0: 7469 616c 5f70 6861 7365 305f 7661 6c75  tial_phase0_valu
+00000db0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00000dc0: 3d20 302e 3020 2020 2020 2020 2320 696e  = 0.0       # in
+00000dd0: 6974 6961 6c20 7068 6173 6530 2069 6e20  itial phase0 in 
+00000de0: 6465 670d 0a20 2020 2020 2020 2073 656c  deg..        sel
+00000df0: 662e 696e 6974 6961 6c5f 7068 6173 6531  f.initial_phase1
+00000e00: 5f76 616c 7565 2020 2020 2020 2020 2020  _value          
+00000e10: 2020 2020 203d 2030 2e30 2020 2020 2020       = 0.0      
+00000e20: 2023 2069 6e69 7469 616c 2070 6861 7365   # initial phase
+00000e30: 3120 696e 2064 6567 0d0a 2020 2020 2020  1 in deg..      
+00000e40: 2020 7365 6c66 2e69 6e69 7469 616c 5f61    self.initial_a
+00000e50: 7070 6c79 5f6b 6f5f 6669 6c74 6572 2020  pply_ko_filter  
+00000e60: 2020 2020 2020 2020 2020 3d20 4661 6c73            = Fals
+00000e70: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00000e80: 696e 6974 6961 6c5f 6b6f 5f6c 696e 6577  initial_ko_linew
+00000e90: 6964 7468 5f6d 696e 696d 756d 2020 2020  idth_minimum    
+00000ea0: 2020 203d 2032 300d 0a20 2020 2020 2020     = 20..       
+00000eb0: 2073 656c 662e 696e 6974 6961 6c5f 6b6f   self.initial_ko
+00000ec0: 5f70 6f69 6e74 7320 2020 2020 2020 2020  _points         
+00000ed0: 2020 2020 2020 2020 203d 2030 0d0a 2020           = 0..  
+00000ee0: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
+00000ef0: 616c 5f70 6861 7365 315f 6669 645f 636f  al_phase1_fid_co
+00000f00: 6e73 7461 6e74 2020 2020 2020 2020 3d20  nstant        = 
+00000f10: 302e 3020 2020 2020 2020 2320 666f 7220  0.0       # for 
+00000f20: 756c 7472 612d 7368 6f72 7420 4649 4420  ultra-short FID 
+00000f30: 6461 7461 2070 6861 7365 3120 756e 7772  data phase1 unwr
+00000f40: 6170 0d0a 2020 2020 2020 2020 7365 6c66  ap..        self
+00000f50: 2e69 6e69 7469 616c 5f6c 6163 5f6d 6574  .initial_lac_met
+00000f60: 686f 6420 2020 2020 2020 2020 2020 2020  hod             
+00000f70: 2020 2020 3d20 310d 0a20 2020 2020 2020      = 1..       
+00000f80: 2073 656c 662e 696e 6974 6961 6c5f 7065   self.initial_pe
+00000f90: 616b 5f6e 6567 6174 6976 655f 666c 6167  ak_negative_flag
+00000fa0: 2020 2020 2020 2020 203d 2030 2020 2020           = 0    
+00000fb0: 2020 2020 2023 2069 652e 2066 6f72 204c       # ie. for L
+00000fc0: 6163 2061 7420 3732 6d73 2c20 6e6f 7420  ac at 72ms, not 
+00000fd0: 696d 706c 656d 656e 7465 6420 696e 2047  implemented in G
+00000fe0: 5549 2079 6574 2020 2020 0d0a 0d0a 2020  UI yet    ....  
+00000ff0: 2020 2020 2020 7365 6c66 2e62 6173 656c        self.basel
+00001000: 696e 655f 6d65 7468 6f64 2020 2020 2020  ine_method      
+00001010: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+00001020: 636f 6e73 7461 6e74 732e 4669 7442 6173  constants.FitBas
+00001030: 656c 696e 654d 6574 686f 642e 4445 4641  elineMethod.DEFA
+00001040: 554c 540d 0a20 2020 2020 2020 2073 656c  ULT..        sel
+00001050: 662e 6261 7365 6c69 6e65 5f73 6d6f 6f74  f.baseline_smoot
+00001060: 6869 6e67 5f66 6c61 6720 2020 2020 2020  hing_flag       
+00001070: 2020 2020 203d 2046 616c 7365 0d0a 2020       = False..  
+00001080: 2020 2020 2020 7365 6c66 2e62 6173 656c        self.basel
+00001090: 696e 655f 736b 6970 5f6c 6173 745f 736d  ine_skip_last_sm
+000010a0: 6f6f 7468 2020 2020 2020 2020 2020 3d20  ooth          = 
+000010b0: 5472 7565 0d0a 2020 2020 2020 2020 7365  True..        se
+000010c0: 6c66 2e62 6173 656c 696e 655f 736d 6f6f  lf.baseline_smoo
+000010d0: 7468 696e 675f 7769 6474 6820 2020 2020  thing_width     
+000010e0: 2020 2020 2020 3d20 3230 2e30 2020 2020        = 20.0    
+000010f0: 2020 2320 696e 2048 7a0d 0a20 2020 2020    # in Hz..     
+00001100: 2020 2073 656c 662e 6261 7365 6c69 6e65     self.baseline
+00001110: 5f73 6d6f 6f74 6869 6e67 5f64 656c 7461  _smoothing_delta
+00001120: 2020 2020 2020 2020 2020 203d 2033 2e32             = 3.2
+00001130: 2020 2020 2020 2023 206c 6f77 6573 7320         # lowess 
+00001140: 736d 6f6f 7468 696e 6720 7074 2073 6b69  smoothing pt ski
+00001150: 7020 6465 6c74 6120 6475 7269 6e67 2077  p delta during w
+00001160: 6176 656c 6574 2062 6173 656c 696e 6520  avelet baseline 
+00001170: 6361 6c63 0d0a 2020 2020 2020 2020 7365  calc..        se
+00001180: 6c66 2e62 6173 656c 696e 655f 756e 6465  lf.baseline_unde
+00001190: 7265 7374 696d 6174 655f 6d65 7468 6f64  restimate_method
+000011a0: 2020 2020 2020 3d20 636f 6e73 7461 6e74        = constant
+000011b0: 732e 4669 7442 6173 656c 696e 6555 6e64  s.FitBaselineUnd
+000011c0: 6572 6573 7469 6d61 7465 4d65 7468 6f64  erestimateMethod
+000011d0: 2e44 4546 4155 4c54 0d0a 2020 2020 2020  .DEFAULT..      
+000011e0: 2020 7365 6c66 2e62 6173 656c 696e 655f    self.baseline_
+000011f0: 756e 6465 7265 7374 696d 6174 6520 2020  underestimate   
+00001200: 2020 2020 2020 2020 2020 3d20 302e 3020            = 0.0 
+00001210: 2020 2020 2020 2320 696e 2025 0d0a 2020        # in %..  
+00001220: 2020 2020 2020 7365 6c66 2e62 6173 656c        self.basel
+00001230: 696e 655f 756e 6465 7265 7374 696d 6174  ine_underestimat
+00001240: 655f 6c61 7374 2020 2020 2020 2020 3d20  e_last        = 
+00001250: 302e 3020 2020 2020 2020 2320 696e 2025  0.0       # in %
+00001260: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00001270: 6173 656c 696e 655f 756e 6465 7265 7374  aseline_underest
+00001280: 696d 6174 655f 7374 6570 7320 2020 2020  imate_steps     
+00001290: 2020 3d20 3320 2020 2020 2020 2020 2320    = 3         # 
+000012a0: 696e 2025 0d0a 0d0a 2020 2020 2020 2020  in %....        
+000012b0: 7365 6c66 2e62 6173 656c 696e 655f 7370  self.baseline_sp
+000012c0: 6c69 6e65 5f6e 6b6e 6f74 7320 2020 2020  line_nknots     
+000012d0: 2020 2020 2020 2020 3d20 3130 0d0a 2020          = 10..  
+000012e0: 2020 2020 2020 7365 6c66 2e62 6173 656c        self.basel
+000012f0: 696e 655f 7370 6c69 6e65 5f73 7061 6369  ine_spline_spaci
+00001300: 6e67 2020 2020 2020 2020 2020 2020 3d20  ng            = 
+00001310: 3130 2020 2020 2020 2020 2320 696e 2070  10        # in p
+00001320: 6f69 6e74 730d 0a20 2020 2020 2020 2073  oints..        s
+00001330: 656c 662e 6261 7365 6c69 6e65 5f73 706c  elf.baseline_spl
+00001340: 696e 655f 6f72 6465 7220 2020 2020 2020  ine_order       
+00001350: 2020 2020 2020 203d 2033 0d0a 2020 2020         = 3..    
+00001360: 2020 2020 7365 6c66 2e62 6173 656c 696e      self.baselin
+00001370: 655f 7761 7665 6c65 745f 7363 616c 6520  e_wavelet_scale 
+00001380: 2020 2020 2020 2020 2020 2020 3d20 340d              = 4.
+00001390: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
+000013a0: 7365 6c69 6e65 5f77 6176 656c 6574 5f6d  seline_wavelet_m
+000013b0: 696e 5f64 7961 6420 2020 2020 2020 2020  in_dyad         
+000013c0: 203d 2035 2e30 2020 2023 2066 6c6f 6174   = 5.0   # float
+000013d0: 2c20 696e 2048 7a20 6d69 6e20 7468 7265  , in Hz min thre
+000013e0: 7368 6f6c 640d 0a20 2020 2020 2020 2073  shold..        s
+000013f0: 656c 662e 6261 7365 6c69 6e65 5f77 6176  elf.baseline_wav
+00001400: 656c 6574 5f73 6872 696e 6b61 6765 5f66  elet_shrinkage_f
+00001410: 6c61 6720 2020 203d 2030 2020 2020 2023  lag    = 0     #
+00001420: 2066 6c67 202d 2064 6f20 7761 7665 6c65   flg - do wavele
+00001430: 7420 7368 7269 6e6b 6167 6520 302f 310d  t shrinkage 0/1.
+00001440: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
+00001450: 7365 6c69 6e65 5f77 6176 656c 6574 5f69  seline_wavelet_i
+00001460: 6e76 6172 6961 6e63 655f 6c61 6720 2020  nvariance_lag   
+00001470: 203d 2032 2020 2020 2023 2077 6176 656c   = 2     # wavel
+00001480: 6574 2069 6e76 6172 6961 6e63 6520 6c61  et invariance la
+00001490: 6720 4641 4354 4f52 2028 2b2f 2d20 706f  g FACTOR (+/- po
+000014a0: 696e 7473 290d 0a20 2020 2020 2020 2073  ints)..        s
+000014b0: 656c 662e 6261 7365 6c69 6e65 5f77 6176  elf.baseline_wav
+000014c0: 656c 6574 5f69 6e76 6172 6961 6e63 655f  elet_invariance_
+000014d0: 7265 636f 6d62 696e 6520 3d20 3020 2023  recombine = 0  #
+000014e0: 2072 6563 6f6d 6269 6e61 7469 6f6e 206d   recombination m
+000014f0: 6574 686f 6420 666f 7220 696e 7661 7269  ethod for invari
+00001500: 616e 6365 206c 6167 730d 0a0d 0a20 2020  ance lags....   
+00001510: 2020 2020 2073 656c 662e 6d61 6372 6f6d       self.macrom
+00001520: 6f6c 5f6d 6f64 656c 2020 2020 2020 2020  ol_model        
 00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 2020 2020 3d20 5b30 2c31 5d20 2020        = [0,1]   
-00001550: 2020 2320 6d69 6e2f 6d61 7820 782d 7261    # min/max x-ra
-00001560: 6e67 650d 0a20 2020 2020 2020 2073 656c  nge..        sel
-00001570: 662e 7072 696f 725f 7972 616e 6765 2020  f.prior_yrange  
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 203d 205b 302c 315d 2020 2020       = [0,1]    
-000015a0: 2023 206d 696e 2f6d 6178 2079 2d72 616e   # min/max y-ran
-000015b0: 6765 0d0a 2020 2020 2020 2020 7365 6c66  ge..        self
-000015c0: 2e70 7269 6f72 5f7a 7261 6e67 6520 2020  .prior_zrange   
-000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 2020 2020 3d20 5b30 2c31 5d20 2020 2020      = [0,1]     
-000015f0: 2320 6d69 6e2f 6d61 7820 7a2d 7261 6e67  # min/max z-rang
-00001600: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00001610: 7072 696f 725f 6967 6e6f 7265 5f6d 6173  prior_ignore_mas
-00001620: 6b20 2020 2020 2020 2020 2020 2020 2020  k               
-00001630: 2020 203d 2046 616c 7365 2020 2020 2020     = False      
-00001640: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001650: 2020 2020 7365 6c66 2e6c 696e 6573 6861      self.linesha
-00001660: 7065 5f6d 6f64 656c 2020 2020 2020 2020  pe_model        
-00001670: 2020 2020 2020 2020 2020 2020 3d20 4669              = Fi
-00001680: 744c 696e 6573 6861 7065 4d6f 6465 6c2e  tLineshapeModel.
-00001690: 4741 5553 5320 0d0a 0d0a 2020 2020 2020  GAUSS ....      
-000016a0: 2020 7365 6c66 2e69 6e69 7469 616c 5f62    self.initial_b
-000016b0: 305f 7368 6966 745f 6d65 7468 6f64 2020  0_shift_method  
-000016c0: 2020 2020 2020 2020 2020 3d20 636f 6e73            = cons
-000016d0: 7461 6e74 732e 4669 7449 6e69 7469 616c  tants.FitInitial
-000016e0: 4230 5368 6966 744d 6574 686f 642e 4d41  B0ShiftMethod.MA
-000016f0: 4e55 414c 0d0a 2020 2020 2020 2020 7365  NUAL..        se
-00001700: 6c66 2e69 6e69 7469 616c 5f62 305f 7661  lf.initial_b0_va
-00001710: 6c75 6520 2020 2020 2020 2020 2020 2020  lue             
-00001720: 2020 2020 2020 3d20 302e 3020 2020 2020        = 0.0     
-00001730: 2020 2320 696e 6974 6961 6c20 6230 2073    # initial b0 s
-00001740: 6869 6674 2069 6e20 687a 0d0a 2020 2020  hift in hz..    
-00001750: 2020 2020 7365 6c66 2e69 6e69 7469 616c      self.initial
-00001760: 5f62 6173 656c 696e 655f 6d65 7468 6f64  _baseline_method
-00001770: 2020 2020 2020 2020 2020 2020 3d20 636f              = co
-00001780: 6e73 7461 6e74 732e 4669 7449 6e69 7469  nstants.FitIniti
-00001790: 616c 4261 7365 6c69 6e65 4d65 7468 6f64  alBaselineMethod
-000017a0: 2e4e 4f4e 450d 0a20 2020 2020 2020 2073  .NONE..        s
-000017b0: 656c 662e 696e 6974 6961 6c5f 6261 7365  elf.initial_base
-000017c0: 6c69 6e65 5f6c 6f77 6573 735f 7769 6474  line_lowess_widt
-000017d0: 6820 2020 2020 2020 203d 2033 352e 3020  h        = 35.0 
-000017e0: 2020 2023 2048 7a0d 0a20 2020 2020 2020     # Hz..       
-000017f0: 2073 656c 662e 696e 6974 6961 6c5f 6261   self.initial_ba
-00001800: 7365 6c69 6e65 5f6c 6f77 6573 735f 6465  seline_lowess_de
-00001810: 6c74 6120 2020 2020 2020 203d 2033 2e32  lta        = 3.2
-00001820: 2020 2020 2023 200d 0a20 2020 2020 2020       # ..       
-00001830: 2073 656c 662e 696e 6974 6961 6c5f 6261   self.initial_ba
-00001840: 7365 6c69 6e65 5f6c 6f77 6573 735f 6967  seline_lowess_ig
-00001850: 6e6f 7265 5f77 6964 7468 203d 2031 352e  nore_width = 15.
-00001860: 3020 2020 2023 2048 7a0d 0a20 2020 2020  0    # Hz..     
-00001870: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
-00001880: 662e 696e 6974 6961 6c5f 6372 5f63 686f  f.initial_cr_cho
-00001890: 5f73 6570 6172 6174 696f 6e20 2020 2020  _separation     
-000018a0: 2020 2020 203d 2054 7275 650d 0a20 2020       = True..   
-000018b0: 2020 2020 2073 656c 662e 696e 6974 6961       self.initia
-000018c0: 6c5f 7065 616b 5f73 6561 7263 685f 6162  l_peak_search_ab
-000018d0: 7320 2020 2020 2020 2020 2020 203d 2046  s            = F
-000018e0: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
-000018f0: 6c66 2e69 6e69 7469 616c 5f73 6d61 6c6c  lf.initial_small
-00001900: 5f70 6561 6b5f 6172 6561 7320 2020 2020  _peak_areas     
-00001910: 2020 2020 2020 3d20 636f 6e73 7461 6e74        = constant
-00001920: 732e 4669 7449 6e69 7469 616c 536d 616c  s.FitInitialSmal
-00001930: 6c50 6561 6b41 7265 6173 2e4e 4141 5f52  lPeakAreas.NAA_R
-00001940: 4154 494f 0d0a 2020 2020 2020 2020 7365  ATIO..        se
-00001950: 6c66 2e69 6e69 7469 616c 5f73 6d61 6c6c  lf.initial_small
-00001960: 5f70 6561 6b5f 6672 6571 7320 2020 2020  _peak_freqs     
-00001970: 2020 2020 2020 3d20 636f 6e73 7461 6e74        = constant
-00001980: 732e 4669 7449 6e69 7469 616c 536d 616c  s.FitInitialSmal
-00001990: 6c50 6561 6b46 7265 7173 2e52 4546 5f50  lPeakFreqs.REF_P
-000019a0: 4541 4b0d 0a20 2020 2020 2020 2073 656c  EAK..        sel
-000019b0: 662e 696e 6974 6961 6c5f 6c69 6e65 7769  f.initial_linewi
-000019c0: 6474 685f 6d65 7468 6f64 2020 2020 2020  dth_method      
-000019d0: 2020 2020 203d 2063 6f6e 7374 616e 7473       = constants
-000019e0: 2e46 6974 496e 6974 6961 6c4c 696e 6577  .FitInitialLinew
-000019f0: 6964 7468 4d65 7468 6f64 2e4d 414e 5541  idthMethod.MANUA
-00001a00: 4c20 0d0a 2020 2020 2020 2020 7365 6c66  L ..        self
-00001a10: 2e69 6e69 7469 616c 5f6c 696e 6577 6964  .initial_linewid
-00001a20: 7468 5f76 616c 7565 2020 2020 2020 2020  th_value        
-00001a30: 2020 2020 3d20 382e 3020 2020 2020 2020      = 8.0       
-00001a40: 2320 696e 6974 6961 6c20 6c69 6e65 7769  # initial linewi
-00001a50: 6474 6820 696e 2068 7a0d 0a20 2020 2020  dth in hz..     
-00001a60: 2020 2073 656c 662e 696e 6974 6961 6c5f     self.initial_
-00001a70: 6c69 6e65 7769 6474 685f 7261 6e67 655f  linewidth_range_
-00001a80: 7374 6172 7420 2020 2020 203d 2031 2e39  start      = 1.9
-00001a90: 2020 2020 2020 2023 204e 4220 7468 6973         # NB this
-00001aa0: 2069 7320 2a4c 572a 206f 7074 696d 697a   is *LW* optimiz
-00001ab0: 6174 696f 6e20 7261 6e67 650d 0a20 2020  ation range..   
-00001ac0: 2020 2020 2073 656c 662e 696e 6974 6961       self.initia
-00001ad0: 6c5f 6c69 6e65 7769 6474 685f 7261 6e67  l_linewidth_rang
-00001ae0: 655f 656e 6420 2020 2020 2020 203d 2034  e_end        = 4
-00001af0: 2e31 2020 2020 2020 2023 2020 7374 6172  .1       #  star
-00001b00: 742f 656e 6420 696e 2070 706d 0d0a 2020  t/end in ppm..  
-00001b10: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
-00001b20: 616c 5f6c 696e 6577 6964 7468 5f66 7564  al_linewidth_fud
-00001b30: 6765 2020 2020 2020 2020 2020 2020 3d20  ge            = 
-00001b40: 312e 3020 2020 2020 2020 2320 4c57 2066  1.0       # LW f
-00001b50: 7564 6765 2076 616c 7565 2028 6c69 6e65  udge value (line
-00001b60: 6172 2073 6361 6c65 7229 0d0a 2020 2020  ar scaler)..    
-00001b70: 2020 2020 7365 6c66 2e69 6e69 7469 616c      self.initial
-00001b80: 5f70 6861 7365 5f6d 6574 686f 6420 2020  _phase_method   
-00001b90: 2020 2020 2020 2020 2020 2020 3d20 636f              = co
-00001ba0: 6e73 7461 6e74 732e 4669 7449 6e69 7469  nstants.FitIniti
-00001bb0: 616c 5068 6173 654d 6574 686f 642e 4d41  alPhaseMethod.MA
-00001bc0: 4e55 414c 2020 0d0a 2020 2020 2020 2020  NUAL  ..        
-00001bd0: 7365 6c66 2e69 6e69 7469 616c 5f70 6861  self.initial_pha
-00001be0: 7365 305f 7661 6c75 6520 2020 2020 2020  se0_value       
-00001bf0: 2020 2020 2020 2020 3d20 302e 3020 2020          = 0.0   
-00001c00: 2020 2020 2320 696e 6974 6961 6c20 7068      # initial ph
-00001c10: 6173 6530 2069 6e20 6465 670d 0a20 2020  ase0 in deg..   
-00001c20: 2020 2020 2073 656c 662e 696e 6974 6961       self.initia
-00001c30: 6c5f 7068 6173 6531 5f76 616c 7565 2020  l_phase1_value  
-00001c40: 2020 2020 2020 2020 2020 2020 203d 2030               = 0
-00001c50: 2e30 2020 2020 2020 2023 2069 6e69 7469  .0       # initi
-00001c60: 616c 2070 6861 7365 3120 696e 2064 6567  al phase1 in deg
-00001c70: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-00001c80: 6e69 7469 616c 5f61 7070 6c79 5f6b 6f5f  nitial_apply_ko_
-00001c90: 6669 6c74 6572 2020 2020 2020 2020 2020  filter          
-00001ca0: 2020 3d20 4661 6c73 650d 0a20 2020 2020    = False..     
-00001cb0: 2020 2073 656c 662e 696e 6974 6961 6c5f     self.initial_
-00001cc0: 6b6f 5f6c 696e 6577 6964 7468 5f6d 696e  ko_linewidth_min
-00001cd0: 696d 756d 2020 2020 2020 203d 2032 300d  imum       = 20.
-00001ce0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00001cf0: 6974 6961 6c5f 6b6f 5f70 6f69 6e74 7320  itial_ko_points 
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 203d 2030 0d0a 2020 2020 2020 2020 7365   = 0..        se
-00001d20: 6c66 2e69 6e69 7469 616c 5f70 6861 7365  lf.initial_phase
-00001d30: 315f 6669 645f 636f 6e73 7461 6e74 2020  1_fid_constant  
-00001d40: 2020 2020 2020 3d20 302e 3020 2020 2020        = 0.0     
-00001d50: 2020 2320 666f 7220 756c 7472 612d 7368    # for ultra-sh
-00001d60: 6f72 7420 4649 4420 6461 7461 2070 6861  ort FID data pha
-00001d70: 7365 3120 756e 7772 6170 0d0a 2020 2020  se1 unwrap..    
-00001d80: 2020 2020 7365 6c66 2e69 6e69 7469 616c      self.initial
-00001d90: 5f6c 6163 5f6d 6574 686f 6420 2020 2020  _lac_method     
-00001da0: 2020 2020 2020 2020 2020 2020 3d20 310d              = 1.
-00001db0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00001dc0: 6974 6961 6c5f 7065 616b 5f6e 6567 6174  itial_peak_negat
-00001dd0: 6976 655f 666c 6167 2020 2020 2020 2020  ive_flag        
-00001de0: 203d 2030 2020 2020 2020 2020 2023 2069   = 0         # i
-00001df0: 652e 2066 6f72 204c 6163 2061 7420 3732  e. for Lac at 72
-00001e00: 6d73 2c20 6e6f 7420 696d 706c 656d 656e  ms, not implemen
-00001e10: 7465 6420 696e 2047 5549 2079 6574 2020  ted in GUI yet  
-00001e20: 2020 0d0a 0d0a 2020 2020 2020 2020 7365    ....        se
-00001e30: 6c66 2e62 6173 656c 696e 655f 6d65 7468  lf.baseline_meth
-00001e40: 6f64 2020 2020 2020 2020 2020 2020 2020  od              
-00001e50: 2020 2020 2020 3d20 636f 6e73 7461 6e74        = constant
-00001e60: 732e 4669 7442 6173 656c 696e 654d 6574  s.FitBaselineMet
-00001e70: 686f 642e 4445 4641 554c 540d 0a20 2020  hod.DEFAULT..   
-00001e80: 2020 2020 2073 656c 662e 6261 7365 6c69       self.baseli
-00001e90: 6e65 5f73 6d6f 6f74 6869 6e67 5f66 6c61  ne_smoothing_fla
-00001ea0: 6720 2020 2020 2020 2020 2020 203d 2046  g            = F
-00001eb0: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
-00001ec0: 6c66 2e62 6173 656c 696e 655f 736b 6970  lf.baseline_skip
-00001ed0: 5f6c 6173 745f 736d 6f6f 7468 2020 2020  _last_smooth    
-00001ee0: 2020 2020 2020 3d20 5472 7565 0d0a 2020        = True..  
-00001ef0: 2020 2020 2020 7365 6c66 2e62 6173 656c        self.basel
-00001f00: 696e 655f 736d 6f6f 7468 696e 675f 7769  ine_smoothing_wi
-00001f10: 6474 6820 2020 2020 2020 2020 2020 3d20  dth           = 
-00001f20: 3230 2e30 2020 2020 2020 2320 696e 2048  20.0      # in H
-00001f30: 7a0d 0a20 2020 2020 2020 2073 656c 662e  z..        self.
-00001f40: 6261 7365 6c69 6e65 5f73 6d6f 6f74 6869  baseline_smoothi
-00001f50: 6e67 5f64 656c 7461 2020 2020 2020 2020  ng_delta        
-00001f60: 2020 203d 2033 2e32 2020 2020 2020 2023     = 3.2       #
-00001f70: 206c 6f77 6573 7320 736d 6f6f 7468 696e   lowess smoothin
-00001f80: 6720 7074 2073 6b69 7020 6465 6c74 6120  g pt skip delta 
-00001f90: 6475 7269 6e67 2077 6176 656c 6574 2062  during wavelet b
-00001fa0: 6173 656c 696e 6520 6361 6c63 0d0a 2020  aseline calc..  
-00001fb0: 2020 2020 2020 7365 6c66 2e62 6173 656c        self.basel
-00001fc0: 696e 655f 756e 6465 7265 7374 696d 6174  ine_underestimat
-00001fd0: 6520 2020 2020 2020 2020 2020 2020 3d20  e             = 
-00001fe0: 302e 3020 2020 2020 2020 2320 696e 2025  0.0       # in %
-00001ff0: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-00002000: 6173 656c 696e 655f 7370 6c69 6e65 5f6e  aseline_spline_n
-00002010: 6b6e 6f74 7320 2020 2020 2020 2020 2020  knots           
-00002020: 2020 3d20 3130 0d0a 2020 2020 2020 2020    = 10..        
-00002030: 7365 6c66 2e62 6173 656c 696e 655f 7370  self.baseline_sp
-00002040: 6c69 6e65 5f73 7061 6369 6e67 2020 2020  line_spacing    
-00002050: 2020 2020 2020 2020 3d20 3130 2020 2020          = 10    
-00002060: 2020 2020 2320 696e 2070 6f69 6e74 730d      # in points.
-00002070: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
-00002080: 7365 6c69 6e65 5f73 706c 696e 655f 6f72  seline_spline_or
-00002090: 6465 7220 2020 2020 2020 2020 2020 2020  der             
-000020a0: 203d 2033 0d0a 2020 2020 2020 2020 7365   = 3..        se
-000020b0: 6c66 2e62 6173 656c 696e 655f 7761 7665  lf.baseline_wave
-000020c0: 6c65 745f 7363 616c 6520 2020 2020 2020  let_scale       
-000020d0: 2020 2020 2020 3d20 340d 0a20 2020 2020        = 4..     
-000020e0: 2020 2073 656c 662e 6261 7365 6c69 6e65     self.baseline
-000020f0: 5f77 6176 656c 6574 5f6d 696e 5f64 7961  _wavelet_min_dya
-00002100: 6420 2020 2020 2020 2020 203d 2035 2e30  d          = 5.0
-00002110: 2020 2023 2066 6c6f 6174 2c20 696e 2048     # float, in H
-00002120: 7a20 6d69 6e20 7468 7265 7368 6f6c 640d  z min threshold.
-00002130: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
-00002140: 7365 6c69 6e65 5f77 6176 656c 6574 5f73  seline_wavelet_s
-00002150: 6872 696e 6b61 6765 5f66 6c61 6720 2020  hrinkage_flag   
-00002160: 203d 2030 2020 2020 2023 2066 6c67 202d   = 0     # flg -
-00002170: 2064 6f20 7761 7665 6c65 7420 7368 7269   do wavelet shri
-00002180: 6e6b 6167 6520 302f 310d 0a20 2020 2020  nkage 0/1..     
-00002190: 2020 2073 656c 662e 6261 7365 6c69 6e65     self.baseline
-000021a0: 5f77 6176 656c 6574 5f69 6e76 6172 6961  _wavelet_invaria
-000021b0: 6e63 655f 6c61 6720 2020 203d 2032 2020  nce_lag    = 2  
-000021c0: 2020 2023 2077 6176 656c 6574 2069 6e76     # wavelet inv
-000021d0: 6172 6961 6e63 6520 6c61 6720 4641 4354  ariance lag FACT
-000021e0: 4f52 2028 2b2f 2d20 706f 696e 7473 290d  OR (+/- points).
-000021f0: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
-00002200: 7365 6c69 6e65 5f77 6176 656c 6574 5f69  seline_wavelet_i
-00002210: 6e76 6172 6961 6e63 655f 7265 636f 6d62  nvariance_recomb
-00002220: 696e 6520 3d20 3020 2023 2072 6563 6f6d  ine = 0  # recom
-00002230: 6269 6e61 7469 6f6e 206d 6574 686f 6420  bination method 
-00002240: 666f 7220 696e 7661 7269 616e 6365 206c  for invariance l
-00002250: 6167 730d 0a0d 0a20 2020 2020 2020 2073  ags....        s
-00002260: 656c 662e 6d61 6372 6f6d 6f6c 5f6d 6f64  elf.macromol_mod
-00002270: 656c 2020 2020 2020 2020 2020 2020 2020  el              
-00002280: 2020 2020 2020 2020 2020 2020 203d 2046               = F
-00002290: 6974 4d61 6372 6f6d 6f6c 6563 756c 654d  itMacromoleculeM
-000022a0: 6574 686f 642e 4445 4641 554c 540d 0a20  ethod.DEFAULT.. 
-000022b0: 2020 2020 2020 2073 656c 662e 6d61 6372         self.macr
-000022c0: 6f6d 6f6c 5f73 696e 676c 655f 6261 7369  omol_single_basi
-000022d0: 735f 6461 7461 7365 7420 2020 2020 2020  s_dataset       
-000022e0: 2020 2020 203d 204e 6f6e 650d 0a20 2020       = None..   
-000022f0: 2020 2020 2073 656c 662e 6d61 6372 6f6d       self.macrom
-00002300: 6f6c 5f73 696e 676c 655f 6261 7369 735f  ol_single_basis_
-00002310: 6461 7461 7365 745f 6964 2020 2020 2020  dataset_id      
-00002320: 2020 203d 2027 2720 0d0a 2020 2020 2020     = '' ..      
-00002330: 2020 7365 6c66 2e6d 6163 726f 6d6f 6c5f    self.macromol_
-00002340: 7369 6e67 6c65 5f62 6173 6973 5f64 6174  single_basis_dat
-00002350: 6173 6574 5f73 7461 7274 5f61 7265 6120  aset_start_area 
-00002360: 3d20 312e 300d 0a0d 0a20 2020 2020 2020  = 1.0....       
-00002370: 2073 656c 662e 6f70 7469 6d69 7a65 5f6d   self.optimize_m
-00002380: 6574 686f 6420 2020 2020 2020 2020 2020  ethod           
-00002390: 2020 2020 2020 2020 203d 2063 6f6e 7374           = const
-000023a0: 616e 7473 2e46 6974 4f70 7469 6d69 7a65  ants.FitOptimize
-000023b0: 4d65 7468 6f64 2e43 4f4e 5354 5241 494e  Method.CONSTRAIN
-000023c0: 4544 5f4c 4556 454e 4245 5247 5f4d 4152  ED_LEVENBERG_MAR
-000023d0: 5155 4152 4454 0d0a 2020 2020 2020 2020  QUARDT..        
-000023e0: 7365 6c66 2e6f 7074 696d 697a 655f 7363  self.optimize_sc
-000023f0: 616c 696e 675f 666c 6167 2020 2020 2020  aling_flag      
-00002400: 2020 2020 2020 2020 3d20 4661 6c73 650d          = False.
-00002410: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-00002420: 7469 6d69 7a65 5f73 746f 705f 746f 6c65  timize_stop_tole
-00002430: 7261 6e63 6520 2020 2020 2020 2020 2020  rance           
-00002440: 203d 2030 2e30 3035 2020 2020 2020 2020   = 0.005        
-00002450: 2023 2066 6974 2074 6f6c 6572 616e 6365   # fit tolerance
-00002460: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-00002470: 7074 696d 697a 655f 6d61 785f 6974 6572  ptimize_max_iter
-00002480: 6174 696f 6e73 2020 2020 2020 2020 2020  ations          
-00002490: 2020 3d20 3130 3020 2020 2020 2020 2020    = 100         
-000024a0: 2020 2320 6d61 7820 6974 6572 6174 696f    # max iteratio
-000024b0: 6e73 0d0a 2020 2020 2020 2020 7365 6c66  ns..        self
-000024c0: 2e6f 7074 696d 697a 655f 6c69 6d69 7473  .optimize_limits
-000024d0: 5f72 616e 6765 5f61 7265 6120 2020 2020  _range_area     
-000024e0: 2020 2020 3d20 3530 2e30 2020 2020 2020      = 50.0      
-000024f0: 2020 2020 2320 250d 0a20 2020 2020 2020      # %..       
-00002500: 2073 656c 662e 6f70 7469 6d69 7a65 5f6c   self.optimize_l
-00002510: 696d 6974 735f 7261 6e67 655f 7070 6d20  imits_range_ppm 
-00002520: 2020 2020 2020 2020 203d 2038 2e30 2020           = 8.0  
-00002530: 2020 2020 2020 2020 2023 2048 7a0d 0a20           # Hz.. 
-00002540: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
-00002550: 6d69 7a65 5f6c 696d 6974 735f 7261 6e67  mize_limits_rang
-00002560: 655f 7068 6173 6530 2020 2020 2020 203d  e_phase0       =
-00002570: 2034 352e 3020 2020 2020 2020 2020 2023   45.0          #
-00002580: 2064 6567 0d0a 2020 2020 2020 2020 7365   deg..        se
-00002590: 6c66 2e6f 7074 696d 697a 655f 6c69 6d69  lf.optimize_limi
-000025a0: 7473 5f72 616e 6765 5f70 6861 7365 3120  ts_range_phase1 
-000025b0: 2020 2020 2020 3d20 3230 3030 2e30 2020        = 2000.0  
-000025c0: 2020 2020 2020 2320 6465 670d 0a20 2020        # deg..   
-000025d0: 2020 2020 2073 656c 662e 6f70 7469 6d69       self.optimi
-000025e0: 7a65 5f6c 696d 6974 735f 6d61 785f 6c69  ze_limits_max_li
-000025f0: 6e65 7769 6474 6820 2020 2020 203d 2031  newidth      = 1
-00002600: 2e30 0d0a 2020 2020 2020 2020 7365 6c66  .0..        self
-00002610: 2e6f 7074 696d 697a 655f 6c69 6d69 7473  .optimize_limits
-00002620: 5f6d 696e 5f6c 696e 6577 6964 7468 2020  _min_linewidth  
-00002630: 2020 2020 3d20 302e 3034 0d0a 2020 2020      = 0.04..    
-00002640: 2020 2020 7365 6c66 2e6f 7074 696d 697a      self.optimiz
-00002650: 655f 676c 6f62 616c 5f69 7465 7261 7469  e_global_iterati
-00002660: 6f6e 7320 2020 2020 2020 2020 3d20 3130  ons         = 10
-00002670: 2020 2020 2020 2020 2020 2020 2023 2067               # g
-00002680: 6c6f 6261 6c20 6974 6572 6174 696f 6e73  lobal iterations
-00002690: 2066 6f72 206f 7074 696d 697a 6174 696f   for optimizatio
-000026a0: 6e20 6d65 7461 622f 6261 7365 0d0a 2020  n metab/base..  
-000026b0: 2020 2020 2020 7365 6c66 2e6f 7074 696d        self.optim
-000026c0: 697a 655f 7765 6967 6874 735f 6d65 7468  ize_weights_meth
-000026d0: 6f64 2020 2020 2020 2020 2020 2020 3d20  od            = 
-000026e0: 636f 6e73 7461 6e74 732e 4669 744f 7074  constants.FitOpt
-000026f0: 696d 697a 6557 6569 6768 7473 4d65 7468  imizeWeightsMeth
-00002700: 6f64 2e4c 4f43 414c 5f57 4549 4748 5449  od.LOCAL_WEIGHTI
-00002710: 4e47 0d0a 2020 2020 2020 2020 7365 6c66  NG..        self
-00002720: 2e6f 7074 696d 697a 655f 7765 6967 6874  .optimize_weight
-00002730: 735f 7363 616c 655f 6661 6374 6f72 2020  s_scale_factor  
-00002740: 2020 2020 3d20 3130 3030 2e30 2020 2020      = 1000.0    
-00002750: 2020 2020 2320 6d75 6c74 6970 6c69 6572      # multiplier
-00002760: 2066 6f72 2077 6569 6768 7465 6420 6f70   for weighted op
-00002770: 7469 6d69 7a61 7469 6f6e 0d0a 2020 2020  timization..    
-00002780: 2020 2020 7365 6c66 2e6f 7074 696d 697a      self.optimiz
-00002790: 655f 7765 6967 6874 735f 7769 6474 685f  e_weights_width_
-000027a0: 6661 6374 6f72 2020 2020 2020 3d20 362e  factor      = 6.
-000027b0: 3020 2020 2020 2020 2020 2020 2320 6d75  0           # mu
-000027c0: 6c74 6970 6c69 6572 2066 6f72 2077 6964  ltiplier for wid
-000027d0: 7468 206f 6620 7765 6967 6874 6564 2072  th of weighted r
-000027e0: 6567 696f 6e73 0d0a 2020 2020 2020 2020  egions..        
-000027f0: 7365 6c66 2e6f 7074 696d 697a 655f 7765  self.optimize_we
-00002800: 6967 6874 735f 7761 7465 725f 666c 6167  ights_water_flag
-00002810: 2020 2020 2020 2020 3d20 5472 7565 2020          = True  
-00002820: 2020 2020 2020 2020 2320 4f66 662f 4f6e          # Off/On
-00002830: 207a 6572 6f20 7761 7465 7220 7265 6769   zero water regi
-00002840: 6f6e 0d0a 2020 2020 2020 2020 7365 6c66  on..        self
-00002850: 2e6f 7074 696d 697a 655f 7765 6967 6874  .optimize_weight
-00002860: 735f 7761 7465 725f 7374 6172 7420 2020  s_water_start   
-00002870: 2020 2020 3d20 342e 3120 2020 2020 2020      = 4.1       
-00002880: 2020 2020 2320 7761 7465 7220 7375 7070      # water supp
-00002890: 7265 7373 696f 6e20 6166 6665 6374 6564  ression affected
-000028a0: 2072 6567 696f 6e0d 0a20 2020 2020 2020   region..       
-000028b0: 2073 656c 662e 6f70 7469 6d69 7a65 5f77   self.optimize_w
-000028c0: 6569 6768 7473 5f77 6174 6572 5f65 6e64  eights_water_end
-000028d0: 2020 2020 2020 2020 203d 2035 2e33 2020           = 5.3  
-000028e0: 2020 2020 2020 2020 2023 2020 7374 6172           #  star
-000028f0: 742f 656e 6420 696e 2070 706d 0d0a 2020  t/end in ppm..  
-00002900: 2020 2020 2020 7365 6c66 2e6f 7074 696d        self.optim
-00002910: 697a 655f 7765 6967 6874 735f 6c69 7069  ize_weights_lipi
-00002920: 645f 666c 6167 2020 2020 2020 2020 3d20  d_flag        = 
-00002930: 4661 6c73 6520 2020 2020 2020 2020 2320  False         # 
-00002940: 4f66 662f 4f6e 207a 6572 6f20 6c69 7069  Off/On zero lipi
-00002950: 6420 7265 6769 6f6e 0d0a 2020 2020 2020  d region..      
-00002960: 2020 7365 6c66 2e6f 7074 696d 697a 655f    self.optimize_
-00002970: 7765 6967 6874 735f 6c69 7069 645f 7374  weights_lipid_st
-00002980: 6172 7420 2020 2020 2020 3d20 2d30 2e35  art       = -0.5
-00002990: 2020 2020 2020 2020 2020 2320 7265 6769            # regi
-000029a0: 6f6e 2077 6974 6820 6c69 7069 6420 2d20  on with lipid - 
-000029b0: 6c6f 7765 7220 7765 6967 6874 2068 6572  lower weight her
-000029c0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-000029d0: 6f70 7469 6d69 7a65 5f77 6569 6768 7473  optimize_weights
-000029e0: 5f6c 6970 6964 5f65 6e64 2020 2020 2020  _lipid_end      
-000029f0: 2020 203d 2031 2e31 2020 2020 2020 2020     = 1.1        
-00002a00: 2020 2023 2020 7374 6172 742f 656e 6420     #  start/end 
-00002a10: 696e 2070 706d 0d0a 2020 2020 2020 2020  in ppm..        
-00002a20: 7365 6c66 2e6f 7074 696d 697a 655f 7765  self.optimize_we
-00002a30: 6967 6874 735f 736d 616c 6c5f 7065 616b  ights_small_peak
-00002a40: 5f66 6163 746f 7220 3d20 312e 3020 2020  _factor = 1.0   
-00002a50: 2020 2020 2020 2020 2320 7363 616c 6520          # scale 
-00002a60: 6d75 6c74 6970 6c65 2066 6f72 2073 6d61  multiple for sma
-00002a70: 6c6c 2070 6561 6b20 7265 6769 6f6e 730d  ll peak regions.
-00002a80: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00002a90: 636f 6e66 6964 656e 6365 5f69 6e74 6572  confidence_inter
-00002aa0: 7661 6c73 5f66 6c61 6720 2020 2020 2020  vals_flag       
-00002ab0: 2020 203d 2046 616c 7365 0d0a 2020 2020     = False..    
-00002ac0: 2020 2020 7365 6c66 2e63 6f6e 6669 6465      self.confide
-00002ad0: 6e63 655f 616c 7068 6120 2020 2020 2020  nce_alpha       
-00002ae0: 2020 2020 2020 2020 2020 2020 3d20 302e              = 0.
-00002af0: 3835 0d0a 2020 2020 2020 2020 7365 6c66  85..        self
-00002b00: 2e63 6f6e 6669 6465 6e63 655f 6172 6561  .confidence_area
-00002b10: 5f66 6c61 6720 2020 2020 2020 2020 2020  _flag           
-00002b20: 2020 2020 3d20 4661 6c73 650d 0a20 2020      = False..   
-00002b30: 2020 2020 2073 656c 662e 636f 6e66 6964       self.confid
-00002b40: 656e 6365 5f70 706d 5f66 6c61 6720 2020  ence_ppm_flag   
-00002b50: 2020 2020 2020 2020 2020 2020 203d 2046               = F
-00002b60: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
-00002b70: 6c66 2e63 6f6e 6669 6465 6e63 655f 6c69  lf.confidence_li
-00002b80: 6e65 7769 6474 685f 666c 6167 2020 2020  newidth_flag    
-00002b90: 2020 2020 2020 3d20 4661 6c73 650d 0a20        = False.. 
-00002ba0: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
-00002bb0: 6964 656e 6365 5f70 6861 7365 5f66 6c61  idence_phase_fla
-00002bc0: 6720 2020 2020 2020 2020 2020 2020 203d  g              =
-00002bd0: 2046 616c 7365 0d0a 0d0a 2020 2020 2020   False....      
-00002be0: 2020 7365 6c66 2e63 7261 6d65 725f 7261    self.cramer_ra
-00002bf0: 6f5f 666c 6167 2020 2020 2020 2020 2020  o_flag          
-00002c00: 2020 2020 2020 2020 2020 3d20 5472 7565            = True
-00002c10: 2020 2020 2020 2320 666c 6167 2074 6f20        # flag to 
-00002c20: 646f 2063 7261 6d65 722d 7261 6f20 626f  do cramer-rao bo
-00002c30: 756e 6420 6361 6c63 756c 6174 696f 6e73  und calculations
-00002c40: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00002c50: 7261 6d65 725f 7261 6f5f 7070 6d5f 7374  ramer_rao_ppm_st
-00002c60: 6172 7420 2020 2020 2020 2020 2020 2020  art             
-00002c70: 2020 3d20 2d38 2e30 2020 2020 2020 2320    = -8.0      # 
-00002c80: 7070 6d20 7261 6e67 6520 666f 7220 6e6f  ppm range for no
-00002c90: 6973 6520 6d65 6173 7572 656d 656e 7420  ise measurement 
-00002ca0: 746f 2063 616c 630d 0a20 2020 2020 2020  to calc..       
-00002cb0: 2073 656c 662e 6372 616d 6572 5f72 616f   self.cramer_rao
-00002cc0: 5f70 706d 5f65 6e64 2020 2020 2020 2020  _ppm_end        
-00002cd0: 2020 2020 2020 2020 203d 202d 362e 3020           = -6.0 
-00002ce0: 2020 2020 2023 2020 7468 6520 7369 676d       #  the sigm
-00002cf0: 6120 7371 7561 7265 6420 7661 7269 616e  a squared varian
-00002d00: 6365 2e0d 0a0d 0a20 2020 2020 2020 2023  ce.....        #
-00002d10: 2047 4953 4f20 616c 676f 7269 7468 6d20   GISO algorithm 
-00002d20: 696e 7075 7420 6f62 6a65 6374 730d 0a20  input objects.. 
-00002d30: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
-00002d40: 7220 2020 2020 2020 2020 2020 2020 203d  r              =
-00002d50: 206d 7273 5f70 7269 6f72 2e50 7269 6f72   mrs_prior.Prior
-00002d60: 2829 0d0a 0d0a 2020 2020 2020 2020 6966  ()....        if
-00002d70: 2061 7474 7269 6275 7465 7320 6973 206e   attributes is n
-00002d80: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00002d90: 2020 2020 2020 7365 6c66 2e69 6e66 6c61        self.infla
-00002da0: 7465 2861 7474 7269 6275 7465 7329 0d0a  te(attributes)..
-00002db0: 0d0a 2020 2020 2323 2323 2320 5374 616e  ..    ##### Stan
-00002dc0: 6461 7264 204d 6574 686f 6473 2061 6e64  dard Methods and
-00002dd0: 2050 726f 7065 7274 6965 7320 2323 2323   Properties ####
-00002de0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002df0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002e00: 230d 0a0d 0a20 2020 2064 6566 205f 5f73  #....    def __s
-00002e10: 7472 5f5f 2873 656c 6629 3a0d 0a20 2020  tr__(self):..   
-00002e20: 2020 2020 206c 696e 6573 203d 205b 5d0d       lines = [].
-00002e30: 0a20 2020 2020 2020 206c 696e 6573 2e61  .        lines.a
-00002e40: 7070 656e 6428 222d 2d2d 2d2d 2d2d 207b  ppend("------- {
-00002e50: 307d 204f 626a 6563 7420 2d2d 2d2d 2d2d  0} Object ------
-00002e60: 2d22 2e66 6f72 6d61 7428 7365 6c66 2e5f  -".format(self._
-00002e70: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
-00002e80: 5f29 290d 0a20 2020 2020 2020 206c 696e  _))..        lin
-00002e90: 6573 2e61 7070 656e 6428 224e 6f74 2063  es.append("Not c
-00002ea0: 7572 7265 6e74 6c79 2077 7269 7474 656e  urrently written
-00002eb0: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00002ec0: 726e 2027 5c6e 272e 6a6f 696e 286c 696e  rn '\n'.join(lin
-00002ed0: 6573 290d 0a0d 0a0d 0a20 2020 2064 6566  es)......    def
-00002ee0: 2064 6566 6c61 7465 2873 656c 662c 2066   deflate(self, f
-00002ef0: 6c61 766f 723d 4465 666c 6174 652e 4554  lavor=Deflate.ET
-00002f00: 5245 4529 3a0d 0a20 2020 2020 2020 2069  REE):..        i
-00002f10: 6620 666c 6176 6f72 203d 3d20 4465 666c  f flavor == Defl
-00002f20: 6174 652e 4554 5245 453a 0d0a 2020 2020  ate.ETREE:..    
-00002f30: 2020 2020 2020 2020 6520 3d20 456c 656d          e = Elem
-00002f40: 656e 7428 2273 6574 7469 6e67 7322 2c20  ent("settings", 
-00002f50: 7b22 7665 7273 696f 6e22 203a 2073 656c  {"version" : sel
-00002f60: 662e 584d 4c5f 5645 5253 494f 4e7d 290d  f.XML_VERSION}).
-00002f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00002fa0: 2020 2020 2020 2020 2020 2023 2054 6865             # The
-00002fb0: 7365 2061 7474 7269 6275 7465 7320 6172  se attributes ar
-00002fc0: 6520 616c 6c20 6c69 7374 732e 0d0a 2020  e all lists...  
-00002fd0: 2020 2020 2020 2020 2020 666f 7220 6174            for at
-00002fe0: 7472 6962 7574 6520 696e 2028 2270 7269  tribute in ("pri
-00002ff0: 6f72 5f6c 6973 7422 2c20 2270 7269 6f72  or_list", "prior
-00003000: 5f61 7265 615f 7363 616c 6522 2c20 0d0a  _area_scale", ..
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00003030: 7269 6f72 5f70 6561 6b5f 7070 6d22 2c20  rior_peak_ppm", 
-00003040: 2270 7269 6f72 5f73 6561 7263 685f 7070  "prior_search_pp
-00003050: 6d22 2c0d 0a20 2020 2020 2020 2020 2020  m",..           
-00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003070: 2020 2022 7072 696f 725f 6462 5f70 706d     "prior_db_ppm
-00003080: 222c 2022 7072 696f 725f 6669 785f 7432  ", "prior_fix_t2
-00003090: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 2020 2270 7269 6f72 5f73 6561 7263 685f    "prior_search_
-000030c0: 7068 3022 2c0d 0a20 2020 2020 2020 2020  ph0",..         
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 2020 2020 2022 7072 696f 725f 7872 616e       "prior_xran
-000030f0: 6765 222c 2022 7072 696f 725f 7972 616e  ge", "prior_yran
-00003100: 6765 222c 0d0a 2020 2020 2020 2020 2020  ge",..          
+00001540: 2020 203d 2046 6974 4d61 6372 6f6d 6f6c     = FitMacromol
+00001550: 6563 756c 654d 6574 686f 642e 4445 4641  eculeMethod.DEFA
+00001560: 554c 540d 0a20 2020 2020 2020 2073 656c  ULT..        sel
+00001570: 662e 6d61 6372 6f6d 6f6c 5f73 696e 676c  f.macromol_singl
+00001580: 655f 6261 7369 735f 6461 7461 7365 7420  e_basis_dataset 
+00001590: 2020 2020 2020 2020 2020 203d 204e 6f6e             = Non
+000015a0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+000015b0: 6d61 6372 6f6d 6f6c 5f73 696e 676c 655f  macromol_single_
+000015c0: 6261 7369 735f 6461 7461 7365 745f 6964  basis_dataset_id
+000015d0: 2020 2020 2020 2020 203d 2027 2720 0d0a           = '' ..
+000015e0: 2020 2020 2020 2020 7365 6c66 2e6d 6163          self.mac
+000015f0: 726f 6d6f 6c5f 7369 6e67 6c65 5f62 6173  romol_single_bas
+00001600: 6973 5f64 6174 6173 6574 5f66 6e61 6d65  is_dataset_fname
+00001610: 2020 2020 2020 203d 2027 2720 0d0a 2020         = '' ..  
+00001620: 2020 2020 2020 7365 6c66 2e6d 6163 726f        self.macro
+00001630: 6d6f 6c5f 7369 6e67 6c65 5f62 6173 6973  mol_single_basis
+00001640: 5f64 6174 6173 6574 5f69 6e69 7476 616c  _dataset_initval
+00001650: 2020 2020 203d 2046 6974 4d61 6372 6f6d       = FitMacrom
+00001660: 6f6c 6563 756c 654d 6574 686f 6449 6e69  oleculeMethodIni
+00001670: 7456 616c 2e44 4546 4155 4c54 0d0a 2020  tVal.DEFAULT..  
+00001680: 2020 2020 2020 7365 6c66 2e6d 6163 726f        self.macro
+00001690: 6d6f 6c5f 7369 6e67 6c65 5f62 6173 6973  mol_single_basis
+000016a0: 5f64 6174 6173 6574 5f73 7461 7274 5f61  _dataset_start_a
+000016b0: 7265 6120 3d20 312e 300d 0a20 2020 2020  rea = 1.0..     
+000016c0: 2020 2073 656c 662e 6d61 6372 6f6d 6f6c     self.macromol
+000016d0: 5f73 696e 676c 655f 6261 7369 735f 6461  _single_basis_da
+000016e0: 7461 7365 745f 7374 6172 745f 6675 6467  taset_start_fudg
+000016f0: 6520 3d20 312e 3020 2020 2020 2020 2023  e = 1.0        #
+00001700: 206d 756c 7469 706c 6965 722c 2074 696d   multiplier, tim
+00001710: 6573 2073 7461 7274 5f61 7265 610d 0a20  es start_area.. 
+00001720: 2020 2020 2020 2073 656c 662e 6d61 6372         self.macr
+00001730: 6f6d 6f6c 5f73 696e 676c 655f 6261 7369  omol_single_basi
+00001740: 735f 6461 7461 7365 745f 7070 6d5f 7374  s_dataset_ppm_st
+00001750: 6172 7420 2020 3d20 312e 3520 2020 2020  art   = 1.5     
+00001760: 2020 2023 2070 706d 0d0a 2020 2020 2020     # ppm..      
+00001770: 2020 7365 6c66 2e6d 6163 726f 6d6f 6c5f    self.macromol_
+00001780: 7369 6e67 6c65 5f62 6173 6973 5f64 6174  single_basis_dat
+00001790: 6173 6574 5f70 706d 5f65 6e64 2020 2020  aset_ppm_end    
+000017a0: 203d 2031 2e38 2020 2020 2020 2020 2320   = 1.8        # 
+000017b0: 7070 6d0d 0a20 2020 2020 2020 2073 656c  ppm..        sel
+000017c0: 662e 6d61 6372 6f6d 6f6c 5f73 696e 676c  f.macromol_singl
+000017d0: 655f 6261 7369 735f 6461 7461 7365 745f  e_basis_dataset_
+000017e0: 6c69 6d69 745f 6d61 7820 2020 3d20 312e  limit_max   = 1.
+000017f0: 3520 2020 2020 2020 2023 206d 756c 7469  5        # multi
+00001800: 706c 6965 7220 7469 6d65 7320 7374 6172  plier times star
+00001810: 7420 7661 6c75 650d 0a20 2020 2020 2020  t value..       
+00001820: 2073 656c 662e 6d61 6372 6f6d 6f6c 5f73   self.macromol_s
+00001830: 696e 676c 655f 6261 7369 735f 6461 7461  ingle_basis_data
+00001840: 7365 745f 6c69 6d69 745f 6d69 6e20 2020  set_limit_min   
+00001850: 3d20 302e 3030 3030 3031 2020 2023 206d  = 0.000001   # m
+00001860: 756c 7469 706c 6965 7220 7469 6d65 7320  ultiplier times 
+00001870: 7374 6172 7420 7661 6c75 652c 206e 6f6e  start value, non
+00001880: 2d6e 6567 6174 6976 650d 0a0d 0a20 2020  -negative....   
+00001890: 2020 2020 2073 656c 662e 6f70 7469 6d69       self.optimi
+000018a0: 7a65 5f6d 6574 686f 6420 2020 2020 2020  ze_method       
+000018b0: 2020 2020 2020 2020 2020 2020 203d 2063               = c
+000018c0: 6f6e 7374 616e 7473 2e46 6974 4f70 7469  onstants.FitOpti
+000018d0: 6d69 7a65 4d65 7468 6f64 2e43 4f4e 5354  mizeMethod.CONST
+000018e0: 5241 494e 4544 5f4c 4556 454e 4245 5247  RAINED_LEVENBERG
+000018f0: 5f4d 4152 5155 4152 4454 0d0a 2020 2020  _MARQUARDT..    
+00001900: 2020 2020 7365 6c66 2e6f 7074 696d 697a      self.optimiz
+00001910: 655f 7363 616c 696e 675f 666c 6167 2020  e_scaling_flag  
+00001920: 2020 2020 2020 2020 2020 2020 3d20 4661              = Fa
+00001930: 6c73 650d 0a20 2020 2020 2020 2073 656c  lse..        sel
+00001940: 662e 6f70 7469 6d69 7a65 5f73 746f 705f  f.optimize_stop_
+00001950: 746f 6c65 7261 6e63 6520 2020 2020 2020  tolerance       
+00001960: 2020 2020 203d 2030 2e30 3035 2020 2020       = 0.005    
+00001970: 2020 2020 2023 2066 6974 2074 6f6c 6572       # fit toler
+00001980: 616e 6365 0d0a 2020 2020 2020 2020 7365  ance..        se
+00001990: 6c66 2e6f 7074 696d 697a 655f 6d61 785f  lf.optimize_max_
+000019a0: 6974 6572 6174 696f 6e73 2020 2020 2020  iterations      
+000019b0: 2020 2020 2020 3d20 3130 3020 2020 2020        = 100     
+000019c0: 2020 2020 2020 2320 6d61 7820 6974 6572        # max iter
+000019d0: 6174 696f 6e73 0d0a 2020 2020 2020 2020  ations..        
+000019e0: 7365 6c66 2e6f 7074 696d 697a 655f 676c  self.optimize_gl
+000019f0: 6f62 616c 5f69 7465 7261 7469 6f6e 7320  obal_iterations 
+00001a00: 2020 2020 2020 2020 3d20 3130 2020 2020          = 10    
+00001a10: 2020 2020 2020 2020 2023 2067 6c6f 6261           # globa
+00001a20: 6c20 6974 6572 6174 696f 6e73 2066 6f72  l iterations for
+00001a30: 206f 7074 696d 697a 6174 696f 6e20 6d65   optimization me
+00001a40: 7461 622f 6261 7365 0d0a 2020 2020 2020  tab/base..      
+00001a50: 2020 7365 6c66 2e6f 7074 696d 697a 655f    self.optimize_
+00001a60: 7765 6967 6874 735f 6d65 7468 6f64 2020  weights_method  
+00001a70: 2020 2020 2020 2020 2020 3d20 636f 6e73            = cons
+00001a80: 7461 6e74 732e 4669 744f 7074 696d 697a  tants.FitOptimiz
+00001a90: 6557 6569 6768 7473 4d65 7468 6f64 2e4c  eWeightsMethod.L
+00001aa0: 4f43 414c 5f57 4549 4748 5449 4e47 0d0a  OCAL_WEIGHTING..
+00001ab0: 2020 2020 2020 2020 7365 6c66 2e6f 7074          self.opt
+00001ac0: 696d 697a 655f 7765 6967 6874 735f 7363  imize_weights_sc
+00001ad0: 616c 655f 6661 6374 6f72 2020 2020 2020  ale_factor      
+00001ae0: 3d20 3130 3030 2e30 2020 2020 2020 2020  = 1000.0        
+00001af0: 2320 6d75 6c74 6970 6c69 6572 2066 6f72  # multiplier for
+00001b00: 2077 6569 6768 7465 6420 6f70 7469 6d69   weighted optimi
+00001b10: 7a61 7469 6f6e 0d0a 2020 2020 2020 2020  zation..        
+00001b20: 7365 6c66 2e6f 7074 696d 697a 655f 7765  self.optimize_we
+00001b30: 6967 6874 735f 7769 6474 685f 6661 6374  ights_width_fact
+00001b40: 6f72 2020 2020 2020 3d20 362e 3020 2020  or      = 6.0   
+00001b50: 2020 2020 2020 2020 2320 6d75 6c74 6970          # multip
+00001b60: 6c69 6572 2066 6f72 2077 6964 7468 206f  lier for width o
+00001b70: 6620 7765 6967 6874 6564 2072 6567 696f  f weighted regio
+00001b80: 6e73 0d0a 2020 2020 2020 2020 7365 6c66  ns..        self
+00001b90: 2e6f 7074 696d 697a 655f 7765 6967 6874  .optimize_weight
+00001ba0: 735f 7761 7465 725f 666c 6167 2020 2020  s_water_flag    
+00001bb0: 2020 2020 3d20 5472 7565 2020 2020 2020      = True      
+00001bc0: 2020 2020 2320 4f66 662f 4f6e 207a 6572      # Off/On zer
+00001bd0: 6f20 7761 7465 7220 7265 6769 6f6e 0d0a  o water region..
+00001be0: 2020 2020 2020 2020 7365 6c66 2e6f 7074          self.opt
+00001bf0: 696d 697a 655f 7765 6967 6874 735f 7761  imize_weights_wa
+00001c00: 7465 725f 7374 6172 7420 2020 2020 2020  ter_start       
+00001c10: 3d20 342e 3120 2020 2020 2020 2020 2020  = 4.1           
+00001c20: 2320 7761 7465 7220 7375 7070 7265 7373  # water suppress
+00001c30: 696f 6e20 6166 6665 6374 6564 2072 6567  ion affected reg
+00001c40: 696f 6e0d 0a20 2020 2020 2020 2073 656c  ion..        sel
+00001c50: 662e 6f70 7469 6d69 7a65 5f77 6569 6768  f.optimize_weigh
+00001c60: 7473 5f77 6174 6572 5f65 6e64 2020 2020  ts_water_end    
+00001c70: 2020 2020 203d 2035 2e33 2020 2020 2020       = 5.3      
+00001c80: 2020 2020 2023 2020 7374 6172 742f 656e       #  start/en
+00001c90: 6420 696e 2070 706d 0d0a 2020 2020 2020  d in ppm..      
+00001ca0: 2020 7365 6c66 2e6f 7074 696d 697a 655f    self.optimize_
+00001cb0: 7765 6967 6874 735f 6c69 7069 645f 666c  weights_lipid_fl
+00001cc0: 6167 2020 2020 2020 2020 3d20 4661 6c73  ag        = Fals
+00001cd0: 6520 2020 2020 2020 2020 2320 4f66 662f  e         # Off/
+00001ce0: 4f6e 207a 6572 6f20 6c69 7069 6420 7265  On zero lipid re
+00001cf0: 6769 6f6e 0d0a 2020 2020 2020 2020 7365  gion..        se
+00001d00: 6c66 2e6f 7074 696d 697a 655f 7765 6967  lf.optimize_weig
+00001d10: 6874 735f 6c69 7069 645f 7374 6172 7420  hts_lipid_start 
+00001d20: 2020 2020 2020 3d20 2d30 2e35 2020 2020        = -0.5    
+00001d30: 2020 2020 2020 2320 7265 6769 6f6e 2077        # region w
+00001d40: 6974 6820 6c69 7069 6420 2d20 6c6f 7765  ith lipid - lowe
+00001d50: 7220 7765 6967 6874 2068 6572 650d 0a20  r weight here.. 
+00001d60: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
+00001d70: 6d69 7a65 5f77 6569 6768 7473 5f6c 6970  mize_weights_lip
+00001d80: 6964 5f65 6e64 2020 2020 2020 2020 203d  id_end         =
+00001d90: 2031 2e31 2020 2020 2020 2020 2020 2023   1.1           #
+00001da0: 2020 7374 6172 742f 656e 6420 696e 2070    start/end in p
+00001db0: 706d 0d0a 2020 2020 2020 2020 7365 6c66  pm..        self
+00001dc0: 2e6f 7074 696d 697a 655f 7765 6967 6874  .optimize_weight
+00001dd0: 735f 736d 616c 6c5f 7065 616b 5f66 6163  s_small_peak_fac
+00001de0: 746f 7220 3d20 312e 3020 2020 2020 2020  tor = 1.0       
+00001df0: 2020 2020 2320 7363 616c 6520 6d75 6c74      # scale mult
+00001e00: 6970 6c65 2066 6f72 2073 6d61 6c6c 2070  iple for small p
+00001e10: 6561 6b20 7265 6769 6f6e 730d 0a0d 0a20  eak regions.... 
+00001e20: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
+00001e30: 6d69 7a65 5f62 6f75 6e64 735f 6172 6561  mize_bounds_area
+00001e40: 5f6d 6178 2020 2020 2020 2020 2020 203d  _max           =
+00001e50: 2031 3530 2e30 2020 2020 2020 2020 2020   150.0          
+00001e60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00001e70: 2073 656c 662e 6f70 7469 6d69 7a65 5f62   self.optimize_b
+00001e80: 6f75 6e64 735f 6172 6561 5f6d 696e 2020  ounds_area_min  
+00001e90: 2020 2020 2020 2020 203d 2035 302e 3020           = 50.0 
+00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001eb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
+00001ec0: 7074 696d 697a 655f 626f 756e 6473 5f61  ptimize_bounds_a
+00001ed0: 7265 615f 6d61 785f 736d 616c 6c20 2020  rea_max_small   
+00001ee0: 2020 3d20 3135 302e 3020 2020 2020 2020    = 150.0       
+00001ef0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00001f00: 2020 2020 7365 6c66 2e6f 7074 696d 697a      self.optimiz
+00001f10: 655f 626f 756e 6473 5f61 7265 615f 6d69  e_bounds_area_mi
+00001f20: 6e5f 736d 616c 6c20 2020 2020 3d20 3530  n_small     = 50
+00001f30: 2e30 2020 2020 2020 2020 2020 2020 2020  .0              
+00001f40: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
+00001f50: 662e 6f70 7469 6d69 7a65 5f65 6e61 626c  f.optimize_enabl
+00001f60: 655f 626f 756e 6473 5f61 7265 615f 736d  e_bounds_area_sm
+00001f70: 616c 6c20 203d 2046 616c 7365 2020 2020  all  = False    
+00001f80: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+00001f90: 656c 662e 6f70 7469 6d69 7a65 5f62 6f75  elf.optimize_bou
+00001fa0: 6e64 735f 7261 6e67 655f 7070 6d20 2020  nds_range_ppm   
+00001fb0: 2020 2020 2020 203d 2038 2e30 2020 2020         = 8.0    
+00001fc0: 2020 2020 2020 2023 2048 7a20 2020 202d         # Hz    -
+00001fd0: 2063 616e 2062 6520 676c 6f62 616c 206f   can be global o
+00001fe0: 7220 6f6e 6c79 2066 6f72 2027 6c61 7267  r only for 'larg
+00001ff0: 6527 2073 696e 676c 6574 2070 6561 6b73  e' singlet peaks
+00002000: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
+00002010: 7074 696d 697a 655f 626f 756e 6473 5f72  ptimize_bounds_r
+00002020: 616e 6765 5f70 706d 5f73 6d61 6c6c 2020  ange_ppm_small  
+00002030: 2020 3d20 322e 3020 2020 2020 2020 2020    = 2.0         
+00002040: 2020 2320 487a 2020 2020 2d20 616c 7465    # Hz    - alte
+00002050: 726e 6174 6976 6520 7261 6e67 6520 666f  rnative range fo
+00002060: 7220 2773 6d61 6c6c 2720 7065 616b 730d  r 'small' peaks.
+00002070: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+00002080: 7469 6d69 7a65 5f65 6e61 626c 655f 626f  timize_enable_bo
+00002090: 756e 6473 5f70 706d 5f73 6d61 6c6c 2020  unds_ppm_small  
+000020a0: 203d 2046 616c 7365 2020 2020 2020 2020   = False        
+000020b0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+000020c0: 6f70 7469 6d69 7a65 5f62 6f75 6e64 735f  optimize_bounds_
+000020d0: 7261 6e67 655f 7068 6173 6530 2020 2020  range_phase0    
+000020e0: 2020 203d 2034 352e 3020 2020 2020 2020     = 45.0       
+000020f0: 2020 2023 2064 6567 0d0a 2020 2020 2020     # deg..      
+00002100: 2020 7365 6c66 2e6f 7074 696d 697a 655f    self.optimize_
+00002110: 626f 756e 6473 5f72 616e 6765 5f70 6861  bounds_range_pha
+00002120: 7365 3120 2020 2020 2020 3d20 3230 3030  se1       = 2000
+00002130: 2e30 2020 2020 2020 2020 2320 6465 670d  .0        # deg.
+00002140: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+00002150: 7469 6d69 7a65 5f62 6f75 6e64 735f 6d61  timize_bounds_ma
+00002160: 785f 6c69 6e65 7769 6474 6820 2020 2020  x_linewidth     
+00002170: 203d 2031 2e30 0d0a 2020 2020 2020 2020   = 1.0..        
+00002180: 7365 6c66 2e6f 7074 696d 697a 655f 626f  self.optimize_bo
+00002190: 756e 6473 5f6d 696e 5f6c 696e 6577 6964  unds_min_linewid
+000021a0: 7468 2020 2020 2020 3d20 302e 3034 0d0a  th      = 0.04..
+000021b0: 2020 2020 2020 2020 7365 6c66 2e6f 7074          self.opt
+000021c0: 696d 697a 655f 626f 756e 6473 5f6d 6d6f  imize_bounds_mmo
+000021d0: 6c5f 7261 6e67 655f 6172 6561 2020 2020  l_range_area    
+000021e0: 3d20 3530 2e30 2020 2020 2020 2020 2020  = 50.0          
+000021f0: 2320 2520 6672 6f6d 2073 7461 7274 2076  # % from start v
+00002200: 616c 7565 730d 0a20 2020 2020 2020 2073  alues..        s
+00002210: 656c 662e 6f70 7469 6d69 7a65 5f62 6f75  elf.optimize_bou
+00002220: 6e64 735f 6d6d 6f6c 5f72 616e 6765 5f70  nds_mmol_range_p
+00002230: 706d 2020 2020 203d 2038 2e30 2020 2020  pm     = 8.0    
+00002240: 2020 2020 2020 2023 2048 7a0d 0a20 2020         # Hz..   
+00002250: 2020 2020 2073 656c 662e 6f70 7469 6d69       self.optimi
+00002260: 7a65 5f63 6f6e 7374 7261 696e 5f70 706d  ze_constrain_ppm
+00002270: 5f6e 6161 5f6e 6161 6720 2020 203d 2046  _naa_naag    = F
+00002280: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
+00002290: 6c66 2e6f 7074 696d 697a 655f 636f 6e73  lf.optimize_cons
+000022a0: 7472 6169 6e5f 7070 6d5f 6372 5f70 6372  train_ppm_cr_pcr
+000022b0: 2020 2020 2020 3d20 4661 6c73 650d 0a20        = False.. 
+000022c0: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
+000022d0: 6d69 7a65 5f63 6f6e 7374 7261 696e 5f70  mize_constrain_p
+000022e0: 706d 5f67 7063 5f70 6368 6f20 2020 203d  pm_gpc_pcho    =
+000022f0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00002300: 7365 6c66 2e6f 7074 696d 697a 655f 636f  self.optimize_co
+00002310: 6e73 7472 6169 6e5f 7070 6d5f 6372 325f  nstrain_ppm_cr2_
+00002320: 7063 7232 2020 2020 3d20 4661 6c73 650d  pcr2    = False.
+00002330: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+00002340: 7469 6d69 7a65 5f63 6f6e 7374 7261 696e  timize_constrain
+00002350: 5f70 706d 5f67 6c75 5f67 6c6e 2020 2020  _ppm_glu_gln    
+00002360: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00002370: 2020 7365 6c66 2e6f 7074 696d 697a 655f    self.optimize_
+00002380: 636f 6e73 7472 6169 6e5f 7070 6d5f 7461  constrain_ppm_ta
+00002390: 755f 676c 6320 2020 2020 3d20 4661 6c73  u_glc     = Fals
+000023a0: 650d 0a20 2020 2020 2020 200d 0a20 2020  e..        ..   
+000023b0: 2020 2020 2073 656c 662e 6f70 7469 6d69       self.optimi
+000023c0: 7a65 5f6c 696d 6974 735f 7261 6e67 655f  ze_limits_range_
+000023d0: 6172 6561 2020 2020 2020 2020 203d 2035  area         = 5
+000023e0: 302e 3020 2020 2020 2020 2020 2023 2025  0.0          # %
+000023f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
+00002400: 7074 696d 697a 655f 6c69 6d69 7473 5f72  ptimize_limits_r
+00002410: 616e 6765 5f70 706d 2020 2020 2020 2020  ange_ppm        
+00002420: 2020 3d20 382e 3020 2020 2020 2020 2020    = 8.0         
+00002430: 2020 2320 487a 0d0a 2020 2020 2020 2020    # Hz..        
+00002440: 7365 6c66 2e6f 7074 696d 697a 655f 6c69  self.optimize_li
+00002450: 6d69 7473 5f72 616e 6765 5f70 6861 7365  mits_range_phase
+00002460: 3020 2020 2020 2020 3d20 3435 2e30 2020  0       = 45.0  
+00002470: 2020 2020 2020 2020 2320 6465 670d 0a20          # deg.. 
+00002480: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
+00002490: 6d69 7a65 5f6c 696d 6974 735f 7261 6e67  mize_limits_rang
+000024a0: 655f 7068 6173 6531 2020 2020 2020 203d  e_phase1       =
+000024b0: 2032 3030 302e 3020 2020 2020 2020 2023   2000.0        #
+000024c0: 2064 6567 0d0a 2020 2020 2020 2020 7365   deg..        se
+000024d0: 6c66 2e6f 7074 696d 697a 655f 6c69 6d69  lf.optimize_limi
+000024e0: 7473 5f6d 6178 5f6c 696e 6577 6964 7468  ts_max_linewidth
+000024f0: 2020 2020 2020 3d20 312e 300d 0a20 2020        = 1.0..   
+00002500: 2020 2020 2073 656c 662e 6f70 7469 6d69       self.optimi
+00002510: 7a65 5f6c 696d 6974 735f 6d69 6e5f 6c69  ze_limits_min_li
+00002520: 6e65 7769 6474 6820 2020 2020 203d 2030  newidth      = 0
+00002530: 2e30 340d 0a0d 0a20 2020 2020 2020 2073  .04....        s
+00002540: 656c 662e 636f 6e66 6964 656e 6365 5f69  elf.confidence_i
+00002550: 6e74 6572 7661 6c73 5f66 6c61 6720 2020  ntervals_flag   
+00002560: 2020 2020 2020 203d 2046 616c 7365 0d0a         = False..
+00002570: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00002580: 6669 6465 6e63 655f 616c 7068 6120 2020  fidence_alpha   
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 3d20 302e 3835 0d0a 2020 2020 2020 2020  = 0.85..        
+000025b0: 7365 6c66 2e63 6f6e 6669 6465 6e63 655f  self.confidence_
+000025c0: 6172 6561 5f66 6c61 6720 2020 2020 2020  area_flag       
+000025d0: 2020 2020 2020 2020 3d20 4661 6c73 650d          = False.
+000025e0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+000025f0: 6e66 6964 656e 6365 5f70 706d 5f66 6c61  nfidence_ppm_fla
+00002600: 6720 2020 2020 2020 2020 2020 2020 2020  g               
+00002610: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00002620: 2020 7365 6c66 2e63 6f6e 6669 6465 6e63    self.confidenc
+00002630: 655f 6c69 6e65 7769 6474 685f 666c 6167  e_linewidth_flag
+00002640: 2020 2020 2020 2020 2020 3d20 4661 6c73            = Fals
+00002650: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00002660: 636f 6e66 6964 656e 6365 5f70 6861 7365  confidence_phase
+00002670: 5f66 6c61 6720 2020 2020 2020 2020 2020  _flag           
+00002680: 2020 203d 2046 616c 7365 0d0a 0d0a 2020     = False....  
+00002690: 2020 2020 2020 7365 6c66 2e63 7261 6d65        self.crame
+000026a0: 725f 7261 6f5f 666c 6167 2020 2020 2020  r_rao_flag      
+000026b0: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+000026c0: 5472 7565 2020 2020 2020 2320 666c 6167  True      # flag
+000026d0: 2074 6f20 646f 2063 7261 6d65 722d 7261   to do cramer-ra
+000026e0: 6f20 626f 756e 6420 6361 6c63 756c 6174  o bound calculat
+000026f0: 696f 6e73 0d0a 2020 2020 2020 2020 7365  ions..        se
+00002700: 6c66 2e63 7261 6d65 725f 7261 6f5f 7070  lf.cramer_rao_pp
+00002710: 6d5f 7374 6172 7420 2020 2020 2020 2020  m_start         
+00002720: 2020 2020 2020 3d20 2d38 2e30 2020 2020        = -8.0    
+00002730: 2020 2320 7070 6d20 7261 6e67 6520 666f    # ppm range fo
+00002740: 7220 6e6f 6973 6520 6d65 6173 7572 656d  r noise measurem
+00002750: 656e 7420 746f 2063 616c 630d 0a20 2020  ent to calc..   
+00002760: 2020 2020 2073 656c 662e 6372 616d 6572       self.cramer
+00002770: 5f72 616f 5f70 706d 5f65 6e64 2020 2020  _rao_ppm_end    
+00002780: 2020 2020 2020 2020 2020 2020 203d 202d               = -
+00002790: 362e 3020 2020 2020 2023 2020 7468 6520  6.0      #  the 
+000027a0: 7369 676d 6120 7371 7561 7265 6420 7661  sigma squared va
+000027b0: 7269 616e 6365 2e0d 0a0d 0a20 2020 2020  riance.....     
+000027c0: 2020 2023 2047 4953 4f20 616c 676f 7269     # GISO algori
+000027d0: 7468 6d20 696e 7075 7420 6f62 6a65 6374  thm input object
+000027e0: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+000027f0: 7072 696f 7220 2020 2020 2020 2020 2020  prior           
+00002800: 2020 203d 206d 7273 5f70 7269 6f72 2e50     = mrs_prior.P
+00002810: 7269 6f72 2829 0d0a 0d0a 2020 2020 2020  rior()....      
+00002820: 2020 6966 2061 7474 7269 6275 7465 7320    if attributes 
+00002830: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00002840: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+00002850: 6e66 6c61 7465 2861 7474 7269 6275 7465  nflate(attribute
+00002860: 7329 0d0a 0d0a 2020 2020 2323 2323 2320  s)....    ##### 
+00002870: 5374 616e 6461 7264 204d 6574 686f 6473  Standard Methods
+00002880: 2061 6e64 2050 726f 7065 7274 6965 7320   and Properties 
+00002890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000028a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000028b0: 2323 2323 230d 0a0d 0a20 2020 2064 6566  #####....    def
+000028c0: 205f 5f73 7472 5f5f 2873 656c 6629 3a0d   __str__(self):.
+000028d0: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
+000028e0: 205b 5d0d 0a20 2020 2020 2020 206c 696e   []..        lin
+000028f0: 6573 2e61 7070 656e 6428 222d 2d2d 2d2d  es.append("-----
+00002900: 2d2d 207b 307d 204f 626a 6563 7420 2d2d  -- {0} Object --
+00002910: 2d2d 2d2d 2d22 2e66 6f72 6d61 7428 7365  -----".format(se
+00002920: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
+00002930: 616d 655f 5f29 290d 0a20 2020 2020 2020  ame__))..       
+00002940: 206c 696e 6573 2e61 7070 656e 6428 224e   lines.append("N
+00002950: 6f74 2063 7572 7265 6e74 6c79 2077 7269  ot currently wri
+00002960: 7474 656e 2229 0d0a 2020 2020 2020 2020  tten")..        
+00002970: 7265 7475 726e 2027 5c6e 272e 6a6f 696e  return '\n'.join
+00002980: 286c 696e 6573 290d 0a0d 0a0d 0a20 2020  (lines)......   
+00002990: 2064 6566 2064 6566 6c61 7465 2873 656c   def deflate(sel
+000029a0: 662c 2066 6c61 766f 723d 4465 666c 6174  f, flavor=Deflat
+000029b0: 652e 4554 5245 4529 3a0d 0a20 2020 2020  e.ETREE):..     
+000029c0: 2020 2069 6620 666c 6176 6f72 203d 3d20     if flavor == 
+000029d0: 4465 666c 6174 652e 4554 5245 453a 0d0a  Deflate.ETREE:..
+000029e0: 2020 2020 2020 2020 2020 2020 6520 3d20              e = 
+000029f0: 456c 656d 656e 7428 2273 6574 7469 6e67  Element("setting
+00002a00: 7322 2c20 7b22 7665 7273 696f 6e22 203a  s", {"version" :
+00002a10: 2073 656c 662e 584d 4c5f 5645 5253 494f   self.XML_VERSIO
+00002a20: 4e7d 290d 0a20 2020 2020 2020 2020 2020  N})..           
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 200d 0a20 2020 2020 2020 2020 2020 2023   ..            #
+00002a60: 2054 6865 7365 2061 7474 7269 6275 7465   These attribute
+00002a70: 7320 6172 6520 616c 6c20 6c69 7374 732e  s are all lists.
+00002a80: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00002a90: 7220 6174 7472 6962 7574 6520 696e 2028  r attribute in (
+00002aa0: 2270 7269 6f72 5f6c 6973 7422 2c20 2270  "prior_list", "p
+00002ab0: 7269 6f72 5f61 7265 615f 7363 616c 6522  rior_area_scale"
+00002ac0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ae0: 2020 2270 7269 6f72 5f70 6561 6b5f 7070    "prior_peak_pp
+00002af0: 6d22 2c20 2270 7269 6f72 5f73 6561 7263  m", "prior_searc
+00002b00: 685f 7070 6d22 2c0d 0a20 2020 2020 2020  h_ppm",..       
+00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b20: 2020 2020 2020 2022 7072 696f 725f 6462         "prior_db
+00002b30: 5f70 706d 222c 2022 7072 696f 725f 6669  _ppm", "prior_fi
+00002b40: 785f 7432 222c 0d0a 2020 2020 2020 2020  x_t2",..        
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2020 2020 2270 7269 6f72 5f73 6561        "prior_sea
+00002b70: 7263 685f 7068 3022 2c0d 0a20 2020 2020  rch_ph0",..     
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 2020 2022 7072 696f 725f           "prior_
+00002ba0: 7872 616e 6765 222c 2022 7072 696f 725f  xrange", "prior_
+00002bb0: 7972 616e 6765 222c 0d0a 2020 2020 2020  yrange",..      
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 2020 2020 2020 2020 2270 7269 6f72 5f7a          "prior_z
+00002be0: 7261 6e67 6522 2c20 293a 0d0a 2020 2020  range", ):..    
+00002bf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002c00: 7661 6c75 6520 696e 2067 6574 6174 7472  value in getattr
+00002c10: 2873 656c 662c 2061 7474 7269 6275 7465  (self, attribute
+00002c20: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00002c30: 2020 2020 2020 2020 7574 696c 5f78 6d6c          util_xml
+00002c40: 2e54 6578 7453 7562 456c 656d 656e 7428  .TextSubElement(
+00002c50: 652c 2061 7474 7269 6275 7465 2c20 7661  e, attribute, va
+00002c60: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
+00002c70: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00002c80: 2020 2020 2020 2020 2320 5468 6573 6520          # These 
+00002c90: 6174 7474 7269 6275 7465 7320 6172 6520  atttributes are 
+00002ca0: 616c 6c20 7363 616c 6172 7320 616e 6420  all scalars and 
+00002cb0: 6d61 7020 6469 7265 6374 6c79 2074 6f20  map directly to 
+00002cc0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00002cd0: 584d 4c20 656c 656d 656e 7473 206f 6620  XML elements of 
+00002ce0: 7468 6520 7361 6d65 206e 616d 652e 0d0a  the same name...
+00002cf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002d00: 6174 7472 6962 7574 6520 696e 2028 2270  attribute in ("p
+00002d10: 7269 6f72 5f70 706d 5f73 7461 7274 222c  rior_ppm_start",
+00002d20: 2022 7072 696f 725f 7070 6d5f 656e 6422   "prior_ppm_end"
+00002d30: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00002d40: 2020 2020 2020 2020 2270 7269 6f72 5f6d          "prior_m
+00002d50: 6173 6b5f 736f 7572 6365 222c 2022 7072  ask_source", "pr
+00002d60: 696f 725f 6967 6e6f 7265 5f6d 6173 6b22  ior_ignore_mask"
+00002d70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002d80: 2020 2020 2020 2022 6c69 6e65 7368 6170         "lineshap
+00002d90: 655f 6d6f 6465 6c22 2c20 2269 6e69 7469  e_model", "initi
+00002da0: 616c 5f62 305f 7368 6966 745f 6d65 7468  al_b0_shift_meth
+00002db0: 6f64 222c 0d0a 2020 2020 2020 2020 2020  od",..          
+00002dc0: 2020 2020 2020 2020 2020 2269 6e69 7469            "initi
+00002dd0: 616c 5f62 305f 7661 6c75 6522 2c20 2269  al_b0_value", "i
+00002de0: 6e69 7469 616c 5f62 6173 656c 696e 655f  nitial_baseline_
+00002df0: 6d65 7468 6f64 222c 0d0a 2020 2020 2020  method",..      
+00002e00: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00002e10: 6e69 7469 616c 5f62 6173 656c 696e 655f  nitial_baseline_
+00002e20: 6c6f 7765 7373 5f77 6964 7468 222c 0d0a  lowess_width",..
+00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e40: 2020 2020 2269 6e69 7469 616c 5f62 6173      "initial_bas
+00002e50: 656c 696e 655f 6c6f 7765 7373 5f64 656c  eline_lowess_del
+00002e60: 7461 222c 0d0a 2020 2020 2020 2020 2020  ta",..          
+00002e70: 2020 2020 2020 2020 2020 2269 6e69 7469            "initi
+00002e80: 616c 5f62 6173 656c 696e 655f 6c6f 7765  al_baseline_lowe
+00002e90: 7373 5f69 676e 6f72 655f 7769 6474 6822  ss_ignore_width"
+00002ea0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002eb0: 2020 2020 2020 2022 696e 6974 6961 6c5f         "initial_
+00002ec0: 6372 5f63 686f 5f73 6570 6172 6174 696f  cr_cho_separatio
+00002ed0: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
+00002ee0: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
+00002ef0: 6c5f 7065 616b 5f73 6561 7263 685f 6162  l_peak_search_ab
+00002f00: 7322 2c20 2269 6e69 7469 616c 5f73 6d61  s", "initial_sma
+00002f10: 6c6c 5f70 6561 6b5f 6172 6561 7322 2c0d  ll_peak_areas",.
+00002f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f30: 2020 2020 2022 696e 6974 6961 6c5f 736d       "initial_sm
+00002f40: 616c 6c5f 7065 616b 5f66 7265 7173 222c  all_peak_freqs",
+00002f50: 2022 696e 6974 6961 6c5f 6c69 6e65 7769   "initial_linewi
+00002f60: 6474 685f 6d65 7468 6f64 222c 0d0a 2020  dth_method",..  
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f80: 2020 2269 6e69 7469 616c 5f6c 696e 6577    "initial_linew
+00002f90: 6964 7468 5f76 616c 7565 222c 0d0a 2020  idth_value",..  
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fb0: 2020 2269 6e69 7469 616c 5f6c 696e 6577    "initial_linew
+00002fc0: 6964 7468 5f72 616e 6765 5f73 7461 7274  idth_range_start
+00002fd0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00002fe0: 2020 2020 2020 2020 2269 6e69 7469 616c          "initial
+00002ff0: 5f6c 696e 6577 6964 7468 5f72 616e 6765  _linewidth_range
+00003000: 5f65 6e64 222c 2022 696e 6974 6961 6c5f  _end", "initial_
+00003010: 6c69 6e65 7769 6474 685f 6675 6467 6522  linewidth_fudge"
+00003020: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003030: 2020 2020 2020 2022 696e 6974 6961 6c5f         "initial_
+00003040: 7068 6173 655f 6d65 7468 6f64 222c 0d0a  phase_method",..
+00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003060: 2020 2020 2269 6e69 7469 616c 5f70 6861      "initial_pha
+00003070: 7365 305f 7661 6c75 6522 2c20 2269 6e69  se0_value", "ini
+00003080: 7469 616c 5f70 6861 7365 315f 7661 6c75  tial_phase1_valu
+00003090: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+000030a0: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
+000030b0: 6c5f 6170 706c 795f 6b6f 5f66 696c 7465  l_apply_ko_filte
+000030c0: 7222 2c0d 0a20 2020 2020 2020 2020 2020  r",..           
+000030d0: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
+000030e0: 6c5f 6b6f 5f6c 696e 6577 6964 7468 5f6d  l_ko_linewidth_m
+000030f0: 696e 696d 756d 222c 2022 696e 6974 6961  inimum", "initia
+00003100: 6c5f 6b6f 5f70 6f69 6e74 7322 2c0d 0a20  l_ko_points",.. 
 00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 2020 2270 7269 6f72 5f7a 7261 6e67      "prior_zrang
-00003130: 6522 2c20 293a 0d0a 2020 2020 2020 2020  e", ):..        
-00003140: 2020 2020 2020 2020 666f 7220 7661 6c75          for valu
-00003150: 6520 696e 2067 6574 6174 7472 2873 656c  e in getattr(sel
-00003160: 662c 2061 7474 7269 6275 7465 293a 0d0a  f, attribute):..
+00003120: 2020 2022 696e 6974 6961 6c5f 7068 6173     "initial_phas
+00003130: 6531 5f66 6964 5f63 6f6e 7374 616e 7422  e1_fid_constant"
+00003140: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003150: 2020 2020 2020 2022 696e 6974 6961 6c5f         "initial_
+00003160: 6c61 635f 6d65 7468 6f64 222c 0d0a 2020  lac_method",..  
 00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 7574 696c 5f78 6d6c 2e54 6578      util_xml.Tex
-00003190: 7453 7562 456c 656d 656e 7428 652c 2061  tSubElement(e, a
-000031a0: 7474 7269 6275 7465 2c20 7661 6c75 6529  ttribute, value)
-000031b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000031c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000031d0: 2020 2020 2320 5468 6573 6520 6174 7474      # These attt
-000031e0: 7269 6275 7465 7320 6172 6520 616c 6c20  ributes are all 
-000031f0: 7363 616c 6172 7320 616e 6420 6d61 7020  scalars and map 
-00003200: 6469 7265 6374 6c79 2074 6f20 0d0a 2020  directly to ..  
-00003210: 2020 2020 2020 2020 2020 2320 584d 4c20            # XML 
-00003220: 656c 656d 656e 7473 206f 6620 7468 6520  elements of the 
-00003230: 7361 6d65 206e 616d 652e 0d0a 2020 2020  same name...    
-00003240: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-00003250: 6962 7574 6520 696e 2028 2270 7269 6f72  ibute in ("prior
-00003260: 5f70 706d 5f73 7461 7274 222c 2022 7072  _ppm_start", "pr
-00003270: 696f 725f 7070 6d5f 656e 6422 2c20 0d0a  ior_ppm_end", ..
-00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003290: 2020 2020 2270 7269 6f72 5f6d 6173 6b5f      "prior_mask_
-000032a0: 736f 7572 6365 222c 2022 7072 696f 725f  source", "prior_
-000032b0: 6967 6e6f 7265 5f6d 6173 6b22 2c0d 0a20  ignore_mask",.. 
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 2022 6c69 6e65 7368 6170 655f 6d6f     "lineshape_mo
-000032e0: 6465 6c22 2c20 2269 6e69 7469 616c 5f62  del", "initial_b
-000032f0: 305f 7368 6966 745f 6d65 7468 6f64 222c  0_shift_method",
-00003300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003310: 2020 2020 2020 2269 6e69 7469 616c 5f62        "initial_b
-00003320: 305f 7661 6c75 6522 2c20 2269 6e69 7469  0_value", "initi
-00003330: 616c 5f62 6173 656c 696e 655f 6d65 7468  al_baseline_meth
-00003340: 6f64 222c 0d0a 2020 2020 2020 2020 2020  od",..          
-00003350: 2020 2020 2020 2020 2020 2269 6e69 7469            "initi
-00003360: 616c 5f62 6173 656c 696e 655f 6c6f 7765  al_baseline_lowe
-00003370: 7373 5f77 6964 7468 222c 0d0a 2020 2020  ss_width",..    
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2269 6e69 7469 616c 5f62 6173 656c 696e  "initial_baselin
-000033a0: 655f 6c6f 7765 7373 5f64 656c 7461 222c  e_lowess_delta",
-000033b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000033c0: 2020 2020 2020 2269 6e69 7469 616c 5f62        "initial_b
-000033d0: 6173 656c 696e 655f 6c6f 7765 7373 5f69  aseline_lowess_i
-000033e0: 676e 6f72 655f 7769 6474 6822 2c0d 0a20  gnore_width",.. 
+00003180: 2020 2269 6e69 7469 616c 5f70 6561 6b5f    "initial_peak_
+00003190: 6e65 6761 7469 7665 5f66 6c61 6722 2c0d  negative_flag",.
+000031a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000031b0: 2020 2020 2022 6261 7365 6c69 6e65 5f6d       "baseline_m
+000031c0: 6574 686f 6422 2c0d 0a20 2020 2020 2020  ethod",..       
+000031d0: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+000031e0: 7365 6c69 6e65 5f73 6d6f 6f74 6869 6e67  seline_smoothing
+000031f0: 5f66 6c61 6722 2c20 2262 6173 656c 696e  _flag", "baselin
+00003200: 655f 736b 6970 5f6c 6173 745f 736d 6f6f  e_skip_last_smoo
+00003210: 7468 222c 0d0a 2020 2020 2020 2020 2020  th",..          
+00003220: 2020 2020 2020 2020 2020 2262 6173 656c            "basel
+00003230: 696e 655f 736d 6f6f 7468 696e 675f 7769  ine_smoothing_wi
+00003240: 6474 6822 2c20 2262 6173 656c 696e 655f  dth", "baseline_
+00003250: 736d 6f6f 7468 696e 675f 6465 6c74 6122  smoothing_delta"
+00003260: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003270: 2020 2020 2020 2022 6261 7365 6c69 6e65         "baseline
+00003280: 5f75 6e64 6572 6573 7469 6d61 7465 222c  _underestimate",
+00003290: 2022 6261 7365 6c69 6e65 5f73 706c 696e   "baseline_splin
+000032a0: 655f 6e6b 6e6f 7473 222c 0d0a 2020 2020  e_nknots",..    
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032c0: 2262 6173 656c 696e 655f 7370 6c69 6e65  "baseline_spline
+000032d0: 5f73 7061 6369 6e67 222c 2022 6261 7365  _spacing", "base
+000032e0: 6c69 6e65 5f73 706c 696e 655f 6f72 6465  line_spline_orde
+000032f0: 7222 2c0d 0a20 2020 2020 2020 2020 2020  r",..           
+00003300: 2020 2020 2020 2020 2022 6261 7365 6c69           "baseli
+00003310: 6e65 5f77 6176 656c 6574 5f73 6361 6c65  ne_wavelet_scale
+00003320: 222c 2022 6261 7365 6c69 6e65 5f77 6176  ", "baseline_wav
+00003330: 656c 6574 5f6d 696e 5f64 7961 6422 2c0d  elet_min_dyad",.
+00003340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003350: 2020 2020 2022 6261 7365 6c69 6e65 5f77       "baseline_w
+00003360: 6176 656c 6574 5f73 6872 696e 6b61 6765  avelet_shrinkage
+00003370: 5f66 6c61 6722 2c0d 0a20 2020 2020 2020  _flag",..       
+00003380: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+00003390: 7365 6c69 6e65 5f77 6176 656c 6574 5f69  seline_wavelet_i
+000033a0: 6e76 6172 6961 6e63 655f 6c61 6722 2c0d  nvariance_lag",.
+000033b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000033c0: 2020 2020 2022 6261 7365 6c69 6e65 5f77       "baseline_w
+000033d0: 6176 656c 6574 5f69 6e76 6172 6961 6e63  avelet_invarianc
+000033e0: 655f 7265 636f 6d62 696e 6522 2c0d 0a20  e_recombine",.. 
 000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2022 696e 6974 6961 6c5f 6372 5f63     "initial_cr_c
-00003410: 686f 5f73 6570 6172 6174 696f 6e22 2c0d  ho_separation",.
-00003420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003430: 2020 2020 2022 696e 6974 6961 6c5f 7065       "initial_pe
-00003440: 616b 5f73 6561 7263 685f 6162 7322 2c20  ak_search_abs", 
-00003450: 2269 6e69 7469 616c 5f73 6d61 6c6c 5f70  "initial_small_p
-00003460: 6561 6b5f 6172 6561 7322 2c0d 0a20 2020  eak_areas",..   
-00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003480: 2022 696e 6974 6961 6c5f 736d 616c 6c5f   "initial_small_
-00003490: 7065 616b 5f66 7265 7173 222c 2022 696e  peak_freqs", "in
-000034a0: 6974 6961 6c5f 6c69 6e65 7769 6474 685f  itial_linewidth_
-000034b0: 6d65 7468 6f64 222c 0d0a 2020 2020 2020  method",..      
-000034c0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-000034d0: 6e69 7469 616c 5f6c 696e 6577 6964 7468  nitial_linewidth
-000034e0: 5f76 616c 7565 222c 0d0a 2020 2020 2020  _value",..      
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00003500: 6e69 7469 616c 5f6c 696e 6577 6964 7468  nitial_linewidth
-00003510: 5f72 616e 6765 5f73 7461 7274 222c 0d0a  _range_start",..
-00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003530: 2020 2020 2269 6e69 7469 616c 5f6c 696e      "initial_lin
-00003540: 6577 6964 7468 5f72 616e 6765 5f65 6e64  ewidth_range_end
-00003550: 222c 2022 696e 6974 6961 6c5f 6c69 6e65  ", "initial_line
-00003560: 7769 6474 685f 6675 6467 6522 2c0d 0a20  width_fudge",.. 
-00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 2020 2022 696e 6974 6961 6c5f 7068 6173     "initial_phas
-00003590: 655f 6d65 7468 6f64 222c 0d0a 2020 2020  e_method",..    
+00003400: 2020 2022 6d61 6372 6f6d 6f6c 5f6d 6f64     "macromol_mod
+00003410: 656c 222c 0d0a 2020 2020 2020 2020 2020  el",..          
+00003420: 2020 2020 2020 2020 2020 226d 6163 726f            "macro
+00003430: 6d6f 6c5f 7369 6e67 6c65 5f62 6173 6973  mol_single_basis
+00003440: 5f64 6174 6173 6574 5f73 7461 7274 5f61  _dataset_start_a
+00003450: 7265 6122 2c0d 0a20 2020 2020 2020 2020  rea",..         
+00003460: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
+00003470: 6d69 7a65 5f6d 6574 686f 6422 2c20 226f  mize_method", "o
+00003480: 7074 696d 697a 655f 7363 616c 696e 675f  ptimize_scaling_
+00003490: 666c 6167 222c 0d0a 2020 2020 2020 2020  flag",..        
+000034a0: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
+000034b0: 696d 697a 655f 7374 6f70 5f74 6f6c 6572  imize_stop_toler
+000034c0: 616e 6365 222c 2022 6f70 7469 6d69 7a65  ance", "optimize
+000034d0: 5f6d 6178 5f69 7465 7261 7469 6f6e 7322  _max_iterations"
+000034e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000034f0: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
+00003500: 5f6c 696d 6974 735f 7261 6e67 655f 6172  _limits_range_ar
+00003510: 6561 222c 2022 6f70 7469 6d69 7a65 5f6c  ea", "optimize_l
+00003520: 696d 6974 735f 7261 6e67 655f 7070 6d22  imits_range_ppm"
+00003530: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003540: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
+00003550: 5f6c 696d 6974 735f 7261 6e67 655f 7068  _limits_range_ph
+00003560: 6173 6530 222c 0d0a 2020 2020 2020 2020  ase0",..        
+00003570: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
+00003580: 696d 697a 655f 6c69 6d69 7473 5f72 616e  imize_limits_ran
+00003590: 6765 5f70 6861 7365 3122 2c0d 0a20 2020  ge_phase1",..   
 000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2269 6e69 7469 616c 5f70 6861 7365 305f  "initial_phase0_
-000035c0: 7661 6c75 6522 2c20 2269 6e69 7469 616c  value", "initial
-000035d0: 5f70 6861 7365 315f 7661 6c75 6522 2c0d  _phase1_value",.
-000035e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000035f0: 2020 2020 2022 696e 6974 6961 6c5f 6170       "initial_ap
-00003600: 706c 795f 6b6f 5f66 696c 7465 7222 2c0d  ply_ko_filter",.
-00003610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003620: 2020 2020 2022 696e 6974 6961 6c5f 6b6f       "initial_ko
-00003630: 5f6c 696e 6577 6964 7468 5f6d 696e 696d  _linewidth_minim
-00003640: 756d 222c 2022 696e 6974 6961 6c5f 6b6f  um", "initial_ko
-00003650: 5f70 6f69 6e74 7322 2c0d 0a20 2020 2020  _points",..     
-00003660: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003670: 696e 6974 6961 6c5f 7068 6173 6531 5f66  initial_phase1_f
-00003680: 6964 5f63 6f6e 7374 616e 7422 2c0d 0a20  id_constant",.. 
+000035b0: 2022 6f70 7469 6d69 7a65 5f6c 696d 6974   "optimize_limit
+000035c0: 735f 6d61 785f 6c69 6e65 7769 6474 6822  s_max_linewidth"
+000035d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000035e0: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
+000035f0: 5f6c 696d 6974 735f 6d69 6e5f 6c69 6e65  _limits_min_line
+00003600: 7769 6474 6822 2c0d 0a20 2020 2020 2020  width",..       
+00003610: 2020 2020 2020 2020 2020 2020 2022 6f70               "op
+00003620: 7469 6d69 7a65 5f67 6c6f 6261 6c5f 6974  timize_global_it
+00003630: 6572 6174 696f 6e73 222c 2022 6f70 7469  erations", "opti
+00003640: 6d69 7a65 5f77 6569 6768 7473 5f6d 6574  mize_weights_met
+00003650: 686f 6422 2c0d 0a20 2020 2020 2020 2020  hod",..         
+00003660: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
+00003670: 6d69 7a65 5f77 6569 6768 7473 5f73 6361  mize_weights_sca
+00003680: 6c65 5f66 6163 746f 7222 2c0d 0a20 2020  le_factor",..   
 00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036a0: 2020 2022 696e 6974 6961 6c5f 6c61 635f     "initial_lac_
-000036b0: 6d65 7468 6f64 222c 0d0a 2020 2020 2020  method",..      
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-000036d0: 6e69 7469 616c 5f70 6561 6b5f 6e65 6761  nitial_peak_nega
-000036e0: 7469 7665 5f66 6c61 6722 2c0d 0a20 2020  tive_flag",..   
-000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003700: 2022 6261 7365 6c69 6e65 5f6d 6574 686f   "baseline_metho
-00003710: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-00003720: 2020 2020 2020 2020 2022 6261 7365 6c69           "baseli
-00003730: 6e65 5f73 6d6f 6f74 6869 6e67 5f66 6c61  ne_smoothing_fla
-00003740: 6722 2c20 2262 6173 656c 696e 655f 736b  g", "baseline_sk
-00003750: 6970 5f6c 6173 745f 736d 6f6f 7468 222c  ip_last_smooth",
-00003760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003770: 2020 2020 2020 2262 6173 656c 696e 655f        "baseline_
-00003780: 736d 6f6f 7468 696e 675f 7769 6474 6822  smoothing_width"
-00003790: 2c20 2262 6173 656c 696e 655f 736d 6f6f  , "baseline_smoo
-000037a0: 7468 696e 675f 6465 6c74 6122 2c0d 0a20  thing_delta",.. 
-000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 2020 2022 6261 7365 6c69 6e65 5f75 6e64     "baseline_und
-000037d0: 6572 6573 7469 6d61 7465 222c 2022 6261  erestimate", "ba
-000037e0: 7365 6c69 6e65 5f73 706c 696e 655f 6e6b  seline_spline_nk
-000037f0: 6e6f 7473 222c 0d0a 2020 2020 2020 2020  nots",..        
-00003800: 2020 2020 2020 2020 2020 2020 2262 6173              "bas
-00003810: 656c 696e 655f 7370 6c69 6e65 5f73 7061  eline_spline_spa
-00003820: 6369 6e67 222c 2022 6261 7365 6c69 6e65  cing", "baseline
-00003830: 5f73 706c 696e 655f 6f72 6465 7222 2c0d  _spline_order",.
-00003840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003850: 2020 2020 2022 6261 7365 6c69 6e65 5f77       "baseline_w
-00003860: 6176 656c 6574 5f73 6361 6c65 222c 2022  avelet_scale", "
-00003870: 6261 7365 6c69 6e65 5f77 6176 656c 6574  baseline_wavelet
-00003880: 5f6d 696e 5f64 7961 6422 2c0d 0a20 2020  _min_dyad",..   
-00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038a0: 2022 6261 7365 6c69 6e65 5f77 6176 656c   "baseline_wavel
-000038b0: 6574 5f73 6872 696e 6b61 6765 5f66 6c61  et_shrinkage_fla
-000038c0: 6722 2c0d 0a20 2020 2020 2020 2020 2020  g",..           
-000038d0: 2020 2020 2020 2020 2022 6261 7365 6c69           "baseli
-000038e0: 6e65 5f77 6176 656c 6574 5f69 6e76 6172  ne_wavelet_invar
-000038f0: 6961 6e63 655f 6c61 6722 2c0d 0a20 2020  iance_lag",..   
-00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2022 6261 7365 6c69 6e65 5f77 6176 656c   "baseline_wavel
-00003920: 6574 5f69 6e76 6172 6961 6e63 655f 7265  et_invariance_re
-00003930: 636f 6d62 696e 6522 2c0d 0a20 2020 2020  combine",..     
-00003940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003950: 6d61 6372 6f6d 6f6c 5f6d 6f64 656c 222c  macromol_model",
-00003960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003970: 2020 2020 2020 226d 6163 726f 6d6f 6c5f        "macromol_
-00003980: 7369 6e67 6c65 5f62 6173 6973 5f64 6174  single_basis_dat
-00003990: 6173 6574 5f73 7461 7274 5f61 7265 6122  aset_start_area"
-000039a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000039b0: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
-000039c0: 5f6d 6574 686f 6422 2c20 226f 7074 696d  _method", "optim
-000039d0: 697a 655f 7363 616c 696e 675f 666c 6167  ize_scaling_flag
-000039e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000039f0: 2020 2020 2020 2020 226f 7074 696d 697a          "optimiz
-00003a00: 655f 7374 6f70 5f74 6f6c 6572 616e 6365  e_stop_tolerance
-00003a10: 222c 2022 6f70 7469 6d69 7a65 5f6d 6178  ", "optimize_max
-00003a20: 5f69 7465 7261 7469 6f6e 7322 2c0d 0a20  _iterations",.. 
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2022 6f70 7469 6d69 7a65 5f6c 696d     "optimize_lim
-00003a50: 6974 735f 7261 6e67 655f 6172 6561 222c  its_range_area",
-00003a60: 2022 6f70 7469 6d69 7a65 5f6c 696d 6974   "optimize_limit
-00003a70: 735f 7261 6e67 655f 7070 6d22 2c0d 0a20  s_range_ppm",.. 
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a90: 2020 2022 6f70 7469 6d69 7a65 5f6c 696d     "optimize_lim
-00003aa0: 6974 735f 7261 6e67 655f 7068 6173 6530  its_range_phase0
-00003ab0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00003ac0: 2020 2020 2020 2020 226f 7074 696d 697a          "optimiz
-00003ad0: 655f 6c69 6d69 7473 5f72 616e 6765 5f70  e_limits_range_p
-00003ae0: 6861 7365 3122 2c0d 0a20 2020 2020 2020  hase1",..       
-00003af0: 2020 2020 2020 2020 2020 2020 2022 6f70               "op
-00003b00: 7469 6d69 7a65 5f6c 696d 6974 735f 6d61  timize_limits_ma
-00003b10: 785f 6c69 6e65 7769 6474 6822 2c0d 0a20  x_linewidth",.. 
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b30: 2020 2022 6f70 7469 6d69 7a65 5f6c 696d     "optimize_lim
-00003b40: 6974 735f 6d69 6e5f 6c69 6e65 7769 6474  its_min_linewidt
-00003b50: 6822 2c0d 0a20 2020 2020 2020 2020 2020  h",..           
-00003b60: 2020 2020 2020 2020 2022 6f70 7469 6d69           "optimi
-00003b70: 7a65 5f67 6c6f 6261 6c5f 6974 6572 6174  ze_global_iterat
-00003b80: 696f 6e73 222c 2022 6f70 7469 6d69 7a65  ions", "optimize
-00003b90: 5f77 6569 6768 7473 5f6d 6574 686f 6422  _weights_method"
-00003ba0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003bb0: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
-00003bc0: 5f77 6569 6768 7473 5f73 6361 6c65 5f66  _weights_scale_f
-00003bd0: 6163 746f 7222 2c0d 0a20 2020 2020 2020  actor",..       
-00003be0: 2020 2020 2020 2020 2020 2020 2022 6f70               "op
-00003bf0: 7469 6d69 7a65 5f77 6569 6768 7473 5f77  timize_weights_w
-00003c00: 6964 7468 5f66 6163 746f 7222 2c0d 0a20  idth_factor",.. 
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2020 2022 6f70 7469 6d69 7a65 5f77 6569     "optimize_wei
-00003c30: 6768 7473 5f77 6174 6572 5f66 6c61 6722  ghts_water_flag"
-00003c40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003c50: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
-00003c60: 5f77 6569 6768 7473 5f77 6174 6572 5f73  _weights_water_s
-00003c70: 7461 7274 222c 0d0a 2020 2020 2020 2020  tart",..        
-00003c80: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
-00003c90: 696d 697a 655f 7765 6967 6874 735f 7761  imize_weights_wa
-00003ca0: 7465 725f 656e 6422 2c0d 0a20 2020 2020  ter_end",..     
-00003cb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003cc0: 6f70 7469 6d69 7a65 5f77 6569 6768 7473  optimize_weights
-00003cd0: 5f6c 6970 6964 5f66 6c61 6722 2c0d 0a20  _lipid_flag",.. 
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2020 2022 6f70 7469 6d69 7a65 5f77 6569     "optimize_wei
-00003d00: 6768 7473 5f6c 6970 6964 5f73 7461 7274  ghts_lipid_start
-00003d10: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00003d20: 2020 2020 2020 2020 226f 7074 696d 697a          "optimiz
-00003d30: 655f 7765 6967 6874 735f 6c69 7069 645f  e_weights_lipid_
-00003d40: 656e 6422 2c0d 0a20 2020 2020 2020 2020  end",..         
-00003d50: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
-00003d60: 6d69 7a65 5f77 6569 6768 7473 5f73 6d61  mize_weights_sma
-00003d70: 6c6c 5f70 6561 6b5f 6661 6374 6f72 222c  ll_peak_factor",
-00003d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003d90: 2020 2020 2020 2263 6f6e 6669 6465 6e63        "confidenc
-00003da0: 655f 696e 7465 7276 616c 735f 666c 6167  e_intervals_flag
-00003db0: 222c 2022 636f 6e66 6964 656e 6365 5f61  ", "confidence_a
-00003dc0: 6c70 6861 222c 0d0a 2020 2020 2020 2020  lpha",..        
-00003dd0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00003de0: 6669 6465 6e63 655f 6172 6561 5f66 6c61  fidence_area_fla
-00003df0: 6722 2c20 2263 6f6e 6669 6465 6e63 655f  g", "confidence_
-00003e00: 7070 6d5f 666c 6167 222c 0d0a 2020 2020  ppm_flag",..    
-00003e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e20: 2263 6f6e 6669 6465 6e63 655f 6c69 6e65  "confidence_line
-00003e30: 7769 6474 685f 666c 6167 222c 2022 636f  width_flag", "co
-00003e40: 6e66 6964 656e 6365 5f70 6861 7365 5f66  nfidence_phase_f
-00003e50: 6c61 6722 2c0d 0a20 2020 2020 2020 2020  lag",..         
-00003e60: 2020 2020 2020 2020 2020 2022 6372 616d             "cram
-00003e70: 6572 5f72 616f 5f66 6c61 6722 2c20 2263  er_rao_flag", "c
-00003e80: 7261 6d65 725f 7261 6f5f 7070 6d5f 7374  ramer_rao_ppm_st
-00003e90: 6172 7422 2c0d 0a20 2020 2020 2020 2020  art",..         
-00003ea0: 2020 2020 2020 2020 2020 2022 6372 616d             "cram
-00003eb0: 6572 5f72 616f 5f70 706d 5f65 6e64 222c  er_rao_ppm_end",
-00003ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003ed0: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
-00003ee0: 2020 2020 2020 2020 2020 7574 696c 5f78            util_x
-00003ef0: 6d6c 2e54 6578 7453 7562 456c 656d 656e  ml.TextSubElemen
-00003f00: 7428 652c 2061 7474 7269 6275 7465 2c20  t(e, attribute, 
-00003f10: 6765 7461 7474 7228 7365 6c66 2c20 6174  getattr(self, at
-00003f20: 7472 6962 7574 6529 290d 0a0d 0a20 2020  tribute))....   
-00003f30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00003f40: 2e6d 6163 726f 6d6f 6c5f 7369 6e67 6c65  .macromol_single
-00003f50: 5f62 6173 6973 5f64 6174 6173 6574 3a0d  _basis_dataset:.
-00003f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f70: 2023 2049 6e20 7468 6520 6e65 7874 206c   # In the next l
-00003f80: 696e 652c 2077 6520 2a68 6176 652a 2074  ine, we *have* t
-00003f90: 6f20 7361 7665 2074 6865 2075 7569 6420  o save the uuid 
-00003fa0: 7661 6c75 6573 2066 726f 6d20 7468 6520  values from the 
-00003fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003fc0: 2020 2320 6163 7475 616c 206f 626a 6563    # actual objec
-00003fd0: 7420 7261 7468 6572 2074 6861 6e20 6672  t rather than fr
-00003fe0: 6f6d 2074 6865 2061 7474 7269 6275 7465  om the attribute
-00003ff0: 2061 626f 7665 2c20 696e 2020 0d0a 2020   above, in  ..  
-00004000: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00004010: 6f72 6465 7220 666f 7220 7468 6520 6173  order for the as
-00004020: 736f 6369 6174 6564 2064 6174 6173 6574  sociated dataset
-00004030: 2075 7569 6420 746f 2072 6566 6c65 6374   uuid to reflect
-00004040: 2074 6865 206e 6577 2069 640d 0a20 2020   the new id..   
-00004050: 2020 2020 2020 2020 2020 2020 2023 2074               # t
-00004060: 6861 7420 6973 2067 6976 656e 2069 6e20  hat is given in 
-00004070: 7468 6520 746f 7020 6c65 7665 6c20 6461  the top level da
-00004080: 7461 7365 742e 2041 7373 6f63 6961 7465  taset. Associate
-00004090: 6420 6461 7461 7365 7473 2061 7265 0d0a  d datasets are..
-000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040b0: 2320 6769 7665 6e20 6e65 7720 7465 6d70  # given new temp
-000040c0: 6f72 6172 7920 7575 6964 2076 616c 7565  orary uuid value
-000040d0: 7320 736f 2074 6861 7420 6966 2074 6865  s so that if the
-000040e0: 206d 6169 6e20 6461 7461 7365 7420 6973   main dataset is
-000040f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004100: 2020 2023 2073 6176 6564 2061 6e64 2069     # saved and i
-00004110: 6d6d 6564 6961 7465 6c79 206c 6f61 6465  mmediately loade
-00004120: 6420 6261 636b 2069 6e2c 2077 6520 646f  d back in, we do
-00004130: 206e 6f74 2067 6574 2063 6f6c 6c69 7369   not get collisi
-00004140: 6f6e 730d 0a20 2020 2020 2020 2020 2020  ons..           
-00004150: 2020 2020 2023 2062 6574 7765 656e 2074       # between t
-00004160: 6865 206e 6577 6c79 206f 7065 6e65 6420  he newly opened 
-00004170: 6461 7461 7365 7473 2061 6e64 2061 6c72  datasets and alr
-00004180: 6561 6479 2065 7869 7374 696e 6720 6f6e  eady existing on
-00004190: 6573 2e0d 0a20 2020 2020 2020 2020 2020  es...           
-000041a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000041b0: 2020 2020 2020 2075 7469 6c5f 786d 6c2e         util_xml.
-000041c0: 5465 7874 5375 6245 6c65 6d65 6e74 2865  TextSubElement(e
-000041d0: 2c20 226d 6163 726f 6d6f 6c5f 7369 6e67  , "macromol_sing
-000041e0: 6c65 5f62 6173 6973 5f64 6174 6173 6574  le_basis_dataset
-000041f0: 5f69 6422 2c20 7365 6c66 2e6d 6163 726f  _id", self.macro
-00004200: 6d6f 6c5f 7369 6e67 6c65 5f62 6173 6973  mol_single_basis
-00004210: 5f64 6174 6173 6574 2e69 6429 0d0a 0d0a  _dataset.id)....
-00004220: 0d0a 2020 2020 2020 2020 2020 2020 652e  ..            e.
-00004230: 6170 7065 6e64 2873 656c 662e 7072 696f  append(self.prio
-00004240: 722e 6465 666c 6174 6528 2929 0d0a 2020  r.deflate())..  
-00004250: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00004260: 2020 2020 2020 2020 7265 7475 726e 2065          return e
-00004270: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00004280: 2020 2020 2020 2020 656c 6966 2066 6c61          elif fla
-00004290: 766f 7220 3d3d 2044 6566 6c61 7465 2e44  vor == Deflate.D
-000042a0: 4943 5449 4f4e 4152 593a 0d0a 2020 2020  ICTIONARY:..    
-000042b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000042c0: 656c 662e 5f5f 6469 6374 5f5f 2e63 6f70  elf.__dict__.cop
-000042d0: 7928 290d 0a0d 0a0d 0a20 2020 2064 6566  y()......    def
-000042e0: 2069 6e66 6c61 7465 2873 656c 662c 2073   inflate(self, s
-000042f0: 6f75 7263 6529 3a0d 0a20 2020 2020 2020  ource):..       
-00004300: 2069 6620 6861 7361 7474 7228 736f 7572   if hasattr(sour
-00004310: 6365 2c20 226d 616b 6565 6c65 6d65 6e74  ce, "makeelement
-00004320: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00004330: 2023 2051 7561 636b 7320 6c69 6b65 2061   # Quacks like a
-00004340: 6e20 456c 656d 656e 7454 7265 652e 456c  n ElementTree.El
-00004350: 656d 656e 740d 0a20 2020 2020 2020 2020  ement..         
-00004360: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00004370: 2023 2057 6520 696e 666c 6174 6520 696e   # We inflate in
-00004380: 2061 7474 7269 6275 7465 7320 6772 6f75   attributes grou
-00004390: 7065 6420 6279 2074 7970 6520 7369 6e63  ped by type sinc
-000043a0: 6520 7468 6572 6527 7320 736f 0d0a 2020  e there's so..  
-000043b0: 2020 2020 2020 2020 2020 2320 646f 6767            # dogg
-000043c0: 6f6e 6520 6d61 6e79 2061 7474 7273 206f  one many attrs o
-000043d0: 6e20 7468 6973 2063 6c61 7373 2e0d 0a20  n this class... 
-000043e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000043f0: 2020 2020 2020 2020 2023 2042 6f6f 6c65           # Boole
-00004400: 616e 730d 0a20 2020 2020 2020 2020 2020  ans..           
-00004410: 2066 6f72 2061 7474 7269 6275 7465 2069   for attribute i
-00004420: 6e20 2822 7072 696f 725f 6967 6e6f 7265  n ("prior_ignore
-00004430: 5f6d 6173 6b22 2c20 0d0a 2020 2020 2020  _mask", ..      
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 2020 2020 2020 2020 2269 6e69 7469 616c          "initial
-00004460: 5f63 725f 6368 6f5f 7365 7061 7261 7469  _cr_cho_separati
-00004470: 6f6e 222c 0d0a 2020 2020 2020 2020 2020  on",..          
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 2020 2020 2269 6e69 7469 616c 5f70 6561      "initial_pea
-000044a0: 6b5f 7365 6172 6368 5f61 6273 222c 0d0a  k_search_abs",..
+000036a0: 2022 6f70 7469 6d69 7a65 5f77 6569 6768   "optimize_weigh
+000036b0: 7473 5f77 6964 7468 5f66 6163 746f 7222  ts_width_factor"
+000036c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000036d0: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
+000036e0: 5f77 6569 6768 7473 5f77 6174 6572 5f66  _weights_water_f
+000036f0: 6c61 6722 2c0d 0a20 2020 2020 2020 2020  lag",..         
+00003700: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
+00003710: 6d69 7a65 5f77 6569 6768 7473 5f77 6174  mize_weights_wat
+00003720: 6572 5f73 7461 7274 222c 0d0a 2020 2020  er_start",..    
+00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003740: 226f 7074 696d 697a 655f 7765 6967 6874  "optimize_weight
+00003750: 735f 7761 7465 725f 656e 6422 2c0d 0a20  s_water_end",.. 
+00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003770: 2020 2022 6f70 7469 6d69 7a65 5f77 6569     "optimize_wei
+00003780: 6768 7473 5f6c 6970 6964 5f66 6c61 6722  ghts_lipid_flag"
+00003790: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000037a0: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
+000037b0: 5f77 6569 6768 7473 5f6c 6970 6964 5f73  _weights_lipid_s
+000037c0: 7461 7274 222c 0d0a 2020 2020 2020 2020  tart",..        
+000037d0: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
+000037e0: 696d 697a 655f 7765 6967 6874 735f 6c69  imize_weights_li
+000037f0: 7069 645f 656e 6422 2c0d 0a20 2020 2020  pid_end",..     
+00003800: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003810: 6f70 7469 6d69 7a65 5f77 6569 6768 7473  optimize_weights
+00003820: 5f73 6d61 6c6c 5f70 6561 6b5f 6661 6374  _small_peak_fact
+00003830: 6f72 222c 0d0a 2020 2020 2020 2020 2020  or",..          
+00003840: 2020 2020 2020 2020 2020 2263 6f6e 6669            "confi
+00003850: 6465 6e63 655f 696e 7465 7276 616c 735f  dence_intervals_
+00003860: 666c 6167 222c 2022 636f 6e66 6964 656e  flag", "confiden
+00003870: 6365 5f61 6c70 6861 222c 0d0a 2020 2020  ce_alpha",..    
+00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003890: 2263 6f6e 6669 6465 6e63 655f 6172 6561  "confidence_area
+000038a0: 5f66 6c61 6722 2c20 2263 6f6e 6669 6465  _flag", "confide
+000038b0: 6e63 655f 7070 6d5f 666c 6167 222c 0d0a  nce_ppm_flag",..
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 2020 2020 2263 6f6e 6669 6465 6e63 655f      "confidence_
+000038e0: 6c69 6e65 7769 6474 685f 666c 6167 222c  linewidth_flag",
+000038f0: 2022 636f 6e66 6964 656e 6365 5f70 6861   "confidence_pha
+00003900: 7365 5f66 6c61 6722 2c0d 0a20 2020 2020  se_flag",..     
+00003910: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003920: 6372 616d 6572 5f72 616f 5f66 6c61 6722  cramer_rao_flag"
+00003930: 2c20 2263 7261 6d65 725f 7261 6f5f 7070  , "cramer_rao_pp
+00003940: 6d5f 7374 6172 7422 2c0d 0a20 2020 2020  m_start",..     
+00003950: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003960: 6372 616d 6572 5f72 616f 5f70 706d 5f65  cramer_rao_ppm_e
+00003970: 6e64 222c 0d0a 2020 2020 2020 2020 2020  nd",..          
+00003980: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
+00003990: 2020 2020 2020 2020 2020 2020 2020 7574                ut
+000039a0: 696c 5f78 6d6c 2e54 6578 7453 7562 456c  il_xml.TextSubEl
+000039b0: 656d 656e 7428 652c 2061 7474 7269 6275  ement(e, attribu
+000039c0: 7465 2c20 6765 7461 7474 7228 7365 6c66  te, getattr(self
+000039d0: 2c20 6174 7472 6962 7574 6529 290d 0a0d  , attribute))...
+000039e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000039f0: 7365 6c66 2e6d 6163 726f 6d6f 6c5f 7369  self.macromol_si
+00003a00: 6e67 6c65 5f62 6173 6973 5f64 6174 6173  ngle_basis_datas
+00003a10: 6574 3a0d 0a20 2020 2020 2020 2020 2020  et:..           
+00003a20: 2020 2020 2023 2049 6e20 7468 6520 6e65       # In the ne
+00003a30: 7874 206c 696e 652c 2077 6520 2a68 6176  xt line, we *hav
+00003a40: 652a 2074 6f20 7361 7665 2074 6865 2075  e* to save the u
+00003a50: 7569 6420 7661 6c75 6573 2066 726f 6d20  uid values from 
+00003a60: 7468 6520 0d0a 2020 2020 2020 2020 2020  the ..          
+00003a70: 2020 2020 2020 2320 6163 7475 616c 206f        # actual o
+00003a80: 626a 6563 7420 7261 7468 6572 2074 6861  bject rather tha
+00003a90: 6e20 6672 6f6d 2074 6865 2061 7474 7269  n from the attri
+00003aa0: 6275 7465 2061 626f 7665 2c20 696e 2020  bute above, in  
+00003ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003ac0: 2020 2320 6f72 6465 7220 666f 7220 7468    # order for th
+00003ad0: 6520 6173 736f 6369 6174 6564 2064 6174  e associated dat
+00003ae0: 6173 6574 2075 7569 6420 746f 2072 6566  aset uuid to ref
+00003af0: 6c65 6374 2074 6865 206e 6577 2069 640d  lect the new id.
+00003b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b10: 2023 2074 6861 7420 6973 2067 6976 656e   # that is given
+00003b20: 2069 6e20 7468 6520 746f 7020 6c65 7665   in the top leve
+00003b30: 6c20 6461 7461 7365 742e 2041 7373 6f63  l dataset. Assoc
+00003b40: 6961 7465 6420 6461 7461 7365 7473 2061  iated datasets a
+00003b50: 7265 0d0a 2020 2020 2020 2020 2020 2020  re..            
+00003b60: 2020 2020 2320 6769 7665 6e20 6e65 7720      # given new 
+00003b70: 7465 6d70 6f72 6172 7920 7575 6964 2076  temporary uuid v
+00003b80: 616c 7565 7320 736f 2074 6861 7420 6966  alues so that if
+00003b90: 2074 6865 206d 6169 6e20 6461 7461 7365   the main datase
+00003ba0: 7420 6973 200d 0a20 2020 2020 2020 2020  t is ..         
+00003bb0: 2020 2020 2020 2023 2073 6176 6564 2061         # saved a
+00003bc0: 6e64 2069 6d6d 6564 6961 7465 6c79 206c  nd immediately l
+00003bd0: 6f61 6465 6420 6261 636b 2069 6e2c 2077  oaded back in, w
+00003be0: 6520 646f 206e 6f74 2067 6574 2063 6f6c  e do not get col
+00003bf0: 6c69 7369 6f6e 730d 0a20 2020 2020 2020  lisions..       
+00003c00: 2020 2020 2020 2020 2023 2062 6574 7765           # betwe
+00003c10: 656e 2074 6865 206e 6577 6c79 206f 7065  en the newly ope
+00003c20: 6e65 6420 6461 7461 7365 7473 2061 6e64  ned datasets and
+00003c30: 2061 6c72 6561 6479 2065 7869 7374 696e   already existin
+00003c40: 6720 6f6e 6573 2e0d 0a20 2020 2020 2020  g ones...       
+00003c50: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003c60: 2020 2020 2020 2020 2020 2075 7469 6c5f             util_
+00003c70: 786d 6c2e 5465 7874 5375 6245 6c65 6d65  xml.TextSubEleme
+00003c80: 6e74 2865 2c20 226d 6163 726f 6d6f 6c5f  nt(e, "macromol_
+00003c90: 7369 6e67 6c65 5f62 6173 6973 5f64 6174  single_basis_dat
+00003ca0: 6173 6574 5f69 6422 2c20 7365 6c66 2e6d  aset_id", self.m
+00003cb0: 6163 726f 6d6f 6c5f 7369 6e67 6c65 5f62  acromol_single_b
+00003cc0: 6173 6973 5f64 6174 6173 6574 2e69 6429  asis_dataset.id)
+00003cd0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00003ce0: 2020 652e 6170 7065 6e64 2873 656c 662e    e.append(self.
+00003cf0: 7072 696f 722e 6465 666c 6174 6528 2929  prior.deflate())
+00003d00: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00003d10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003d20: 726e 2065 0d0a 2020 2020 2020 2020 2020  rn e..          
+00003d30: 2020 0d0a 2020 2020 2020 2020 656c 6966    ..        elif
+00003d40: 2066 6c61 766f 7220 3d3d 2044 6566 6c61   flavor == Defla
+00003d50: 7465 2e44 4943 5449 4f4e 4152 593a 0d0a  te.DICTIONARY:..
+00003d60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003d70: 726e 2073 656c 662e 5f5f 6469 6374 5f5f  rn self.__dict__
+00003d80: 2e63 6f70 7928 290d 0a0d 0a0d 0a20 2020  .copy()......   
+00003d90: 2064 6566 2069 6e66 6c61 7465 2873 656c   def inflate(sel
+00003da0: 662c 2073 6f75 7263 6529 3a0d 0a20 2020  f, source):..   
+00003db0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00003dc0: 736f 7572 6365 2c20 226d 616b 6565 6c65  source, "makeele
+00003dd0: 6d65 6e74 2229 3a0d 0a20 2020 2020 2020  ment"):..       
+00003de0: 2020 2020 2023 2051 7561 636b 7320 6c69       # Quacks li
+00003df0: 6b65 2061 6e20 456c 656d 656e 7454 7265  ke an ElementTre
+00003e00: 652e 456c 656d 656e 740d 0a20 2020 2020  e.Element..     
+00003e10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003e20: 2020 2020 2023 2057 6520 696e 666c 6174       # We inflat
+00003e30: 6520 696e 2061 7474 7269 6275 7465 7320  e in attributes 
+00003e40: 6772 6f75 7065 6420 6279 2074 7970 6520  grouped by type 
+00003e50: 7369 6e63 6520 7468 6572 6527 7320 736f  since there's so
+00003e60: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00003e70: 646f 6767 6f6e 6520 6d61 6e79 2061 7474  doggone many att
+00003e80: 7273 206f 6e20 7468 6973 2063 6c61 7373  rs on this class
+00003e90: 2e0d 0a20 2020 2020 2020 2020 2020 200d  ...            .
+00003ea0: 0a20 2020 2020 2020 2020 2020 2023 2042  .            # B
+00003eb0: 6f6f 6c65 616e 730d 0a20 2020 2020 2020  ooleans..       
+00003ec0: 2020 2020 2066 6f72 2061 7474 7269 6275       for attribu
+00003ed0: 7465 2069 6e20 2822 7072 696f 725f 6967  te in ("prior_ig
+00003ee0: 6e6f 7265 5f6d 6173 6b22 2c20 0d0a 2020  nore_mask", ..  
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 2020 2020 2020 2020 2020 2020 2269 6e69              "ini
+00003f10: 7469 616c 5f63 725f 6368 6f5f 7365 7061  tial_cr_cho_sepa
+00003f20: 7261 7469 6f6e 222c 0d0a 2020 2020 2020  ration",..      
+00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f40: 2020 2020 2020 2020 2269 6e69 7469 616c          "initial
+00003f50: 5f70 6561 6b5f 7365 6172 6368 5f61 6273  _peak_search_abs
+00003f60: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f80: 2020 2269 6e69 7469 616c 5f61 7070 6c79    "initial_apply
+00003f90: 5f6b 6f5f 6669 6c74 6572 222c 200d 0a20  _ko_filter", .. 
+00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fb0: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+00003fc0: 7365 6c69 6e65 5f73 6d6f 6f74 6869 6e67  seline_smoothing
+00003fd0: 5f66 6c61 6722 2c0d 0a20 2020 2020 2020  _flag",..       
+00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ff0: 2020 2020 2020 2022 6261 7365 6c69 6e65         "baseline
+00004000: 5f73 6b69 705f 6c61 7374 5f73 6d6f 6f74  _skip_last_smoot
+00004010: 6822 2c0d 0a20 2020 2020 2020 2020 2020  h",..           
+00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004030: 2020 2022 6f70 7469 6d69 7a65 5f73 6361     "optimize_sca
+00004040: 6c69 6e67 5f66 6c61 6722 2c20 2020 2020  ling_flag",     
+00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004060: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004080: 2020 2020 2020 2020 2022 6f70 7469 6d69           "optimi
+00004090: 7a65 5f77 6569 6768 7473 5f6c 6970 6964  ze_weights_lipid
+000040a0: 5f66 6c61 6722 2c0d 0a20 2020 2020 2020  _flag",..       
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
+000040d0: 5f77 6569 6768 7473 5f77 6174 6572 5f66  _weights_water_f
+000040e0: 6c61 6722 2c0d 0a20 2020 2020 2020 2020  lag",..         
+000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004100: 2020 2020 2022 636f 6e66 6964 656e 6365       "confidence
+00004110: 5f69 6e74 6572 7661 6c73 5f66 6c61 6722  _intervals_flag"
+00004120: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004140: 2022 636f 6e66 6964 656e 6365 5f61 7265   "confidence_are
+00004150: 615f 666c 6167 222c 200d 0a20 2020 2020  a_flag", ..     
+00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004170: 2020 2020 2020 2020 2022 636f 6e66 6964           "confid
+00004180: 656e 6365 5f70 706d 5f66 6c61 6722 2c0d  ence_ppm_flag",.
+00004190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000041b0: 636f 6e66 6964 656e 6365 5f6c 696e 6577  confidence_linew
+000041c0: 6964 7468 5f66 6c61 6722 2c0d 0a20 2020  idth_flag",..   
+000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041e0: 2020 2020 2020 2020 2020 2022 636f 6e66             "conf
+000041f0: 6964 656e 6365 5f70 6861 7365 5f66 6c61  idence_phase_fla
+00004200: 6722 2c20 0d0a 2020 2020 2020 2020 2020  g", ..          
+00004210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004220: 2020 2020 2263 7261 6d65 725f 7261 6f5f      "cramer_rao_
+00004230: 666c 6167 222c 0d0a 2020 2020 2020 2020  flag",..        
+00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004250: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00004260: 2020 2020 2020 2020 2069 7465 6d20 3d20           item = 
+00004270: 736f 7572 6365 2e66 696e 6474 6578 7428  source.findtext(
+00004280: 6174 7472 6962 7574 6529 0d0a 2020 2020  attribute)..    
+00004290: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000042a0: 7465 6d20 6973 206e 6f74 204e 6f6e 653a  tem is not None:
+000042b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000042c0: 2020 2020 2020 7365 7461 7474 7228 7365        setattr(se
+000042d0: 6c66 2c20 6174 7472 6962 7574 652c 2075  lf, attribute, u
+000042e0: 7469 6c5f 786d 6c2e 424f 4f4c 4541 4e53  til_xml.BOOLEANS
+000042f0: 5b69 7465 6d5d 290d 0a20 2020 2020 2020  [item])..       
+00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004310: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00004320: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004330: 2020 2020 2020 2020 2023 2066 6c6f 6174           # float
+00004340: 730d 0a20 2020 2020 2020 2020 2020 2066  s..            f
+00004350: 6f72 2061 7474 7269 6275 7465 2069 6e20  or attribute in 
+00004360: 2822 7072 696f 725f 7070 6d5f 7374 6172  ("prior_ppm_star
+00004370: 7422 2c20 0d0a 2020 2020 2020 2020 2020  t", ..          
+00004380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004390: 2020 2020 2270 7269 6f72 5f70 706d 5f65      "prior_ppm_e
+000043a0: 6e64 222c 200d 0a20 2020 2020 2020 2020  nd", ..         
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 2020 2020 2022 696e 6974 6961 6c5f 6230       "initial_b0
+000043d0: 5f76 616c 7565 222c 200d 0a20 2020 2020  _value", ..     
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
+00004400: 6c5f 6261 7365 6c69 6e65 5f6c 6f77 6573  l_baseline_lowes
+00004410: 735f 7769 6474 6822 2c0d 0a20 2020 2020  s_width",..     
+00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004430: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
+00004440: 6c5f 6261 7365 6c69 6e65 5f6c 6f77 6573  l_baseline_lowes
+00004450: 735f 6465 6c74 6122 2c0d 0a20 2020 2020  s_delta",..     
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
+00004480: 6c5f 6261 7365 6c69 6e65 5f6c 6f77 6573  l_baseline_lowes
+00004490: 735f 6967 6e6f 7265 5f77 6964 7468 222c  s_ignore_width",
+000044a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044c0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-000044d0: 6e69 7469 616c 5f61 7070 6c79 5f6b 6f5f  nitial_apply_ko_
-000044e0: 6669 6c74 6572 222c 200d 0a20 2020 2020  filter", ..     
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 2020 2020 2020 2022 6261 7365 6c69           "baseli
-00004510: 6e65 5f73 6d6f 6f74 6869 6e67 5f66 6c61  ne_smoothing_fla
-00004520: 6722 2c0d 0a20 2020 2020 2020 2020 2020  g",..           
-00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004540: 2020 2022 6261 7365 6c69 6e65 5f73 6b69     "baseline_ski
-00004550: 705f 6c61 7374 5f73 6d6f 6f74 6822 2c0d  p_last_smooth",.
-00004560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004570: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004580: 6f70 7469 6d69 7a65 5f73 6361 6c69 6e67  optimize_scaling
-00004590: 5f66 6c61 6722 2c20 2020 2020 2020 2020  _flag",         
+000044c0: 2269 6e69 7469 616c 5f6c 696e 6577 6964  "initial_linewid
+000044d0: 7468 5f76 616c 7565 222c 0d0a 2020 2020  th_value",..    
+000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 2020 2020 2020 2020 2020 2269 6e69 7469            "initi
+00004500: 616c 5f6c 696e 6577 6964 7468 5f72 616e  al_linewidth_ran
+00004510: 6765 5f73 7461 7274 222c 0d0a 2020 2020  ge_start",..    
+00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004530: 2020 2020 2020 2020 2020 2269 6e69 7469            "initi
+00004540: 616c 5f6c 696e 6577 6964 7468 5f72 616e  al_linewidth_ran
+00004550: 6765 5f65 6e64 222c 200d 0a20 2020 2020  ge_end", ..     
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
+00004580: 6c5f 6c69 6e65 7769 6474 685f 6675 6467  l_linewidth_fudg
+00004590: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
 000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045d0: 2020 2020 2022 6f70 7469 6d69 7a65 5f77       "optimize_w
-000045e0: 6569 6768 7473 5f6c 6970 6964 5f66 6c61  eights_lipid_fla
-000045f0: 6722 2c0d 0a20 2020 2020 2020 2020 2020  g",..           
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2022 6f70 7469 6d69 7a65 5f77 6569     "optimize_wei
-00004620: 6768 7473 5f77 6174 6572 5f66 6c61 6722  ghts_water_flag"
-00004630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004650: 2022 636f 6e66 6964 656e 6365 5f69 6e74   "confidence_int
-00004660: 6572 7661 6c73 5f66 6c61 6722 2c0d 0a20  ervals_flag",.. 
-00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004680: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00004690: 6e66 6964 656e 6365 5f61 7265 615f 666c  nfidence_area_fl
-000046a0: 6167 222c 200d 0a20 2020 2020 2020 2020  ag", ..         
-000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046c0: 2020 2020 2022 636f 6e66 6964 656e 6365       "confidence
-000046d0: 5f70 706d 5f66 6c61 6722 2c0d 0a20 2020  _ppm_flag",..   
-000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 2020 2020 2020 2022 636f 6e66             "conf
-00004700: 6964 656e 6365 5f6c 696e 6577 6964 7468  idence_linewidth
-00004710: 5f66 6c61 6722 2c0d 0a20 2020 2020 2020  _flag",..       
-00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 2020 2020 2022 636f 6e66 6964 656e         "confiden
-00004740: 6365 5f70 6861 7365 5f66 6c61 6722 2c20  ce_phase_flag", 
-00004750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2263 7261 6d65 725f 7261 6f5f 666c 6167  "cramer_rao_flag
-00004780: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047a0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-000047b0: 2020 2020 2069 7465 6d20 3d20 736f 7572       item = sour
-000047c0: 6365 2e66 696e 6474 6578 7428 6174 7472  ce.findtext(attr
-000047d0: 6962 7574 6529 0d0a 2020 2020 2020 2020  ibute)..        
-000047e0: 2020 2020 2020 2020 6966 2069 7465 6d20          if item 
-000047f0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2020 7365 7461 7474 7228 7365 6c66 2c20    setattr(self, 
-00004820: 6174 7472 6962 7574 652c 2075 7469 6c5f  attribute, util_
-00004830: 786d 6c2e 424f 4f4c 4541 4e53 5b69 7465  xml.BOOLEANS[ite
-00004840: 6d5d 290d 0a20 2020 2020 2020 2020 2020  m])..           
-00004850: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004870: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00004880: 2020 2020 2023 2066 6c6f 6174 730d 0a20       # floats.. 
-00004890: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
-000048a0: 7474 7269 6275 7465 2069 6e20 2822 7072  ttribute in ("pr
-000048b0: 696f 725f 7070 6d5f 7374 6172 7422 2c20  ior_ppm_start", 
-000048c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2270 7269 6f72 5f70 706d 5f65 6e64 222c  "prior_ppm_end",
-000048f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2022 696e 6974 6961 6c5f 6230 5f76 616c   "initial_b0_val
-00004920: 7565 222c 200d 0a20 2020 2020 2020 2020  ue", ..         
+000045b0: 2020 2022 696e 6974 6961 6c5f 7068 6173     "initial_phas
+000045c0: 6530 5f76 616c 7565 222c 200d 0a20 2020  e0_value", ..   
+000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045e0: 2020 2020 2020 2020 2020 2022 696e 6974             "init
+000045f0: 6961 6c5f 7068 6173 6531 5f76 616c 7565  ial_phase1_value
+00004600: 222c 200d 0a20 2020 2020 2020 2020 2020  ", ..           
+00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004620: 2020 2022 696e 6974 6961 6c5f 6b6f 5f6c     "initial_ko_l
+00004630: 696e 6577 6964 7468 5f6d 696e 696d 756d  inewidth_minimum
+00004640: 222c 200d 0a20 2020 2020 2020 2020 2020  ", ..           
+00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004660: 2020 2022 696e 6974 6961 6c5f 7068 6173     "initial_phas
+00004670: 6531 5f66 6964 5f63 6f6e 7374 616e 7422  e1_fid_constant"
+00004680: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2022 696e 6974 6961 6c5f 6c61 635f 6d65   "initial_lac_me
+000046b0: 7468 6f64 222c 0d0a 2020 2020 2020 2020  thod",..        
+000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046d0: 2020 2020 2020 2262 6173 656c 696e 655f        "baseline_
+000046e0: 736d 6f6f 7468 696e 675f 7769 6474 6822  smoothing_width"
+000046f0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00004700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004710: 2020 2262 6173 656c 696e 655f 736d 6f6f    "baseline_smoo
+00004720: 7468 696e 675f 6465 6c74 6122 2c0d 0a20  thing_delta",.. 
+00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+00004750: 7365 6c69 6e65 5f75 6e64 6572 6573 7469  seline_underesti
+00004760: 6d61 7465 222c 200d 0a20 2020 2020 2020  mate", ..       
+00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004780: 2020 2020 2020 2022 6261 7365 6c69 6e65         "baseline
+00004790: 5f77 6176 656c 6574 5f6d 696e 5f64 7961  _wavelet_min_dya
+000047a0: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047c0: 2020 2022 6d61 6372 6f6d 6f6c 5f73 696e     "macromol_sin
+000047d0: 676c 655f 6261 7369 735f 6461 7461 7365  gle_basis_datase
+000047e0: 745f 7374 6172 745f 6172 6561 222c 0d0a  t_start_area",..
+000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004800: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+00004810: 7074 696d 697a 655f 7374 6f70 5f74 6f6c  ptimize_stop_tol
+00004820: 6572 616e 6365 222c 200d 0a20 2020 2020  erance", ..     
+00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004840: 2020 2020 2020 2020 2022 6f70 7469 6d69           "optimi
+00004850: 7a65 5f6c 696d 6974 735f 7261 6e67 655f  ze_limits_range_
+00004860: 6172 6561 222c 0d0a 2020 2020 2020 2020  area",..        
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2020 2020 2020 226f 7074 696d 697a 655f        "optimize_
+00004890: 6c69 6d69 7473 5f72 616e 6765 5f70 706d  limits_range_ppm
+000048a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048c0: 2020 226f 7074 696d 697a 655f 6c69 6d69    "optimize_limi
+000048d0: 7473 5f72 616e 6765 5f70 6861 7365 3022  ts_range_phase0"
+000048e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 2022 6f70 7469 6d69 7a65 5f6c 696d 6974   "optimize_limit
+00004910: 735f 7261 6e67 655f 7068 6173 6531 222c  s_range_phase1",
+00004920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2020 2020 2022 696e 6974 6961 6c5f 6261       "initial_ba
-00004950: 7365 6c69 6e65 5f6c 6f77 6573 735f 7769  seline_lowess_wi
-00004960: 6474 6822 2c0d 0a20 2020 2020 2020 2020  dth",..         
+00004940: 226f 7074 696d 697a 655f 6c69 6d69 7473  "optimize_limits
+00004950: 5f6d 6178 5f6c 696e 6577 6964 7468 222c  _max_linewidth",
+00004960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2020 2020 2022 696e 6974 6961 6c5f 6261       "initial_ba
-00004990: 7365 6c69 6e65 5f6c 6f77 6573 735f 6465  seline_lowess_de
-000049a0: 6c74 6122 2c0d 0a20 2020 2020 2020 2020  lta",..         
+00004980: 226f 7074 696d 697a 655f 6c69 6d69 7473  "optimize_limits
+00004990: 5f6d 696e 5f6c 696e 6577 6964 7468 222c  _min_linewidth",
+000049a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049c0: 2020 2020 2022 696e 6974 6961 6c5f 6261       "initial_ba
-000049d0: 7365 6c69 6e65 5f6c 6f77 6573 735f 6967  seline_lowess_ig
-000049e0: 6e6f 7265 5f77 6964 7468 222c 0d0a 2020  nore_width",..  
+000049c0: 226f 7074 696d 697a 655f 7765 6967 6874  "optimize_weight
+000049d0: 735f 7363 616c 655f 6661 6374 6f72 222c  s_scale_factor",
+000049e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 2020 2020 2020 2020 2020 2269 6e69              "ini
-00004a10: 7469 616c 5f6c 696e 6577 6964 7468 5f76  tial_linewidth_v
-00004a20: 616c 7565 222c 0d0a 2020 2020 2020 2020  alue",..        
+00004a00: 226f 7074 696d 697a 655f 7765 6967 6874  "optimize_weight
+00004a10: 735f 7769 6474 685f 6661 6374 6f72 222c  s_width_factor",
+00004a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2020 2020 2020 2269 6e69 7469 616c 5f6c        "initial_l
-00004a50: 696e 6577 6964 7468 5f72 616e 6765 5f73  inewidth_range_s
-00004a60: 7461 7274 222c 0d0a 2020 2020 2020 2020  tart",..        
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 2020 2020 2269 6e69 7469 616c 5f6c        "initial_l
-00004a90: 696e 6577 6964 7468 5f72 616e 6765 5f65  inewidth_range_e
-00004aa0: 6e64 222c 200d 0a20 2020 2020 2020 2020  nd", ..         
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2020 2020 2022 696e 6974 6961 6c5f 6c69       "initial_li
-00004ad0: 6e65 7769 6474 685f 6675 6467 6522 2c0d  newidth_fudge",.
-00004ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004af0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004b00: 696e 6974 6961 6c5f 7068 6173 6530 5f76  initial_phase0_v
-00004b10: 616c 7565 222c 200d 0a20 2020 2020 2020  alue", ..       
+00004a40: 226f 7074 696d 697a 655f 7765 6967 6874  "optimize_weight
+00004a50: 735f 7761 7465 725f 7374 6172 7422 2c0d  s_water_start",.
+00004a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004a70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004a80: 6f70 7469 6d69 7a65 5f77 6569 6768 7473  optimize_weights
+00004a90: 5f77 6174 6572 5f65 6e64 222c 0d0a 2020  _water_end",..  
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ab0: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
+00004ac0: 696d 697a 655f 7765 6967 6874 735f 6c69  imize_weights_li
+00004ad0: 7069 645f 7374 6172 7422 2c0d 0a20 2020  pid_start",..   
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004af0: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
+00004b00: 6d69 7a65 5f77 6569 6768 7473 5f6c 6970  mize_weights_lip
+00004b10: 6964 5f65 6e64 222c 0d0a 2020 2020 2020  id_end",..      
 00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 2020 2020 2020 2022 696e 6974 6961 6c5f         "initial_
-00004b40: 7068 6173 6531 5f76 616c 7565 222c 200d  phase1_value", .
-00004b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004b70: 696e 6974 6961 6c5f 6b6f 5f6c 696e 6577  initial_ko_linew
-00004b80: 6964 7468 5f6d 696e 696d 756d 222c 200d  idth_minimum", .
-00004b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004bb0: 696e 6974 6961 6c5f 7068 6173 6531 5f66  initial_phase1_f
-00004bc0: 6964 5f63 6f6e 7374 616e 7422 2c0d 0a20  id_constant",.. 
+00004b30: 2020 2020 2020 2020 226f 7074 696d 697a          "optimiz
+00004b40: 655f 7765 6967 6874 735f 736d 616c 6c5f  e_weights_small_
+00004b50: 7065 616b 5f66 6163 746f 7222 2c20 0d0a  peak_factor", ..
+00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00004b80: 6f6e 6669 6465 6e63 655f 616c 7068 6122  onfidence_alpha"
+00004b90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bb0: 2022 6372 616d 6572 5f72 616f 5f70 706d   "cramer_rao_ppm
+00004bc0: 5f73 7461 7274 222c 200d 0a20 2020 2020  _start", ..     
 00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004be0: 2020 2020 2020 2020 2020 2020 2022 696e               "in
-00004bf0: 6974 6961 6c5f 6c61 635f 6d65 7468 6f64  itial_lac_method
-00004c00: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c20: 2020 2262 6173 656c 696e 655f 736d 6f6f    "baseline_smoo
-00004c30: 7468 696e 675f 7769 6474 6822 2c20 0d0a  thing_width", ..
-00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c50: 2020 2020 2020 2020 2020 2020 2020 2262                "b
-00004c60: 6173 656c 696e 655f 736d 6f6f 7468 696e  aseline_smoothin
-00004c70: 675f 6465 6c74 6122 2c0d 0a20 2020 2020  g_delta",..     
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2020 2020 2022 6261 7365 6c69           "baseli
-00004ca0: 6e65 5f75 6e64 6572 6573 7469 6d61 7465  ne_underestimate
-00004cb0: 222c 200d 0a20 2020 2020 2020 2020 2020  ", ..           
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2022 6261 7365 6c69 6e65 5f77 6176     "baseline_wav
-00004ce0: 656c 6574 5f6d 696e 5f64 7961 6422 2c0d  elet_min_dyad",.
-00004cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004d10: 6d61 6372 6f6d 6f6c 5f73 696e 676c 655f  macromol_single_
-00004d20: 6261 7369 735f 6461 7461 7365 745f 7374  basis_dataset_st
-00004d30: 6172 745f 6172 6561 222c 0d0a 2020 2020  art_area",..    
+00004be0: 2020 2020 2020 2020 2022 6372 616d 6572           "cramer
+00004bf0: 5f72 616f 5f70 706d 5f65 6e64 222c 0d0a  _rao_ppm_end",..
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
+00004c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c30: 2069 7465 6d20 3d20 736f 7572 6365 2e66   item = source.f
+00004c40: 696e 6474 6578 7428 6174 7472 6962 7574  indtext(attribut
+00004c50: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00004c60: 2020 2020 6966 2069 7465 6d20 6973 206e      if item is n
+00004c70: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00004c80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004c90: 7461 7474 7228 7365 6c66 2c20 6174 7472  tattr(self, attr
+00004ca0: 6962 7574 652c 2066 6c6f 6174 2869 7465  ibute, float(ite
+00004cb0: 6d29 290d 0a0d 0a20 2020 2020 2020 2020  m))....         
+00004cc0: 2020 2023 2069 6e74 730d 0a20 2020 2020     # ints..     
+00004cd0: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
+00004ce0: 6275 7465 2069 6e20 2822 696e 6974 6961  bute in ("initia
+00004cf0: 6c5f 6b6f 5f70 6f69 6e74 7322 2c0d 0a20  l_ko_points",.. 
+00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d10: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+00004d20: 6974 6961 6c5f 7065 616b 5f6e 6567 6174  itial_peak_negat
+00004d30: 6976 655f 666c 6167 222c 0d0a 2020 2020  ive_flag",..    
 00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d50: 2020 2020 2020 2020 2020 226f 7074 696d            "optim
-00004d60: 697a 655f 7374 6f70 5f74 6f6c 6572 616e  ize_stop_toleran
-00004d70: 6365 222c 200d 0a20 2020 2020 2020 2020  ce", ..         
+00004d50: 2020 2020 2020 2020 2020 2262 6173 656c            "basel
+00004d60: 696e 655f 7370 6c69 6e65 5f6e 6b6e 6f74  ine_spline_nknot
+00004d70: 7322 2c20 0d0a 2020 2020 2020 2020 2020  s", ..          
 00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d90: 2020 2020 2022 6f70 7469 6d69 7a65 5f6c       "optimize_l
-00004da0: 696d 6974 735f 7261 6e67 655f 6172 6561  imits_range_area
-00004db0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dd0: 2020 226f 7074 696d 697a 655f 6c69 6d69    "optimize_limi
-00004de0: 7473 5f72 616e 6765 5f70 706d 222c 0d0a  ts_range_ppm",..
+00004d90: 2020 2020 2262 6173 656c 696e 655f 7370      "baseline_sp
+00004da0: 6c69 6e65 5f73 7061 6369 6e67 222c 0d0a  line_spacing",..
+00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00004dd0: 6173 656c 696e 655f 7370 6c69 6e65 5f6f  aseline_spline_o
+00004de0: 7264 6572 222c 0d0a 2020 2020 2020 2020  rder",..        
 00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e00: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-00004e10: 7074 696d 697a 655f 6c69 6d69 7473 5f72  ptimize_limits_r
-00004e20: 616e 6765 5f70 6861 7365 3022 2c0d 0a20  ange_phase0",.. 
-00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 2020 2020 2020 2020 2020 2020 2022 6f70               "op
-00004e50: 7469 6d69 7a65 5f6c 696d 6974 735f 7261  timize_limits_ra
-00004e60: 6e67 655f 7068 6173 6531 222c 0d0a 2020  nge_phase1",..  
+00004e00: 2020 2020 2020 2262 6173 656c 696e 655f        "baseline_
+00004e10: 7761 7665 6c65 745f 7363 616c 6522 2c0d  wavelet_scale",.
+00004e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004e30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004e40: 6261 7365 6c69 6e65 5f77 6176 656c 6574  baseline_wavelet
+00004e50: 5f73 6872 696e 6b61 6765 5f66 6c61 6722  _shrinkage_flag"
+00004e60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e80: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
-00004e90: 696d 697a 655f 6c69 6d69 7473 5f6d 6178  imize_limits_max
-00004ea0: 5f6c 696e 6577 6964 7468 222c 0d0a 2020  _linewidth",..  
+00004e80: 2022 6261 7365 6c69 6e65 5f77 6176 656c   "baseline_wavel
+00004e90: 6574 5f69 6e76 6172 6961 6e63 655f 6c61  et_invariance_la
+00004ea0: 6722 2c0d 0a20 2020 2020 2020 2020 2020  g",..           
 00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ec0: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
-00004ed0: 696d 697a 655f 6c69 6d69 7473 5f6d 696e  imize_limits_min
-00004ee0: 5f6c 696e 6577 6964 7468 222c 0d0a 2020  _linewidth",..  
+00004ec0: 2020 2022 6261 7365 6c69 6e65 5f77 6176     "baseline_wav
+00004ed0: 656c 6574 5f69 6e76 6172 6961 6e63 655f  elet_invariance_
+00004ee0: 7265 636f 6d62 696e 6522 2c0d 0a20 2020  recombine",..   
 00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f00: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
-00004f10: 696d 697a 655f 7765 6967 6874 735f 7363  imize_weights_sc
-00004f20: 616c 655f 6661 6374 6f72 222c 0d0a 2020  ale_factor",..  
+00004f00: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
+00004f10: 6d69 7a65 5f6d 6178 5f69 7465 7261 7469  mize_max_iterati
+00004f20: 6f6e 7322 2c0d 0a20 2020 2020 2020 2020  ons",..         
 00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f40: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
-00004f50: 696d 697a 655f 7765 6967 6874 735f 7769  imize_weights_wi
-00004f60: 6474 685f 6661 6374 6f72 222c 0d0a 2020  dth_factor",..  
+00004f40: 2020 2020 2022 6f70 7469 6d69 7a65 5f67       "optimize_g
+00004f50: 6c6f 6261 6c5f 6974 6572 6174 696f 6e73  lobal_iterations
+00004f60: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
 00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f80: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
-00004f90: 696d 697a 655f 7765 6967 6874 735f 7761  imize_weights_wa
-00004fa0: 7465 725f 7374 6172 7422 2c0d 0a20 2020  ter_start",..   
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fc0: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
-00004fd0: 6d69 7a65 5f77 6569 6768 7473 5f77 6174  mize_weights_wat
-00004fe0: 6572 5f65 6e64 222c 0d0a 2020 2020 2020  er_end",..      
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2020 2020 2020 226f 7074 696d 697a          "optimiz
-00005010: 655f 7765 6967 6874 735f 6c69 7069 645f  e_weights_lipid_
-00005020: 7374 6172 7422 2c0d 0a20 2020 2020 2020  start",..       
-00005030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005040: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
-00005050: 5f77 6569 6768 7473 5f6c 6970 6964 5f65  _weights_lipid_e
-00005060: 6e64 222c 0d0a 2020 2020 2020 2020 2020  nd",..          
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2020 2020 226f 7074 696d 697a 655f 7765      "optimize_we
-00005090: 6967 6874 735f 736d 616c 6c5f 7065 616b  ights_small_peak
-000050a0: 5f66 6163 746f 7222 2c20 0d0a 2020 2020  _factor", ..    
-000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050c0: 2020 2020 2020 2020 2020 2263 6f6e 6669            "confi
-000050d0: 6465 6e63 655f 616c 7068 6122 2c0d 0a20  dence_alpha",.. 
-000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050f0: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
-00005100: 616d 6572 5f72 616f 5f70 706d 5f73 7461  amer_rao_ppm_sta
-00005110: 7274 222c 200d 0a20 2020 2020 2020 2020  rt", ..         
-00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2020 2020 2022 6372 616d 6572 5f72 616f       "cramer_rao
-00005140: 5f70 706d 5f65 6e64 222c 0d0a 2020 2020  _ppm_end",..    
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
-00005170: 2020 2020 2020 2020 2020 2020 2069 7465               ite
-00005180: 6d20 3d20 736f 7572 6365 2e66 696e 6474  m = source.findt
-00005190: 6578 7428 6174 7472 6962 7574 6529 0d0a  ext(attribute)..
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051b0: 6966 2069 7465 6d20 6973 206e 6f74 204e  if item is not N
-000051c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000051d0: 2020 2020 2020 2020 2020 7365 7461 7474            setatt
-000051e0: 7228 7365 6c66 2c20 6174 7472 6962 7574  r(self, attribut
-000051f0: 652c 2066 6c6f 6174 2869 7465 6d29 290d  e, float(item)).
-00005200: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00005210: 2069 6e74 730d 0a20 2020 2020 2020 2020   ints..         
-00005220: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
-00005230: 2069 6e20 2822 696e 6974 6961 6c5f 6b6f   in ("initial_ko
-00005240: 5f70 6f69 6e74 7322 2c0d 0a20 2020 2020  _points",..     
+00004f80: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+00004f90: 2020 2020 2069 7465 6d20 3d20 736f 7572       item = sour
+00004fa0: 6365 2e66 696e 6474 6578 7428 6174 7472  ce.findtext(attr
+00004fb0: 6962 7574 6529 0d0a 2020 2020 2020 2020  ibute)..        
+00004fc0: 2020 2020 2020 2020 6966 2069 7465 6d20          if item 
+00004fd0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ff0: 2020 7365 7461 7474 7228 7365 6c66 2c20    setattr(self, 
+00005000: 6174 7472 6962 7574 652c 2069 6e74 2866  attribute, int(f
+00005010: 6c6f 6174 2869 7465 6d29 2929 0d0a 0d0a  loat(item)))....
+00005020: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
+00005030: 2074 7261 6e73 6c61 7469 6f6e 2072 6571   translation req
+00005040: 7569 7265 6420 666f 7220 7468 6573 6520  uired for these 
+00005050: 6174 7472 730d 0a20 2020 2020 2020 2020  attrs..         
+00005060: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
+00005070: 2069 6e20 2822 7072 696f 725f 6d61 736b   in ("prior_mask
+00005080: 5f73 6f75 7263 6522 2c20 0d0a 2020 2020  _source", ..    
+00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050a0: 2020 2020 2020 2020 2020 226c 696e 6573            "lines
+000050b0: 6861 7065 5f6d 6f64 656c 222c 200d 0a20  hape_model", .. 
+000050c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050d0: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+000050e0: 6974 6961 6c5f 6230 5f73 6869 6674 5f6d  itial_b0_shift_m
+000050f0: 6574 686f 6422 2c0d 0a20 2020 2020 2020  ethod",..       
+00005100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005110: 2020 2020 2020 2022 696e 6974 6961 6c5f         "initial_
+00005120: 6261 7365 6c69 6e65 5f6d 6574 686f 6422  baseline_method"
+00005130: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005150: 2022 696e 6974 6961 6c5f 736d 616c 6c5f   "initial_small_
+00005160: 7065 616b 5f61 7265 6173 222c 0d0a 2020  peak_areas",..  
+00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005180: 2020 2020 2020 2020 2020 2020 2269 6e69              "ini
+00005190: 7469 616c 5f73 6d61 6c6c 5f70 6561 6b5f  tial_small_peak_
+000051a0: 6672 6571 7322 2c0d 0a20 2020 2020 2020  freqs",..       
+000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051c0: 2020 2020 2020 2022 696e 6974 6961 6c5f         "initial_
+000051d0: 6c69 6e65 7769 6474 685f 6d65 7468 6f64  linewidth_method
+000051e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 2020 2269 6e69 7469 616c 5f70 6861 7365    "initial_phase
+00005210: 5f6d 6574 686f 6422 2c20 0d0a 2020 2020  _method", ..    
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 2020 2020 2020 2020 2020 2262 6173 656c            "basel
+00005240: 696e 655f 6d65 7468 6f64 222c 0d0a 2020  ine_method",..  
 00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005260: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
-00005270: 6c5f 7065 616b 5f6e 6567 6174 6976 655f  l_peak_negative_
-00005280: 666c 6167 222c 0d0a 2020 2020 2020 2020  flag",..        
-00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052a0: 2020 2020 2020 2262 6173 656c 696e 655f        "baseline_
-000052b0: 7370 6c69 6e65 5f6e 6b6e 6f74 7322 2c20  spline_nknots", 
+00005260: 2020 2020 2020 2020 2020 2020 226d 6163              "mac
+00005270: 726f 6d6f 6c5f 6d6f 6465 6c22 2c0d 0a20  romol_model",.. 
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 2020 2020 2020 2022 6d61               "ma
+000052a0: 6372 6f6d 6f6c 5f73 696e 676c 655f 6261  cromol_single_ba
+000052b0: 7369 735f 6461 7461 7365 745f 6964 222c  sis_dataset_id",
 000052c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052e0: 2262 6173 656c 696e 655f 7370 6c69 6e65  "baseline_spline
-000052f0: 5f73 7061 6369 6e67 222c 0d0a 2020 2020  _spacing",..    
+000052e0: 226f 7074 696d 697a 655f 6d65 7468 6f64  "optimize_method
+000052f0: 222c 200d 0a20 2020 2020 2020 2020 2020  ", ..           
 00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005310: 2020 2020 2020 2020 2020 2262 6173 656c            "basel
-00005320: 696e 655f 7370 6c69 6e65 5f6f 7264 6572  ine_spline_order
-00005330: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005350: 2020 2262 6173 656c 696e 655f 7761 7665    "baseline_wave
-00005360: 6c65 745f 7363 616c 6522 2c0d 0a20 2020  let_scale",..   
-00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2020 2020 2020 2020 2022 6261 7365             "base
-00005390: 6c69 6e65 5f77 6176 656c 6574 5f73 6872  line_wavelet_shr
-000053a0: 696e 6b61 6765 5f66 6c61 6722 2c0d 0a20  inkage_flag",.. 
-000053b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053c0: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
-000053d0: 7365 6c69 6e65 5f77 6176 656c 6574 5f69  seline_wavelet_i
-000053e0: 6e76 6172 6961 6e63 655f 6c61 6722 2c0d  nvariance_lag",.
-000053f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005410: 6261 7365 6c69 6e65 5f77 6176 656c 6574  baseline_wavelet
-00005420: 5f69 6e76 6172 6961 6e63 655f 7265 636f  _invariance_reco
-00005430: 6d62 696e 6522 2c0d 0a20 2020 2020 2020  mbine",..       
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 2020 2022 6f70 7469 6d69 7a65         "optimize
-00005460: 5f6d 6178 5f69 7465 7261 7469 6f6e 7322  _max_iterations"
-00005470: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2022 6f70 7469 6d69 7a65 5f67 6c6f 6261   "optimize_globa
-000054a0: 6c5f 6974 6572 6174 696f 6e73 222c 0d0a  l_iterations",..
-000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054c0: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
-000054d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000054e0: 2069 7465 6d20 3d20 736f 7572 6365 2e66   item = source.f
-000054f0: 696e 6474 6578 7428 6174 7472 6962 7574  indtext(attribut
-00005500: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00005510: 2020 2020 6966 2069 7465 6d20 6973 206e      if item is n
-00005520: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00005530: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005540: 7461 7474 7228 7365 6c66 2c20 6174 7472  tattr(self, attr
-00005550: 6962 7574 652c 2069 6e74 2866 6c6f 6174  ibute, int(float
-00005560: 2869 7465 6d29 2929 0d0a 0d0a 2020 2020  (item)))....    
-00005570: 2020 2020 2020 2020 2320 4e6f 2074 7261          # No tra
-00005580: 6e73 6c61 7469 6f6e 2072 6571 7569 7265  nslation require
-00005590: 6420 666f 7220 7468 6573 6520 6174 7472  d for these attr
-000055a0: 730d 0a20 2020 2020 2020 2020 2020 2066  s..            f
-000055b0: 6f72 2061 7474 7269 6275 7465 2069 6e20  or attribute in 
-000055c0: 2822 7072 696f 725f 6d61 736b 5f73 6f75  ("prior_mask_sou
-000055d0: 7263 6522 2c20 0d0a 2020 2020 2020 2020  rce", ..        
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2020 226c 696e 6573 6861 7065        "lineshape
-00005600: 5f6d 6f64 656c 222c 200d 0a20 2020 2020  _model", ..     
-00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005620: 2020 2020 2020 2020 2022 696e 6974 6961           "initia
-00005630: 6c5f 6230 5f73 6869 6674 5f6d 6574 686f  l_b0_shift_metho
-00005640: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005660: 2020 2022 696e 6974 6961 6c5f 6261 7365     "initial_base
-00005670: 6c69 6e65 5f6d 6574 686f 6422 2c0d 0a20  line_method",.. 
-00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005690: 2020 2020 2020 2020 2020 2020 2022 696e               "in
-000056a0: 6974 6961 6c5f 736d 616c 6c5f 7065 616b  itial_small_peak
-000056b0: 5f61 7265 6173 222c 0d0a 2020 2020 2020  _areas",..      
-000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056d0: 2020 2020 2020 2020 2269 6e69 7469 616c          "initial
-000056e0: 5f73 6d61 6c6c 5f70 6561 6b5f 6672 6571  _small_peak_freq
-000056f0: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2022 696e 6974 6961 6c5f 6c69 6e65     "initial_line
-00005720: 7769 6474 685f 6d65 7468 6f64 222c 0d0a  width_method",..
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00005750: 6e69 7469 616c 5f70 6861 7365 5f6d 6574  nitial_phase_met
-00005760: 686f 6422 2c20 0d0a 2020 2020 2020 2020  hod", ..        
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 2020 2020 2020 2262 6173 656c 696e 655f        "baseline_
-00005790: 6d65 7468 6f64 222c 0d0a 2020 2020 2020  method",..      
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2020 2020 2020 2020 226d 6163 726f 6d6f          "macromo
-000057c0: 6c5f 6d6f 6465 6c22 2c0d 0a20 2020 2020  l_model",..     
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2020 2020 2020 2022 6d61 6372 6f6d           "macrom
-000057f0: 6f6c 5f73 696e 676c 655f 6261 7369 735f  ol_single_basis_
-00005800: 6461 7461 7365 745f 6964 222c 0d0a 2020  dataset_id",..  
-00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2020 2020 2020 2020 2020 226f 7074              "opt
-00005830: 696d 697a 655f 6d65 7468 6f64 222c 200d  imize_method", .
-00005840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005850: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005860: 6f70 7469 6d69 7a65 5f77 6569 6768 7473  optimize_weights
-00005870: 5f6d 6574 686f 6422 2c0d 0a20 2020 2020  _method",..     
-00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005890: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-000058a0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-000058b0: 203d 2073 6f75 7263 652e 6669 6e64 7465   = source.findte
-000058c0: 7874 2861 7474 7269 6275 7465 290d 0a20  xt(attribute).. 
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000058e0: 6620 6974 656d 2069 7320 6e6f 7420 4e6f  f item is not No
-000058f0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00005900: 2020 2020 2020 2020 2073 6574 6174 7472           setattr
-00005910: 2873 656c 662c 2061 7474 7269 6275 7465  (self, attribute
-00005920: 2c20 6974 656d 290d 0a0d 0a20 2020 2020  , item)....     
-00005930: 2020 2020 2020 2023 206c 6973 7473 0d0a         # lists..
-00005940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005950: 2e70 7269 6f72 5f6c 6973 7420 2020 2020  .prior_list     
-00005960: 2020 3d20 5b76 616c 2e74 6578 7420 666f    = [val.text fo
-00005970: 7220 7661 6c20 696e 2073 6f75 7263 652e  r val in source.
-00005980: 6765 7469 7465 7261 746f 7228 2270 7269  getiterator("pri
-00005990: 6f72 5f6c 6973 7422 295d 0d0a 2020 2020  or_list")]..    
-000059a0: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-000059b0: 6f72 5f61 7265 615f 7363 616c 6520 3d20  or_area_scale = 
-000059c0: 5b66 6c6f 6174 2876 616c 2e74 6578 7429  [float(val.text)
-000059d0: 2066 6f72 2076 616c 2069 6e20 736f 7572   for val in sour
-000059e0: 6365 2e67 6574 6974 6572 6174 6f72 2822  ce.getiterator("
-000059f0: 7072 696f 725f 6172 6561 5f73 6361 6c65  prior_area_scale
-00005a00: 2229 5d0d 0a20 2020 2020 2020 2020 2020  ")]..           
-00005a10: 2073 656c 662e 7072 696f 725f 7065 616b   self.prior_peak
-00005a20: 5f70 706d 2020 203d 205b 666c 6f61 7428  _ppm   = [float(
-00005a30: 7661 6c2e 7465 7874 2920 666f 7220 7661  val.text) for va
-00005a40: 6c20 696e 2073 6f75 7263 652e 6765 7469  l in source.geti
-00005a50: 7465 7261 746f 7228 2270 7269 6f72 5f70  terator("prior_p
-00005a60: 6561 6b5f 7070 6d22 295d 0d0a 2020 2020  eak_ppm")]..    
-00005a70: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-00005a80: 6f72 5f73 6561 7263 685f 7070 6d20 3d20  or_search_ppm = 
-00005a90: 5b66 6c6f 6174 2876 616c 2e74 6578 7429  [float(val.text)
-00005aa0: 2066 6f72 2076 616c 2069 6e20 736f 7572   for val in sour
-00005ab0: 6365 2e67 6574 6974 6572 6174 6f72 2822  ce.getiterator("
-00005ac0: 7072 696f 725f 7365 6172 6368 5f70 706d  prior_search_ppm
-00005ad0: 2229 5d0d 0a20 2020 2020 2020 2020 2020  ")]..           
-00005ae0: 2073 656c 662e 7072 696f 725f 6462 5f70   self.prior_db_p
-00005af0: 706d 2020 2020 203d 205b 7574 696c 5f78  pm     = [util_x
-00005b00: 6d6c 2e42 4f4f 4c45 414e 535b 7661 6c2e  ml.BOOLEANS[val.
-00005b10: 7465 7874 5d20 666f 7220 7661 6c20 696e  text] for val in
-00005b20: 2073 6f75 7263 652e 6765 7469 7465 7261   source.getitera
-00005b30: 746f 7228 2270 7269 6f72 5f64 625f 7070  tor("prior_db_pp
-00005b40: 6d22 295d 0d0a 2020 2020 2020 2020 2020  m")]..          
-00005b50: 2020 7365 6c66 2e70 7269 6f72 5f66 6978    self.prior_fix
-00005b60: 5f74 3220 2020 2020 3d20 5b66 6c6f 6174  _t2     = [float
-00005b70: 2876 616c 2e74 6578 7429 2066 6f72 2076  (val.text) for v
-00005b80: 616c 2069 6e20 736f 7572 6365 2e67 6574  al in source.get
-00005b90: 6974 6572 6174 6f72 2822 7072 696f 725f  iterator("prior_
-00005ba0: 6669 785f 7432 2229 5d0d 0a20 2020 2020  fix_t2")]..     
-00005bb0: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
-00005bc0: 725f 7365 6172 6368 5f70 6830 203d 205b  r_search_ph0 = [
-00005bd0: 666c 6f61 7428 7661 6c2e 7465 7874 2920  float(val.text) 
-00005be0: 666f 7220 7661 6c20 696e 2073 6f75 7263  for val in sourc
-00005bf0: 652e 6765 7469 7465 7261 746f 7228 2270  e.getiterator("p
-00005c00: 7269 6f72 5f73 6561 7263 685f 7068 3022  rior_search_ph0"
-00005c10: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00005c20: 0d0a 2020 2020 2020 2020 2020 2020 6e6d  ..            nm
-00005c30: 6574 203d 206c 656e 2873 656c 662e 7072  et = len(self.pr
-00005c40: 696f 725f 6c69 7374 290d 0a20 2020 2020  ior_list)..     
-00005c50: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00005c60: 6c66 2e70 7269 6f72 5f61 7265 615f 7363  lf.prior_area_sc
-00005c70: 616c 653a 0d0a 2020 2020 2020 2020 2020  ale:..          
-00005c80: 2020 2020 2020 7365 6c66 2e70 7269 6f72        self.prior
-00005c90: 5f61 7265 615f 7363 616c 6520 3d20 5b31  _area_scale = [1
-00005ca0: 2e30 2066 6f72 2069 2069 6e20 7261 6e67  .0 for i in rang
-00005cb0: 6528 6e6d 6574 295d 0d0a 2020 2020 2020  e(nmet)]..      
-00005cc0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00005cd0: 662e 7072 696f 725f 7365 6172 6368 5f70  f.prior_search_p
-00005ce0: 706d 3a0d 0a20 2020 2020 2020 2020 2020  pm:..           
-00005cf0: 2020 2020 2073 656c 662e 7072 696f 725f       self.prior_
-00005d00: 7365 6172 6368 5f70 706d 203d 205b 302e  search_ppm = [0.
-00005d10: 3120 666f 7220 6920 696e 2072 616e 6765  1 for i in range
-00005d20: 286e 6d65 7429 5d0d 0a20 2020 2020 2020  (nmet)]..       
-00005d30: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00005d40: 2e70 7269 6f72 5f64 625f 7070 6d3a 0d0a  .prior_db_ppm:..
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 7365 6c66 2e70 7269 6f72 5f64 625f 7070  self.prior_db_pp
-00005d70: 6d20 3d20 5b46 616c 7365 2066 6f72 2069  m = [False for i
-00005d80: 2069 6e20 7261 6e67 6528 6e6d 6574 295d   in range(nmet)]
-00005d90: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00005da0: 206e 6f74 2073 656c 662e 7072 696f 725f   not self.prior_
-00005db0: 6669 785f 7432 3a0d 0a20 2020 2020 2020  fix_t2:..       
-00005dc0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00005dd0: 696f 725f 6669 785f 7432 203d 205b 3130  ior_fix_t2 = [10
-00005de0: 3030 2e30 2066 6f72 2069 2069 6e20 7261  00.0 for i in ra
-00005df0: 6e67 6528 6e6d 6574 295d 0d0a 2020 2020  nge(nmet)]..    
-00005e00: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00005e10: 656c 662e 7072 696f 725f 7365 6172 6368  elf.prior_search
-00005e20: 5f70 6830 3a0d 0a20 2020 2020 2020 2020  _ph0:..         
-00005e30: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
-00005e40: 725f 7365 6172 6368 5f70 6830 203d 205b  r_search_ph0 = [
-00005e50: 302e 3020 666f 7220 6920 696e 2072 616e  0.0 for i in ran
-00005e60: 6765 286e 6d65 7429 5d0d 0a0d 0a20 2020  ge(nmet)]....   
-00005e70: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00005e80: 696f 725f 7872 616e 6765 2020 2020 203d  ior_xrange     =
-00005e90: 205b 696e 7428 7661 6c2e 7465 7874 2920   [int(val.text) 
-00005ea0: 666f 7220 7661 6c20 696e 2073 6f75 7263  for val in sourc
-00005eb0: 652e 6765 7469 7465 7261 746f 7228 2270  e.getiterator("p
-00005ec0: 7269 6f72 5f78 7261 6e67 6522 295d 0d0a  rior_xrange")]..
-00005ed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005ee0: 2e70 7269 6f72 5f79 7261 6e67 6520 2020  .prior_yrange   
-00005ef0: 2020 3d20 5b69 6e74 2876 616c 2e74 6578    = [int(val.tex
-00005f00: 7429 2066 6f72 2076 616c 2069 6e20 736f  t) for val in so
-00005f10: 7572 6365 2e67 6574 6974 6572 6174 6f72  urce.getiterator
-00005f20: 2822 7072 696f 725f 7972 616e 6765 2229  ("prior_yrange")
-00005f30: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-00005f40: 656c 662e 7072 696f 725f 7a72 616e 6765  elf.prior_zrange
-00005f50: 2020 2020 203d 205b 696e 7428 7661 6c2e       = [int(val.
-00005f60: 7465 7874 2920 666f 7220 7661 6c20 696e  text) for val in
-00005f70: 2073 6f75 7263 652e 6765 7469 7465 7261   source.getitera
-00005f80: 746f 7228 2270 7269 6f72 5f7a 7261 6e67  tor("prior_zrang
-00005f90: 6522 295d 0d0a 2020 2020 2020 2020 2020  e")]..          
-00005fa0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00005fb0: 2320 7375 626f 626a 6563 7473 0d0a 2020  # subobjects..  
-00005fc0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00005fd0: 7269 6f72 203d 206d 7273 5f70 7269 6f72  rior = mrs_prior
-00005fe0: 2e50 7269 6f72 2873 6f75 7263 652e 6669  .Prior(source.fi
-00005ff0: 6e64 2822 7072 696f 7222 2929 0d0a 2020  nd("prior"))..  
-00006000: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00006010: 2020 2020 2020 656c 6966 2068 6173 6174        elif hasat
-00006020: 7472 2873 6f75 7263 652c 2022 6b65 7973  tr(source, "keys
-00006030: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00006040: 2023 2051 7561 636b 7320 6c69 6b65 2061   # Quacks like a
-00006050: 2064 6963 740d 0a20 2020 2020 2020 2020   dict..         
-00006060: 2020 2066 6f72 206b 6579 2069 6e20 6c69     for key in li
-00006070: 7374 2873 6f75 7263 652e 6b65 7973 2829  st(source.keys()
-00006080: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00006090: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
-000060a0: 656c 662c 206b 6579 293a 0d0a 2020 2020  elf, key):..    
-000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060c0: 7365 7461 7474 7228 7365 6c66 2c20 6b65  setattr(self, ke
-000060d0: 792c 2073 6f75 7263 655b 6b65 795d 290d  y, source[key]).
-000060e0: 0a0d 0a0d 0a0d 0a0d 0a63 6c61 7373 2042  .........class B
-000060f0: 6c6f 636b 4669 7447 6973 6f28 626c 6f63  lockFitGiso(bloc
-00006100: 6b5f 6669 745f 6964 656e 7469 7479 2e42  k_fit_identity.B
-00006110: 6c6f 636b 4669 7449 6465 6e74 6974 7929  lockFitIdentity)
-00006120: 3a0d 0a20 2020 2022 2222 200d 0a20 2020  :..    """ ..   
-00006130: 2042 7569 6c64 696e 6720 626c 6f63 6b20   Building block 
-00006140: 746f 2068 6f6c 6420 7468 6520 7374 6174  to hold the stat
-00006150: 6520 6f66 2061 2073 7465 7020 696e 2061  e of a step in a
-00006160: 6e20 4d52 5320 7072 6f63 6573 7369 6e67  n MRS processing
-00006170: 2063 6861 696e 2e0d 0a20 2020 2049 6e63   chain...    Inc
-00006180: 6c75 6465 7320 7468 6520 6675 6e63 7469  ludes the functi
-00006190: 6f6e 616c 6974 7920 746f 2073 6176 652f  onality to save/
-000061a0: 7265 6361 6c6c 2074 6869 7320 6f62 6a65  recall this obje
-000061b0: 6374 2074 6f2f 6672 6f6d 2061 6e20 584d  ct to/from an XM
-000061c0: 4c20 6e6f 6465 2e0d 0a0d 0a20 2020 2043  L node.....    C
-000061d0: 6f6e 7461 696e 7320 696e 7075 7473 2f72  ontains inputs/r
-000061e0: 6573 756c 7473 2066 6f72 2063 6f6e 7665  esults for conve
-000061f0: 7274 696e 6720 7468 6520 6669 7474 6564  rting the fitted
-00006200: 206d 6574 6162 6f6c 6974 6520 6172 6561   metabolite area
-00006210: 7320 746f 200d 0a20 2020 2063 6f6e 6365  s to ..    conce
-00006220: 6e74 7261 7469 6f6e 2076 616c 7565 732e  ntration values.
-00006230: 0d0a 2020 2020 0d0a 2020 2020 2222 220d  ..    ..    """.
-00006240: 0a20 2020 2058 4d4c 5f56 4552 5349 4f4e  .    XML_VERSION
-00006250: 203d 2022 312e 302e 3022 0d0a 2020 2020   = "1.0.0"..    
-00006260: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00006270: 5f5f 2873 656c 662c 2061 7474 7269 6275  __(self, attribu
-00006280: 7465 733d 4e6f 6e65 293a 0d0a 2020 2020  tes=None):..    
-00006290: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
-000062a0: 2020 2047 656e 6572 616c 2050 6172 616d     General Param
-000062b0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-000062c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000062d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000062e0: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 2020 2020  --------....    
-000062f0: 2020 2020 6964 2020 2020 2020 2020 2020      id          
-00006300: 4120 7065 726d 616e 656e 742c 2075 6e69  A permanent, uni
-00006310: 7175 6520 6964 656e 7469 6679 696e 6720  que identifying 
-00006320: 7374 7269 6e67 2066 6f72 2074 6869 7320  string for this 
-00006330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006340: 2020 2020 2020 6f62 6a65 6374 2e20 5479        object. Ty
-00006350: 7069 6361 6c6c 7920 7365 7276 6573 2061  pically serves a
-00006360: 7320 6120 2273 6f75 7263 655f 6964 2220  s a "source_id" 
-00006370: 666f 7220 0d0a 2020 2020 2020 2020 2020  for ..          
-00006380: 2020 2020 2020 2020 2020 736f 6d65 206f            some o
-00006390: 7468 6572 206f 626a 6563 742e 2049 7420  ther object. It 
-000063a0: 6973 2070 6172 7420 6f66 2074 6865 2070  is part of the p
-000063b0: 726f 7665 6e61 6e63 650d 0a20 2020 2020  rovenance..     
-000063c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000063d0: 6f72 2074 6869 7320 7072 6f63 6573 7369  or this processi
-000063e0: 6e67 2066 756e 6374 6f72 2063 6861 696e  ng functor chain
-000063f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006400: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-00006410: 6f75 7263 655f 6964 2020 2054 6865 2075  ource_id   The u
-00006420: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
-00006430: 2075 7365 6420 746f 2066 696e 6420 7468   used to find th
-00006440: 6520 696e 7075 7420 6461 7461 0d0a 2020  e input data..  
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 666f 7220 7468 6973 206f 626a 6563    for this objec
-00006470: 742e 2049 7420 6d61 7920 7265 6665 7220  t. It may refer 
-00006480: 746f 206f 6e65 2077 686f 6c65 206f 626a  to one whole obj
-00006490: 6563 740d 0a20 2020 2020 2020 2020 2020  ect..           
-000064a0: 2020 2020 2020 2020 2074 6861 7420 6861           that ha
-000064b0: 7320 6f6e 6c79 206f 6e65 2072 6573 756c  s only one resul
-000064c0: 742c 204f 5220 6974 2063 6f75 6c64 2072  t, OR it could r
-000064d0: 6566 6572 2074 6f20 730d 0a20 2020 2020  efer to s..     
-000064e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000064f0: 696e 676c 6520 7265 7375 6c74 7320 696e  ingle results in
-00006500: 7369 6465 2061 6e20 6f62 6a65 6374 2074  side an object t
-00006510: 6861 7420 6861 7320 6d75 6c74 6970 6c65  hat has multiple
-00006520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006530: 2020 2020 2020 7265 7375 6c74 732e 0d0a        results...
-00006540: 0d0a 2020 2020 2020 2020 2222 2220 2020  ..        """   
-00006550: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-00006560: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00006570: 6174 7472 6962 7574 6573 290d 0a0d 0a20  attributes).... 
-00006580: 2020 2020 2020 2023 2d2d 2d2d 2d2d 2d2d         #--------
-00006590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000065a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000065b0: 0d0a 2020 2020 2020 2020 2320 4749 534f  ..        # GISO
-000065c0: 2061 6c67 6f72 6974 686d 2069 6e70 7574   algorithm input
-000065d0: 2073 6574 7469 6e67 730d 0a20 2020 2020   settings..     
-000065e0: 2020 2073 656c 662e 7365 7420 3d20 5f53     self.set = _S
-000065f0: 6574 7469 6e67 7328 290d 0a20 2020 2020  ettings()..     
-00006600: 2020 200d 0a20 2020 2020 2020 2023 2d2d     ..        #--
-00006610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006630: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00006640: 2320 4749 534f 2072 6573 756c 7420 6f62  # GISO result ob
-00006650: 6a65 6374 730d 0a20 2020 2020 2020 2073  jects..        s
-00006660: 656c 662e 6669 745f 7265 7375 6c74 7320  elf.fit_results 
-00006670: 2020 2020 2020 203d 204e 6f6e 6520 2020         = None   
-00006680: 2020 2023 2066 6974 2070 6172 616d 6574     # fit paramet
-00006690: 6572 7320 6672 6f6d 206f 7074 696d 697a  ers from optimiz
-000066a0: 6174 696f 6e0d 0a20 2020 2020 2020 2073  ation..        s
-000066b0: 656c 662e 6669 745f 7374 6174 7320 2020  elf.fit_stats   
-000066c0: 2020 2020 2020 203d 204e 6f6e 6520 2020         = None   
-000066d0: 2020 2023 2073 7461 7473 2066 726f 6d20     # stats from 
-000066e0: 7468 6520 6f70 7469 6d69 7a61 7469 6f6e  the optimization
-000066f0: 2066 6f72 2065 6163 6820 766f 7865 6c0d   for each voxel.
-00006700: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
-00006710: 745f 6261 7365 6c69 6e65 2020 2020 2020  t_baseline      
-00006720: 203d 204e 6f6e 6520 2020 2020 2023 2062   = None      # b
-00006730: 6173 656c 696e 6520 7265 7375 6c74 2028  aseline result (
-00006740: 6d61 7920 6265 2076 6563 746f 7220 6f72  may be vector or
-00006750: 2070 6172 616d 6574 6572 697a 6564 290d   parameterized).
-00006760: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00006770: 6e66 6964 656e 6365 2020 2020 2020 2020  nfidence        
-00006780: 203d 204e 6f6e 6520 2020 2020 2023 2063   = None      # c
-00006790: 6f6e 6669 6465 6e63 6520 6c69 6d69 7473  onfidence limits
-000067a0: 2072 6573 756c 7473 2073 746f 7261 6765   results storage
-000067b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-000067c0: 7261 6d65 725f 7261 6f20 2020 2020 2020  ramer_rao       
-000067d0: 2020 3d20 4e6f 6e65 2020 2020 2020 2320    = None      # 
-000067e0: 6372 616d 6572 2d72 616f 2062 6f75 6e64  cramer-rao bound
-000067f0: 7320 7265 7375 6c74 7320 7374 6f72 6167  s results storag
-00006800: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00006810: 696e 6974 6961 6c5f 7661 6c75 6573 2020  initial_values  
-00006820: 2020 203d 204e 6f6e 6520 2020 2020 2023     = None      #
-00006830: 2069 6e69 7469 616c 2076 616c 7565 7320   initial values 
-00006840: 666f 7220 6d65 7461 6220 6f70 7469 6d69  for metab optimi
-00006850: 7a61 7469 6f6e 2020 200d 0a20 2020 2020  zation   ..     
-00006860: 2020 2073 656c 662e 7072 696f 725f 6d61     self.prior_ma
-00006870: 736b 2020 2020 2020 2020 203d 204e 6f6e  sk         = Non
-00006880: 650d 0a0d 0a20 2020 2020 2020 2069 6620  e....        if 
-00006890: 6174 7472 6962 7574 6573 2069 7320 6e6f  attributes is no
-000068a0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000068b0: 2020 2020 2073 656c 662e 696e 666c 6174       self.inflat
-000068c0: 6528 6174 7472 6962 7574 6573 290d 0a0d  e(attributes)...
-000068d0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
-000068e0: 6169 6e20 3d20 4e6f 6e65 0d0a 0d0a 0d0a  ain = None......
-000068f0: 2020 2020 2323 2323 2320 5374 616e 6461      ##### Standa
-00006900: 7264 204d 6574 686f 6473 2061 6e64 2050  rd Methods and P
-00006910: 726f 7065 7274 6965 7320 2323 2323 2323  roperties ######
-00006920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006930: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-00006940: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00006950: 0d0a 2020 2020 6465 6620 6461 7461 2873  ..    def data(s
-00006960: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-00006970: 656c 662e 6669 745f 7265 7375 6c74 730d  elf.fit_results.
-00006980: 0a0d 0a0d 0a20 2020 2040 7072 6f70 6572  .....    @proper
-00006990: 7479 0d0a 2020 2020 6465 6620 6469 6d73  ty..    def dims
-000069a0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000069b0: 2022 2222 4469 6d65 6e73 696f 6e73 2066   """Dimensions f
-000069c0: 6f72 2066 6974 7469 6e67 2072 6573 756c  or fitting resul
-000069d0: 7473 2069 6e20 6120 6c69 7374 2c20 7265  ts in a list, re
-000069e0: 6164 206f 6e6c 792e 2222 220d 0a20 2020  ad only."""..   
-000069f0: 2020 2020 2072 6574 7572 6e20 6c69 7374       return list
-00006a00: 2873 656c 662e 6669 745f 7265 7375 6c74  (self.fit_result
-00006a10: 732e 7368 6170 6529 2069 6620 7365 6c66  s.shape) if self
-00006a20: 2e66 6974 5f72 6573 756c 7473 2069 7320  .fit_results is 
-00006a30: 6e6f 7420 4e6f 6e65 2065 6c73 6520 4e6f  not None else No
-00006a40: 6e65 0d0a 0d0a 0d0a 2020 2020 4070 726f  ne......    @pro
-00006a50: 7065 7274 790d 0a20 2020 2064 6566 206e  perty..    def n
-00006a60: 7061 7261 6d28 7365 6c66 293a 0d0a 2020  param(self):..  
-00006a70: 2020 2020 2020 6e70 6172 616d 203d 206c        nparam = l
-00006a80: 656e 2873 656c 662e 7365 742e 7072 696f  en(self.set.prio
-00006a90: 725f 6c69 7374 292a 332b 3220 2b20 7365  r_list)*3+2 + se
-00006aa0: 6c66 2e6e 6d6d 6f6c 0d0a 2020 2020 2020  lf.nmmol..      
-00006ab0: 2020 7265 7475 726e 206e 7061 7261 6d20    return nparam 
-00006ac0: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-00006ad0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00006ae0: 6465 6620 6e6d 6d6f 6c28 7365 6c66 293a  def nmmol(self):
-00006af0: 0d0a 2020 2020 2020 2020 6e6d 6d6f 6c20  ..        nmmol 
-00006b00: 3d20 300d 0a20 2020 2020 2020 2069 6620  = 0..        if 
-00006b10: 7365 6c66 2e73 6574 2e6d 6163 726f 6d6f  self.set.macromo
-00006b20: 6c5f 6d6f 6465 6c20 3d3d 2046 6974 4d61  l_model == FitMa
-00006b30: 6372 6f6d 6f6c 6563 756c 654d 6574 686f  cromoleculeMetho
-00006b40: 642e 5349 4e47 4c45 5f42 4153 4953 5f44  d.SINGLE_BASIS_D
-00006b50: 4154 4153 4554 3a0d 0a20 2020 2020 2020  ATASET:..       
-00006b60: 2020 2020 206e 6d6d 6f6c 202b 3d20 320d       nmmol += 2.
-00006b70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006b80: 6e6d 6d6f 6c0d 0a20 2020 2020 2020 200d  nmmol..        .
-00006b90: 0a0d 0a20 2020 2064 6566 205f 5f73 7472  ...    def __str
-00006ba0: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
-00006bb0: 2020 206c 696e 6573 203d 205b 5d0d 0a20     lines = [].. 
-00006bc0: 2020 2020 2020 206c 696e 6573 2e61 7070         lines.app
-00006bd0: 656e 6428 222d 2d2d 2d2d 2d2d 207b 307d  end("------- {0}
-00006be0: 204f 626a 6563 7420 2d2d 2d2d 2d2d 2d22   Object -------"
-00006bf0: 2e66 6f72 6d61 7428 7365 6c66 2e5f 5f63  .format(self.__c
-00006c00: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f29  lass__.__name__)
-00006c10: 290d 0a20 2020 2020 2020 206c 696e 6573  )..        lines
-00006c20: 2e61 7070 656e 6428 225c 6e22 290d 0a20  .append("\n").. 
-00006c30: 2020 2020 2020 206c 696e 6573 202b 3d20         lines += 
-00006c40: 5f53 6574 7469 6e67 732e 5f5f 7374 725f  _Settings.__str_
-00006c50: 5f28 7365 6c66 292e 7370 6c69 7428 275c  _(self).split('\
-00006c60: 6e27 290d 0a20 2020 2020 2020 206c 696e  n')..        lin
-00006c70: 6573 2e61 7070 656e 6428 225c 6e22 290d  es.append("\n").
-00006c80: 0a20 2020 2020 2020 206c 696e 6573 2e61  .        lines.a
-00006c90: 7070 656e 6428 222d 2d2d 2d2d 2d2d 204d  ppend("------- M
-00006ca0: 6169 6e20 4f62 6a65 6374 202d 2d2d 2d2d  ain Object -----
-00006cb0: 2d2d 2229 0d0a 2020 2020 2020 2020 6c69  --")..        li
-00006cc0: 6e65 732e 6170 7065 6e64 2822 4e6f 2061  nes.append("No a
-00006cd0: 6464 6974 696f 6e61 6c20 6461 7461 2229  dditional data")
-00006ce0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00006cf0: 206c 696e 6573 0d0a 2020 2020 2020 2020   lines..        
-00006d00: 0d0a 0d0a 2020 2020 6465 6620 6372 6561  ....    def crea
-00006d10: 7465 5f63 6861 696e 2873 656c 662c 2064  te_chain(self, d
-00006d20: 6174 6173 6574 293a 0d0a 2020 2020 2020  ataset):..      
-00006d30: 2020 7365 6c66 2e63 6861 696e 203d 2063    self.chain = c
-00006d40: 6861 696e 5f66 6974 5f67 6973 6f2e 4368  hain_fit_giso.Ch
-00006d50: 6169 6e46 6974 4769 736f 2864 6174 6173  ainFitGiso(datas
-00006d60: 6574 2c20 7365 6c66 290d 0a0d 0a0d 0a20  et, self)...... 
-00006d70: 2020 2064 6566 2073 6574 5f64 696d 7328     def set_dims(
-00006d80: 7365 6c66 2c20 6461 7461 7365 7429 3a0d  self, dataset):.
-00006d90: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00006da0: 2020 2020 2020 4769 7665 6e20 6120 4461        Given a Da
-00006db0: 7461 7365 7420 6f62 6a65 6374 2c20 7468  taset object, th
-00006dc0: 6973 2069 7320 616e 206f 7070 6f72 7475  is is an opportu
-00006dd0: 6e69 7479 2066 6f72 2074 6869 7320 626c  nity for this bl
-00006de0: 6f63 6b20 6f62 6a65 6374 200d 0a20 2020  ock object ..   
-00006df0: 2020 2020 2074 6f20 656e 7375 7265 2074       to ensure t
-00006e00: 6861 7420 6974 7320 7265 7375 6c74 7320  hat its results 
-00006e10: 6469 6d73 206d 6174 6368 2074 686f 7365  dims match those
-00006e20: 206f 6620 7468 6520 7061 7265 6e74 2064   of the parent d
-00006e30: 6174 6173 6574 2e0d 0a20 2020 2020 2020  ataset...       
-00006e40: 2042 6563 6175 7365 2074 6865 2066 6974   Because the fit
-00006e50: 7469 6e67 2072 6573 756c 7473 2061 7265  ting results are
-00006e60: 2070 6172 616d 6574 6572 732c 2074 6865   parameters, the
-00006e70: 7920 646f 206e 6f74 2068 6176 6520 746f  y do not have to
-00006e80: 206d 6174 6368 0d0a 2020 2020 2020 2020   match..        
-00006e90: 696e 2074 6865 2073 7065 6374 7261 6c20  in the spectral 
-00006ea0: 6469 6d65 6e73 696f 6e73 2c20 6a75 7374  dimensions, just
-00006eb0: 2069 6e20 7468 6520 7370 6174 6961 6c20   in the spatial 
-00006ec0: 6469 6d65 6e73 696f 6e73 2e20 4275 742c  dimensions. But,
-00006ed0: 2077 6520 0d0a 2020 2020 2020 2020 6861   we ..        ha
-00006ee0: 7665 2074 6f20 6361 6c63 756c 6174 6520  ve to calculate 
-00006ef0: 7468 6520 7061 7261 6d65 7465 7220 6469  the parameter di
-00006f00: 6d65 6e73 696f 6e20 7369 7a65 2066 726f  mension size fro
-00006f10: 6d20 6375 7272 656e 7420 7365 7474 696e  m current settin
-00006f20: 6773 0d0a 2020 2020 2020 2020 746f 2063  gs..        to c
-00006f30: 6f6d 7061 7265 2074 6f20 7468 6520 6578  ompare to the ex
-00006f40: 6973 6974 696e 6720 6172 7261 7920 6469  isiting array di
-00006f50: 6d65 6e73 696f 6e73 2e0d 0a20 2020 2020  mensions...     
-00006f60: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00006f70: 6966 2073 656c 662e 6469 6d73 2069 7320  if self.dims is 
-00006f80: 4e6f 6e65 206f 7220 7365 6c66 2e66 6974  None or self.fit
-00006f90: 5f62 6173 656c 696e 6520 6973 204e 6f6e  _baseline is Non
-00006fa0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00006fb0: 2320 6e65 6564 2074 6869 7320 6865 7265  # need this here
-00006fc0: 2066 6f72 2069 6e69 7469 616c 697a 6174   for initializat
-00006fd0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00006fe0: 2073 656c 662e 5f72 6573 6574 5f64 696d   self._reset_dim
-00006ff0: 656e 7369 6f6e 616c 5f64 6174 6128 6461  ensional_data(da
-00007000: 7461 7365 7429 0d0a 2020 2020 2020 2020  taset)..        
-00007010: 2020 2020 6966 2073 656c 662e 6368 6169      if self.chai
-00007020: 6e20 6973 206e 6f74 204e 6f6e 653a 0d0a  n is not None:..
-00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 7365 6c66 2e63 6861 696e 2e72 6573 6574  self.chain.reset
-00007050: 5f72 6573 756c 7473 5f61 7272 6179 7328  _results_arrays(
-00007060: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00007070: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-00007080: 2020 2020 2320 5072 696f 7220 6465 7065      # Prior depe
-00007090: 6e64 7320 6f6e 2073 7065 6374 7261 6c20  nds on spectral 
-000070a0: 6461 7461 2073 6574 7469 6e67 730d 0a20  data settings.. 
-000070b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000070c0: 7365 742e 7072 696f 722e 6361 6c63 756c  set.prior.calcul
-000070d0: 6174 655f 6675 6c6c 5f62 6173 6973 5f73  ate_full_basis_s
-000070e0: 6574 284e 6f6e 652c 204e 6f6e 652c 2064  et(None, None, d
-000070f0: 6174 6173 6574 290d 0a23 2020 2020 2020  ataset)..#      
-00007100: 2020 2020 2020 2073 656c 662e 7365 742e         self.set.
-00007110: 7072 696f 722e 6361 6c63 756c 6174 655f  prior.calculate_
-00007120: 6675 6c6c 5f62 6173 6973 5f73 6574 2873  full_basis_set(s
-00007130: 656c 662e 7365 742e 7072 696f 725f 7070  elf.set.prior_pp
-00007140: 6d5f 7374 6172 742c 0d0a 2320 2020 2020  m_start,..#     
-00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007180: 7365 6c66 2e73 6574 2e70 7269 6f72 5f70  self.set.prior_p
-00007190: 706d 5f65 6e64 2c20 0d0a 2320 2020 2020  pm_end, ..#     
-000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 6461 7461 7365 7429 0d0a 2020 2020 0d0a  dataset)..    ..
-000071e0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-000071f0: 2074 6865 2073 7065 6374 7261 6c2c 2073   the spectral, s
-00007200: 7061 7469 616c 206f 7220 6669 7420 7061  patial or fit pa
-00007210: 7261 6d65 7465 7220 6469 6d65 6e73 696f  rameter dimensio
-00007220: 6e73 2068 6176 6520 6368 616e 6765 642c  ns have changed,
-00007230: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00007240: 7468 656e 2073 6574 2061 2066 6c61 6720  then set a flag 
-00007250: 746f 2072 6573 6574 2072 6573 756c 7473  to reset results
-00007260: 2061 7272 6179 730d 0a20 2020 2020 2020   arrays..       
-00007270: 2020 2020 2073 7065 6374 7261 6c5f 6469       spectral_di
-00007280: 6d73 2020 3d20 6461 7461 7365 742e 7370  ms  = dataset.sp
-00007290: 6563 7472 616c 5f64 696d 730d 0a20 2020  ectral_dims..   
-000072a0: 2020 2020 2020 2020 2072 6573 756c 745f           result_
-000072b0: 6469 6d73 2020 2020 3d20 6c69 7374 2873  dims    = list(s
-000072c0: 7065 6374 7261 6c5f 6469 6d73 290d 0a20  pectral_dims).. 
-000072d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000072e0: 745f 6469 6d73 5b30 5d20 3d20 7365 6c66  t_dims[0] = self
-000072f0: 2e6e 7061 7261 6d0d 0a20 2020 2020 2020  .nparam..       
-00007300: 2020 2020 2073 7065 6374 7261 6c5f 666c       spectral_fl
-00007310: 6167 2020 3d20 7365 6c66 2e66 6974 5f62  ag  = self.fit_b
-00007320: 6173 656c 696e 652e 7368 6170 655b 305d  aseline.shape[0]
-00007330: 2021 3d20 7370 6563 7472 616c 5f64 696d   != spectral_dim
-00007340: 735b 305d 0d0a 2020 2020 2020 2020 2020  s[0]..          
-00007350: 2020 7265 7375 6c74 5f66 6c61 6720 2020    result_flag   
-00007360: 203d 2073 656c 662e 6469 6d73 2021 3d20   = self.dims != 
-00007370: 7265 7375 6c74 5f64 696d 730d 0a20 2020  result_dims..   
-00007380: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
-00007390: 6620 7370 6563 7472 616c 5f66 6c61 6720  f spectral_flag 
-000073a0: 6f72 2072 6573 756c 745f 666c 6167 3a0d  or result_flag:.
-000073b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000073c0: 2073 656c 662e 5f72 6573 6574 5f64 696d   self._reset_dim
-000073d0: 656e 7369 6f6e 616c 5f64 6174 6128 6461  ensional_data(da
-000073e0: 7461 7365 7429 0d0a 2020 2020 2020 2020  taset)..        
-000073f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007400: 6368 6169 6e20 6973 206e 6f74 204e 6f6e  chain is not Non
-00007410: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00007420: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00007430: 696e 2e72 6573 6574 5f72 6573 756c 7473  in.reset_results
-00007440: 5f61 7272 6179 7328 290d 0a0d 0a0d 0a20  _arrays()...... 
-00007450: 2020 2064 6566 2063 6865 636b 5f70 6172     def check_par
-00007460: 616d 6574 6572 5f64 696d 656e 7369 6f6e  ameter_dimension
-00007470: 7328 7365 6c66 2c20 6461 7461 7365 7429  s(self, dataset)
-00007480: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00007490: 2020 2020 2020 2020 4368 6563 6b73 2074          Checks t
-000074a0: 6865 2022 6e70 6172 616d 2220 6469 6d65  he "nparam" dime
-000074b0: 6e73 696f 6e20 696e 2074 6865 2072 6573  nsion in the res
-000074c0: 756c 7473 2074 6f20 7365 6520 6966 2074  ults to see if t
-000074d0: 6865 206e 756d 6265 7220 6f66 200d 0a20  he number of .. 
-000074e0: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
-000074f0: 7320 696e 2074 6865 206d 6f64 656c 2068  s in the model h
-00007500: 6173 2063 6861 6e67 6564 2e20 4f6e 6c79  as changed. Only
-00007510: 2072 6573 6574 7320 7265 7375 6c74 7320   resets results 
-00007520: 6966 2074 6869 730d 0a20 2020 2020 2020  if this..       
-00007530: 2064 696d 656e 7369 6f6e 2068 6173 2063   dimension has c
-00007540: 6861 6e67 6564 2e0d 0a20 2020 2020 2020  hanged...       
-00007550: 200d 0a20 2020 2020 2020 2022 2222 0d0a   ..        """..
-00007560: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007570: 6669 745f 7265 7375 6c74 732e 7368 6170  fit_results.shap
-00007580: 655b 305d 2021 3d20 7365 6c66 2e6e 7061  e[0] != self.npa
-00007590: 7261 6d3a 0d0a 2020 2020 2020 2020 2020  ram:..          
-000075a0: 2020 7365 6c66 2e5f 7265 7365 745f 6469    self._reset_di
-000075b0: 6d65 6e73 696f 6e61 6c5f 6461 7461 2864  mensional_data(d
-000075c0: 6174 6173 6574 290d 0a0d 0a0d 0a20 2020  ataset)......   
-000075d0: 2064 6566 205f 7265 7365 745f 6469 6d65   def _reset_dime
-000075e0: 6e73 696f 6e61 6c5f 6461 7461 2873 656c  nsional_data(sel
-000075f0: 662c 2064 6174 6173 6574 293a 0d0a 2020  f, dataset):..  
-00007600: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00007610: 2020 2052 6573 6574 7320 2874 6f20 7a65     Resets (to ze
-00007620: 726f 2920 616e 6420 7265 7369 7a65 7320  ro) and resizes 
-00007630: 6469 6d65 6e73 696f 6e61 6c6c 792d 6465  dimensionally-de
-00007640: 7065 6e64 656e 7420 6461 7461 0d0a 2020  pendent data..  
-00007650: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00007660: 6669 745f 7265 7375 6c74 7320 2020 2020  fit_results     
-00007670: 2d20 6669 7420 7061 7261 6d65 7465 7273  - fit parameters
-00007680: 2066 726f 6d20 6f70 7469 6d69 7a61 7469   from optimizati
-00007690: 6f6e 0d0a 2020 2020 2020 2020 6669 745f  on..        fit_
-000076a0: 7374 6174 7320 2020 2020 2020 2d20 6f70  stats       - op
-000076b0: 7469 6d69 7a61 7469 6f6e 2063 6869 7371  timization chisq
-000076c0: 722c 2077 7463 6869 7371 7220 616e 6420  r, wtchisqr and 
-000076d0: 6669 6e69 7465 6d61 7468 2076 616c 7565  finitemath value
-000076e0: 730d 0a20 2020 2020 2020 2066 6974 5f62  s..        fit_b
-000076f0: 6173 656c 696e 6520 2020 202d 2062 6173  aseline    - bas
-00007700: 656c 696e 6520 7265 7375 6c74 2028 6d61  eline result (ma
-00007710: 7920 6265 2076 6563 746f 7220 6f72 2070  y be vector or p
-00007720: 6172 616d 6574 6572 697a 6564 290d 0a20  arameterized).. 
-00007730: 2020 2020 2020 2063 6f6e 6669 6465 6e63         confidenc
-00007740: 6520 2020 2020 202d 2063 6f6e 6669 6465  e      - confide
-00007750: 6e63 6520 6c69 6d69 7473 2072 6573 756c  nce limits resul
-00007760: 7473 2073 746f 7261 6765 0d0a 2020 2020  ts storage..    
-00007770: 2020 2020 6372 616d 6572 5f72 616f 2020      cramer_rao  
-00007780: 2020 2020 2d20 6372 616d 6572 2d72 616f      - cramer-rao
-00007790: 2062 6f75 6e64 7320 7265 7375 6c74 7320   bounds results 
-000077a0: 7374 6f72 6167 650d 0a20 2020 2020 2020  storage..       
-000077b0: 2069 6e69 7469 616c 5f76 616c 7565 7320   initial_values 
-000077c0: 202d 2069 6e69 7469 616c 2076 616c 7565   - initial value
-000077d0: 7320 666f 7220 6d65 7461 6220 6f70 7469  s for metab opti
-000077e0: 6d69 7a61 7469 6f6e 0d0a 2020 2020 2020  mization..      
-000077f0: 2020 7072 696f 725f 6d61 736b 2020 2020    prior_mask    
-00007800: 2020 2d20 7370 6174 6961 6c20 2878 2c79    - spatial (x,y
-00007810: 2c7a 2920 6d61 736b 2074 6f20 696e 6469  ,z) mask to indi
-00007820: 6361 7465 2077 6861 7420 766f 7865 6c73  cate what voxels
-00007830: 2074 6f20 6669 740d 0a20 2020 2020 2020   to fit..       
-00007840: 200d 0a20 2020 2020 2020 204e 6f74 652e   ..        Note.
-00007850: 2042 3020 7368 6966 7420 6973 2061 6363   B0 shift is acc
-00007860: 6f75 6e74 6564 2066 6f72 2069 6e20 5370  ounted for in Sp
-00007870: 6563 7472 616c 206f 626a 6563 742f 7461  ectral object/ta
-00007880: 6273 0d0a 2020 2020 2020 2020 0d0a 2020  bs..        ..  
-00007890: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000078a0: 2020 2064 696d 7320 3d20 6461 7461 7365     dims = datase
-000078b0: 742e 7370 6563 7472 616c 5f64 696d 730d  t.spectral_dims.
-000078c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000078d0: 2020 206e 7061 7261 6d20 3d20 7365 6c66     nparam = self
-000078e0: 2e6e 7061 7261 6d20 2020 2020 2020 200d  .nparam        .
-000078f0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00007900: 2020 2069 6620 7365 6c66 2e66 6974 5f72     if self.fit_r
-00007910: 6573 756c 7473 2069 7320 4e6f 6e65 3a0d  esults is None:.
-00007920: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00007930: 2020 2020 2020 2073 656c 662e 6669 745f         self.fit_
-00007940: 7265 7375 6c74 7320 2020 203d 206e 702e  results    = np.
-00007950: 7a65 726f 7328 286e 7061 7261 6d2c 2064  zeros((nparam, d
-00007960: 696d 735b 315d 2c20 6469 6d73 5b32 5d2c  ims[1], dims[2],
-00007970: 2064 696d 735b 335d 2929 2020 2020 2020   dims[3]))      
-00007980: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007990: 6c66 2e66 6974 5f73 7461 7473 2020 2020  lf.fit_stats    
-000079a0: 2020 3d20 6e70 2e7a 6572 6f73 2828 332c    = np.zeros((3,
-000079b0: 2064 696d 735b 315d 2c20 6469 6d73 5b32   dims[1], dims[2
-000079c0: 5d2c 2064 696d 735b 335d 2929 2020 2020  ], dims[3]))    
-000079d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000079e0: 7365 6c66 2e66 6974 5f62 6173 656c 696e  self.fit_baselin
-000079f0: 6520 2020 3d20 6e70 2e7a 6572 6f73 2874  e   = np.zeros(t
-00007a00: 7570 6c65 2864 6174 6173 6574 2e73 7065  uple(dataset.spe
-00007a10: 6374 7261 6c5f 6469 6d73 292c 2064 7479  ctral_dims), dty
-00007a20: 7065 3d27 636f 6d70 6c65 7836 3427 290d  pe='complex64').
-00007a30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007a40: 662e 636f 6e66 6964 656e 6365 2020 2020  f.confidence    
-00007a50: 203d 206e 702e 7a65 726f 7328 286e 7061   = np.zeros((npa
-00007a60: 7261 6d2c 2064 696d 735b 315d 2c20 6469  ram, dims[1], di
-00007a70: 6d73 5b32 5d2c 2064 696d 735b 335d 2929  ms[2], dims[3]))
-00007a80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00007a90: 2020 2020 7365 6c66 2e63 7261 6d65 725f      self.cramer_
-00007aa0: 7261 6f20 2020 2020 3d20 6e70 2e7a 6572  rao     = np.zer
-00007ab0: 6f73 2828 6e70 6172 616d 2c20 6469 6d73  os((nparam, dims
-00007ac0: 5b31 5d2c 2064 696d 735b 325d 2c20 6469  [1], dims[2], di
-00007ad0: 6d73 5b33 5d29 2920 2020 2020 200d 0a20  ms[3]))      .. 
-00007ae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007af0: 696e 6974 6961 6c5f 7661 6c75 6573 203d  initial_values =
-00007b00: 206e 702e 7a65 726f 7328 286e 7061 7261   np.zeros((npara
-00007b10: 6d2c 2064 696d 735b 315d 2c20 6469 6d73  m, dims[1], dims
-00007b20: 5b32 5d2c 2064 696d 735b 335d 2929 2020  [2], dims[3]))  
-00007b30: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00007b40: 2020 7365 6c66 2e70 7269 6f72 5f6d 6173    self.prior_mas
-00007b50: 6b20 2020 2020 3d20 6e70 2e6f 6e65 7328  k     = np.ones(
-00007b60: 2864 696d 735b 315d 2c20 6469 6d73 5b32  (dims[1], dims[2
-00007b70: 5d2c 2064 696d 735b 335d 2929 200d 0a20  ], dims[3])) .. 
-00007b80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00007b90: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00007ba0: 2020 2020 7061 7261 6d5f 6469 6d73 203d      param_dims =
-00007bb0: 206c 6973 7428 6469 6d73 290d 0a20 2020   list(dims)..   
-00007bc0: 2020 2020 2020 2020 2070 6172 616d 5f64           param_d
-00007bd0: 696d 735b 305d 203d 206e 7061 7261 6d0d  ims[0] = nparam.
-00007be0: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00007bf0: 206d 6169 6e74 6169 6e20 7265 7375 6c74   maintain result
-00007c00: 7320 6966 206e 6f20 6469 6d65 6e73 696f  s if no dimensio
-00007c10: 6e20 6861 7320 6368 616e 6765 640d 0a20  n has changed.. 
-00007c20: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007c30: 6c66 2e66 6974 5f62 6173 656c 696e 652e  lf.fit_baseline.
-00007c40: 7368 6170 655b 3a3a 2d31 5d20 213d 2064  shape[::-1] != d
-00007c50: 696d 7320 6f72 205c 0d0a 2020 2020 2020  ims or \..      
-00007c60: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00007c70: 6974 5f72 6573 756c 7473 2e73 6861 7065  it_results.shape
-00007c80: 5b3a 3a2d 315d 2021 3d20 7061 7261 6d5f  [::-1] != param_
-00007c90: 6469 6d73 3a0d 0a20 2020 2020 2020 2020  dims:..         
-00007ca0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00007cb0: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-00007cc0: 745f 6261 7365 6c69 6e65 2020 203d 206e  t_baseline   = n
-00007cd0: 702e 7a65 726f 7328 7475 706c 6528 6469  p.zeros(tuple(di
-00007ce0: 6d73 292c 2064 7479 7065 3d27 636f 6d70  ms), dtype='comp
-00007cf0: 6c65 7836 3427 2920 2020 2020 2020 200d  lex64')        .
-00007d00: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00007d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007d20: 6669 745f 7265 7375 6c74 7320 2020 203d  fit_results    =
-00007d30: 206e 702e 7a65 726f 7328 286e 7061 7261   np.zeros((npara
-00007d40: 6d2c 2064 696d 735b 315d 2c20 6469 6d73  m, dims[1], dims
-00007d50: 5b32 5d2c 2064 696d 735b 335d 2929 2020  [2], dims[3]))  
-00007d60: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00007d70: 2020 2020 2020 7365 6c66 2e66 6974 5f73        self.fit_s
-00007d80: 7461 7473 2020 2020 2020 3d20 6e70 2e7a  tats      = np.z
-00007d90: 6572 6f73 2828 332c 2064 696d 735b 315d  eros((3, dims[1]
-00007da0: 2c20 6469 6d73 5b32 5d2c 2064 696d 735b  , dims[2], dims[
-00007db0: 335d 2929 2020 2020 2020 0d0a 2020 2020  3]))      ..    
-00007dc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007dd0: 2e66 6974 5f62 6173 656c 696e 6520 2020  .fit_baseline   
-00007de0: 3d20 6e70 2e7a 6572 6f73 2874 7570 6c65  = np.zeros(tuple
-00007df0: 2864 6174 6173 6574 2e73 7065 6374 7261  (dataset.spectra
-00007e00: 6c5f 6469 6d73 292c 2064 7479 7065 3d27  l_dims), dtype='
-00007e10: 636f 6d70 6c65 7836 3427 290d 0a20 2020  complex64')..   
-00007e20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007e30: 662e 636f 6e66 6964 656e 6365 2020 2020  f.confidence    
-00007e40: 203d 206e 702e 7a65 726f 7328 286e 7061   = np.zeros((npa
-00007e50: 7261 6d2c 2064 696d 735b 315d 2c20 6469  ram, dims[1], di
-00007e60: 6d73 5b32 5d2c 2064 696d 735b 335d 2929  ms[2], dims[3]))
-00007e70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00007e80: 2020 2020 2020 2020 7365 6c66 2e63 7261          self.cra
-00007e90: 6d65 725f 7261 6f20 2020 2020 3d20 6e70  mer_rao     = np
-00007ea0: 2e7a 6572 6f73 2828 6e70 6172 616d 2c20  .zeros((nparam, 
-00007eb0: 6469 6d73 5b31 5d2c 2064 696d 735b 325d  dims[1], dims[2]
-00007ec0: 2c20 6469 6d73 5b33 5d29 2920 2020 2020  , dims[3]))     
-00007ed0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00007ee0: 2020 2073 656c 662e 696e 6974 6961 6c5f     self.initial_
-00007ef0: 7661 6c75 6573 203d 206e 702e 7a65 726f  values = np.zero
-00007f00: 7328 286e 7061 7261 6d2c 2064 696d 735b  s((nparam, dims[
-00007f10: 315d 2c20 6469 6d73 5b32 5d2c 2064 696d  1], dims[2], dim
-00007f20: 735b 335d 2929 2020 2020 2020 0d0a 2020  s[3]))      ..  
-00007f30: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00007f40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007f50: 2e70 7269 6f72 5f6d 6173 6b20 2020 2020  .prior_mask     
-00007f60: 3d20 6e70 2e6f 6e65 7328 2864 696d 735b  = np.ones((dims[
-00007f70: 315d 2c20 6469 6d73 5b32 5d2c 2064 696d  1], dims[2], dim
-00007f80: 735b 335d 2929 200d 0a0d 0a0d 0a20 2020  s[3])) ......   
-00007f90: 2064 6566 2067 6574 5f66 6974 7465 645f   def get_fitted_
-00007fa0: 7761 7465 725f 6172 6561 2873 656c 6629  water_area(self)
-00007fb0: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-00007fc0: 2020 2020 2066 6c61 675f 7761 7465 7220       flag_water 
-00007fd0: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-00007fe0: 2066 6f72 2069 6e64 782c 2069 7465 6d20   for indx, item 
-00007ff0: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
-00008000: 662e 7365 742e 7072 696f 725f 6c69 7374  f.set.prior_list
-00008010: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00008020: 6966 2027 7761 7465 7227 2069 6e20 6974  if 'water' in it
-00008030: 656d 2e6c 6f77 6572 2829 206f 7220 2768  em.lower() or 'h
-00008040: 326f 2720 696e 2069 7465 6d2e 6c6f 7765  2o' in item.lowe
-00008050: 7228 293a 0d0a 2020 2020 2020 2020 2020  r():..          
-00008060: 2020 2020 2020 666c 6167 5f77 6174 6572        flag_water
-00008070: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-00008080: 2020 2020 2020 2020 2069 6e64 785f 7761           indx_wa
-00008090: 7465 7220 3d20 696e 6478 0d0a 2020 2020  ter = indx..    
-000080a0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000080b0: 6b0d 0a20 2020 2020 2020 200d 0a20 2020  k..        ..   
-000080c0: 2020 2020 2069 6620 6e6f 7420 666c 6167       if not flag
-000080d0: 5f77 6174 6572 3a0d 0a20 2020 2020 2020  _water:..       
-000080e0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-000080f0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00008100: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
-00008110: 7320 3d20 7365 6c66 2e66 6974 5f72 6573  s = self.fit_res
-00008120: 756c 7473 2e73 6861 7065 0d0a 2020 2020  ults.shape..    
-00008130: 2020 2020 2020 2020 7265 7320 203d 2073          res  = s
-00008140: 656c 662e 6669 745f 7265 7375 6c74 735b  elf.fit_results[
-00008150: 696e 6478 5f77 6174 6572 2c3a 2c3a 2c3a  indx_water,:,:,:
-00008160: 5d0d 0a20 2020 2020 2020 2020 2020 2072  ]..            r
-00008170: 6573 2020 3d20 7265 732e 636f 7079 2829  es  = res.copy()
-00008180: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
-00008190: 6620 6469 6d73 5b31 5d20 2a20 6469 6d73  f dims[1] * dims
-000081a0: 5b32 5d20 2a20 6469 6d73 5b33 5d20 3d3d  [2] * dims[3] ==
-000081b0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-000081c0: 2020 2020 2072 6573 2e73 6861 7065 203d       res.shape =
-000081d0: 2031 2c31 2c31 2c31 0d0a 2020 2020 2020   1,1,1,1..      
-000081e0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000081f0: 2020 2320 7265 7475 726e 2077 6174 6572    # return water
-00008200: 2061 7265 6173 0d0a 0d0a 0d0a 2020 2020   areas......    
-00008210: 6465 6620 6765 745f 6173 736f 6369 6174  def get_associat
-00008220: 6564 5f64 6174 6173 6574 7328 7365 6c66  ed_datasets(self
-00008230: 2c20 6973 5f6d 6169 6e5f 6461 7461 7365  , is_main_datase
-00008240: 743d 5472 7565 293a 0d0a 2020 2020 2020  t=True):..      
-00008250: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
-00008260: 6574 7572 6e73 2061 206c 6973 7420 6f66  eturns a list of
-00008270: 2064 6174 6173 6574 7320 6173 736f 6369   datasets associ
-00008280: 6174 6564 2077 6974 6820 7468 6973 206f  ated with this o
-00008290: 626a 6563 740d 0a0d 0a20 2020 2020 2020  bject....       
-000082a0: 2027 6973 5f6d 6169 6e5f 6461 7461 7365   'is_main_datase
-000082b0: 7427 2073 6967 6e61 6c73 2074 6861 7420  t' signals that 
-000082c0: 7468 6973 2069 7320 7468 6520 746f 7020  this is the top 
-000082d0: 6c65 7665 6c20 6461 7461 7365 7420 6761  level dataset ga
-000082e0: 7468 6572 696e 6720 0d0a 2020 2020 2020  thering ..      
-000082f0: 2020 6173 736f 6369 6174 6564 2064 6174    associated dat
-00008300: 6173 6574 732c 2061 6e64 2069 7320 7573  asets, and is us
-00008310: 6564 2074 6f20 7374 6f70 2063 6972 6375  ed to stop circu
-00008320: 6c61 7220 7265 6665 7265 6e63 6573 0d0a  lar references..
-00008330: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00008340: 2020 2020 2020 2064 6174 6173 6574 7320         datasets 
-00008350: 3d20 626c 6f63 6b5f 6669 745f 6964 656e  = block_fit_iden
-00008360: 7469 7479 2e42 6c6f 636b 4669 7449 6465  tity.BlockFitIde
-00008370: 6e74 6974 792e 6765 745f 6173 736f 6369  ntity.get_associ
-00008380: 6174 6564 5f64 6174 6173 6574 7328 7365  ated_datasets(se
-00008390: 6c66 2c20 6973 5f6d 6169 6e5f 6461 7461  lf, is_main_data
-000083a0: 7365 7429 0d0a 0d0a 2020 2020 2020 2020  set)....        
-000083b0: 6966 2069 735f 6d61 696e 5f64 6174 6173  if is_main_datas
-000083c0: 6574 3a0d 0a20 2020 2020 2020 2020 2020  et:..           
-000083d0: 2023 2061 7420 7468 6973 2070 6f69 6e74   # at this point
-000083e0: 2c20 6f6e 6c79 2061 206d 6163 726f 6d6f  , only a macromo
-000083f0: 6c65 6375 6c65 206d 6f64 656c 206d 6179  lecule model may
-00008400: 206e 6565 6420 616e 2061 7373 6f63 6961   need an associa
-00008410: 7465 6420 6461 7461 7365 740d 0a20 2020  ted dataset..   
-00008420: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00008430: 2e73 6574 2e6d 6163 726f 6d6f 6c5f 7369  .set.macromol_si
-00008440: 6e67 6c65 5f62 6173 6973 5f64 6174 6173  ngle_basis_datas
-00008450: 6574 3a0d 0a20 2020 2020 2020 2020 2020  et:..           
-00008460: 2020 2020 2064 6174 6173 6574 7320 2b3d       datasets +=
-00008470: 2073 656c 662e 7365 742e 6d61 6372 6f6d   self.set.macrom
-00008480: 6f6c 5f73 696e 676c 655f 6261 7369 735f  ol_single_basis_
-00008490: 6461 7461 7365 742e 6765 745f 6173 736f  dataset.get_asso
-000084a0: 6369 6174 6564 5f64 6174 6173 6574 7328  ciated_datasets(
-000084b0: 6973 5f6d 6169 6e5f 6461 7461 7365 743d  is_main_dataset=
-000084c0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
-000084d0: 2020 2020 2020 2020 6461 7461 7365 7473          datasets
-000084e0: 202b 3d20 5b73 656c 662e 7365 742e 6d61   += [self.set.ma
-000084f0: 6372 6f6d 6f6c 5f73 696e 676c 655f 6261  cromol_single_ba
-00008500: 7369 735f 6461 7461 7365 745d 0d0a 0d0a  sis_dataset]....
-00008510: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00008520: 6174 6173 6574 730d 0a0d 0a0d 0a20 2020  atasets......   
-00008530: 2064 6566 2073 6574 5f61 7373 6f63 6961   def set_associa
-00008540: 7465 645f 6461 7461 7365 7473 2873 656c  ted_datasets(sel
-00008550: 662c 2064 6174 6173 6574 7329 3a20 0d0a  f, datasets): ..
-00008560: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00008570: 2020 2020 2057 6865 6e20 7765 206f 7065       When we ope
-00008580: 6e20 6120 5649 4646 2066 6f72 6d61 7420  n a VIFF format 
-00008590: 6669 6c65 2c20 6d61 696e 2e5f 696d 706f  file, main._impo
-000085a0: 7274 5f66 696c 6528 2920 6361 6c6c 7320  rt_file() calls 
-000085b0: 7468 6973 206d 6574 686f 640d 0a20 2020  this method..   
-000085c0: 2020 2020 2074 6f20 7061 7273 652f 7374       to parse/st
-000085d0: 6f72 6520 616e 7920 6461 7461 7365 7473  ore any datasets
-000085e0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000085f0: 2074 6869 7320 6f6e 6520 6173 2064 6573   this one as des
-00008600: 6372 6962 6564 2062 656c 6f77 2e0d 0a20  cribed below... 
-00008610: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00008620: 2022 2222 0d0a 2020 2020 2020 2020 666f   """..        fo
-00008630: 7220 6461 7461 7365 7420 696e 2064 6174  r dataset in dat
-00008640: 6173 6574 733a 0d0a 2020 2020 2020 2020  asets:..        
-00008650: 2020 2020 6966 2064 6174 6173 6574 2e69      if dataset.i
-00008660: 6420 3d3d 2073 656c 662e 7365 742e 6d61  d == self.set.ma
-00008670: 6372 6f6d 6f6c 5f73 696e 676c 655f 6261  cromol_single_ba
-00008680: 7369 735f 6461 7461 7365 745f 6964 3a0d  sis_dataset_id:.
-00008690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000086a0: 2073 656c 662e 7365 742e 6d61 6372 6f6d   self.set.macrom
-000086b0: 6f6c 5f73 696e 676c 655f 6261 7369 735f  ol_single_basis_
-000086c0: 6461 7461 7365 7420 3d20 6461 7461 7365  dataset = datase
-000086d0: 740d 0a0d 0a0d 0a20 2020 2064 6566 2064  t......    def d
-000086e0: 6566 6c61 7465 2873 656c 662c 2066 6c61  eflate(self, fla
-000086f0: 766f 723d 4465 666c 6174 652e 4554 5245  vor=Deflate.ETRE
-00008700: 4529 3a0d 0a20 2020 2020 2020 2069 6620  E):..        if 
-00008710: 666c 6176 6f72 203d 3d20 4465 666c 6174  flavor == Deflat
-00008720: 652e 4554 5245 453a 0d0a 2020 2020 2020  e.ETREE:..      
-00008730: 2020 2020 2020 6520 3d20 456c 656d 656e        e = Elemen
-00008740: 7428 2262 6c6f 636b 5f66 6974 5f67 6973  t("block_fit_gis
-00008750: 6f22 2c20 7b20 2269 6422 203a 2073 656c  o", { "id" : sel
-00008760: 662e 6964 2c0d 0a20 2020 2020 2020 2020  f.id,..         
-00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008790: 2020 2022 7665 7273 696f 6e22 203a 2073     "version" : s
-000087a0: 656c 662e 584d 4c5f 5645 5253 494f 4e7d  elf.XML_VERSION}
-000087b0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-000087c0: 0a20 2020 2020 2020 2020 2020 2075 7469  .            uti
-000087d0: 6c5f 786d 6c2e 5465 7874 5375 6245 6c65  l_xml.TextSubEle
-000087e0: 6d65 6e74 2865 2c20 2262 6568 6176 655f  ment(e, "behave_
-000087f0: 6173 5f70 7265 7365 7422 2c20 7365 6c66  as_preset", self
-00008800: 2e62 6568 6176 655f 6173 5f70 7265 7365  .behave_as_prese
-00008810: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-00008820: 0d0a 2020 2020 2020 2020 2020 2020 652e  ..            e.
-00008830: 6170 7065 6e64 2873 656c 662e 7365 742e  append(self.set.
-00008840: 6465 666c 6174 6528 2929 0d0a 0d0a 2020  deflate())....  
-00008850: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00008860: 2073 656c 662e 6265 6861 7665 5f61 735f   self.behave_as_
-00008870: 7072 6573 6574 3a0d 0a20 2020 2020 2020  preset:..       
-00008880: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00008890: 2020 2020 2020 2066 6f72 2064 696d 2069         for dim i
-000088a0: 6e20 7365 6c66 2e64 696d 733a 0d0a 2020  n self.dims:..  
-000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 2020 7574 696c 5f78 6d6c 2e54 6578 7453    util_xml.TextS
-000088d0: 7562 456c 656d 656e 7428 652c 2022 6469  ubElement(e, "di
-000088e0: 6d22 2c20 6469 6d29 0d0a 0d0a 2020 2020  m", dim)....    
-000088f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00008900: 656c 662e 6669 745f 7265 7375 6c74 7320  elf.fit_results 
-00008910: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 652e 6170 7065 6e64 2875 7469 6c5f    e.append(util_
-00008940: 786d 6c2e 6e75 6d70 795f 6172 7261 795f  xml.numpy_array_
-00008950: 746f 5f65 6c65 6d65 6e74 2873 656c 662e  to_element(self.
-00008960: 6669 745f 7265 7375 6c74 732c 2766 6974  fit_results,'fit
-00008970: 5f72 6573 756c 7473 2729 290d 0a20 2020  _results'))..   
-00008980: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00008990: 7365 6c66 2e66 6974 5f73 7461 7473 2069  self.fit_stats i
-000089a0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 2065 2e61 7070 656e 6428 7574 696c 5f78   e.append(util_x
-000089d0: 6d6c 2e6e 756d 7079 5f61 7272 6179 5f74  ml.numpy_array_t
-000089e0: 6f5f 656c 656d 656e 7428 7365 6c66 2e66  o_element(self.f
-000089f0: 6974 5f73 7461 7473 2c27 6669 745f 7374  it_stats,'fit_st
-00008a00: 6174 7327 2929 0d0a 2020 2020 2020 2020  ats'))..        
-00008a10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008a20: 6669 745f 6261 7365 6c69 6e65 2069 7320  fit_baseline is 
-00008a30: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00008a40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00008a50: 2e61 7070 656e 6428 7574 696c 5f78 6d6c  .append(util_xml
-00008a60: 2e6e 756d 7079 5f61 7272 6179 5f74 6f5f  .numpy_array_to_
-00008a70: 656c 656d 656e 7428 7365 6c66 2e66 6974  element(self.fit
-00008a80: 5f62 6173 656c 696e 652c 2766 6974 5f62  _baseline,'fit_b
-00008a90: 6173 656c 696e 6527 2929 0d0a 2020 2020  aseline'))..    
-00008aa0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00008ab0: 656c 662e 636f 6e66 6964 656e 6365 2069  elf.confidence i
-00008ac0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 2065 2e61 7070 656e 6428 7574 696c 5f78   e.append(util_x
-00008af0: 6d6c 2e6e 756d 7079 5f61 7272 6179 5f74  ml.numpy_array_t
-00008b00: 6f5f 656c 656d 656e 7428 7365 6c66 2e63  o_element(self.c
-00008b10: 6f6e 6669 6465 6e63 652c 2763 6f6e 6669  onfidence,'confi
-00008b20: 6465 6e63 6527 2929 0d0a 2020 2020 2020  dence'))..      
-00008b30: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00008b40: 662e 6372 616d 6572 5f72 616f 2069 7320  f.cramer_rao is 
-00008b50: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00008b60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00008b70: 2e61 7070 656e 6428 7574 696c 5f78 6d6c  .append(util_xml
-00008b80: 2e6e 756d 7079 5f61 7272 6179 5f74 6f5f  .numpy_array_to_
-00008b90: 656c 656d 656e 7428 7365 6c66 2e63 7261  element(self.cra
-00008ba0: 6d65 725f 7261 6f2c 2763 7261 6d65 725f  mer_rao,'cramer_
-00008bb0: 7261 6f27 2929 0d0a 2020 2020 2020 2020  rao'))..        
-00008bc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008bd0: 696e 6974 6961 6c5f 7661 6c75 6573 2069  initial_values i
-00008be0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c00: 2065 2e61 7070 656e 6428 7574 696c 5f78   e.append(util_x
-00008c10: 6d6c 2e6e 756d 7079 5f61 7272 6179 5f74  ml.numpy_array_t
-00008c20: 6f5f 656c 656d 656e 7428 7365 6c66 2e69  o_element(self.i
-00008c30: 6e69 7469 616c 5f76 616c 7565 732c 2769  nitial_values,'i
-00008c40: 6e69 7469 616c 5f76 616c 7565 7327 2929  nitial_values'))
-00008c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008c60: 2020 6966 2073 656c 662e 7072 696f 725f    if self.prior_
-00008c70: 6d61 736b 2069 7320 6e6f 7420 4e6f 6e65  mask is not None
-00008c80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00008c90: 2020 2020 2020 2065 2e61 7070 656e 6428         e.append(
-00008ca0: 7574 696c 5f78 6d6c 2e6e 756d 7079 5f61  util_xml.numpy_a
-00008cb0: 7272 6179 5f74 6f5f 656c 656d 656e 7428  rray_to_element(
-00008cc0: 7365 6c66 2e70 7269 6f72 5f6d 6173 6b2c  self.prior_mask,
-00008cd0: 2770 7269 6f72 5f6d 6173 6b27 2929 0d0a  'prior_mask'))..
-00008ce0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00008cf0: 7475 726e 2065 0d0a 2020 2020 2020 2020  turn e..        
-00008d00: 2020 2020 0d0a 2020 2020 2020 2020 656c      ..        el
-00008d10: 6966 2066 6c61 766f 7220 3d3d 2044 6566  if flavor == Def
-00008d20: 6c61 7465 2e44 4943 5449 4f4e 4152 593a  late.DICTIONARY:
-00008d30: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00008d40: 7475 726e 2073 656c 662e 5f5f 6469 6374  turn self.__dict
-00008d50: 5f5f 2e63 6f70 7928 290d 0a0d 0a0d 0a20  __.copy()...... 
-00008d60: 2020 2064 6566 2069 6e66 6c61 7465 2873     def inflate(s
-00008d70: 656c 662c 2073 6f75 7263 6529 3a0d 0a20  elf, source):.. 
-00008d80: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-00008d90: 7228 736f 7572 6365 2c20 226d 616b 6565  r(source, "makee
-00008da0: 6c65 6d65 6e74 2229 3a0d 0a20 2020 2020  lement"):..     
-00008db0: 2020 2020 2020 2023 2051 7561 636b 7320         # Quacks 
-00008dc0: 6c69 6b65 2061 6e20 456c 656d 656e 7454  like an ElementT
-00008dd0: 7265 652e 456c 656d 656e 740d 0a0d 0a20  ree.Element.... 
-00008de0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008df0: 6964 203d 2073 6f75 7263 652e 6765 7428  id = source.get(
-00008e00: 2269 6422 290d 0a0d 0a20 2020 2020 2020  "id")....       
-00008e10: 2020 2020 2076 616c 203d 2073 6f75 7263       val = sourc
-00008e20: 652e 6669 6e64 7465 7874 2822 6265 6861  e.findtext("beha
-00008e30: 7665 5f61 735f 7072 6573 6574 2229 2020  ve_as_preset")  
-00008e40: 2023 2064 6566 6175 6c74 2069 7320 4661   # default is Fa
-00008e50: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00008e60: 2069 6620 7661 6c20 6973 206e 6f74 204e   if val is not N
-00008e70: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00008e80: 2020 2020 2020 7365 6c66 2e62 6568 6176        self.behav
-00008e90: 655f 6173 5f70 7265 7365 7420 3d20 7574  e_as_preset = ut
-00008ea0: 696c 5f78 6d6c 2e42 4f4f 4c45 414e 535b  il_xml.BOOLEANS[
-00008eb0: 7661 6c5d 0d0a 0d0a 2020 2020 2020 2020  val]....        
-00008ec0: 2020 2020 2320 4c6f 6f6b 2066 6f72 2073      # Look for s
-00008ed0: 6574 7469 6e67 7320 756e 6465 7220 7468  ettings under th
-00008ee0: 6520 6f6c 6420 6e61 6d65 2061 7320 7765  e old name as we
-00008ef0: 6c6c 2061 7320 7468 6520 7374 616e 6461  ll as the standa
-00008f00: 7264 206e 616d 652e 0d0a 2020 2020 2020  rd name...      
-00008f10: 2020 2020 2020 7365 6c66 2e73 6574 203d        self.set =
-00008f20: 2075 7469 6c5f 786d 6c2e 6669 6e64 5f73   util_xml.find_s
-00008f30: 6574 7469 6e67 7328 736f 7572 6365 2c20  ettings(source, 
-00008f40: 2262 6c6f 636b 5f67 6973 6f5f 7365 7474  "block_giso_sett
-00008f50: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
-00008f60: 2020 2020 7365 6c66 2e73 6574 203d 205f      self.set = _
-00008f70: 5365 7474 696e 6773 2873 656c 662e 7365  Settings(self.se
-00008f80: 7429 0d0a 0d0a 2020 2020 2020 2020 2020  t)....          
-00008f90: 2020 6966 206e 6f74 2073 656c 662e 6265    if not self.be
-00008fa0: 6861 7665 5f61 735f 7072 6573 6574 3a0d  have_as_preset:.
-00008fb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00008fc0: 2020 2023 2045 7870 6c69 6369 7420 7465     # Explicit te
-00008fd0: 7374 7320 666f 7220 4e6f 6e65 206e 6563  sts for None nec
-00008fe0: 6573 7361 7279 2069 6e20 7468 6520 636f  essary in the co
-00008ff0: 6465 2062 656c 6f77 2e20 0d0a 2020 2020  de below. ..    
-00009000: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00009010: 203d 2073 6f75 7263 652e 6669 6e64 2822   = source.find("
-00009020: 6669 745f 7265 7375 6c74 7322 290d 0a20  fit_results").. 
-00009030: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009040: 6620 7465 6d70 2069 7320 6e6f 7420 4e6f  f temp is not No
-00009050: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00009060: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-00009070: 745f 7265 7375 6c74 7320 3d20 7574 696c  t_results = util
-00009080: 5f78 6d6c 2e65 6c65 6d65 6e74 5f74 6f5f  _xml.element_to_
-00009090: 6e75 6d70 795f 6172 7261 7928 7465 6d70  numpy_array(temp
-000090a0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000090b0: 2020 2020 2074 656d 7020 3d20 736f 7572       temp = sour
-000090c0: 6365 2e66 696e 6428 2266 6974 5f73 7461  ce.find("fit_sta
-000090d0: 7473 2229 0d0a 2020 2020 2020 2020 2020  ts")..          
-000090e0: 2020 2020 2020 6966 2074 656d 7020 6973        if temp is
-000090f0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 7365 6c66 2e66 6974 5f73 7461 7473 203d  self.fit_stats =
-00009120: 2075 7469 6c5f 786d 6c2e 656c 656d 656e   util_xml.elemen
-00009130: 745f 746f 5f6e 756d 7079 5f61 7272 6179  t_to_numpy_array
-00009140: 2874 656d 7029 0d0a 0d0a 2020 2020 2020  (temp)....      
-00009150: 2020 2020 2020 2020 2020 7465 6d70 203d            temp =
-00009160: 2073 6f75 7263 652e 6669 6e64 2822 6669   source.find("fi
-00009170: 745f 6261 7365 6c69 6e65 2229 0d0a 2020  t_baseline")..  
-00009180: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00009190: 2074 656d 7020 6973 206e 6f74 204e 6f6e   temp is not Non
-000091a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000091b0: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
-000091c0: 5f62 6173 656c 696e 6520 3d20 7574 696c  _baseline = util
-000091d0: 5f78 6d6c 2e65 6c65 6d65 6e74 5f74 6f5f  _xml.element_to_
-000091e0: 6e75 6d70 795f 6172 7261 7928 7465 6d70  numpy_array(temp
-000091f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00009200: 2020 2020 2074 656d 7020 3d20 736f 7572       temp = sour
-00009210: 6365 2e66 696e 6428 2263 6f6e 6669 6465  ce.find("confide
-00009220: 6e63 6522 290d 0a20 2020 2020 2020 2020  nce")..         
-00009230: 2020 2020 2020 2069 6620 7465 6d70 2069         if temp i
-00009240: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009260: 2073 656c 662e 636f 6e66 6964 656e 6365   self.confidence
-00009270: 203d 2075 7469 6c5f 786d 6c2e 656c 656d   = util_xml.elem
-00009280: 656e 745f 746f 5f6e 756d 7079 5f61 7272  ent_to_numpy_arr
-00009290: 6179 2874 656d 7029 0d0a 0d0a 2020 2020  ay(temp)....    
-000092a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000092b0: 203d 2073 6f75 7263 652e 6669 6e64 2822   = source.find("
-000092c0: 6372 616d 6572 5f72 616f 2229 0d0a 2020  cramer_rao")..  
-000092d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000092e0: 2074 656d 7020 6973 206e 6f74 204e 6f6e   temp is not Non
-000092f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00009300: 2020 2020 2020 2020 7365 6c66 2e63 7261          self.cra
-00009310: 6d65 725f 7261 6f20 3d20 7574 696c 5f78  mer_rao = util_x
-00009320: 6d6c 2e65 6c65 6d65 6e74 5f74 6f5f 6e75  ml.element_to_nu
-00009330: 6d70 795f 6172 7261 7928 7465 6d70 290d  mpy_array(temp).
-00009340: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00009350: 2020 2074 656d 7020 3d20 736f 7572 6365     temp = source
-00009360: 2e66 696e 6428 2269 6e69 7469 616c 5f76  .find("initial_v
-00009370: 616c 7565 7322 290d 0a20 2020 2020 2020  alues")..       
-00009380: 2020 2020 2020 2020 2069 6620 7465 6d70           if temp
-00009390: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-000093a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093b0: 2020 2073 656c 662e 696e 6974 6961 6c5f     self.initial_
-000093c0: 7661 6c75 6573 203d 2075 7469 6c5f 786d  values = util_xm
-000093d0: 6c2e 656c 656d 656e 745f 746f 5f6e 756d  l.element_to_num
-000093e0: 7079 5f61 7272 6179 2874 656d 7029 0d0a  py_array(temp)..
-000093f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009400: 2020 7465 6d70 203d 2073 6f75 7263 652e    temp = source.
-00009410: 6669 6e64 2822 7072 696f 725f 6d61 736b  find("prior_mask
-00009420: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00009430: 2020 2020 6966 2074 656d 7020 6973 206e      if temp is n
-00009440: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00009450: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009460: 6c66 2e70 7269 6f72 5f6d 6173 6b20 3d20  lf.prior_mask = 
-00009470: 7574 696c 5f78 6d6c 2e65 6c65 6d65 6e74  util_xml.element
-00009480: 5f74 6f5f 6e75 6d70 795f 6172 7261 7928  _to_numpy_array(
-00009490: 7465 6d70 290d 0a0d 0a0d 0a20 2020 2020  temp)......     
-000094a0: 2020 2065 6c69 6620 6861 7361 7474 7228     elif hasattr(
-000094b0: 736f 7572 6365 2c20 226b 6579 7322 293a  source, "keys"):
-000094c0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000094d0: 5175 6163 6b73 206c 696b 6520 6120 6469  Quacks like a di
-000094e0: 6374 0d0a 2020 2020 2020 2020 2020 2020  ct..            
-000094f0: 666f 7220 6b65 7920 696e 206c 6973 7428  for key in list(
-00009500: 736f 7572 6365 2e6b 6579 7328 2929 3a0d  source.keys()):.
-00009510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009520: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
-00009530: 2c20 6b65 7929 3a0d 0a20 2020 2020 2020  , key):..       
-00009540: 2020 2020 2020 2020 2020 2020 2073 6574               set
-00009550: 6174 7472 2873 656c 662c 206b 6579 2c20  attr(self, key, 
-00009560: 736f 7572 6365 5b6b 6579 5d29 0d0a 0d0a  source[key])....
-00009570: 0d0a 2020 2020 6465 6620 7265 7375 6c74  ..    def result
-00009580: 735f 6173 5f68 746d 6c28 7365 6c66 2c20  s_as_html(self, 
-00009590: 766f 7865 6c2c 206c 773d 302e 302c 206c  voxel, lw=0.0, l
-000095a0: 776d 696e 3d30 2e30 2c20 6c77 6d61 783d  wmin=0.0, lwmax=
-000095b0: 302e 302c 200d 0a20 2020 2020 2020 2020  0.0, ..         
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000095d0: 6174 615f 736f 7572 6365 3d22 222c 2069  ata_source="", i
-000095e0: 6d61 6765 3d4e 6f6e 6529 3a0d 0a20 2020  mage=None):..   
-000095f0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00009600: 2020 4769 7665 6e20 6120 766f 7865 6c2c    Given a voxel,
-00009610: 206c 696e 6577 6964 7468 2070 6172 616d   linewidth param
-00009620: 732c 2061 6e64 2061 2064 6174 6120 736f  s, and a data so
-00009630: 7572 6365 2028 6f66 7465 6e20 6120 6669  urce (often a fi
-00009640: 6c65 6e61 6d65 292c 200d 0a20 2020 2020  lename), ..     
-00009650: 2020 2072 6574 7572 6e73 2048 544d 4c2d     returns HTML-
-00009660: 666f 726d 6174 7465 6420 7265 7375 6c74  formatted result
-00009670: 7320 666f 7220 7468 6174 2076 6f78 656c  s for that voxel
-00009680: 2e20 5468 6520 4854 4d4c 2069 7320 6170  . The HTML is ap
-00009690: 7072 6f70 7269 6174 6520 0d0a 2020 2020  propriate ..    
-000096a0: 2020 2020 666f 7220 7468 6520 7778 2e48      for the wx.H
-000096b0: 746d 6c20 636f 6e74 726f 6c20 2877 6869  tml control (whi
-000096c0: 6368 2075 6e64 6572 7374 616e 6420 6c69  ch understand li
-000096d0: 6d69 7465 6420 4854 4d4c 2920 6173 2077  mited HTML) as w
-000096e0: 656c 6c20 6173 2066 6f72 0d0a 2020 2020  ell as for..    
-000096f0: 2020 2020 7772 6974 696e 6720 746f 2061      writing to a
-00009700: 2066 696c 652e 0d0a 0d0a 2020 2020 2020   file.....      
-00009710: 2020 4966 2074 6865 2069 6d61 6765 2070    If the image p
-00009720: 6172 616d 2069 7320 706f 7075 6c61 7465  aram is populate
-00009730: 642c 2069 7420 7368 6f75 6c64 2062 6520  d, it should be 
-00009740: 6120 7475 706c 6520 6f66 200d 0a20 2020  a tuple of ..   
-00009750: 2020 2020 2028 6d69 6d65 5f74 7970 652c       (mime_type,
-00009760: 2069 6d61 6765 5f64 6174 6129 2e20 5468   image_data). Th
-00009770: 6520 666f 726d 6572 2073 686f 756c 6420  e former should 
-00009780: 6265 2061 2073 7472 696e 6720 6c69 6b65  be a string like
-00009790: 2022 696d 6167 652f 706e 6722 2e0d 0a20   "image/png"... 
-000097a0: 2020 2020 2020 2054 6865 206c 6174 7465         The latte
-000097b0: 7220 7368 6f75 6c64 2062 6520 6261 7365  r should be base
-000097c0: 3634 2d65 6e63 6f64 6564 2069 6d61 6765  64-encoded image
-000097d0: 2064 6174 612e 0d0a 2020 2020 2020 2020   data...        
-000097e0: 2222 220d 0a20 2020 2020 2020 2023 2046  """..        # F
-000097f0: 6972 7374 2077 6520 6173 7365 6d62 6c65  irst we assemble
-00009800: 2074 6865 2064 6174 6120 7765 206e 6565   the data we nee
-00009810: 642e 0d0a 2020 2020 2020 2020 6e6d 6574  d...        nmet
-00009820: 203d 206c 656e 2873 656c 662e 7365 742e   = len(self.set.
-00009830: 7072 696f 725f 6c69 7374 290d 0a20 2020  prior_list)..   
-00009840: 2020 2020 200d 0a20 2020 2020 2020 206e       ..        n
-00009850: 616d 6573 203d 2073 656c 662e 7365 742e  ames = self.set.
-00009860: 7072 696f 725f 6c69 7374 0d0a 2020 2020  prior_list..    
-00009870: 2020 2020 7265 7320 2020 3d20 7365 6c66      res   = self
-00009880: 2e66 6974 5f72 6573 756c 7473 5b3a 2c76  .fit_results[:,v
-00009890: 6f78 656c 5b30 5d2c 766f 7865 6c5b 315d  oxel[0],voxel[1]
-000098a0: 2c76 6f78 656c 5b32 5d5d 0d0a 2020 2020  ,voxel[2]]..    
-000098b0: 2020 2020 6372 616f 2020 3d20 7365 6c66      crao  = self
-000098c0: 2e63 7261 6d65 725f 7261 6f5b 3a2c 766f  .cramer_rao[:,vo
-000098d0: 7865 6c5b 305d 2c76 6f78 656c 5b31 5d2c  xel[0],voxel[1],
-000098e0: 766f 7865 6c5b 325d 5d0d 0a20 2020 2020  voxel[2]]..     
-000098f0: 2020 2063 6f6e 6620 203d 2073 656c 662e     conf  = self.
-00009900: 636f 6e66 6964 656e 6365 5b3a 2c76 6f78  confidence[:,vox
-00009910: 656c 5b30 5d2c 766f 7865 6c5b 315d 2c76  el[0],voxel[1],v
-00009920: 6f78 656c 5b32 5d5d 0d0a 2020 2020 2020  oxel[2]]..      
-00009930: 2020 7374 6174 7320 3d20 7365 6c66 2e66    stats = self.f
-00009940: 6974 5f73 7461 7473 5b3a 2c76 6f78 656c  it_stats[:,voxel
-00009950: 5b30 5d2c 766f 7865 6c5b 315d 2c76 6f78  [0],voxel[1],vox
-00009960: 656c 5b32 5d5d 0d0a 2020 2020 2020 2020  el[2]]..        
-00009970: 2320 626f 7468 2063 7261 6d65 722d 7261  # both cramer-ra
-00009980: 6f20 616e 6420 636f 6e66 6964 656e 6365  o and confidence
-00009990: 2069 6e74 6572 7661 6c73 206d 6179 2062   intervals may b
-000099a0: 6520 6f66 662f 6f6e 0d0a 2020 2020 2020  e off/on..      
-000099b0: 2020 6966 206c 656e 2863 7261 6f29 2021    if len(crao) !
-000099c0: 3d20 6c65 6e28 7265 7329 3a0d 0a20 2020  = len(res):..   
-000099d0: 2020 2020 2020 2020 2063 7261 6f20 3d20           crao = 
-000099e0: 7265 7320 2a20 300d 0a20 2020 2020 2020  res * 0..       
-000099f0: 2069 6620 6c65 6e28 636f 6e66 2920 213d   if len(conf) !=
-00009a00: 206c 656e 2872 6573 293a 0d0a 2020 2020   len(res):..    
-00009a10: 2020 2020 2020 2020 636f 6e66 203d 2072          conf = r
-00009a20: 6573 202a 2030 0d0a 0d0a 2020 2020 2020  es * 0....      
-00009a30: 2020 7461 626c 6531 203d 205b 5b27 4172    table1 = [['Ar
-00009a40: 6561 2052 6573 756c 7473 272c 2027 4172  ea Results', 'Ar
-00009a50: 6561 272c 2027 2043 7252 616f 5b25 5d27  ea', ' CrRao[%]'
-00009a60: 2c20 2720 436e 6649 6e74 5b25 5d27 5d5d  , ' CnfInt[%]']]
-00009a70: 0d0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-00009a80: 2069 7465 6d20 696e 2065 6e75 6d65 7261   item in enumera
-00009a90: 7465 286e 616d 6573 293a 0d0a 2020 2020  te(names):..    
-00009aa0: 2020 2020 2020 2020 7461 626c 6531 2e61          table1.a
-00009ab0: 7070 656e 6428 5b69 7465 6d2c 2072 6573  ppend([item, res
-00009ac0: 5b69 5d2c 2063 7261 6f5b 695d 2c20 636f  [i], crao[i], co
-00009ad0: 6e66 5b69 5d5d 290d 0a0d 0a20 2020 2020  nf[i]])....     
-00009ae0: 2020 2069 6620 7365 6c66 2e73 6574 2e6d     if self.set.m
-00009af0: 6163 726f 6d6f 6c5f 6d6f 6465 6c20 3d3d  acromol_model ==
-00009b00: 2046 6974 4d61 6372 6f6d 6f6c 6563 756c   FitMacromolecul
-00009b10: 654d 6574 686f 642e 5349 4e47 4c45 5f42  eMethod.SINGLE_B
-00009b20: 4153 4953 5f44 4154 4153 4554 3a0d 0a20  ASIS_DATASET:.. 
-00009b30: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00009b40: 312e 6170 7065 6e64 285b 274d 4d6f 6c27  1.append(['MMol'
-00009b50: 2c20 7265 735b 6e6d 6574 2a33 2b32 5d2c  , res[nmet*3+2],
-00009b60: 2030 2e30 2c20 302e 305d 290d 0a20 2020   0.0, 0.0])..   
-00009b70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00009b80: 2020 2074 6162 6c65 3120 3d20 5f70 7265     table1 = _pre
-00009b90: 7474 795f 7370 6163 655f 7461 626c 6528  tty_space_table(
-00009ba0: 7461 626c 6531 2c20 706c 6163 6573 3d34  table1, places=4
-00009bb0: 290d 0a0d 0a20 2020 2020 2020 2074 6162  )....        tab
-00009bc0: 6c65 3220 3d20 5b5b 2750 504d 2052 6573  le2 = [['PPM Res
-00009bd0: 756c 7473 272c 2027 5050 4d27 2c20 2720  ults', 'PPM', ' 
-00009be0: 4372 5261 6f5b 7070 6d5d 272c 2027 2043  CrRao[ppm]', ' C
-00009bf0: 6e66 496e 745b 7070 6d5d 275d 5d0d 0a20  nfInt[ppm]']].. 
-00009c00: 2020 2020 2020 2066 6f72 2069 2c69 7465         for i,ite
-00009c10: 6d20 696e 2065 6e75 6d65 7261 7465 286e  m in enumerate(n
-00009c20: 616d 6573 293a 0d0a 2020 2020 2020 2020  ames):..        
-00009c30: 2020 2020 7461 626c 6532 2e61 7070 656e      table2.appen
-00009c40: 6428 5b69 7465 6d2c 2072 6573 5b69 2b6e  d([item, res[i+n
-00009c50: 6d65 745d 2c20 6372 616f 5b69 2b6e 6d65  met], crao[i+nme
-00009c60: 745d 2c20 636f 6e66 5b69 2b6e 6d65 745d  t], conf[i+nmet]
-00009c70: 5d29 0d0a 0d0a 2020 2020 2020 2020 6966  ])....        if
-00009c80: 2073 656c 662e 7365 742e 6d61 6372 6f6d   self.set.macrom
-00009c90: 6f6c 5f6d 6f64 656c 203d 3d20 4669 744d  ol_model == FitM
-00009ca0: 6163 726f 6d6f 6c65 6375 6c65 4d65 7468  acromoleculeMeth
-00009cb0: 6f64 2e53 494e 474c 455f 4241 5349 535f  od.SINGLE_BASIS_
-00009cc0: 4441 5441 5345 543a 0d0a 2020 2020 2020  DATASET:..      
-00009cd0: 2020 2020 2020 7461 626c 6532 2e61 7070        table2.app
-00009ce0: 656e 6428 5b27 4d4d 6f6c 272c 2072 6573  end(['MMol', res
-00009cf0: 5b6e 6d65 742a 332b 335d 2c20 302e 302c  [nmet*3+3], 0.0,
-00009d00: 2030 2e30 5d29 0d0a 0d0a 2020 2020 2020   0.0])....      
-00009d10: 2020 7461 626c 6532 203d 205f 7072 6574    table2 = _pret
-00009d20: 7479 5f73 7061 6365 5f74 6162 6c65 2874  ty_space_table(t
-00009d30: 6162 6c65 322c 2070 6c61 6365 733d 3429  able2, places=4)
-00009d40: 0d0a 0d0a 2020 2020 2020 2020 7461 626c  ....        tabl
-00009d50: 6532 6120 3d20 5b5b 2754 6220 5265 7375  e2a = [['Tb Resu
-00009d60: 6c74 7327 2c20 2754 625b 7365 635d 272c  lts', 'Tb[sec]',
-00009d70: 2027 4c57 5b48 7a5d 272c 2027 4372 5261   'LW[Hz]', 'CrRa
-00009d80: 6f5b 7365 635d 272c 2027 2043 6e66 496e  o[sec]', ' CnfIn
-00009d90: 745b 7365 635d 275d 5d0d 0a20 2020 2020  t[sec]']]..     
-00009da0: 2020 2066 6f72 2069 2c69 7465 6d20 696e     for i,item in
-00009db0: 2065 6e75 6d65 7261 7465 286e 616d 6573   enumerate(names
-00009dc0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00009dd0: 7461 626c 6532 612e 6170 7065 6e64 285b  table2a.append([
-00009de0: 6974 656d 2c20 7265 735b 692b 6e6d 6574  item, res[i+nmet
-00009df0: 2a32 5d2c 206c 775b 695d 2c20 6372 616f  *2], lw[i], crao
-00009e00: 5b69 2b6e 6d65 742a 325d 2c20 636f 6e66  [i+nmet*2], conf
-00009e10: 5b69 2b6e 6d65 742a 325d 5d29 0d0a 0d0a  [i+nmet*2]])....
-00009e20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009e30: 7365 742e 6d61 6372 6f6d 6f6c 5f6d 6f64  set.macromol_mod
-00009e40: 656c 203d 3d20 4669 744d 6163 726f 6d6f  el == FitMacromo
-00009e50: 6c65 6375 6c65 4d65 7468 6f64 2e53 494e  leculeMethod.SIN
-00009e60: 474c 455f 4241 5349 535f 4441 5441 5345  GLE_BASIS_DATASE
-00009e70: 543a 0d0a 2020 2020 2020 2020 2020 2020  T:..            
-00009e80: 7461 626c 6532 612e 6170 7065 6e64 285b  table2a.append([
-00009e90: 274d 4d6f 6c27 2c20 7265 735b 6e6d 6574  'MMol', res[nmet
-00009ea0: 2a33 2b34 5d2c 2030 2e30 2c20 302e 305d  *3+4], 0.0, 0.0]
-00009eb0: 290d 0a0d 0a20 2020 2020 2020 2074 6162  )....        tab
-00009ec0: 6c65 3261 203d 205f 7072 6574 7479 5f73  le2a = _pretty_s
-00009ed0: 7061 6365 5f74 6162 6c65 2874 6162 6c65  pace_table(table
-00009ee0: 3261 2c20 706c 6163 6573 3d34 290d 0a0d  2a, places=4)...
-00009ef0: 0a20 2020 2020 2020 2074 6162 6c65 3320  .        table3 
-00009f00: 3d20 2020 2020 5b5b 2747 6c6f 6261 6c20  =     [['Global 
-00009f10: 5265 7375 6c74 7327 2c20 2756 616c 7565  Results', 'Value
-00009f20: 272c 2027 2043 7252 616f 5b64 656c 7461  ', ' CrRao[delta
-00009f30: 5d27 2c20 2720 436e 6649 6e74 5b25 5d27  ]', ' CnfInt[%]'
-00009f40: 5d5d 0d0a 2020 2020 2020 2020 7461 626c  ]]..        tabl
-00009f50: 6533 2e61 7070 656e 6428 5b27 5068 6173  e3.append(['Phas
-00009f60: 6530 272c 2020 2020 2072 6573 5b6e 6d65  e0',     res[nme
-00009f70: 742a 332b 305d 2c20 6372 616f 5b6e 6d65  t*3+0], crao[nme
-00009f80: 742a 332b 305d 2c20 636f 6e66 5b6e 6d65  t*3+0], conf[nme
-00009f90: 742a 332b 305d 205d 290d 0a20 2020 2020  t*3+0] ])..     
-00009fa0: 2020 2074 6162 6c65 332e 6170 7065 6e64     table3.append
-00009fb0: 285b 2750 6861 7365 3127 2c20 2020 2020  (['Phase1',     
-00009fc0: 7265 735b 6e6d 6574 2a33 2b31 5d2c 2063  res[nmet*3+1], c
-00009fd0: 7261 6f5b 6e6d 6574 2a33 2b31 5d2c 2063  rao[nmet*3+1], c
-00009fe0: 6f6e 665b 6e6d 6574 2a33 2b31 5d20 5d29  onf[nmet*3+1] ])
-00009ff0: 0d0a 2020 2020 2020 2020 7461 626c 6533  ..        table3
-0000a000: 203d 205f 7072 6574 7479 5f73 7061 6365   = _pretty_space
-0000a010: 5f74 6162 6c65 2874 6162 6c65 332c 2070  _table(table3, p
-0000a020: 6c61 6365 733d 3529 0d0a 2020 2020 2020  laces=5)..      
-0000a030: 2020 0d0a 2020 2020 2020 2020 7461 626c    ..        tabl
-0000a040: 6534 203d 205b 5b27 4361 6c63 756c 6174  e4 = [['Calculat
-0000a050: 696f 6e20 5265 7375 6c74 7327 2c20 2720  ion Results', ' 
-0000a060: 5661 6c75 6527 2c20 2720 204d 6178 204c  Value', '  Max L
-0000a070: 5727 2c20 2720 204d 696e 204c 5727 5d5d  W', '  Min LW']]
-0000a080: 0d0a 2020 2020 2020 2020 7461 626c 6534  ..        table4
-0000a090: 2e61 7070 656e 6428 5b27 4368 6953 7175  .append(['ChiSqu
-0000a0a0: 6172 6527 2c20 7374 6174 735b 305d 2c20  are', stats[0], 
-0000a0b0: 2720 272c 2027 2027 5d29 0d0a 2020 2020  ' ', ' '])..    
-0000a0c0: 2020 2020 7461 626c 6534 2e61 7070 656e      table4.appen
-0000a0d0: 6428 5b27 5765 6967 6874 6564 2043 6869  d(['Weighted Chi
-0000a0e0: 5371 7561 7265 272c 2073 7461 7473 5b31  Square', stats[1
-0000a0f0: 5d2c 2027 2027 2c20 2720 275d 290d 0a20  ], ' ', ' ']).. 
-0000a100: 2020 2020 2020 206d 6174 6865 7272 203d         matherr =
-0000a110: 2073 7472 2873 7461 7473 5b32 5d20 213d   str(stats[2] !=
-0000a120: 2030 290d 0a20 2020 2020 2020 2074 6162   0)..        tab
-0000a130: 6c65 342e 6170 7065 6e64 285b 274d 6174  le4.append(['Mat
-0000a140: 6820 4669 6e69 7465 2045 7272 6f72 272c  h Finite Error',
-0000a150: 206d 6174 6865 7272 2c20 2720 272c 2027   matherr, ' ', '
-0000a160: 2027 5d29 0d0a 2020 2020 2020 2020 7461   '])..        ta
-0000a170: 626c 6534 203d 205f 7072 6574 7479 5f73  ble4 = _pretty_s
-0000a180: 7061 6365 5f74 6162 6c65 2874 6162 6c65  pace_table(table
-0000a190: 342c 2070 6c61 6365 733d 3529 0d0a 0d0a  4, places=5)....
-0000a1a0: 2020 2020 2020 2020 2320 4e6f 7720 7468          # Now th
-0000a1b0: 6174 2074 6865 2064 6174 6120 6973 2061  at the data is a
-0000a1c0: 7373 656d 626c 6564 2c20 7765 2048 544d  ssembled, we HTM
-0000a1d0: 4c2d 6966 7920 6974 2e0d 0a20 2020 2020  L-ify it...     
-0000a1e0: 2020 2068 746d 6c20 3d20 456c 656d 656e     html = Elemen
-0000a1f0: 7454 7265 652e 456c 656d 656e 7428 2268  tTree.Element("h
-0000a200: 746d 6c22 290d 0a20 2020 2020 2020 2068  tml")..        h
-0000a210: 6561 6420 3d20 456c 656d 656e 7454 7265  ead = ElementTre
-0000a220: 652e 5375 6245 6c65 6d65 6e74 2868 746d  e.SubElement(htm
-0000a230: 6c2c 2022 6865 6164 2229 0d0a 2020 2020  l, "head")..    
-0000a240: 2020 2020 7374 796c 6520 3d20 7574 696c      style = util
-0000a250: 5f78 6d6c 2e54 6578 7453 7562 456c 656d  _xml.TextSubElem
-0000a260: 656e 7428 6865 6164 2c20 2273 7479 6c65  ent(head, "style
-0000a270: 222c 205f 4353 5329 0d0a 2020 2020 2020  ", _CSS)..      
-0000a280: 2020 7374 796c 652e 7365 7428 2274 7970    style.set("typ
-0000a290: 6522 2c20 2274 6578 742f 6373 7322 290d  e", "text/css").
-0000a2a0: 0a0d 0a20 2020 2020 2020 2062 6f64 7920  ...        body 
-0000a2b0: 3d20 456c 656d 656e 7454 7265 652e 5375  = ElementTree.Su
-0000a2c0: 6245 6c65 6d65 6e74 2868 746d 6c2c 2022  bElement(html, "
-0000a2d0: 626f 6479 2229 0d0a 2020 2020 2020 2020  body")..        
-0000a2e0: 0d0a 2020 2020 2020 2020 7574 696c 5f78  ..        util_x
-0000a2f0: 6d6c 2e54 6578 7453 7562 456c 656d 656e  ml.TextSubElemen
-0000a300: 7428 626f 6479 2c20 2268 3222 2c20 2241  t(body, "h2", "A
-0000a310: 6e61 6c79 7369 7320 4669 742d 4769 736f  nalysis Fit-Giso
-0000a320: 2052 6573 756c 7473 2229 0d0a 0d0a 2020   Results")....  
-0000a330: 2020 2020 2020 655f 6469 7620 3d20 456c        e_div = El
-0000a340: 656d 656e 7454 7265 652e 5375 6245 6c65  ementTree.SubEle
-0000a350: 6d65 6e74 2862 6f64 792c 2022 6469 7622  ment(body, "div"
-0000a360: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-0000a370: 6461 7461 5f73 6f75 7263 653a 0d0a 2020  data_source:..  
-0000a380: 2020 2020 2020 2020 2020 655f 7474 203d            e_tt =
-0000a390: 2075 7469 6c5f 786d 6c2e 5465 7874 5375   util_xml.TextSu
-0000a3a0: 6245 6c65 6d65 6e74 2865 5f64 6976 2c20  bElement(e_div, 
-0000a3b0: 2274 7422 2c20 2244 6174 6120 536f 7572  "tt", "Data Sour
-0000a3c0: 6365 3a20 2229 0d0a 2020 2020 2020 2020  ce: ")..        
-0000a3d0: 2020 2020 7574 696c 5f78 6d6c 2e54 6578      util_xml.Tex
-0000a3e0: 7453 7562 456c 656d 656e 7428 655f 7474  tSubElement(e_tt
-0000a3f0: 2c20 2273 6d61 6c6c 222c 2064 6174 615f  , "small", data_
-0000a400: 736f 7572 6365 290d 0a20 2020 2020 2020  source)..       
-0000a410: 2020 2020 2045 6c65 6d65 6e74 5472 6565       ElementTree
-0000a420: 2e53 7562 456c 656d 656e 7428 655f 6469  .SubElement(e_di
-0000a430: 762c 2022 6272 2229 0d0a 2020 2020 2020  v, "br")..      
-0000a440: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000a450: 766f 7865 6c20 3d20 5b78 202b 2031 2066  voxel = [x + 1 f
-0000a460: 6f72 2078 2069 6e20 766f 7865 6c5d 0d0a  or x in voxel]..
-0000a470: 2020 2020 2020 2020 7574 696c 5f78 6d6c          util_xml
-0000a480: 2e54 6578 7453 7562 456c 656d 656e 7428  .TextSubElement(
-0000a490: 655f 6469 762c 2022 7474 222c 2027 566f  e_div, "tt", 'Vo
-0000a4a0: 7865 6c3a 2028 2564 2c25 642c 2564 2927  xel: (%d,%d,%d)'
-0000a4b0: 2025 2074 7570 6c65 2876 6f78 656c 2929   % tuple(voxel))
-0000a4c0: 0d0a 0d0a 2020 2020 2020 2020 6966 2069  ....        if i
-0000a4d0: 6d61 6765 3a0d 0a20 2020 2020 2020 2020  mage:..         
-0000a4e0: 2020 2023 2049 6620 7468 6572 6527 7320     # If there's 
-0000a4f0: 696d 6167 6520 6461 7461 2c20 7765 2061  image data, we a
-0000a500: 7373 756d 6520 7468 6174 2074 6869 7320  ssume that this 
-0000a510: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
-0000a520: 746f 200d 0a20 2020 2020 2020 2020 2020  to ..           
-0000a530: 2023 2061 2066 696c 6520 666f 7220 6469   # a file for di
-0000a540: 7370 6c61 7920 696e 2061 2070 726f 7065  splay in a prope
-0000a550: 7220 6272 6f77 7365 722c 2073 6f20 7765  r browser, so we
-0000a560: 2063 616e 2075 7365 2073 6c69 6768 746c   can use slightl
-0000a570: 790d 0a20 2020 2020 2020 2020 2020 2023  y..            #
-0000a580: 2066 616e 6369 6572 2048 544d 4c2e 0d0a   fancier HTML...
-0000a590: 2020 2020 2020 2020 2020 2020 6d69 6d65              mime
-0000a5a0: 5f74 7970 652c 2069 6d61 6765 5f64 6174  _type, image_dat
-0000a5b0: 6120 3d20 696d 6167 650d 0a0d 0a20 2020  a = image....   
-0000a5c0: 2020 2020 2020 2020 2065 5f64 6976 203d           e_div =
-0000a5d0: 2045 6c65 6d65 6e74 5472 6565 2e53 7562   ElementTree.Sub
-0000a5e0: 456c 656d 656e 7428 626f 6479 2c20 2264  Element(body, "d
-0000a5f0: 6976 222c 200d 0a20 2020 2020 2020 2020  iv", ..         
-0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 7b20 2269 6422 203a 2022 696d 6167    { "id" : "imag
-0000a630: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a660: 2020 2273 7479 6c65 2220 3a20 2266 6c6f    "style" : "flo
-0000a670: 6174 3a20 7269 6768 743b 2077 6964 7468  at: right; width
-0000a680: 3a20 3530 2522 2c0d 0a20 2020 2020 2020  : 50%",..       
-0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
-0000a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6e0: 2029 0d0a 0d0a 2020 2020 2020 2020 2020   )....          
-0000a6f0: 2020 655f 6469 762e 6170 7065 6e64 2845    e_div.append(E
-0000a700: 6c65 6d65 6e74 5472 6565 2e43 6f6d 6d65  lementTree.Comme
-0000a710: 6e74 285f 4945 5f49 4e43 4150 4142 4c45  nt(_IE_INCAPABLE
-0000a720: 5f4d 5347 2929 0d0a 0d0a 2020 2020 2020  _MSG))....      
-0000a730: 2020 2020 2020 2320 496e 206f 7264 6572        # In order
-0000a740: 2074 6f20 6b65 6570 2074 6865 2048 544d   to keep the HTM
-0000a750: 4c20 2b20 696d 6167 6520 696e 206f 6e65  L + image in one
-0000a760: 2066 696c 652c 2077 6520 7573 6520 7468   file, we use th
-0000a770: 650d 0a20 2020 2020 2020 2020 2020 2023  e..            #
-0000a780: 206c 6974 746c 652d 6b6e 6f77 6e20 2264   little-known "d
-0000a790: 6174 6122 2073 6368 656d 652e 0d0a 2020  ata" scheme...  
-0000a7a0: 2020 2020 2020 2020 2020 2320 7265 663a            # ref:
-0000a7b0: 2068 7474 703a 2f2f 656e 2e77 696b 6970   http://en.wikip
-0000a7c0: 6564 6961 2e6f 7267 2f77 696b 692f 4461  edia.org/wiki/Da
-0000a7d0: 7461 5f55 5249 5f73 6368 656d 650d 0a20  ta_URI_scheme.. 
-0000a7e0: 2020 2020 2020 2020 2020 2073 7263 203d             src =
-0000a7f0: 2022 6461 7461 3a25 733b 6261 7365 3634   "data:%s;base64
-0000a800: 2c25 7322 2025 2028 6d69 6d65 5f74 7970  ,%s" % (mime_typ
-0000a810: 652c 2069 6d61 6765 5f64 6174 6129 0d0a  e, image_data)..
-0000a820: 0d0a 2020 2020 2020 2020 2020 2020 456c  ..            El
-0000a830: 656d 656e 7454 7265 652e 5375 6245 6c65  ementTree.SubEle
-0000a840: 6d65 6e74 2865 5f64 6976 2c20 2269 6d67  ment(e_div, "img
-0000a850: 222c 200d 0a20 2020 2020 2020 2020 2020  ", ..           
-0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 7b22 7374 796c 6522 203a 2022 7769 6474  {"style" : "widt
-0000a890: 683a 2039 3025 222c 0d0a 2020 2020 2020  h: 90%",..      
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 2020 2020 2020 2273 7263 2220 3a20 7372        "src" : sr
-0000a8d0: 630d 0a20 2020 2020 2020 2020 2020 2020  c..             
-0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-0000a900: 290d 0a0d 0a20 2020 2020 2020 2065 5f64  )....        e_d
-0000a910: 6976 203d 2045 6c65 6d65 6e74 5472 6565  iv = ElementTree
-0000a920: 2e53 7562 456c 656d 656e 7428 626f 6479  .SubElement(body
-0000a930: 2c20 2264 6976 222c 207b 2269 6422 203a  , "div", {"id" :
-0000a940: 2022 7461 626c 6522 7d29 0d0a 0d0a 2020   "table"})....  
-0000a950: 2020 2020 2020 7461 626c 6573 203d 2028        tables = (
-0000a960: 7461 626c 6531 2c20 7461 626c 6532 2c20  table1, table2, 
-0000a970: 7461 626c 6532 612c 2074 6162 6c65 332c  table2a, table3,
-0000a980: 2074 6162 6c65 3429 0d0a 0d0a 2020 2020   table4)....    
-0000a990: 2020 2020 666f 7220 7461 626c 6520 696e      for table in
-0000a9a0: 2074 6162 6c65 733a 0d0a 2020 2020 2020   tables:..      
-0000a9b0: 2020 2020 2020 7469 746c 6520 3d20 7461        title = ta
-0000a9c0: 626c 655b 305d 0d0a 2020 2020 2020 2020  ble[0]..        
-0000a9d0: 2020 2020 655f 7072 6520 3d20 456c 656d      e_pre = Elem
-0000a9e0: 656e 7454 7265 652e 5375 6245 6c65 6d65  entTree.SubEleme
-0000a9f0: 6e74 2865 5f64 6976 2c20 2270 7265 2229  nt(e_div, "pre")
-0000aa00: 0d0a 2020 2020 2020 2020 2020 2020 655f  ..            e_
-0000aa10: 7520 2020 3d20 456c 656d 656e 7454 7265  u   = ElementTre
-0000aa20: 652e 5375 6245 6c65 6d65 6e74 2865 5f70  e.SubElement(e_p
-0000aa30: 7265 2c20 2275 2229 0d0a 2020 2020 2020  re, "u")..      
-0000aa40: 2020 2020 2020 7574 696c 5f78 6d6c 2e54        util_xml.T
-0000aa50: 6578 7453 7562 456c 656d 656e 7428 655f  extSubElement(e_
-0000aa60: 752c 2022 6222 2c20 7469 746c 6529 0d0a  u, "b", title)..
-0000aa70: 2020 2020 2020 2020 2020 2020 6520 2020              e   
-0000aa80: 2020 3d20 7574 696c 5f78 6d6c 2e54 6578    = util_xml.Tex
-0000aa90: 7453 7562 456c 656d 656e 7428 655f 6469  tSubElement(e_di
-0000aaa0: 762c 2022 7072 6522 2c20 275c 6e27 2e6a  v, "pre", '\n'.j
-0000aab0: 6f69 6e28 7461 626c 655b 313a 5d29 290d  oin(table[1:])).
-0000aac0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000aad0: 2020 2020 2020 2023 204b 6565 7020 696e         # Keep in
-0000aae0: 206d 696e 6420 7468 6174 2048 544d 4c20   mind that HTML 
-0000aaf0: 6973 2077 6869 7465 7370 6163 6520 7365  is whitespace se
-0000ab00: 6e73 6974 6976 652c 2061 6e64 2069 6620  nsitive, and if 
-0000ab10: 796f 7520 6361 6c6c 200d 0a20 2020 2020  you call ..     
-0000ab20: 2020 2023 2075 7469 6c5f 786d 6c2e 696e     # util_xml.in
-0000ab30: 6465 6e74 2829 206f 6e20 7468 6520 4854  dent() on the HT
-0000ab40: 4d4c 2c20 6974 2077 696c 6c20 6368 616e  ML, it will chan
-0000ab50: 6765 2074 6865 2066 6f72 6d61 7474 696e  ge the formattin
-0000ab60: 672e 0d0a 0d0a 2020 2020 2020 2020 7265  g.....        re
-0000ab70: 7475 726e 2045 6c65 6d65 6e74 5472 6565  turn ElementTree
-0000ab80: 2e74 6f73 7472 696e 6728 6874 6d6c 290d  .tostring(html).
-0000ab90: 0a0d 0a0d 0a20 2020 2064 6566 2072 6573  .....    def res
-0000aba0: 756c 7473 5f61 735f 6373 7628 7365 6c66  ults_as_csv(self
-0000abb0: 2c20 766f 7865 6c2c 206c 773d 302e 302c  , voxel, lw=0.0,
-0000abc0: 206c 776d 696e 3d30 2e30 2c20 6c77 6d61   lwmin=0.0, lwma
-0000abd0: 783d 302e 302c 2073 6f75 7263 653d 2222  x=0.0, source=""
-0000abe0: 2c20 6473 6574 6e61 6d65 3d22 2229 3a0d  , dsetname=""):.
-0000abf0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000ac00: 2020 2020 2020 4769 7665 6e20 6120 766f        Given a vo
-0000ac10: 7865 6c2c 206c 696e 6577 6964 7468 2070  xel, linewidth p
-0000ac20: 6172 616d 732c 2061 6e64 2061 2064 6174  arams, and a dat
-0000ac30: 6120 736f 7572 6365 2028 6f66 7465 6e20  a source (often 
-0000ac40: 6120 6669 6c65 6e61 6d65 292c 200d 0a20  a filename), .. 
-0000ac50: 2020 2020 2020 2072 6574 7572 6e73 2043         returns C
-0000ac60: 5356 2d66 6f72 6d61 7474 6564 2028 636f  SV-formatted (co
-0000ac70: 6d6d 6120 7365 7061 7261 7465 6420 7661  mma separated va
-0000ac80: 7269 6162 6c65 7329 7374 7269 6e67 2063  riables)string c
-0000ac90: 6f6e 7461 696e 696e 6720 626f 7468 0d0a  ontaining both..
-0000aca0: 2020 2020 2020 2020 7468 6520 766f 7865          the voxe
-0000acb0: 6c20 6669 7474 696e 6720 7265 7375 6c74  l fitting result
-0000acc0: 7320 616e 6420 6865 6164 6572 2073 7472  s and header str
-0000acd0: 696e 6720 6465 7363 7269 7074 696f 6e73  ing descriptions
-0000ace0: 2066 6f72 2065 6163 6820 0d0a 2020 2020   for each ..    
-0000acf0: 2020 2020 636f 6c75 6d6e 2e0d 0a0d 0a20      column..... 
-0000ad00: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0000ad10: 2020 2020 6864 7220 3d20 5b5d 0d0a 2020      hdr = []..  
-0000ad20: 2020 2020 2020 7661 6c20 3d20 5b5d 0d0a        val = []..
-0000ad30: 0d0a 2020 2020 2020 2020 6864 722e 6170  ..        hdr.ap
-0000ad40: 7065 6e64 2827 4669 6c65 6e61 6d65 2729  pend('Filename')
-0000ad50: 2020 200d 0a20 2020 2020 2020 2073 6f75     ..        sou
-0000ad60: 7263 6520 3d20 736f 7572 6365 2e72 6570  rce = source.rep
-0000ad70: 6c61 6365 2822 2c22 2c22 5f22 2920 2020  lace(",","_")   
-0000ad80: 2020 2320 736f 6d65 2075 7365 7273 2068    # some users h
-0000ad90: 6176 6520 636f 6d6d 6173 2069 6e20 6669  ave commas in fi
-0000ada0: 6c65 6e61 6d65 7320 0d0a 2020 2020 2020  lenames ..      
-0000adb0: 2020 7661 6c2e 6170 7065 6e64 2873 6f75    val.append(sou
-0000adc0: 7263 6529 0d0a 0d0a 2020 2020 2020 2020  rce)....        
-0000add0: 6864 722e 6170 7065 6e64 2827 4461 7461  hdr.append('Data
-0000ade0: 7365 7420 4e61 6d65 2729 2020 2020 2020  set Name')      
-0000adf0: 2020 0d0a 2020 2020 2020 2020 6473 6574    ..        dset
-0000ae00: 6e61 6d65 203d 2064 7365 746e 616d 652e  name = dsetname.
-0000ae10: 7265 706c 6163 6528 222c 222c 225f 2229  replace(",","_")
-0000ae20: 2023 2073 6f6d 6520 7573 6572 7320 6861   # some users ha
-0000ae30: 7665 2063 6f6d 6d61 7320 696e 2066 696c  ve commas in fil
-0000ae40: 656e 616d 6573 2020 2020 0d0a 2020 2020  enames    ..    
-0000ae50: 2020 2020 7661 6c2e 6170 7065 6e64 2864      val.append(d
-0000ae60: 7365 746e 616d 6529 0d0a 2020 2020 2020  setname)..      
-0000ae70: 2020 0d0a 2020 2020 2020 2020 6864 722e    ..        hdr.
-0000ae80: 6170 7065 6e64 2827 566f 7865 6c27 290d  append('Voxel').
-0000ae90: 0a20 2020 2020 2020 2076 616c 2e61 7070  .        val.app
-0000aea0: 656e 6428 7374 7228 766f 7865 6c5b 305d  end(str(voxel[0]
-0000aeb0: 292b 2720 272b 7374 7228 766f 7865 6c5b  )+' '+str(voxel[
-0000aec0: 315d 292b 2720 272b 7374 7228 766f 7865  1])+' '+str(voxe
-0000aed0: 6c5b 325d 2929 0d0a 2020 2020 2020 2020  l[2]))..        
-0000aee0: 0d0a 2020 2020 2020 2020 6e6d 6574 203d  ..        nmet =
-0000aef0: 206c 656e 2873 656c 662e 7365 742e 7072   len(self.set.pr
-0000af00: 696f 725f 6c69 7374 290d 0a20 2020 2020  ior_list)..     
-0000af10: 2020 200d 0a20 2020 2020 2020 206e 616d     ..        nam
-0000af20: 6573 203d 2073 656c 662e 7365 742e 7072  es = self.set.pr
-0000af30: 696f 725f 6c69 7374 0d0a 2020 2020 2020  ior_list..      
-0000af40: 2020 7265 7320 2020 3d20 7365 6c66 2e66    res   = self.f
-0000af50: 6974 5f72 6573 756c 7473 5b3a 2c76 6f78  it_results[:,vox
-0000af60: 656c 5b30 5d2c 766f 7865 6c5b 315d 2c76  el[0],voxel[1],v
-0000af70: 6f78 656c 5b32 5d5d 0d0a 2020 2020 2020  oxel[2]]..      
-0000af80: 2020 6372 616f 2020 3d20 7365 6c66 2e63    crao  = self.c
-0000af90: 7261 6d65 725f 7261 6f5b 203a 2c76 6f78  ramer_rao[ :,vox
-0000afa0: 656c 5b30 5d2c 766f 7865 6c5b 315d 2c76  el[0],voxel[1],v
-0000afb0: 6f78 656c 5b32 5d5d 0d0a 2020 2020 2020  oxel[2]]..      
-0000afc0: 2020 636f 6e66 2020 3d20 7365 6c66 2e63    conf  = self.c
-0000afd0: 6f6e 6669 6465 6e63 655b 203a 2c76 6f78  onfidence[ :,vox
-0000afe0: 656c 5b30 5d2c 766f 7865 6c5b 315d 2c76  el[0],voxel[1],v
-0000aff0: 6f78 656c 5b32 5d5d 0d0a 2020 2020 2020  oxel[2]]..      
-0000b000: 2020 7374 6174 7320 3d20 7365 6c66 2e66    stats = self.f
-0000b010: 6974 5f73 7461 7473 5b20 203a 2c76 6f78  it_stats[  :,vox
-0000b020: 656c 5b30 5d2c 766f 7865 6c5b 315d 2c76  el[0],voxel[1],v
-0000b030: 6f78 656c 5b32 5d5d 0d0a 2020 2020 2020  oxel[2]]..      
-0000b040: 2020 2320 626f 7468 2063 7261 6d65 722d    # both cramer-
-0000b050: 7261 6f20 616e 6420 636f 6e66 6964 656e  rao and confiden
-0000b060: 6365 2069 6e74 6572 7661 6c73 206d 6179  ce intervals may
-0000b070: 2062 6520 6f66 662f 6f6e 0d0a 2020 2020   be off/on..    
-0000b080: 2020 2020 6966 206c 656e 2863 7261 6f29      if len(crao)
-0000b090: 2021 3d20 6c65 6e28 7265 7329 3a0d 0a20   != len(res):.. 
-0000b0a0: 2020 2020 2020 2020 2020 2063 7261 6f20             crao 
-0000b0b0: 3d20 7265 7320 2a20 300d 0a20 2020 2020  = res * 0..     
-0000b0c0: 2020 2069 6620 6c65 6e28 636f 6e66 2920     if len(conf) 
-0000b0d0: 213d 206c 656e 2872 6573 293a 0d0a 2020  != len(res):..  
-0000b0e0: 2020 2020 2020 2020 2020 636f 6e66 203d            conf =
-0000b0f0: 2072 6573 202a 2030 0d0a 0d0a 2020 2020   res * 0....    
-0000b100: 2020 2020 666f 7220 692c 2069 7465 6d20      for i, item 
-0000b110: 696e 2065 6e75 6d65 7261 7465 286e 616d  in enumerate(nam
-0000b120: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
-0000b130: 2020 6864 722e 6170 7065 6e64 2827 4172    hdr.append('Ar
-0000b140: 6561 2027 2b69 7465 6d29 2020 2020 2020  ea '+item)      
-0000b150: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000b160: 6864 722e 6170 7065 6e64 2827 4372 5261  hdr.append('CrRa
-0000b170: 6f5b 255d 2729 2020 2020 2020 2020 0d0a  o[%]')        ..
-0000b180: 2020 2020 2020 2020 2020 2020 6864 722e              hdr.
-0000b190: 6170 7065 6e64 2827 436e 6649 6e74 5b25  append('CnfInt[%
-0000b1a0: 5d27 2920 2020 2020 2020 200d 0a20 2020  ]')        ..   
-0000b1b0: 2020 2020 2020 2020 2076 616c 2e61 7070           val.app
-0000b1c0: 656e 6428 7374 7228 7265 735b 695d 2929  end(str(res[i]))
-0000b1d0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000b1e0: 6c2e 6170 7065 6e64 2873 7472 2863 7261  l.append(str(cra
-0000b1f0: 6f5b 695d 2929 0d0a 2020 2020 2020 2020  o[i]))..        
-0000b200: 2020 2020 7661 6c2e 6170 7065 6e64 2873      val.append(s
-0000b210: 7472 2863 6f6e 665b 695d 2929 0d0a 0d0a  tr(conf[i]))....
-0000b220: 2020 2020 2020 2020 666f 7220 692c 6974          for i,it
-0000b230: 656d 2069 6e20 656e 756d 6572 6174 6528  em in enumerate(
-0000b240: 6e61 6d65 7329 3a0d 0a20 2020 2020 2020  names):..       
-0000b250: 2020 2020 2068 6472 2e61 7070 656e 6428       hdr.append(
-0000b260: 2750 504d 2027 2b69 7465 6d29 2020 2020  'PPM '+item)    
-0000b270: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000b280: 2020 6864 722e 6170 7065 6e64 2827 4372    hdr.append('Cr
-0000b290: 5261 6f5b 255d 2729 2020 2020 2020 2020  Rao[%]')        
-0000b2a0: 0d0a 2020 2020 2020 2020 2020 2020 6864  ..            hd
-0000b2b0: 722e 6170 7065 6e64 2827 436e 6649 6e74  r.append('CnfInt
-0000b2c0: 5b25 5d27 2920 2020 2020 2020 200d 0a20  [%]')        .. 
-0000b2d0: 2020 2020 2020 2020 2020 2076 616c 2e61             val.a
-0000b2e0: 7070 656e 6428 7374 7228 7265 735b 692b  ppend(str(res[i+
-0000b2f0: 6e6d 6574 5d29 290d 0a20 2020 2020 2020  nmet]))..       
-0000b300: 2020 2020 2076 616c 2e61 7070 656e 6428       val.append(
-0000b310: 7374 7228 6372 616f 5b69 2b6e 6d65 745d  str(crao[i+nmet]
-0000b320: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000b330: 7661 6c2e 6170 7065 6e64 2873 7472 2863  val.append(str(c
-0000b340: 6f6e 665b 692b 6e6d 6574 5d29 290d 0a0d  onf[i+nmet]))...
-0000b350: 0a20 2020 2020 2020 2066 6f72 2069 2c69  .        for i,i
-0000b360: 7465 6d20 696e 2065 6e75 6d65 7261 7465  tem in enumerate
-0000b370: 286e 616d 6573 293a 0d0a 2020 2020 2020  (names):..      
-0000b380: 2020 2020 2020 6864 722e 6170 7065 6e64        hdr.append
-0000b390: 2827 5462 5b73 6563 5d27 2b69 7465 6d29  ('Tb[sec]'+item)
-0000b3a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000b3b0: 2020 2020 2020 6864 722e 6170 7065 6e64        hdr.append
-0000b3c0: 2827 4c57 5b48 7a5d 272b 6974 656d 2920  ('LW[Hz]'+item) 
-0000b3d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000b3e0: 2020 2020 2068 6472 2e61 7070 656e 6428       hdr.append(
-0000b3f0: 2743 7252 616f 5b25 5d27 2920 2020 2020  'CrRao[%]')     
-0000b400: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000b410: 2068 6472 2e61 7070 656e 6428 2743 6e66   hdr.append('Cnf
-0000b420: 496e 745b 255d 2729 2020 2020 2020 2020  Int[%]')        
-0000b430: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000b440: 6c2e 6170 7065 6e64 2873 7472 2872 6573  l.append(str(res
-0000b450: 5b69 2b6e 6d65 742a 325d 2929 0d0a 2020  [i+nmet*2]))..  
-0000b460: 2020 2020 2020 2020 2020 7661 6c2e 6170            val.ap
-0000b470: 7065 6e64 2873 7472 286c 775b 695d 2929  pend(str(lw[i]))
-0000b480: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000b490: 6c2e 6170 7065 6e64 2873 7472 2863 7261  l.append(str(cra
-0000b4a0: 6f5b 692b 6e6d 6574 2a32 5d29 290d 0a20  o[i+nmet*2])).. 
-0000b4b0: 2020 2020 2020 2020 2020 2076 616c 2e61             val.a
-0000b4c0: 7070 656e 6428 7374 7228 636f 6e66 5b69  ppend(str(conf[i
-0000b4d0: 2b6e 6d65 742a 325d 2929 0d0a 0d0a 2020  +nmet*2]))....  
-0000b4e0: 2020 2020 2020 6864 722e 6170 7065 6e64        hdr.append
-0000b4f0: 2827 5068 6173 6530 2027 2920 2020 2020  ('Phase0 ')     
-0000b500: 2020 200d 0a20 2020 2020 2020 2068 6472     ..        hdr
-0000b510: 2e61 7070 656e 6428 2743 7252 616f 5b25  .append('CrRao[%
-0000b520: 5d27 2920 2020 2020 2020 200d 0a20 2020  ]')        ..   
-0000b530: 2020 2020 2068 6472 2e61 7070 656e 6428       hdr.append(
-0000b540: 2743 6e66 496e 745b 255d 2729 2020 2020  'CnfInt[%]')    
-0000b550: 2020 2020 0d0a 2020 2020 2020 2020 7661      ..        va
-0000b560: 6c2e 6170 7065 6e64 2873 7472 2872 6573  l.append(str(res
-0000b570: 5b6e 6d65 742a 332b 305d 2929 0d0a 2020  [nmet*3+0]))..  
-0000b580: 2020 2020 2020 7661 6c2e 6170 7065 6e64        val.append
-0000b590: 2873 7472 2863 7261 6f5b 6e6d 6574 2a33  (str(crao[nmet*3
-0000b5a0: 2b30 5d29 290d 0a20 2020 2020 2020 2076  +0]))..        v
-0000b5b0: 616c 2e61 7070 656e 6428 7374 7228 636f  al.append(str(co
-0000b5c0: 6e66 5b6e 6d65 742a 332b 305d 2929 0d0a  nf[nmet*3+0]))..
-0000b5d0: 0d0a 2020 2020 2020 2020 6864 722e 6170  ..        hdr.ap
-0000b5e0: 7065 6e64 2827 5068 6173 6531 2027 2920  pend('Phase1 ') 
-0000b5f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000b600: 2068 6472 2e61 7070 656e 6428 2743 7252   hdr.append('CrR
-0000b610: 616f 5b25 5d27 2920 2020 2020 2020 200d  ao[%]')        .
-0000b620: 0a20 2020 2020 2020 2068 6472 2e61 7070  .        hdr.app
-0000b630: 656e 6428 2743 6e66 496e 745b 255d 2729  end('CnfInt[%]')
-0000b640: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000b650: 2020 7661 6c2e 6170 7065 6e64 2873 7472    val.append(str
-0000b660: 2872 6573 5b6e 6d65 742a 332b 315d 2929  (res[nmet*3+1]))
-0000b670: 0d0a 2020 2020 2020 2020 7661 6c2e 6170  ..        val.ap
-0000b680: 7065 6e64 2873 7472 2863 7261 6f5b 6e6d  pend(str(crao[nm
-0000b690: 6574 2a33 2b31 5d29 290d 0a20 2020 2020  et*3+1]))..     
-0000b6a0: 2020 2076 616c 2e61 7070 656e 6428 7374     val.append(st
-0000b6b0: 7228 636f 6e66 5b6e 6d65 742a 332b 315d  r(conf[nmet*3+1]
-0000b6c0: 2929 0d0a 0d0a 2020 2020 2020 2020 6864  ))....        hd
-0000b6d0: 722e 6170 7065 6e64 2827 4368 6953 7175  r.append('ChiSqu
-0000b6e0: 6172 6520 2729 2020 2020 2020 2020 0d0a  are ')        ..
-0000b6f0: 2020 2020 2020 2020 7661 6c2e 6170 7065          val.appe
-0000b700: 6e64 2873 7472 2873 7461 7473 5b30 5d29  nd(str(stats[0])
-0000b710: 290d 0a0d 0a20 2020 2020 2020 2068 6472  )....        hdr
-0000b720: 2e61 7070 656e 6428 2757 7443 6869 5371  .append('WtChiSq
-0000b730: 7561 7265 2027 2920 2020 2020 2020 200d  uare ')        .
-0000b740: 0a20 2020 2020 2020 2076 616c 2e61 7070  .        val.app
-0000b750: 656e 6428 7374 7228 7374 6174 735b 315d  end(str(stats[1]
-0000b760: 2929 0d0a 0d0a 2020 2020 2020 2020 6864  ))....        hd
-0000b770: 722e 6170 7065 6e64 2827 4d61 7468 2046  r.append('Math F
-0000b780: 696e 6974 6520 4572 726f 7220 2729 2020  inite Error ')  
-0000b790: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000b7a0: 6d61 7468 6572 7220 3d20 7374 7228 7374  matherr = str(st
-0000b7b0: 6174 735b 325d 2021 3d20 3029 0d0a 2020  ats[2] != 0)..  
-0000b7c0: 2020 2020 2020 7661 6c2e 6170 7065 6e64        val.append
-0000b7d0: 2873 7472 286d 6174 6865 7272 2929 0d0a  (str(matherr))..
-0000b7e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000b7f0: 2076 616c 2c20 6864 720d 0a20 2020 200d   val, hdr..    .
-0000b800: 0a20 2020 200d 0a20 2020 2064 6566 2072  .    ..    def r
-0000b810: 6573 756c 7473 5f61 735f 6373 765f 616c  esults_as_csv_al
-0000b820: 6c5f 766f 7865 6c73 5f74 7275 6e63 6174  l_voxels_truncat
-0000b830: 6564 2873 656c 662c 2076 6f78 656c 732c  ed(self, voxels,
-0000b840: 2064 6174 6166 696c 653d 2720 272c 206d   datafile=' ', m
-0000b850: 6561 7375 7265 5f74 696d 6573 3d5b 5d29  easure_times=[])
-0000b860: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0000b870: 2020 2020 2020 2020 4769 7665 6e20 6120          Given a 
-0000b880: 766f 7865 6c2c 206c 696e 6577 6964 7468  voxel, linewidth
-0000b890: 2070 6172 616d 732c 2061 6e64 2061 2064   params, and a d
-0000b8a0: 6174 6120 736f 7572 6365 2028 6f66 7465  ata source (ofte
-0000b8b0: 6e20 6120 6669 6c65 6e61 6d65 292c 200d  n a filename), .
-0000b8c0: 0a20 2020 2020 2020 2072 6574 7572 6e73  .        returns
-0000b8d0: 2043 5356 2d66 6f72 6d61 7474 6564 2028   CSV-formatted (
-0000b8e0: 636f 6d6d 6120 7365 7061 7261 7465 6420  comma separated 
-0000b8f0: 7661 7269 6162 6c65 7329 7374 7269 6e67  variables)string
-0000b900: 2063 6f6e 7461 696e 696e 6720 626f 7468   containing both
-0000b910: 0d0a 2020 2020 2020 2020 7468 6520 766f  ..        the vo
-0000b920: 7865 6c20 6669 7474 696e 6720 7265 7375  xel fitting resu
-0000b930: 6c74 7320 616e 6420 6865 6164 6572 2073  lts and header s
-0000b940: 7472 696e 6720 6465 7363 7269 7074 696f  tring descriptio
-0000b950: 6e73 2066 6f72 2065 6163 6820 0d0a 2020  ns for each ..  
-0000b960: 2020 2020 2020 636f 6c75 6d6e 2e0d 0a0d        column....
-0000b970: 0a20 2020 2020 2020 2022 2222 0d0a 0d0a  .        """....
-0000b980: 2020 2020 2020 2020 736f 7572 6365 203d          source =
-0000b990: 2064 6174 6166 696c 652e 7265 706c 6163   datafile.replac
-0000b9a0: 6528 222c 222c 225f 2229 2020 2020 2023  e(",","_")     #
-0000b9b0: 2073 6f6d 6520 7573 6572 7320 6861 7665   some users have
-0000b9c0: 2063 6f6d 6d61 7320 696e 2066 696c 656e   commas in filen
-0000b9d0: 616d 6573 200d 0a0d 0a20 2020 2020 2020  ames ....       
-0000b9e0: 206e 6d65 7420 3d20 6c65 6e28 7365 6c66   nmet = len(self
-0000b9f0: 2e73 6574 2e70 7269 6f72 5f6c 6973 7429  .set.prior_list)
-0000ba00: 0d0a 2020 2020 2020 2020 6e61 6d65 7320  ..        names 
-0000ba10: 3d20 7365 6c66 2e73 6574 2e70 7269 6f72  = self.set.prior
-0000ba20: 5f6c 6973 740d 0a20 2020 2020 2020 200d  _list..        .
-0000ba30: 0a20 2020 2020 2020 2068 6472 203d 205b  .        hdr = [
-0000ba40: 5d0d 0a20 2020 2020 2020 2076 616c 203d  ]..        val =
-0000ba50: 205b 5d0d 0a0d 0a20 2020 2020 2020 2068   []....        h
-0000ba60: 6472 2e61 7070 656e 6428 2744 6174 6166  dr.append('Dataf
-0000ba70: 696c 6527 2920 2020 0d0a 2020 2020 2020  ile')   ..      
-0000ba80: 2020 6864 722e 6170 7065 6e64 2827 566f    hdr.append('Vo
-0000ba90: 7865 6c27 290d 0a20 2020 2020 2020 2068  xel')..        h
-0000baa0: 6472 2e61 7070 656e 6428 2754 696d 6520  dr.append('Time 
-0000bab0: 5b73 6563 5d27 290d 0a0d 0a20 2020 2020  [sec]')....     
-0000bac0: 2020 2066 6f72 2069 2c20 6974 656d 2069     for i, item i
-0000bad0: 6e20 656e 756d 6572 6174 6528 6e61 6d65  n enumerate(name
-0000bae0: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-0000baf0: 2068 6472 2e61 7070 656e 6428 2741 7265   hdr.append('Are
-0000bb00: 6120 272b 6974 656d 2920 2020 2020 2020  a '+item)       
-0000bb10: 200d 0a20 2020 2020 2020 2020 2020 2068   ..            h
-0000bb20: 6472 2e61 7070 656e 6428 2750 504d 2027  dr.append('PPM '
-0000bb30: 2b69 7465 6d29 2020 2020 2020 2020 0d0a  +item)        ..
-0000bb40: 2020 2020 2020 2020 2020 2020 6864 722e              hdr.
-0000bb50: 6170 7065 6e64 2827 5462 5b73 6563 5d27  append('Tb[sec]'
-0000bb60: 2b69 7465 6d29 2020 2020 2020 2020 0d0a  +item)        ..
-0000bb70: 2020 2020 2020 2020 6864 722e 6170 7065          hdr.appe
-0000bb80: 6e64 2827 5068 6173 6530 2027 2920 2020  nd('Phase0 ')   
-0000bb90: 2020 2020 200d 0a20 2020 2020 2020 2068       ..        h
-0000bba0: 6472 2e61 7070 656e 6428 2750 6861 7365  dr.append('Phase
-0000bbb0: 3120 2729 2020 2020 2020 2020 0d0a 0d0a  1 ')        ....
-0000bbc0: 0d0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-0000bbd0: 766f 7865 6c20 696e 2065 6e75 6d65 7261  voxel in enumera
-0000bbe0: 7465 2876 6f78 656c 7329 3a0d 0a0d 0a20  te(voxels):.... 
-0000bbf0: 2020 2020 2020 2020 2020 2072 6573 2020             res  
-0000bc00: 203d 2073 656c 662e 6669 745f 7265 7375   = self.fit_resu
-0000bc10: 6c74 735b 3a2c 766f 7865 6c5b 305d 2c76  lts[:,voxel[0],v
-0000bc20: 6f78 656c 5b31 5d2c 766f 7865 6c5b 325d  oxel[1],voxel[2]
-0000bc30: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
-0000bc40: 7469 6d65 203d 206d 6561 7375 7265 5f74  time = measure_t
-0000bc50: 696d 6573 5b69 5d0d 0a20 2020 2020 2020  imes[i]..       
-0000bc60: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000bc70: 2020 2076 616c 2e61 7070 656e 6428 6461     val.append(da
-0000bc80: 7461 6669 6c65 290d 0a20 2020 2020 2020  tafile)..       
-0000bc90: 2020 2020 2076 616c 2e61 7070 656e 6428       val.append(
-0000bca0: 7374 7228 766f 7865 6c5b 305d 292b 2720  str(voxel[0])+' 
-0000bcb0: 272b 7374 7228 766f 7865 6c5b 315d 292b  '+str(voxel[1])+
-0000bcc0: 2720 272b 7374 7228 766f 7865 6c5b 325d  ' '+str(voxel[2]
-0000bcd0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000bce0: 7661 6c2e 6170 7065 6e64 2869 7469 6d65  val.append(itime
-0000bcf0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-0000bd00: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000bd10: 2069 2c20 6974 656d 2069 6e20 656e 756d   i, item in enum
-0000bd20: 6572 6174 6528 6e61 6d65 7329 3a0d 0a20  erate(names):.. 
-0000bd30: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000bd40: 616c 2e61 7070 656e 6428 7374 7228 7265  al.append(str(re
-0000bd50: 735b 692b 6e6d 6574 2a30 5d29 290d 0a20  s[i+nmet*0])).. 
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000bd70: 616c 2e61 7070 656e 6428 7374 7228 7265  al.append(str(re
-0000bd80: 735b 692b 6e6d 6574 2a31 5d29 290d 0a20  s[i+nmet*1])).. 
-0000bd90: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000bda0: 616c 2e61 7070 656e 6428 7374 7228 7265  al.append(str(re
-0000bdb0: 735b 692b 6e6d 6574 2a32 5d29 290d 0a0d  s[i+nmet*2]))...
-0000bdc0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000bdd0: 2e61 7070 656e 6428 7374 7228 7265 735b  .append(str(res[
-0000bde0: 6e6d 6574 2a33 2b30 5d29 290d 0a20 2020  nmet*3+0]))..   
-0000bdf0: 2020 2020 2020 2020 2076 616c 2e61 7070           val.app
-0000be00: 656e 6428 7374 7228 7265 735b 6e6d 6574  end(str(res[nmet
-0000be10: 2a33 2b31 5d29 290d 0a20 2020 200d 0a0d  *3+1]))..    ...
-0000be20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000be30: 7661 6c2c 2068 6472 2020 2020 0d0a 2020  val, hdr    ..  
-0000be40: 2020 0d0a 2020 2020 0d0a 2020 2020 6465    ..    ..    de
-0000be50: 6620 7265 7375 6c74 735f 6173 5f63 7376  f results_as_csv
-0000be60: 5f61 6c6c 5f76 6f78 656c 735f 6172 6561  _all_voxels_area
-0000be70: 7328 7365 6c66 2c20 766f 7865 6c73 2c20  s(self, voxels, 
-0000be80: 6461 7461 6669 6c65 3d27 2027 2c20 6d65  datafile=' ', me
-0000be90: 6173 7572 655f 7469 6d65 733d 5b5d 293a  asure_times=[]):
-0000bea0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000beb0: 2020 2020 2020 2047 6976 656e 2061 2076         Given a v
-0000bec0: 6f78 656c 2c20 6c69 6e65 7769 6474 6820  oxel, linewidth 
-0000bed0: 7061 7261 6d73 2c20 616e 6420 6120 6461  params, and a da
-0000bee0: 7461 2073 6f75 7263 6520 286f 6674 656e  ta source (often
-0000bef0: 2061 2066 696c 656e 616d 6529 2c20 0d0a   a filename), ..
-0000bf00: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-0000bf10: 4353 562d 666f 726d 6174 7465 6420 2863  CSV-formatted (c
-0000bf20: 6f6d 6d61 2073 6570 6172 6174 6564 2076  omma separated v
-0000bf30: 6172 6961 626c 6573 2973 7472 696e 6720  ariables)string 
-0000bf40: 636f 6e74 6169 6e69 6e67 2062 6f74 680d  containing both.
-0000bf50: 0a20 2020 2020 2020 2074 6865 2076 6f78  .        the vox
-0000bf60: 656c 2066 6974 7469 6e67 2072 6573 756c  el fitting resul
-0000bf70: 7473 2061 6e64 2068 6561 6465 7220 7374  ts and header st
-0000bf80: 7269 6e67 2064 6573 6372 6970 7469 6f6e  ring description
-0000bf90: 7320 666f 7220 6561 6368 200d 0a20 2020  s for each ..   
-0000bfa0: 2020 2020 2063 6f6c 756d 6e2e 0d0a 0d0a       column.....
-0000bfb0: 2020 2020 2020 2020 2222 220d 0a0d 0a20          """.... 
-0000bfc0: 2020 2020 2020 2073 6f75 7263 6520 3d20         source = 
-0000bfd0: 6461 7461 6669 6c65 2e72 6570 6c61 6365  datafile.replace
-0000bfe0: 2822 2c22 2c22 5f22 2920 2020 2020 2320  (",","_")     # 
-0000bff0: 736f 6d65 2075 7365 7273 2068 6176 6520  some users have 
-0000c000: 636f 6d6d 6173 2069 6e20 6669 6c65 6e61  commas in filena
-0000c010: 6d65 7320 0d0a 0d0a 2020 2020 2020 2020  mes ....        
-0000c020: 6e6d 6574 203d 206c 656e 2873 656c 662e  nmet = len(self.
-0000c030: 7365 742e 7072 696f 725f 6c69 7374 290d  set.prior_list).
-0000c040: 0a20 2020 2020 2020 206e 616d 6573 203d  .        names =
-0000c050: 2073 656c 662e 7365 742e 7072 696f 725f   self.set.prior_
-0000c060: 6c69 7374 0d0a 2020 2020 2020 2020 0d0a  list..        ..
-0000c070: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
-0000c080: 5b5d 0d0a 0d0a 2020 2020 2020 2020 7469  []....        ti
-0000c090: 6d65 7320 3d20 5b5d 0d0a 2020 2020 2020  mes = []..      
-0000c0a0: 2020 7469 6d65 732e 6170 7065 6e64 2873    times.append(s
-0000c0b0: 6f75 7263 6529 0d0a 2020 2020 2020 2020  ource)..        
-0000c0c0: 7469 6d65 732e 6170 7065 6e64 2827 5f54  times.append('_T
-0000c0d0: 696d 6520 5b6d 696e 5d20 2729 0d0a 2020  ime [min] ')..  
-0000c0e0: 2020 2020 2020 666f 7220 6d65 6173 7572        for measur
-0000c0f0: 655f 7469 6d65 2069 6e20 6d65 6173 7572  e_time in measur
-0000c100: 655f 7469 6d65 733a 0d0a 2020 2020 2020  e_times:..      
-0000c110: 2020 2020 2020 7469 6d65 732e 6170 7065        times.appe
-0000c120: 6e64 2873 7472 2828 6d65 6173 7572 655f  nd(str((measure_
-0000c130: 7469 6d65 202d 206d 6561 7375 7265 5f74  time - measure_t
-0000c140: 696d 6573 5b30 5d29 2f36 302e 3029 2920  imes[0])/60.0)) 
-0000c150: 2020 2020 2020 2320 696e 206d 696e 7574        # in minut
-0000c160: 6573 0d0a 2020 2020 2020 2020 6c69 6e65  es..        line
-0000c170: 732e 6170 7065 6e64 2874 696d 6573 290d  s.append(times).
-0000c180: 0a0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
-0000c190: 2020 2020 2066 6f72 206a 2c20 6e61 6d65       for j, name
-0000c1a0: 2069 6e20 656e 756d 6572 6174 6528 6e61   in enumerate(na
-0000c1b0: 6d65 7329 3a0d 0a20 2020 2020 2020 2020  mes):..         
-0000c1c0: 2020 2076 616c 203d 205b 5d0d 0a20 2020     val = []..   
-0000c1d0: 2020 2020 2020 2020 2076 616c 2e61 7070           val.app
-0000c1e0: 656e 6428 736f 7572 6365 290d 0a20 2020  end(source)..   
-0000c1f0: 2020 2020 2020 2020 2076 616c 2e61 7070           val.app
-0000c200: 656e 6428 6e61 6d65 2b27 2041 7265 6127  end(name+' Area'
-0000c210: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0000c220: 6f72 2069 2c76 6f78 656c 2069 6e20 656e  or i,voxel in en
-0000c230: 756d 6572 6174 6528 766f 7865 6c73 293a  umerate(voxels):
-0000c240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c250: 2020 7661 6c2e 6170 7065 6e64 2820 7374    val.append( st
-0000c260: 7228 7365 6c66 2e66 6974 5f72 6573 756c  r(self.fit_resul
-0000c270: 7473 5b6a 2b6e 6d65 742a 302c 766f 7865  ts[j+nmet*0,voxe
-0000c280: 6c5b 305d 2c76 6f78 656c 5b31 5d2c 766f  l[0],voxel[1],vo
-0000c290: 7865 6c5b 325d 5d29 2029 0d0a 2020 2020  xel[2]]) )..    
-0000c2a0: 2020 2020 2020 2020 6c69 6e65 732e 6170          lines.ap
-0000c2b0: 7065 6e64 2876 616c 290d 0a0d 0a20 2020  pend(val)....   
-0000c2c0: 2020 2020 2072 6574 7572 6e20 6c69 6e65       return line
-0000c2d0: 7320 2020 200d 0a0d 0a0d 0a0d 0a20 2020  s    ........   
-0000c2e0: 2064 6566 2072 6573 756c 7473 5f69 6e5f   def results_in_
-0000c2f0: 7461 626c 6528 7365 6c66 2c20 766f 7865  table(self, voxe
-0000c300: 6c2c 206c 773d 302e 302c 206c 776d 696e  l, lw=0.0, lwmin
-0000c310: 3d30 2e30 2c20 6c77 6d61 783d 302e 302c  =0.0, lwmax=0.0,
-0000c320: 206e 6f7a 6572 6f73 3d46 616c 7365 2c20   nozeros=False, 
-0000c330: 6e6f 7070 6d3d 4661 6c73 652c 2066 6978  noppm=False, fix
-0000c340: 7068 6173 653d 4661 6c73 6529 3a0d 0a20  phase=False):.. 
-0000c350: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0000c360: 2020 2020 4769 7665 6e20 6120 766f 7865      Given a voxe
-0000c370: 6c2c 206c 696e 6577 6964 7468 2070 6172  l, linewidth par
-0000c380: 616d 732c 2061 6e64 2061 2064 6174 6120  ams, and a data 
-0000c390: 736f 7572 6365 2028 6f66 7465 6e20 6120  source (often a 
-0000c3a0: 6669 6c65 6e61 6d65 292c 200d 0a20 2020  filename), ..   
-0000c3b0: 2020 2020 2072 6574 7572 6e73 2066 6f72       returns for
-0000c3c0: 6d61 7474 6564 2072 6573 756c 7473 2066  matted results f
-0000c3d0: 6f72 2074 6861 7420 766f 7865 6c2e 200d  or that voxel. .
-0000c3e0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0000c3f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000c400: 2320 4669 7273 7420 7765 2061 7373 656d  # First we assem
-0000c410: 626c 6520 7468 6520 6461 7461 2077 6520  ble the data we 
-0000c420: 6e65 6564 2e0d 0a20 2020 2020 2020 206e  need...        n
-0000c430: 6d65 7420 203d 206c 656e 2873 656c 662e  met  = len(self.
-0000c440: 7365 742e 7072 696f 725f 6c69 7374 290d  set.prior_list).
-0000c450: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0000c460: 2020 206e 616d 6573 203d 2073 656c 662e     names = self.
-0000c470: 7365 742e 7072 696f 725f 6c69 7374 0d0a  set.prior_list..
-0000c480: 2020 2020 2020 2020 7265 7320 2020 3d20          res   = 
-0000c490: 7365 6c66 2e66 6974 5f72 6573 756c 7473  self.fit_results
-0000c4a0: 5b3a 2c76 6f78 656c 5b30 5d2c 766f 7865  [:,voxel[0],voxe
-0000c4b0: 6c5b 315d 2c76 6f78 656c 5b32 5d5d 0d0a  l[1],voxel[2]]..
-0000c4c0: 2020 2020 2020 2020 6372 616f 2020 3d20          crao  = 
-0000c4d0: 7365 6c66 2e63 7261 6d65 725f 7261 6f5b  self.cramer_rao[
-0000c4e0: 3a2c 766f 7865 6c5b 305d 2c76 6f78 656c  :,voxel[0],voxel
-0000c4f0: 5b31 5d2c 766f 7865 6c5b 325d 5d0d 0a20  [1],voxel[2]].. 
-0000c500: 2020 2020 2020 2063 6f6e 6620 203d 2073         conf  = s
-0000c510: 656c 662e 636f 6e66 6964 656e 6365 5b3a  elf.confidence[:
-0000c520: 2c76 6f78 656c 5b30 5d2c 766f 7865 6c5b  ,voxel[0],voxel[
-0000c530: 315d 2c76 6f78 656c 5b32 5d5d 0d0a 2020  1],voxel[2]]..  
-0000c540: 2020 2020 2020 7374 6174 7320 3d20 7365        stats = se
-0000c550: 6c66 2e66 6974 5f73 7461 7473 5b3a 2c76  lf.fit_stats[:,v
-0000c560: 6f78 656c 5b30 5d2c 766f 7865 6c5b 315d  oxel[0],voxel[1]
-0000c570: 2c76 6f78 656c 5b32 5d5d 0d0a 2020 2020  ,voxel[2]]..    
-0000c580: 2020 2020 0d0a 2020 2020 2020 2020 646f      ..        do
-0000c590: 5f63 7261 6f20 3d20 4661 6c73 6520 6966  _crao = False if
-0000c5a0: 206d 6178 2863 7261 6f29 203d 3d20 302e   max(crao) == 0.
-0000c5b0: 3020 616e 6420 6e6f 7a65 726f 7320 656c  0 and nozeros el
-0000c5c0: 7365 2054 7275 650d 0a20 2020 2020 2020  se True..       
-0000c5d0: 2064 6f5f 636f 6e66 203d 2046 616c 7365   do_conf = False
-0000c5e0: 2069 6620 6d61 7828 636f 6e66 2920 3d3d   if max(conf) ==
-0000c5f0: 2030 2e30 2061 6e64 206e 6f7a 6572 6f73   0.0 and nozeros
-0000c600: 2065 6c73 6520 5472 7565 0d0a 2020 2020   else True..    
-0000c610: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
-0000c620: 626f 7468 2063 7261 6d65 722d 7261 6f20  both cramer-rao 
-0000c630: 616e 6420 636f 6e66 6964 656e 6365 2069  and confidence i
-0000c640: 6e74 6572 7661 6c73 206d 6179 2062 6520  ntervals may be 
-0000c650: 6f66 662f 6f6e 0d0a 2020 2020 2020 2020  off/on..        
-0000c660: 6966 206c 656e 2863 7261 6f29 2021 3d20  if len(crao) != 
-0000c670: 6c65 6e28 7265 7329 3a0d 0a20 2020 2020  len(res):..     
-0000c680: 2020 2020 2020 2063 7261 6f20 3d20 7265         crao = re
-0000c690: 7320 2a20 300d 0a20 2020 2020 2020 2069  s * 0..        i
-0000c6a0: 6620 6c65 6e28 636f 6e66 2920 213d 206c  f len(conf) != l
-0000c6b0: 656e 2872 6573 293a 0d0a 2020 2020 2020  en(res):..      
-0000c6c0: 2020 2020 2020 636f 6e66 203d 2072 6573        conf = res
-0000c6d0: 202a 2030 0d0a 0d0a 2020 2020 2020 2020   * 0....        
-0000c6e0: 6864 7231 2020 3d20 5b27 4d65 7461 6220  hdr1  = ['Metab 
-0000c6f0: 5265 7375 6c74 7327 2c20 2741 7265 6127  Results', 'Area'
-0000c700: 5d0d 0a20 2020 2020 2020 2068 6472 3220  ]..        hdr2 
-0000c710: 203d 205b 2750 504d 2052 6573 756c 7473   = ['PPM Results
-0000c720: 272c 2027 5050 4d27 5d0d 0a20 2020 2020  ', 'PPM']..     
-0000c730: 2020 2068 6472 3261 203d 205b 2754 6220     hdr2a = ['Tb 
-0000c740: 5265 7375 6c74 7327 2c20 2754 6220 5b73  Results', 'Tb [s
-0000c750: 6563 5d27 2c20 274c 5720 5b48 7a5d 275d  ec]', 'LW [Hz]']
-0000c760: 0d0a 2020 2020 2020 2020 6864 7233 2020  ..        hdr3  
-0000c770: 3d20 5b27 476c 6f62 616c 2052 6573 756c  = ['Global Resul
-0000c780: 7473 272c 2027 5661 6c75 6527 5d0d 0a20  ts', 'Value'].. 
-0000c790: 2020 2020 2020 2068 6472 3420 203d 205b         hdr4  = [
-0000c7a0: 2743 616c 6320 5265 7375 6c74 7327 2c20  'Calc Results', 
-0000c7b0: 2720 5661 6c75 6527 5d0d 0a20 2020 2020  ' Value']..     
-0000c7c0: 2020 2069 6620 646f 5f63 7261 6f3a 200d     if do_crao: .
-0000c7d0: 0a20 2020 2020 2020 2020 2020 2068 6472  .            hdr
-0000c7e0: 312e 6170 7065 6e64 2827 4372 5261 6f5b  1.append('CrRao[
-0000c7f0: 255d 2729 0d0a 2020 2020 2020 2020 2020  %]')..          
-0000c800: 2020 6864 7232 2e61 7070 656e 6428 2743    hdr2.append('C
-0000c810: 7252 616f 5b64 656c 7461 5d27 290d 0a20  rRao[delta]').. 
-0000c820: 2020 2020 2020 2020 2020 2068 6472 3261             hdr2a
-0000c830: 2e61 7070 656e 6428 2743 7252 616f 5b64  .append('CrRao[d
-0000c840: 656c 7461 5d27 290d 0a20 2020 2020 2020  elta]')..       
-0000c850: 2020 2020 2068 6472 332e 6170 7065 6e64       hdr3.append
-0000c860: 2827 4372 5261 6f5b 6465 6c74 615d 2729  ('CrRao[delta]')
-0000c870: 0d0a 2020 2020 2020 2020 2020 2020 6864  ..            hd
-0000c880: 7234 2e61 7070 656e 6428 2720 2729 0d0a  r4.append(' ')..
-0000c890: 2020 2020 2020 2020 6966 2064 6f5f 636f          if do_co
-0000c8a0: 6e66 3a20 0d0a 2020 2020 2020 2020 2020  nf: ..          
-0000c8b0: 2020 6864 7231 2e61 7070 656e 6428 2743    hdr1.append('C
-0000c8c0: 6e66 496e 745b 255d 2729 0d0a 2020 2020  nfInt[%]')..    
-0000c8d0: 2020 2020 2020 2020 6864 7232 2e61 7070          hdr2.app
-0000c8e0: 656e 6428 2743 6e66 496e 745b 6465 6c74  end('CnfInt[delt
-0000c8f0: 615d 2729 0d0a 2020 2020 2020 2020 2020  a]')..          
-0000c900: 2020 6864 7232 612e 6170 7065 6e64 2827    hdr2a.append('
-0000c910: 436e 6649 6e74 5b64 656c 7461 5d27 290d  CnfInt[delta]').
-0000c920: 0a20 2020 2020 2020 2020 2020 2068 6472  .            hdr
-0000c930: 332e 6170 7065 6e64 2827 436e 6649 6e74  3.append('CnfInt
-0000c940: 5b64 656c 7461 5d27 290d 0a20 2020 2020  [delta]')..     
-0000c950: 2020 2020 2020 2068 6472 342e 6170 7065         hdr4.appe
-0000c960: 6e64 2827 2027 290d 0a0d 0a20 2020 2020  nd(' ')....     
-0000c970: 2020 206e 7365 6374 203d 205b 302c 5d0d     nsect = [0,].
-0000c980: 0a20 2020 2020 2020 2074 6162 6c65 3120  .        table1 
-0000c990: 3d20 5b68 6472 312c 5d0d 0a20 2020 2020  = [hdr1,]..     
-0000c9a0: 2020 200d 0a20 2020 2020 2020 2066 6f72     ..        for
-0000c9b0: 2069 2c20 6974 656d 2069 6e20 656e 756d   i, item in enum
-0000c9c0: 6572 6174 6528 6e61 6d65 7329 3a0d 0a20  erate(names):.. 
-0000c9d0: 2020 2020 2020 2020 2020 2074 6d70 203d             tmp =
-0000c9e0: 205b 6974 656d 2c20 7265 735b 695d 5d0d   [item, res[i]].
-0000c9f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ca00: 646f 5f63 7261 6f3a 2074 6d70 2e61 7070  do_crao: tmp.app
-0000ca10: 656e 6428 6372 616f 5b69 5d29 0d0a 2020  end(crao[i])..  
-0000ca20: 2020 2020 2020 2020 2020 6966 2064 6f5f            if do_
-0000ca30: 636f 6e66 3a20 746d 702e 6170 7065 6e64  conf: tmp.append
-0000ca40: 2863 6f6e 665b 695d 290d 0a20 2020 2020  (conf[i])..     
-0000ca50: 2020 2020 2020 2074 6162 6c65 312e 6170         table1.ap
-0000ca60: 7065 6e64 2874 6d70 290d 0a0d 0a20 2020  pend(tmp)....   
-0000ca70: 2020 2020 2069 6620 7365 6c66 2e73 6574       if self.set
-0000ca80: 2e6d 6163 726f 6d6f 6c5f 6d6f 6465 6c20  .macromol_model 
-0000ca90: 3d3d 2046 6974 4d61 6372 6f6d 6f6c 6563  == FitMacromolec
-0000caa0: 756c 654d 6574 686f 642e 5349 4e47 4c45  uleMethod.SINGLE
-0000cab0: 5f42 4153 4953 5f44 4154 4153 4554 3a0d  _BASIS_DATASET:.
-0000cac0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-0000cad0: 203d 205b 274d 4d6f 6c27 2c20 7265 735b   = ['MMol', res[
-0000cae0: 6e6d 6574 2a33 2b32 5d5d 0d0a 2020 2020  nmet*3+2]]..    
-0000caf0: 2020 2020 2020 2020 6966 2064 6f5f 6372          if do_cr
-0000cb00: 616f 3a20 746d 702e 6170 7065 6e64 2830  ao: tmp.append(0
-0000cb10: 2e30 290d 0a20 2020 2020 2020 2020 2020  .0)..           
-0000cb20: 2069 6620 646f 5f63 6f6e 663a 2074 6d70   if do_conf: tmp
-0000cb30: 2e61 7070 656e 6428 302e 3029 0d0a 2020  .append(0.0)..  
-0000cb40: 2020 2020 2020 2020 2020 7461 626c 6531            table1
-0000cb50: 2e61 7070 656e 6428 746d 7029 0d0a 2020  .append(tmp)..  
-0000cb60: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000cb70: 2020 2020 6e73 6563 742e 6170 7065 6e64      nsect.append
-0000cb80: 286c 656e 2874 6162 6c65 3129 290d 0a0d  (len(table1))...
-0000cb90: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000cba0: 6e6f 7070 6d3a 0d0a 2020 2020 2020 2020  noppm:..        
-0000cbb0: 2020 2020 7461 626c 6531 2e61 7070 656e      table1.appen
-0000cbc0: 6428 6864 7232 290d 0a20 2020 2020 2020  d(hdr2)..       
-0000cbd0: 2020 2020 2066 6f72 2069 2c69 7465 6d20       for i,item 
-0000cbe0: 696e 2065 6e75 6d65 7261 7465 286e 616d  in enumerate(nam
-0000cbf0: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
-0000cc00: 2020 2020 2020 746d 7020 3d20 5b69 7465        tmp = [ite
-0000cc10: 6d2c 2072 6573 5b69 2b6e 6d65 745d 5d0d  m, res[i+nmet]].
-0000cc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cc30: 2069 6620 646f 5f63 7261 6f3a 2074 6d70   if do_crao: tmp
-0000cc40: 2e61 7070 656e 6428 6372 616f 5b69 2b6e  .append(crao[i+n
-0000cc50: 6d65 745d 290d 0a20 2020 2020 2020 2020  met])..         
-0000cc60: 2020 2020 2020 2069 6620 646f 5f63 6f6e         if do_con
-0000cc70: 663a 2074 6d70 2e61 7070 656e 6428 636f  f: tmp.append(co
-0000cc80: 6e66 5b69 2b6e 6d65 745d 290d 0a20 2020  nf[i+nmet])..   
-0000cc90: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-0000cca0: 6c65 312e 6170 7065 6e64 2874 6d70 290d  le1.append(tmp).
-0000ccb0: 0a20 2020 2020 0d0a 2020 2020 2020 2020  .     ..        
-0000ccc0: 2020 2020 6966 2073 656c 662e 7365 742e      if self.set.
-0000ccd0: 6d61 6372 6f6d 6f6c 5f6d 6f64 656c 203d  macromol_model =
-0000cce0: 3d20 4669 744d 6163 726f 6d6f 6c65 6375  = FitMacromolecu
-0000ccf0: 6c65 4d65 7468 6f64 2e53 494e 474c 455f  leMethod.SINGLE_
-0000cd00: 4241 5349 535f 4441 5441 5345 543a 0d0a  BASIS_DATASET:..
-0000cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd20: 746d 7020 3d20 5b27 4d4d 6f6c 272c 2072  tmp = ['MMol', r
-0000cd30: 6573 5b6e 6d65 742a 332b 335d 5d0d 0a20  es[nmet*3+3]].. 
-0000cd40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000cd50: 6620 646f 5f63 7261 6f3a 2074 6d70 2e61  f do_crao: tmp.a
-0000cd60: 7070 656e 6428 302e 3029 0d0a 2020 2020  ppend(0.0)..    
-0000cd70: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0000cd80: 6f5f 636f 6e66 3a20 746d 702e 6170 7065  o_conf: tmp.appe
-0000cd90: 6e64 2830 2e30 290d 0a20 2020 2020 2020  nd(0.0)..       
-0000cda0: 2020 2020 2020 2020 2074 6162 6c65 312e           table1.
-0000cdb0: 6170 7065 6e64 2874 6d70 290d 0a0d 0a20  append(tmp).... 
-0000cdc0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-0000cdd0: 312e 6170 7065 6e64 2868 6472 3261 290d  1.append(hdr2a).
-0000cde0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000cdf0: 2069 2c69 7465 6d20 696e 2065 6e75 6d65   i,item in enume
-0000ce00: 7261 7465 286e 616d 6573 293a 0d0a 2020  rate(names):..  
-0000ce10: 2020 2020 2020 2020 2020 2020 2020 746d                tm
-0000ce20: 7020 3d20 5b69 7465 6d2c 2072 6573 5b69  p = [item, res[i
-0000ce30: 2b6e 6d65 742a 325d 2c20 6c77 5b69 5d5d  +nmet*2], lw[i]]
-0000ce40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ce50: 2020 6966 2064 6f5f 6372 616f 3a20 746d    if do_crao: tm
-0000ce60: 702e 6170 7065 6e64 2863 7261 6f5b 692b  p.append(crao[i+
-0000ce70: 6e6d 6574 2a32 5d29 0d0a 2020 2020 2020  nmet*2])..      
-0000ce80: 2020 2020 2020 2020 2020 6966 2064 6f5f            if do_
-0000ce90: 636f 6e66 3a20 746d 702e 6170 7065 6e64  conf: tmp.append
-0000cea0: 2863 6f6e 665b 692b 6e6d 6574 2a32 5d29  (conf[i+nmet*2])
-0000ceb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cec0: 2020 7461 626c 6531 2e61 7070 656e 6428    table1.append(
-0000ced0: 746d 7029 0d0a 2020 2020 200d 0a20 2020  tmp)..     ..   
-0000cee0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000cef0: 2e73 6574 2e6d 6163 726f 6d6f 6c5f 6d6f  .set.macromol_mo
-0000cf00: 6465 6c20 3d3d 2046 6974 4d61 6372 6f6d  del == FitMacrom
-0000cf10: 6f6c 6563 756c 654d 6574 686f 642e 5349  oleculeMethod.SI
-0000cf20: 4e47 4c45 5f42 4153 4953 5f44 4154 4153  NGLE_BASIS_DATAS
-0000cf30: 4554 3a0d 0a20 2020 2020 2020 2020 2020  ET:..           
-0000cf40: 2020 2020 2074 6d70 203d 205b 274d 4d6f       tmp = ['MMo
-0000cf50: 6c27 2c20 7265 735b 6e6d 6574 2a33 2b34  l', res[nmet*3+4
-0000cf60: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
-0000cf70: 2020 2020 6966 2064 6f5f 6372 616f 3a20      if do_crao: 
-0000cf80: 746d 702e 6170 7065 6e64 2830 2e30 290d  tmp.append(0.0).
-0000cf90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cfa0: 2069 6620 646f 5f63 6f6e 663a 2074 6d70   if do_conf: tmp
-0000cfb0: 2e61 7070 656e 6428 302e 3029 0d0a 2020  .append(0.0)..  
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000cfd0: 626c 6531 2e61 7070 656e 6428 746d 7029  ble1.append(tmp)
-0000cfe0: 0d0a 0d0a 2020 2020 2020 2020 6e73 6563  ....        nsec
-0000cff0: 742e 6170 7065 6e64 286c 656e 2874 6162  t.append(len(tab
-0000d000: 6c65 3129 290d 0a20 2020 2020 2020 2074  le1))..        t
-0000d010: 6162 6c65 312e 6170 7065 6e64 2868 6472  able1.append(hdr
-0000d020: 3329 0d0a 2020 2020 2020 2020 0d0a 2020  3)..        ..  
-0000d030: 2020 2020 2020 6966 206e 6f74 2066 6978        if not fix
-0000d040: 7068 6173 653a 0d0a 2020 2020 2020 2020  phase:..        
-0000d050: 2020 2020 746d 7020 3d20 5b27 5068 6173      tmp = ['Phas
-0000d060: 6530 272c 2072 6573 5b6e 6d65 742a 332b  e0', res[nmet*3+
-0000d070: 305d 5d0d 0a20 2020 2020 2020 2020 2020  0]]..           
-0000d080: 2069 6620 646f 5f63 7261 6f3a 2074 6d70   if do_crao: tmp
-0000d090: 2e61 7070 656e 6428 6372 616f 5b6e 6d65  .append(crao[nme
-0000d0a0: 742a 332b 305d 290d 0a20 2020 2020 2020  t*3+0])..       
-0000d0b0: 2020 2020 2069 6620 646f 5f63 6f6e 663a       if do_conf:
-0000d0c0: 2074 6d70 2e61 7070 656e 6428 636f 6e66   tmp.append(conf
-0000d0d0: 5b6e 6d65 742a 332b 305d 290d 0a20 2020  [nmet*3+0])..   
-0000d0e0: 2020 2020 2020 2020 2074 6162 6c65 312e           table1.
-0000d0f0: 6170 7065 6e64 2874 6d70 290d 0a20 2020  append(tmp)..   
-0000d100: 200d 0a20 2020 2020 2020 2020 2020 2074   ..            t
-0000d110: 6d70 203d 205b 2750 6861 7365 3127 2c20  mp = ['Phase1', 
-0000d120: 7265 735b 6e6d 6574 2a33 2b31 5d5d 0d0a  res[nmet*3+1]]..
-0000d130: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0000d140: 6f5f 6372 616f 3a20 746d 702e 6170 7065  o_crao: tmp.appe
-0000d150: 6e64 2863 7261 6f5b 6e6d 6574 2a33 2b31  nd(crao[nmet*3+1
-0000d160: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-0000d170: 6966 2064 6f5f 636f 6e66 3a20 746d 702e  if do_conf: tmp.
-0000d180: 6170 7065 6e64 2863 6f6e 665b 6e6d 6574  append(conf[nmet
-0000d190: 2a33 2b31 5d29 0d0a 2020 2020 2020 2020  *3+1])..        
-0000d1a0: 2020 2020 7461 626c 6531 2e61 7070 656e      table1.appen
-0000d1b0: 6428 746d 7029 0d0a 2020 2020 2020 2020  d(tmp)..        
-0000d1c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000d1d0: 2020 2074 6d70 203d 205b 2750 6861 7365     tmp = ['Phase
-0000d1e0: 3027 2c20 2730 2e30 2028 272b 7374 7228  0', '0.0 ('+str(
-0000d1f0: 6e70 2e72 6f75 6e64 2872 6573 5b6e 6d65  np.round(res[nme
-0000d200: 742a 332b 305d 2c31 2929 2b27 2927 5d0d  t*3+0],1))+')'].
-0000d210: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d220: 646f 5f63 7261 6f3a 2074 6d70 2e61 7070  do_crao: tmp.app
-0000d230: 656e 6428 6372 616f 5b6e 6d65 742a 332b  end(crao[nmet*3+
-0000d240: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
-0000d250: 2069 6620 646f 5f63 6f6e 663a 2074 6d70   if do_conf: tmp
-0000d260: 2e61 7070 656e 6428 636f 6e66 5b6e 6d65  .append(conf[nme
-0000d270: 742a 332b 305d 290d 0a20 2020 2020 2020  t*3+0])..       
-0000d280: 2020 2020 2074 6162 6c65 312e 6170 7065       table1.appe
-0000d290: 6e64 2874 6d70 290d 0a20 2020 200d 0a20  nd(tmp)..    .. 
-0000d2a0: 2020 2020 2020 2020 2020 2074 6d70 203d             tmp =
-0000d2b0: 205b 2750 6861 7365 3127 2c20 2730 2e30   ['Phase1', '0.0
-0000d2c0: 2028 272b 7374 7228 6e70 2e72 6f75 6e64   ('+str(np.round
-0000d2d0: 2872 6573 5b6e 6d65 742a 332b 315d 2c31  (res[nmet*3+1],1
-0000d2e0: 2929 2b27 2927 5d0d 0a20 2020 2020 2020  ))+')']..       
-0000d2f0: 2020 2020 2069 6620 646f 5f63 7261 6f3a       if do_crao:
-0000d300: 2074 6d70 2e61 7070 656e 6428 6372 616f   tmp.append(crao
-0000d310: 5b6e 6d65 742a 332b 315d 290d 0a20 2020  [nmet*3+1])..   
-0000d320: 2020 2020 2020 2020 2069 6620 646f 5f63           if do_c
-0000d330: 6f6e 663a 2074 6d70 2e61 7070 656e 6428  onf: tmp.append(
-0000d340: 636f 6e66 5b6e 6d65 742a 332b 315d 290d  conf[nmet*3+1]).
-0000d350: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-0000d360: 6c65 312e 6170 7065 6e64 2874 6d70 290d  le1.append(tmp).
-0000d370: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000d380: 2020 2020 2020 206e 7365 6374 2e61 7070         nsect.app
-0000d390: 656e 6428 6c65 6e28 7461 626c 6531 2929  end(len(table1))
-0000d3a0: 0d0a 2020 2020 2020 2020 7461 626c 6531  ..        table1
-0000d3b0: 2e61 7070 656e 6428 6864 7234 290d 0a0d  .append(hdr4)...
-0000d3c0: 0a20 2020 2020 2020 2074 6d70 203d 205b  .        tmp = [
-0000d3d0: 2743 6869 5371 7561 7265 272c 2073 7461  'ChiSquare', sta
-0000d3e0: 7473 5b30 5d5d 0d0a 2020 2020 2020 2020  ts[0]]..        
-0000d3f0: 6966 2064 6f5f 6372 616f 3a20 746d 702e  if do_crao: tmp.
-0000d400: 6170 7065 6e64 2827 2027 290d 0a20 2020  append(' ')..   
-0000d410: 2020 2020 2069 6620 646f 5f63 6f6e 663a       if do_conf:
-0000d420: 2074 6d70 2e61 7070 656e 6428 2720 2729   tmp.append(' ')
-0000d430: 0d0a 2020 2020 2020 2020 7461 626c 6531  ..        table1
-0000d440: 2e61 7070 656e 6428 746d 7029 0d0a 2020  .append(tmp)..  
-0000d450: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000d460: 746d 7020 3d20 5b27 5765 6967 6874 6564  tmp = ['Weighted
-0000d470: 2043 6869 5371 7561 7265 272c 2073 7461   ChiSquare', sta
-0000d480: 7473 5b31 5d5d 0d0a 2020 2020 2020 2020  ts[1]]..        
-0000d490: 6966 2064 6f5f 6372 616f 3a20 746d 702e  if do_crao: tmp.
-0000d4a0: 6170 7065 6e64 2827 2027 290d 0a20 2020  append(' ')..   
-0000d4b0: 2020 2020 2069 6620 646f 5f63 6f6e 663a       if do_conf:
-0000d4c0: 2074 6d70 2e61 7070 656e 6428 2720 2729   tmp.append(' ')
-0000d4d0: 0d0a 2020 2020 2020 2020 7461 626c 6531  ..        table1
-0000d4e0: 2e61 7070 656e 6428 746d 7029 0d0a 0d0a  .append(tmp)....
-0000d4f0: 2020 2020 2020 2020 6d61 7468 6572 7220          matherr 
-0000d500: 3d20 7374 7228 7374 6174 735b 325d 2021  = str(stats[2] !
-0000d510: 3d20 3029 0d0a 2020 2020 2020 2020 746d  = 0)..        tm
-0000d520: 7020 3d20 5b27 4d61 7468 2046 696e 6974  p = ['Math Finit
-0000d530: 6520 4572 726f 7227 2c20 6d61 7468 6572  e Error', mather
-0000d540: 725d 0d0a 2020 2020 2020 2020 6966 2064  r]..        if d
-0000d550: 6f5f 6372 616f 3a20 746d 702e 6170 7065  o_crao: tmp.appe
-0000d560: 6e64 2827 2027 290d 0a20 2020 2020 2020  nd(' ')..       
-0000d570: 2069 6620 646f 5f63 6f6e 663a 2074 6d70   if do_conf: tmp
-0000d580: 2e61 7070 656e 6428 2720 2729 0d0a 2020  .append(' ')..  
-0000d590: 2020 2020 2020 7461 626c 6531 2e61 7070        table1.app
-0000d5a0: 656e 6428 746d 7029 0d0a 2020 2020 2020  end(tmp)..      
-0000d5b0: 2020 0d0a 2020 2020 2020 2020 7461 626c    ..        tabl
-0000d5c0: 6531 203d 205f 7072 6574 7479 5f73 7061  e1 = _pretty_spa
-0000d5d0: 6365 5f74 6162 6c65 5f69 6e70 6c61 6365  ce_table_inplace
-0000d5e0: 2874 6162 6c65 312c 2070 6c61 6365 733d  (table1, places=
-0000d5f0: 3529 0d0a 0d0a 2020 2020 2020 2020 7265  5)....        re
-0000d600: 7475 726e 2074 6162 6c65 312c 206e 7365  turn table1, nse
-0000d610: 6374 0d0a 2020 2020 0d0a 200d 0a         ct..    .. ..
+00005310: 2020 2022 6f70 7469 6d69 7a65 5f77 6569     "optimize_wei
+00005320: 6768 7473 5f6d 6574 686f 6422 2c0d 0a20  ghts_method",.. 
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
+00005350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005360: 6974 656d 203d 2073 6f75 7263 652e 6669  item = source.fi
+00005370: 6e64 7465 7874 2861 7474 7269 6275 7465  ndtext(attribute
+00005380: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005390: 2020 2069 6620 6974 656d 2069 7320 6e6f     if item is no
+000053a0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+000053b0: 2020 2020 2020 2020 2020 2020 2073 6574               set
+000053c0: 6174 7472 2873 656c 662c 2061 7474 7269  attr(self, attri
+000053d0: 6275 7465 2c20 6974 656d 290d 0a0d 0a20  bute, item).... 
+000053e0: 2020 2020 2020 2020 2020 2023 206c 6973             # lis
+000053f0: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
+00005400: 7365 6c66 2e70 7269 6f72 5f6c 6973 7420  self.prior_list 
+00005410: 2020 2020 2020 3d20 5b76 616c 2e74 6578        = [val.tex
+00005420: 7420 666f 7220 7661 6c20 696e 2073 6f75  t for val in sou
+00005430: 7263 652e 6765 7469 7465 7261 746f 7228  rce.getiterator(
+00005440: 2270 7269 6f72 5f6c 6973 7422 295d 0d0a  "prior_list")]..
+00005450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005460: 2e70 7269 6f72 5f61 7265 615f 7363 616c  .prior_area_scal
+00005470: 6520 3d20 5b66 6c6f 6174 2876 616c 2e74  e = [float(val.t
+00005480: 6578 7429 2066 6f72 2076 616c 2069 6e20  ext) for val in 
+00005490: 736f 7572 6365 2e67 6574 6974 6572 6174  source.getiterat
+000054a0: 6f72 2822 7072 696f 725f 6172 6561 5f73  or("prior_area_s
+000054b0: 6361 6c65 2229 5d0d 0a20 2020 2020 2020  cale")]..       
+000054c0: 2020 2020 2073 656c 662e 7072 696f 725f       self.prior_
+000054d0: 7065 616b 5f70 706d 2020 203d 205b 666c  peak_ppm   = [fl
+000054e0: 6f61 7428 7661 6c2e 7465 7874 2920 666f  oat(val.text) fo
+000054f0: 7220 7661 6c20 696e 2073 6f75 7263 652e  r val in source.
+00005500: 6765 7469 7465 7261 746f 7228 2270 7269  getiterator("pri
+00005510: 6f72 5f70 6561 6b5f 7070 6d22 295d 0d0a  or_peak_ppm")]..
+00005520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005530: 2e70 7269 6f72 5f73 6561 7263 685f 7070  .prior_search_pp
+00005540: 6d20 3d20 5b66 6c6f 6174 2876 616c 2e74  m = [float(val.t
+00005550: 6578 7429 2066 6f72 2076 616c 2069 6e20  ext) for val in 
+00005560: 736f 7572 6365 2e67 6574 6974 6572 6174  source.getiterat
+00005570: 6f72 2822 7072 696f 725f 7365 6172 6368  or("prior_search
+00005580: 5f70 706d 2229 5d0d 0a20 2020 2020 2020  _ppm")]..       
+00005590: 2020 2020 2073 656c 662e 7072 696f 725f       self.prior_
+000055a0: 6462 5f70 706d 2020 2020 203d 205b 7574  db_ppm     = [ut
+000055b0: 696c 5f78 6d6c 2e42 4f4f 4c45 414e 535b  il_xml.BOOLEANS[
+000055c0: 7661 6c2e 7465 7874 5d20 666f 7220 7661  val.text] for va
+000055d0: 6c20 696e 2073 6f75 7263 652e 6765 7469  l in source.geti
+000055e0: 7465 7261 746f 7228 2270 7269 6f72 5f64  terator("prior_d
+000055f0: 625f 7070 6d22 295d 0d0a 2020 2020 2020  b_ppm")]..      
+00005600: 2020 2020 2020 7365 6c66 2e70 7269 6f72        self.prior
+00005610: 5f66 6978 5f74 3220 2020 2020 3d20 5b66  _fix_t2     = [f
+00005620: 6c6f 6174 2876 616c 2e74 6578 7429 2066  loat(val.text) f
+00005630: 6f72 2076 616c 2069 6e20 736f 7572 6365  or val in source
+00005640: 2e67 6574 6974 6572 6174 6f72 2822 7072  .getiterator("pr
+00005650: 696f 725f 6669 785f 7432 2229 5d0d 0a20  ior_fix_t2")].. 
+00005660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005670: 7072 696f 725f 7365 6172 6368 5f70 6830  prior_search_ph0
+00005680: 203d 205b 666c 6f61 7428 7661 6c2e 7465   = [float(val.te
+00005690: 7874 2920 666f 7220 7661 6c20 696e 2073  xt) for val in s
+000056a0: 6f75 7263 652e 6765 7469 7465 7261 746f  ource.getiterato
+000056b0: 7228 2270 7269 6f72 5f73 6561 7263 685f  r("prior_search_
+000056c0: 7068 3022 295d 0d0a 2020 2020 2020 2020  ph0")]..        
+000056d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000056e0: 2020 6e6d 6574 203d 206c 656e 2873 656c    nmet = len(sel
+000056f0: 662e 7072 696f 725f 6c69 7374 290d 0a20  f.prior_list).. 
+00005700: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00005710: 7420 7365 6c66 2e70 7269 6f72 5f61 7265  t self.prior_are
+00005720: 615f 7363 616c 653a 0d0a 2020 2020 2020  a_scale:..      
+00005730: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00005740: 7269 6f72 5f61 7265 615f 7363 616c 6520  rior_area_scale 
+00005750: 3d20 5b31 2e30 2066 6f72 2069 2069 6e20  = [1.0 for i in 
+00005760: 7261 6e67 6528 6e6d 6574 295d 0d0a 2020  range(nmet)]..  
+00005770: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00005780: 2073 656c 662e 7072 696f 725f 7365 6172   self.prior_sear
+00005790: 6368 5f70 706d 3a0d 0a20 2020 2020 2020  ch_ppm:..       
+000057a0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+000057b0: 696f 725f 7365 6172 6368 5f70 706d 203d  ior_search_ppm =
+000057c0: 205b 302e 3120 666f 7220 6920 696e 2072   [0.1 for i in r
+000057d0: 616e 6765 286e 6d65 7429 5d0d 0a20 2020  ange(nmet)]..   
+000057e0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000057f0: 7365 6c66 2e70 7269 6f72 5f64 625f 7070  self.prior_db_pp
+00005800: 6d3a 0d0a 2020 2020 2020 2020 2020 2020  m:..            
+00005810: 2020 2020 7365 6c66 2e70 7269 6f72 5f64      self.prior_d
+00005820: 625f 7070 6d20 3d20 5b46 616c 7365 2066  b_ppm = [False f
+00005830: 6f72 2069 2069 6e20 7261 6e67 6528 6e6d  or i in range(nm
+00005840: 6574 295d 0d0a 2020 2020 2020 2020 2020  et)]..          
+00005850: 2020 6966 206e 6f74 2073 656c 662e 7072    if not self.pr
+00005860: 696f 725f 6669 785f 7432 3a0d 0a20 2020  ior_fix_t2:..   
+00005870: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005880: 662e 7072 696f 725f 6669 785f 7432 203d  f.prior_fix_t2 =
+00005890: 205b 3130 3030 2e30 2066 6f72 2069 2069   [1000.0 for i i
+000058a0: 6e20 7261 6e67 6528 6e6d 6574 295d 0d0a  n range(nmet)]..
+000058b0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+000058c0: 6f74 2073 656c 662e 7072 696f 725f 7365  ot self.prior_se
+000058d0: 6172 6368 5f70 6830 3a0d 0a20 2020 2020  arch_ph0:..     
+000058e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000058f0: 7072 696f 725f 7365 6172 6368 5f70 6830  prior_search_ph0
+00005900: 203d 205b 302e 3020 666f 7220 6920 696e   = [0.0 for i in
+00005910: 2072 616e 6765 286e 6d65 7429 5d0d 0a0d   range(nmet)]...
+00005920: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005930: 662e 7072 696f 725f 7872 616e 6765 2020  f.prior_xrange  
+00005940: 2020 203d 205b 696e 7428 7661 6c2e 7465     = [int(val.te
+00005950: 7874 2920 666f 7220 7661 6c20 696e 2073  xt) for val in s
+00005960: 6f75 7263 652e 6765 7469 7465 7261 746f  ource.getiterato
+00005970: 7228 2270 7269 6f72 5f78 7261 6e67 6522  r("prior_xrange"
+00005980: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+00005990: 7365 6c66 2e70 7269 6f72 5f79 7261 6e67  self.prior_yrang
+000059a0: 6520 2020 2020 3d20 5b69 6e74 2876 616c  e     = [int(val
+000059b0: 2e74 6578 7429 2066 6f72 2076 616c 2069  .text) for val i
+000059c0: 6e20 736f 7572 6365 2e67 6574 6974 6572  n source.getiter
+000059d0: 6174 6f72 2822 7072 696f 725f 7972 616e  ator("prior_yran
+000059e0: 6765 2229 5d0d 0a20 2020 2020 2020 2020  ge")]..         
+000059f0: 2020 2073 656c 662e 7072 696f 725f 7a72     self.prior_zr
+00005a00: 616e 6765 2020 2020 203d 205b 696e 7428  ange     = [int(
+00005a10: 7661 6c2e 7465 7874 2920 666f 7220 7661  val.text) for va
+00005a20: 6c20 696e 2073 6f75 7263 652e 6765 7469  l in source.geti
+00005a30: 7465 7261 746f 7228 2270 7269 6f72 5f7a  terator("prior_z
+00005a40: 7261 6e67 6522 295d 0d0a 2020 2020 2020  range")]..      
+00005a50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005a60: 2020 2020 2320 7375 626f 626a 6563 7473      # subobjects
+00005a70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00005a80: 6c66 2e70 7269 6f72 203d 206d 7273 5f70  lf.prior = mrs_p
+00005a90: 7269 6f72 2e50 7269 6f72 2873 6f75 7263  rior.Prior(sourc
+00005aa0: 652e 6669 6e64 2822 7072 696f 7222 2929  e.find("prior"))
+00005ab0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00005ac0: 0d0a 2020 2020 2020 2020 656c 6966 2068  ..        elif h
+00005ad0: 6173 6174 7472 2873 6f75 7263 652c 2022  asattr(source, "
+00005ae0: 6b65 7973 2229 3a0d 0a20 2020 2020 2020  keys"):..       
+00005af0: 2020 2020 2023 2051 7561 636b 7320 6c69       # Quacks li
+00005b00: 6b65 2061 2064 6963 740d 0a20 2020 2020  ke a dict..     
+00005b10: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
+00005b20: 6e20 6c69 7374 2873 6f75 7263 652e 6b65  n list(source.ke
+00005b30: 7973 2829 293a 0d0a 2020 2020 2020 2020  ys()):..        
+00005b40: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+00005b50: 7472 2873 656c 662c 206b 6579 293a 0d0a  tr(self, key):..
+00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b70: 2020 2020 7365 7461 7474 7228 7365 6c66      setattr(self
+00005b80: 2c20 6b65 792c 2073 6f75 7263 655b 6b65  , key, source[ke
+00005b90: 795d 290d 0a0d 0a0d 0a0d 0a0d 0a63 6c61  y])..........cla
+00005ba0: 7373 2042 6c6f 636b 4669 7447 6973 6f28  ss BlockFitGiso(
+00005bb0: 626c 6f63 6b5f 6669 745f 6964 656e 7469  block_fit_identi
+00005bc0: 7479 2e42 6c6f 636b 4669 7449 6465 6e74  ty.BlockFitIdent
+00005bd0: 6974 7929 3a0d 0a20 2020 2022 2222 200d  ity):..    """ .
+00005be0: 0a20 2020 2042 7569 6c64 696e 6720 626c  .    Building bl
+00005bf0: 6f63 6b20 746f 2068 6f6c 6420 7468 6520  ock to hold the 
+00005c00: 7374 6174 6520 6f66 2061 2073 7465 7020  state of a step 
+00005c10: 696e 2061 6e20 4d52 5320 7072 6f63 6573  in an MRS proces
+00005c20: 7369 6e67 2063 6861 696e 2e0d 0a20 2020  sing chain...   
+00005c30: 2049 6e63 6c75 6465 7320 7468 6520 6675   Includes the fu
+00005c40: 6e63 7469 6f6e 616c 6974 7920 746f 2073  nctionality to s
+00005c50: 6176 652f 7265 6361 6c6c 2074 6869 7320  ave/recall this 
+00005c60: 6f62 6a65 6374 2074 6f2f 6672 6f6d 2061  object to/from a
+00005c70: 6e20 584d 4c20 6e6f 6465 2e0d 0a0d 0a20  n XML node..... 
+00005c80: 2020 2043 6f6e 7461 696e 7320 696e 7075     Contains inpu
+00005c90: 7473 2f72 6573 756c 7473 2066 6f72 2063  ts/results for c
+00005ca0: 6f6e 7665 7274 696e 6720 7468 6520 6669  onverting the fi
+00005cb0: 7474 6564 206d 6574 6162 6f6c 6974 6520  tted metabolite 
+00005cc0: 6172 6561 7320 746f 200d 0a20 2020 2063  areas to ..    c
+00005cd0: 6f6e 6365 6e74 7261 7469 6f6e 2076 616c  oncentration val
+00005ce0: 7565 732e 0d0a 2020 2020 0d0a 2020 2020  ues...    ..    
+00005cf0: 2222 220d 0a20 2020 2058 4d4c 5f56 4552  """..    XML_VER
+00005d00: 5349 4f4e 203d 2022 312e 302e 3022 0d0a  SION = "1.0.0"..
+00005d10: 2020 2020 0d0a 2020 2020 6465 6620 5f5f      ..    def __
+00005d20: 696e 6974 5f5f 2873 656c 662c 2061 7474  init__(self, att
+00005d30: 7269 6275 7465 733d 4e6f 6e65 293a 0d0a  ributes=None):..
+00005d40: 2020 2020 2020 2020 2222 220d 0a0d 0a20          """.... 
+00005d50: 2020 2020 2020 2047 656e 6572 616c 2050         General P
+00005d60: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+00005d70: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00005d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ------------....
+00005da0: 2020 2020 2020 2020 6964 2020 2020 2020          id      
+00005db0: 2020 2020 4120 7065 726d 616e 656e 742c      A permanent,
+00005dc0: 2075 6e69 7175 6520 6964 656e 7469 6679   unique identify
+00005dd0: 696e 6720 7374 7269 6e67 2066 6f72 2074  ing string for t
+00005de0: 6869 7320 0d0a 2020 2020 2020 2020 2020  his ..          
+00005df0: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+00005e00: 2e20 5479 7069 6361 6c6c 7920 7365 7276  . Typically serv
+00005e10: 6573 2061 7320 6120 2273 6f75 7263 655f  es as a "source_
+00005e20: 6964 2220 666f 7220 0d0a 2020 2020 2020  id" for ..      
+00005e30: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00005e40: 6d65 206f 7468 6572 206f 626a 6563 742e  me other object.
+00005e50: 2049 7420 6973 2070 6172 7420 6f66 2074   It is part of t
+00005e60: 6865 2070 726f 7665 6e61 6e63 650d 0a20  he provenance.. 
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2066 6f72 2074 6869 7320 7072 6f63     for this proc
+00005e90: 6573 7369 6e67 2066 756e 6374 6f72 2063  essing functor c
+00005ea0: 6861 696e 0d0a 2020 2020 2020 2020 2020  hain..          
+00005eb0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00005ec0: 2020 2073 6f75 7263 655f 6964 2020 2054     source_id   T
+00005ed0: 6865 2075 6e69 7175 6520 6964 656e 7469  he unique identi
+00005ee0: 6669 6572 2075 7365 6420 746f 2066 696e  fier used to fin
+00005ef0: 6420 7468 6520 696e 7075 7420 6461 7461  d the input data
+00005f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005f10: 2020 2020 2020 666f 7220 7468 6973 206f        for this o
+00005f20: 626a 6563 742e 2049 7420 6d61 7920 7265  bject. It may re
+00005f30: 6665 7220 746f 206f 6e65 2077 686f 6c65  fer to one whole
+00005f40: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
+00005f50: 2020 2020 2020 2020 2020 2020 2074 6861               tha
+00005f60: 7420 6861 7320 6f6e 6c79 206f 6e65 2072  t has only one r
+00005f70: 6573 756c 742c 204f 5220 6974 2063 6f75  esult, OR it cou
+00005f80: 6c64 2072 6566 6572 2074 6f20 730d 0a20  ld refer to s.. 
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2073 696e 676c 6520 7265 7375 6c74     single result
+00005fb0: 7320 696e 7369 6465 2061 6e20 6f62 6a65  s inside an obje
+00005fc0: 6374 2074 6861 7420 6861 7320 6d75 6c74  ct that has mult
+00005fd0: 6970 6c65 0d0a 2020 2020 2020 2020 2020  iple..          
+00005fe0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00005ff0: 732e 0d0a 0d0a 2020 2020 2020 2020 2222  s.....        ""
+00006000: 2220 2020 2020 2020 200d 0a20 2020 2020  "        ..     
+00006010: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00006020: 745f 5f28 6174 7472 6962 7574 6573 290d  t__(attributes).
+00006030: 0a0d 0a20 2020 2020 2020 2023 2d2d 2d2d  ...        #----
+00006040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006060: 2d2d 2d2d 0d0a 2020 2020 2020 2020 2320  ----..        # 
+00006070: 4749 534f 2061 6c67 6f72 6974 686d 2069  GISO algorithm i
+00006080: 6e70 7574 2073 6574 7469 6e67 730d 0a20  nput settings.. 
+00006090: 2020 2020 2020 2073 656c 662e 7365 7420         self.set 
+000060a0: 3d20 5f53 6574 7469 6e67 7328 290d 0a20  = _Settings().. 
+000060b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000060c0: 2023 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   #--------------
+000060d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000060e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+000060f0: 2020 2020 2320 4749 534f 2072 6573 756c      # GISO resul
+00006100: 7420 6f62 6a65 6374 730d 0a20 2020 2020  t objects..     
+00006110: 2020 2073 656c 662e 6669 745f 7265 7375     self.fit_resu
+00006120: 6c74 7320 2020 2020 2020 203d 204e 6f6e  lts        = Non
+00006130: 6520 2020 2020 2023 2066 6974 2070 6172  e      # fit par
+00006140: 616d 6574 6572 7320 6672 6f6d 206f 7074  ameters from opt
+00006150: 696d 697a 6174 696f 6e0d 0a20 2020 2020  imization..     
+00006160: 2020 2073 656c 662e 6669 745f 7374 6174     self.fit_stat
+00006170: 7320 2020 2020 2020 2020 203d 204e 6f6e  s          = Non
+00006180: 6520 2020 2020 2023 2073 7461 7473 2066  e      # stats f
+00006190: 726f 6d20 7468 6520 6f70 7469 6d69 7a61  rom the optimiza
+000061a0: 7469 6f6e 2066 6f72 2065 6163 6820 766f  tion for each vo
+000061b0: 7865 6c0d 0a20 2020 2020 2020 2073 656c  xel..        sel
+000061c0: 662e 6669 745f 6261 7365 6c69 6e65 2020  f.fit_baseline  
+000061d0: 2020 2020 203d 204e 6f6e 6520 2020 2020       = None     
+000061e0: 2023 2062 6173 656c 696e 6520 7265 7375   # baseline resu
+000061f0: 6c74 2028 6d61 7920 6265 2076 6563 746f  lt (may be vecto
+00006200: 7220 6f72 2070 6172 616d 6574 6572 697a  r or parameteriz
+00006210: 6564 290d 0a20 2020 2020 2020 2073 656c  ed)..        sel
+00006220: 662e 636f 6e66 6964 656e 6365 2020 2020  f.confidence    
+00006230: 2020 2020 203d 204e 6f6e 6520 2020 2020       = None     
+00006240: 2023 2063 6f6e 6669 6465 6e63 6520 6c69   # confidence li
+00006250: 6d69 7473 2072 6573 756c 7473 2073 746f  mits results sto
+00006260: 7261 6765 0d0a 2020 2020 2020 2020 7365  rage..        se
+00006270: 6c66 2e63 7261 6d65 725f 7261 6f20 2020  lf.cramer_rao   
+00006280: 2020 2020 2020 3d20 4e6f 6e65 2020 2020        = None    
+00006290: 2020 2320 6372 616d 6572 2d72 616f 2062    # cramer-rao b
+000062a0: 6f75 6e64 7320 7265 7375 6c74 7320 7374  ounds results st
+000062b0: 6f72 6167 650d 0a20 2020 2020 2020 2073  orage..        s
+000062c0: 656c 662e 696e 6974 6961 6c5f 7661 6c75  elf.initial_valu
+000062d0: 6573 2020 2020 203d 204e 6f6e 6520 2020  es     = None   
+000062e0: 2020 2023 2069 6e69 7469 616c 2076 616c     # initial val
+000062f0: 7565 7320 666f 7220 6d65 7461 6220 6f70  ues for metab op
+00006300: 7469 6d69 7a61 7469 6f6e 2020 200d 0a20  timization   .. 
+00006310: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
+00006320: 725f 6d61 736b 2020 2020 2020 2020 203d  r_mask         =
+00006330: 204e 6f6e 650d 0a0d 0a20 2020 2020 2020   None....       
+00006340: 2069 6620 6174 7472 6962 7574 6573 2069   if attributes i
+00006350: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00006360: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+00006370: 666c 6174 6528 6174 7472 6962 7574 6573  flate(attributes
+00006380: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+00006390: 662e 6368 6169 6e20 3d20 4e6f 6e65 0d0a  f.chain = None..
+000063a0: 0d0a 0d0a 2020 2020 2323 2323 2320 5374  ....    ##### St
+000063b0: 616e 6461 7264 204d 6574 686f 6473 2061  andard Methods a
+000063c0: 6e64 2050 726f 7065 7274 6965 7320 2323  nd Properties ##
+000063d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000063e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000063f0: 2323 230d 0a0d 0a20 2020 2040 7072 6f70  ###....    @prop
+00006400: 6572 7479 0d0a 2020 2020 6465 6620 6461  erty..    def da
+00006410: 7461 2873 656c 6629 3a0d 0a20 2020 2020  ta(self):..     
+00006420: 2020 2073 656c 662e 6669 745f 7265 7375     self.fit_resu
+00006430: 6c74 730d 0a0d 0a0d 0a20 2020 2040 7072  lts......    @pr
+00006440: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00006450: 6469 6d73 2873 656c 6629 3a0d 0a20 2020  dims(self):..   
+00006460: 2020 2020 2022 2222 4469 6d65 6e73 696f       """Dimensio
+00006470: 6e73 2066 6f72 2066 6974 7469 6e67 2072  ns for fitting r
+00006480: 6573 756c 7473 2069 6e20 6120 6c69 7374  esults in a list
+00006490: 2c20 7265 6164 206f 6e6c 792e 2222 220d  , read only.""".
+000064a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000064b0: 6c69 7374 2873 656c 662e 6669 745f 7265  list(self.fit_re
+000064c0: 7375 6c74 732e 7368 6170 6529 2069 6620  sults.shape) if 
+000064d0: 7365 6c66 2e66 6974 5f72 6573 756c 7473  self.fit_results
+000064e0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+000064f0: 6520 4e6f 6e65 0d0a 0d0a 0d0a 2020 2020  e None......    
+00006500: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00006510: 6566 206e 7061 7261 6d28 7365 6c66 293a  ef nparam(self):
+00006520: 0d0a 2020 2020 2020 2020 6e70 6172 616d  ..        nparam
+00006530: 203d 206c 656e 2873 656c 662e 7365 742e   = len(self.set.
+00006540: 7072 696f 725f 6c69 7374 292a 332b 3220  prior_list)*3+2 
+00006550: 2b20 7365 6c66 2e6e 6d6d 6f6c 0d0a 2020  + self.nmmol..  
+00006560: 2020 2020 2020 7265 7475 726e 206e 7061        return npa
+00006570: 7261 6d20 200d 0a20 2020 2020 2020 200d  ram  ..        .
+00006580: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00006590: 2020 2020 6465 6620 6e6d 6d6f 6c28 7365      def nmmol(se
+000065a0: 6c66 293a 0d0a 2020 2020 2020 2020 6e6d  lf):..        nm
+000065b0: 6d6f 6c20 3d20 300d 0a20 2020 2020 2020  mol = 0..       
+000065c0: 2069 6620 7365 6c66 2e73 6574 2e6d 6163   if self.set.mac
+000065d0: 726f 6d6f 6c5f 6d6f 6465 6c20 3d3d 2046  romol_model == F
+000065e0: 6974 4d61 6372 6f6d 6f6c 6563 756c 654d  itMacromoleculeM
+000065f0: 6574 686f 642e 5349 4e47 4c45 5f42 4153  ethod.SINGLE_BAS
+00006600: 4953 5f44 4154 4153 4554 3a0d 0a20 2020  IS_DATASET:..   
+00006610: 2020 2020 2020 2020 206e 6d6d 6f6c 202b           nmmol +
+00006620: 3d20 320d 0a20 2020 2020 2020 2072 6574  = 2..        ret
+00006630: 7572 6e20 6e6d 6d6f 6c0d 0a20 2020 2020  urn nmmol..     
+00006640: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
+00006650: 5f73 7472 5f5f 2873 656c 6629 3a0d 0a20  _str__(self):.. 
+00006660: 2020 2020 2020 206c 696e 6573 203d 205b         lines = [
+00006670: 5d0d 0a20 2020 2020 2020 206c 696e 6573  ]..        lines
+00006680: 2e61 7070 656e 6428 222d 2d2d 2d2d 2d2d  .append("-------
+00006690: 207b 307d 204f 626a 6563 7420 2d2d 2d2d   {0} Object ----
+000066a0: 2d2d 2d22 2e66 6f72 6d61 7428 7365 6c66  ---".format(self
+000066b0: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+000066c0: 655f 5f29 290d 0a20 2020 2020 2020 206c  e__))..        l
+000066d0: 696e 6573 2e61 7070 656e 6428 225c 6e22  ines.append("\n"
+000066e0: 290d 0a20 2020 2020 2020 206c 696e 6573  )..        lines
+000066f0: 202b 3d20 5f53 6574 7469 6e67 732e 5f5f   += _Settings.__
+00006700: 7374 725f 5f28 7365 6c66 292e 7370 6c69  str__(self).spli
+00006710: 7428 275c 6e27 290d 0a20 2020 2020 2020  t('\n')..       
+00006720: 206c 696e 6573 2e61 7070 656e 6428 225c   lines.append("\
+00006730: 6e22 290d 0a20 2020 2020 2020 206c 696e  n")..        lin
+00006740: 6573 2e61 7070 656e 6428 222d 2d2d 2d2d  es.append("-----
+00006750: 2d2d 204d 6169 6e20 4f62 6a65 6374 202d  -- Main Object -
+00006760: 2d2d 2d2d 2d2d 2229 0d0a 2020 2020 2020  ------")..      
+00006770: 2020 6c69 6e65 732e 6170 7065 6e64 2822    lines.append("
+00006780: 4e6f 2061 6464 6974 696f 6e61 6c20 6461  No additional da
+00006790: 7461 2229 0d0a 2020 2020 2020 2020 7265  ta")..        re
+000067a0: 7475 726e 206c 696e 6573 0d0a 2020 2020  turn lines..    
+000067b0: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+000067c0: 6372 6561 7465 5f63 6861 696e 2873 656c  create_chain(sel
+000067d0: 662c 2064 6174 6173 6574 293a 0d0a 2020  f, dataset):..  
+000067e0: 2020 2020 2020 7365 6c66 2e63 6861 696e        self.chain
+000067f0: 203d 2063 6861 696e 5f66 6974 5f67 6973   = chain_fit_gis
+00006800: 6f2e 4368 6169 6e46 6974 4769 736f 2864  o.ChainFitGiso(d
+00006810: 6174 6173 6574 2c20 7365 6c66 290d 0a0d  ataset, self)...
+00006820: 0a0d 0a20 2020 2064 6566 2073 6574 5f64  ...    def set_d
+00006830: 696d 7328 7365 6c66 2c20 6461 7461 7365  ims(self, datase
+00006840: 7429 3a0d 0a20 2020 2020 2020 2022 2222  t):..        """
+00006850: 0d0a 2020 2020 2020 2020 4769 7665 6e20  ..        Given 
+00006860: 6120 4461 7461 7365 7420 6f62 6a65 6374  a Dataset object
+00006870: 2c20 7468 6973 2069 7320 616e 206f 7070  , this is an opp
+00006880: 6f72 7475 6e69 7479 2066 6f72 2074 6869  ortunity for thi
+00006890: 7320 626c 6f63 6b20 6f62 6a65 6374 200d  s block object .
+000068a0: 0a20 2020 2020 2020 2074 6f20 656e 7375  .        to ensu
+000068b0: 7265 2074 6861 7420 6974 7320 7265 7375  re that its resu
+000068c0: 6c74 7320 6469 6d73 206d 6174 6368 2074  lts dims match t
+000068d0: 686f 7365 206f 6620 7468 6520 7061 7265  hose of the pare
+000068e0: 6e74 2064 6174 6173 6574 2e0d 0a20 2020  nt dataset...   
+000068f0: 2020 2020 2042 6563 6175 7365 2074 6865       Because the
+00006900: 2066 6974 7469 6e67 2072 6573 756c 7473   fitting results
+00006910: 2061 7265 2070 6172 616d 6574 6572 732c   are parameters,
+00006920: 2074 6865 7920 646f 206e 6f74 2068 6176   they do not hav
+00006930: 6520 746f 206d 6174 6368 0d0a 2020 2020  e to match..    
+00006940: 2020 2020 696e 2074 6865 2073 7065 6374      in the spect
+00006950: 7261 6c20 6469 6d65 6e73 696f 6e73 2c20  ral dimensions, 
+00006960: 6a75 7374 2069 6e20 7468 6520 7370 6174  just in the spat
+00006970: 6961 6c20 6469 6d65 6e73 696f 6e73 2e20  ial dimensions. 
+00006980: 4275 742c 2077 6520 0d0a 2020 2020 2020  But, we ..      
+00006990: 2020 6861 7665 2074 6f20 6361 6c63 756c    have to calcul
+000069a0: 6174 6520 7468 6520 7061 7261 6d65 7465  ate the paramete
+000069b0: 7220 6469 6d65 6e73 696f 6e20 7369 7a65  r dimension size
+000069c0: 2066 726f 6d20 6375 7272 656e 7420 7365   from current se
+000069d0: 7474 696e 6773 0d0a 2020 2020 2020 2020  ttings..        
+000069e0: 746f 2063 6f6d 7061 7265 2074 6f20 7468  to compare to th
+000069f0: 6520 6578 6973 6974 696e 6720 6172 7261  e exisiting arra
+00006a00: 7920 6469 6d65 6e73 696f 6e73 2e0d 0a20  y dimensions... 
+00006a10: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00006a20: 2020 2020 6966 2073 656c 662e 6469 6d73      if self.dims
+00006a30: 2069 7320 4e6f 6e65 206f 7220 7365 6c66   is None or self
+00006a40: 2e66 6974 5f62 6173 656c 696e 6520 6973  .fit_baseline is
+00006a50: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00006a60: 2020 2020 2320 6e65 6564 2074 6869 7320      # need this 
+00006a70: 6865 7265 2066 6f72 2069 6e69 7469 616c  here for initial
+00006a80: 697a 6174 696f 6e0d 0a20 2020 2020 2020  ization..       
+00006a90: 2020 2020 2073 656c 662e 5f72 6573 6574       self._reset
+00006aa0: 5f64 696d 656e 7369 6f6e 616c 5f64 6174  _dimensional_dat
+00006ab0: 6128 6461 7461 7365 7429 0d0a 2020 2020  a(dataset)..    
+00006ac0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006ad0: 6368 6169 6e20 6973 206e 6f74 204e 6f6e  chain is not Non
+00006ae0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00006af0: 2020 2020 7365 6c66 2e63 6861 696e 2e72      self.chain.r
+00006b00: 6573 6574 5f72 6573 756c 7473 5f61 7272  eset_results_arr
+00006b10: 6179 7328 290d 0a20 2020 2020 2020 2065  ays()..        e
+00006b20: 6c73 653a 0d0a 2020 2020 0d0a 2020 2020  lse:..    ..    
+00006b30: 2020 2020 2020 2020 2320 5072 696f 7220          # Prior 
+00006b40: 6465 7065 6e64 7320 6f6e 2073 7065 6374  depends on spect
+00006b50: 7261 6c20 6461 7461 2073 6574 7469 6e67  ral data setting
+00006b60: 730d 0a20 2020 2020 2020 2020 2020 2073  s..            s
+00006b70: 656c 662e 7365 742e 7072 696f 722e 6361  elf.set.prior.ca
+00006b80: 6c63 756c 6174 655f 6675 6c6c 5f62 6173  lculate_full_bas
+00006b90: 6973 5f73 6574 284e 6f6e 652c 204e 6f6e  is_set(None, Non
+00006ba0: 652c 2064 6174 6173 6574 290d 0a23 2020  e, dataset)..#  
+00006bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006bc0: 7365 742e 7072 696f 722e 6361 6c63 756c  set.prior.calcul
+00006bd0: 6174 655f 6675 6c6c 5f62 6173 6973 5f73  ate_full_basis_s
+00006be0: 6574 2873 656c 662e 7365 742e 7072 696f  et(self.set.prio
+00006bf0: 725f 7070 6d5f 7374 6172 742c 0d0a 2320  r_ppm_start,..# 
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c30: 2020 2020 7365 6c66 2e73 6574 2e70 7269      self.set.pri
+00006c40: 6f72 5f70 706d 5f65 6e64 2c20 0d0a 2320  or_ppm_end, ..# 
+00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c80: 2020 2020 6461 7461 7365 7429 0d0a 2020      dataset)..  
+00006c90: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00006ca0: 2320 6966 2074 6865 2073 7065 6374 7261  # if the spectra
+00006cb0: 6c2c 2073 7061 7469 616c 206f 7220 6669  l, spatial or fi
+00006cc0: 7420 7061 7261 6d65 7465 7220 6469 6d65  t parameter dime
+00006cd0: 6e73 696f 6e73 2068 6176 6520 6368 616e  nsions have chan
+00006ce0: 6765 642c 0d0a 2020 2020 2020 2020 2020  ged,..          
+00006cf0: 2020 2320 7468 656e 2073 6574 2061 2066    # then set a f
+00006d00: 6c61 6720 746f 2072 6573 6574 2072 6573  lag to reset res
+00006d10: 756c 7473 2061 7272 6179 730d 0a20 2020  ults arrays..   
+00006d20: 2020 2020 2020 2020 2073 7065 6374 7261           spectra
+00006d30: 6c5f 6469 6d73 2020 3d20 6461 7461 7365  l_dims  = datase
+00006d40: 742e 7370 6563 7472 616c 5f64 696d 730d  t.spectral_dims.
+00006d50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00006d60: 756c 745f 6469 6d73 2020 2020 3d20 6c69  ult_dims    = li
+00006d70: 7374 2873 7065 6374 7261 6c5f 6469 6d73  st(spectral_dims
+00006d80: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00006d90: 6573 756c 745f 6469 6d73 5b30 5d20 3d20  esult_dims[0] = 
+00006da0: 7365 6c66 2e6e 7061 7261 6d0d 0a20 2020  self.nparam..   
+00006db0: 2020 2020 2020 2020 2073 7065 6374 7261           spectra
+00006dc0: 6c5f 666c 6167 2020 3d20 7365 6c66 2e66  l_flag  = self.f
+00006dd0: 6974 5f62 6173 656c 696e 652e 7368 6170  it_baseline.shap
+00006de0: 655b 305d 2021 3d20 7370 6563 7472 616c  e[0] != spectral
+00006df0: 5f64 696d 735b 305d 0d0a 2020 2020 2020  _dims[0]..      
+00006e00: 2020 2020 2020 7265 7375 6c74 5f66 6c61        result_fla
+00006e10: 6720 2020 203d 2073 656c 662e 6469 6d73  g    = self.dims
+00006e20: 2021 3d20 7265 7375 6c74 5f64 696d 730d   != result_dims.
+00006e30: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
+00006e40: 2020 2069 6620 7370 6563 7472 616c 5f66     if spectral_f
+00006e50: 6c61 6720 6f72 2072 6573 756c 745f 666c  lag or result_fl
+00006e60: 6167 3a0d 0a20 2020 2020 2020 2020 2020  ag:..           
+00006e70: 2020 2020 2073 656c 662e 5f72 6573 6574       self._reset
+00006e80: 5f64 696d 656e 7369 6f6e 616c 5f64 6174  _dimensional_dat
+00006e90: 6128 6461 7461 7365 7429 0d0a 2020 2020  a(dataset)..    
+00006ea0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00006eb0: 656c 662e 6368 6169 6e20 6973 206e 6f74  elf.chain is not
+00006ec0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00006ed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006ee0: 2e63 6861 696e 2e72 6573 6574 5f72 6573  .chain.reset_res
+00006ef0: 756c 7473 5f61 7272 6179 7328 290d 0a0d  ults_arrays()...
+00006f00: 0a0d 0a20 2020 2064 6566 2063 6865 636b  ...    def check
+00006f10: 5f70 6172 616d 6574 6572 5f64 696d 656e  _parameter_dimen
+00006f20: 7369 6f6e 7328 7365 6c66 2c20 6461 7461  sions(self, data
+00006f30: 7365 7429 3a0d 0a20 2020 2020 2020 2022  set):..        "
+00006f40: 2222 0d0a 2020 2020 2020 2020 4368 6563  ""..        Chec
+00006f50: 6b73 2074 6865 2022 6e70 6172 616d 2220  ks the "nparam" 
+00006f60: 6469 6d65 6e73 696f 6e20 696e 2074 6865  dimension in the
+00006f70: 2072 6573 756c 7473 2074 6f20 7365 6520   results to see 
+00006f80: 6966 2074 6865 206e 756d 6265 7220 6f66  if the number of
+00006f90: 200d 0a20 2020 2020 2020 2070 6172 616d   ..        param
+00006fa0: 6574 6572 7320 696e 2074 6865 206d 6f64  eters in the mod
+00006fb0: 656c 2068 6173 2063 6861 6e67 6564 2e20  el has changed. 
+00006fc0: 4f6e 6c79 2072 6573 6574 7320 7265 7375  Only resets resu
+00006fd0: 6c74 7320 6966 2074 6869 730d 0a20 2020  lts if this..   
+00006fe0: 2020 2020 2064 696d 656e 7369 6f6e 2068       dimension h
+00006ff0: 6173 2063 6861 6e67 6564 2e0d 0a20 2020  as changed...   
+00007000: 2020 2020 200d 0a20 2020 2020 2020 2022       ..        "
+00007010: 2222 0d0a 2020 2020 2020 2020 6966 2073  ""..        if s
+00007020: 656c 662e 6669 745f 7265 7375 6c74 732e  elf.fit_results.
+00007030: 7368 6170 655b 305d 2021 3d20 7365 6c66  shape[0] != self
+00007040: 2e6e 7061 7261 6d3a 0d0a 2020 2020 2020  .nparam:..      
+00007050: 2020 2020 2020 7365 6c66 2e5f 7265 7365        self._rese
+00007060: 745f 6469 6d65 6e73 696f 6e61 6c5f 6461  t_dimensional_da
+00007070: 7461 2864 6174 6173 6574 290d 0a0d 0a0d  ta(dataset).....
+00007080: 0a20 2020 2064 6566 205f 7265 7365 745f  .    def _reset_
+00007090: 6469 6d65 6e73 696f 6e61 6c5f 6461 7461  dimensional_data
+000070a0: 2873 656c 662c 2064 6174 6173 6574 293a  (self, dataset):
+000070b0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000070c0: 2020 2020 2020 2052 6573 6574 7320 2874         Resets (t
+000070d0: 6f20 7a65 726f 2920 616e 6420 7265 7369  o zero) and resi
+000070e0: 7a65 7320 6469 6d65 6e73 696f 6e61 6c6c  zes dimensionall
+000070f0: 792d 6465 7065 6e64 656e 7420 6461 7461  y-dependent data
+00007100: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00007110: 2020 2020 6669 745f 7265 7375 6c74 7320      fit_results 
+00007120: 2020 2020 2d20 6669 7420 7061 7261 6d65      - fit parame
+00007130: 7465 7273 2066 726f 6d20 6f70 7469 6d69  ters from optimi
+00007140: 7a61 7469 6f6e 0d0a 2020 2020 2020 2020  zation..        
+00007150: 6669 745f 7374 6174 7320 2020 2020 2020  fit_stats       
+00007160: 2d20 6f70 7469 6d69 7a61 7469 6f6e 2063  - optimization c
+00007170: 6869 7371 722c 2077 7463 6869 7371 7220  hisqr, wtchisqr 
+00007180: 616e 6420 6669 6e69 7465 6d61 7468 2076  and finitemath v
+00007190: 616c 7565 730d 0a20 2020 2020 2020 2066  alues..        f
+000071a0: 6974 5f62 6173 656c 696e 6520 2020 202d  it_baseline    -
+000071b0: 2062 6173 656c 696e 6520 7265 7375 6c74   baseline result
+000071c0: 2028 6d61 7920 6265 2076 6563 746f 7220   (may be vector 
+000071d0: 6f72 2070 6172 616d 6574 6572 697a 6564  or parameterized
+000071e0: 290d 0a20 2020 2020 2020 2063 6f6e 6669  )..        confi
+000071f0: 6465 6e63 6520 2020 2020 202d 2063 6f6e  dence      - con
+00007200: 6669 6465 6e63 6520 6c69 6d69 7473 2072  fidence limits r
+00007210: 6573 756c 7473 2073 746f 7261 6765 0d0a  esults storage..
+00007220: 2020 2020 2020 2020 6372 616d 6572 5f72          cramer_r
+00007230: 616f 2020 2020 2020 2d20 6372 616d 6572  ao      - cramer
+00007240: 2d72 616f 2062 6f75 6e64 7320 7265 7375  -rao bounds resu
+00007250: 6c74 7320 7374 6f72 6167 650d 0a20 2020  lts storage..   
+00007260: 2020 2020 2069 6e69 7469 616c 5f76 616c       initial_val
+00007270: 7565 7320 202d 2069 6e69 7469 616c 2076  ues  - initial v
+00007280: 616c 7565 7320 666f 7220 6d65 7461 6220  alues for metab 
+00007290: 6f70 7469 6d69 7a61 7469 6f6e 0d0a 2020  optimization..  
+000072a0: 2020 2020 2020 7072 696f 725f 6d61 736b        prior_mask
+000072b0: 2020 2020 2020 2d20 7370 6174 6961 6c20        - spatial 
+000072c0: 2878 2c79 2c7a 2920 6d61 736b 2074 6f20  (x,y,z) mask to 
+000072d0: 696e 6469 6361 7465 2077 6861 7420 766f  indicate what vo
+000072e0: 7865 6c73 2074 6f20 6669 740d 0a20 2020  xels to fit..   
+000072f0: 2020 2020 200d 0a20 2020 2020 2020 204e       ..        N
+00007300: 6f74 652e 2042 3020 7368 6966 7420 6973  ote. B0 shift is
+00007310: 2061 6363 6f75 6e74 6564 2066 6f72 2069   accounted for i
+00007320: 6e20 5370 6563 7472 616c 206f 626a 6563  n Spectral objec
+00007330: 742f 7461 6273 0d0a 2020 2020 2020 2020  t/tabs..        
+00007340: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00007350: 2020 2020 2020 2064 696d 7320 3d20 6461         dims = da
+00007360: 7461 7365 742e 7370 6563 7472 616c 5f64  taset.spectral_d
+00007370: 696d 730d 0a20 2020 2020 2020 200d 0a20  ims..        .. 
+00007380: 2020 2020 2020 206e 7061 7261 6d20 3d20         nparam = 
+00007390: 7365 6c66 2e6e 7061 7261 6d20 2020 2020  self.nparam     
+000073a0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+000073b0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+000073c0: 6974 5f72 6573 756c 7473 2069 7320 4e6f  it_results is No
+000073d0: 6e65 3a0d 0a20 2020 2020 2020 200d 0a20  ne:..        .. 
+000073e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000073f0: 6669 745f 7265 7375 6c74 7320 2020 203d  fit_results    =
+00007400: 206e 702e 7a65 726f 7328 286e 7061 7261   np.zeros((npara
+00007410: 6d2c 2064 696d 735b 315d 2c20 6469 6d73  m, dims[1], dims
+00007420: 5b32 5d2c 2064 696d 735b 335d 2929 2020  [2], dims[3]))  
+00007430: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00007440: 2020 7365 6c66 2e66 6974 5f73 7461 7473    self.fit_stats
+00007450: 2020 2020 2020 3d20 6e70 2e7a 6572 6f73        = np.zeros
+00007460: 2828 332c 2064 696d 735b 315d 2c20 6469  ((3, dims[1], di
+00007470: 6d73 5b32 5d2c 2064 696d 735b 335d 2929  ms[2], dims[3]))
+00007480: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00007490: 2020 2020 7365 6c66 2e66 6974 5f62 6173      self.fit_bas
+000074a0: 656c 696e 6520 2020 3d20 6e70 2e7a 6572  eline   = np.zer
+000074b0: 6f73 2874 7570 6c65 2864 6174 6173 6574  os(tuple(dataset
+000074c0: 2e73 7065 6374 7261 6c5f 6469 6d73 292c  .spectral_dims),
+000074d0: 2064 7479 7065 3d27 636f 6d70 6c65 7836   dtype='complex6
+000074e0: 3427 290d 0a20 2020 2020 2020 2020 2020  4')..           
+000074f0: 2073 656c 662e 636f 6e66 6964 656e 6365   self.confidence
+00007500: 2020 2020 203d 206e 702e 7a65 726f 7328       = np.zeros(
+00007510: 286e 7061 7261 6d2c 2064 696d 735b 315d  (nparam, dims[1]
+00007520: 2c20 6469 6d73 5b32 5d2c 2064 696d 735b  , dims[2], dims[
+00007530: 335d 2929 2020 2020 2020 0d0a 2020 2020  3]))      ..    
+00007540: 2020 2020 2020 2020 7365 6c66 2e63 7261          self.cra
+00007550: 6d65 725f 7261 6f20 2020 2020 3d20 6e70  mer_rao     = np
+00007560: 2e7a 6572 6f73 2828 6e70 6172 616d 2c20  .zeros((nparam, 
+00007570: 6469 6d73 5b31 5d2c 2064 696d 735b 325d  dims[1], dims[2]
+00007580: 2c20 6469 6d73 5b33 5d29 2920 2020 2020  , dims[3]))     
+00007590: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+000075a0: 656c 662e 696e 6974 6961 6c5f 7661 6c75  elf.initial_valu
+000075b0: 6573 203d 206e 702e 7a65 726f 7328 286e  es = np.zeros((n
+000075c0: 7061 7261 6d2c 2064 696d 735b 315d 2c20  param, dims[1], 
+000075d0: 6469 6d73 5b32 5d2c 2064 696d 735b 335d  dims[2], dims[3]
+000075e0: 2929 2020 2020 2020 0d0a 2020 2020 2020  ))      ..      
+000075f0: 2020 2020 2020 7365 6c66 2e70 7269 6f72        self.prior
+00007600: 5f6d 6173 6b20 2020 2020 3d20 6e70 2e6f  _mask     = np.o
+00007610: 6e65 7328 2864 696d 735b 315d 2c20 6469  nes((dims[1], di
+00007620: 6d73 5b32 5d2c 2064 696d 735b 335d 2929  ms[2], dims[3]))
+00007630: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
+00007640: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00007650: 2020 2020 2020 2020 7061 7261 6d5f 6469          param_di
+00007660: 6d73 203d 206c 6973 7428 6469 6d73 290d  ms = list(dims).
+00007670: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+00007680: 616d 5f64 696d 735b 305d 203d 206e 7061  am_dims[0] = npa
+00007690: 7261 6d0d 0a0d 0a20 2020 2020 2020 2020  ram....         
+000076a0: 2020 2023 206d 6169 6e74 6169 6e20 7265     # maintain re
+000076b0: 7375 6c74 7320 6966 206e 6f20 6469 6d65  sults if no dime
+000076c0: 6e73 696f 6e20 6861 7320 6368 616e 6765  nsion has change
+000076d0: 640d 0a20 2020 2020 2020 2020 2020 2069  d..            i
+000076e0: 6620 7365 6c66 2e66 6974 5f62 6173 656c  f self.fit_basel
+000076f0: 696e 652e 7368 6170 655b 3a3a 2d31 5d20  ine.shape[::-1] 
+00007700: 213d 2064 696d 7320 6f72 205c 0d0a 2020  != dims or \..  
+00007710: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007720: 6c66 2e66 6974 5f72 6573 756c 7473 2e73  lf.fit_results.s
+00007730: 6861 7065 5b3a 3a2d 315d 2021 3d20 7061  hape[::-1] != pa
+00007740: 7261 6d5f 6469 6d73 3a0d 0a20 2020 2020  ram_dims:..     
+00007750: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00007760: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007770: 662e 6669 745f 6261 7365 6c69 6e65 2020  f.fit_baseline  
+00007780: 203d 206e 702e 7a65 726f 7328 7475 706c   = np.zeros(tupl
+00007790: 6528 6469 6d73 292c 2064 7479 7065 3d27  e(dims), dtype='
+000077a0: 636f 6d70 6c65 7836 3427 2920 2020 2020  complex64')     
+000077b0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000077d0: 656c 662e 6669 745f 7265 7375 6c74 7320  elf.fit_results 
+000077e0: 2020 203d 206e 702e 7a65 726f 7328 286e     = np.zeros((n
+000077f0: 7061 7261 6d2c 2064 696d 735b 315d 2c20  param, dims[1], 
+00007800: 6469 6d73 5b32 5d2c 2064 696d 735b 335d  dims[2], dims[3]
+00007810: 2929 2020 2020 2020 0d0a 2020 2020 2020  ))      ..      
+00007820: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00007830: 6974 5f73 7461 7473 2020 2020 2020 3d20  it_stats      = 
+00007840: 6e70 2e7a 6572 6f73 2828 332c 2064 696d  np.zeros((3, dim
+00007850: 735b 315d 2c20 6469 6d73 5b32 5d2c 2064  s[1], dims[2], d
+00007860: 696d 735b 335d 2929 2020 2020 2020 0d0a  ims[3]))      ..
+00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007880: 7365 6c66 2e66 6974 5f62 6173 656c 696e  self.fit_baselin
+00007890: 6520 2020 3d20 6e70 2e7a 6572 6f73 2874  e   = np.zeros(t
+000078a0: 7570 6c65 2864 6174 6173 6574 2e73 7065  uple(dataset.spe
+000078b0: 6374 7261 6c5f 6469 6d73 292c 2064 7479  ctral_dims), dty
+000078c0: 7065 3d27 636f 6d70 6c65 7836 3427 290d  pe='complex64').
+000078d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000078e0: 2073 656c 662e 636f 6e66 6964 656e 6365   self.confidence
+000078f0: 2020 2020 203d 206e 702e 7a65 726f 7328       = np.zeros(
+00007900: 286e 7061 7261 6d2c 2064 696d 735b 315d  (nparam, dims[1]
+00007910: 2c20 6469 6d73 5b32 5d2c 2064 696d 735b  , dims[2], dims[
+00007920: 335d 2929 2020 2020 2020 0d0a 2020 2020  3]))      ..    
+00007930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007940: 2e63 7261 6d65 725f 7261 6f20 2020 2020  .cramer_rao     
+00007950: 3d20 6e70 2e7a 6572 6f73 2828 6e70 6172  = np.zeros((npar
+00007960: 616d 2c20 6469 6d73 5b31 5d2c 2064 696d  am, dims[1], dim
+00007970: 735b 325d 2c20 6469 6d73 5b33 5d29 2920  s[2], dims[3])) 
+00007980: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007990: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+000079a0: 6961 6c5f 7661 6c75 6573 203d 206e 702e  ial_values = np.
+000079b0: 7a65 726f 7328 286e 7061 7261 6d2c 2064  zeros((nparam, d
+000079c0: 696d 735b 315d 2c20 6469 6d73 5b32 5d2c  ims[1], dims[2],
+000079d0: 2064 696d 735b 335d 2929 2020 2020 2020   dims[3]))      
+000079e0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a00: 7365 6c66 2e70 7269 6f72 5f6d 6173 6b20  self.prior_mask 
+00007a10: 2020 2020 3d20 6e70 2e6f 6e65 7328 2864      = np.ones((d
+00007a20: 696d 735b 315d 2c20 6469 6d73 5b32 5d2c  ims[1], dims[2],
+00007a30: 2064 696d 735b 335d 2929 200d 0a0d 0a0d   dims[3])) .....
+00007a40: 0a20 2020 2064 6566 2067 6574 5f66 6974  .    def get_fit
+00007a50: 7465 645f 7761 7465 725f 6172 6561 2873  ted_water_area(s
+00007a60: 656c 6629 3a0d 0a20 2020 2020 2020 200d  elf):..        .
+00007a70: 0a20 2020 2020 2020 2066 6c61 675f 7761  .        flag_wa
+00007a80: 7465 7220 3d20 4661 6c73 650d 0a20 2020  ter = False..   
+00007a90: 2020 2020 2066 6f72 2069 6e64 782c 2069       for indx, i
+00007aa0: 7465 6d20 696e 2065 6e75 6d65 7261 7465  tem in enumerate
+00007ab0: 2873 656c 662e 7365 742e 7072 696f 725f  (self.set.prior_
+00007ac0: 6c69 7374 293a 0d0a 2020 2020 2020 2020  list):..        
+00007ad0: 2020 2020 6966 2027 7761 7465 7227 2069      if 'water' i
+00007ae0: 6e20 6974 656d 2e6c 6f77 6572 2829 206f  n item.lower() o
+00007af0: 7220 2768 326f 2720 696e 2069 7465 6d2e  r 'h2o' in item.
+00007b00: 6c6f 7765 7228 293a 0d0a 2020 2020 2020  lower():..      
+00007b10: 2020 2020 2020 2020 2020 666c 6167 5f77            flag_w
+00007b20: 6174 6572 203d 2054 7275 650d 0a20 2020  ater = True..   
+00007b30: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00007b40: 785f 7761 7465 7220 3d20 696e 6478 0d0a  x_water = indx..
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 6272 6561 6b0d 0a20 2020 2020 2020 200d  break..        .
+00007b70: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00007b80: 666c 6167 5f77 6174 6572 3a0d 0a20 2020  flag_water:..   
+00007b90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007ba0: 4e6f 6e65 0d0a 2020 2020 2020 2020 656c  None..        el
+00007bb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00007bc0: 2064 696d 7320 3d20 7365 6c66 2e66 6974   dims = self.fit
+00007bd0: 5f72 6573 756c 7473 2e73 6861 7065 0d0a  _results.shape..
+00007be0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00007bf0: 203d 2073 656c 662e 6669 745f 7265 7375   = self.fit_resu
+00007c00: 6c74 735b 696e 6478 5f77 6174 6572 2c3a  lts[indx_water,:
+00007c10: 2c3a 2c3a 5d0d 0a20 2020 2020 2020 2020  ,:,:]..         
+00007c20: 2020 2072 6573 2020 3d20 7265 732e 636f     res  = res.co
+00007c30: 7079 2829 200d 0a20 2020 2020 2020 2020  py() ..         
+00007c40: 2020 2069 6620 6469 6d73 5b31 5d20 2a20     if dims[1] * 
+00007c50: 6469 6d73 5b32 5d20 2a20 6469 6d73 5b33  dims[2] * dims[3
+00007c60: 5d20 3d3d 2031 3a0d 0a20 2020 2020 2020  ] == 1:..       
+00007c70: 2020 2020 2020 2020 2072 6573 2e73 6861           res.sha
+00007c80: 7065 203d 2031 2c31 2c31 2c31 0d0a 2020  pe = 1,1,1,1..  
+00007c90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007ca0: 2072 6573 2020 2320 7265 7475 726e 2077   res  # return w
+00007cb0: 6174 6572 2061 7265 6173 0d0a 0d0a 0d0a  ater areas......
+00007cc0: 2020 2020 6465 6620 6765 745f 6173 736f      def get_asso
+00007cd0: 6369 6174 6564 5f64 6174 6173 6574 7328  ciated_datasets(
+00007ce0: 7365 6c66 2c20 6973 5f6d 6169 6e5f 6461  self, is_main_da
+00007cf0: 7461 7365 743d 5472 7565 293a 0d0a 2020  taset=True):..  
+00007d00: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00007d10: 2020 2052 6574 7572 6e73 2061 206c 6973     Returns a lis
+00007d20: 7420 6f66 2064 6174 6173 6574 7320 6173  t of datasets as
+00007d30: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
+00007d40: 6973 206f 626a 6563 740d 0a0d 0a20 2020  is object....   
+00007d50: 2020 2020 2027 6973 5f6d 6169 6e5f 6461       'is_main_da
+00007d60: 7461 7365 7427 2073 6967 6e61 6c73 2074  taset' signals t
+00007d70: 6861 7420 7468 6973 2069 7320 7468 6520  hat this is the 
+00007d80: 746f 7020 6c65 7665 6c20 6461 7461 7365  top level datase
+00007d90: 7420 6761 7468 6572 696e 6720 0d0a 2020  t gathering ..  
+00007da0: 2020 2020 2020 6173 736f 6369 6174 6564        associated
+00007db0: 2064 6174 6173 6574 732c 2061 6e64 2069   datasets, and i
+00007dc0: 7320 7573 6564 2074 6f20 7374 6f70 2063  s used to stop c
+00007dd0: 6972 6375 6c61 7220 7265 6665 7265 6e63  ircular referenc
+00007de0: 6573 0d0a 0d0a 2020 2020 2020 2020 2222  es....        ""
+00007df0: 220d 0a20 2020 2020 2020 2064 6174 6173  "..        datas
+00007e00: 6574 7320 3d20 626c 6f63 6b5f 6669 745f  ets = block_fit_
+00007e10: 6964 656e 7469 7479 2e42 6c6f 636b 4669  identity.BlockFi
+00007e20: 7449 6465 6e74 6974 792e 6765 745f 6173  tIdentity.get_as
+00007e30: 736f 6369 6174 6564 5f64 6174 6173 6574  sociated_dataset
+00007e40: 7328 7365 6c66 2c20 6973 5f6d 6169 6e5f  s(self, is_main_
+00007e50: 6461 7461 7365 7429 0d0a 0d0a 2020 2020  dataset)....    
+00007e60: 2020 2020 6966 2069 735f 6d61 696e 5f64      if is_main_d
+00007e70: 6174 6173 6574 3a0d 0a20 2020 2020 2020  ataset:..       
+00007e80: 2020 2020 2023 2061 7420 7468 6973 2070       # at this p
+00007e90: 6f69 6e74 2c20 6f6e 6c79 2061 206d 6163  oint, only a mac
+00007ea0: 726f 6d6f 6c65 6375 6c65 206d 6f64 656c  romolecule model
+00007eb0: 206d 6179 206e 6565 6420 616e 2061 7373   may need an ass
+00007ec0: 6f63 6961 7465 6420 6461 7461 7365 740d  ociated dataset.
+00007ed0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007ee0: 7365 6c66 2e73 6574 2e6d 6163 726f 6d6f  self.set.macromo
+00007ef0: 6c5f 7369 6e67 6c65 5f62 6173 6973 5f64  l_single_basis_d
+00007f00: 6174 6173 6574 3a0d 0a20 2020 2020 2020  ataset:..       
+00007f10: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
+00007f20: 7320 2b3d 2073 656c 662e 7365 742e 6d61  s += self.set.ma
+00007f30: 6372 6f6d 6f6c 5f73 696e 676c 655f 6261  cromol_single_ba
+00007f40: 7369 735f 6461 7461 7365 742e 6765 745f  sis_dataset.get_
+00007f50: 6173 736f 6369 6174 6564 5f64 6174 6173  associated_datas
+00007f60: 6574 7328 6973 5f6d 6169 6e5f 6461 7461  ets(is_main_data
+00007f70: 7365 743d 4661 6c73 6529 0d0a 2020 2020  set=False)..    
+00007f80: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00007f90: 7365 7473 202b 3d20 5b73 656c 662e 7365  sets += [self.se
+00007fa0: 742e 6d61 6372 6f6d 6f6c 5f73 696e 676c  t.macromol_singl
+00007fb0: 655f 6261 7369 735f 6461 7461 7365 745d  e_basis_dataset]
+00007fc0: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00007fd0: 726e 2064 6174 6173 6574 730d 0a0d 0a0d  rn datasets.....
+00007fe0: 0a20 2020 2064 6566 2073 6574 5f61 7373  .    def set_ass
+00007ff0: 6f63 6961 7465 645f 6461 7461 7365 7473  ociated_datasets
+00008000: 2873 656c 662c 2064 6174 6173 6574 7329  (self, datasets)
+00008010: 3a20 0d0a 2020 2020 2020 2020 2222 220d  : ..        """.
+00008020: 0a20 2020 2020 2020 2057 6865 6e20 7765  .        When we
+00008030: 206f 7065 6e20 6120 5649 4646 2066 6f72   open a VIFF for
+00008040: 6d61 7420 6669 6c65 2c20 6d61 696e 2e5f  mat file, main._
+00008050: 696d 706f 7274 5f66 696c 6528 2920 6361  import_file() ca
+00008060: 6c6c 7320 7468 6973 206d 6574 686f 640d  lls this method.
+00008070: 0a20 2020 2020 2020 2074 6f20 7061 7273  .        to pars
+00008080: 652f 7374 6f72 6520 616e 7920 6461 7461  e/store any data
+00008090: 7365 7473 2061 7373 6f63 6961 7465 6420  sets associated 
+000080a0: 7769 7468 2074 6869 7320 6f6e 6520 6173  with this one as
+000080b0: 2064 6573 6372 6962 6564 2062 656c 6f77   described below
+000080c0: 2e0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
+000080d0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000080e0: 2020 666f 7220 6461 7461 7365 7420 696e    for dataset in
+000080f0: 2064 6174 6173 6574 733a 0d0a 2020 2020   datasets:..    
+00008100: 2020 2020 2020 2020 6966 2064 6174 6173          if datas
+00008110: 6574 2e69 6420 3d3d 2073 656c 662e 7365  et.id == self.se
+00008120: 742e 6d61 6372 6f6d 6f6c 5f73 696e 676c  t.macromol_singl
+00008130: 655f 6261 7369 735f 6461 7461 7365 745f  e_basis_dataset_
+00008140: 6964 3a0d 0a20 2020 2020 2020 2020 2020  id:..           
+00008150: 2020 2020 2073 656c 662e 7365 742e 6d61       self.set.ma
+00008160: 6372 6f6d 6f6c 5f73 696e 676c 655f 6261  cromol_single_ba
+00008170: 7369 735f 6461 7461 7365 7420 3d20 6461  sis_dataset = da
+00008180: 7461 7365 740d 0a0d 0a0d 0a20 2020 2064  taset......    d
+00008190: 6566 2064 6566 6c61 7465 2873 656c 662c  ef deflate(self,
+000081a0: 2066 6c61 766f 723d 4465 666c 6174 652e   flavor=Deflate.
+000081b0: 4554 5245 4529 3a0d 0a20 2020 2020 2020  ETREE):..       
+000081c0: 2069 6620 666c 6176 6f72 203d 3d20 4465   if flavor == De
+000081d0: 666c 6174 652e 4554 5245 453a 0d0a 2020  flate.ETREE:..  
+000081e0: 2020 2020 2020 2020 2020 6520 3d20 456c            e = El
+000081f0: 656d 656e 7428 2262 6c6f 636b 5f66 6974  ement("block_fit
+00008200: 5f67 6973 6f22 2c20 7b20 2269 6422 203a  _giso", { "id" :
+00008210: 2073 656c 662e 6964 2c0d 0a20 2020 2020   self.id,..     
+00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
+00008250: 203a 2073 656c 662e 584d 4c5f 5645 5253   : self.XML_VERS
+00008260: 494f 4e7d 290d 0a20 2020 2020 2020 2020  ION})..         
+00008270: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008280: 2075 7469 6c5f 786d 6c2e 5465 7874 5375   util_xml.TextSu
+00008290: 6245 6c65 6d65 6e74 2865 2c20 2262 6568  bElement(e, "beh
+000082a0: 6176 655f 6173 5f70 7265 7365 7422 2c20  ave_as_preset", 
+000082b0: 7365 6c66 2e62 6568 6176 655f 6173 5f70  self.behave_as_p
+000082c0: 7265 7365 7429 0d0a 2020 2020 2020 2020  reset)..        
+000082d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000082e0: 2020 652e 6170 7065 6e64 2873 656c 662e    e.append(self.
+000082f0: 7365 742e 6465 666c 6174 6528 2929 0d0a  set.deflate())..
+00008300: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00008310: 206e 6f74 2073 656c 662e 6265 6861 7665   not self.behave
+00008320: 5f61 735f 7072 6573 6574 3a0d 0a20 2020  _as_preset:..   
+00008330: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00008340: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
+00008350: 696d 2069 6e20 7365 6c66 2e64 696d 733a  im in self.dims:
+00008360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008370: 2020 2020 2020 7574 696c 5f78 6d6c 2e54        util_xml.T
+00008380: 6578 7453 7562 456c 656d 656e 7428 652c  extSubElement(e,
+00008390: 2022 6469 6d22 2c20 6469 6d29 0d0a 0d0a   "dim", dim)....
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 6966 2073 656c 662e 6669 745f 7265 7375  if self.fit_resu
+000083c0: 6c74 7320 6973 206e 6f74 204e 6f6e 653a  lts is not None:
+000083d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000083e0: 2020 2020 2020 652e 6170 7065 6e64 2875        e.append(u
+000083f0: 7469 6c5f 786d 6c2e 6e75 6d70 795f 6172  til_xml.numpy_ar
+00008400: 7261 795f 746f 5f65 6c65 6d65 6e74 2873  ray_to_element(s
+00008410: 656c 662e 6669 745f 7265 7375 6c74 732c  elf.fit_results,
+00008420: 2766 6974 5f72 6573 756c 7473 2729 290d  'fit_results')).
+00008430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008440: 2069 6620 7365 6c66 2e66 6974 5f73 7461   if self.fit_sta
+00008450: 7473 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ts is not None:.
+00008460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008470: 2020 2020 2065 2e61 7070 656e 6428 7574       e.append(ut
+00008480: 696c 5f78 6d6c 2e6e 756d 7079 5f61 7272  il_xml.numpy_arr
+00008490: 6179 5f74 6f5f 656c 656d 656e 7428 7365  ay_to_element(se
+000084a0: 6c66 2e66 6974 5f73 7461 7473 2c27 6669  lf.fit_stats,'fi
+000084b0: 745f 7374 6174 7327 2929 0d0a 2020 2020  t_stats'))..    
+000084c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000084d0: 656c 662e 6669 745f 6261 7365 6c69 6e65  elf.fit_baseline
+000084e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008500: 2020 2065 2e61 7070 656e 6428 7574 696c     e.append(util
+00008510: 5f78 6d6c 2e6e 756d 7079 5f61 7272 6179  _xml.numpy_array
+00008520: 5f74 6f5f 656c 656d 656e 7428 7365 6c66  _to_element(self
+00008530: 2e66 6974 5f62 6173 656c 696e 652c 2766  .fit_baseline,'f
+00008540: 6974 5f62 6173 656c 696e 6527 2929 0d0a  it_baseline'))..
+00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008560: 6966 2073 656c 662e 636f 6e66 6964 656e  if self.confiden
+00008570: 6365 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ce is not None:.
+00008580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008590: 2020 2020 2065 2e61 7070 656e 6428 7574       e.append(ut
+000085a0: 696c 5f78 6d6c 2e6e 756d 7079 5f61 7272  il_xml.numpy_arr
+000085b0: 6179 5f74 6f5f 656c 656d 656e 7428 7365  ay_to_element(se
+000085c0: 6c66 2e63 6f6e 6669 6465 6e63 652c 2763  lf.confidence,'c
+000085d0: 6f6e 6669 6465 6e63 6527 2929 0d0a 2020  onfidence'))..  
+000085e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000085f0: 2073 656c 662e 6372 616d 6572 5f72 616f   self.cramer_rao
+00008600: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008620: 2020 2065 2e61 7070 656e 6428 7574 696c     e.append(util
+00008630: 5f78 6d6c 2e6e 756d 7079 5f61 7272 6179  _xml.numpy_array
+00008640: 5f74 6f5f 656c 656d 656e 7428 7365 6c66  _to_element(self
+00008650: 2e63 7261 6d65 725f 7261 6f2c 2763 7261  .cramer_rao,'cra
+00008660: 6d65 725f 7261 6f27 2929 0d0a 2020 2020  mer_rao'))..    
+00008670: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00008680: 656c 662e 696e 6974 6961 6c5f 7661 6c75  elf.initial_valu
+00008690: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0d  es is not None:.
+000086a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000086b0: 2020 2020 2065 2e61 7070 656e 6428 7574       e.append(ut
+000086c0: 696c 5f78 6d6c 2e6e 756d 7079 5f61 7272  il_xml.numpy_arr
+000086d0: 6179 5f74 6f5f 656c 656d 656e 7428 7365  ay_to_element(se
+000086e0: 6c66 2e69 6e69 7469 616c 5f76 616c 7565  lf.initial_value
+000086f0: 732c 2769 6e69 7469 616c 5f76 616c 7565  s,'initial_value
+00008700: 7327 2929 0d0a 2020 2020 2020 2020 2020  s'))..          
+00008710: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+00008720: 696f 725f 6d61 736b 2069 7320 6e6f 7420  ior_mask is not 
+00008730: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00008740: 2020 2020 2020 2020 2020 2065 2e61 7070             e.app
+00008750: 656e 6428 7574 696c 5f78 6d6c 2e6e 756d  end(util_xml.num
+00008760: 7079 5f61 7272 6179 5f74 6f5f 656c 656d  py_array_to_elem
+00008770: 656e 7428 7365 6c66 2e70 7269 6f72 5f6d  ent(self.prior_m
+00008780: 6173 6b2c 2770 7269 6f72 5f6d 6173 6b27  ask,'prior_mask'
+00008790: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000087a0: 2020 7265 7475 726e 2065 0d0a 2020 2020    return e..    
+000087b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000087c0: 2020 656c 6966 2066 6c61 766f 7220 3d3d    elif flavor ==
+000087d0: 2044 6566 6c61 7465 2e44 4943 5449 4f4e   Deflate.DICTION
+000087e0: 4152 593a 0d0a 2020 2020 2020 2020 2020  ARY:..          
+000087f0: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00008800: 6469 6374 5f5f 2e63 6f70 7928 290d 0a0d  dict__.copy()...
+00008810: 0a0d 0a20 2020 2064 6566 2069 6e66 6c61  ...    def infla
+00008820: 7465 2873 656c 662c 2073 6f75 7263 6529  te(self, source)
+00008830: 3a0d 0a20 2020 2020 2020 2069 6620 6861  :..        if ha
+00008840: 7361 7474 7228 736f 7572 6365 2c20 226d  sattr(source, "m
+00008850: 616b 6565 6c65 6d65 6e74 2229 3a0d 0a20  akeelement"):.. 
+00008860: 2020 2020 2020 2020 2020 2023 2051 7561             # Qua
+00008870: 636b 7320 6c69 6b65 2061 6e20 456c 656d  cks like an Elem
+00008880: 656e 7454 7265 652e 456c 656d 656e 740d  entTree.Element.
+00008890: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+000088a0: 656c 662e 6964 203d 2073 6f75 7263 652e  elf.id = source.
+000088b0: 6765 7428 2269 6422 290d 0a0d 0a20 2020  get("id")....   
+000088c0: 2020 2020 2020 2020 2076 616c 203d 2073           val = s
+000088d0: 6f75 7263 652e 6669 6e64 7465 7874 2822  ource.findtext("
+000088e0: 6265 6861 7665 5f61 735f 7072 6573 6574  behave_as_preset
+000088f0: 2229 2020 2023 2064 6566 6175 6c74 2069  ")   # default i
+00008900: 7320 4661 6c73 650d 0a20 2020 2020 2020  s False..       
+00008910: 2020 2020 2069 6620 7661 6c20 6973 206e       if val is n
+00008920: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00008930: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00008940: 6568 6176 655f 6173 5f70 7265 7365 7420  ehave_as_preset 
+00008950: 3d20 7574 696c 5f78 6d6c 2e42 4f4f 4c45  = util_xml.BOOLE
+00008960: 414e 535b 7661 6c5d 0d0a 0d0a 2020 2020  ANS[val]....    
+00008970: 2020 2020 2020 2020 2320 4c6f 6f6b 2066          # Look f
+00008980: 6f72 2073 6574 7469 6e67 7320 756e 6465  or settings unde
+00008990: 7220 7468 6520 6f6c 6420 6e61 6d65 2061  r the old name a
+000089a0: 7320 7765 6c6c 2061 7320 7468 6520 7374  s well as the st
+000089b0: 616e 6461 7264 206e 616d 652e 0d0a 2020  andard name...  
+000089c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000089d0: 6574 203d 2075 7469 6c5f 786d 6c2e 6669  et = util_xml.fi
+000089e0: 6e64 5f73 6574 7469 6e67 7328 736f 7572  nd_settings(sour
+000089f0: 6365 2c20 2262 6c6f 636b 5f67 6973 6f5f  ce, "block_giso_
+00008a00: 7365 7474 696e 6773 2229 0d0a 2020 2020  settings")..    
+00008a10: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00008a20: 203d 205f 5365 7474 696e 6773 2873 656c   = _Settings(sel
+00008a30: 662e 7365 7429 0d0a 0d0a 2020 2020 2020  f.set)....      
+00008a40: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00008a50: 662e 6265 6861 7665 5f61 735f 7072 6573  f.behave_as_pres
+00008a60: 6574 3a0d 0a0d 0a20 2020 2020 2020 2020  et:....         
+00008a70: 2020 2020 2020 2023 2045 7870 6c69 6369         # Explici
+00008a80: 7420 7465 7374 7320 666f 7220 4e6f 6e65  t tests for None
+00008a90: 206e 6563 6573 7361 7279 2069 6e20 7468   necessary in th
+00008aa0: 6520 636f 6465 2062 656c 6f77 2e20 0d0a  e code below. ..
+00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ac0: 7465 6d70 203d 2073 6f75 7263 652e 6669  temp = source.fi
+00008ad0: 6e64 2822 6669 745f 7265 7375 6c74 7322  nd("fit_results"
+00008ae0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00008af0: 2020 2069 6620 7465 6d70 2069 7320 6e6f     if temp is no
+00008b00: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00008b10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008b20: 662e 6669 745f 7265 7375 6c74 7320 3d20  f.fit_results = 
+00008b30: 7574 696c 5f78 6d6c 2e65 6c65 6d65 6e74  util_xml.element
+00008b40: 5f74 6f5f 6e75 6d70 795f 6172 7261 7928  _to_numpy_array(
+00008b50: 7465 6d70 290d 0a0d 0a20 2020 2020 2020  temp)....       
+00008b60: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
+00008b70: 736f 7572 6365 2e66 696e 6428 2266 6974  source.find("fit
+00008b80: 5f73 7461 7473 2229 0d0a 2020 2020 2020  _stats")..      
+00008b90: 2020 2020 2020 2020 2020 6966 2074 656d            if tem
+00008ba0: 7020 6973 206e 6f74 204e 6f6e 653a 0d0a  p is not None:..
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 2020 2020 7365 6c66 2e66 6974 5f73 7461      self.fit_sta
+00008bd0: 7473 203d 2075 7469 6c5f 786d 6c2e 656c  ts = util_xml.el
+00008be0: 656d 656e 745f 746f 5f6e 756d 7079 5f61  ement_to_numpy_a
+00008bf0: 7272 6179 2874 656d 7029 0d0a 0d0a 2020  rray(temp)....  
+00008c00: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00008c10: 6d70 203d 2073 6f75 7263 652e 6669 6e64  mp = source.find
+00008c20: 2822 6669 745f 6261 7365 6c69 6e65 2229  ("fit_baseline")
+00008c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008c40: 2020 6966 2074 656d 7020 6973 206e 6f74    if temp is not
+00008c50: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00008c60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008c70: 2e66 6974 5f62 6173 656c 696e 6520 3d20  .fit_baseline = 
+00008c80: 7574 696c 5f78 6d6c 2e65 6c65 6d65 6e74  util_xml.element
+00008c90: 5f74 6f5f 6e75 6d70 795f 6172 7261 7928  _to_numpy_array(
+00008ca0: 7465 6d70 290d 0a0d 0a20 2020 2020 2020  temp)....       
+00008cb0: 2020 2020 2020 2020 2074 656d 7020 3d20           temp = 
+00008cc0: 736f 7572 6365 2e66 696e 6428 2263 6f6e  source.find("con
+00008cd0: 6669 6465 6e63 6522 290d 0a20 2020 2020  fidence")..     
+00008ce0: 2020 2020 2020 2020 2020 2069 6620 7465             if te
+00008cf0: 6d70 2069 7320 6e6f 7420 4e6f 6e65 3a0d  mp is not None:.
+00008d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008d10: 2020 2020 2073 656c 662e 636f 6e66 6964       self.confid
+00008d20: 656e 6365 203d 2075 7469 6c5f 786d 6c2e  ence = util_xml.
+00008d30: 656c 656d 656e 745f 746f 5f6e 756d 7079  element_to_numpy
+00008d40: 5f61 7272 6179 2874 656d 7029 0d0a 0d0a  _array(temp)....
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d60: 7465 6d70 203d 2073 6f75 7263 652e 6669  temp = source.fi
+00008d70: 6e64 2822 6372 616d 6572 5f72 616f 2229  nd("cramer_rao")
+00008d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008d90: 2020 6966 2074 656d 7020 6973 206e 6f74    if temp is not
+00008da0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00008db0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008dc0: 2e63 7261 6d65 725f 7261 6f20 3d20 7574  .cramer_rao = ut
+00008dd0: 696c 5f78 6d6c 2e65 6c65 6d65 6e74 5f74  il_xml.element_t
+00008de0: 6f5f 6e75 6d70 795f 6172 7261 7928 7465  o_numpy_array(te
+00008df0: 6d70 290d 0a0d 0a20 2020 2020 2020 2020  mp)....         
+00008e00: 2020 2020 2020 2074 656d 7020 3d20 736f         temp = so
+00008e10: 7572 6365 2e66 696e 6428 2269 6e69 7469  urce.find("initi
+00008e20: 616c 5f76 616c 7565 7322 290d 0a20 2020  al_values")..   
+00008e30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00008e40: 7465 6d70 2069 7320 6e6f 7420 4e6f 6e65  temp is not None
+00008e50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00008e60: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+00008e70: 6961 6c5f 7661 6c75 6573 203d 2075 7469  ial_values = uti
+00008e80: 6c5f 786d 6c2e 656c 656d 656e 745f 746f  l_xml.element_to
+00008e90: 5f6e 756d 7079 5f61 7272 6179 2874 656d  _numpy_array(tem
+00008ea0: 7029 0d0a 0d0a 2020 2020 2020 2020 2020  p)....          
+00008eb0: 2020 2020 2020 7465 6d70 203d 2073 6f75        temp = sou
+00008ec0: 7263 652e 6669 6e64 2822 7072 696f 725f  rce.find("prior_
+00008ed0: 6d61 736b 2229 0d0a 2020 2020 2020 2020  mask")..        
+00008ee0: 2020 2020 2020 2020 6966 2074 656d 7020          if temp 
+00008ef0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f10: 2020 7365 6c66 2e70 7269 6f72 5f6d 6173    self.prior_mas
+00008f20: 6b20 3d20 7574 696c 5f78 6d6c 2e65 6c65  k = util_xml.ele
+00008f30: 6d65 6e74 5f74 6f5f 6e75 6d70 795f 6172  ment_to_numpy_ar
+00008f40: 7261 7928 7465 6d70 290d 0a0d 0a0d 0a20  ray(temp)...... 
+00008f50: 2020 2020 2020 2065 6c69 6620 6861 7361         elif hasa
+00008f60: 7474 7228 736f 7572 6365 2c20 226b 6579  ttr(source, "key
+00008f70: 7322 293a 0d0a 2020 2020 2020 2020 2020  s"):..          
+00008f80: 2020 2320 5175 6163 6b73 206c 696b 6520    # Quacks like 
+00008f90: 6120 6469 6374 0d0a 2020 2020 2020 2020  a dict..        
+00008fa0: 2020 2020 666f 7220 6b65 7920 696e 206c      for key in l
+00008fb0: 6973 7428 736f 7572 6365 2e6b 6579 7328  ist(source.keys(
+00008fc0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00008fd0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00008fe0: 7365 6c66 2c20 6b65 7929 3a0d 0a20 2020  self, key):..   
+00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009000: 2073 6574 6174 7472 2873 656c 662c 206b   setattr(self, k
+00009010: 6579 2c20 736f 7572 6365 5b6b 6579 5d29  ey, source[key])
+00009020: 0d0a 0d0a 0d0a 2020 2020 6465 6620 7265  ......    def re
+00009030: 7375 6c74 735f 6173 5f68 746d 6c28 7365  sults_as_html(se
+00009040: 6c66 2c20 766f 7865 6c2c 206c 773d 302e  lf, voxel, lw=0.
+00009050: 302c 206c 776d 696e 3d30 2e30 2c20 6c77  0, lwmin=0.0, lw
+00009060: 6d61 783d 302e 302c 200d 0a20 2020 2020  max=0.0, ..     
+00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009080: 2020 2064 6174 615f 736f 7572 6365 3d22     data_source="
+00009090: 222c 2069 6d61 6765 3d4e 6f6e 6529 3a0d  ", image=None):.
+000090a0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000090b0: 2020 2020 2020 4769 7665 6e20 6120 766f        Given a vo
+000090c0: 7865 6c2c 206c 696e 6577 6964 7468 2070  xel, linewidth p
+000090d0: 6172 616d 732c 2061 6e64 2061 2064 6174  arams, and a dat
+000090e0: 6120 736f 7572 6365 2028 6f66 7465 6e20  a source (often 
+000090f0: 6120 6669 6c65 6e61 6d65 292c 200d 0a20  a filename), .. 
+00009100: 2020 2020 2020 2072 6574 7572 6e73 2048         returns H
+00009110: 544d 4c2d 666f 726d 6174 7465 6420 7265  TML-formatted re
+00009120: 7375 6c74 7320 666f 7220 7468 6174 2076  sults for that v
+00009130: 6f78 656c 2e20 5468 6520 4854 4d4c 2069  oxel. The HTML i
+00009140: 7320 6170 7072 6f70 7269 6174 6520 0d0a  s appropriate ..
+00009150: 2020 2020 2020 2020 666f 7220 7468 6520          for the 
+00009160: 7778 2e48 746d 6c20 636f 6e74 726f 6c20  wx.Html control 
+00009170: 2877 6869 6368 2075 6e64 6572 7374 616e  (which understan
+00009180: 6420 6c69 6d69 7465 6420 4854 4d4c 2920  d limited HTML) 
+00009190: 6173 2077 656c 6c20 6173 2066 6f72 0d0a  as well as for..
+000091a0: 2020 2020 2020 2020 7772 6974 696e 6720          writing 
+000091b0: 746f 2061 2066 696c 652e 0d0a 0d0a 2020  to a file.....  
+000091c0: 2020 2020 2020 4966 2074 6865 2069 6d61        If the ima
+000091d0: 6765 2070 6172 616d 2069 7320 706f 7075  ge param is popu
+000091e0: 6c61 7465 642c 2069 7420 7368 6f75 6c64  lated, it should
+000091f0: 2062 6520 6120 7475 706c 6520 6f66 200d   be a tuple of .
+00009200: 0a20 2020 2020 2020 2028 6d69 6d65 5f74  .        (mime_t
+00009210: 7970 652c 2069 6d61 6765 5f64 6174 6129  ype, image_data)
+00009220: 2e20 5468 6520 666f 726d 6572 2073 686f  . The former sho
+00009230: 756c 6420 6265 2061 2073 7472 696e 6720  uld be a string 
+00009240: 6c69 6b65 2022 696d 6167 652f 706e 6722  like "image/png"
+00009250: 2e0d 0a20 2020 2020 2020 2054 6865 206c  ...        The l
+00009260: 6174 7465 7220 7368 6f75 6c64 2062 6520  atter should be 
+00009270: 6261 7365 3634 2d65 6e63 6f64 6564 2069  base64-encoded i
+00009280: 6d61 6765 2064 6174 612e 0d0a 2020 2020  mage data...    
+00009290: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000092a0: 2023 2046 6972 7374 2077 6520 6173 7365   # First we asse
+000092b0: 6d62 6c65 2074 6865 2064 6174 6120 7765  mble the data we
+000092c0: 206e 6565 642e 0d0a 2020 2020 2020 2020   need...        
+000092d0: 6e6d 6574 203d 206c 656e 2873 656c 662e  nmet = len(self.
+000092e0: 7365 742e 7072 696f 725f 6c69 7374 290d  set.prior_list).
+000092f0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00009300: 2020 206e 616d 6573 203d 2073 656c 662e     names = self.
+00009310: 7365 742e 7072 696f 725f 6c69 7374 0d0a  set.prior_list..
+00009320: 2020 2020 2020 2020 7265 7320 2020 3d20          res   = 
+00009330: 7365 6c66 2e66 6974 5f72 6573 756c 7473  self.fit_results
+00009340: 5b3a 2c76 6f78 656c 5b30 5d2c 766f 7865  [:,voxel[0],voxe
+00009350: 6c5b 315d 2c76 6f78 656c 5b32 5d5d 0d0a  l[1],voxel[2]]..
+00009360: 2020 2020 2020 2020 6372 616f 2020 3d20          crao  = 
+00009370: 7365 6c66 2e63 7261 6d65 725f 7261 6f5b  self.cramer_rao[
+00009380: 3a2c 766f 7865 6c5b 305d 2c76 6f78 656c  :,voxel[0],voxel
+00009390: 5b31 5d2c 766f 7865 6c5b 325d 5d0d 0a20  [1],voxel[2]].. 
+000093a0: 2020 2020 2020 2063 6f6e 6620 203d 2073         conf  = s
+000093b0: 656c 662e 636f 6e66 6964 656e 6365 5b3a  elf.confidence[:
+000093c0: 2c76 6f78 656c 5b30 5d2c 766f 7865 6c5b  ,voxel[0],voxel[
+000093d0: 315d 2c76 6f78 656c 5b32 5d5d 0d0a 2020  1],voxel[2]]..  
+000093e0: 2020 2020 2020 7374 6174 7320 3d20 7365        stats = se
+000093f0: 6c66 2e66 6974 5f73 7461 7473 5b3a 2c76  lf.fit_stats[:,v
+00009400: 6f78 656c 5b30 5d2c 766f 7865 6c5b 315d  oxel[0],voxel[1]
+00009410: 2c76 6f78 656c 5b32 5d5d 0d0a 2020 2020  ,voxel[2]]..    
+00009420: 2020 2020 2320 626f 7468 2063 7261 6d65      # both crame
+00009430: 722d 7261 6f20 616e 6420 636f 6e66 6964  r-rao and confid
+00009440: 656e 6365 2069 6e74 6572 7661 6c73 206d  ence intervals m
+00009450: 6179 2062 6520 6f66 662f 6f6e 0d0a 2020  ay be off/on..  
+00009460: 2020 2020 2020 6966 206c 656e 2863 7261        if len(cra
+00009470: 6f29 2021 3d20 6c65 6e28 7265 7329 3a0d  o) != len(res):.
+00009480: 0a20 2020 2020 2020 2020 2020 2063 7261  .            cra
+00009490: 6f20 3d20 7265 7320 2a20 300d 0a20 2020  o = res * 0..   
+000094a0: 2020 2020 2069 6620 6c65 6e28 636f 6e66       if len(conf
+000094b0: 2920 213d 206c 656e 2872 6573 293a 0d0a  ) != len(res):..
+000094c0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+000094d0: 203d 2072 6573 202a 2030 0d0a 0d0a 2020   = res * 0....  
+000094e0: 2020 2020 2020 7461 626c 6531 203d 205b        table1 = [
+000094f0: 5b27 4172 6561 2052 6573 756c 7473 272c  ['Area Results',
+00009500: 2027 4172 6561 272c 2027 2043 7252 616f   'Area', ' CrRao
+00009510: 5b25 5d27 2c20 2720 436e 6649 6e74 5b25  [%]', ' CnfInt[%
+00009520: 5d27 5d5d 0d0a 2020 2020 2020 2020 666f  ]']]..        fo
+00009530: 7220 692c 2069 7465 6d20 696e 2065 6e75  r i, item in enu
+00009540: 6d65 7261 7465 286e 616d 6573 293a 0d0a  merate(names):..
+00009550: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+00009560: 6531 2e61 7070 656e 6428 5b69 7465 6d2c  e1.append([item,
+00009570: 2072 6573 5b69 5d2c 2063 7261 6f5b 695d   res[i], crao[i]
+00009580: 2c20 636f 6e66 5b69 5d5d 290d 0a0d 0a20  , conf[i]]).... 
+00009590: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000095a0: 6574 2e6d 6163 726f 6d6f 6c5f 6d6f 6465  et.macromol_mode
+000095b0: 6c20 3d3d 2046 6974 4d61 6372 6f6d 6f6c  l == FitMacromol
+000095c0: 6563 756c 654d 6574 686f 642e 5349 4e47  eculeMethod.SING
+000095d0: 4c45 5f42 4153 4953 5f44 4154 4153 4554  LE_BASIS_DATASET
+000095e0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+000095f0: 6162 6c65 312e 6170 7065 6e64 285b 274d  able1.append(['M
+00009600: 4d6f 6c27 2c20 7265 735b 6e6d 6574 2a33  Mol', res[nmet*3
+00009610: 2b32 5d2c 2030 2e30 2c20 302e 305d 290d  +2], 0.0, 0.0]).
+00009620: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00009630: 2020 2020 2020 2074 6162 6c65 3120 3d20         table1 = 
+00009640: 5f70 7265 7474 795f 7370 6163 655f 7461  _pretty_space_ta
+00009650: 626c 6528 7461 626c 6531 2c20 706c 6163  ble(table1, plac
+00009660: 6573 3d34 290d 0a0d 0a20 2020 2020 2020  es=4)....       
+00009670: 2074 6162 6c65 3220 3d20 5b5b 2750 504d   table2 = [['PPM
+00009680: 2052 6573 756c 7473 272c 2027 5050 4d27   Results', 'PPM'
+00009690: 2c20 2720 4372 5261 6f5b 7070 6d5d 272c  , ' CrRao[ppm]',
+000096a0: 2027 2043 6e66 496e 745b 7070 6d5d 275d   ' CnfInt[ppm]']
+000096b0: 5d0d 0a20 2020 2020 2020 2066 6f72 2069  ]..        for i
+000096c0: 2c69 7465 6d20 696e 2065 6e75 6d65 7261  ,item in enumera
+000096d0: 7465 286e 616d 6573 293a 0d0a 2020 2020  te(names):..    
+000096e0: 2020 2020 2020 2020 7461 626c 6532 2e61          table2.a
+000096f0: 7070 656e 6428 5b69 7465 6d2c 2072 6573  ppend([item, res
+00009700: 5b69 2b6e 6d65 745d 2c20 6372 616f 5b69  [i+nmet], crao[i
+00009710: 2b6e 6d65 745d 2c20 636f 6e66 5b69 2b6e  +nmet], conf[i+n
+00009720: 6d65 745d 5d29 0d0a 0d0a 2020 2020 2020  met]])....      
+00009730: 2020 6966 2073 656c 662e 7365 742e 6d61    if self.set.ma
+00009740: 6372 6f6d 6f6c 5f6d 6f64 656c 203d 3d20  cromol_model == 
+00009750: 4669 744d 6163 726f 6d6f 6c65 6375 6c65  FitMacromolecule
+00009760: 4d65 7468 6f64 2e53 494e 474c 455f 4241  Method.SINGLE_BA
+00009770: 5349 535f 4441 5441 5345 543a 0d0a 2020  SIS_DATASET:..  
+00009780: 2020 2020 2020 2020 2020 7461 626c 6532            table2
+00009790: 2e61 7070 656e 6428 5b27 4d4d 6f6c 272c  .append(['MMol',
+000097a0: 2072 6573 5b6e 6d65 742a 332b 335d 2c20   res[nmet*3+3], 
+000097b0: 302e 302c 2030 2e30 5d29 0d0a 0d0a 2020  0.0, 0.0])....  
+000097c0: 2020 2020 2020 7461 626c 6532 203d 205f        table2 = _
+000097d0: 7072 6574 7479 5f73 7061 6365 5f74 6162  pretty_space_tab
+000097e0: 6c65 2874 6162 6c65 322c 2070 6c61 6365  le(table2, place
+000097f0: 733d 3429 0d0a 0d0a 2020 2020 2020 2020  s=4)....        
+00009800: 7461 626c 6532 6120 3d20 5b5b 2754 6220  table2a = [['Tb 
+00009810: 5265 7375 6c74 7327 2c20 2754 625b 7365  Results', 'Tb[se
+00009820: 635d 272c 2027 4c57 5b48 7a5d 272c 2027  c]', 'LW[Hz]', '
+00009830: 4372 5261 6f5b 7365 635d 272c 2027 2043  CrRao[sec]', ' C
+00009840: 6e66 496e 745b 7365 635d 275d 5d0d 0a20  nfInt[sec]']].. 
+00009850: 2020 2020 2020 2066 6f72 2069 2c69 7465         for i,ite
+00009860: 6d20 696e 2065 6e75 6d65 7261 7465 286e  m in enumerate(n
+00009870: 616d 6573 293a 0d0a 2020 2020 2020 2020  ames):..        
+00009880: 2020 2020 7461 626c 6532 612e 6170 7065      table2a.appe
+00009890: 6e64 285b 6974 656d 2c20 7265 735b 692b  nd([item, res[i+
+000098a0: 6e6d 6574 2a32 5d2c 206c 775b 695d 2c20  nmet*2], lw[i], 
+000098b0: 6372 616f 5b69 2b6e 6d65 742a 325d 2c20  crao[i+nmet*2], 
+000098c0: 636f 6e66 5b69 2b6e 6d65 742a 325d 5d29  conf[i+nmet*2]])
+000098d0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
+000098e0: 656c 662e 7365 742e 6d61 6372 6f6d 6f6c  elf.set.macromol
+000098f0: 5f6d 6f64 656c 203d 3d20 4669 744d 6163  _model == FitMac
+00009900: 726f 6d6f 6c65 6375 6c65 4d65 7468 6f64  romoleculeMethod
+00009910: 2e53 494e 474c 455f 4241 5349 535f 4441  .SINGLE_BASIS_DA
+00009920: 5441 5345 543a 0d0a 2020 2020 2020 2020  TASET:..        
+00009930: 2020 2020 7461 626c 6532 612e 6170 7065      table2a.appe
+00009940: 6e64 285b 274d 4d6f 6c27 2c20 7265 735b  nd(['MMol', res[
+00009950: 6e6d 6574 2a33 2b34 5d2c 2030 2e30 2c20  nmet*3+4], 0.0, 
+00009960: 302e 305d 290d 0a0d 0a20 2020 2020 2020  0.0])....       
+00009970: 2074 6162 6c65 3261 203d 205f 7072 6574   table2a = _pret
+00009980: 7479 5f73 7061 6365 5f74 6162 6c65 2874  ty_space_table(t
+00009990: 6162 6c65 3261 2c20 706c 6163 6573 3d34  able2a, places=4
+000099a0: 290d 0a0d 0a20 2020 2020 2020 2074 6162  )....        tab
+000099b0: 6c65 3320 3d20 2020 2020 5b5b 2747 6c6f  le3 =     [['Glo
+000099c0: 6261 6c20 5265 7375 6c74 7327 2c20 2756  bal Results', 'V
+000099d0: 616c 7565 272c 2027 2043 7252 616f 5b64  alue', ' CrRao[d
+000099e0: 656c 7461 5d27 2c20 2720 436e 6649 6e74  elta]', ' CnfInt
+000099f0: 5b25 5d27 5d5d 0d0a 2020 2020 2020 2020  [%]']]..        
+00009a00: 7461 626c 6533 2e61 7070 656e 6428 5b27  table3.append(['
+00009a10: 5068 6173 6530 272c 2020 2020 2072 6573  Phase0',     res
+00009a20: 5b6e 6d65 742a 332b 305d 2c20 6372 616f  [nmet*3+0], crao
+00009a30: 5b6e 6d65 742a 332b 305d 2c20 636f 6e66  [nmet*3+0], conf
+00009a40: 5b6e 6d65 742a 332b 305d 205d 290d 0a20  [nmet*3+0] ]).. 
+00009a50: 2020 2020 2020 2074 6162 6c65 332e 6170         table3.ap
+00009a60: 7065 6e64 285b 2750 6861 7365 3127 2c20  pend(['Phase1', 
+00009a70: 2020 2020 7265 735b 6e6d 6574 2a33 2b31      res[nmet*3+1
+00009a80: 5d2c 2063 7261 6f5b 6e6d 6574 2a33 2b31  ], crao[nmet*3+1
+00009a90: 5d2c 2063 6f6e 665b 6e6d 6574 2a33 2b31  ], conf[nmet*3+1
+00009aa0: 5d20 5d29 0d0a 2020 2020 2020 2020 7461  ] ])..        ta
+00009ab0: 626c 6533 203d 205f 7072 6574 7479 5f73  ble3 = _pretty_s
+00009ac0: 7061 6365 5f74 6162 6c65 2874 6162 6c65  pace_table(table
+00009ad0: 332c 2070 6c61 6365 733d 3529 0d0a 2020  3, places=5)..  
+00009ae0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00009af0: 7461 626c 6534 203d 205b 5b27 4361 6c63  table4 = [['Calc
+00009b00: 756c 6174 696f 6e20 5265 7375 6c74 7327  ulation Results'
+00009b10: 2c20 2720 5661 6c75 6527 2c20 2720 204d  , ' Value', '  M
+00009b20: 6178 204c 5727 2c20 2720 204d 696e 204c  ax LW', '  Min L
+00009b30: 5727 5d5d 0d0a 2020 2020 2020 2020 7461  W']]..        ta
+00009b40: 626c 6534 2e61 7070 656e 6428 5b27 4368  ble4.append(['Ch
+00009b50: 6953 7175 6172 6527 2c20 7374 6174 735b  iSquare', stats[
+00009b60: 305d 2c20 2720 272c 2027 2027 5d29 0d0a  0], ' ', ' '])..
+00009b70: 2020 2020 2020 2020 7461 626c 6534 2e61          table4.a
+00009b80: 7070 656e 6428 5b27 5765 6967 6874 6564  ppend(['Weighted
+00009b90: 2043 6869 5371 7561 7265 272c 2073 7461   ChiSquare', sta
+00009ba0: 7473 5b31 5d2c 2027 2027 2c20 2720 275d  ts[1], ' ', ' ']
+00009bb0: 290d 0a20 2020 2020 2020 206d 6174 6865  )..        mathe
+00009bc0: 7272 203d 2073 7472 2873 7461 7473 5b32  rr = str(stats[2
+00009bd0: 5d20 213d 2030 290d 0a20 2020 2020 2020  ] != 0)..       
+00009be0: 2074 6162 6c65 342e 6170 7065 6e64 285b   table4.append([
+00009bf0: 274d 6174 6820 4669 6e69 7465 2045 7272  'Math Finite Err
+00009c00: 6f72 272c 206d 6174 6865 7272 2c20 2720  or', matherr, ' 
+00009c10: 272c 2027 2027 5d29 0d0a 2020 2020 2020  ', ' '])..      
+00009c20: 2020 7461 626c 6534 203d 205f 7072 6574    table4 = _pret
+00009c30: 7479 5f73 7061 6365 5f74 6162 6c65 2874  ty_space_table(t
+00009c40: 6162 6c65 342c 2070 6c61 6365 733d 3529  able4, places=5)
+00009c50: 0d0a 0d0a 2020 2020 2020 2020 2320 4e6f  ....        # No
+00009c60: 7720 7468 6174 2074 6865 2064 6174 6120  w that the data 
+00009c70: 6973 2061 7373 656d 626c 6564 2c20 7765  is assembled, we
+00009c80: 2048 544d 4c2d 6966 7920 6974 2e0d 0a20   HTML-ify it... 
+00009c90: 2020 2020 2020 2068 746d 6c20 3d20 456c         html = El
+00009ca0: 656d 656e 7454 7265 652e 456c 656d 656e  ementTree.Elemen
+00009cb0: 7428 2268 746d 6c22 290d 0a20 2020 2020  t("html")..     
+00009cc0: 2020 2068 6561 6420 3d20 456c 656d 656e     head = Elemen
+00009cd0: 7454 7265 652e 5375 6245 6c65 6d65 6e74  tTree.SubElement
+00009ce0: 2868 746d 6c2c 2022 6865 6164 2229 0d0a  (html, "head")..
+00009cf0: 2020 2020 2020 2020 7374 796c 6520 3d20          style = 
+00009d00: 7574 696c 5f78 6d6c 2e54 6578 7453 7562  util_xml.TextSub
+00009d10: 456c 656d 656e 7428 6865 6164 2c20 2273  Element(head, "s
+00009d20: 7479 6c65 222c 205f 4353 5329 0d0a 2020  tyle", _CSS)..  
+00009d30: 2020 2020 2020 7374 796c 652e 7365 7428        style.set(
+00009d40: 2274 7970 6522 2c20 2274 6578 742f 6373  "type", "text/cs
+00009d50: 7322 290d 0a0d 0a20 2020 2020 2020 2062  s")....        b
+00009d60: 6f64 7920 3d20 456c 656d 656e 7454 7265  ody = ElementTre
+00009d70: 652e 5375 6245 6c65 6d65 6e74 2868 746d  e.SubElement(htm
+00009d80: 6c2c 2022 626f 6479 2229 0d0a 2020 2020  l, "body")..    
+00009d90: 2020 2020 0d0a 2020 2020 2020 2020 7574      ..        ut
+00009da0: 696c 5f78 6d6c 2e54 6578 7453 7562 456c  il_xml.TextSubEl
+00009db0: 656d 656e 7428 626f 6479 2c20 2268 3222  ement(body, "h2"
+00009dc0: 2c20 2241 6e61 6c79 7369 7320 4669 742d  , "Analysis Fit-
+00009dd0: 4769 736f 2052 6573 756c 7473 2229 0d0a  Giso Results")..
+00009de0: 0d0a 2020 2020 2020 2020 655f 6469 7620  ..        e_div 
+00009df0: 3d20 456c 656d 656e 7454 7265 652e 5375  = ElementTree.Su
+00009e00: 6245 6c65 6d65 6e74 2862 6f64 792c 2022  bElement(body, "
+00009e10: 6469 7622 290d 0a0d 0a20 2020 2020 2020  div")....       
+00009e20: 2069 6620 6461 7461 5f73 6f75 7263 653a   if data_source:
+00009e30: 0d0a 2020 2020 2020 2020 2020 2020 655f  ..            e_
+00009e40: 7474 203d 2075 7469 6c5f 786d 6c2e 5465  tt = util_xml.Te
+00009e50: 7874 5375 6245 6c65 6d65 6e74 2865 5f64  xtSubElement(e_d
+00009e60: 6976 2c20 2274 7422 2c20 2244 6174 6120  iv, "tt", "Data 
+00009e70: 536f 7572 6365 3a20 2229 0d0a 2020 2020  Source: ")..    
+00009e80: 2020 2020 2020 2020 7574 696c 5f78 6d6c          util_xml
+00009e90: 2e54 6578 7453 7562 456c 656d 656e 7428  .TextSubElement(
+00009ea0: 655f 7474 2c20 2273 6d61 6c6c 222c 2064  e_tt, "small", d
+00009eb0: 6174 615f 736f 7572 6365 290d 0a20 2020  ata_source)..   
+00009ec0: 2020 2020 2020 2020 2045 6c65 6d65 6e74           Element
+00009ed0: 5472 6565 2e53 7562 456c 656d 656e 7428  Tree.SubElement(
+00009ee0: 655f 6469 762c 2022 6272 2229 0d0a 2020  e_div, "br")..  
+00009ef0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00009f00: 2020 2020 766f 7865 6c20 3d20 5b78 202b      voxel = [x +
+00009f10: 2031 2066 6f72 2078 2069 6e20 766f 7865   1 for x in voxe
+00009f20: 6c5d 0d0a 2020 2020 2020 2020 7574 696c  l]..        util
+00009f30: 5f78 6d6c 2e54 6578 7453 7562 456c 656d  _xml.TextSubElem
+00009f40: 656e 7428 655f 6469 762c 2022 7474 222c  ent(e_div, "tt",
+00009f50: 2027 566f 7865 6c3a 2028 2564 2c25 642c   'Voxel: (%d,%d,
+00009f60: 2564 2927 2025 2074 7570 6c65 2876 6f78  %d)' % tuple(vox
+00009f70: 656c 2929 0d0a 0d0a 2020 2020 2020 2020  el))....        
+00009f80: 6966 2069 6d61 6765 3a0d 0a20 2020 2020  if image:..     
+00009f90: 2020 2020 2020 2023 2049 6620 7468 6572         # If ther
+00009fa0: 6527 7320 696d 6167 6520 6461 7461 2c20  e's image data, 
+00009fb0: 7765 2061 7373 756d 6520 7468 6174 2074  we assume that t
+00009fc0: 6869 7320 7769 6c6c 2062 6520 7772 6974  his will be writ
+00009fd0: 7465 6e20 746f 200d 0a20 2020 2020 2020  ten to ..       
+00009fe0: 2020 2020 2023 2061 2066 696c 6520 666f       # a file fo
+00009ff0: 7220 6469 7370 6c61 7920 696e 2061 2070  r display in a p
+0000a000: 726f 7065 7220 6272 6f77 7365 722c 2073  roper browser, s
+0000a010: 6f20 7765 2063 616e 2075 7365 2073 6c69  o we can use sli
+0000a020: 6768 746c 790d 0a20 2020 2020 2020 2020  ghtly..         
+0000a030: 2020 2023 2066 616e 6369 6572 2048 544d     # fancier HTM
+0000a040: 4c2e 0d0a 2020 2020 2020 2020 2020 2020  L...            
+0000a050: 6d69 6d65 5f74 7970 652c 2069 6d61 6765  mime_type, image
+0000a060: 5f64 6174 6120 3d20 696d 6167 650d 0a0d  _data = image...
+0000a070: 0a20 2020 2020 2020 2020 2020 2065 5f64  .            e_d
+0000a080: 6976 203d 2045 6c65 6d65 6e74 5472 6565  iv = ElementTree
+0000a090: 2e53 7562 456c 656d 656e 7428 626f 6479  .SubElement(body
+0000a0a0: 2c20 2264 6976 222c 200d 0a20 2020 2020  , "div", ..     
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0d0: 2020 2020 2020 7b20 2269 6422 203a 2022        { "id" : "
+0000a0e0: 696d 6167 6522 2c0d 0a20 2020 2020 2020  image",..       
+0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a110: 2020 2020 2020 2273 7479 6c65 2220 3a20        "style" : 
+0000a120: 2266 6c6f 6174 3a20 7269 6768 743b 2077  "float: right; w
+0000a130: 6964 7468 3a20 3530 2522 2c0d 0a20 2020  idth: 50%",..   
+0000a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a160: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a190: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+0000a1a0: 2020 2020 2020 655f 6469 762e 6170 7065        e_div.appe
+0000a1b0: 6e64 2845 6c65 6d65 6e74 5472 6565 2e43  nd(ElementTree.C
+0000a1c0: 6f6d 6d65 6e74 285f 4945 5f49 4e43 4150  omment(_IE_INCAP
+0000a1d0: 4142 4c45 5f4d 5347 2929 0d0a 0d0a 2020  ABLE_MSG))....  
+0000a1e0: 2020 2020 2020 2020 2020 2320 496e 206f            # In o
+0000a1f0: 7264 6572 2074 6f20 6b65 6570 2074 6865  rder to keep the
+0000a200: 2048 544d 4c20 2b20 696d 6167 6520 696e   HTML + image in
+0000a210: 206f 6e65 2066 696c 652c 2077 6520 7573   one file, we us
+0000a220: 6520 7468 650d 0a20 2020 2020 2020 2020  e the..         
+0000a230: 2020 2023 206c 6974 746c 652d 6b6e 6f77     # little-know
+0000a240: 6e20 2264 6174 6122 2073 6368 656d 652e  n "data" scheme.
+0000a250: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000a260: 7265 663a 2068 7474 703a 2f2f 656e 2e77  ref: http://en.w
+0000a270: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+0000a280: 692f 4461 7461 5f55 5249 5f73 6368 656d  i/Data_URI_schem
+0000a290: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
+0000a2a0: 7263 203d 2022 6461 7461 3a25 733b 6261  rc = "data:%s;ba
+0000a2b0: 7365 3634 2c25 7322 2025 2028 6d69 6d65  se64,%s" % (mime
+0000a2c0: 5f74 7970 652c 2069 6d61 6765 5f64 6174  _type, image_dat
+0000a2d0: 6129 0d0a 0d0a 2020 2020 2020 2020 2020  a)....          
+0000a2e0: 2020 456c 656d 656e 7454 7265 652e 5375    ElementTree.Su
+0000a2f0: 6245 6c65 6d65 6e74 2865 5f64 6976 2c20  bElement(e_div, 
+0000a300: 2269 6d67 222c 200d 0a20 2020 2020 2020  "img", ..       
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a330: 2020 2020 7b22 7374 796c 6522 203a 2022      {"style" : "
+0000a340: 7769 6474 683a 2039 3025 222c 0d0a 2020  width: 90%",..  
+0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a370: 2020 2020 2020 2020 2020 2273 7263 2220            "src" 
+0000a380: 3a20 7372 630d 0a20 2020 2020 2020 2020  : src..         
+0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3b0: 2020 207d 290d 0a0d 0a20 2020 2020 2020     })....       
+0000a3c0: 2065 5f64 6976 203d 2045 6c65 6d65 6e74   e_div = Element
+0000a3d0: 5472 6565 2e53 7562 456c 656d 656e 7428  Tree.SubElement(
+0000a3e0: 626f 6479 2c20 2264 6976 222c 207b 2269  body, "div", {"i
+0000a3f0: 6422 203a 2022 7461 626c 6522 7d29 0d0a  d" : "table"})..
+0000a400: 0d0a 2020 2020 2020 2020 7461 626c 6573  ..        tables
+0000a410: 203d 2028 7461 626c 6531 2c20 7461 626c   = (table1, tabl
+0000a420: 6532 2c20 7461 626c 6532 612c 2074 6162  e2, table2a, tab
+0000a430: 6c65 332c 2074 6162 6c65 3429 0d0a 0d0a  le3, table4)....
+0000a440: 2020 2020 2020 2020 666f 7220 7461 626c          for tabl
+0000a450: 6520 696e 2074 6162 6c65 733a 0d0a 2020  e in tables:..  
+0000a460: 2020 2020 2020 2020 2020 7469 746c 6520            title 
+0000a470: 3d20 7461 626c 655b 305d 0d0a 2020 2020  = table[0]..    
+0000a480: 2020 2020 2020 2020 655f 7072 6520 3d20          e_pre = 
+0000a490: 456c 656d 656e 7454 7265 652e 5375 6245  ElementTree.SubE
+0000a4a0: 6c65 6d65 6e74 2865 5f64 6976 2c20 2270  lement(e_div, "p
+0000a4b0: 7265 2229 0d0a 2020 2020 2020 2020 2020  re")..          
+0000a4c0: 2020 655f 7520 2020 3d20 456c 656d 656e    e_u   = Elemen
+0000a4d0: 7454 7265 652e 5375 6245 6c65 6d65 6e74  tTree.SubElement
+0000a4e0: 2865 5f70 7265 2c20 2275 2229 0d0a 2020  (e_pre, "u")..  
+0000a4f0: 2020 2020 2020 2020 2020 7574 696c 5f78            util_x
+0000a500: 6d6c 2e54 6578 7453 7562 456c 656d 656e  ml.TextSubElemen
+0000a510: 7428 655f 752c 2022 6222 2c20 7469 746c  t(e_u, "b", titl
+0000a520: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+0000a530: 6520 2020 2020 3d20 7574 696c 5f78 6d6c  e     = util_xml
+0000a540: 2e54 6578 7453 7562 456c 656d 656e 7428  .TextSubElement(
+0000a550: 655f 6469 762c 2022 7072 6522 2c20 275c  e_div, "pre", '\
+0000a560: 6e27 2e6a 6f69 6e28 7461 626c 655b 313a  n'.join(table[1:
+0000a570: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+0000a580: 200d 0a20 2020 2020 2020 2023 204b 6565   ..        # Kee
+0000a590: 7020 696e 206d 696e 6420 7468 6174 2048  p in mind that H
+0000a5a0: 544d 4c20 6973 2077 6869 7465 7370 6163  TML is whitespac
+0000a5b0: 6520 7365 6e73 6974 6976 652c 2061 6e64  e sensitive, and
+0000a5c0: 2069 6620 796f 7520 6361 6c6c 200d 0a20   if you call .. 
+0000a5d0: 2020 2020 2020 2023 2075 7469 6c5f 786d         # util_xm
+0000a5e0: 6c2e 696e 6465 6e74 2829 206f 6e20 7468  l.indent() on th
+0000a5f0: 6520 4854 4d4c 2c20 6974 2077 696c 6c20  e HTML, it will 
+0000a600: 6368 616e 6765 2074 6865 2066 6f72 6d61  change the forma
+0000a610: 7474 696e 672e 0d0a 0d0a 2020 2020 2020  tting.....      
+0000a620: 2020 7265 7475 726e 2045 6c65 6d65 6e74    return Element
+0000a630: 5472 6565 2e74 6f73 7472 696e 6728 6874  Tree.tostring(ht
+0000a640: 6d6c 290d 0a0d 0a0d 0a20 2020 2064 6566  ml)......    def
+0000a650: 2072 6573 756c 7473 5f61 735f 6373 7628   results_as_csv(
+0000a660: 7365 6c66 2c20 766f 7865 6c2c 206c 773d  self, voxel, lw=
+0000a670: 302e 302c 206c 776d 696e 3d30 2e30 2c20  0.0, lwmin=0.0, 
+0000a680: 6c77 6d61 783d 302e 302c 2073 6f75 7263  lwmax=0.0, sourc
+0000a690: 653d 2222 2c20 6473 6574 6e61 6d65 3d22  e="", dsetname="
+0000a6a0: 2229 3a0d 0a20 2020 2020 2020 2022 2222  "):..        """
+0000a6b0: 0d0a 2020 2020 2020 2020 4769 7665 6e20  ..        Given 
+0000a6c0: 6120 766f 7865 6c2c 206c 696e 6577 6964  a voxel, linewid
+0000a6d0: 7468 2070 6172 616d 732c 2061 6e64 2061  th params, and a
+0000a6e0: 2064 6174 6120 736f 7572 6365 2028 6f66   data source (of
+0000a6f0: 7465 6e20 6120 6669 6c65 6e61 6d65 292c  ten a filename),
+0000a700: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+0000a710: 6e73 2043 5356 2d66 6f72 6d61 7474 6564  ns CSV-formatted
+0000a720: 2028 636f 6d6d 6120 7365 7061 7261 7465   (comma separate
+0000a730: 6420 7661 7269 6162 6c65 7329 7374 7269  d variables)stri
+0000a740: 6e67 2063 6f6e 7461 696e 696e 6720 626f  ng containing bo
+0000a750: 7468 0d0a 2020 2020 2020 2020 7468 6520  th..        the 
+0000a760: 766f 7865 6c20 6669 7474 696e 6720 7265  voxel fitting re
+0000a770: 7375 6c74 7320 616e 6420 6865 6164 6572  sults and header
+0000a780: 2073 7472 696e 6720 6465 7363 7269 7074   string descript
+0000a790: 696f 6e73 2066 6f72 2065 6163 6820 0d0a  ions for each ..
+0000a7a0: 2020 2020 2020 2020 636f 6c75 6d6e 2e0d          column..
+0000a7b0: 0a0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+0000a7c0: 2020 2020 2020 2020 6864 7220 3d20 5b5d          hdr = []
+0000a7d0: 0d0a 2020 2020 2020 2020 7661 6c20 3d20  ..        val = 
+0000a7e0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 6864  []....        hd
+0000a7f0: 722e 6170 7065 6e64 2827 4669 6c65 6e61  r.append('Filena
+0000a800: 6d65 2729 2020 200d 0a20 2020 2020 2020  me')   ..       
+0000a810: 2073 6f75 7263 6520 3d20 736f 7572 6365   source = source
+0000a820: 2e72 6570 6c61 6365 2822 2c22 2c22 5f22  .replace(",","_"
+0000a830: 2920 2020 2020 2320 736f 6d65 2075 7365  )     # some use
+0000a840: 7273 2068 6176 6520 636f 6d6d 6173 2069  rs have commas i
+0000a850: 6e20 6669 6c65 6e61 6d65 7320 0d0a 2020  n filenames ..  
+0000a860: 2020 2020 2020 7661 6c2e 6170 7065 6e64        val.append
+0000a870: 2873 6f75 7263 6529 0d0a 0d0a 2020 2020  (source)....    
+0000a880: 2020 2020 6864 722e 6170 7065 6e64 2827      hdr.append('
+0000a890: 4461 7461 7365 7420 4e61 6d65 2729 2020  Dataset Name')  
+0000a8a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a8b0: 6473 6574 6e61 6d65 203d 2064 7365 746e  dsetname = dsetn
+0000a8c0: 616d 652e 7265 706c 6163 6528 222c 222c  ame.replace(",",
+0000a8d0: 225f 2229 2023 2073 6f6d 6520 7573 6572  "_") # some user
+0000a8e0: 7320 6861 7665 2063 6f6d 6d61 7320 696e  s have commas in
+0000a8f0: 2066 696c 656e 616d 6573 2020 2020 0d0a   filenames    ..
+0000a900: 2020 2020 2020 2020 7661 6c2e 6170 7065          val.appe
+0000a910: 6e64 2864 7365 746e 616d 6529 0d0a 2020  nd(dsetname)..  
+0000a920: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a930: 6864 722e 6170 7065 6e64 2827 566f 7865  hdr.append('Voxe
+0000a940: 6c27 290d 0a20 2020 2020 2020 2076 616c  l')..        val
+0000a950: 2e61 7070 656e 6428 7374 7228 766f 7865  .append(str(voxe
+0000a960: 6c5b 305d 292b 2720 272b 7374 7228 766f  l[0])+' '+str(vo
+0000a970: 7865 6c5b 315d 292b 2720 272b 7374 7228  xel[1])+' '+str(
+0000a980: 766f 7865 6c5b 325d 2929 0d0a 2020 2020  voxel[2]))..    
+0000a990: 2020 2020 0d0a 2020 2020 2020 2020 6e6d      ..        nm
+0000a9a0: 6574 203d 206c 656e 2873 656c 662e 7365  et = len(self.se
+0000a9b0: 742e 7072 696f 725f 6c69 7374 290d 0a20  t.prior_list).. 
+0000a9c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000a9d0: 206e 616d 6573 203d 2073 656c 662e 7365   names = self.se
+0000a9e0: 742e 7072 696f 725f 6c69 7374 0d0a 2020  t.prior_list..  
+0000a9f0: 2020 2020 2020 7265 7320 2020 3d20 7365        res   = se
+0000aa00: 6c66 2e66 6974 5f72 6573 756c 7473 5b3a  lf.fit_results[:
+0000aa10: 2c76 6f78 656c 5b30 5d2c 766f 7865 6c5b  ,voxel[0],voxel[
+0000aa20: 315d 2c76 6f78 656c 5b32 5d5d 0d0a 2020  1],voxel[2]]..  
+0000aa30: 2020 2020 2020 6372 616f 2020 3d20 7365        crao  = se
+0000aa40: 6c66 2e63 7261 6d65 725f 7261 6f5b 203a  lf.cramer_rao[ :
+0000aa50: 2c76 6f78 656c 5b30 5d2c 766f 7865 6c5b  ,voxel[0],voxel[
+0000aa60: 315d 2c76 6f78 656c 5b32 5d5d 0d0a 2020  1],voxel[2]]..  
+0000aa70: 2020 2020 2020 636f 6e66 2020 3d20 7365        conf  = se
+0000aa80: 6c66 2e63 6f6e 6669 6465 6e63 655b 203a  lf.confidence[ :
+0000aa90: 2c76 6f78 656c 5b30 5d2c 766f 7865 6c5b  ,voxel[0],voxel[
+0000aaa0: 315d 2c76 6f78 656c 5b32 5d5d 0d0a 2020  1],voxel[2]]..  
+0000aab0: 2020 2020 2020 7374 6174 7320 3d20 7365        stats = se
+0000aac0: 6c66 2e66 6974 5f73 7461 7473 5b20 203a  lf.fit_stats[  :
+0000aad0: 2c76 6f78 656c 5b30 5d2c 766f 7865 6c5b  ,voxel[0],voxel[
+0000aae0: 315d 2c76 6f78 656c 5b32 5d5d 0d0a 2020  1],voxel[2]]..  
+0000aaf0: 2020 2020 2020 2320 626f 7468 2063 7261        # both cra
+0000ab00: 6d65 722d 7261 6f20 616e 6420 636f 6e66  mer-rao and conf
+0000ab10: 6964 656e 6365 2069 6e74 6572 7661 6c73  idence intervals
+0000ab20: 206d 6179 2062 6520 6f66 662f 6f6e 0d0a   may be off/on..
+0000ab30: 2020 2020 2020 2020 6966 206c 656e 2863          if len(c
+0000ab40: 7261 6f29 2021 3d20 6c65 6e28 7265 7329  rao) != len(res)
+0000ab50: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+0000ab60: 7261 6f20 3d20 7265 7320 2a20 300d 0a20  rao = res * 0.. 
+0000ab70: 2020 2020 2020 2069 6620 6c65 6e28 636f         if len(co
+0000ab80: 6e66 2920 213d 206c 656e 2872 6573 293a  nf) != len(res):
+0000ab90: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+0000aba0: 6e66 203d 2072 6573 202a 2030 0d0a 0d0a  nf = res * 0....
+0000abb0: 2020 2020 2020 2020 666f 7220 692c 2069          for i, i
+0000abc0: 7465 6d20 696e 2065 6e75 6d65 7261 7465  tem in enumerate
+0000abd0: 286e 616d 6573 293a 0d0a 2020 2020 2020  (names):..      
+0000abe0: 2020 2020 2020 6864 722e 6170 7065 6e64        hdr.append
+0000abf0: 2827 4172 6561 2027 2b69 7465 6d29 2020  ('Area '+item)  
+0000ac00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000ac10: 2020 2020 6864 722e 6170 7065 6e64 2827      hdr.append('
+0000ac20: 4372 5261 6f5b 255d 2729 2020 2020 2020  CrRao[%]')      
+0000ac30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ac40: 6864 722e 6170 7065 6e64 2827 436e 6649  hdr.append('CnfI
+0000ac50: 6e74 5b25 5d27 2920 2020 2020 2020 200d  nt[%]')        .
+0000ac60: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+0000ac70: 2e61 7070 656e 6428 7374 7228 7265 735b  .append(str(res[
+0000ac80: 695d 2929 0d0a 2020 2020 2020 2020 2020  i]))..          
+0000ac90: 2020 7661 6c2e 6170 7065 6e64 2873 7472    val.append(str
+0000aca0: 2863 7261 6f5b 695d 2929 0d0a 2020 2020  (crao[i]))..    
+0000acb0: 2020 2020 2020 2020 7661 6c2e 6170 7065          val.appe
+0000acc0: 6e64 2873 7472 2863 6f6e 665b 695d 2929  nd(str(conf[i]))
+0000acd0: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+0000ace0: 692c 6974 656d 2069 6e20 656e 756d 6572  i,item in enumer
+0000acf0: 6174 6528 6e61 6d65 7329 3a0d 0a20 2020  ate(names):..   
+0000ad00: 2020 2020 2020 2020 2068 6472 2e61 7070           hdr.app
+0000ad10: 656e 6428 2750 504d 2027 2b69 7465 6d29  end('PPM '+item)
+0000ad20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000ad30: 2020 2020 2020 6864 722e 6170 7065 6e64        hdr.append
+0000ad40: 2827 4372 5261 6f5b 255d 2729 2020 2020  ('CrRao[%]')    
+0000ad50: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ad60: 2020 6864 722e 6170 7065 6e64 2827 436e    hdr.append('Cn
+0000ad70: 6649 6e74 5b25 5d27 2920 2020 2020 2020  fInt[%]')       
+0000ad80: 200d 0a20 2020 2020 2020 2020 2020 2076   ..            v
+0000ad90: 616c 2e61 7070 656e 6428 7374 7228 7265  al.append(str(re
+0000ada0: 735b 692b 6e6d 6574 5d29 290d 0a20 2020  s[i+nmet]))..   
+0000adb0: 2020 2020 2020 2020 2076 616c 2e61 7070           val.app
+0000adc0: 656e 6428 7374 7228 6372 616f 5b69 2b6e  end(str(crao[i+n
+0000add0: 6d65 745d 2929 0d0a 2020 2020 2020 2020  met]))..        
+0000ade0: 2020 2020 7661 6c2e 6170 7065 6e64 2873      val.append(s
+0000adf0: 7472 2863 6f6e 665b 692b 6e6d 6574 5d29  tr(conf[i+nmet])
+0000ae00: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
+0000ae10: 2069 2c69 7465 6d20 696e 2065 6e75 6d65   i,item in enume
+0000ae20: 7261 7465 286e 616d 6573 293a 0d0a 2020  rate(names):..  
+0000ae30: 2020 2020 2020 2020 2020 6864 722e 6170            hdr.ap
+0000ae40: 7065 6e64 2827 5462 5b73 6563 5d27 2b69  pend('Tb[sec]'+i
+0000ae50: 7465 6d29 2020 2020 2020 2020 0d0a 2020  tem)        ..  
+0000ae60: 2020 2020 2020 2020 2020 6864 722e 6170            hdr.ap
+0000ae70: 7065 6e64 2827 4c57 5b48 7a5d 272b 6974  pend('LW[Hz]'+it
+0000ae80: 656d 2920 2020 2020 2020 200d 0a20 2020  em)        ..   
+0000ae90: 2020 2020 2020 2020 2068 6472 2e61 7070           hdr.app
+0000aea0: 656e 6428 2743 7252 616f 5b25 5d27 2920  end('CrRao[%]') 
+0000aeb0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000aec0: 2020 2020 2068 6472 2e61 7070 656e 6428       hdr.append(
+0000aed0: 2743 6e66 496e 745b 255d 2729 2020 2020  'CnfInt[%]')    
+0000aee0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000aef0: 2020 7661 6c2e 6170 7065 6e64 2873 7472    val.append(str
+0000af00: 2872 6573 5b69 2b6e 6d65 742a 325d 2929  (res[i+nmet*2]))
+0000af10: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+0000af20: 6c2e 6170 7065 6e64 2873 7472 286c 775b  l.append(str(lw[
+0000af30: 695d 2929 0d0a 2020 2020 2020 2020 2020  i]))..          
+0000af40: 2020 7661 6c2e 6170 7065 6e64 2873 7472    val.append(str
+0000af50: 2863 7261 6f5b 692b 6e6d 6574 2a32 5d29  (crao[i+nmet*2])
+0000af60: 290d 0a20 2020 2020 2020 2020 2020 2076  )..            v
+0000af70: 616c 2e61 7070 656e 6428 7374 7228 636f  al.append(str(co
+0000af80: 6e66 5b69 2b6e 6d65 742a 325d 2929 0d0a  nf[i+nmet*2]))..
+0000af90: 0d0a 2020 2020 2020 2020 6864 722e 6170  ..        hdr.ap
+0000afa0: 7065 6e64 2827 5068 6173 6530 2027 2920  pend('Phase0 ') 
+0000afb0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000afc0: 2068 6472 2e61 7070 656e 6428 2743 7252   hdr.append('CrR
+0000afd0: 616f 5b25 5d27 2920 2020 2020 2020 200d  ao[%]')        .
+0000afe0: 0a20 2020 2020 2020 2068 6472 2e61 7070  .        hdr.app
+0000aff0: 656e 6428 2743 6e66 496e 745b 255d 2729  end('CnfInt[%]')
+0000b000: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000b010: 2020 7661 6c2e 6170 7065 6e64 2873 7472    val.append(str
+0000b020: 2872 6573 5b6e 6d65 742a 332b 305d 2929  (res[nmet*3+0]))
+0000b030: 0d0a 2020 2020 2020 2020 7661 6c2e 6170  ..        val.ap
+0000b040: 7065 6e64 2873 7472 2863 7261 6f5b 6e6d  pend(str(crao[nm
+0000b050: 6574 2a33 2b30 5d29 290d 0a20 2020 2020  et*3+0]))..     
+0000b060: 2020 2076 616c 2e61 7070 656e 6428 7374     val.append(st
+0000b070: 7228 636f 6e66 5b6e 6d65 742a 332b 305d  r(conf[nmet*3+0]
+0000b080: 2929 0d0a 0d0a 2020 2020 2020 2020 6864  ))....        hd
+0000b090: 722e 6170 7065 6e64 2827 5068 6173 6531  r.append('Phase1
+0000b0a0: 2027 2920 2020 2020 2020 200d 0a20 2020   ')        ..   
+0000b0b0: 2020 2020 2068 6472 2e61 7070 656e 6428       hdr.append(
+0000b0c0: 2743 7252 616f 5b25 5d27 2920 2020 2020  'CrRao[%]')     
+0000b0d0: 2020 200d 0a20 2020 2020 2020 2068 6472     ..        hdr
+0000b0e0: 2e61 7070 656e 6428 2743 6e66 496e 745b  .append('CnfInt[
+0000b0f0: 255d 2729 2020 2020 2020 2020 0d0a 2020  %]')        ..  
+0000b100: 2020 2020 2020 7661 6c2e 6170 7065 6e64        val.append
+0000b110: 2873 7472 2872 6573 5b6e 6d65 742a 332b  (str(res[nmet*3+
+0000b120: 315d 2929 0d0a 2020 2020 2020 2020 7661  1]))..        va
+0000b130: 6c2e 6170 7065 6e64 2873 7472 2863 7261  l.append(str(cra
+0000b140: 6f5b 6e6d 6574 2a33 2b31 5d29 290d 0a20  o[nmet*3+1])).. 
+0000b150: 2020 2020 2020 2076 616c 2e61 7070 656e         val.appen
+0000b160: 6428 7374 7228 636f 6e66 5b6e 6d65 742a  d(str(conf[nmet*
+0000b170: 332b 315d 2929 0d0a 0d0a 2020 2020 2020  3+1]))....      
+0000b180: 2020 6864 722e 6170 7065 6e64 2827 4368    hdr.append('Ch
+0000b190: 6953 7175 6172 6520 2729 2020 2020 2020  iSquare ')      
+0000b1a0: 2020 0d0a 2020 2020 2020 2020 7661 6c2e    ..        val.
+0000b1b0: 6170 7065 6e64 2873 7472 2873 7461 7473  append(str(stats
+0000b1c0: 5b30 5d29 290d 0a0d 0a20 2020 2020 2020  [0]))....       
+0000b1d0: 2068 6472 2e61 7070 656e 6428 2757 7443   hdr.append('WtC
+0000b1e0: 6869 5371 7561 7265 2027 2920 2020 2020  hiSquare ')     
+0000b1f0: 2020 200d 0a20 2020 2020 2020 2076 616c     ..        val
+0000b200: 2e61 7070 656e 6428 7374 7228 7374 6174  .append(str(stat
+0000b210: 735b 315d 2929 0d0a 0d0a 2020 2020 2020  s[1]))....      
+0000b220: 2020 6864 722e 6170 7065 6e64 2827 4d61    hdr.append('Ma
+0000b230: 7468 2046 696e 6974 6520 4572 726f 7220  th Finite Error 
+0000b240: 2729 2020 2020 2020 2020 0d0a 2020 2020  ')        ..    
+0000b250: 2020 2020 6d61 7468 6572 7220 3d20 7374      matherr = st
+0000b260: 7228 7374 6174 735b 325d 2021 3d20 3029  r(stats[2] != 0)
+0000b270: 0d0a 2020 2020 2020 2020 7661 6c2e 6170  ..        val.ap
+0000b280: 7065 6e64 2873 7472 286d 6174 6865 7272  pend(str(matherr
+0000b290: 2929 0d0a 0d0a 2020 2020 2020 2020 7265  ))....        re
+0000b2a0: 7475 726e 2076 616c 2c20 6864 720d 0a20  turn val, hdr.. 
+0000b2b0: 2020 200d 0a20 2020 200d 0a20 2020 2064     ..    ..    d
+0000b2c0: 6566 2072 6573 756c 7473 5f61 735f 6373  ef results_as_cs
+0000b2d0: 765f 616c 6c5f 766f 7865 6c73 5f74 7275  v_all_voxels_tru
+0000b2e0: 6e63 6174 6564 2873 656c 662c 2076 6f78  ncated(self, vox
+0000b2f0: 656c 732c 2064 6174 6166 696c 653d 2720  els, datafile=' 
+0000b300: 272c 206d 6561 7375 7265 5f74 696d 6573  ', measure_times
+0000b310: 3d5b 5d29 3a0d 0a20 2020 2020 2020 2022  =[]):..        "
+0000b320: 2222 0d0a 2020 2020 2020 2020 4769 7665  ""..        Give
+0000b330: 6e20 6120 766f 7865 6c2c 206c 696e 6577  n a voxel, linew
+0000b340: 6964 7468 2070 6172 616d 732c 2061 6e64  idth params, and
+0000b350: 2061 2064 6174 6120 736f 7572 6365 2028   a data source (
+0000b360: 6f66 7465 6e20 6120 6669 6c65 6e61 6d65  often a filename
+0000b370: 292c 200d 0a20 2020 2020 2020 2072 6574  ), ..        ret
+0000b380: 7572 6e73 2043 5356 2d66 6f72 6d61 7474  urns CSV-formatt
+0000b390: 6564 2028 636f 6d6d 6120 7365 7061 7261  ed (comma separa
+0000b3a0: 7465 6420 7661 7269 6162 6c65 7329 7374  ted variables)st
+0000b3b0: 7269 6e67 2063 6f6e 7461 696e 696e 6720  ring containing 
+0000b3c0: 626f 7468 0d0a 2020 2020 2020 2020 7468  both..        th
+0000b3d0: 6520 766f 7865 6c20 6669 7474 696e 6720  e voxel fitting 
+0000b3e0: 7265 7375 6c74 7320 616e 6420 6865 6164  results and head
+0000b3f0: 6572 2073 7472 696e 6720 6465 7363 7269  er string descri
+0000b400: 7074 696f 6e73 2066 6f72 2065 6163 6820  ptions for each 
+0000b410: 0d0a 2020 2020 2020 2020 636f 6c75 6d6e  ..        column
+0000b420: 2e0d 0a0d 0a20 2020 2020 2020 2022 2222  .....        """
+0000b430: 0d0a 0d0a 2020 2020 2020 2020 736f 7572  ....        sour
+0000b440: 6365 203d 2064 6174 6166 696c 652e 7265  ce = datafile.re
+0000b450: 706c 6163 6528 222c 222c 225f 2229 2020  place(",","_")  
+0000b460: 2020 2023 2073 6f6d 6520 7573 6572 7320     # some users 
+0000b470: 6861 7665 2063 6f6d 6d61 7320 696e 2066  have commas in f
+0000b480: 696c 656e 616d 6573 200d 0a0d 0a20 2020  ilenames ....   
+0000b490: 2020 2020 206e 6d65 7420 3d20 6c65 6e28       nmet = len(
+0000b4a0: 7365 6c66 2e73 6574 2e70 7269 6f72 5f6c  self.set.prior_l
+0000b4b0: 6973 7429 0d0a 2020 2020 2020 2020 6e61  ist)..        na
+0000b4c0: 6d65 7320 3d20 7365 6c66 2e73 6574 2e70  mes = self.set.p
+0000b4d0: 7269 6f72 5f6c 6973 740d 0a20 2020 2020  rior_list..     
+0000b4e0: 2020 200d 0a20 2020 2020 2020 2068 6472     ..        hdr
+0000b4f0: 203d 205b 5d0d 0a20 2020 2020 2020 2076   = []..        v
+0000b500: 616c 203d 205b 5d0d 0a0d 0a20 2020 2020  al = []....     
+0000b510: 2020 2068 6472 2e61 7070 656e 6428 2744     hdr.append('D
+0000b520: 6174 6166 696c 6527 2920 2020 0d0a 2020  atafile')   ..  
+0000b530: 2020 2020 2020 6864 722e 6170 7065 6e64        hdr.append
+0000b540: 2827 566f 7865 6c27 290d 0a20 2020 2020  ('Voxel')..     
+0000b550: 2020 2068 6472 2e61 7070 656e 6428 2754     hdr.append('T
+0000b560: 696d 6520 5b73 6563 5d27 290d 0a0d 0a20  ime [sec]').... 
+0000b570: 2020 2020 2020 2066 6f72 2069 2c20 6974         for i, it
+0000b580: 656d 2069 6e20 656e 756d 6572 6174 6528  em in enumerate(
+0000b590: 6e61 6d65 7329 3a0d 0a20 2020 2020 2020  names):..       
+0000b5a0: 2020 2020 2068 6472 2e61 7070 656e 6428       hdr.append(
+0000b5b0: 2741 7265 6120 272b 6974 656d 2920 2020  'Area '+item)   
+0000b5c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000b5d0: 2020 2068 6472 2e61 7070 656e 6428 2750     hdr.append('P
+0000b5e0: 504d 2027 2b69 7465 6d29 2020 2020 2020  PM '+item)      
+0000b5f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000b600: 6864 722e 6170 7065 6e64 2827 5462 5b73  hdr.append('Tb[s
+0000b610: 6563 5d27 2b69 7465 6d29 2020 2020 2020  ec]'+item)      
+0000b620: 2020 0d0a 2020 2020 2020 2020 6864 722e    ..        hdr.
+0000b630: 6170 7065 6e64 2827 5068 6173 6530 2027  append('Phase0 '
+0000b640: 2920 2020 2020 2020 200d 0a20 2020 2020  )        ..     
+0000b650: 2020 2068 6472 2e61 7070 656e 6428 2750     hdr.append('P
+0000b660: 6861 7365 3120 2729 2020 2020 2020 2020  hase1 ')        
+0000b670: 0d0a 0d0a 0d0a 2020 2020 2020 2020 666f  ......        fo
+0000b680: 7220 692c 766f 7865 6c20 696e 2065 6e75  r i,voxel in enu
+0000b690: 6d65 7261 7465 2876 6f78 656c 7329 3a0d  merate(voxels):.
+0000b6a0: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+0000b6b0: 6573 2020 203d 2073 656c 662e 6669 745f  es   = self.fit_
+0000b6c0: 7265 7375 6c74 735b 3a2c 766f 7865 6c5b  results[:,voxel[
+0000b6d0: 305d 2c76 6f78 656c 5b31 5d2c 766f 7865  0],voxel[1],voxe
+0000b6e0: 6c5b 325d 5d0d 0a20 2020 2020 2020 2020  l[2]]..         
+0000b6f0: 2020 2069 7469 6d65 203d 206d 6561 7375     itime = measu
+0000b700: 7265 5f74 696d 6573 5b69 5d0d 0a20 2020  re_times[i]..   
+0000b710: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000b720: 2020 2020 2020 2076 616c 2e61 7070 656e         val.appen
+0000b730: 6428 6461 7461 6669 6c65 290d 0a20 2020  d(datafile)..   
+0000b740: 2020 2020 2020 2020 2076 616c 2e61 7070           val.app
+0000b750: 656e 6428 7374 7228 766f 7865 6c5b 305d  end(str(voxel[0]
+0000b760: 292b 2720 272b 7374 7228 766f 7865 6c5b  )+' '+str(voxel[
+0000b770: 315d 292b 2720 272b 7374 7228 766f 7865  1])+' '+str(voxe
+0000b780: 6c5b 325d 2929 0d0a 2020 2020 2020 2020  l[2]))..        
+0000b790: 2020 2020 7661 6c2e 6170 7065 6e64 2869      val.append(i
+0000b7a0: 7469 6d65 290d 0a20 2020 2020 2020 2020  time)..         
+0000b7b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000b7c0: 2066 6f72 2069 2c20 6974 656d 2069 6e20   for i, item in 
+0000b7d0: 656e 756d 6572 6174 6528 6e61 6d65 7329  enumerate(names)
+0000b7e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000b7f0: 2020 2076 616c 2e61 7070 656e 6428 7374     val.append(st
+0000b800: 7228 7265 735b 692b 6e6d 6574 2a30 5d29  r(res[i+nmet*0])
+0000b810: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b820: 2020 2076 616c 2e61 7070 656e 6428 7374     val.append(st
+0000b830: 7228 7265 735b 692b 6e6d 6574 2a31 5d29  r(res[i+nmet*1])
+0000b840: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b850: 2020 2076 616c 2e61 7070 656e 6428 7374     val.append(st
+0000b860: 7228 7265 735b 692b 6e6d 6574 2a32 5d29  r(res[i+nmet*2])
+0000b870: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000b880: 2076 616c 2e61 7070 656e 6428 7374 7228   val.append(str(
+0000b890: 7265 735b 6e6d 6574 2a33 2b30 5d29 290d  res[nmet*3+0])).
+0000b8a0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+0000b8b0: 2e61 7070 656e 6428 7374 7228 7265 735b  .append(str(res[
+0000b8c0: 6e6d 6574 2a33 2b31 5d29 290d 0a20 2020  nmet*3+1]))..   
+0000b8d0: 200d 0a0d 0a20 2020 2020 2020 2072 6574   ....        ret
+0000b8e0: 7572 6e20 7661 6c2c 2068 6472 2020 2020  urn val, hdr    
+0000b8f0: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
+0000b900: 2020 6465 6620 7265 7375 6c74 735f 6173    def results_as
+0000b910: 5f63 7376 5f61 6c6c 5f76 6f78 656c 735f  _csv_all_voxels_
+0000b920: 6172 6561 7328 7365 6c66 2c20 766f 7865  areas(self, voxe
+0000b930: 6c73 2c20 6461 7461 6669 6c65 3d27 2027  ls, datafile=' '
+0000b940: 2c20 6d65 6173 7572 655f 7469 6d65 733d  , measure_times=
+0000b950: 5b5d 293a 0d0a 2020 2020 2020 2020 2222  []):..        ""
+0000b960: 220d 0a20 2020 2020 2020 2047 6976 656e  "..        Given
+0000b970: 2061 2076 6f78 656c 2c20 6c69 6e65 7769   a voxel, linewi
+0000b980: 6474 6820 7061 7261 6d73 2c20 616e 6420  dth params, and 
+0000b990: 6120 6461 7461 2073 6f75 7263 6520 286f  a data source (o
+0000b9a0: 6674 656e 2061 2066 696c 656e 616d 6529  ften a filename)
+0000b9b0: 2c20 0d0a 2020 2020 2020 2020 7265 7475  , ..        retu
+0000b9c0: 726e 7320 4353 562d 666f 726d 6174 7465  rns CSV-formatte
+0000b9d0: 6420 2863 6f6d 6d61 2073 6570 6172 6174  d (comma separat
+0000b9e0: 6564 2076 6172 6961 626c 6573 2973 7472  ed variables)str
+0000b9f0: 696e 6720 636f 6e74 6169 6e69 6e67 2062  ing containing b
+0000ba00: 6f74 680d 0a20 2020 2020 2020 2074 6865  oth..        the
+0000ba10: 2076 6f78 656c 2066 6974 7469 6e67 2072   voxel fitting r
+0000ba20: 6573 756c 7473 2061 6e64 2068 6561 6465  esults and heade
+0000ba30: 7220 7374 7269 6e67 2064 6573 6372 6970  r string descrip
+0000ba40: 7469 6f6e 7320 666f 7220 6561 6368 200d  tions for each .
+0000ba50: 0a20 2020 2020 2020 2063 6f6c 756d 6e2e  .        column.
+0000ba60: 0d0a 0d0a 2020 2020 2020 2020 2222 220d  ....        """.
+0000ba70: 0a0d 0a20 2020 2020 2020 2073 6f75 7263  ...        sourc
+0000ba80: 6520 3d20 6461 7461 6669 6c65 2e72 6570  e = datafile.rep
+0000ba90: 6c61 6365 2822 2c22 2c22 5f22 2920 2020  lace(",","_")   
+0000baa0: 2020 2320 736f 6d65 2075 7365 7273 2068    # some users h
+0000bab0: 6176 6520 636f 6d6d 6173 2069 6e20 6669  ave commas in fi
+0000bac0: 6c65 6e61 6d65 7320 0d0a 0d0a 2020 2020  lenames ....    
+0000bad0: 2020 2020 6e6d 6574 203d 206c 656e 2873      nmet = len(s
+0000bae0: 656c 662e 7365 742e 7072 696f 725f 6c69  elf.set.prior_li
+0000baf0: 7374 290d 0a20 2020 2020 2020 206e 616d  st)..        nam
+0000bb00: 6573 203d 2073 656c 662e 7365 742e 7072  es = self.set.pr
+0000bb10: 696f 725f 6c69 7374 0d0a 2020 2020 2020  ior_list..      
+0000bb20: 2020 0d0a 2020 2020 2020 2020 6c69 6e65    ..        line
+0000bb30: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+0000bb40: 2020 7469 6d65 7320 3d20 5b5d 0d0a 2020    times = []..  
+0000bb50: 2020 2020 2020 7469 6d65 732e 6170 7065        times.appe
+0000bb60: 6e64 2873 6f75 7263 6529 0d0a 2020 2020  nd(source)..    
+0000bb70: 2020 2020 7469 6d65 732e 6170 7065 6e64      times.append
+0000bb80: 2827 5f54 696d 6520 5b6d 696e 5d20 2729  ('_Time [min] ')
+0000bb90: 0d0a 2020 2020 2020 2020 666f 7220 6d65  ..        for me
+0000bba0: 6173 7572 655f 7469 6d65 2069 6e20 6d65  asure_time in me
+0000bbb0: 6173 7572 655f 7469 6d65 733a 0d0a 2020  asure_times:..  
+0000bbc0: 2020 2020 2020 2020 2020 7469 6d65 732e            times.
+0000bbd0: 6170 7065 6e64 2873 7472 2828 6d65 6173  append(str((meas
+0000bbe0: 7572 655f 7469 6d65 202d 206d 6561 7375  ure_time - measu
+0000bbf0: 7265 5f74 696d 6573 5b30 5d29 2f36 302e  re_times[0])/60.
+0000bc00: 3029 2920 2020 2020 2020 2320 696e 206d  0))       # in m
+0000bc10: 696e 7574 6573 0d0a 2020 2020 2020 2020  inutes..        
+0000bc20: 6c69 6e65 732e 6170 7065 6e64 2874 696d  lines.append(tim
+0000bc30: 6573 290d 0a0d 0a20 2020 2020 2020 200d  es)....        .
+0000bc40: 0a20 2020 2020 2020 2066 6f72 206a 2c20  .        for j, 
+0000bc50: 6e61 6d65 2069 6e20 656e 756d 6572 6174  name in enumerat
+0000bc60: 6528 6e61 6d65 7329 3a0d 0a20 2020 2020  e(names):..     
+0000bc70: 2020 2020 2020 2076 616c 203d 205b 5d0d         val = [].
+0000bc80: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+0000bc90: 2e61 7070 656e 6428 736f 7572 6365 290d  .append(source).
+0000bca0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+0000bcb0: 2e61 7070 656e 6428 6e61 6d65 2b27 2041  .append(name+' A
+0000bcc0: 7265 6127 290d 0a20 2020 2020 2020 2020  rea')..         
+0000bcd0: 2020 2066 6f72 2069 2c76 6f78 656c 2069     for i,voxel i
+0000bce0: 6e20 656e 756d 6572 6174 6528 766f 7865  n enumerate(voxe
+0000bcf0: 6c73 293a 0d0a 2020 2020 2020 2020 2020  ls):..          
+0000bd00: 2020 2020 2020 7661 6c2e 6170 7065 6e64        val.append
+0000bd10: 2820 7374 7228 7365 6c66 2e66 6974 5f72  ( str(self.fit_r
+0000bd20: 6573 756c 7473 5b6a 2b6e 6d65 742a 302c  esults[j+nmet*0,
+0000bd30: 766f 7865 6c5b 305d 2c76 6f78 656c 5b31  voxel[0],voxel[1
+0000bd40: 5d2c 766f 7865 6c5b 325d 5d29 2029 0d0a  ],voxel[2]]) )..
+0000bd50: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0000bd60: 732e 6170 7065 6e64 2876 616c 290d 0a0d  s.append(val)...
+0000bd70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000bd80: 6c69 6e65 7320 2020 200d 0a0d 0a0d 0a0d  lines    .......
+0000bd90: 0a20 2020 2064 6566 2072 6573 756c 7473  .    def results
+0000bda0: 5f69 6e5f 7461 626c 6528 7365 6c66 2c20  _in_table(self, 
+0000bdb0: 766f 7865 6c2c 206c 773d 302e 302c 206c  voxel, lw=0.0, l
+0000bdc0: 776d 696e 3d30 2e30 2c20 6c77 6d61 783d  wmin=0.0, lwmax=
+0000bdd0: 302e 302c 206e 6f7a 6572 6f73 3d46 616c  0.0, nozeros=Fal
+0000bde0: 7365 2c20 6e6f 7070 6d3d 4661 6c73 652c  se, noppm=False,
+0000bdf0: 2066 6978 7068 6173 653d 4661 6c73 6529   fixphase=False)
+0000be00: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+0000be10: 2020 2020 2020 2020 4769 7665 6e20 6120          Given a 
+0000be20: 766f 7865 6c2c 206c 696e 6577 6964 7468  voxel, linewidth
+0000be30: 2070 6172 616d 732c 2061 6e64 2061 2064   params, and a d
+0000be40: 6174 6120 736f 7572 6365 2028 6f66 7465  ata source (ofte
+0000be50: 6e20 6120 6669 6c65 6e61 6d65 292c 200d  n a filename), .
+0000be60: 0a20 2020 2020 2020 2072 6574 7572 6e73  .        returns
+0000be70: 2066 6f72 6d61 7474 6564 2072 6573 756c   formatted resul
+0000be80: 7473 2066 6f72 2074 6861 7420 766f 7865  ts for that voxe
+0000be90: 6c2e 200d 0a20 2020 2020 2020 200d 0a20  l. ..        .. 
+0000bea0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0000beb0: 2020 2020 2320 4669 7273 7420 7765 2061      # First we a
+0000bec0: 7373 656d 626c 6520 7468 6520 6461 7461  ssemble the data
+0000bed0: 2077 6520 6e65 6564 2e0d 0a20 2020 2020   we need...     
+0000bee0: 2020 206e 6d65 7420 203d 206c 656e 2873     nmet  = len(s
+0000bef0: 656c 662e 7365 742e 7072 696f 725f 6c69  elf.set.prior_li
+0000bf00: 7374 290d 0a20 2020 2020 2020 200d 0a20  st)..        .. 
+0000bf10: 2020 2020 2020 206e 616d 6573 203d 2073         names = s
+0000bf20: 656c 662e 7365 742e 7072 696f 725f 6c69  elf.set.prior_li
+0000bf30: 7374 0d0a 2020 2020 2020 2020 7265 7320  st..        res 
+0000bf40: 2020 3d20 7365 6c66 2e66 6974 5f72 6573    = self.fit_res
+0000bf50: 756c 7473 5b3a 2c76 6f78 656c 5b30 5d2c  ults[:,voxel[0],
+0000bf60: 766f 7865 6c5b 315d 2c76 6f78 656c 5b32  voxel[1],voxel[2
+0000bf70: 5d5d 0d0a 2020 2020 2020 2020 6372 616f  ]]..        crao
+0000bf80: 2020 3d20 7365 6c66 2e63 7261 6d65 725f    = self.cramer_
+0000bf90: 7261 6f5b 3a2c 766f 7865 6c5b 305d 2c76  rao[:,voxel[0],v
+0000bfa0: 6f78 656c 5b31 5d2c 766f 7865 6c5b 325d  oxel[1],voxel[2]
+0000bfb0: 5d0d 0a20 2020 2020 2020 2063 6f6e 6620  ]..        conf 
+0000bfc0: 203d 2073 656c 662e 636f 6e66 6964 656e   = self.confiden
+0000bfd0: 6365 5b3a 2c76 6f78 656c 5b30 5d2c 766f  ce[:,voxel[0],vo
+0000bfe0: 7865 6c5b 315d 2c76 6f78 656c 5b32 5d5d  xel[1],voxel[2]]
+0000bff0: 0d0a 2020 2020 2020 2020 7374 6174 7320  ..        stats 
+0000c000: 3d20 7365 6c66 2e66 6974 5f73 7461 7473  = self.fit_stats
+0000c010: 5b3a 2c76 6f78 656c 5b30 5d2c 766f 7865  [:,voxel[0],voxe
+0000c020: 6c5b 315d 2c76 6f78 656c 5b32 5d5d 0d0a  l[1],voxel[2]]..
+0000c030: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c040: 2020 646f 5f63 7261 6f20 3d20 4661 6c73    do_crao = Fals
+0000c050: 6520 6966 206d 6178 2863 7261 6f29 203d  e if max(crao) =
+0000c060: 3d20 302e 3020 616e 6420 6e6f 7a65 726f  = 0.0 and nozero
+0000c070: 7320 656c 7365 2054 7275 650d 0a20 2020  s else True..   
+0000c080: 2020 2020 2064 6f5f 636f 6e66 203d 2046       do_conf = F
+0000c090: 616c 7365 2069 6620 6d61 7828 636f 6e66  alse if max(conf
+0000c0a0: 2920 3d3d 2030 2e30 2061 6e64 206e 6f7a  ) == 0.0 and noz
+0000c0b0: 6572 6f73 2065 6c73 6520 5472 7565 0d0a  eros else True..
+0000c0c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c0d0: 2020 2320 626f 7468 2063 7261 6d65 722d    # both cramer-
+0000c0e0: 7261 6f20 616e 6420 636f 6e66 6964 656e  rao and confiden
+0000c0f0: 6365 2069 6e74 6572 7661 6c73 206d 6179  ce intervals may
+0000c100: 2062 6520 6f66 662f 6f6e 0d0a 2020 2020   be off/on..    
+0000c110: 2020 2020 6966 206c 656e 2863 7261 6f29      if len(crao)
+0000c120: 2021 3d20 6c65 6e28 7265 7329 3a0d 0a20   != len(res):.. 
+0000c130: 2020 2020 2020 2020 2020 2063 7261 6f20             crao 
+0000c140: 3d20 7265 7320 2a20 300d 0a20 2020 2020  = res * 0..     
+0000c150: 2020 2069 6620 6c65 6e28 636f 6e66 2920     if len(conf) 
+0000c160: 213d 206c 656e 2872 6573 293a 0d0a 2020  != len(res):..  
+0000c170: 2020 2020 2020 2020 2020 636f 6e66 203d            conf =
+0000c180: 2072 6573 202a 2030 0d0a 0d0a 2020 2020   res * 0....    
+0000c190: 2020 2020 6864 7231 2020 3d20 5b27 4d65      hdr1  = ['Me
+0000c1a0: 7461 6220 5265 7375 6c74 7327 2c20 2741  tab Results', 'A
+0000c1b0: 7265 6127 5d0d 0a20 2020 2020 2020 2068  rea']..        h
+0000c1c0: 6472 3220 203d 205b 2750 504d 2052 6573  dr2  = ['PPM Res
+0000c1d0: 756c 7473 272c 2027 5050 4d27 5d0d 0a20  ults', 'PPM'].. 
+0000c1e0: 2020 2020 2020 2068 6472 3261 203d 205b         hdr2a = [
+0000c1f0: 2754 6220 5265 7375 6c74 7327 2c20 2754  'Tb Results', 'T
+0000c200: 6220 5b73 6563 5d27 2c20 274c 5720 5b48  b [sec]', 'LW [H
+0000c210: 7a5d 275d 0d0a 2020 2020 2020 2020 6864  z]']..        hd
+0000c220: 7233 2020 3d20 5b27 476c 6f62 616c 2052  r3  = ['Global R
+0000c230: 6573 756c 7473 272c 2027 5661 6c75 6527  esults', 'Value'
+0000c240: 5d0d 0a20 2020 2020 2020 2068 6472 3420  ]..        hdr4 
+0000c250: 203d 205b 2743 616c 6320 5265 7375 6c74   = ['Calc Result
+0000c260: 7327 2c20 2720 5661 6c75 6527 5d0d 0a20  s', ' Value'].. 
+0000c270: 2020 2020 2020 2069 6620 646f 5f63 7261         if do_cra
+0000c280: 6f3a 200d 0a20 2020 2020 2020 2020 2020  o: ..           
+0000c290: 2068 6472 312e 6170 7065 6e64 2827 4372   hdr1.append('Cr
+0000c2a0: 5261 6f5b 255d 2729 0d0a 2020 2020 2020  Rao[%]')..      
+0000c2b0: 2020 2020 2020 6864 7232 2e61 7070 656e        hdr2.appen
+0000c2c0: 6428 2743 7252 616f 5b64 656c 7461 5d27  d('CrRao[delta]'
+0000c2d0: 290d 0a20 2020 2020 2020 2020 2020 2068  )..            h
+0000c2e0: 6472 3261 2e61 7070 656e 6428 2743 7252  dr2a.append('CrR
+0000c2f0: 616f 5b64 656c 7461 5d27 290d 0a20 2020  ao[delta]')..   
+0000c300: 2020 2020 2020 2020 2068 6472 332e 6170           hdr3.ap
+0000c310: 7065 6e64 2827 4372 5261 6f5b 6465 6c74  pend('CrRao[delt
+0000c320: 615d 2729 0d0a 2020 2020 2020 2020 2020  a]')..          
+0000c330: 2020 6864 7234 2e61 7070 656e 6428 2720    hdr4.append(' 
+0000c340: 2729 0d0a 2020 2020 2020 2020 6966 2064  ')..        if d
+0000c350: 6f5f 636f 6e66 3a20 0d0a 2020 2020 2020  o_conf: ..      
+0000c360: 2020 2020 2020 6864 7231 2e61 7070 656e        hdr1.appen
+0000c370: 6428 2743 6e66 496e 745b 255d 2729 0d0a  d('CnfInt[%]')..
+0000c380: 2020 2020 2020 2020 2020 2020 6864 7232              hdr2
+0000c390: 2e61 7070 656e 6428 2743 6e66 496e 745b  .append('CnfInt[
+0000c3a0: 6465 6c74 615d 2729 0d0a 2020 2020 2020  delta]')..      
+0000c3b0: 2020 2020 2020 6864 7232 612e 6170 7065        hdr2a.appe
+0000c3c0: 6e64 2827 436e 6649 6e74 5b64 656c 7461  nd('CnfInt[delta
+0000c3d0: 5d27 290d 0a20 2020 2020 2020 2020 2020  ]')..           
+0000c3e0: 2068 6472 332e 6170 7065 6e64 2827 436e   hdr3.append('Cn
+0000c3f0: 6649 6e74 5b64 656c 7461 5d27 290d 0a20  fInt[delta]').. 
+0000c400: 2020 2020 2020 2020 2020 2068 6472 342e             hdr4.
+0000c410: 6170 7065 6e64 2827 2027 290d 0a0d 0a20  append(' ').... 
+0000c420: 2020 2020 2020 206e 7365 6374 203d 205b         nsect = [
+0000c430: 302c 5d0d 0a20 2020 2020 2020 2074 6162  0,]..        tab
+0000c440: 6c65 3120 3d20 5b68 6472 312c 5d0d 0a20  le1 = [hdr1,].. 
+0000c450: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000c460: 2066 6f72 2069 2c20 6974 656d 2069 6e20   for i, item in 
+0000c470: 656e 756d 6572 6174 6528 6e61 6d65 7329  enumerate(names)
+0000c480: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+0000c490: 6d70 203d 205b 6974 656d 2c20 7265 735b  mp = [item, res[
+0000c4a0: 695d 5d0d 0a20 2020 2020 2020 2020 2020  i]]..           
+0000c4b0: 2069 6620 646f 5f63 7261 6f3a 2074 6d70   if do_crao: tmp
+0000c4c0: 2e61 7070 656e 6428 6372 616f 5b69 5d29  .append(crao[i])
+0000c4d0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000c4e0: 2064 6f5f 636f 6e66 3a20 746d 702e 6170   do_conf: tmp.ap
+0000c4f0: 7065 6e64 2863 6f6e 665b 695d 290d 0a20  pend(conf[i]).. 
+0000c500: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+0000c510: 312e 6170 7065 6e64 2874 6d70 290d 0a0d  1.append(tmp)...
+0000c520: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000c530: 2e73 6574 2e6d 6163 726f 6d6f 6c5f 6d6f  .set.macromol_mo
+0000c540: 6465 6c20 3d3d 2046 6974 4d61 6372 6f6d  del == FitMacrom
+0000c550: 6f6c 6563 756c 654d 6574 686f 642e 5349  oleculeMethod.SI
+0000c560: 4e47 4c45 5f42 4153 4953 5f44 4154 4153  NGLE_BASIS_DATAS
+0000c570: 4554 3a0d 0a20 2020 2020 2020 2020 2020  ET:..           
+0000c580: 2074 6d70 203d 205b 274d 4d6f 6c27 2c20   tmp = ['MMol', 
+0000c590: 7265 735b 6e6d 6574 2a33 2b32 5d5d 0d0a  res[nmet*3+2]]..
+0000c5a0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0000c5b0: 6f5f 6372 616f 3a20 746d 702e 6170 7065  o_crao: tmp.appe
+0000c5c0: 6e64 2830 2e30 290d 0a20 2020 2020 2020  nd(0.0)..       
+0000c5d0: 2020 2020 2069 6620 646f 5f63 6f6e 663a       if do_conf:
+0000c5e0: 2074 6d70 2e61 7070 656e 6428 302e 3029   tmp.append(0.0)
+0000c5f0: 0d0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+0000c600: 626c 6531 2e61 7070 656e 6428 746d 7029  ble1.append(tmp)
+0000c610: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000c620: 2020 2020 2020 2020 6e73 6563 742e 6170          nsect.ap
+0000c630: 7065 6e64 286c 656e 2874 6162 6c65 3129  pend(len(table1)
+0000c640: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+0000c650: 6e6f 7420 6e6f 7070 6d3a 0d0a 2020 2020  not noppm:..    
+0000c660: 2020 2020 2020 2020 7461 626c 6531 2e61          table1.a
+0000c670: 7070 656e 6428 6864 7232 290d 0a20 2020  ppend(hdr2)..   
+0000c680: 2020 2020 2020 2020 2066 6f72 2069 2c69           for i,i
+0000c690: 7465 6d20 696e 2065 6e75 6d65 7261 7465  tem in enumerate
+0000c6a0: 286e 616d 6573 293a 0d0a 2020 2020 2020  (names):..      
+0000c6b0: 2020 2020 2020 2020 2020 746d 7020 3d20            tmp = 
+0000c6c0: 5b69 7465 6d2c 2072 6573 5b69 2b6e 6d65  [item, res[i+nme
+0000c6d0: 745d 5d0d 0a20 2020 2020 2020 2020 2020  t]]..           
+0000c6e0: 2020 2020 2069 6620 646f 5f63 7261 6f3a       if do_crao:
+0000c6f0: 2074 6d70 2e61 7070 656e 6428 6372 616f   tmp.append(crao
+0000c700: 5b69 2b6e 6d65 745d 290d 0a20 2020 2020  [i+nmet])..     
+0000c710: 2020 2020 2020 2020 2020 2069 6620 646f             if do
+0000c720: 5f63 6f6e 663a 2074 6d70 2e61 7070 656e  _conf: tmp.appen
+0000c730: 6428 636f 6e66 5b69 2b6e 6d65 745d 290d  d(conf[i+nmet]).
+0000c740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c750: 2074 6162 6c65 312e 6170 7065 6e64 2874   table1.append(t
+0000c760: 6d70 290d 0a20 2020 2020 0d0a 2020 2020  mp)..     ..    
+0000c770: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000c780: 7365 742e 6d61 6372 6f6d 6f6c 5f6d 6f64  set.macromol_mod
+0000c790: 656c 203d 3d20 4669 744d 6163 726f 6d6f  el == FitMacromo
+0000c7a0: 6c65 6375 6c65 4d65 7468 6f64 2e53 494e  leculeMethod.SIN
+0000c7b0: 474c 455f 4241 5349 535f 4441 5441 5345  GLE_BASIS_DATASE
+0000c7c0: 543a 0d0a 2020 2020 2020 2020 2020 2020  T:..            
+0000c7d0: 2020 2020 746d 7020 3d20 5b27 4d4d 6f6c      tmp = ['MMol
+0000c7e0: 272c 2072 6573 5b6e 6d65 742a 332b 335d  ', res[nmet*3+3]
+0000c7f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000c800: 2020 2069 6620 646f 5f63 7261 6f3a 2074     if do_crao: t
+0000c810: 6d70 2e61 7070 656e 6428 302e 3029 0d0a  mp.append(0.0)..
+0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c830: 6966 2064 6f5f 636f 6e66 3a20 746d 702e  if do_conf: tmp.
+0000c840: 6170 7065 6e64 2830 2e30 290d 0a20 2020  append(0.0)..   
+0000c850: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+0000c860: 6c65 312e 6170 7065 6e64 2874 6d70 290d  le1.append(tmp).
+0000c870: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+0000c880: 6162 6c65 312e 6170 7065 6e64 2868 6472  able1.append(hdr
+0000c890: 3261 290d 0a20 2020 2020 2020 2020 2020  2a)..           
+0000c8a0: 2066 6f72 2069 2c69 7465 6d20 696e 2065   for i,item in e
+0000c8b0: 6e75 6d65 7261 7465 286e 616d 6573 293a  numerate(names):
+0000c8c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c8d0: 2020 746d 7020 3d20 5b69 7465 6d2c 2072    tmp = [item, r
+0000c8e0: 6573 5b69 2b6e 6d65 742a 325d 2c20 6c77  es[i+nmet*2], lw
+0000c8f0: 5b69 5d5d 0d0a 2020 2020 2020 2020 2020  [i]]..          
+0000c900: 2020 2020 2020 6966 2064 6f5f 6372 616f        if do_crao
+0000c910: 3a20 746d 702e 6170 7065 6e64 2863 7261  : tmp.append(cra
+0000c920: 6f5b 692b 6e6d 6574 2a32 5d29 0d0a 2020  o[i+nmet*2])..  
+0000c930: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c940: 2064 6f5f 636f 6e66 3a20 746d 702e 6170   do_conf: tmp.ap
+0000c950: 7065 6e64 2863 6f6e 665b 692b 6e6d 6574  pend(conf[i+nmet
+0000c960: 2a32 5d29 0d0a 2020 2020 2020 2020 2020  *2])..          
+0000c970: 2020 2020 2020 7461 626c 6531 2e61 7070        table1.app
+0000c980: 656e 6428 746d 7029 0d0a 2020 2020 200d  end(tmp)..     .
+0000c990: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c9a0: 7365 6c66 2e73 6574 2e6d 6163 726f 6d6f  self.set.macromo
+0000c9b0: 6c5f 6d6f 6465 6c20 3d3d 2046 6974 4d61  l_model == FitMa
+0000c9c0: 6372 6f6d 6f6c 6563 756c 654d 6574 686f  cromoleculeMetho
+0000c9d0: 642e 5349 4e47 4c45 5f42 4153 4953 5f44  d.SINGLE_BASIS_D
+0000c9e0: 4154 4153 4554 3a0d 0a20 2020 2020 2020  ATASET:..       
+0000c9f0: 2020 2020 2020 2020 2074 6d70 203d 205b           tmp = [
+0000ca00: 274d 4d6f 6c27 2c20 7265 735b 6e6d 6574  'MMol', res[nmet
+0000ca10: 2a33 2b34 5d5d 0d0a 2020 2020 2020 2020  *3+4]]..        
+0000ca20: 2020 2020 2020 2020 6966 2064 6f5f 6372          if do_cr
+0000ca30: 616f 3a20 746d 702e 6170 7065 6e64 2830  ao: tmp.append(0
+0000ca40: 2e30 290d 0a20 2020 2020 2020 2020 2020  .0)..           
+0000ca50: 2020 2020 2069 6620 646f 5f63 6f6e 663a       if do_conf:
+0000ca60: 2074 6d70 2e61 7070 656e 6428 302e 3029   tmp.append(0.0)
+0000ca70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ca80: 2020 7461 626c 6531 2e61 7070 656e 6428    table1.append(
+0000ca90: 746d 7029 0d0a 0d0a 2020 2020 2020 2020  tmp)....        
+0000caa0: 6e73 6563 742e 6170 7065 6e64 286c 656e  nsect.append(len
+0000cab0: 2874 6162 6c65 3129 290d 0a20 2020 2020  (table1))..     
+0000cac0: 2020 2074 6162 6c65 312e 6170 7065 6e64     table1.append
+0000cad0: 2868 6472 3329 0d0a 2020 2020 2020 2020  (hdr3)..        
+0000cae0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+0000caf0: 2066 6978 7068 6173 653a 0d0a 2020 2020   fixphase:..    
+0000cb00: 2020 2020 2020 2020 746d 7020 3d20 5b27          tmp = ['
+0000cb10: 5068 6173 6530 272c 2072 6573 5b6e 6d65  Phase0', res[nme
+0000cb20: 742a 332b 305d 5d0d 0a20 2020 2020 2020  t*3+0]]..       
+0000cb30: 2020 2020 2069 6620 646f 5f63 7261 6f3a       if do_crao:
+0000cb40: 2074 6d70 2e61 7070 656e 6428 6372 616f   tmp.append(crao
+0000cb50: 5b6e 6d65 742a 332b 305d 290d 0a20 2020  [nmet*3+0])..   
+0000cb60: 2020 2020 2020 2020 2069 6620 646f 5f63           if do_c
+0000cb70: 6f6e 663a 2074 6d70 2e61 7070 656e 6428  onf: tmp.append(
+0000cb80: 636f 6e66 5b6e 6d65 742a 332b 305d 290d  conf[nmet*3+0]).
+0000cb90: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+0000cba0: 6c65 312e 6170 7065 6e64 2874 6d70 290d  le1.append(tmp).
+0000cbb0: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
+0000cbc0: 2020 2074 6d70 203d 205b 2750 6861 7365     tmp = ['Phase
+0000cbd0: 3127 2c20 7265 735b 6e6d 6574 2a33 2b31  1', res[nmet*3+1
+0000cbe0: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
+0000cbf0: 6966 2064 6f5f 6372 616f 3a20 746d 702e  if do_crao: tmp.
+0000cc00: 6170 7065 6e64 2863 7261 6f5b 6e6d 6574  append(crao[nmet
+0000cc10: 2a33 2b31 5d29 0d0a 2020 2020 2020 2020  *3+1])..        
+0000cc20: 2020 2020 6966 2064 6f5f 636f 6e66 3a20      if do_conf: 
+0000cc30: 746d 702e 6170 7065 6e64 2863 6f6e 665b  tmp.append(conf[
+0000cc40: 6e6d 6574 2a33 2b31 5d29 0d0a 2020 2020  nmet*3+1])..    
+0000cc50: 2020 2020 2020 2020 7461 626c 6531 2e61          table1.a
+0000cc60: 7070 656e 6428 746d 7029 0d0a 2020 2020  ppend(tmp)..    
+0000cc70: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000cc80: 2020 2020 2020 2074 6d70 203d 205b 2750         tmp = ['P
+0000cc90: 6861 7365 3027 2c20 2730 2e30 2028 272b  hase0', '0.0 ('+
+0000cca0: 7374 7228 6e70 2e72 6f75 6e64 2872 6573  str(np.round(res
+0000ccb0: 5b6e 6d65 742a 332b 305d 2c31 2929 2b27  [nmet*3+0],1))+'
+0000ccc0: 2927 5d0d 0a20 2020 2020 2020 2020 2020  )']..           
+0000ccd0: 2069 6620 646f 5f63 7261 6f3a 2074 6d70   if do_crao: tmp
+0000cce0: 2e61 7070 656e 6428 6372 616f 5b6e 6d65  .append(crao[nme
+0000ccf0: 742a 332b 305d 290d 0a20 2020 2020 2020  t*3+0])..       
+0000cd00: 2020 2020 2069 6620 646f 5f63 6f6e 663a       if do_conf:
+0000cd10: 2074 6d70 2e61 7070 656e 6428 636f 6e66   tmp.append(conf
+0000cd20: 5b6e 6d65 742a 332b 305d 290d 0a20 2020  [nmet*3+0])..   
+0000cd30: 2020 2020 2020 2020 2074 6162 6c65 312e           table1.
+0000cd40: 6170 7065 6e64 2874 6d70 290d 0a20 2020  append(tmp)..   
+0000cd50: 200d 0a20 2020 2020 2020 2020 2020 2074   ..            t
+0000cd60: 6d70 203d 205b 2750 6861 7365 3127 2c20  mp = ['Phase1', 
+0000cd70: 2730 2e30 2028 272b 7374 7228 6e70 2e72  '0.0 ('+str(np.r
+0000cd80: 6f75 6e64 2872 6573 5b6e 6d65 742a 332b  ound(res[nmet*3+
+0000cd90: 315d 2c31 2929 2b27 2927 5d0d 0a20 2020  1],1))+')']..   
+0000cda0: 2020 2020 2020 2020 2069 6620 646f 5f63           if do_c
+0000cdb0: 7261 6f3a 2074 6d70 2e61 7070 656e 6428  rao: tmp.append(
+0000cdc0: 6372 616f 5b6e 6d65 742a 332b 315d 290d  crao[nmet*3+1]).
+0000cdd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000cde0: 646f 5f63 6f6e 663a 2074 6d70 2e61 7070  do_conf: tmp.app
+0000cdf0: 656e 6428 636f 6e66 5b6e 6d65 742a 332b  end(conf[nmet*3+
+0000ce00: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
+0000ce10: 2074 6162 6c65 312e 6170 7065 6e64 2874   table1.append(t
+0000ce20: 6d70 290d 0a20 2020 2020 2020 2020 2020  mp)..           
+0000ce30: 200d 0a20 2020 2020 2020 206e 7365 6374   ..        nsect
+0000ce40: 2e61 7070 656e 6428 6c65 6e28 7461 626c  .append(len(tabl
+0000ce50: 6531 2929 0d0a 2020 2020 2020 2020 7461  e1))..        ta
+0000ce60: 626c 6531 2e61 7070 656e 6428 6864 7234  ble1.append(hdr4
+0000ce70: 290d 0a0d 0a20 2020 2020 2020 2074 6d70  )....        tmp
+0000ce80: 203d 205b 2743 6869 5371 7561 7265 272c   = ['ChiSquare',
+0000ce90: 2073 7461 7473 5b30 5d5d 0d0a 2020 2020   stats[0]]..    
+0000cea0: 2020 2020 6966 2064 6f5f 6372 616f 3a20      if do_crao: 
+0000ceb0: 746d 702e 6170 7065 6e64 2827 2027 290d  tmp.append(' ').
+0000cec0: 0a20 2020 2020 2020 2069 6620 646f 5f63  .        if do_c
+0000ced0: 6f6e 663a 2074 6d70 2e61 7070 656e 6428  onf: tmp.append(
+0000cee0: 2720 2729 0d0a 2020 2020 2020 2020 7461  ' ')..        ta
+0000cef0: 626c 6531 2e61 7070 656e 6428 746d 7029  ble1.append(tmp)
+0000cf00: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000cf10: 2020 2020 746d 7020 3d20 5b27 5765 6967      tmp = ['Weig
+0000cf20: 6874 6564 2043 6869 5371 7561 7265 272c  hted ChiSquare',
+0000cf30: 2073 7461 7473 5b31 5d5d 0d0a 2020 2020   stats[1]]..    
+0000cf40: 2020 2020 6966 2064 6f5f 6372 616f 3a20      if do_crao: 
+0000cf50: 746d 702e 6170 7065 6e64 2827 2027 290d  tmp.append(' ').
+0000cf60: 0a20 2020 2020 2020 2069 6620 646f 5f63  .        if do_c
+0000cf70: 6f6e 663a 2074 6d70 2e61 7070 656e 6428  onf: tmp.append(
+0000cf80: 2720 2729 0d0a 2020 2020 2020 2020 7461  ' ')..        ta
+0000cf90: 626c 6531 2e61 7070 656e 6428 746d 7029  ble1.append(tmp)
+0000cfa0: 0d0a 0d0a 2020 2020 2020 2020 6d61 7468  ....        math
+0000cfb0: 6572 7220 3d20 7374 7228 7374 6174 735b  err = str(stats[
+0000cfc0: 325d 2021 3d20 3029 0d0a 2020 2020 2020  2] != 0)..      
+0000cfd0: 2020 746d 7020 3d20 5b27 4d61 7468 2046    tmp = ['Math F
+0000cfe0: 696e 6974 6520 4572 726f 7227 2c20 6d61  inite Error', ma
+0000cff0: 7468 6572 725d 0d0a 2020 2020 2020 2020  therr]..        
+0000d000: 6966 2064 6f5f 6372 616f 3a20 746d 702e  if do_crao: tmp.
+0000d010: 6170 7065 6e64 2827 2027 290d 0a20 2020  append(' ')..   
+0000d020: 2020 2020 2069 6620 646f 5f63 6f6e 663a       if do_conf:
+0000d030: 2074 6d70 2e61 7070 656e 6428 2720 2729   tmp.append(' ')
+0000d040: 0d0a 2020 2020 2020 2020 7461 626c 6531  ..        table1
+0000d050: 2e61 7070 656e 6428 746d 7029 0d0a 2020  .append(tmp)..  
+0000d060: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000d070: 7461 626c 6531 203d 205f 7072 6574 7479  table1 = _pretty
+0000d080: 5f73 7061 6365 5f74 6162 6c65 5f69 6e70  _space_table_inp
+0000d090: 6c61 6365 2874 6162 6c65 312c 2070 6c61  lace(table1, pla
+0000d0a0: 6365 733d 3529 0d0a 0d0a 2020 2020 2020  ces=5)....      
+0000d0b0: 2020 7265 7475 726e 2074 6162 6c65 312c    return table1,
+0000d0c0: 206e 7365 6374 0d0a 2020 2020 0d0a 200d   nsect..    .. .
+0000d0d0: 0a                                       .
```

## vespa/analysis/block_raw_edit_fidsum.py

```diff
@@ -27,90 +27,130 @@
     references to all of them. We have also added methods for get_/set_
     associated datasets based on the multiple file relationships
 
     """
     XML_VERSION = "1.0.0"
     
     def __init__(self, attributes=None):
-        super().__init__(attributes)
 
         self.data_on  = None
         self.data_off = None
+        self.data_sum_indiv = None
+        self.data_dif_indiv = None
         self.data_sum = None
         self.data_dif = None
         self.data_on_id  = ''
         self.data_off_id = ''
+        self.data_sum_indiv_id = ''
+        self.data_dif_indiv_id = ''
         self.data_sum_id = ''
         self.data_dif_id = ''
 
+        # called last because inflate called inside here and values above would reset
+
+        super().__init__(attributes)
+
 
     ##### Standard Methods and Properties #####################################
 
     def __str__(self):
         lines = mrs_data_raw.DataRaw.__str__(self).split('\n')
         # Replace the heading line
         lines[0] = "------- {0} Object -------".format(self.__class__.__name__)
         lines.append("No printable data ")
         return '\n'.join(lines)
 
 
     def clear_associated_datasets(self):
         self.data_on  = None
         self.data_off = None
+        self.data_sum_indiv = None      # for derived dataset completeness
+        self.data_dif_indiv = None      # for derived dataset completeness
         self.data_sum = None
         self.data_dif = None
         self.data_on_id  = ''
         self.data_off_id = ''
+        self.data_sum_indiv_id = ''      # for derived dataset completeness
+        self.data_dif_indiv_id = ''      # for derived dataset completeness
         self.data_sum_id = ''
         self.data_dif_id = ''
 
 
     def get_associated_datasets(self, is_main_dataset=True):
         """
         Return list of datasets associated with this object
         - is_main_dataset: flag for top dataset, used to stop circular references
 
+        Order matters here
+        - ON, OFF, then SUM_INDIV, DIF_INDIV, then SUM, DIF
+        - because of Fidsum object
+        - Note. this is different in block_raw_edit (non-Fidsum) object
+
         """
-        # order matters here - on, off, sum, then diff
-        return [] if not is_main_dataset else [self.data_on, self.data_off, self.data_sum, self.data_dif]
+        r = []
+        if is_main_dataset:
+            # None values dealt with in notebook_datasets.global_poll_associated_tabs
+            r = [self.data_on, self.data_off, self.data_sum_indiv, self.data_dif_indiv, self.data_sum, self.data_dif]
+
+        return r
 
 
     def set_associated_datasets(self, datasets): 
         """
         When we open a VIFF format file, main._import_file() calls this method
         to parse/store any datasets associated with this one as described below.
-        
+
+        Order matters here, datasets expected to be in following order:
+        - ON, OFF, then SUM_INDIV, DIF_INDIV, then SUM, DIF
+        - because of Fidsum object
+        - Note. this is different in block_raw_edit (non-Fidsum) object
+
         """
+        ndatasets = len(datasets)
+
+        # pass1 - use defined IDs to set
+        for dataset in datasets:
+            if self.data_on_id == dataset.id:
+                self.data_on = dataset
+            if self.data_off_id == dataset.id:
+                self.data_off = dataset
+            if self.data_sum_indiv_id == dataset.id:
+                self.data_sum_indiv = dataset
+            if self.data_dif_indiv_id == dataset.id:
+                self.data_dif_indiv = dataset
+            if self.data_sum_id == dataset.id:
+                self.data_sum = dataset
+            if self.data_dif_id == dataset.id:
+                self.data_dif = dataset
+
+        # pass2 - define by position if necessary
         if self.data_on_id == '':
             self.data_on = datasets[0]
-        else:
-            for dataset in datasets:
-                if self.data_on_id == dataset.id:
-                    self.data_on = dataset
+            self.data_on_id = datasets[0].id
 
         if self.data_off_id == '':
             self.data_off = datasets[1]
-        else:
-            for dataset in datasets:
-                if self.data_off_id == dataset.id:
-                    self.data_off = dataset
-
-        if self.data_sum_id == '':
-            self.data_sum = datasets[2]
-        else:
-            for dataset in datasets:
-                if self.data_sum_id == dataset.id:
-                    self.data_sum = dataset
-
-        if self.data_dif_id == '':
-            self.data_dif = datasets[3]
-        else:
-            for dataset in datasets:
-                if self.data_dif_id == dataset.id:
-                    self.data_dif = dataset
+            self.data_off_id = datasets[1].id
+
+        if self.data_sum_indiv_id == '' and ndatasets > 2:
+            self.data_sum_indiv = datasets[2]
+            self.data_sum_indiv_id = datasets[2].id
+
+        if self.data_dif_indiv_id == '' and ndatasets > 3:
+            self.data_dif_indiv = datasets[3]
+            self.data_dif_indiv_id = datasets[3].id
+
+        if self.data_sum_id == '' and ndatasets > 4:
+            self.data_sum = datasets[4]
+            self.data_sum_id = datasets[4].id
+
+        if self.data_dif_id == '' and ndatasets > 5:
+            self.data_dif = datasets[5]
+            self.data_dif_id = datasets[5].id
+
                     
 
     def deflate(self, flavor=Deflate.ETREE):
         
         # Make my base class do its deflate work
         e = block_raw.BlockRaw.deflate(self, flavor)
 
@@ -134,14 +174,18 @@
                     util_xml.TextSubElement(e, "data_on_id",  self.data_on.id)
                 if self.data_off:
                     util_xml.TextSubElement(e, "data_off_id", self.data_off.id)
                 if self.data_sum:
                     util_xml.TextSubElement(e, "data_sum_id", self.data_sum.id)
                 if self.data_dif:
                     util_xml.TextSubElement(e, "data_dif_id", self.data_dif.id)
+                if self.data_sum_indiv:
+                    util_xml.TextSubElement(e, "data_sum_indiv_id", self.data_sum_indiv.id)
+                if self.data_dif_indiv:
+                    util_xml.TextSubElement(e, "data_dif_indiv_id", self.data_dif_indiv.id)
 
             return e
 
         elif flavor == Deflate.DICTIONARY:
             return e
 
 
@@ -156,15 +200,17 @@
             # Quacks like an ElementTree.Element
             if not self.behave_as_preset:
             
                 self.data_on_id  = source.findtext("data_on_id")
                 self.data_off_id = source.findtext("data_off_id")
                 self.data_sum_id = source.findtext("data_sum_id")
                 self.data_dif_id = source.findtext("data_dif_id")
-            
+                self.data_sum_indiv_id = source.findtext("data_sum_indiv_id")
+                self.data_dif_indiv_id = source.findtext("data_dif_indiv_id")
+
             # Look for settings under the old name as well as the standard name.
             self.set = util_xml.find_settings(source, "block_raw_edit_fidsum_settings")
             self.set = block_raw._Settings(self.set)
 
         elif hasattr(source, "keys"):
             # Quacks like a dict
             for key in list(source.keys()):
@@ -173,14 +219,19 @@
                         self.data_on_id = source["data_on_id"]
                     if key == "data_off_id":
                         self.data_off_id = source["data_off_id"]
                     if key == "data_sum_id":
                         self.data_sum_id = source["data_sum_id"]
                     if key == "data_dif_id":
                         self.data_dif_id = source["data_dif_id"]
+                    if key == "data_sum_indiv_id":
+                        self.data_sum_indiv_id = source["data_sum_indiv_id"]
+                    if key == "data_dif_indiv_id":
+                        self.data_dif_indiv_id = source["data_dif_indiv_id"]
+                    bob = 1
 
                 if key == "set":
                     setattr(self, key, source[key])
```

## vespa/analysis/block_raw_probep.py

```diff
@@ -58,16 +58,17 @@
     def get_associated_datasets(self, is_main_dataset=True):
         """
         Return list of datasets associated with this object
         - is_main_dataset: flag for top dataset, used to stop circular references
         
         """
         # order matters here - water then metab
-        return [] if not is_main_dataset else [self.water_dataset, self.metab_dataset]
-
+        r = [self.water_dataset, self.metab_dataset] if is_main_dataset else []
+        return r
+        
 
     def set_associated_datasets(self, datasets): 
         """ 'datasets' order matters here - water[0] then metab[1] """
         if self.metab_dataset_id == '':
             self.metab_dataset = datasets[1]
         else:
             for dataset in datasets:
```

## vespa/analysis/constants.py

```diff
@@ -399,15 +399,15 @@
                                        (USER_DEFINED , "User Defined"),
                                        (ALL_ON ,       "All Voxels On"),
                                        (ALL_OFF ,      "All Voxels Off"),
                                       ))
 
 class FitPriorCalculateCombinations(object):
     """ lists available metabolite combinations that can be calculated """
-    choices = ["naa+naag", "cr+pcr", "gpc+pcho", "cr2+pcr2", "glu+gln", "tau+glc"]
+    choices = ["gaba+", "naa+naag", "cr+pcr", "gpc+pcho", "cr2+pcr2", "glu+gln", "tau+glc"]
     
 
 class FitLineshapeModel(object):
     """ Lineshape model """
     NONE    = ''
     VOIGT   = 'voigt'
     LORENTZ = 'lorentzian'
```

## vespa/analysis/main.py

```diff
@@ -12,14 +12,15 @@
 import wx.lib.agw.aui as aui        # NB. wx.aui version throws odd wxWidgets exception on Close/Exit  ?? Not anymore in wxPython 4.0.6 ??
 import numpy as np
 #import wx.aui as aui
 
 # Our modules
 import vespa.analysis.mrs_dataset as mrs_dataset
 import vespa.analysis.notebook_datasets as notebook_datasets
+import vespa.analysis.utils as utils
 import vespa.analysis.util_menu as util_menu
 import vespa.analysis.util_analysis_config as util_analysis_config
 import vespa.analysis.util_import as util_import
 import vespa.analysis.util_file_import as util_file_import
 
 import vespa.common.constants as common_constants
 import vespa.common.util.init as util_init
@@ -90,15 +91,15 @@
         # because multiple places in the app want to use them.
         wx.GetApp().vespa.statusbar = self.statusbar
         wx.GetApp().vespa.update_title = self.update_title
 
         # set up default and user import data classes
         #
         # TODO - FIXME - bjs this is a hack for 2to3 convert ... rethink in future
-        if (sys.version_info > (3, 0)):
+        if (tuple(sys.version_info)[0:2] > (3, 0)):
             # Python 3 code in this block
             fname = os.path.join(util_misc.get_data_dir(), "analysis_import_menu_additions.ini")
         else:
             fname = os.path.join(util_misc.get_data_dir(), "analysis_import_menu_additions_py2.ini")
         classes, full_cfg, msg = util_file_import.set_import_data_classes(filename=fname)
         if msg:
             # some class was not found ... but we continue
@@ -428,14 +429,17 @@
 
     def on_menu_view_option(self, event):
         self.notebook_datasets.on_menu_view_option(event)
 
     def on_menu_view_output(self, event):
         self.notebook_datasets.on_menu_view_output(event)
 
+    def on_menu_view_derived(self, event):
+        self.notebook_datasets.on_menu_view_derived(event)
+
     def on_menu_view_results(self, event):
         self.notebook_datasets.on_menu_view_results(event)
 
     def on_menu_view_debug(self, event):
         self.notebook_datasets.on_menu_view_debug(event)
 
     def on_menu_plot_x(self, event):
@@ -452,14 +456,23 @@
 
     def on_analysis_online_user_manual(self, event):
         webbrowser.open("https://vespa-mrs.github.io/vespa.io/user_manuals/analysis_user_manual.html", 1)
 
     def on_vespa_help_online(self, event):
         webbrowser.open("https://vespa-mrs.github.io/vespa.io/", 1)
 
+    def on_util_dicom_series_sort(self, event):
+        ini_name = "util_dicom_series_sort"
+        default_path = util_analysis_config.get_path(ini_name)
+        base_path = wx.DirSelector('Select DICOM Directory', default_path)
+        if base_path != '':
+            utils.dicom_series_sort(base_path)
+            util_analysis_config.set_path(ini_name, base_path)
+
+
     def on_about(self, event):
 
         pyver = str(sys.version_info.major) + '.' + str(sys.version_info.minor)
         bit = str(8 * struct.calcsize('P')) + '-bit Python ' + pyver
         info = wx_adv.AboutDialogInfo()
         info.SetVersion(util_misc.get_vespa_version())
         info.SetCopyright("Copyright 2010, Brian J Soher. All rights reserved.")
@@ -789,13 +802,19 @@
     config = util_analysis_config.Config()
 
     position, size = config.get_window_coordinates("main")
     frame = Main(db, position, size)
     app.SetTopWindow(frame)
     frame.Show()
 
-#    import cProfile
+    # import cProfile
+    # import pstats as ps
+    # fname = 'D:\\Users\\bsoher\\profile.data'
+    # if os.path.exists(fname):
+    #     os.remove(fname)
+
     app.MainLoop()
-#    cProfile.run('app.MainLoop()')
 
-#    to time this call user
-#    >python -m cProfile -s cumulative bloch_lib_hargreaves.py
+    # cProfile.run('app.MainLoop()', fname)
+    # p = ps.Stats(fname)
+    # p.strip_dirs().sort_stats('cumulative').print_stats()
+    #
```

## vespa/analysis/mrs_dataset.py

```diff
@@ -8,14 +8,15 @@
 import xml.etree.cElementTree as ElementTree
 
 # Our modules
 import vespa.analysis.constants as constants
 import vespa.analysis.block_raw as block_raw
 import vespa.analysis.block_raw_probep as block_raw_probep
 import vespa.analysis.block_raw_cmrr_slaser as block_raw_cmrr_slaser
+import vespa.analysis.block_raw_edit as block_raw_edit
 import vespa.analysis.block_raw_edit_fidsum as block_raw_edit_fidsum
 import vespa.analysis.block_prep_identity as block_prep_identity
 import vespa.analysis.block_prep_fidsum as block_prep_fidsum
 import vespa.analysis.block_prep_timeseries as block_prep_timeseries
 import vespa.analysis.block_prep_wbnaa as block_prep_wbnaa
 import vespa.analysis.block_prep_edit_fidsum as block_prep_edit_fidsum
 import vespa.analysis.block_spectral as block_spectral
@@ -154,14 +155,15 @@
 # _XML_TAG_TO_SLOT_CLASS_MAP maps XML element tags to 2-tuples of
 # (slot name, block class) where slot name is one of "raw", "prep", "spectral",
 # or "fit" and the class can be any class appropriate for that slot.
 _XML_TAG_TO_SLOT_CLASS_MAP = {
     "block_raw"                 : ("raw", block_raw.BlockRaw),
     "block_raw_probep"          : ("raw", block_raw_probep.BlockRawProbep),
     "block_raw_cmrr_slaser"     : ("raw", block_raw_cmrr_slaser.BlockRawCmrrSlaser),
+    "block_raw_edit"            : ("raw", block_raw_edit.BlockRawEdit),
     "block_raw_edit_fidsum"     : ("raw", block_raw_edit_fidsum.BlockRawEditFidsum),
     "block_prep_identity"       : ("prep", block_prep_identity.BlockPrepIdentity),
     "block_prep_fidsum"         : ("prep", block_prep_fidsum.BlockPrepFidsum),
     "block_prep_timeseries"     : ("prep", block_prep_timeseries.BlockPrepTimeseries),
     "block_prep_edit_fidsum"    : ("prep", block_prep_edit_fidsum.BlockPrepEditFidsum),
     "block_prep_wbnaa"          : ("prep", block_prep_wbnaa.BlockPrepWbnaa),
     "block_spectral_identity"   : ("spectral", block_spectral_identity.BlockSpectralIdentity),
@@ -995,19 +997,29 @@
 
         prior_list_unique = self.prior_list_unique
 
         combos = []
 
         all_combos = constants.FitPriorCalculateCombinations.choices
         for item in all_combos:
-            met1, met2 = item.split('+')
-            if met1 in prior_list_unique and met2 in prior_list_unique:
-                imet1 = prior_list_unique.index(met1)
-                imet2 = prior_list_unique.index(met2)
-                combos.append([item, res[imet1]+res[imet2]])
+            if item == 'gaba+':
+                if self.blocks["fit"].set.macromol_model == FitMacromoleculeMethod.SINGLE_BASIS_DATASET:
+                    nmet = len(prior_list_unique)
+                    if 'gaba' in prior_list_unique:
+                        igaba = prior_list_unique.index('gaba')
+                        combos.append(['gaba+', res[igaba]+res[nmet*2+4]])
+                    if 'gaba_umn' in prior_list_unique:
+                        igaba = prior_list_unique.index('gaba_umn')
+                        combos.append(['gaba+', res[igaba]+res[nmet*2+4]])
+            else:
+                met1, met2 = item.split('+')
+                if met1 in prior_list_unique and met2 in prior_list_unique:
+                    imet1 = prior_list_unique.index(met1)
+                    imet2 = prior_list_unique.index(met2)
+                    combos.append([item, res[imet1]+res[imet2]])
 
         if combos == []:
             combos = None
 
         return combos
 
 
@@ -2026,15 +2038,14 @@
             else:
                 tmp = ['MMol', res[nmet*2+4]]
                 if do_crao: tmp.append(0.0)
                 if do_conf: tmp.append(0.0)
             table1.append(tmp)
 
         if fit.set.prior_calculate_combinations:
-            #combo = self.get_combo_results(voxel)
             combo = self.get_combo_results(voxel, quant=True)
             if combo is not None:
                 for item in combo:
                     if format_float:
                         tmp = [item[0], fmt_area % item[1]]
                         if do_crao: tmp.append(fmt_arcr % 0.0)
                         if do_conf: tmp.append(fmt_arcr % 0.0)
@@ -2174,15 +2185,15 @@
                 # gather all associated datasets, unique or not
                 all_datasets += block.get_associated_datasets(is_main_dataset)
 
             for item in all_datasets:
                 # create list of unique associated datasets maintaining order but
                 # also be sure that we do not include ourselves. This could occur
                 # in Edited datasets which have on/off/add/sub states.
-                if item not in unique_datasets and item is not self:
+                if item not in unique_datasets and item is not self and item is not None:
                     unique_datasets.append(item)
 
             # rename all dataset IDs if main dataset
             for dataset in unique_datasets:
                 # As we save these associated datasets, we want to use unique
                 # ids that won't collide with ids in memory now, should they
                 # be loaded right back in again. So here the dataset.id is changed
@@ -2191,15 +2202,15 @@
                 # associated datasets ids are restored
 
                 dataset.id_saved = dataset.id
                 dataset.id = util_misc.uuid()
 
             # save all associated datasets if main
             for dataset in unique_datasets:
-                # FIXME - BJS test if this is a true thing, we do NOT want
+                # TODO - BJS test if this is a true thing, we do NOT want
                 #   to save any associated datasets when we do presets save
                 if not self.behave_as_preset:
                     associated.append(dataset.deflate(flavor, is_main_dataset=False))
 
 
         if flavor == Deflate.ETREE:
             e = ElementTree.Element("dataset",
```

### html2text {}

```diff
@@ -1,12 +1,13 @@
 # Python modules import os import copy import collections # 3rd party modules
 import numpy as np import xml.etree.cElementTree as ElementTree # Our modules
 import vespa.analysis.constants as constants import vespa.analysis.block_raw as
 block_raw import vespa.analysis.block_raw_probep as block_raw_probep import
 vespa.analysis.block_raw_cmrr_slaser as block_raw_cmrr_slaser import
+vespa.analysis.block_raw_edit as block_raw_edit import
 vespa.analysis.block_raw_edit_fidsum as block_raw_edit_fidsum import
 vespa.analysis.block_prep_identity as block_prep_identity import
 vespa.analysis.block_prep_fidsum as block_prep_fidsum import
 vespa.analysis.block_prep_timeseries as block_prep_timeseries import
 vespa.analysis.block_prep_wbnaa as block_prep_wbnaa import
 vespa.analysis.block_prep_edit_fidsum as block_prep_edit_fidsum import
 vespa.analysis.block_spectral as block_spectral import
@@ -67,14 +68,15 @@
 "14023031-ad45-4662-a89c-4e35d8732244" # deprecated, so hard wired #
 _XML_TAG_TO_SLOT_CLASS_MAP maps XML element tags to 2-tuples of # (slot name,
 block class) where slot name is one of "raw", "prep", "spectral", # or "fit"
 and the class can be any class appropriate for that slot.
 _XML_TAG_TO_SLOT_CLASS_MAP = { "block_raw" : ("raw", block_raw.BlockRaw),
 "block_raw_probep" : ("raw", block_raw_probep.BlockRawProbep),
 "block_raw_cmrr_slaser" : ("raw", block_raw_cmrr_slaser.BlockRawCmrrSlaser),
+"block_raw_edit" : ("raw", block_raw_edit.BlockRawEdit),
 "block_raw_edit_fidsum" : ("raw", block_raw_edit_fidsum.BlockRawEditFidsum),
 "block_prep_identity" : ("prep", block_prep_identity.BlockPrepIdentity),
 "block_prep_fidsum" : ("prep", block_prep_fidsum.BlockPrepFidsum),
 "block_prep_timeseries" : ("prep", block_prep_timeseries.BlockPrepTimeseries),
 "block_prep_edit_fidsum" : ("prep",
 block_prep_edit_fidsum.BlockPrepEditFidsum), "block_prep_wbnaa" : ("prep",
 block_prep_wbnaa.BlockPrepWbnaa), "block_spectral_identity" : ("spectral",
@@ -449,34 +451,40 @@
 = copy.deepcopy(preset.user_prior) self.user_prior.basis.update(self) # parent
 dataset may have different points/dwell self.preset_filename = presetfile def
 get_combo_results(self, voxel, quant=False): block = self.blocks["quant"] if
 quant else self.blocks["fit"] if block.is_identity: return None if quant: res =
 block.watref_results[:,voxel[0],voxel[1],voxel[2]] else: res =
 block.fit_results[:,voxel[0],voxel[1],voxel[2]] prior_list_unique =
 self.prior_list_unique combos = [] all_combos =
-constants.FitPriorCalculateCombinations.choices for item in all_combos: met1,
-met2 = item.split('+') if met1 in prior_list_unique and met2 in
-prior_list_unique: imet1 = prior_list_unique.index(met1) imet2 =
-prior_list_unique.index(met2) combos.append([item, res[imet1]+res[imet2]]) if
-combos == []: combos = None return combos def fit_results_as_html(self, voxel,
-lw=0.0, lwmin=0.0, lwmax=0.0, data_source="", image=None): """ Given a voxel,
-linewidth params, and a data source (often a filename), returns HTML-formatted
-results for that voxel. The HTML is appropriate for the wx.Html control (which
-understand limited HTML) as well as for writing to a file. If the image param
-is populated, it should be a tuple of (mime_type, image_data). The former
-should be a string like "image/png". The latter should be base64-encoded image
-data. """ fit = self.blocks["fit"] # First we assemble the data we need. nmet =
-len(fit.set.prior_list) names = fit.set.prior_list res = fit.fit_results
-[:,voxel[0],voxel[1],voxel[2]] crao = fit.cramer_rao[:,voxel[0],voxel[1],voxel
-[2]] conf = fit.confidence[:,voxel[0],voxel[1],voxel[2]] stats = fit.fit_stats
-[:,voxel[0],voxel[1],voxel[2]] # both cramer-rao and confidence intervals may
-be off/on if len(crao) != len(res): crao = res * 0 if len(conf) != len(res):
-conf = res * 0 table1 = [['Area Results', 'Area', ' CrRao[%]', ' CnfInt[%]']]
-for i, item in enumerate(names): table1.append([item, res[i], crao[i], conf
-[i]]) if fit.set.macromol_model == FitMacromoleculeMethod.SINGLE_BASIS_DATASET:
+constants.FitPriorCalculateCombinations.choices for item in all_combos: if item
+== 'gaba+': if self.blocks["fit"].set.macromol_model ==
+FitMacromoleculeMethod.SINGLE_BASIS_DATASET: nmet = len(prior_list_unique) if
+'gaba' in prior_list_unique: igaba = prior_list_unique.index('gaba')
+combos.append(['gaba+', res[igaba]+res[nmet*2+4]]) if 'gaba_umn' in
+prior_list_unique: igaba = prior_list_unique.index('gaba_umn') combos.append(
+['gaba+', res[igaba]+res[nmet*2+4]]) else: met1, met2 = item.split('+') if met1
+in prior_list_unique and met2 in prior_list_unique: imet1 =
+prior_list_unique.index(met1) imet2 = prior_list_unique.index(met2)
+combos.append([item, res[imet1]+res[imet2]]) if combos == []: combos = None
+return combos def fit_results_as_html(self, voxel, lw=0.0, lwmin=0.0,
+lwmax=0.0, data_source="", image=None): """ Given a voxel, linewidth params,
+and a data source (often a filename), returns HTML-formatted results for that
+voxel. The HTML is appropriate for the wx.Html control (which understand
+limited HTML) as well as for writing to a file. If the image param is
+populated, it should be a tuple of (mime_type, image_data). The former should
+be a string like "image/png". The latter should be base64-encoded image data.
+""" fit = self.blocks["fit"] # First we assemble the data we need. nmet = len
+(fit.set.prior_list) names = fit.set.prior_list res = fit.fit_results[:,voxel
+[0],voxel[1],voxel[2]] crao = fit.cramer_rao[:,voxel[0],voxel[1],voxel[2]] conf
+= fit.confidence[:,voxel[0],voxel[1],voxel[2]] stats = fit.fit_stats[:,voxel
+[0],voxel[1],voxel[2]] # both cramer-rao and confidence intervals may be off/on
+if len(crao) != len(res): crao = res * 0 if len(conf) != len(res): conf = res *
+0 table1 = [['Area Results', 'Area', ' CrRao[%]', ' CnfInt[%]']] for i, item in
+enumerate(names): table1.append([item, res[i], crao[i], conf[i]]) if
+fit.set.macromol_model == FitMacromoleculeMethod.SINGLE_BASIS_DATASET:
 table1.append(['MMol', res[nmet*2+4], 0.0, 0.0]) if
 fit.set.prior_calculate_combinations: combo = self.get_combo_results(voxel) if
 combo is not None: for item in combo: table1.append([item[0], item[1], 0.0,
 0.0]) table1 = _pretty_space_table(table1, places=4) table2 = [['PPM Results',
 'PPM', ' CrRao[ppm]', ' CnfInt[ppm]']] for i,item in enumerate(names):
 table2.append([item, res[i+nmet], crao[i+nmet], conf[i+nmet]]) if
 fit.set.macromol_model == FitMacromoleculeMethod.SINGLE_BASIS_DATASET:
@@ -849,40 +857,40 @@
 (fmt_arcr % crao[i]) if do_conf: tmp.append(fmt_arcr % conf[i]) else: tmp =
 [item, res[i]] if do_crao: tmp.append(crao[i]) if do_conf: tmp.append(conf[i])
 table1.append(tmp) if fit.set.macromol_model ==
 FitMacromoleculeMethod.SINGLE_BASIS_DATASET: if format_float: tmp = ['MMol',
 fmt_area % res[nmet*2+4]] if do_crao: tmp.append(fmt_arcr % 0.0) if do_conf:
 tmp.append(fmt_arcr % 0.0) else: tmp = ['MMol', res[nmet*2+4]] if do_crao:
 tmp.append(0.0) if do_conf: tmp.append(0.0) table1.append(tmp) if
-fit.set.prior_calculate_combinations: #combo = self.get_combo_results(voxel)
-combo = self.get_combo_results(voxel, quant=True) if combo is not None: for
-item in combo: if format_float: tmp = [item[0], fmt_area % item[1]] if do_crao:
-tmp.append(fmt_arcr % 0.0) if do_conf: tmp.append(fmt_arcr % 0.0) else: tmp =
-[item[0], item[1]] if do_crao: tmp.append(0.0) if do_conf: tmp.append(0.0)
-table1.append(tmp) nsect.append(len(table1)) if not noppm: table1.append(hdr2)
-for i,item in enumerate(names): if format_float: tmp = [item, fmt_ppm % res
-[i+nmet]] if do_crao: tmp.append(fmt_ppcr % crao[i+nmet]) if do_conf:
-tmp.append(fmt_ppcr % conf[i+nmet]) else: tmp = [item, res[i+nmet]] if do_crao:
-tmp.append(crao[i+nmet]) if do_conf: tmp.append(conf[i+nmet]) table1.append
-(tmp) if fit.set.macromol_model == FitMacromoleculeMethod.SINGLE_BASIS_DATASET:
-if format_float: tmp = ['MMol', fmt_ppm % res[nmet*2+5]] if do_crao: tmp.append
-(fmt_ppcr % 0.0) if do_conf: tmp.append(fmt_ppcr % 0.0) else: tmp = ['MMol',
-res[nmet*2+5]] if do_crao: tmp.append(0.0) if do_conf: tmp.append(0.0)
-table1.append(tmp) nsect.append(len(table1)) table1.append(hdr3) tmp = ['Ta',
-res[nmet*2+0]] if do_crao: tmp.append(crao[nmet*2+0]) if do_conf: tmp.append
-(conf[nmet*2+0]) table1.append(tmp) tmp = ['Tb', res[nmet*2+1]] if do_crao:
-tmp.append(crao[nmet*2+1]) if do_conf: tmp.append(conf[nmet*2+1]) table1.append
-(tmp) if not fixphase: tmp = ['Phase0', res[nmet*2+2]] if do_crao: tmp.append
-(crao[nmet*2+2]) if do_conf: tmp.append(conf[nmet*2+2]) table1.append(tmp) tmp
-= ['Phase1', res[nmet*2+3]] if do_crao: tmp.append(crao[nmet*2+3]) if do_conf:
-tmp.append(conf[nmet*2+3]) table1.append(tmp) else: tmp = ['Phase0', '0.0
-('+str(np.round(res[nmet*2+2],1))+')'] if do_crao: tmp.append(crao[nmet*2+2])
-if do_conf: tmp.append(conf[nmet*2+2]) table1.append(tmp) tmp = ['Phase1', '0.0
-('+str(np.round(res[nmet*2+3],1))+')'] if do_crao: tmp.append(crao[nmet*2+3])
-if do_conf: tmp.append(conf[nmet*2+3]) table1.append(tmp) nsect.append(len
+fit.set.prior_calculate_combinations: combo = self.get_combo_results(voxel,
+quant=True) if combo is not None: for item in combo: if format_float: tmp =
+[item[0], fmt_area % item[1]] if do_crao: tmp.append(fmt_arcr % 0.0) if
+do_conf: tmp.append(fmt_arcr % 0.0) else: tmp = [item[0], item[1]] if do_crao:
+tmp.append(0.0) if do_conf: tmp.append(0.0) table1.append(tmp) nsect.append(len
+(table1)) if not noppm: table1.append(hdr2) for i,item in enumerate(names): if
+format_float: tmp = [item, fmt_ppm % res[i+nmet]] if do_crao: tmp.append
+(fmt_ppcr % crao[i+nmet]) if do_conf: tmp.append(fmt_ppcr % conf[i+nmet]) else:
+tmp = [item, res[i+nmet]] if do_crao: tmp.append(crao[i+nmet]) if do_conf:
+tmp.append(conf[i+nmet]) table1.append(tmp) if fit.set.macromol_model ==
+FitMacromoleculeMethod.SINGLE_BASIS_DATASET: if format_float: tmp = ['MMol',
+fmt_ppm % res[nmet*2+5]] if do_crao: tmp.append(fmt_ppcr % 0.0) if do_conf:
+tmp.append(fmt_ppcr % 0.0) else: tmp = ['MMol', res[nmet*2+5]] if do_crao:
+tmp.append(0.0) if do_conf: tmp.append(0.0) table1.append(tmp) nsect.append(len
+(table1)) table1.append(hdr3) tmp = ['Ta', res[nmet*2+0]] if do_crao:
+tmp.append(crao[nmet*2+0]) if do_conf: tmp.append(conf[nmet*2+0]) table1.append
+(tmp) tmp = ['Tb', res[nmet*2+1]] if do_crao: tmp.append(crao[nmet*2+1]) if
+do_conf: tmp.append(conf[nmet*2+1]) table1.append(tmp) if not fixphase: tmp =
+['Phase0', res[nmet*2+2]] if do_crao: tmp.append(crao[nmet*2+2]) if do_conf:
+tmp.append(conf[nmet*2+2]) table1.append(tmp) tmp = ['Phase1', res[nmet*2+3]]
+if do_crao: tmp.append(crao[nmet*2+3]) if do_conf: tmp.append(conf[nmet*2+3])
+table1.append(tmp) else: tmp = ['Phase0', '0.0 ('+str(np.round(res
+[nmet*2+2],1))+')'] if do_crao: tmp.append(crao[nmet*2+2]) if do_conf:
+tmp.append(conf[nmet*2+2]) table1.append(tmp) tmp = ['Phase1', '0.0 ('+str
+(np.round(res[nmet*2+3],1))+')'] if do_crao: tmp.append(crao[nmet*2+3]) if
+do_conf: tmp.append(conf[nmet*2+3]) table1.append(tmp) nsect.append(len
 (table1)) table1.append(hdr4) tmp = ['Linewidth', lw] if do_crao: tmp.append('
 ') if do_conf: tmp.append(' ') table1.append(tmp) if not short_form: tmp =
 ['ChiSquare', stats[0]] if do_crao: tmp.append(' ') if do_conf: tmp.append(' ')
 table1.append(tmp) tmp = ['Weighted ChiSquare', stats[1]] if do_crao:
 tmp.append(' ') if do_conf: tmp.append(' ') table1.append(tmp) if not
 short_form: matherr = str(stats[2] != 0) tmp = ['Math Finite Error', matherr]
 if do_crao: tmp.append(' ') if do_conf: tmp.append(' ') table1.append(tmp)
@@ -905,31 +913,31 @@
 we gather all associated datasets, filter for uniqueness, change # the id,
 deflate it then change the id back for the currently open # dataset.
 all_datasets = [] for block in self.blocks.values(): # gather all associated
 datasets, unique or not all_datasets += block.get_associated_datasets
 (is_main_dataset) for item in all_datasets: # create list of unique associated
 datasets maintaining order but # also be sure that we do not include ourselves.
 This could occur # in Edited datasets which have on/off/add/sub states. if item
-not in unique_datasets and item is not self: unique_datasets.append(item) #
-rename all dataset IDs if main dataset for dataset in unique_datasets: # As we
-save these associated datasets, we want to use unique # ids that won't collide
-with ids in memory now, should they # be loaded right back in again. So here
-the dataset.id is changed # and deflated. Then all the rest of the main dataset
-(including # any refs to the associated datasets) are deflated. Then the #
-associated datasets ids are restored dataset.id_saved = dataset.id dataset.id =
-util_misc.uuid() # save all associated datasets if main for dataset in
-unique_datasets: # FIXME - BJS test if this is a true thing, we do NOT want #
-to save any associated datasets when we do presets save if not
-self.behave_as_preset: associated.append(dataset.deflate(flavor,
-is_main_dataset=False)) if flavor == Deflate.ETREE: e = ElementTree.Element
-("dataset", { "id" : self.id, "version" : self.XML_VERSION}) if
-self.behave_as_preset: util_xml.TextSubElement(e, "behave_as_preset",
-self.behave_as_preset) util_xml.TextSubElement(e, "preset_filename",
-self.preset_filename) e.append(self.user_prior.deflate()) ee =
-ElementTree.SubElement(e, "blocks") for block in self.blocks.values(): if not
+not in unique_datasets and item is not self and item is not None:
+unique_datasets.append(item) # rename all dataset IDs if main dataset for
+dataset in unique_datasets: # As we save these associated datasets, we want to
+use unique # ids that won't collide with ids in memory now, should they # be
+loaded right back in again. So here the dataset.id is changed # and deflated.
+Then all the rest of the main dataset (including # any refs to the associated
+datasets) are deflated. Then the # associated datasets ids are restored
+dataset.id_saved = dataset.id dataset.id = util_misc.uuid() # save all
+associated datasets if main for dataset in unique_datasets: # TODO - BJS test
+if this is a true thing, we do NOT want # to save any associated datasets when
+we do presets save if not self.behave_as_preset: associated.append
+(dataset.deflate(flavor, is_main_dataset=False)) if flavor == Deflate.ETREE: e
+= ElementTree.Element("dataset", { "id" : self.id, "version" :
+self.XML_VERSION}) if self.behave_as_preset: util_xml.TextSubElement(e,
+"behave_as_preset", self.behave_as_preset) util_xml.TextSubElement(e,
+"preset_filename", self.preset_filename) e.append(self.user_prior.deflate()) ee
+= ElementTree.SubElement(e, "blocks") for block in self.blocks.values(): if not
 block.is_identity: ee.append(block.deflate()) #else: # We don't clutter up the
 XML with identity blocks. if associated and is_main_dataset: # e goes at the
 end here so that later when we reload this dataset, # all assoc datasets are
 loaded in before we try to load this 'main' one associated.append(e) e =
 associated return e elif flavor == Deflate.DICTIONARY: return
 self.__dict__.copy() if is_main_dataset: for dataset in unique_datasets: #
 Restore the original UUID in associated datasets dataset.id = dataset.id_saved
```

## vespa/analysis/notebook_datasets.py

```diff
@@ -10,15 +10,17 @@
 
 # Our modules
 import vespa.analysis.util_menu as util_menu
 import vespa.analysis.tab_dataset as tab_dataset
 import vespa.analysis.block_prep_fidsum as block_prep_fidsum
 import vespa.analysis.block_raw_probep as block_raw_probep
 import vespa.analysis.block_prep_wbnaa as block_prep_wbnaa
+import vespa.analysis.block_raw_edit as block_raw_edit
 import vespa.analysis.block_raw_cmrr_slaser as block_raw_cmrr_slaser
+import vespa.analysis.block_raw_edit as block_raw_edit
 import vespa.analysis.block_raw_edit_fidsum as block_raw_edit_fidsum
 import vespa.analysis.block_prep_timeseries as block_prep_timeseries
 
 import vespa.common.util.misc as util_misc
 import vespa.common.wx_gravy.util as wx_util
 import vespa.common.wx_gravy.notebooks as vespa_notebooks
 
@@ -75,14 +77,18 @@
         if self.active_tab:
             self.active_tab.on_menu_view_option(event)
 
     def on_menu_view_output(self, event):
         if self.active_tab:
             self.active_tab.on_menu_view_output(event)
 
+    def on_menu_view_derived(self, event):
+        if self.active_tab:
+            self.active_tab.on_menu_view_derived(event)
+
     def on_menu_view_results(self, event):
         if self.active_tab:
             self.active_tab.on_menu_view_results(event)
 
     def on_menu_view_debug(self, event):
         if self.active_tab:
             self.active_tab.on_menu_view_debug(event)
@@ -113,15 +119,16 @@
     def on_tab_close(self, event):
         """
         This is a two step event. Here we give the user a chance to cancel
         the Close action. If user selects to continue, then the on_tab_closed()
         event will also fire.  event.GetPageCound()
 
         """
-        assoc_classes = (block_raw_edit_fidsum.BlockRawEditFidsum,
+        assoc_classes = (block_raw_edit.BlockRawEdit,
+                         block_raw_edit_fidsum.BlockRawEditFidsum,
                          block_raw_cmrr_slaser.BlockRawCmrrSlaser,
                          block_raw_probep.BlockRawProbep)
         
         
         raw = self.active_tab.dataset.blocks['raw']
         if isinstance(raw, assoc_classes):
             if not self.associated_close:
@@ -223,21 +230,25 @@
     #=======================================================
     #
     #           Public methods shown below
     #             in alphabetical order
     #
     #=======================================================
 
-    def add_dataset_tab(self, datasets=None):
+    def add_dataset_tab(self, datasets=None, force_name=None):
         # If the welcome tab is open, close it.
         if self.is_welcome_tab_open:
             self.DeletePage(0)
 
-        names, count = self.custom_tab_names(datasets, self.count)
-        self.count = count
+        if force_name is None:
+            names, count = self.custom_tab_names(datasets, self.count)
+            self.count = count
+        else:
+            # NB. there should only be one dataset and one forced name
+            names = [force_name,]
 
         for i,dataset in enumerate(datasets):
 
             name = names[i]
 
             # register Dataset object at top level
             self.top.datasets[name] = dataset                   # NAME HAS TO BE UNIQUE!!!
@@ -263,52 +274,32 @@
                 return self.GetPage(i)
 
         return None
 
 
     def global_poll_associated_tabs(self, dataset):
         """
-        Here is the list of object classes that we polling for associated tabs:
+        Here is the list of object classes that we poll for associated tabs:
         
+          block_raw_edit.BlockRawEdit
           block_raw_edit_fidsum.BlockRawEditFidsum
           block_raw_cmrr_slaser.BlockRawCmrrSlaser  
         
         
         """
-        assoc_classes = (block_raw_edit_fidsum.BlockRawEditFidsum,
+        assoc_classes = (block_raw_edit.BlockRawEdit,
+                         block_raw_edit_fidsum.BlockRawEditFidsum,
                          block_raw_cmrr_slaser.BlockRawCmrrSlaser,
                          block_raw_probep.BlockRawProbep)
         tabs = []
         raw = dataset.blocks['raw']
 
-        # if isinstance(raw, block_raw_edit_fidsum.BlockRawEditFidsum):
-        #     ids = [raw.data_on.id, raw.data_off.id, raw.data_sum.id, raw.data_dif.id]
-        #     for label in list(self.top.datasets.keys()):
-        #         tab = self.get_tab_by_label(label)
-        #         if tab.dataset.id in ids and tab.dataset.id != dataset.id:
-        #             tabs.append(tab)
-        #
-        # elif isinstance(raw, block_raw_probep.BlockRawProbep):
-        #     ids = [raw.data_on.id, raw.data_off.id, raw.data_sum.id, raw.data_dif.id]
-        #     for label in list(self.top.datasets.keys()):
-        #         tab = self.get_tab_by_label(label)
-        #         if tab.dataset.id in ids and tab.dataset.id != dataset.id:
-        #             tabs.append(tab)
-        #
-        # elif isinstance(raw, block_raw_cmrr_slaser.BlockRawCmrrSlaser):
-        #     ids = [raw.data_coil_combine, raw.data_ecc1, raw.data_water1, raw.data_metab64, raw.data_ecc2, raw.data_water2]
-        #     ids = [item.id for item in ids if item is not None]
-        #     for label in list(self.top.datasets.keys()):
-        #         tab = self.get_tab_by_label(label)
-        #         if tab.dataset.id in ids and tab.dataset.id != dataset.id:
-        #             tabs.append(tab)
-
         if isinstance(raw, assoc_classes):
-            ids = raw.get_associated_datasets()
-            ids = [item.id for item in ids if item is not None]
+            dsets = raw.get_associated_datasets()
+            ids = [item.id for item in dsets if item is not None]
             for label in list(self.top.datasets.keys()):
                 tab = self.get_tab_by_label(label)
                 if tab.dataset.id in ids and tab.dataset.id != dataset.id:
                     tabs.append(tab)
         else:
             return tabs
 
@@ -640,17 +631,81 @@
                 if ".water" in fname:
                     names.append("Probe%d.Water" % count)
                 elif ".metab" in fname:
                     names.append("Probe%d.Metab" % count)
                 else:
                     names.append("Probe%d.Unknown" % count)
 
+        elif isinstance(dataset.blocks['raw'], block_raw_edit.BlockRawEdit):
+            base = "Edit%d." % count
+            ndatasets = len(datasets)
+            if ndatasets == 2:
+                names = [base+"On", base+"Off"]
+            elif ndatasets==4:
+                names = [base+"On", base+"Off", base+"Sum", base+"Dif"]
+            elif ndatasets>4:
+                # generally should not happen
+                names = [base+"On", base+"Off", base+"Sum"]
+                for i in range(len(datasets)-4):
+                    names.append("Dataset%d_%d." % (count, i))
+                names.append(base+"Dif")
+            count += 1
+
         elif isinstance(dataset.blocks['raw'], block_raw_edit_fidsum.BlockRawEditFidsum):
+            ds = datasets[0]
+            raw = ds.blocks['raw']
+            ndatasets = len(datasets)
             base = "Edit%d." % count
-            names = [base+"On", base+"Off", base+"Sum", base+"Dif"]
+
+            ids = {}
+            ids['On'] = raw.data_on_id
+            ids['Off'] = raw.data_off_id
+            ids['Sum'] = raw.data_sum_id
+            ids['Dif'] = raw.data_dif_id
+            ids['SumIndiv'] = raw.data_sum_indiv_id
+            ids['DifIndiv'] = raw.data_dif_indiv_id
+
+            labels = {}
+            labels[raw.data_on_id] = 'On'
+            labels[raw.data_off_id] = 'Off'
+            labels[raw.data_sum_id] = 'Sum'
+            labels[raw.data_dif_id] = 'Dif'
+            labels[raw.data_sum_indiv_id] = 'SumIndiv'
+            labels[raw.data_dif_indiv_id] = 'DifIndiv'
+
+            nids = 0
+            for val in list(ids.values()):
+                if val != '':
+                    nids+=1
+
+            if nids > 0:
+                # Set names from Associated datasets info, others set to 'DataseN'
+
+                names = []
+                other_count = 0
+                for dset in datasets:
+                    if dset.id in labels.keys():
+                        names.append(base+labels[dset.id])
+                    else:
+                        names.append(base+'OtherData%d'%(other_count,))
+
+
+            else:
+                # Set name from dataset position
+
+                if ndatasets == 2:
+                    names = [base+"On", base+"Off"]
+                elif ndatasets==4:
+                    names = [base+"On", base+"Off", base+"SumIndiv", base+"DifIndiv"]
+                elif ndatasets>4:
+                    # generally should not happen
+                    names = [base+"On", base+"Off", base+"SumIndiv"]
+                    for i in range(len(datasets)-4):
+                        names.append("Dataset%d_%d." % (count, i))
+                    names.append(base+"DifIndiv")
             count += 1
 
         elif isinstance(dataset.blocks['raw'], block_raw_cmrr_slaser.BlockRawCmrrSlaser):
             count += 1
             iother = 1
             names = []
             for dataset in datasets:
```

## vespa/analysis/tab_dataset.py

```diff
@@ -7,14 +7,15 @@
 #import wx.aui as aui
 import wx.lib.agw.aui as aui        # NB. wx.aui version throws odd wxWidgets exception on Close/Exit  ?? Not anymore in wxPython 4.0.6 ??
 
 # Our modules
 import vespa.analysis.util_menu as util_menu
 import vespa.analysis.block_raw as block_raw
 import vespa.analysis.block_raw_probep as block_raw_probep
+import vespa.analysis.block_raw_edit as block_raw_edit
 import vespa.analysis.block_raw_edit_fidsum as block_raw_edit_fidsum
 import vespa.analysis.block_prep_fidsum as block_prep_fidsum
 import vespa.analysis.block_prep_timeseries as block_prep_timeseries
 import vespa.analysis.block_prep_wbnaa as block_prep_wbnaa
 import vespa.analysis.block_prep_edit_fidsum as block_prep_edit_fidsum
 import vespa.analysis.block_spectral as block_spectral
 import vespa.analysis.block_fit_voigt as block_fit_voigt
@@ -120,14 +121,15 @@
                 # Identity blocks don't need a tab.
                 pass
             else:
                 # Match block/tab types. Block order determines GUI tab order
 
                 if isinstance(block, block_raw.BlockRaw) or \
                    isinstance(block, block_raw_probep.BlockRawProbep) or \
+                   isinstance(block, block_raw_edit.BlockRawEdit) or \
                    isinstance(block, block_raw_edit_fidsum.BlockRawEditFidsum):
                     tab = tab_raw.TabRaw(self, self.top, block)
                     self._tabs["raw"] = tab
                     self.NotebookDataset.AddPage(tab, "Raw", False)
 
                 elif isinstance(block, block_prep_fidsum.BlockPrepFidsum) or \
                      isinstance(block, block_prep_edit_fidsum.BlockPrepEditFidsum):
@@ -275,14 +277,17 @@
 
     def on_menu_view_option(self, event):
         self.NotebookDataset.active_tab.on_menu_view_option(event)
 
     def on_menu_view_output(self, event):
         self.NotebookDataset.active_tab.on_menu_view_output(event)
 
+    def on_menu_view_derived(self, event):
+        self.NotebookDataset.active_tab.on_menu_view_derived(event)
+
     def on_menu_view_results(self, event):
         self.NotebookDataset.active_tab.on_menu_view_results(event)
 
     def on_menu_view_debug(self, event):
         self.NotebookDataset.active_tab.on_menu_view_debug(event)
 
     def on_menu_plot_x(self, event):
```

## vespa/analysis/tab_prep_fidsum.py

```diff
@@ -422,14 +422,18 @@
     
     #=======================================================
     #
     #           Global and Menu Event Handlers 
     #
     #=======================================================
 
+    def on_destroy(self, event):
+        tab_base.Tab.on_destroy(self, event)
+        pubsub.unsubscribe(self.on_push_prep_fidsum_results, "push_prep_fidsum_results")
+
     def on_activation(self):
         super().on_activation()
         # plot is necessary here to resize img0/img1 waterfall plots
         # after a dataset loads tried a bunch of other locations, and
         # CallLater/CallAfter, but only this works ... annoying.
         self.plot()
 
@@ -969,15 +973,17 @@
     
         raw = self.dataset.blocks['raw']
         if isinstance(raw, block_raw_edit_fidsum.BlockRawEditFidsum):
             shifts = self.block.frequency_shift
             phase0 = self.block.phase_0
             phase1 = self.block.set.global_phase1
             
-            uids = [raw.data_on.id, raw.data_off.id, raw.data_sum.id, raw.data_dif.id]
+            uids = [raw.data_on.id, raw.data_off.id]
+            if raw.data_sum is not None: uids.append(raw.data_sum.id)
+            if raw.data_dif is not None: uids.append(raw.data_dif.id)
 
             pubsub.sendMessage("push_prep_fidsum_results", 
                                uids=uids, 
                                shifts=shifts, 
                                phase0=phase0, 
                                phase1=phase1)
```

## vespa/analysis/tab_prep_timeseries.py

```diff
@@ -76,14 +76,15 @@
         #------------------------------------------------------------
         # Setup the canvas 
         self.process_and_plot()
 
         #------------------------------------------------------------
         # PubSub subscriptions
 #        pubsub.subscribe(self.on_push_prep_fidsum_results, "push_prep_fidsum_results")
+# TODO bjs    don't forget to add unsubscribe() code in Destroy when tab closed
 
 
         # If the sash position isn't recorded in the INI file, we use the
         # arbitrary-ish value of 400.
         if not self._prefs.sash_position:
             self._prefs.sash_position = 400
```

## vespa/analysis/tab_spectral.py

```diff
@@ -1,21 +1,23 @@
 # Python modules
 import os
 import sys
+import importlib
 import xml.etree.cElementTree as ElementTree
 from xml.etree.cElementTree import Element
 
 # 3rd party modules
 import wx
 import wx.grid as gridlib
 import numpy as np
 from pubsub import pub as pubsub
 from wx.lib.mixins.listctrl import CheckListCtrlMixin, ColumnSorterMixin
 
 # Our modules
+import vespa.analysis.mrs_dataset as mrs_dataset
 import vespa.analysis.tab_base as tab_base
 import vespa.analysis.constants as constants
 import vespa.analysis.util_menu as util_menu
 import vespa.analysis.prefs as prefs_module
 import vespa.analysis.util_analysis_config as util_analysis_config
 import vespa.analysis.dialog_dataset_browser as dialog_dataset_browser
 import vespa.analysis.auto_gui.spectral as spectral
@@ -215,14 +217,127 @@
         pmax = max(val_min, val_max)
         obj_min.SetValue(pmin)
         obj_max.SetValue(pmax)
         return pmin, pmax    
 
 
 #------------------------------------------------------------------------------
+
+def derived_dataset(ds, dsB, view, _tab_dataset, top, mode):
+
+    if mode in ['plotc_a_plus_b', 'plotc_a_minus_b']:
+
+        # Create new tab label from current - check for uniqueness in Tab label list
+        tab_name = _tab_dataset.indexAB[0]
+        label_base = tab_name.split('.')
+        label_new = label_base[0]+'.Sum' if mode == 'plotc_a_plus_b' else label_base[0]+'.Dif'
+
+        tab_labels = list(top.datasets.keys())
+        if label_new in tab_labels:
+            msg = 'Warning (derived_dataset) - New Tab/Dataset has same label as existing Tab, adding Suffix.'
+            r = common_dialogs.message(msg, style=common_dialogs.I_OK)
+            for s in range(2,10):
+                ss = str(s)
+                label_new = label_base[0]+'.Sum'+ss if mode == 'plotc_a_plus_b' else label_base[0]+'.Dif'+ss
+                if not label_new in tab_labels:
+                    break
+
+        # Grab the A and B data, specify the derived data
+
+        stamp = util_time.now(util_time.ISO_TIMESTAMP_FORMAT).split('T')
+        if mode == 'plotc_a_plus_b':
+            labl_func = 'PlotA + PlotB'
+            dat = view.get_data(0)+view.get_data(1)
+        elif mode == 'plotc_a_minus_b':
+            labl_func = 'PlotA - PlotB'
+            dat = view.get_data(0)-view.get_data(1)
+        dat = dat.ravel()
+        dat = np.fft.ifft(np.fft.fftshift(dat))*len(dat)
+        dat.shape = 1, 1, 1, len(dat)
+
+        # Create informative header - re. provenance of this spectrum
+
+        lines = ['Derived Dataset from Analysis Spectral General Tab - PlotC ('+labl_func+')']
+        lines.append('------------------------------------------------------------------')
+        lines.append('An IFFT() was performed on the Plot C spectrum and the resultant FID written into')
+        lines.append('this Dataset object. All other parameters were taken from the parent Dataset')
+
+        lines.append(' ')
+        lines.append('Creation_date            - '+stamp[0])
+        lines.append('Creation_time            - '+stamp[1])
+        lines.append(' ')
+        lines.append('Filename Dataset A - '+str(ds.blocks['raw'].data_sources[0]))
+        lines.append('UUID Dataset A - '+str(ds.id))
+        lines.append('Filename Dataset B - '+str(dsB.blocks['raw'].data_sources[0]))
+        lines.append('UUID Dataset B - '+str(dsB.id))
+        lines = "\n".join(lines)
+        if (sys.platform == "win32"):
+            lines = lines.replace("\n", "\r\n")
+
+        # Create raw data object
+        met = mrs_data_raw.DataRawEdit()
+        met.data_sources = ['analysis_spectral_plotc_derived_dataset_edit_sum_dif']  # todo bjs - set on/off filenames
+        met.sw = ds.sw
+        met.frequency = ds.frequency
+        met.resppm = ds.resppm
+        met.echopeak = ds.echopeak
+        met.nucleus = ds.nucleus
+        met.seqte = ds.seqte
+        met.seqtr = ds.seqtr
+        met.voxel_dimensions = ds.blocks['raw'].voxel_dimensions
+        met.headers = [lines]
+        met.data = dat
+        met.transform = ds.blocks['raw'].transform
+
+        # Convert Raw to Dataset - from util_file_import.get_datasets() line 356-ish
+        block_classes = {}
+        block_classes["raw"] = getattr(importlib.import_module('vespa.analysis.block_raw_edit'), 'BlockRawEdit')
+        derived = mrs_dataset.dataset_from_raw(met, block_classes, ds.zero_fill_multiplier)
+
+        # set up associated datasets in original and derived objects
+        # - get existing values first from original
+        # - overwrite with derived values
+
+        derived.blocks['raw'].data_off_id = ds.id
+        derived.blocks['raw'].data_off = ds
+        derived.blocks['raw'].data_on_id = dsB.id
+        derived.blocks['raw'].data_on = dsB
+        derived.blocks['raw'].data_sum_id = ds.blocks['raw'].data_sum_id
+        derived.blocks['raw'].data_sum = ds.blocks['raw'].data_sum
+        derived.blocks['raw'].data_dif_id = ds.blocks['raw'].data_dif_id
+        derived.blocks['raw'].data_dif = ds.blocks['raw'].data_dif
+        derived.blocks['raw'].data_sum_indiv_id = ds.blocks['raw'].data_sum_indiv_id
+        derived.blocks['raw'].data_sum_indiv = ds.blocks['raw'].data_sum_indiv
+        derived.blocks['raw'].data_dif_indiv_id = ds.blocks['raw'].data_dif_indiv_id
+        derived.blocks['raw'].data_dif_indiv = ds.blocks['raw'].data_dif_indiv
+
+        if mode == 'plotc_a_plus_b':
+            derived.blocks['raw'].data_sum_id = derived.id
+            derived.blocks['raw'].data_sum = derived
+            for ds in list(top.datasets.values()):
+                raw = ds.blocks['raw']
+                if hasattr(raw, 'data_sum_id'): raw.data_sum_id = derived.id
+                if hasattr(raw, 'data_sum'): raw.data_sum = derived
+        elif mode == 'plotc_a_minus_b':
+            derived.blocks['raw'].data_dif_id = derived.id
+            derived.blocks['raw'].data_dif = derived
+            for ds in list(top.datasets.values()):
+                raw = ds.blocks['raw']
+                if hasattr(raw, 'data_dif_id'): raw.data_dif_id = derived.id
+                if hasattr(raw, 'data_dif'): raw.data_dif = derived
+
+        # insert into Tab Notebook
+        _tab_dataset._outer_notebook.add_dataset_tab(datasets=[derived, ], force_name=label_new)
+
+
+
+
+
+
+#------------------------------------------------------------------------------
 #
 #  Tab SPECTRAL
 #
 #------------------------------------------------------------------------------
 
 class TabSpectral(tab_base.Tab, spectral.PanelSpectralUI):
     
@@ -745,14 +860,19 @@
 
     #=======================================================
     #
     #           Global and Menu Event Handlers
     #
     #=======================================================
 
+    def on_destroy(self, event):
+        tab_base.Tab.on_destroy(self, event)
+        pubsub.subscribe(self.on_check_datasetb_status, "check_datasetb_status")
+        pubsub.subscribe(self.on_dataset_keys_change, "dataset_keys_change")
+
     def on_activation(self):
         tab_base.Tab.on_activation(self)
 
         # these BlockSpectral object values may be changed by other tabs, so
         # update their widget values on activation of this tab
         voxel      = self._tab_dataset.voxel
         freq_shift = self.dataset.get_frequency_shift(voxel)
@@ -855,77 +975,133 @@
                 if event_id == util_menu.ViewIdsSpectral.USER_BUTTON_PHASING:
                     label = 'Do Automatic Phasing'
                 elif event_id == util_menu.ViewIdsSpectral.USER_BUTTON_AREA:
                     label = 'Output Area Value'
                 self.ButtonUserFunction.SetLabel(label)
 
 
+    def on_menu_view_derived(self, event):
+        event_id = event.GetId()
+
+        if event_id == util_menu.ViewIdsSpectral.PLOTA_FID_TO_BINARY:
+            filename = common_dialogs.save_as("Plot A FID to Binary", "BIN files (*.bin)|*.bin", default_filename='analysis_plota_fid_to_binary.bin')
+            if filename:
+                data = self.view.get_data(0)
+                data = np.fft.ifft(np.fft.fftshift(data)) * len(data)
+                util_fileio.dump_iterable(filename, data)
+        elif event_id == util_menu.ViewIdsSpectral.PLOTA_FID_TO_ASCII:
+            filename = common_dialogs.save_as("Plot A FID to ASCII", "TXT files (*.txt)|*.txt", default_filename='analysis_plota_fid_to_text.txt')
+            if filename:
+                data = self.view.get_data(0)
+                data = np.fft.ifft(np.fft.fftshift(data)) * len(data)
+                data.tofile(filename, sep=' ')
+        elif event_id == util_menu.ViewIdsSpectral.PLOTA_SPECTRUM_TO_BINARY:
+            filename = common_dialogs.save_as("Plot A Spectrum to Binary", "BIN files (*.bin)|*.bin", default_filename='analysis_plota_spectrum_to_binary.bin')
+            if filename:
+                data = self.view.get_data(0)
+                util_fileio.dump_iterable(filename, data)
+        elif event_id == util_menu.ViewIdsSpectral.PLOTA_SPECTRUM_TO_ASCII:
+            filename = common_dialogs.save_as("Plot A Spectrum to ASCII", "TXT files (*.txt)|*.txt", default_filename='analysis_plota_spectrum_to_text.txt')
+            if filename:
+                data = self.view.get_data(0)
+                data.tofile(filename, sep=' ')
+        elif event_id == util_menu.ViewIdsSpectral.PLOTA_FID_TO_VIFF:
+            self.dump_to_viff('plota_fid')
+
+        if event_id == util_menu.ViewIdsSpectral.PLOTC_FID_TO_BINARY:
+            filename = common_dialogs.save_as("Plot C FID to Binary", "BIN files (*.bin)|*.bin", default_filename='analysis_plotc_fid_to_binary.bin')
+            if filename:
+                data = self.view.get_data(2)
+                data = np.fft.ifft(np.fft.fftshift(data)) * len(data)
+                util_fileio.dump_iterable(filename, data)
+        elif event_id == util_menu.ViewIdsSpectral.PLOTC_FID_TO_ASCII:
+            filename = common_dialogs.save_as("Plot C FID to ASCII", "TXT files (*.txt)|*.txt", default_filename='analysis_plotc_fid_to_text.txt')
+            if filename:
+                data = self.view.get_data(2)
+                data = np.fft.ifft(np.fft.fftshift(data)) * len(data)
+                data.tofile(filename, sep=' ')
+        elif event_id == util_menu.ViewIdsSpectral.PLOTC_SPECTRUM_TO_BINARY:
+            filename = common_dialogs.save_as("Plot C Spectrum to Binary", "BIN files (*.bin)|*.bin", default_filename='analysis_plotc_spectrum_to_binary.bin')
+            if filename:
+                data = self.view.get_data(2)
+                util_fileio.dump_iterable(filename, data)
+        elif event_id == util_menu.ViewIdsSpectral.PLOTC_SPECTRUM_TO_ASCII:
+            filename = common_dialogs.save_as("Plot C Spectrum to ASCII", "TXT files (*.txt)|*.txt", default_filename='analysis_plotc_spectrum_to_text.txt')
+            if filename:
+                data = self.view.get_data(2)
+                data.tofile(filename, sep=' ')
+        elif event_id == util_menu.ViewIdsSpectral.PLOTC_FID_TO_VIFF:
+            self.dump_to_viff('plotc_fid')
+
+        elif event_id == util_menu.ViewIdsSpectral.SVDA_SPECTRUM_TO_VIFF:
+            self.dump_to_viff('svda_spectrum')
+        elif event_id == util_menu.ViewIdsSpectral.SVDB_SPECTRUM_CHECKED_SUM_TO_VIFF:
+            self.dump_to_viff('svdb_spectrum_checked_sum')
+        elif event_id == util_menu.ViewIdsSpectral.SVDB_FIDS_CHECKED_SUM_TO_VIFF:
+            self.dump_to_viff('svdb_fids_checked_sum')
+        elif event_id == util_menu.ViewIdsSpectral.SVDC_SPECTRUM_TO_VIFF:
+            self.dump_to_viff('svdc_spectrum')
+        elif event_id == util_menu.ViewIdsSpectral.PLOTC_A_PLUS_B_TO_NEW_TAB:
+            if self.datasetB is None:
+                msg = 'Warning (Derived Dataset PlotC): Please select Dataset for Plot B'
+                r = common_dialogs.message(msg, style=common_dialogs.I_OK)
+                return
+            derived_dataset(self.dataset, self.datasetB, self.view, self._tab_dataset, self.top, 'plotc_a_plus_b')
+        elif event_id == util_menu.ViewIdsSpectral.PLOTC_A_MINUS_B_TO_NEW_TAB:
+            if self.datasetB is None:
+                msg = 'Warning (Derived Dataset PlotC): Please select Dataset for Plot B'
+                r = common_dialogs.message(msg, style=common_dialogs.I_OK)
+                return
+            derived_dataset(self.dataset, self.datasetB, self.view, self._tab_dataset, self.top, 'plotc_a_minus_b')
+
+
 
     def on_menu_view_output(self, event):
         event_id = event.GetId()
         
-        if event_id == util_menu.ViewIdsSpectral.SVD_DATA_TO_VIFF:
-            self.dump_to_viff('svd_data')
-        elif event_id == util_menu.ViewIdsSpectral.SVD_PEAKS_CHECKED_SUM_TO_VIFF:
-            self.dump_to_viff('svd_peaks_checked_sum')
-        elif event_id == util_menu.ViewIdsSpectral.SVD_FIDS_CHECKED_SUM_TO_VIFF:
-            self.dump_to_viff('svd_fids_checked_sum')
-        elif event_id == util_menu.ViewIdsSpectral.SVD_PEAKS_CHECKED_DIFF_TO_VIFF:
-            self.dump_to_viff('svd_peak_checked_diff')
-        elif event_id == util_menu.ViewIdsSpectral.SVD_TABLE_VALUES_TO_XML:
+        formats = { util_menu.ViewIdsSpectral.VIEW_TO_PNG : "PNG",
+                    util_menu.ViewIdsSpectral.VIEW_TO_SVG : "SVG",
+                    util_menu.ViewIdsSpectral.VIEW_TO_EPS : "EPS",
+                    util_menu.ViewIdsSpectral.VIEW_TO_PDF : "PDF",
+                  }
+
+        if event_id in formats:
+            format = formats[event_id]
+            lformat = format.lower()
+            filter_ = "%s files (*.%s)|*.%s" % (format, lformat, lformat)
+
+            if self.svd_tab_active:
+                figure = self.view_svd.figure
+            else:
+                figure = self.view.figure
+
+            filename = common_dialogs.save_as("", filter_)
+
+            if filename:
+                msg = ""
+                try:
+                    figure.savefig( filename,
+                                    dpi=300,
+                                    facecolor='w',
+                                    edgecolor='w',
+                                    orientation='portrait',
+                                    papertype='letter',
+                                    format=None,
+                                    transparent=False)
+                except IOError:
+                    msg = """I can't write the file "%s".""" % filename
+
+                if msg:
+                    common_dialogs.message(msg, style=common_dialogs.E_OK)
+
+        elif event_id == util_menu.ViewIdsSpectral.SVD_TABLE_VALUES_TO_VIFF:
             self.export_hlsvd_table_to_xml()
         elif event_id == util_menu.ViewIdsSpectral.SVD_TABLE_VALUES_TO_CSV:
             self.export_hlsvd_table_to_csv()
-        else:
-            formats = { util_menu.ViewIdsSpectral.VIEW_TO_PNG : "PNG",
-                        util_menu.ViewIdsSpectral.VIEW_TO_SVG : "SVG",
-                        util_menu.ViewIdsSpectral.VIEW_TO_EPS : "EPS",
-                        util_menu.ViewIdsSpectral.VIEW_TO_PDF : "PDF",
-                      }
-    
-            if event_id in formats:
-                format = formats[event_id]
-                lformat = format.lower()
-                filter_ = "%s files (*.%s)|*.%s" % (format, lformat, lformat)
-    
-                if self.svd_tab_active:
-                    figure = self.view_svd.figure
-                else:
-                    figure = self.view.figure
-    
-                filename = common_dialogs.save_as("", filter_)
-    
-                if filename:
-                    msg = ""
-                    try:
-                        figure.savefig( filename,
-                                        dpi=300,
-                                        facecolor='w',
-                                        edgecolor='w',
-                                        orientation='portrait',
-                                        papertype='letter',
-                                        format=None,
-                                        transparent=False)
-                    except IOError:
-                        msg = """I can't write the file "%s".""" % filename
-    
-                    if msg:
-                        common_dialogs.message(msg, style=common_dialogs.E_OK)
-    
-            elif event_id == util_menu.ViewIdsSpectral.PLOTS_TO_BINARY:
-                filename = common_dialogs.save_as("", "BIN files (*.bin)|*.bin")
-                if filename:
-                    dataA = self.view.get_data(0)
-                    util_fileio.dump_iterable(filename, dataA)
-    
-            elif event_id == util_menu.ViewIdsSpectral.PLOTS_TO_ASCII:
-                filename = common_dialogs.save_as("", "TXT files (*.txt)|*.txt")
-                if filename:
-                    dataA = self.view.get_data(0)
-                    dataA.tofile(filename, sep=' ')
+
 
 
     def on_dataset_keys_change(self, keys):
         """ Pubsub notifications handler. """
         # The list of available datasets has changed so we update the
         # list of datasets available for plot B. We make note of the
         # currently selected item so we can re-select it if it's
@@ -1002,14 +1178,16 @@
             - data from Plot C, difference between Plot A - Plot B
             - inherently processed similar to the data in Plot A for equivalence
             - has b0 shift, apod, zf, fft, flip, dc, ampl, NO: ph0/ph1
         'svd_fids_checked_sum'
             - Calculated HLSVD FIDs
             - b0 shift is applied to these FIDs before they are output
             - NO apod, zf, fft, flip, ph0/ph1, dc, ampl applied
+        'plotc_fid'
+            - Derived spectrum, but without FFT or ph0/1 or chop, or flip
 
         """
 
         msg   = ''
         voxel = self._tab_dataset.voxel
         ds    = self.dataset
         if ds:
@@ -1018,54 +1196,84 @@
             defname  = "analysis_export_hlsvd_data.xml"
             label    = "Save HLSVDPro Data to VIFF XML Raw Filename"
             filename = common_dialogs.save_as(label, "XML files (*.xml)|*.xml", default_filename=defname)
             if filename:
 
                 stamp = util_time.now(util_time.ISO_TIMESTAMP_FORMAT).split('T')
             
-                if key == 'svd_data':
+                if key == 'svda_spectrum':
                     lines = ['Export from Analysis Spectral SVD Tab - PlotA Spectrum Data']
                     lines.append('------------------------------------------------------------------')
                     lines.append('An IFFT() was performed on the Plot A spectrum and the resultant FID written into')
                     lines.append('this VIFF XML Raw Data file.')
-                elif key == 'svd_peaks_checked_sum':
+                elif key == 'svdb_spectrum_checked_sum':
                     lines = ['Export from Analysis SVD Spectral Tab - PlotB Checked SVD Summed Spectrum']
                     lines.append('------------------------------------------------------------------')
                     lines.append('An IFFT() was performed on the summed SVD peak spectrum and the resultant FID written')
                     lines.append('into this VIFF XML Raw Data file.')
-                elif key == 'svd_fids_checked_sum':
+                elif key == 'svdb_fids_checked_sum':
                     lines = ['Export from Analysis Spectral SVD Tab - PlotB Checked SVD Summed FID Data']
                     lines.append('------------------------------------------------------------------')
                     lines.append('The time data for the summed SVD FIDs was written into this VIFF XML Raw Data file.')
                     lines.append('You can process it the same way your would any other time domain FID data.')
-                elif key == 'svd_peak_checked_diff':
+                elif key == 'svdc_spectrum':
                     lines = ['Export from Analysis Spectral SVD Tab - PlotC (PlotA - PlotB) Spectrum Data']
                     lines.append('------------------------------------------------------------------')
                     lines.append('An IFFT() was performed on the Plot C spectrum and the resultant FID written into')
                     lines.append('this VIFF XML Raw Data file.')
 
+                elif key == 'plota_fid':
+                    lines = ['Export from Analysis Spectral General Tab - PlotA FID Data']
+                    lines.append('------------------------------------------------------------------')
+                    lines.append('An IFFT() was performed on the Plot A spectrum and the resultant FID written into')
+                    lines.append('this VIFF XML Raw Data file.')
+
+                elif key == 'plotc_fid':
+                    if self.plot_C_function == self.plot_C_map[util_menu.ViewIdsSpectral.PLOT_C_FUNCTION_NONE]:
+                        labl_func = 'None'
+                    elif self.plot_C_function == self.plot_C_map[util_menu.ViewIdsSpectral.PLOT_C_FUNCTION_A_MINUS_B]:
+                        labl_func = 'PlotA - PlotB'
+                    elif self.plot_C_function == self.plot_C_map[util_menu.ViewIdsSpectral.PLOT_C_FUNCTION_B_MINUS_A]:
+                        labl_func = 'PlotB - PlotA'
+                    elif self.plot_C_function == self.plot_C_map[util_menu.ViewIdsSpectral.PLOT_C_FUNCTION_A_PLUS_B]:
+                        labl_func = 'PlotA + PlotB'
+
+                    lines = ['Export from Analysis Spectral General Tab - PlotC ('+labl_func+') FID Data']
+                    lines.append('------------------------------------------------------------------')
+                    lines.append('An IFFT() was performed on the Plot C spectrum and the resultant FID written into')
+                    lines.append('this VIFF XML Raw Data file.')
+
                 lines.append(' ')
                 lines.append('Creation_date            - '+stamp[0])
                 lines.append('Creation_time            - '+stamp[1])
                 lines.append(' ')
                 lines = "\n".join(lines)
                 if (sys.platform == "win32"):
                     lines = lines.replace("\n", "\r\n")
 
-                if key == 'svd_data' or key == 'svd_peaks_checked_sum':
-                    dat = results[key].copy()
+                if key == 'svda_spectrum':
+                    dat = results['svd_data'].copy()
                     dat = np.fft.ifft(np.fft.fftshift(dat)) * len(dat)
-                elif key =='svd_peak_checked_diff':
-                    dat = results['svd_data'].copy() - results['svd_peaks_checked_sum'].copy()
+                elif key == 'svdb_spectrum_checked_sum':
+                    dat = results['svd_peaks_checked_sum'].copy()
                     dat = np.fft.ifft(np.fft.fftshift(dat)) * len(dat)
-                elif key == 'svd_fids_checked_sum':
+                elif key == 'svdb_fids_checked_sum':
                     dat = results[key].copy()
+                elif key =='svd_spectrum_checked_diff':
+                    dat = results['svd_data'].copy() - results['svd_peaks_checked_sum'].copy()
+                    dat = np.fft.ifft(np.fft.fftshift(dat)) * len(dat)
+                elif key == 'plota_fid':
+                    dat = self.view.get_data(0)
+                    dat = np.fft.ifft(np.fft.fftshift(dat)) * len(dat)
+                elif key == 'plotc_fid':
+                    dat = self.view.get_data(2)
+                    dat = np.fft.ifft(np.fft.fftshift(dat)) * len(dat)
 
                 met = mrs_data_raw.DataRaw()
-                met.data_sources = ['analysis_spetral_svd_tab_data_export']
+                met.data_sources = ['analysis_spectral_general_tab_plotc_data_export']
                 met.headers      = [lines]
                 met.sw           = ds.sw
                 met.frequency    = ds.frequency
                 met.resppm       = ds.resppm
                 met.data         = dat
                 try:
                     util_export.export(filename, [met], None, lines, False)
@@ -2042,14 +2250,18 @@
 
     def set_plot_c(self):
         data1 = self.view.all_axes[0].lines[0].get_ydata()
         data2 = self.view.all_axes[1].lines[0].get_ydata()
         data3 = self.plot_C_function(data1, data2)
         self.view.all_axes[2].lines[0].set_ydata(data3)
 
+        view_data1 = self.view.get_data(0)
+        view_data2 = self.view.get_data(1)
+        view_data3 = self.plot_C_function(view_data1, view_data2)
+        self.view.set_data_direct(view_data3, 2)
 
     def svd_checklist_update(self):
         """
         This method totally rebuilds the result set in the checklist widget.
 
         Take the hlsvd results for the current voxel and set them into the
         checklist widget. If the spectral tab hlsvd water filter is on and
```

## vespa/analysis/util_file_import.py

```diff
@@ -187,14 +187,45 @@
     'ini_file_name=import_vasf',
 '[import_vasf_fidsum]',
     'path=vespa.analysis.fileio.vasf',
     'class_name=RawReaderVasfFidsum',
     'menu_item_text=VASF Sum FIDs (*.rsd/rsp)',
     'ini_file_name=import_vasf_fidsum',
 '[separator101]',
+# '[import_siemens_dicom_cmrr_mpress]',
+#     'path=vespa.analysis.fileio.dicom_siemens_cmrr_mpress',
+#     'class_name=RawReaderDicomSiemensXaMpress',
+#     'menu_item_text=SiemensXA DICOM CMRR MPress',
+#     'ini_file_name=import_siemens_dicom_cmrr_mpress',
+# '[import_siemens_dicom_cmrr_mpress_fidsum]',
+#     'path=vespa.analysis.fileio.dicom_siemens_cmrr_mpress',
+#     'class_name=RawReaderDicomSiemensFidsumXaMpress',
+#     'menu_item_text=SiemensXA DICOM CMRR MPress Fidsum',
+#     'ini_file_name=import_siemens_dicom_cmrr_mpress_fidsum',
+'[import_siemens_dicom_eja_svs_mpress]',
+    'path=vespa.analysis.fileio.dicom_siemens_eja_svs_mpress',
+    'class_name=RawReaderDicomSiemensXaEjaSvsMpress',
+    'menu_item_text=SiemensXA DICOM eja_svs_mpress',
+    'ini_file_name=import_siemens_dicom_eja_svs_mpress',
+'[import_siemens_dicom_eja_svs_mpress_onoff]',
+    'path=vespa.analysis.fileio.dicom_siemens_eja_svs_mpress',
+    'class_name=RawReaderDicomSiemensXaEjaSvsMpressOnOff',
+    'menu_item_text=SiemensXA DICOM eja_svs_mpress - On/Off only',
+    'ini_file_name=import_siemens_dicom_eja_svs_mpress_onoff',
+'[import_siemens_dicom_eja_svs_mpress_fidsum]',
+    'path=vespa.analysis.fileio.dicom_siemens_eja_svs_mpress',
+    'class_name=RawReaderDicomSiemensFidsumXaEjaSvsMpress',
+    'menu_item_text=SiemensXA DICOM eja_svs_mpress Fidsum',
+    'ini_file_name=import_siemens_dicom_eja_svs_mpress_fidsum',
+'[import_siemens_dicom_eja_svs_mpress_fidsum_onoff]',
+    'path=vespa.analysis.fileio.dicom_siemens_eja_svs_mpress',
+    'class_name=RawReaderDicomSiemensFidsumXaEjaSvsMpressOnOff',
+    'menu_item_text=SiemensXA DICOM eja_svs_mpress Fidsum - On/Off only',
+    'ini_file_name=import_siemens_dicom_eja_svs_mpress_fidsum_onoff',
+'[separator102]',
 ]
 
 
 def set_import_data_classes(filename=''):
     """
     This module creates a configObj with all available data parsers
     - There are standard data classes we guarantee are provided
@@ -309,14 +340,16 @@
             d = { }
 
             raw_class = type(raw).__name__
 
             # these associate multiple files in the Raw block (e.g. On/Off/Sum/Dif for edited data)
             if raw_class == 'DataRawProbep':
                 d["raw"] = getattr(importlib.import_module('vespa.analysis.block_raw_probep'), 'BlockRawProbep')
+            elif raw_class == 'DataRawEdit':
+                d["raw"] = getattr(importlib.import_module('vespa.analysis.block_raw_edit'), 'BlockRawEdit')
             elif raw_class == 'DataRawEditFidsum':
                 d["raw"] = getattr(importlib.import_module('vespa.analysis.block_raw_edit_fidsum'), 'BlockRawEditFidsum')
             elif raw_class == 'DataRawCmrrSlaser':
                 d["raw"] = getattr(importlib.import_module('vespa.analysis.block_raw_cmrr_slaser'), 'BlockRawCmrrSlaser')
 
             # these require a Preprocess tab to be included in the workflow
             if isinstance(raw, DataRawFidsum):
@@ -340,16 +373,24 @@
 
             # GE PROBE-P - returns both water and metabolite data
             if type(dataset.blocks['raw']).__name__ == 'BlockRawProbep':
                 if len(datasets) > 1:
                     dataset.blocks['raw'].set_associated_datasets([datasets[0], datasets[1]])
 
             # Edited SVS Object - four datasets, acquisition ON/OFF and calculated SUM/DIFF.
-            if type(raws[0]).__name__ == 'DataRawEditFidsum':
-                dataset.blocks['raw'].set_associated_datasets([datasets[0], datasets[1], datasets[2], datasets[3]])
+            if len(datasets) == 4:
+                if type(raws[0]).__name__ == 'DataRawEditFidsum':
+                    dataset.blocks['raw'].set_associated_datasets([datasets[0], datasets[1], datasets[2], datasets[3]])
+                if type(raws[0]).__name__ == 'DataRawEdit':
+                    dataset.blocks['raw'].set_associated_datasets([datasets[0], datasets[1], datasets[2], datasets[3]])
+            elif len(datasets) == 2:
+                if type(raws[0]).__name__ == 'DataRawEditFidsum':
+                    dataset.blocks['raw'].set_associated_datasets([datasets[0], datasets[1]])
+                if type(raws[0]).__name__ == 'DataRawEdit':
+                    dataset.blocks['raw'].set_associated_datasets([datasets[0], datasets[1]])
 
             # CMRR sLASER - 3 or 6 datasets:
             #   coil 1 FID, ecc1 2 FIDs, water1 2 FIDs,  metab64 64 FIDs, ecc2 2 FIDs (opt) and water2 2 FIDs (opt)
             if type(raws[0]).__name__ == 'DataRawCmrrSlaser':
                 if len(datasets) == 6:
                     dataset.blocks['raw'].set_associated_datasets([datasets[0], datasets[1], datasets[2], datasets[3], datasets[4], datasets[5]])
                 elif len(datasets) == 3:
```

## vespa/analysis/util_menu.py

```diff
@@ -84,24 +84,35 @@
     USER_BUTTON_PHASING = "replace me"
     USER_BUTTON_AREA = "replace me"
 
     VIEW_TO_PNG  = "replace me"
     VIEW_TO_SVG  = "replace me"
     VIEW_TO_PDF  = "replace me"
     VIEW_TO_EPS  = "replace me"
-    
-    SVD_DATA_TO_VIFF = "replace me"
-    SVD_PEAKS_CHECKED_SUM_TO_VIFF = "replace me"
-    SVD_FIDS_CHECKED_SUM_TO_VIFF = "replace me"
-    SVD_PEAKS_CHECKED_DIFF_TO_VIFF = "replace me"
-    SVD_TABLE_VALUES_TO_XML = "replace me"
-    SVD_TABLE_VALUES_TO_CSV = "replace me"
 
-    PLOTS_TO_BINARY = "replace me"
-    PLOTS_TO_ASCII = "replace me"
+    PLOTA_FID_TO_BINARY = "replace me"
+    PLOTA_FID_TO_ASCII = "replace me"
+    PLOTA_SPECTRUM_TO_BINARY = "replace me"
+    PLOTA_SPECTRUM_TO_ASCII = "replace me"
+    PLOTA_FID_TO_VIFF = "replace me"
+
+    PLOTC_FID_TO_BINARY = "replace me"
+    PLOTC_FID_TO_ASCII = "replace me"
+    PLOTC_SPECTRUM_TO_BINARY = "replace me"
+    PLOTC_SPECTRUM_TO_ASCII = "replace me"
+    PLOTC_FID_TO_VIFF  = "replace me"
+    PLOTC_A_PLUS_B_TO_NEW_TAB = "replace me"
+    PLOTC_A_MINUS_B_TO_NEW_TAB = "replace me"
+
+    SVDA_SPECTRUM_TO_VIFF = "replace me"
+    SVDB_SPECTRUM_CHECKED_SUM_TO_VIFF = "replace me"
+    SVDB_FIDS_CHECKED_SUM_TO_VIFF = "replace me"
+    SVDC_SPECTRUM_TO_VIFF = "replace me"
+    SVD_TABLE_VALUES_TO_VIFF = "replace me"
+    SVD_TABLE_VALUES_TO_CSV = "replace me"
 
 
 class ViewIdsPrepTimeseries(common_menu.IdContainer):
     """
     A container for the ids of all of the menu items to which we need
     explicit references.
     """
@@ -676,64 +687,89 @@
         
     view_spectral = (
             ("Zero Line", (
                 ("Show",   main.on_menu_view_option, wx.ITEM_CHECK, ViewIdsSpectral.ZERO_LINE_SHOW),
                 common_menu.SEPARATOR,
                 ("Top",    main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.ZERO_LINE_TOP),
                 ("Middle", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.ZERO_LINE_MIDDLE),
-                ("Bottom", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.ZERO_LINE_BOTTOM))),
+                ("Bottom", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.ZERO_LINE_BOTTOM),
+            )),
             ("X-Axis", (
                 ("Show", main.on_menu_view_option,   wx.ITEM_CHECK, ViewIdsSpectral.XAXIS_SHOW),
                 common_menu.SEPARATOR,
                 ("PPM",   main.on_menu_view_option,  wx.ITEM_RADIO, ViewIdsSpectral.XAXIS_PPM),
-                ("Hertz", main.on_menu_view_option,  wx.ITEM_RADIO, ViewIdsSpectral.XAXIS_HERTZ))),
+                ("Hertz", main.on_menu_view_option,  wx.ITEM_RADIO, ViewIdsSpectral.XAXIS_HERTZ),
+            )),
             common_menu.SEPARATOR,
             ("Data Type", (
                 ("Real",      main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.DATA_TYPE_REAL),
                 ("Imaginary", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.DATA_TYPE_IMAGINARY),
                 ("Magnitude", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.DATA_TYPE_MAGNITUDE),
                 common_menu.SEPARATOR,
                 ("Summed",    main.on_menu_view_option, wx.ITEM_CHECK, ViewIdsSpectral.DATA_TYPE_SUMMED),
-                          )
-            ),
+            )),
             common_menu.SEPARATOR,
             ("Area Calculation", (
                 ("From Plot A", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.AREA_CALC_PLOT_A),
                 ("From Plot B", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.AREA_CALC_PLOT_B),
-                ("From Plot C", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.AREA_CALC_PLOT_C))),
+                ("From Plot C", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.AREA_CALC_PLOT_C),
+            )),
             ("Plot C Function", (
                 ("None",         main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.PLOT_C_FUNCTION_NONE),
                 ("Residual A-B", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.PLOT_C_FUNCTION_A_MINUS_B),
                 ("Residual B-A", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.PLOT_C_FUNCTION_B_MINUS_A),
-                ("Sum A+B",      main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.PLOT_C_FUNCTION_A_PLUS_B))),
+                ("Sum A+B",      main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.PLOT_C_FUNCTION_A_PLUS_B),
+            )),
             ("User Button Function", (
                 ("Automatic Phasing", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.USER_BUTTON_PHASING),
-                ("Output Area Value", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.USER_BUTTON_AREA))),
+                ("Output Area Value", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsSpectral.USER_BUTTON_AREA),
+            )),
+            common_menu.SEPARATOR,
+            ("Derived Datasets", (
+                ("Plot A", (
+                    ("FID -> Binary", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTA_FID_TO_BINARY),
+                    ("FID -> ASCII",  main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTA_FID_TO_ASCII),
+                    ("Spectrum -> Binary", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTA_SPECTRUM_TO_BINARY),
+                    ("Spectrum -> ASCII",  main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTA_SPECTRUM_TO_ASCII),
+                    ("FID -> VIFF Raw Data", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTA_FID_TO_VIFF),
+                )),
+                common_menu.SEPARATOR,
+                ("Plot C", (
+                    ("FID -> Binary", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTC_FID_TO_BINARY),
+                    ("FID -> ASCII",  main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTC_FID_TO_ASCII),
+                    ("Spectrum -> Binary", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTC_SPECTRUM_TO_BINARY),
+                    ("Spectrum -> ASCII",  main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTC_SPECTRUM_TO_ASCII),
+                    ("FID -> VIFF Raw Data", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTC_FID_TO_VIFF),
+                    ("Spectrum A+B -> New Tab", main.on_menu_view_derived, wx.ITEM_NORMAL,ViewIdsSpectral.PLOTC_A_PLUS_B_TO_NEW_TAB),
+                    ("Spectrum A-B -> New Tab", main.on_menu_view_derived, wx.ITEM_NORMAL,ViewIdsSpectral.PLOTC_A_MINUS_B_TO_NEW_TAB),
+                )),
+                common_menu.SEPARATOR,
+                ("SVD Exports", (
+                    ("Plot A Spectrum -> VIFF Raw Data", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.SVDA_SPECTRUM_TO_VIFF),
+                    ("Plot B Spectrum Sum -> VIFF Raw Data",  main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.SVDB_SPECTRUM_CHECKED_SUM_TO_VIFF),
+                    ("Plot B FID Data Sum -> VIFF Raw Data", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.SVDB_FIDS_CHECKED_SUM_TO_VIFF),
+                    ("Plot C Spectrum Diff -> VIFF Raw Data", main.on_menu_view_derived, wx.ITEM_NORMAL, ViewIdsSpectral.SVDC_SPECTRUM_TO_VIFF),
+                )),
+            )),
             common_menu.SEPARATOR,
             ("Output", (
                 ("View -> PNG", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.VIEW_TO_PNG),
                 ("View -> SVG", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.VIEW_TO_SVG),
                 ("View -> PDF", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.VIEW_TO_PDF),
                 ("View -> EPS", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.VIEW_TO_EPS),
-                common_menu.SEPARATOR,
-                ("Plot A", (
-                    ("to Binary", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTS_TO_BINARY),
-                    ("to ASCII",  main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.PLOTS_TO_ASCII))),
+                ("View -> EPS", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.VIEW_TO_EPS),
+
                 common_menu.SEPARATOR,
                 ("SVD Exports", (
-                    ("Plot A Spectrum -> VIFF Raw Data", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.SVD_DATA_TO_VIFF),
-                    ("Plot B Spectrum Sum -> VIFF Raw Data",  main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.SVD_PEAKS_CHECKED_SUM_TO_VIFF),
-                    ("Plot B FID Data Sum -> VIFF Raw Data", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.SVD_FIDS_CHECKED_SUM_TO_VIFF),
-                    ("Plot C Spectrum Diff -> VIFF Raw Data", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.SVD_PEAKS_CHECKED_DIFF_TO_VIFF),
-                    ("HLSVD Table Values -> VIFF XML", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.SVD_TABLE_VALUES_TO_XML),
+                    ("HLSVD Table Values -> VIFF XML", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.SVD_TABLE_VALUES_TO_VIFF),
                     ("HLSVD Table Values -> CSV File", main.on_menu_view_output, wx.ITEM_NORMAL, ViewIdsSpectral.SVD_TABLE_VALUES_TO_CSV),
-                                )
-                 ),
+                )),
             )))
 
+
     view_voigt = (
             ("Zero Line", (
                 ("Show",   main.on_menu_view_option, wx.ITEM_CHECK, ViewIdsVoigt.ZERO_LINE_SHOW),
                 common_menu.SEPARATOR,
                 ("Top",    main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsVoigt.ZERO_LINE_TOP),
                 ("Middle", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsVoigt.ZERO_LINE_MIDDLE),
                 ("Bottom", main.on_menu_view_option, wx.ITEM_RADIO, ViewIdsVoigt.ZERO_LINE_BOTTOM))),
@@ -873,16 +909,21 @@
                             )
             )
         )
         )
 
     help = [
 #            ("&User Manual",            main.on_user_manual),
-            ("&Analysis Online User Manual",   main.on_analysis_online_user_manual),
-            ("&Vespa Help Online",      main.on_vespa_help_online),
+            ("&Analysis Online User Manual",    main.on_analysis_online_user_manual),
+            ("&Vespa Help Online",              main.on_vespa_help_online),
+            common_menu.SEPARATOR,
+            ("Utilities", (
+                ("DICOM Series Sort and Rename", main.on_util_dicom_series_sort),
+            )),
+            common_menu.SEPARATOR,
             ("&About", main.on_about, wx.ITEM_NORMAL, wx.ID_ABOUT),
            ]
     
     if util_common_config.VespaConfig().show_wx_inspector:  
         help.append(common_menu.SEPARATOR)
         help.append( ("Show Inspection Tool", main.on_show_inspection_tool) )
```

## vespa/analysis/utils.py

```diff
@@ -1,18 +1,51 @@
 # Python modules
+import os
+import shutil
 
 # 3rd party modules
 import numpy as np
+import pydicom as dicom
+
 
 # Our modules
 import vespa.common.constants  as common_constants
 
-# Keep 'em in alphabetical order, please, unless you have a better idea.
+# List Classes then Methods ...
+# - keep 'em in alphabetical order, please, unless you have a better idea.
+
+class DicomFileItems(object):
 
+    def __init__(self, filename):
+        self.filename = filename
+        self.move_path = None
+        self.patient_id = None
+        self.patient_name = None
+        self.study_id = None
+        self.study_description = None
+        self.series_number = None
+        self.series_description = None
+        self.instance_number = None
+
+    def __lt__(self, other):
+        """
+        Python docs say that, "The sort routines are guaranteed to use
+        __lt__() when making comparisons between two objects. So, it is easy
+        to add a standard sort order to a class by defining an __lt__() method.
+
+        For DICOM series sort, we typically sort by the patient ID, then the
+        study id, then series number attributes.
+
+        """
+        original_reverse = [self.patient_id, self.study_id, self.series_number, self.instance_number]
+        other_reverse = [self.patient_id, self.study_id, self.series_number, self.instance_number]
+        original_reverse.reverse()
+        other_reverse.reverse()
 
+        return original_reverse < other_reverse
 
 
 # def calculate_area(dimension_size, frequencies, phases, x_left, x_right):
 #     """
 #     Calculates & returns the selected area.
 #
 #     The param dimension_size is a scalar like data.dims[0].
@@ -32,15 +65,108 @@
 #         area = sum(pdata[x_left:x_right + 1])
 #     else:
 #         area = sum(pdata[x_right:x_left + 1])
 #
 #     return area
 
 
+def dicom_series_sort(base_path):
 
+    # Enumerate the directory contents
+    filenames = []
+    for root, dirs, fnames in os.walk(base_path):
+        for fname in fnames:
+            # Add path to filenames
+            filenames.append(os.path.join(root, fname))
+
+    # Filter out non-files
+    filenames = [filename for filename in filenames if os.path.isfile(filename)]
+
+    headers = []
+    move_paths = []
+
+    # assume that files MAY be in one dir, or in sub-dirs under the
+    # base_path that is searched (and passed in here).
+
+    for filename in filenames:
+        # go through all filenames and ensure each file is DICOM
+        if is_dicom(filename):
+
+            # create storage container for data and refresh control flags
+            hdr = DicomFileItems(filename)
+
+            data_raw = dicom.dcmread(filename, stop_before_pixels=True)
+
+            hdr.patient_id = data_raw.PatientID
+            hdr.study_id = data_raw.StudyID
+            hdr.series_number = data_raw.SeriesNumber
+            hdr.series_description = data_raw.SeriesDescription
+            hdr.instance_number = data_raw.InstanceNumber
+            hdr.study_description = data_raw.StudyDescription
+            hdr.patient_name = str(data_raw.PatientName)
+
+            if hdr.series_number < 10:
+                ser_str = '000' + str(hdr.series_number)
+            elif hdr.series_number < 100:
+                ser_str = '00' + str(hdr.series_number)
+            elif hdr.series_number < 1000:
+                ser_str = '0' + str(hdr.series_number)
+            else:
+                ser_str = str(hdr.series_number)
+
+            # concatenate the destination sub-directory name
+            move_path = ser_str + '_'
+            move_path += str(hdr.series_description).upper()
+            # move_path += str(hdr.patient_id)+'_'
+            # move_path += str(hdr.study_id)+'_'
+            move_path = move_path.replace(" ", "_")
+
+            # creae a list of unique sub-directory names
+            if move_path not in move_paths:
+                move_paths.append(move_path)
+
+            hdr.move_path = move_path
+
+            headers.append(hdr)
+
+    # create all "move directories"
+    #
+    # Note. according to Python docs, the mkdir command
+    #   only works for Windows and *nix, no Mac support
+    for fdir in move_paths:
+        new_path = base_path + '/' + fdir
+        if not os.path.exists(new_path):
+            os.mkdir(new_path)
+            #print('New path - '+new_path)
+
+    # move all files to new sub-directories
+    #
+    # used shutil here to be pure Python and not have to
+    # worry about OS specific command names.
+    for hdr in headers:
+        src = hdr.filename
+        path, fname = os.path.split(src)
+        dst = os.path.join(base_path, hdr.move_path, fname)
+        shutil.move(src, dst)
+        #print('Dst file - '+dst)
+
+
+def is_dicom(filename):
+    """Returns True if the file in question is a DICOM file, else False. """
+    # Per the DICOM specs, a DICOM file starts with 128 reserved bytes
+    # followed by "DICM".
+    # ref: DICOM spec, Part 10: Media Storage and File Format for Media
+    # Interchange, 7.1 DICOM FILE META INFORMATION
+    if os.path.isfile(filename):
+        f = open(filename, "rb")
+        s = f.read(132)
+        f.close()
+        return s.endswith(b"DICM")
+    else:
+        return False
```

## vespa/analysis/fileio/dicom_browser_dialog.py

```diff
@@ -594,28 +594,29 @@
         See also get_all_files().
 
         """
         # get directory contents, fully-qualified filenames, remove non-files
         filenames = os.listdir(path)
         filenames = [os.path.join(path, filename) for filename in filenames]
         filenames = [filename for filename in filenames if os.path.isfile(filename)]
+        filenames = [filename for filename in filenames if self.is_dicom(filename)]
 
         for filename in filenames:
-            if self.is_dicom(filename):
-                dataset = pydicom.read_file(filename)
-                dataset.decode()  # change strings to unicode
-
-                if ("Manufacturer" in dataset) and \
-                   ("SIEMENS" in dataset.Manufacturer.upper()):
-                    df = DicomFileSiemens(dataset, filename)
-                else:
-                    df = DicomFileInfo(dataset, filename)
-                yield df
-            # else:
-                # Not a DICOM file; ignore it.
+            dataset = pydicom.dcmread(filename, stop_before_pixels=True)
+
+            # bjs - oct 2022, this was slowing Tree create down by 10-50x
+            #  not sure if needed just for the limited data required for Tree.
+            #
+            # dataset.decode()  # change strings to unicode
+
+            if ("Manufacturer" in dataset) and ("SIEMENS" in dataset.Manufacturer.upper()):
+                df = DicomFileSiemens(dataset, filename)
+            else:
+                df = DicomFileInfo(dataset, filename)
+            yield df
 
 
     #--------------------------------------------------------------------------
     # Internal methods
 
     def _suggest_a_start_path(self):
         """Returns a path for the user to begin browsing for DICOM files."""
@@ -1114,27 +1115,27 @@
         """
         dataset = dicom_file.dataset
         test = False
         if self.manufacturer:
             if 'Manufacturer' in dataset:
                 for item in self.manufacturer:
                     # we only handle manufacturers in this list
-                    if dataset.Manufacturer.upper() in item:
+                    if item in dataset.Manufacturer.upper() :
                         test = True
             if not test:
                 return False
 
         if self.TAG_SOP_CLASS_UID in dataset:
             item_uid = dataset[self.TAG_SOP_CLASS_UID].value.upper()
             sop_class_uid = pydicom.uid.UID(str(item_uid))
             if sop_class_uid.name == 'MR Image Storage':
                 # this is the condition for Spectroscopy Browser
                 return False
             elif sop_class_uid.name == 'MR Spectroscopy Storage':
-                # this is the UID value for Siemens VD files
+                # this is the UID value for Siemens VD and XA files
                 return True
             elif sop_class_uid.name == str(item_uid):
                 # In software versions VA, VB (maybe others, but not VD), Siemens uses a proprietary
                 # SOP Class UID for their spectroscopy data files. I have seen 1.3.12.2.1107.5.9.1
                 # used but am not sure if it is unique. And this is not in the DICOM dictionary of UIDs
                 # So, we will look for other proprietary tags that will give us solid info that these are
                 # Siemens SPEC file.
@@ -1328,27 +1329,27 @@
         # dialog = DialogDicomBrowser(self,
         #                             preview_size=(96, 96),
         #                             show_tags=False,
         #                             multi_select=True,
         #                             return_objects=False,
         #                             default_path=default_path)
 
-        # dialog = SiemensSpectroscopyDicomBrowserDialog(self,
-        #                             preview_size=(96, 96),
-        #                             show_tags=False,
-        #                             multi_select=True,
-        #                             return_objects=False,
-        #                             default_path=default_path)
-
-        dialog = PhilipsSpectroscopyDicomBrowserDialog(self,
+        dialog = SiemensMrsBrowser(self,
                                     preview_size=(96, 96),
                                     show_tags=False,
                                     multi_select=True,
                                     return_objects=False,
                                     default_path=default_path)
+
+        # dialog = PhilipsMrsBrowser(self,
+        #                             preview_size=(96, 96),
+        #                             show_tags=False,
+        #                             multi_select=True,
+        #                             return_objects=False,
+        #                             default_path=default_path)
         dialog.ShowModal()
 
         if dialog.items:
             print("You selected %d item(s) --" % len(dialog.items))
             for item in dialog.items:
                 if hasattr(item, "filename"):
                     print('- ' + item.filename)
@@ -1359,20 +1360,33 @@
 
         print("\nbye!")
 
         self.Close()
 
 
 def _test():
-    default_path = ''
-    default_path = r'D:\Users\bsoher\code\repository_svn\sample_data\siemens_dicom_export'
+
+    # default_path = ''
+    # default_path = r'D:\Users\bsoher\code\repository_svn\sample_data\siemens_dicom_export'
+    default_path = r'D:\Users\bsoher\projects\2022_Neurona_GABA\data\2022_09_22_NTRT_003_01\dicom\DICOM\0044_EJA_MPRESS_HIPPO_METAB_2_RES'
 
     app = wx.App(0)
     wx.InitAllImageHandlers()
     frame_1 = TestFrame(default_path=default_path)
     app.SetTopWindow(frame_1)
     frame_1.Show()
     app.MainLoop()
 
 
 if __name__ == '__main__':
+
+    # import cProfile
+    # import pstats as ps
+    # fname = 'D:\\Users\\bsoher\\profile.data'
+    # if os.path.exists(fname):
+    #     os.remove(fname)
+    # cmd = '_test()'
+    # cProfile.run(cmd, fname)
+    # p = ps.Stats(fname)
+    # p.strip_dirs().sort_stats('cumulative').print_stats()
+
     _test()
```

## vespa/analysis/fileio/dicom_siemens.py

```diff
@@ -5,14 +5,16 @@
 pp = pprint.PrettyPrinter(depth=2)
 
 # 3rd party modules
 import pydicom
 import pydicom.dicomio
 import numpy as np
 
+from pydicom.values import convert_numbers
+
 # Our modules
 import vespa.analysis.fileio.raw_reader as raw_reader
 import vespa.common.util.config as util_config
 import vespa.common.util.misc as util_misc
 from vespa.common.base_transform import transformation_matrix
 from vespa.common.mrs_data_raw import DataRaw, DataRawFidsum
 from vespa.common.constants import Deflate
@@ -227,15 +229,16 @@
     # get shape of the data (slices, rows, columns, fid_points)
     section = dataset[0x5200,0x9229][0][0x0018,0x9103][0]
     data_shape = (section["SpectroscopyAcquisitionOutOfPlanePhaseSteps"].value,
                   section["SpectroscopyAcquisitionPhaseRows"].value,
                   section["SpectroscopyAcquisitionPhaseColumns"].value,
                   section["SpectroscopyAcquisitionDataColumns"].value, )
 
-    data_iter = iter(dataset['SpectroscopyData'].value)      # (0x5600, 0x0020)
+    dataf =  convert_numbers(dataset['SpectroscopyData'].value, True, 'f') # (0x5600, 0x0020)
+    data_iter = iter(dataf)
     data = [complex(r, i) for r, i in zip(data_iter, data_iter)]
     complex_data = np.fromiter(data, dtype=np.complex64)
     complex_data.shape = data_shape
     complex_data = complex_data.conjugate()
 
     try:
         iorient = dataset[0x5200,0x9229][0][0x0020,0x9116][0]['ImageOrientationPatient'].value
@@ -256,16 +259,16 @@
 
     params = {'is_dicom_sop': True,
               'sw'          : dataset["SpectralWidth"].value,
               'frequency'   : dataset["TransmitterFrequency"].value,
               'resppm'      : 4.7,
               'echopeak'    : 0.0,
               'nucleus'     : dataset["ResonantNucleus"].value,
-              'seqte'       : dataset[0x5200,0x9229][0][0x0018,0x9114][0]['EffectiveEchoTime'].value,
-              'seqtr'       : dataset[0x5200,0x9229][0][0x0018,0x9112][0]['RepetitionTime'].value,
+              'seqte'       : float(dataset[0x5200,0x9229][0][0x0018,0x9114][0]['EffectiveEchoTime'].value),
+              'seqtr'       : float(dataset[0x5200,0x9229][0][0x0018,0x9112][0]['RepetitionTime'].value),
               'voxel_dimensions' : voxel_size,
               'header'      : str(dataset),
               'transform'   : tform,
               'data'        : complex_data}
 
     return params
 
@@ -345,16 +348,16 @@
 
     params = {'is_dicom_sop': False,
               'sw'          : 1.0 / (csa_header["RealDwellTime"] * 1e-9),
               'frequency'   : csa_header["ImagingFrequency"],
               'resppm'      : 4.7,
               'echopeak'    : 0.0,
               'nucleus'     : '1H',
-              'seqte'       : csa_header["EchoTime"],
-              'seqtr'       : csa_header["RepetitionTime"],
+              'seqte'       : float(csa_header["EchoTime"]),
+              'seqtr'       : float(csa_header["RepetitionTime"]),
               'voxel_dimensions' : voxel_size,
               'header'      : header,
               'transform'   : tform,
               'data'        : complex_data}
 
     return params
```

## vespa/analysis/fileio/ge_pfile.py

```diff
@@ -171,23 +171,26 @@
 
     sw = float(hdr.rhr_rh_user0)  # in Hz
     freq = float(hdr.rhr_rh_ps_mps_freq) / 1e7  # in MHz
     te = float(hdr.rhi_te) / 1000  # in ms
     tr = float(hdr.rhi_tr) / 1000  # in ms
 
     #  Use the mps freq and field strength to determine gamma and thus isotope
-    gamma = (hdr.rhr_rh_ps_mps_freq * 1e-7) / (hdr.rhe_magstrength / 10000.0)
-    if abs(gamma - 42.57) < 0.3:
-        nucleus = "1H"
-    elif abs(gamma - 10.7) < 0.3:
-        nucleus = "13C"
-    elif abs(gamma - 17.2) < 0.3:
-        nucleus = "31P"
-    else:
-        nucleus = "1H"
+
+    # Note, some anonymization procedures clear the exam header, which invalidates magstrength; in this case, assume 1H
+    nucleus = "1H"
+
+    if (hdr.rhe_magstrength > 0):
+	    gamma = (hdr.rhr_rh_ps_mps_freq * 1e-7) / (hdr.rhe_magstrength / 10000.0)
+	    if abs(gamma - 42.57) < 0.3:
+	        nucleus = "1H"
+	    elif abs(gamma - 10.7) < 0.3:
+	        nucleus = "13C"
+	    elif abs(gamma - 17.2) < 0.3:
+	        nucleus = "31P"
     resppm = 4.7 if nucleus == "1H" else 0.0
 
     pulseq = hdr.rhi_psdname.decode('utf-8').lower()
 
     # calculate directional cosines to get row/col vectors ---------------------
     dcos = pfile.map.get_dcos
     dcos[dcos == 0.0] = 0.0             # remove -0.0 values
```

## vespa/analysis/fileio/raw_reader.py

```diff
@@ -183,35 +183,46 @@
             
             
     def _check_compatibility(self, raws, open_dataset, fidsum=False):
         """
         Attributes and object type of new object must match those of the open dataset(s)
 
         """
-        raw0 = self.raws[0]
-        raw1 = open_dataset.blocks["prep"]
 
-        new_is_fidsum = False
-        if isinstance(raw0, (DataRawFidsum, DataRawWbnaa)) and not type(raw0) == DataRaw:
-            new_is_fidsum = True
-
-        open_is_fidsum = False
-        if isinstance(raw1, (BlockPrepFidsum, BlockPrepWbnaa)):
-            open_is_fidsum = True
-
-        if not (new_is_fidsum == open_is_fidsum):
-            raise util_exceptions.OpenFileTypeMismatchError
+        # NB. bjs  1/30/23 - commented this out so I can read in MrsDataRaw
+        # files with FidsumMpress files for ECC and Quant rather than have to
+        # save all FIDs and process them in.
+        #
+        # raw0 = raws[0]
+        # raw1 = open_dataset.blocks["prep"]
+        #
+        # new_is_fidsum = False
+        # if isinstance(raw0, (DataRawFidsum, DataRawWbnaa)) and not type(raw0) == DataRaw:
+        #     new_is_fidsum = True
+        #
+        # open_is_fidsum = False
+        # if isinstance(raw1, (BlockPrepFidsum, BlockPrepWbnaa)):
+        #     open_is_fidsum = True
+        #
+        # if not (new_is_fidsum == open_is_fidsum):
+        #     raise util_exceptions.OpenFileTypeMismatchError
 
         for raw in raws:
-            if fidsum:
-                dims_flag = (raw.data_shape[-1] == open_dataset.raw_shape[-1])
-            else:
-                dims_flag = (raw.data_shape == open_dataset.raw_shape)
+            # NB. bjs  1/30/23 - commented this out so I can read in MrsDataRaw
+            # files with FidsumMpress files for ECC and Quant rather than have to
+            # save all FIDs and process them in.
+            #
+            # if fidsum:
+            #     dims_flag = (raw.data_shape[-1] == open_dataset.raw_shape[-1])
+            # else:
+            #     dims_flag = (raw.data_shape == open_dataset.raw_shape)
+
+            dims_flag = (raw.data_shape[-1] == open_dataset.raw_shape[-1])
 
-            if  dims_flag and (abs(raw.sw - open_dataset.sw) < 0.001):
+            if dims_flag and (abs(raw.sw - open_dataset.sw) < 0.001):
                 # Add the 'slight difference' equation for real world conditions. All is well!
                 pass
             else:
                 raise util_exceptions.OpenFileAttributeMismatchError
                    
                    
     def _check_for_si(self):
```

## vespa/analysis/fileio/siemens_twix.py

```diff
@@ -93,24 +93,30 @@
 
     def _get_parameters(self, twix, index='rep'):
         """ Return parameters and data from a Siemens Twix """
 
         evps = twix.evps
 
         header, clean_header = self._parse_protocol_data(evps[3][1])
-
+        hdr_dicom = evps[1][1]
         # CMRR sLASER info - need to move later
         #
         # MEAS.sSpecPara.lAutoRefScanMode [aushFreePara2 for VB] >1, water refs are saved
         # MEAS.sSpecPara.lAutoRefScanNo   [aushFreePara3 for VB] = number of scans acquired for ecc and water scaling references at start and end of protocol.
 
-        software = header['sProtConsistencyInfo.tBaselineString'].lower()
-        if   'n4_vb' in software: software_version = 'vb'
-        elif 'n4_vd' in software: software_version = 'vd'
-        elif 'n4_ve' in software: software_version = 've'
+        if 'sProtConsistencyInfo.tBaselineString' not in list(header.keys()):
+            if "syngo MR XA" in hdr_dicom:
+                software = 'nx_va'
+            else:
+                software_version = 'xx'
+        else:
+            software = header['sProtConsistencyInfo.tBaselineString'].lower()
+            if   'n4_vb' in software: software_version = 'vb'
+            elif 'n4_vd' in software: software_version = 'vd'
+            elif 'n4_ve' in software: software_version = 've'
 
         wiplong, wipdouble = self._get_xprot_wipvars(evps[2][1])
 
         if software_version == 'vb':
             ref_nscans  = int(header['sSpecPara.lAutoRefScanNo']) if 'sSpecPara.lAutoRefScanNo' in header.keys() else 0
             ref_flag    = int(ref_nscans != 0)
             prep_nscans = 0
```

## vespa/analysis/fileio/siemens_twix_svs_edit.py

```diff
@@ -51,15 +51,15 @@
             d["sw"] = d["sw"] / 2.0
 
         data = np.conjugate(data)
 
         dat_on  = data[0, :, :, :].copy()
         dat_off = data[1, :, :, :].copy()
         dat_sum = (dat_on + dat_off).copy()
-        dat_dif = (dat_on - dat_off).copy()
+        dat_dif = (dat_on - dat_off).copy()     # may need external coil combine ON for proper processing
 
         # Create a DataRawEditFidsum objects for the four different states
         # of the data ON, OFF, SUM and DIFFERENCE.
         
         d["data"] = dat_on
         d["data_source"] = filename+'.EditON'
         raw1 = DataRawEditFidsum(d)
```

## vespa/analysis/functors/funct_ecc.py

```diff
@@ -17,88 +17,91 @@
 # Eddy Current Correction Algorithms
 
 
 def ecc_fida(chain, ecc_raw, ecc_dataset):
 
     if ecc_dataset:
         voxel = chain.voxel
-        ecc = ecc_raw[voxel[2], voxel[1], voxel[0], :].copy()
-
-        npts = chain.data.shape[-1]
-        ds = chain._dataset
+        ecc   = ecc_raw[voxel[2], voxel[1], voxel[0], :].copy()
+        npts  = chain.data.shape[-1]
+        ds    = chain._dataset
         dwell = 1.0 / ds.sw
-        t  = np.arange(npts) * dwell
-        t150 = (npts * dwell) * np.arange(150, dtype=np.float)/149.0
-        # choose the part of the phase function that is most linear
-        tmin, tmax = 0.030, 0.400 # in sec
-        trange = np.logical_and(t >= tmin, t <= tmax)
 
-        import matplotlib.pyplot as plt
+        t  = np.arange(npts) * dwell
 
         inph0 = np.arctan2(ecc.imag, ecc.real)
         inph1 = np.unwrap(inph0)
-        inph  = phase2(inph1, trange)
 
+        # following code refines the np.unwrap() result in later 75%
+        # if the data is noisy and still wrapping
+        phi = inph1.copy()
+        npts = len(phi)
+        str2, end2 = int(npts * 0.02), int(npts * 0.25)
+        tt = np.arange(npts)
+        phi1 = np.polyval(np.polyfit(tt[str2:end2], phi[str2:end2], 1), tt)
+        phi2 = phi1.copy()
+        diff = phi - phi1
+        for i in range(end2 + 1, npts):
+            mult = -1 if diff[i] < 0 else 1.0
+            delta = diff[i]
+            while abs(delta) > abs(delta - (mult * np.pi * 2)):
+                delta = delta - (mult * np.pi * 2)
+            phi2[i] = delta + phi1[i]
+
+        inph = phi2
 
         # now fit a straight line to the linear part of the phase function
-        c = np.polyfit(t[trange], inph[trange],1)
+        # - choose a part of the phase function that is most linear
+        # - tmin, tmax = 0.030, 0.350 # in sec
+        str, end = int(npts * 0.03), int(npts * 0.35)
+        c = np.polyfit(t[str:end], inph[str:end],1)
         p = np.polyval(c, t)
 
         # now fit a spline to approximate a smooth version of the phase function
-        ff = sp.interpolate.splrep(t, inph, k=3, task=-1, t=t150[1:npts-1])
-        pp = sp.interpolate.splev(t, ff)
+        smooth = (npts - np.sqrt(2*npts))/1.15     # default in scipy docs, nudge from bjs
+        pp = sp.interpolate.splev(t, sp.interpolate.splrep(t, inph, k=3, s=smooth))
 
         # subtract line from spline -> eddy current related phase offset
         ecphase = pp - p
 
         chain.data = np.abs(chain.data) * util_math.safe_exp(-1j * ecphase)
 
         chain.data *= util_math.safe_exp(1j * 180.0*ecphase[0]/np.pi)
 
+        # import matplotlib.pyplot as plt
+        # plt.plot(t, inph0, t, inph)
+        # plt.show()
 
-def phase2(phi):
-    """
-    Find a linear fit line based on a "nice" part of the data
-    For every point, find the integer multiple of 2π that brings the data closest to the fit line.
-    Return {processed data, fit line object, plot}
-
-    """
-    npts = len(phi)
-    str, end = npts * 0.02, npts * 0.25
-    t = np.arange(npts)
-    phi1 = np.polyval(np.polyfit(t[str:end],phi[str:end], 1),t)
-    phi2 = phi1.copy()
-
-    diff = phi - phi1
-    for i in range(end+1,npts):
-        mult = -1 if diff[i] < 0 else 1.0
-        delta = diff[i]
-        while abs(delta) > abs(delta-(mult*np.pi*2)):
-            delta = delta-(mult*np.pi*2)
-        phi2[i] = delta + phi1[i]
-
-    return phi2
 
 
 
 
 def ecc_klose(chain, ecc_raw, ecc_dataset):
+    """ 
+    Based on Klose U. In vivo proton spectroscopy in presence of eddy currents. 
+    Magn Reson Med 1990;14(1):26-30.
+    
+    """
     if ecc_dataset: 
-        voxel = chain.voxel
+        voxel  = chain.voxel
         ecc    = ecc_raw[voxel[2],voxel[1],voxel[0],:]
-        # phecc  = np.angle(ecc)
-        # phtime = np.angle(chain.data)
-        # chain.data  = abs(chain.data) * util_math.safe_exp(1j*(phtime-phecc))
 
         phecc  = np.angle(ecc) - np.angle(ecc[0])
         phtime = np.angle(chain.data) - np.angle(chain.data[0])
         chain.data  = np.abs(chain.data) * util_math.safe_exp(1j*(phtime-phecc))
 
 
 def ecc_quality(chain, ecc_raw, ecc_dataset):
+    """
+    Based on De Graaf
+    De Graaf AA, van Dijk JE, Bovee WMMJ. QUALITY: Quantification improvement 
+    by converting lineshapes to the Lorentzian type. Magn Reson Med 
+    1990;13:343-357.
+    
+    """
     
     if ecc_dataset: 
         voxel = chain.voxel
         
         ecc = ecc_raw[voxel[2],voxel[1],voxel[0],:]
         
         thresh = 0.01
@@ -111,14 +114,18 @@
         chain.data  = chain.data / ecc  
 
      
 def ecc_quecc(chain, ecc_raw, ecc_dataset):
     """
     Based on Bartha, et.al. MRM Vol 44, p.641-645, 2000
     
+    Bartha R, Drost DJ, Menon RS, Williamson PC. Spectroscopic lineshape 
+    correction by QUECC: combined QUALITY deconvolution and eddy current 
+    correction. Magn Reson Med 2000;44(4):641-645.
+    
     "There are two important issues that must be considered when implementing 
     QUECC: determining the optimal crossover point (time) to end the QUALITY 
     deconvolution and begin the ECC, and ensuring there is no discontinuity 
     at this crossover point.
     
     Phase continuity is automatically maintained at the QUECC crossover point
     because both QUALITY deconvolution and ECC techniques subtract the phase
@@ -205,14 +212,15 @@
             phase = np.angle(ecc[index])
             tom = (thresh * (ecc[index]/abs(ecc[index])) * util_math.safe_exp(1j * phase)).astype('complex64')
             ecc[index] = tom
         
         chain.data  = chain.data / ecc    
 
 
+
 def ecc_traf(chain, ecc_raw, ecc_dataset):
     
     if ecc_dataset: 
 
         voxel = chain.voxel
 
         # water reference FID
@@ -591,16 +599,19 @@
 
     # plt.plot(y0)
     # plt.plot(20+y2*180/np.pi, 'b', linewidth=2)
     # plt.show()
 
     # testing ecc_fida()
 
-    fmetab = r"D:\Users\bsoher\code\repository_svn\sample_data\press_cp_svs_data\press_cp2.rsd"
-    fwater = r"D:\Users\bsoher\code\repository_svn\sample_data\press_cp_svs_data\press_cp2_wref.rsd"
+    #fmetab = r"D:\Users\bsoher\code\repository_svn\sample_data\press_cp_svs_data\press_cp2.rsd"
+    #fwater = r"D:\Users\bsoher\code\repository_svn\sample_data\press_cp_svs_data\press_cp2_wref.rsd"
+
+    fmetab = r"D:\Users\bsoher\code\repository_svn\sample_data\press_cp_svs_data\press_cp1.rsd"
+    fwater = r"D:\Users\bsoher\code\repository_svn\sample_data\press_cp_svs_data\press_cp1_wref.rsd"
 
     dsmet = util_file_import.get_datasets_cli(fmetab, 'import_vasf', None)[0]
     dswat = util_file_import.get_datasets_cli(fwater, 'import_vasf', None)[0]
 
     met = dsmet.blocks['raw'].data
     wat = dswat.blocks['raw'].data
 
@@ -612,16 +623,16 @@
 
     chain = TempObj(met, dsmet)
 
     savdat = chain.data.copy()
 
     ecc_fida(chain, wat, dswat)
 
-    plt.plot(savdat.real)
-    plt.plot(chain.data.real, 'b', linewidth=2)
+    plt.plot(np.ravel(savdat.real))
+    plt.plot(np.ravel(chain.data.real), 'b', linewidth=2)
     plt.show()
 
 
     bob = 10
     bob += 1
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## vespa/analysis/functors/funct_fidsum_correction.py

```diff
@@ -272,14 +272,15 @@
     return corr_freq, corr_phas
 
 
 
 def correction_rats_suspect(raw, chain):
     """ 
     FID frequency and phase correction method - RATS from Suspect
+    https://onlinelibrary.wiley.com/doi/abs/10.1002/mrm.27605
     
     Corrects individual FID data from an MRS data set for frequency and phase
     drifts through time
 
     Inputs:
         raw (ndarray, complex): shape=(1, 1, nfids, npts) dimensions, raw kspace data
         chain (object): block settings for algorithm
```

## vespa/analysis/functors/funct_fit_voigt.py

```diff
@@ -20,65 +20,65 @@
 from vespa.analysis.constants import FitLineshapeModel, FitMacromoleculeMethod
 from vespa.analysis.algos.constrained_levenberg_marquardt import constrained_levenberg_marquardt
 
 from vespa.analysis.constants import FitOptimizeMethod as optmeth
 
 
 def initial_values(chain):
-    
+
     set = chain._block.set
-    
+
     nmet    = chain.nmet
     dim0    = chain._dataset.spectral_dims[0]
-    dat     = chain.data 
-    
+    dat     = chain.data
+
     unique_abbr = chain._dataset.prior_list_unique
 
     util_initial_values.find_initial_values(chain)
 
     if chain.init_ph0 == 0: chain.init_ph0 = 0.0001
     if chain.init_ph1 == 0: chain.init_ph1 = 0.0001
 
     # Calculate parameter initial values
-    a = np.hstack([chain.init_area, 
+    a = np.hstack([chain.init_area,
                    chain.init_freq,         # this is radians here
-                   chain.init_ta[0], 
-                   chain.init_tb[0], 
+                   chain.init_ta[0],
+                   chain.init_tb[0],
                    chain.init_ph0,
                    chain.init_ph1 ])
 
 
-    # Update parameter bounds 
-    
+    # Update parameter bounds
+
     small_excludes = constants.FIT_OPTIMIZE_EXCLUDES_FOR_SMALL_PEAKS
-    
-    # Areas constraints    
+
+    # Areas constraints
     # areamax = chain.init_area * (1.0 + set.optimize_limits_range_area/100.0)
     # areamin = chain.init_area *  1e-8   # no zeros, else derivatives blow up in optimization
 
     areamin = []
     areamax = []
     for i,abbr in enumerate(unique_abbr):
-        
+
         if set.optimize_enable_bounds_area_small and abbr not in small_excludes:
             maxbnd = (set.optimize_bounds_area_max_small/100.0)
             minbnd = (set.optimize_bounds_area_min_small/100.0)
         else:
             maxbnd = (set.optimize_bounds_area_max/100.0)
             minbnd = (set.optimize_bounds_area_min/100.0)
-        
+
         val = chain.init_area[i] * minbnd if chain.init_area[i] * minbnd > 1e-8 else 1e-8
-        areamin.append(val)    
+        areamin.append(val)
         areamax.append(chain.init_area[i] * maxbnd)
-    
+
 #     for labl, minv, maxv in zip(unique_abbr, areamin, areamax):
 #         if len(labl) == 2: labl = labl+'  '
 #         if len(labl) == 3: labl = labl+' '
 #         print "Area - "+labl+" Min/Max = "+str(minv)+"/"+str(maxv) 
-        
+
     # PPM constraints
     fredel       = set.optimize_bounds_range_ppm       * 2.0 * np.pi       # convert Hz to radians here
     fredel_small = set.optimize_bounds_range_ppm_small * 2.0 * np.pi       # convert Hz to radians here
     fremin = []
     fremax = []
     for i,abbr in enumerate(unique_abbr):
         # use either the standard freq delta or the alternative one
@@ -97,18 +97,18 @@
 
     # Linewidth constraints - start with VOIGT assumptions
     lwAmin = set.optimize_bounds_min_linewidth
     lwAmax = set.optimize_bounds_max_linewidth
     lwBmin = set.optimize_bounds_min_linewidth
     lwBmax = set.optimize_bounds_max_linewidth
 
-    if set.lineshape_model == FitLineshapeModel.LORENTZ:  
+    if set.lineshape_model == FitLineshapeModel.LORENTZ:
           lwBmin = 1000.0 - 0.001
           lwBmax = 1000.0 + 0.001
-    elif set.lineshape_model == FitLineshapeModel.GAUSS:  
+    elif set.lineshape_model == FitLineshapeModel.GAUSS:
           lwAmin = chain.fix_t2_center - 0.001
           lwAmax = chain.fix_t2_center + 0.001
 
     # Phase0 constraints
     ph0min = chain.init_ph0 - (set.optimize_bounds_range_phase0 * np.pi / 180.0)
     ph0max = chain.init_ph0 + (set.optimize_bounds_range_phase0 * np.pi / 180.0)
 
@@ -140,19 +140,19 @@
 #         mmol_fre_min = mmol_fre_min * 2.0 * np.pi   # convert to radians
 
     lim = np.array([bot,top])
     chain.limits = lim
 
     # Save results and calculate some other initial value parameters
     chain.initial_values = a.copy()
-    chain.current_lw = set.initial_linewidth_value   
+    chain.current_lw = set.initial_linewidth_value
 
     # set the weight array
     chain.weight_array = util_initial_values.set_weight_array( chain )
-    
+
 
 
 
 
 # def create_param_labels(chain):
 #     """  Create list of unique parameter labels """
 #
@@ -200,20 +200,20 @@
 
     return np.array(a)
 
 
 def initialize_for_fit(chain):
     """
     This is a final step before fitting to do any miscellaneous setup.
-    
+
     1) create list of parameter labels
     2) scale initial values if necessary
     3) move 'initial values' to the 'fit results' attribute which is the
        semi-permanent container used in the fit optimize loop
-    4) convert original style parameter lists to LMFIT Parameter objects. 
+    4) convert original style parameter lists to LMFIT Parameter objects.
        These will be converted back in the finalize_from_fit() method.
     5) if there are any constraints set, these are applied as part of the
        conversion to Parameter objects
 
     Notes about using LMFIT inequality parameter expressions - bjs
     ---------------------------------------------------------------------------
     - great example here: https://lmfit.github.io/lmfit-py/parameters.html
@@ -283,15 +283,15 @@
 
     if set.optimize_method == optmeth.CONSTRAINED_LEVENBERG_MARQUARDT:
         pass        # no changes needed
 
     elif set.optimize_method in [optmeth.LMFIT_DEFAULT, optmeth.LMFIT_JACOBIAN]:
         for i in range(len(a)):
             wig = 0.02       # global wiggle amount in PPM
-                
+
             if set.optimize_constrain_ppm_naa_naag and plabel[i]=='freq_naag' and 'freq_naa' in plabel:
 
                 delta = pkppms['naag'] - pkppms['naa'] + 0.02  # empirical - bjs
                 params.add(name='delta_freq_naag', value=delta*const1, min=(delta-0.01)*const1, max=(delta+0.05)*const1, vary=True)
                 params['freq_naag'].set(expr='freq_naa - delta_freq_naag')
 
             elif set.optimize_constrain_ppm_cr_pcr and plabel[i]=='freq_pcr'and 'freq_cr' in plabel:
@@ -328,83 +328,83 @@
     chain.fit_results = params
 
 
 
 def finalize_from_fit(chain): 
     """
     This is where we:
-    - convert LMFIT Parameter objects back into the lists and numpy arrays 
+    - convert LMFIT Parameter objects back into the lists and numpy arrays
     - undo parameter scaling if necessary
-    
-    
+
+
     """
     set = chain._block.set
-    
-    # Convert Parameters dict to list --- 
+
+    # Convert Parameters dict to list ---
     params = chain.fit_results
 
     a = param2a(chain, params)
 
     # v = params.valuesdict()
     # a = np.array([item[1] for item in list(v.items())])
 
-    # Scale parameter list values if needed --- 
+    # Scale parameter list values if needed ---
     if set.optimize_scaling_flag:
         chis, wchis, badfit = chain.fit_stats
         a, chis, wchis, baseline = parameter_unscale(chain, a, chain.pscale, chis, wchis, baseline=chain.fit_baseline)
         chain.fit_stats    = np.array([chis, wchis, badfit])
         chain.fit_baseline = baseline
-        
+
     chain.fit_results = a
-            
-            
+
+
 
 def baseline_model(chain): 
     set = chain._block.set
     if set.baseline_method:
 
         data = chain.data.copy()
 
         a = chain.fit_results.copy()
         model, _ = chain.fit_function(a, pderflg=False, nobase=True)
 
         v = a.valuesdict()
         a0 = np.array([item[1] for item in list(v.items())])
 
-        # Subtract metabolite model from data 
+        # Subtract metabolite model from data
         basr = data.real - model.real
         basi = data.imag - model.imag
 
         hpp = chain._dataset.spectral_hpp
 
         # Smooth the remaining features
-        if set.baseline_smoothing_flag: 
-            if not (chain.iteration == set.optimize_global_iterations and 
-                    set.baseline_skip_last_smooth): 
+        if set.baseline_smoothing_flag:
+            if not (chain.iteration == set.optimize_global_iterations and
+                    set.baseline_skip_last_smooth):
                 wid  = set.baseline_smoothing_width / chain._dataset.sw    # convert Hz into % points
                 basr = lowess.lowess(basr, frac=wid, delta=3.2)
                 basi = lowess.lowess(basi, frac=wid, delta=3.2)
 
         # Calculate the baseline
 
         if set.baseline_method == constants.FitBaselineMethod.BSPLINE_VARIABLE_KNOT:
             ny     = np.size(basr)
             korder = set.baseline_spline_order
             nknots = set.baseline_spline_nknots
 
-            # Start with evenly distributed interior knots 
+            # Start with evenly distributed interior knots
             baser  = splines.splinevar(basr, nknots, korder, hz_per_pt=hpp)
-            basei  = splines.splinevar(basi, nknots, korder, hz_per_pt=hpp)    
+            basei  = splines.splinevar(basi, nknots, korder, hz_per_pt=hpp)
 
         elif set.baseline_method == constants.FitBaselineMethod.BSPLINE_FIXED_KNOT:
             ny     = np.size(basr)
             korder = set.baseline_spline_order
             nknots  = chain._dataset.sw / (set.baseline_spline_spacing*chain._dataset.spectral_hpp)
 
-            # Calculate an even distribution of the interior knots 
+            # Calculate an even distribution of the interior knots
             baser  = splines.splinefix(basr,nknots,korder)
             basei  = splines.splinefix(basi,nknots,korder)
 
         elif set.baseline_method == constants.FitBaselineMethod.WAVELET_FILTER_BASIC:
 
             # wavelet filter - Requires data to have power of 2 length
             thresh  = chain.current_lw / chain._dataset.spectral_hpp
@@ -415,43 +415,43 @@
             basei = wavelet_filter.wavelet_filter(basi, thresh, scale, dyadmin=dyadmin)
 
         else:
             raise ValueError('Unknown baseline method "%s"' % str(set.baseline_method))
 
         if set.baseline_underestimate_method == constants.FitBaselineUnderestimateMethod.FIRST_ITERATION_ONLY:
 
-            if chain.iteration == 1: 
-                # Account for when metabolites are inverted due to phase 
+            if chain.iteration == 1:
+                # Account for when metabolites are inverted due to phase
                 orient = 1.0
-                if abs(a0[chain.nmet*2+2] / common_constants.DEGREES_TO_RADIANS) > 90.0: 
-                    orient = -1.0 
-    
-                # Set the underestimation for first pass 
+                if abs(a0[chain.nmet*2+2] / common_constants.DEGREES_TO_RADIANS) > 90.0:
+                    orient = -1.0
+
+                # Set the underestimation for first pass
                 baser = baser - (set.baseline_underestimate/100.0)*abs(baser)*orient
                 basei = basei - (set.baseline_underestimate/100.0)*abs(basei)*orient
 
         elif set.baseline_underestimate_method == constants.FitBaselineUnderestimateMethod.MULTI_STEP_UNDERESTIMATION:
-            
+
             if chain.iteration <= set.baseline_underestimate_steps:
-                
+
                 urange = np.linspace(set.baseline_underestimate, set.baseline_underestimate_last, num= set.baseline_underestimate_steps)
-                uscale = urange[chain.iteration-1] 
+                uscale = urange[chain.iteration-1]
 
-                # Account for when metabolites are inverted due to phase 
+                # Account for when metabolites are inverted due to phase
                 orient = 1.0
-                if abs(a0[chain.nmet*2+2] / common_constants.DEGREES_TO_RADIANS) > 90.0: 
-                    orient = -1.0 
-    
-                # Set the underestimation for first pass 
+                if abs(a0[chain.nmet*2+2] / common_constants.DEGREES_TO_RADIANS) > 90.0:
+                    orient = -1.0
+
+                # Set the underestimation for first pass
                 baser = baser - (uscale/100.0)*abs(baser)*orient
                 basei = basei - (uscale/100.0)*abs(basei)*orient
-            
+
 
         base = baser + 1j * basei  #s Make complex array from real and imaginary parts
-        
+
         chain.fit_baseline = base
     else:
         # Baseline == None, we need to zero the result
         chain.fit_baseline = chain.data.copy() * 0.0
 
 
 def optimize_model(chain):
@@ -607,15 +607,15 @@
     v = a.valuesdict()
     a0 = np.array([item[1] for item in list(v.items())])
 
     a0 = a0[0:chain.nparam]
 
     nmet    = chain.nmet
     dim0    = chain._dataset.spectral_dims[0]
-    dat     = chain.data.copy() 
+    dat     = chain.data.copy()
     bas     = chain.fit_baseline
     ww      = chain.weight_array
     lim     = chain.limits
     na      = np.size(a0)
 
     chain.confidence = chain.confidence * 0     # init results array
 
@@ -680,40 +680,40 @@
         for i in range(nmet):
             cinfo.indx = nmet + i
 
             frehi = a0[cinfo.indx]     # use these if optimization hit a limit
             frelo = a0[cinfo.indx]
 
             if a0[cinfo.indx] > lim[0,cinfo.indx] and \
-               a0[cinfo.indx] < lim[1,cinfo.indx]: 
+               a0[cinfo.indx] < lim[1,cinfo.indx]:
                 xa = a0[cinfo.indx] + 0.0
                 xb = a0[cinfo.indx] + 1.0
                 xc = lim[1,cinfo.indx]     # reasonable limit for upper bound
 
                 frehi, _ = minf.minf_parabolic_info(xa, xb, xc, func1, cinfo, tol=1e-6)
                 xa = a0[cinfo.indx] - 0.01
                 xb = a0[cinfo.indx] - 1.0
                 xc = lim[0,cinfo.indx]        # reasonable limit for lower bound
 
                 frelo, _ = minf.minf_parabolic_info(xa, xb, xc, func1, cinfo, tol=1e-6)
 
             # save the confidence interval as it's width in PPM (tends to be tight)
             chain.confidence[cinfo.indx] =  (frehi - frelo) / chain._dataset.frequency
 
-    if set.confidence_linewidth_flag: 
-        # Voigt or Lorentzian 
+    if set.confidence_linewidth_flag:
+        # Voigt or Lorentzian
         cinfo.indx = nmet*2 + 0
 
         tahi = a0[cinfo.indx]    # use these if optimization hit a limit
         talo = a0[cinfo.indx]
 
-        if (set.lineshape_model == FitLineshapeModel.VOIGT or 
-            set.lineshape_model == FitLineshapeModel.LORENTZ): 
+        if (set.lineshape_model == FitLineshapeModel.VOIGT or
+            set.lineshape_model == FitLineshapeModel.LORENTZ):
             if a0[cinfo.indx] > lim[0,cinfo.indx] and \
-               a0[cinfo.indx] < lim[1,cinfo.indx]: 
+               a0[cinfo.indx] < lim[1,cinfo.indx]:
                 xa = a0[cinfo.indx] * 1.0
                 xb = a0[cinfo.indx] + abs(a0[cinfo.indx]) * 0.01
                 xc = lim[0,cinfo.indx]        # reasonable limit for upper bound
 
                 tahi, _ = minf.minf_parabolic_info(xa, xb, xc, func1, cinfo, tol=1e-6)
 
                 xa = a0[cinfo.indx] - abs(a0[cinfo.indx]) * 0.0001
@@ -724,18 +724,18 @@
 
         # Voigt or Gaussian
         cinfo.indx = nmet*2 + 1
 
         tbhi = a0[cinfo.indx]    # use these if optimization hit a limit
         tblo = a0[cinfo.indx]
 
-        if (set.lineshape_model == FitLineshapeModel.VOIGT or 
-            set.lineshape_model == FitLineshapeModel.GAUSS): 
+        if (set.lineshape_model == FitLineshapeModel.VOIGT or
+            set.lineshape_model == FitLineshapeModel.GAUSS):
             if a0[cinfo.indx] > lim[0,cinfo.indx] and \
-               a0[cinfo.indx] < lim[1,cinfo.indx]: 
+               a0[cinfo.indx] < lim[1,cinfo.indx]:
                 xa = a0[cinfo.indx] * 1.0
                 xb = a0[cinfo.indx] + abs(a0[cinfo.indx]) * 0.01
                 xc = lim[0,cinfo.indx]        # reasonable limit for upper bound
 
                 tbhi, _ = minf.minf_parabolic_info(xa, xb, xc, func1, cinfo, tol=1e-6)
 
                 xa = a0[cinfo.indx] - abs(a0[cinfo.indx]) * 0.0001
@@ -748,46 +748,46 @@
         lwmax, _ = util_spectral.voigt_width(tahi, tbhi, chain._dataset)
         lwmin, _ = util_spectral.voigt_width(talo, tblo, chain._dataset)
 
         # save the confidence interval for max and min LW in Hz
         chain.confidence[nmet*2 + 0] = talo - tahi # lwmin
         chain.confidence[nmet*2 + 1] = tblo - tbhi # lwmax
 
-    if set.confidence_phase_flag: 
+    if set.confidence_phase_flag:
         # Zero Order Phase
         cinfo.indx = nmet*2 + 2
 
         ph0hi = a0[cinfo.indx]    # use these if optimization hit a limit
         ph0lo = a0[cinfo.indx]
 
         if a0[cinfo.indx] > lim[0,cinfo.indx] and \
-           a0[cinfo.indx] < lim[1,cinfo.indx]: 
+           a0[cinfo.indx] < lim[1,cinfo.indx]:
             xa = a0[cinfo.indx]
             xb = a0[cinfo.indx] + abs(a[cinfo.indx]) * 0.01
             xc = lim[1,cinfo.indx]        # reasonable limit for upper bound
 
             ph0hi, _ = minf.minf_parabolic_info(xa, xb, xc, func1, cinfo, tol=1e-6)
 
             xa = a0[cinfo.indx] - abs(a0[cinfo.indx]) * 0.0001
             xb = a0[cinfo.indx] - abs(a0[cinfo.indx]) * 0.01
             xc = lim[0,cinfo.indx]        # reasonable limit for lower bound
 
             ph0lo, _ = minf.minf_parabolic_info(xa, xb, xc, func1, cinfo, tol=1e-6)
 
         # save the confidence interval as it's width in Hz (tends to be tight)
-        chain.confidence[cinfo.indx] =  (ph0hi - ph0lo) * 180.0 / np.pi    
+        chain.confidence[cinfo.indx] =  (ph0hi - ph0lo) * 180.0 / np.pi
 
         # Zero Order Phase
         cinfo.indx = nmet*2 + 3
 
         ph1hi = a0[cinfo.indx]    # use these if optimization hit a limit
         ph1lo = a0[cinfo.indx]
 
         if a0[cinfo.indx] > lim[0,cinfo.indx] and \
-           a0[cinfo.indx] < lim[1,cinfo.indx]: 
+           a0[cinfo.indx] < lim[1,cinfo.indx]:
             xa = a0[cinfo.indx]
             xb = a0[cinfo.indx] + abs(a0[cinfo.indx]) * 0.01
             xc = lim[1,cinfo.indx]        # reasonable limit for upper bound
 
             ph1hi, _ = minf.minf_parabolic_info(xa, xb, xc, func1, cinfo, tol=1e-6)
 
             xa = a0[cinfo.indx] - abs(a0[cinfo.indx]) * 0.0001
@@ -798,38 +798,38 @@
 
         # save the confidence interval as it's width in Hz (tends to be tight)
         chain.confidence[cinfo.indx] =  (ph1hi - ph1lo) * 180.0 / np.pi
         chain.minmaxlw = [lwmin,lwmax]
 
 
 def _confidence_interval_function(xq, cinfo):
-    """ 
+    """
     calculation of the weighted chi squared to adjust the fitted array a
-    
+
     """
     a = cinfo.a.copy()
     a[list(a.keys())[cinfo.indx]].set(value=xq)
 
     yfit, _ = cinfo.fit_function(a, pderflg=False)
     if yfit.dtype in ['complex64','complex128']:
         yfit = np.concatenate([yfit.real,yfit.imag])
     wchisqr1 = np.sum(cinfo.ww*(yfit-cinfo.dat)**2)/cinfo.nfree
-    
+
     goal = abs(wchisqr1-cinfo.wchi*cinfo.factor)
-    
+
     return goal
 
-    
+
 def cramer_rao_bounds(chain):
 
     set = chain._block.set
 
     nmet    = chain.nmet
     dim0    = chain._dataset.spectral_dims[0]
-    dat     = chain.data.copy() 
+    dat     = chain.data.copy()
     a       = chain.fit_results.copy()
     bas     = chain.fit_baseline.copy()
     nparam  = chain.nparam
 
     v = a.valuesdict()
     a0 = np.array([item[1] for item in list(v.items())])
 
@@ -839,81 +839,97 @@
     # for estimating variance
 
     nstr = np.round(chain._dataset.ppm2pts(set.cramer_rao_ppm_end))
     nstr = int(np.where(nstr > 0, nstr, 0))
     nend = round(int(chain._dataset.ppm2pts(set.cramer_rao_ppm_start)))
     nend = int(np.where(nend < dim0-1, nend, dim0-1))
 
-    if nstr > nend: 
+    if nstr > nend:
         nstr, nend = nend, nstr     # swap
 
-    # Subtract calculated baseline from data to start residual calculation 
+    # Subtract calculated baseline from data to start residual calculation
     resid = dat-bas
     b = a0.copy()
 
     # we scale the area parameters here to try to keep the PDER array well
     # behaved, but we also have to scale the residual below if we do this
     savscal = set.optimize_scaling_flag
     set.optimize_scaling_flag = True
     b, pscale, _, _, _ = parameter_scale(chain, b)
 
-    # Cramer-Rao calcs here for this voxel - stored in fitt_data.cramer_rao 
+    # Cramer-Rao calcs here for this voxel - stored in fitt_data.cramer_rao
     # First dimension organized as follows:
     #     areas (for N metabs), freqs (xN) , Ta, Tb, Ph0, Ph1
     yfit, _ = chain.fit_function(a, pderflg=False, nobase=True)
     _, pder = chain.fit_function(b, nobase=True)
 
     # Finish residual calculation and calculate variance ---
     resid = (resid - yfit) / pscale[0]
-    section = resid[nstr:(nend+1)] 
-    vari  = np.std(np.concatenate((section.real,section.imag)))
-    #vari  = np.std(np.concatenate((resid[nstr:nend+1],resid[dim0+nstr:dim0+nend+1])))
-    vari  = vari*vari
+    section = resid[nstr:(nend+1)]
+    vari0  = np.std(np.concatenate((section.real,section.imag)))
+    vari  = vari0*vari0
 
     """
      NB. pder returns a fltarr(dim0*2,nparam), the dim0*2 is because the
            representation of complex numbers in the VeSPA program is to
            append the imag portion to the real portion in one long fltarr
 
      We are estimating the Fisher information matrix here using the covariance
       matrix calculated from the partial derivs of the non-linear optimization
 
      NB. the complex calculation: invert(float((conj(transpose(pderc))#pderc)))
          is equivalent to the 'pseudo-complex (double length real matrix)'
          calculation: invert((transpose(pder)#pder))
     """
 
-    # here we are using only the real part of the PDER array as per Bolan 
+    # here we are using only the real part of the PDER array as per Bolan
     try:
         tmp = np.dot(pder[0:dim0,:].real, pder[0:dim0,:].real.transpose())
         cr = np.linalg.inv(tmp)
 
+        osp_sigma = 1.0 / vari
+        osp_fisher = np.dot(pder[0:dim0,:].real, pder[0:dim0,:].real.transpose())
+        osp_fisher = osp_fisher.real
+        osp_fisher = osp_fisher * osp_sigma
+        osp_crlb_tmp = np.sqrt(np.linalg.inv(osp_fisher))
+        osp_crlb_crdiag = osp_crlb_tmp.diagonal()
+        osp_crlb, _, _, _ = parameter_unscale(chain, osp_crlb_crdiag, pscale)
+        osp_crlb_rel = osp_crlb.copy()
+        osp_crlb_rel[0:nmet]      = osp_crlb_rel[0:nmet] * 100.0 / a0[0:nmet]  # % change in area
+        osp_crlb_rel[nmet:nmet*2] = osp_crlb_rel[nmet:nmet*2]/chain._dataset.frequency # delta Hz to delta PPM
+        osp_crlb_rel[nmet*2+2]    = osp_crlb_rel[nmet*2+2] * 180.0 / np.pi  # radians to deg
+
+
         # If Cramer-Rao is not singular take the sqrt of the diagonal
-        # elements of CR times the estimated variance as CR bounds    
+        # elements of CR times the estimated variance as CR bounds
         crdiag = np.sqrt(vari*cr.diagonal())
 
         crdiag, _, _, _ = parameter_unscale(chain, crdiag, pscale)
 
 #            print 'cr   = ', cr.diagonal()
 #            print 'vari = ', vari
 #            print 'crdi = ', crdiag * 100 / a
 
         crdiag[0:nmet]      = crdiag[0:nmet] * 100.0 / a0[0:nmet]  # % change in area
         crdiag[nmet:nmet*2] = crdiag[nmet:nmet*2]/chain._dataset.frequency # delta Hz to delta PPM
         crdiag[nmet*2+2]    = crdiag[nmet*2+2] * 180.0 / np.pi  # radians to deg
         chain.cramer_rao = crdiag
 
+        print('crdiag_orig = ', crdiag)
+        print('crdiag_osp  = ', osp_crlb_rel)
+        bob = 11
+
         # this algorithm is based on the example shown in Bolan, MRM 50:1134-1143 (2003)
         # the factor of 2 here is used since we fit the complex data rather than
         # just the real data.
 
-    except np.linalg.LinAlgError:    
+    except np.linalg.LinAlgError:
         # If Cramer-Rao array is singular or contains a small
         # pivot return zero's for CR bounds
-        chain.cramer_rao = np.zeros(nparam, float)    
+        chain.cramer_rao = np.zeros(nparam, float)
 
 
 def parameter_scale(chain, a0, limits=None, data=None, baseline=None):
     """
     =========
     Arguments
     =========
@@ -939,18 +955,18 @@
     """
 
     if isinstance(a0, Parameters):
         v = a0.valuesdict()
         a = np.array([item[1] for item in list(v.items())])
     else:
         a = a0
-    
+
     nmet = chain.nmet
     set  = chain._block.set
-    
+
     pscale = a*0 + 1.0
 
     # Scale the Amplitude parameters ---
     # - the abs() were necessary when we decided to let areas be negative to fit water.
     amp    = a[0:nmet]
     ampscl = 1.0
 
@@ -960,15 +976,15 @@
     else:
         if max(amp) > 10.0:
             while (max(abs(amp*ampscl)) > 10.0):
                 ampscl = ampscl * 0.1
 
     a[0:nmet]      = amp * ampscl
     pscale[0:nmet] = 1.0 / ampscl
-    
+
     if set.macromol_model == FitMacromoleculeMethod.SINGLE_BASIS_DATASET:
         a[-2] = a[-2] * ampscl
         pscale[-2] = 1.0/ampscl
 
     if baseline is not None:
         baseline = baseline * ampscl
 
@@ -981,15 +997,15 @@
         top = limits[1,:]
         top[0:nmet] = top[0:nmet] * ampscl
         bot[0:nmet] = bot[0:nmet] * ampscl
 
         if set.macromol_model == FitMacromoleculeMethod.SINGLE_BASIS_DATASET:
             top[-2] = top[-2] * ampscl
             bot[-2] = bot[-2] * ampscl
-        
+
         limits = np.array([bot,top])
 
     if isinstance(a0, Parameters):
         v = a0.valuesdict()
         for i,item in enumerate(v.keys()):
             a0[item].set(value=a[i])
 
@@ -1046,29 +1062,29 @@
 
 
 
 
 
 #------------------------------------------------------------------------------
 # Method calls for different entry points' processing
-    
+
 def do_processing_initial(chain):
-    """ 
+    """
     - initial values calc
     - save current plot of model with initial values as input
-    
+
     - NB. Never becomes a Parameters set
-    
+
     """
     initial_values(chain)
     save_yini(chain)
-    
-       
+
+
 def do_processing_full_fit(chain):
-    """ 
+    """
     - initial values calc
     - prep values for fitting loop
     Loop
         - baseline
         - model
     (optional) Confidence Intervals and Cramer-Rao
         - confidence intervals
@@ -1077,70 +1093,70 @@
     - save current plot of model with final values as input
     """
     set   = chain._block.set
     niter = set.optimize_global_iterations
 
     if chain.statusbar: chain.statusbar.SetStatusText(' Functor = initial_values ', 0)
     initial_values(chain)
-    
+
     if chain.statusbar: chain.statusbar.SetStatusText(' Functor = initialize_for_fit ', 0)
     initialize_for_fit(chain)
-    
+
     # fitting loop
     for i in range(niter):
         chain.iteration += 1
         if chain.statusbar: chain.statusbar.SetStatusText(' Functor = baseline_model (Loop %d/%d) ' % (i+1,niter), 0)
         baseline_model(chain)
         if chain.statusbar: chain.statusbar.SetStatusText(' Functor = optimize_model (Loop %d/%d) ' % (i+1,niter), 0)
         optimize_model(chain)
-        
+
     if (set.confidence_intervals_flag==True):
         if chain.statusbar: chain.statusbar.SetStatusText(' Functor = confidence_intervals ', 0)
         confidence_intervals(chain)
-    
+
     if (set.cramer_rao_flag==True):
         if chain.statusbar: chain.statusbar.SetStatusText(' Functor = cramer_rao_bounds ', 0)
         cramer_rao_bounds(chain)
 
     finalize_from_fit(chain)
 
     if chain.statusbar: chain.statusbar.SetStatusText(' Functor = save_yini ', 0)
-    save_yini(chain)        
+    save_yini(chain)
     if chain.statusbar: chain.statusbar.SetStatusText(' Functor = save_yfit ', 0)
-    save_yfit(chain)        
-        
+    save_yfit(chain)
+
 
 def do_processing_output_refresh(chain):
-    """ 
+    """
     - save current plot of model with initial values as input
-    
+
     """
     save_yfit(chain)
-    
+
 
 def do_processing_plot_refresh(chain):
-    """ 
+    """
     - b0 correction
     - initial values calc
     - save current plot of model with initial values as input
-    
+
     """
     initial_values(chain)
     save_yini(chain)
     save_yfit(chain)
 
 
 def do_processing_voxel_change(chain, flag_auto_initvals=False):
-    """ 
+    """
     - save current plot of model with initial values as input
-    - save current plot of fitted values 
-    
+    - save current plot of fitted values
+
     """
     if flag_auto_initvals:
         initial_values(chain)
     save_yini(chain)
     save_yfit(chain)
 
-        
+
```

## vespa/common/constants.py

```diff
@@ -826,15 +826,15 @@
 
 ######################     Pulse constants     ########################
 
 DEFAULT_CALC_RESOLUTION = 5000
 DEFAULT_PULSE_BANDWIDTH_TYPE = 'half_height'
 DEFAULT_GYROMAGNETIC_NUCLEI = '1H'
 DEFAULT_BLOCH_RANGE_VALUE = 4.0
-DEFAULT_BLOCH_RANGE_UNITS = 'cm'
+DEFAULT_BLOCH_RANGE_UNITS = 'kHz'
 DEFAULT_BLOCH_OFFSET_VALUE = 0.0
 
 # sourced gamma vals from website http://bio.groups.et.byu.net/LarmourFreqCal.phtml
 # web site refs are :
 # -M A Bernstein, K F King and X J Zhou (2004). Handbook of MRI Pulse Sequences. 
 #   San Diego: Elsevier Academic Press. p. 960. ISBN 0-1209-2861-2.
 # -R C Weast, M J Astle, ed (1982). Handbook of Chemistry and Physics. Boca
```

## vespa/common/exception_handler.py

```diff
@@ -261,38 +261,37 @@
     # code is here to filter out noise. At any given moment there's lots of
     # modules loaded that we (mostly) don't care about. For instance, try
     # this to see how many modules are loaded just as a result of invoking
     # Python:
     #    python -c "import sys;  print sys.modules"
     #
 
-    # Some don't have a __file__ attr
+    # Some don't have a __file__ attr and some do but they are None, check for both
     modules = [module for module in list(sys.modules.values())
-                                 if hasattr(module, "__file__")]
+                                 if hasattr(module, "__file__") and module.__file__ is not None]
 
     # I figure out where most of the standard library modules are by selecting
     # a module (I picked the re module) and getting that module's path. I
     # then assume that anything with the same path is part of the Python
     # standard lib. This doesn't exclude all of the modules I'd like it to,
     # but it successfully removes many while erring on the side of caution.
     standard_library_path = ""
     for module in modules:
         head, tail = os.path.split(module.__file__)
-        if tail == "re.pyc":
+        if tail == "re.pyc" or tail == "re.py":
             standard_library_path = head
 
     # Remove Python modules
     f = lambda fq_filename: os.path.split(fq_filename)[0] != standard_library_path
     modules = [module for module in modules if f(module.__file__)]
 
     # What's left should be mostly modules that are not part of the standard
     # library. I build a list of 2-tuples consisting of (module filename,
     # module version).
-    modules = [ (module.__file__, _get_module_version(module)) for module
-                                                               in  modules]
+    modules = [ (module.__file__, _get_module_version(module)) for module in modules]
 
     modules = sorted(modules)
 
     return lines + modules
 
 
 def _get_python_info():
```

## vespa/common/ge_read_pfile.py

```diff
@@ -111,21 +111,25 @@
         if self.version < 12:
             if "GE" in self.hdr.rhr_rh_logo:
                 return True
             else:
                 return False
         else:
             offset = self.hdr.rhr_rdb_hdr_off_data
-            if ( offset == 61464  or        # bjs from matlap script for ver = 9 
-                 offset == 66072  or 
-                 offset == 145908 or 
-                 offset == 149788 or
-                 offset == 150336 or
-                 offset == 157276 or        # v24 empirical
-                 offset == 213684 ):        # v26 empirical
+            if offset in [
+              61464,   # bjs from matlap script for ver = 9 
+              66072,
+              145908,
+              149788,
+              150336,
+              157276,  # v24 empirical
+              213684,  # 26.002
+              219828,  # 27.000
+              228020   # 28.003
+              ]:
                 return True
             else:
                 return False
 
 
     @property
     def is_svs(self):
@@ -191,15 +195,15 @@
 
         
     def read_header(self):
 
         filelike = open(self.file_name, 'rb')
 
         # determine version number of this header from revision of rdbm.h
-        version = self._major_version(filelike)
+        version = self._version(filelike)
         if version == 0:
             raise UnknownPfile("Pfile not supported for version %s" % version)    
   
         # Here we dynamically configure the ctypes structures into which the
         # binary file will be read, based on the revision number
         #
         # Note. Determined empirically that I cannot declare the XxxHeader
@@ -209,15 +213,15 @@
         #
         # Note 2. Had to move Class definition into this function so that the
         # class can be reconstituted more than once for multiple GE file reads.
         # At the top level of the module, the _fields_ attribute could be 
         # created once dynamically, but afterwards would stick around and
         # could not then be changed. 
         
-        if version < 11:  # data taken on SGI - big endian
+        if self.endian == 'big':
             class PfileHeaderBig(BigEndianStructure):
                 """
                 Contains the ctypes Structure for a GE P-file rdb header.
                 Dynamically allocate the ctypes _fields_ list later depending on revision
                 """
                 _pack_   = 1            
                 _fields_ = get_pfile_hdr_fields(version)
@@ -257,58 +261,66 @@
         """
         mapper = self.get_mapper
         self.map = mapper(self.file_name, self.hdr, self.version, self.endian)
         self.map.read_data()
         
         
 
-    def _major_version(self, filelike):
+    def _version(self, filelike):
         """
         Get the rdbm.h revision number from first 4 bytes. Then map the rdbm 
         revision to a platform number (e.g. 11.x, 12.x, etc.)
         
         """
         rev_little = RevisionNumLittle()
         rev_big    = RevisionNumBig()
         filelike.seek(0)
         filelike.readinto(rev_little)
         filelike.seek(0)
         filelike.readinto(rev_big)
         
-        rev_little = rev_little.major
-        rev_big    = rev_big.major
+        rev_little = rev_little.revision
+        rev_big    = rev_big.revision
         
-        version = 0
-
-        if (rev_little > 6.95 and rev_little < 8.0) or (rev_big > 6.95 and rev_big < 8.0):
-            version = 9.0; 
-        elif ( rev_little == 9.0  or rev_big == 9.0  ): 
-            version = 11.0;
-        elif ( rev_little == 11.0 or rev_big == 11.0 ): 
-            version = 12.0;
-        elif ( rev_little == 14 or rev_big == 14 ): 
-            version = 14.0;
-        elif ( rev_little == 15 or rev_big == 15 ): 
-            version = 15.0;
-        elif ( rev_little == 16 or rev_big == 16 ): 
-            version = 16.0;
-        elif ( rev_little == 20 or rev_big == 20 ): 
-            version = 20.0;
-        elif ( rev_little == 21 or rev_big == 21 ): 
-            version = 21.0;
-        elif ( rev_little == 23 or rev_big == 23 ): 
-            version = 21.0;
-        elif ( rev_little == 24 or rev_big == 24 ): 
-            version = 24.0;
-        elif ( rev_little == 26 or rev_big == 26 ): 
-            version = 26.0;
+        known_revisions = [
+            7,      8,      9,      10,     11,
+            14.0,   14.1,   14.2,
+            15.000, 15.001, 16.000,
+            20.001, 20.002, 20.003, 20.004, 20.005, 20.006, 20.007,
+            24.000,
+            25.001, 25.002, 25.003, 25.004,
+            26.000, 26.001, 26.002,
+            27.000, 27.001,
+            28.000, 28.002, 28.003 ];
+
+        print(rev_little)
+        print(rev_big)
+        if any(np.isclose(rev_little,known_revisions)):
+            # little-endian: most reasonably recent implementations
+            self.endian = 'little'
+            version = rev_little;
+        elif any(np.isclose(rev_big,known_revisions)) and rev_big < 11:
+            # certain earlier revisions on SGI, big-endian
+            self.endian = 'big'
+            version = rev_big;
         else:
             raise UnknownPfile("Unknown header structure for revision %s" % rev_little)
 
-        return version; 
+        return version
+
+    def _major_version(self, filelike):
+        """
+        Get the rdbm.h revision number from first 4 bytes. Then map the rdbm
+        revision to a platform number (e.g. 11.x, 12.x, etc.)
+
+        """
+
+        version = self._version(filelike)
+
+        return int(np.trunc(version))
 
 
     def dump_header_strarr(self):
 
         dumped = self._dump_struct(self.hdr)
         strarr = []
         for info in dumped:
@@ -1144,15 +1156,17 @@
     This function returs a list of fields for mapping a GE P-file header
     to a ctypes class structure. We define different paddings and variable
     names depending on the software version that created the P-file.
     
     """
     plist = []
 
-    if version == 9:
+    version_major=int(np.trunc(version))
+
+    if version_major in [7, 8]:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -1361,15 +1375,15 @@
         plist.append( ('rhi_user43',               c_float) )
         plist.append( ('rhi_user44',               c_float) )
         plist.append( ('rhi_user45',               c_float) )
         plist.append( ('rhi_user46',               c_float) )
         plist.append( ('rhi_user47',               c_float) )
         plist.append( ('rhi_user48',               c_float) )
 
-    elif version == 11:
+    elif version_major == 9:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -1579,15 +1593,15 @@
         plist.append( ('rhi_user43',               c_float) )
         plist.append( ('rhi_user44',               c_float) )
         plist.append( ('rhi_user45',               c_float) )
         plist.append( ('rhi_user46',               c_float) )
         plist.append( ('rhi_user47',               c_float) )
         plist.append( ('rhi_user48',               c_float) )
 
-    elif version == 12:
+    elif version_major in [11, 12]:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -1803,15 +1817,15 @@
         plist.append( ('pad_xx',                   c_char * 38) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 14:
+    elif version_major == 14:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -2027,15 +2041,15 @@
         plist.append( ('pad_xx',                   c_char * 112) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 15:
+    elif version_major == 15:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -2251,15 +2265,15 @@
         plist.append( ('pad_xx',                   c_char * 116) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 16:
+    elif version_major == 16:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -2475,15 +2489,15 @@
         plist.append( ('pad_xx',                   c_char * 116) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 20:
+    elif version_major == 20:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -2696,15 +2710,15 @@
         plist.append( ('pad_xx',                   c_char * 130) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 21:
+    elif version_major < 23: # 21, 22
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -2917,15 +2931,15 @@
         plist.append( ('pad_xx',                   c_char * 130) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 23:
+    elif version_major == 23:
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -3138,15 +3152,15 @@
         plist.append( ('pad_xx',                   c_char * 130) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 24:  # 25 and 25.1 same pfile
+    elif version_major in [24, 25]:  # 25 and 25.1 same pfile
         plist.append( ('rhr_rh_rdbm_rev',          c_float) )
         plist.append( ('pad_xx',                   c_char * 12) )
         plist.append( ('rhr_rh_scan_date',         c_char * 10) )
         plist.append( ('rhr_rh_scan_time',         c_char * 8) )
         plist.append( ('rhr_rh_logo',              c_char * 10) )
         plist.append( ('rhr_rh_file_contents',     c_short) )
         plist.append( ('pad_xx',                   c_char * 10) )
@@ -3359,28 +3373,31 @@
         plist.append( ('pad_xx',                   c_char * 130) )
         plist.append( ('rhi_psdname',              c_char * 33) )
         plist.append( ('pad_xx',                   c_char * 84) )
         plist.append( ('rhi_cname',                c_char * 17) )
         plist.append( ('pad_xx',                   c_char * 51) )
         plist.append( ('rhi_image_uid',            c_char * 32) )
 
-    elif version == 26:
+    elif version_major in [26,27,28]:
         plist.append( ('rhr_rh_rdbm_rev',           c_float) )
         plist.append( ('rhr_rdb_hdr_off_data',      c_int) )
         plist.append( ('pad_xx',                    c_char * 84) )
         plist.append( ('rhr_rh_scan_date',          c_char * 10) )
         plist.append( ('rhr_rh_scan_time',          c_char * 8) )
         plist.append( ('rhr_rh_logo',               c_char * 10) )
         plist.append( ('rhr_rh_file_contents',      c_short) )
         plist.append( ('pad_xx',                    c_char * 10) )
         plist.append( ('rhr_rh_data_collect_type',  c_short) )
         plist.append( ('pad_xx',                    c_char * 6) )
         plist.append( ('rhr_rh_npasses',            c_short) )
         plist.append( ('pad_xx',                    c_char * 2) )
-        plist.append( ('rhr_rh_nslices',            c_short) )
+        if version < 28.002:
+            plist.append(('rhr_rh_nslices',         c_short)) # uint16
+        else:
+            plist.append(('rhr_rh_nslices_deprecated', c_short))
         plist.append( ('pad_xx',                    c_char * 10) )
         plist.append( ('rhr_rh_frame_size',         c_short) )
         plist.append( ('rhr_rh_point_size',         c_short) )
         plist.append( ('pad_xx',                    c_char * 104) )
         plist.append( ('rhr_rh_dab[0]_start_rcv',   c_short) )
         plist.append( ('rhr_rh_dab[0]_stop_rcv',    c_short) )
         plist.append( ('rhr_rh_dab[1]_start_rcv',   c_short) )
@@ -3450,15 +3467,22 @@
         plist.append( ('rhr_rh_user44',             c_float) )
         plist.append( ('rhr_rh_user45',             c_float) )
         plist.append( ('rhr_rh_user46',             c_float) )
         plist.append( ('rhr_rh_user47',             c_float) )
         plist.append( ('rhr_rh_user48',             c_float) )
         plist.append( ('pad_xx',                    c_char * 488) )
         plist.append( ('rhr_rh_raw_pass_size',      c_longlong) )
-        plist.append( ('pad_xx',                    c_char * 192684) )
+        if version < 28.002:
+            plist.append(('pad_xx',                 c_char * 192684) )
+        else:
+            plist.append(('pad_xx',                 c_char * 1652))
+            plist.append(('rhr_rh_nslices',         c_int)) # uint32
+            plist.append(('pad_xx',                 c_char * ( 192684 - 1652 - 4)))
+        if version > 27.0: # 27.001 +
+            plist.append(('pad_xx',                 c_char * 8192))
         plist.append( ('rhe_magstrength',           c_int) )
         plist.append( ('pad_xx',                    c_char * 4) )
         plist.append( ('rhe_ex_datetime',           c_int) )
         plist.append( ('pad_xx',                    c_char * 112) )
         plist.append( ('rhe_ex_no',                 c_short) )
         plist.append( ('pad_xx',                    c_char * 22) )
         plist.append( ('rhe_patsex',                c_short) )
@@ -3580,228 +3604,43 @@
         plist.append( ('rhi_freq_dir',              c_short) )
         plist.append( ('pad_xx',                    c_char * 130) )
         plist.append( ('rhi_psdname',               c_char * 33) )
         plist.append( ('pad_xx',                    c_char * 84) )
         plist.append( ('rhi_cname',                 c_char * 17) )
         plist.append( ('pad_xx',                    c_char * 51) )
         plist.append( ('rhi_image_uid',             c_char * 32) )
-
-
-
+    else:
+        raise UnknownPfile("Unfamiliar header revision: %0.3f" % (version,));
 
     return plist
         
 
-
-
-#        else if ( (int)(this->pfileVersion) == 26 ) {
-#
-#         offsets.assign (" \
-#             rhr.rh_rdbm_rev                    , FLOAT_4, 1   , 0,\
-#             rhr.rh_scan_date                   , CHAR   , 10  , 92,\
-#             rhr.rh_scan_time                   , CHAR   , 8   , 102,\
-#             rhr.rh_npasses                     , INT_2  , 1   , 140,\
-#             rhr.rh_nslices                     , UINT_2 , 1   , 144,\
-#             rhr.csi_dims                       , INT_2  , 1   , 436,\
-#             rhr.rh_dab[0].start_rcv            , INT_2  , 1   , 264,\
-#             rhr.rh_dab[0].stop_rcv             , INT_2  , 1   , 266,\
-#             rhr.rh_dab[1].start_rcv            , INT_2  , 1   , 268,\
-#             rhr.rh_dab[1].stop_rcv             , INT_2  , 1   , 270,\
-#             rhr.rh_dab[2].start_rcv            , INT_2  , 1   , 272,\
-#             rhr.rh_dab[2].stop_rcv             , INT_2  , 1   , 274,\
-#             rhr.rh_dab[3].start_rcv            , INT_2  , 1   , 276,\
-#             rhr.rh_dab[3].stop_rcv             , INT_2  , 1   , 278,\
-#             rhr.rh_data_collect_type           , INT_2  , 1   , 132,\
-#             rhr.rh_file_contents               , INT_2  , 1   , 120,\
-#             rhr.rdb_hdr_off_data               , INT_4  , 1   , 4,\
-#             rhr.rh_frame_size                  , UINT_2 , 1   , 156,\
-#             rhr.rh_point_size                  , INT_2  , 1   , 158,\
-#             rhr.rh_ps_mps_freq                 , UINT_4 , 1   , 488,\
-#             rhr.rh_user_usage_tag              , UINT_4 , 1   , 924,\
-#             rhr.roilenx                        , FLOAT_4, 1   , 444,\
-#             rhr.roileny                        , FLOAT_4, 1   , 448,\
-#             rhr.roilenz                        , FLOAT_4, 1   , 452,\
-#             rhr.spectral_width                 , FLOAT_4, 1   , 432,\
-#             rhr.xcsi                           , INT_2  , 1   , 438,\
-#             rhr.ycsi                           , INT_2  , 1   , 440,\
-#             rhr.zcsi                           , INT_2  , 1   , 442,\
-#             rhr.rh_logo                        , CHAR   , 10  , 110,\
-#             rhr.rh_raw_pass_size               , LINT_8 , 1   , 1540,\
-#             rhr.rh_user0                       , FLOAT_4, 1   , 280,\
-#             rhr.rh_user1                       , FLOAT_4, 1   , 284,\
-#             rhr.rh_user2                       , FLOAT_4, 1   , 288,\
-#             rhr.rh_user3                       , FLOAT_4, 1   , 292,\
-#             rhr.rh_user4                       , FLOAT_4, 1   , 296,\
-#             rhr.rh_user5                       , FLOAT_4, 1   , 300,\
-#             rhr.rh_user6                       , FLOAT_4, 1   , 304,\
-#             rhr.rh_user7                       , FLOAT_4, 1   , 308,\
-#             rhr.rh_user8                       , FLOAT_4, 1   , 312,\
-#             rhr.rh_user9                       , FLOAT_4, 1   , 316,\
-#             rhr.rh_user10                      , FLOAT_4, 1   , 320,\
-#             rhr.rh_user11                      , FLOAT_4, 1   , 324,\
-#             rhr.rh_user12                      , FLOAT_4, 1   , 328,\
-#             rhr.rh_user13                      , FLOAT_4, 1   , 332,\
-#             rhr.rh_user14                      , FLOAT_4, 1   , 336,\
-#             rhr.rh_user15                      , FLOAT_4, 1   , 340,\
-#             rhr.rh_user16                      , FLOAT_4, 1   , 344,\
-#             rhr.rh_user17                      , FLOAT_4, 1   , 348,\
-#             rhr.rh_user18                      , FLOAT_4, 1   , 352,\
-#             rhr.rh_user19                      , FLOAT_4, 1   , 356,\
-#             rhr.rh_user20                      , FLOAT_4, 1   , 936,\
-#             rhr.rh_user21                      , FLOAT_4, 1   , 940,\
-#             rhr.rh_user22                      , FLOAT_4, 1   , 944,\
-#             rhr.rh_user23                      , FLOAT_4, 1   , 948,\
-#             rhr.rh_user24                      , FLOAT_4, 1   , 952,\
-#             rhr.rh_user25                      , FLOAT_4, 1   , 956,\
-#             rhr.rh_user26                      , FLOAT_4, 1   , 960,\
-#             rhr.rh_user27                      , FLOAT_4, 1   , 964,\
-#             rhr.rh_user28                      , FLOAT_4, 1   , 968,\
-#             rhr.rh_user29                      , FLOAT_4, 1   , 972,\
-#             rhr.rh_user30                      , FLOAT_4, 1   , 976,\
-#             rhr.rh_user31                      , FLOAT_4, 1   , 980,\
-#             rhr.rh_user32                      , FLOAT_4, 1   , 984,\
-#             rhr.rh_user33                      , FLOAT_4, 1   , 988,\
-#             rhr.rh_user34                      , FLOAT_4, 1   , 992,\
-#             rhr.rh_user35                      , FLOAT_4, 1   , 996,\
-#             rhr.rh_user36                      , FLOAT_4, 1   , 1000,\
-#             rhr.rh_user37                      , FLOAT_4, 1   , 1004,\
-#             rhr.rh_user38                      , FLOAT_4, 1   , 1008,\
-#             rhr.rh_user39                      , FLOAT_4, 1   , 1012,\
-#             rhr.rh_user40                      , FLOAT_4, 1   , 1016,\
-#             rhr.rh_user41                      , FLOAT_4, 1   , 1020,\
-#             rhr.rh_user42                      , FLOAT_4, 1   , 1024,\
-#             rhr.rh_user43                      , FLOAT_4, 1   , 1028,\
-#             rhr.rh_user44                      , FLOAT_4, 1   , 1032,\
-#             rhr.rh_user45                      , FLOAT_4, 1   , 1036,\
-#             rhr.rh_user46                      , FLOAT_4, 1   , 1040,\
-#             rhr.rh_user47                      , FLOAT_4, 1   , 1044,\
-#             rhr.rh_user48                      , FLOAT_4, 1   , 1048,\
-#             rhi.psdname                        , CHAR   , 33  , 199812,\
-#             rhi.scanspacing                    , FLOAT_4, 1   , 198500,\
-#             rhi.te                             , INT_4  , 1   , 199244,\
-#             rhi.ti                             , INT_4  , 1   , 199240,\
-#             rhi.tr                             , INT_4  , 1   , 199236,\
-#             rhi.tlhc_A                         , FLOAT_4, 1   , 198904,\
-#             rhi.tlhc_R                         , FLOAT_4, 1   , 198900,\
-#             rhi.tlhc_S                         , FLOAT_4, 1   , 198908,\
-#             rhi.t                              , INT_4  , 1   , 199236,\
-#             rhi.trhc_A                         , FLOAT_4, 1   , 198916,\
-#             rhi.trhc_R                         , FLOAT_4, 1   , 198912,\
-#             rhi.trhc_S                         , FLOAT_4, 1   , 198920,\
-#             rhi.user0                          , FLOAT_4, 1   , 198536,\
-#             rhi.user1                          , FLOAT_4, 1   , 198540,\
-#             rhi.user2                          , FLOAT_4, 1   , 198544,\
-#             rhi.user3                          , FLOAT_4, 1   , 198548,\
-#             rhi.user4                          , FLOAT_4, 1   , 198552,\
-#             rhi.user5                          , FLOAT_4, 1   , 198556,\
-#             rhi.user6                          , FLOAT_4, 1   , 198560,\
-#             rhi.user7                          , FLOAT_4, 1   , 198564,\
-#             rhi.user8                          , FLOAT_4, 1   , 198568,\
-#             rhi.user9                          , FLOAT_4, 1   , 198572,\
-#             rhi.user10                         , FLOAT_4, 1   , 198576,\
-#             rhi.user11                         , FLOAT_4, 1   , 198580,\
-#             rhi.user12                         , FLOAT_4, 1   , 198584,\
-#             rhi.user13                         , FLOAT_4, 1   , 198588,\
-#             rhi.user14                         , FLOAT_4, 1   , 198592,\
-#             rhi.user15                         , FLOAT_4, 1   , 198596,\
-#             rhi.user16                         , FLOAT_4, 1   , 198600,\
-#             rhi.user17                         , FLOAT_4, 1   , 198604,\
-#             rhi.user18                         , FLOAT_4, 1   , 198608,\
-#             rhi.user19                         , FLOAT_4, 1   , 198612,\
-#             rhi.user20                         , FLOAT_4, 1   , 198616,\
-#             rhi.user21                         , FLOAT_4, 1   , 198620,\
-#             rhi.user22                         , FLOAT_4, 1   , 198624,\
-#             rhi.user23                         , FLOAT_4, 1   , 198636,\
-#             rhi.user24                         , FLOAT_4, 1   , 198640,\
-#             rhi.user25                         , FLOAT_4, 1   , 198704,\
-#             rhi.user26                         , FLOAT_4, 1   , 198708,\
-#             rhi.user27                         , FLOAT_4, 1   , 198712,\
-#             rhi.user28                         , FLOAT_4, 1   , 198716,\
-#             rhi.user29                         , FLOAT_4, 1   , 198720,\
-#             rhi.user30                         , FLOAT_4, 1   , 198724,\
-#             rhi.user31                         , FLOAT_4, 1   , 198728,\
-#             rhi.user32                         , FLOAT_4, 1   , 198732,\
-#             rhi.user33                         , FLOAT_4, 1   , 198736,\
-#             rhi.user34                         , FLOAT_4, 1   , 198740,\
-#             rhi.user35                         , FLOAT_4, 1   , 198744,\
-#             rhi.user36                         , FLOAT_4, 1   , 198748,\
-#             rhi.user37                         , FLOAT_4, 1   , 198752,\
-#             rhi.user38                         , FLOAT_4, 1   , 198756,\
-#             rhi.user39                         , FLOAT_4, 1   , 198760,\
-#             rhi.user40                         , FLOAT_4, 1   , 198764,\
-#             rhi.user41                         , FLOAT_4, 1   , 198768,\
-#             rhi.user42                         , FLOAT_4, 1   , 198772,\
-#             rhi.user43                         , FLOAT_4, 1   , 198776,\
-#             rhi.user44                         , FLOAT_4, 1   , 198780,\
-#             rhi.user45                         , FLOAT_4, 1   , 198784,\
-#             rhi.user46                         , FLOAT_4, 1   , 198788,\
-#             rhi.user47                         , FLOAT_4, 1   , 198792,\
-#             rhi.user48                         , FLOAT_4, 1   , 198796,\
-#             rhi.cname                          , CHAR   , 17  , 199929,\
-#             rhi.brhc_A                         , FLOAT_4, 1   , 198928,\
-#             rhi.brhc_R                         , FLOAT_4, 1   , 198924,\
-#             rhi.brhc_S                         , FLOAT_4, 1   , 198932,\
-#             rhi.ctr_A                          , FLOAT_4, 1   , 198880,\
-#             rhi.ctr_R                          , FLOAT_4, 1   , 198876,\
-#             rhi.ctr_S                          , FLOAT_4, 1   , 198884,\
-#             rhi.dfov                           , FLOAT_4, 1   , 198484,\
-#             rhi.freq_dir                       , INT_2  , 1   , 199680,\
-#             rhi.ctyp                           , INT_2  , 1   , 199614,\
-#             rhi.loc                            , FLOAT_4, 1   , 198504,\
-#             rhi.mr_flip                        , INT_2  , 1   , 199592,\
-#             rhi.nex                            , FLOAT_4, 1   , 198512,\
-#             rhi.numecho                        , INT_2  , 1   , 199558,\
-#             rhi.image_uid                      , UID    , 32  , 199997,\
-#             rhi.rawrunnum                      , INT_4  , 1   , 199288,\
-#             rhe.ex_datetime                    , INT_4  , 1   , 194240,\
-#             rhe.ex_no                          , UINT_2 , 1   , 194356,\
-#             rhe.magstrength                    , INT_4  , 1   , 194232,\
-#             rhe.patid                          , CHAR   , 65  , 195249,\
-#             rhe.patname                        , CHAR   , 65  , 195184,\
-#             rhe.refphy                         , CHAR   , 65  , 194717,\
-#             rhe.reqnum                         , CHAR   , 17  , 195314,\
-#             rhe.study_uid                      , UID    , 32  , 195088,\
-#             rhe.dateofbirth                    , CHAR   , 9   , 195331,\
-#             rhe.patsex                         , INT_2  , 1   , 194380,\
-#             rhe.hospname                       , CHAR   , 33  , 195011,\
-#             rhe.ex_sysid                       , CHAR   , 9   , 194980,\
-#             rhe.uniq_sys_id                    , CHAR   , 16  , 195052,\
-#             rhe.ex_verscre                     , CHAR   , 2   , 195048,\
-#             rhs.se_no                          , INT_4  , 1   , 196356,\
-#             rhs.se_desc                        , CHAR   , 65  , 196602,\
-#             rhs.entry                          , INT_4  , 1   , 196264,\
-#             rhs.position                       , INT_4  , 1   , 196260,\
-#             rhs.series_uid                     , UID    , 32  , 196765,\
-#             rhs.landmark_uid                   , UID    , 32  , 196797,\
-#             rhs.anref                          , CHAR   , 3   , 196685,\
-
-
 #----------------------------------------------------------
 # Test routines
 #----------------------------------------------------------
 
 
-
 def main():
 
-    # v16 data - 1 chan
-    fname = 'C:\\Users\\bsoher\\code\\repository_svn\\sample_data\\example_ge_svs_1ch_pom\\P29184.7'
-    
-    # v11 data - 8 chan
-#    fname = 'C:\\Users\\bsoher\\code\\repository_svn\\sample_data\\example_ge_pom_multi-channel\\P01024.7'
-
-    # v20 data - 32 chan
-#    fname = 'C:\\Users\\bsoher\\code\\repository_svn\\sample_data\\example_ge_svs_32ch_gregor\\P32256.7'
+    test_files=sys.argv[1:];
 
-    hdr = Pfile(fname)
-    hdr.dump_header()
+    print(test_files);
+    if len(test_files)==0:
+    	# v16 data - 1 chan
+        test_files.append('C:\\Users\\bsoher\\code\\repository_svn\\sample_data\\example_ge_svs_1ch_pom\\P29184.7');
+    
+    	# v11 data - 8 chan
+		# fname = 'C:\\Users\\bsoher\\code\\repository_svn\\sample_data\\example_ge_pom_multi-channel\\P01024.7'
 
-    bob = 10
-    bob += 1
+    	# v20 data - 32 chan
+		# fname = 'C:\\Users\\bsoher\\code\\repository_svn\\sample_data\\example_ge_svs_32ch_gregor\\P32256.7'
 
+    for fname in test_files:
+	    hdr = Pfile(fname)
+	    hdr.dump_header()
 
 
 
 if __name__ == '__main__':
 
     main()
```

## vespa/common/mrs_data_raw.py

```diff
@@ -469,14 +469,88 @@
 class DataRawEditFidsum(DataRawFidsum):
     """ This subclass serves to differentiate between edited and non-edited data """
     XML_VERSION = "1.0.0"
 
     def __init__(self, attributes=None, transform=None):
         super().__init__(attributes=attributes, transform=transform)
 
+    def concatenate(self, new, ignore_transform=False):
+        """
+        Given an DataRawEditFidsum instance, concatenates that instance's data
+        (and some metadata) onto this object. This object's zeroeth dimension
+        will increase by one. For instance, if self.dims was [1,1,1,4096]
+        before concatenation, it will be [2,1,1,4096] after.
+
+        This axis is concatenated under the assumption that there are multiple
+        FIDs being concatenated.
+
+        There are several conditions that must be met, otherwise this will
+        raise a ValueError.
+
+        1) This data must be single voxel or a stack of single voxels.
+           (i.e. 1st and 2nd dimension == 1)
+        2) The data to be concatenated must be single voxel or a stack of
+           single voxels. (i.e. 1st and 2nd dimension == 1)
+        3) The spectral dimension (dims[3]) must match.
+        4) The attributes data_type, sw, resppm, echopeak, and
+           nucleus must be the same on both DataRaw instances.
+
+        """
+        if len(new.data.shape) != 4:
+            raise ValueError("New data shape does not have 4 dimensions")
+
+        if max(self.data.shape[0:2]) > 1:
+            raise ValueError("Current data is not single voxel or a stack of single voxels")
+
+        if max(new.data.shape[0:2]) > 1:
+            raise ValueError("Data to be concatented is not single voxel or a stack of single voxels")
+
+        if new.data.shape[3] != self.data.shape[3]:
+            raise ValueError("Spectral dimension mismatch")
+
+        attribs = ("data_type", "resppm", "echopeak", "nucleus")
+        for attr in attribs:
+            if getattr(self, attr) != getattr(new, attr):
+                raise ValueError("""Attribute "%s" not equal"""%attr)
+
+        # Frequencies must be within +/- 1 Hz of one another.
+        if abs(abs(self.frequency)-abs(new.frequency)) > 1:
+            raise ValueError("""Frequencies not equal""")
+
+        # Sweep width must be within +/- 1 Hz of one another.
+        if abs(abs(self.sw)-abs(new.sw)) > 1:
+            raise ValueError("""Sweep widths not equal""")
+
+        if not ignore_transform:
+            # Transform must be within 1e-3 of one another
+            if not np.allclose(self.transform, new.transform, rtol=1e-03, atol=1e-04):
+                raise ValueError("""Transforms not equal (within tolerances)""")
+
+        # All is well, we can concatenate.
+        self.data_sources.extend(new.data_sources)
+        self.measure_time.extend(new.measure_time)
+        self.headers.extend(new.headers)
+
+        self.data = np.concatenate((self.data, new.data), axis=2)
+
     def deflate(self, flavor=Deflate.ETREE):
 
         if flavor == Deflate.ETREE:
             return super().deflate(flavor, tag='raw_edit_fidsum', version=self.XML_VERSION)
         elif flavor == Deflate.DICTIONARY:
             return self.__dict__.copy()
 
+
+class DataRawEdit(DataRaw):
+    """ subclass that exists to differentiate summed raw from summed edit FID data """
+    XML_VERSION = "1.0.0"
+
+    def __init__(self, attributes=None, transform=None):
+        super().__init__(attributes=attributes, transform=transform)
+
+    def deflate(self, flavor=Deflate.ETREE, tag='', version=''):
+
+        if flavor == Deflate.ETREE:
+            return super().deflate(flavor, tag='raw_edit', version=self.XML_VERSION)
+        elif flavor == Deflate.DICTIONARY:
+            return self.__dict__.copy()
+
```

## vespa/common/prefs.py

```diff
@@ -67,14 +67,15 @@
 
     In particular, each instance of a Prefs object has a number of 
     "automatic" attributes. These attrs are not explicitly enumerated in the
     class definition. Rather, they are created by inference at class 
     instantiation based on the names of the constants in one of the 
     util_menu.ViewIdXxxx classes.
     """
+    __metaclass__ = abc.ABCMeta
 
 
     def __init__(self, menu_bar, id_class):
         self._menu_bar = menu_bar
 
         # Determine the names of my auto attributes.
         self._auto_names = [name.lower() for name in id_class.BOOLEANS]
```

## vespa/common/rfp_pulse_design.py

```diff
@@ -38,15 +38,15 @@
 
         gyromagnetic_nuclei (str): default '1H'
 
         bloch_range_value (float): default 4.0, +/- width of x-axis displayed
             in the rf pulse plots. This can be in either kHz or cm units
             depending on the value in bloch_range_units attribute.
 
-        bloch_range_units (str): default 'cm', unit of the value in the
+        bloch_range_units (str): default 'kHz', unit of the value in the
             bloch_range_value attribute. Used together with the calc_resolution
             to calculate the point locations for the Bloch calculation.
 
         bloch_offset_value (float): default 0.0, offset frequency value used in
             the Bloch calculations.
 
         machine_specs (object): useful info about the MR scanner specifications
@@ -396,16 +396,16 @@
         """
 
         for transform in self.transforms:
             if transform.result:
                 outputs = {}
                 outputs['calc_resolution']     = self.calc_resolution
                 outputs['gyromagnetic_nuclei'] = self.gyromagnetic_nuclei
-                outputs['bloch_range_value']   = 25.0  #self.bloch_range_value
-                outputs['bloch_range_units']   = 'cm'  #self.bloch_range_units
+                outputs['bloch_range_value']   = self.bloch_range_value  #25.0
+                outputs['bloch_range_units']   = self.bloch_range_units  #'kHz' 
                 outputs['update_profiles']     = True
                 transform.result.update_profiles(outputs)
 
     
 
 # def _convert_project_to_design(db, rfpulse_project):
 #
```

## vespa/common/rfp_rf_result.py

```diff
@@ -116,32 +116,63 @@
         if self.gradient is None:
             return 10.0              # default is 10 mT/m == 1 gauss/cm
         else:
             ig = (np.nonzero(self.gradient))[0][0]  # first non-zero index
             return self.gradient[ig]                # return mT/m
 
       
-    def gradient_refocusing(self, val=None):
+    def gradient_refocusing(self, val, xunits, gamma):
         # This function calls a routine that may throw an exception of type
         #  PulseFuncException
-        
+
+        self.grad_refocus_fraction = val        # assume val if for kHz units xaxis
+
         profile, ax = self.get_profile(constants.UsageType.EXCITE)
-        
         length = len(self.rf_xaxis)
-        mpgpulms = 1000.0*(self.rf_xaxis[length-1]) + self.dwell_time/1000.0
-        
-        if val is None:        
-            try:
-                val = self.grad_refocus(ax, profile, mpgpulms)
-            except PulseFuncException:
-                val = 0.5 
-            pass
-    
+        pulse_dur_ms = 1000.0*(self.rf_xaxis[length-1]) + self.dwell_time/1000.0
+
+        gamma0 = gamma * 0.1                    # for 1H -> 4.2576 kHz/gauss
+        g0 = self.first_gradient_value * 0.1    # for gauss/cm
+        scale = gamma0 * g0                     # scaled for gradient
+
+        self.refocused_profile = np.exp(1j*2.0*math.pi*val * scale * ax*pulse_dur_ms)*profile
+
+        return val
+
+
+    def gradient_refocusing_auto(self, xunits, gamma):
+        # This automatically calculates a value for Gradient Refocus percentage
+        # It does it for an x-axis in kHz units, regardless of what the display
+        # in the GUI is set to.  The 'scale' keyword provides the conversion
+        # factor for cm to kHz if needed. It's set to 1.0 otherwise, no harm no
+        # foul.
+        #
+        # self.grad_refocus_fraction is always assumed to have been relevant to
+        # an x-axis in kHz units.
+        #
+        # This function calls a routine that may throw an exception of type
+        #  PulseFuncException
+
+        gamma0 = gamma * 0.1                    # for 1H -> 4.2576 kHz/gauss
+        g0 = self.first_gradient_value * 0.1    # for gauss/cm
+        scale = gamma0 * g0                     # scaled for gradient
+
+        profile, ax = self.get_profile(constants.UsageType.EXCITE)
+        length = len(self.rf_xaxis)
+        pulse_dur_ms = 1000.0 * (self.rf_xaxis[length - 1]) + self.dwell_time / 1000.0
+
+        try:
+            val = self.grad_refocus(ax, profile, pulse_dur_ms)
+            val = val / scale
+        except PulseFuncException:
+            val = 0.5
+            self.grad_refocus_fraction = val
+
+        self.refocused_profile = np.exp(1j*2.0*math.pi*val*ax * scale * pulse_dur_ms)*profile
         self.grad_refocus_fraction = val
-        self.refocused_profile = np.exp(1j*2.0*math.pi*val*ax*mpgpulms)*profile
 
         return val
 
     def interpolate(self, a, a0, a1, b0, b1):
         if not ((a0 <= a and a <= a1) or (a1 <= a and a <= a0)):
             error_message = 'Interpolation Failed. Target point is not between end points'
             raise PulseFuncException(error_message, 1)
@@ -257,15 +288,15 @@
         # - First zero-pad the profile (rpro)
         rpro = yprofile[ax1:ax2+1]
 
         nrpro = np.hstack( [ np.zeros(len(rpro)), rpro, np.zeros(len(rpro))] ) 
 
         fre0 = np.fft.fft(nrpro)
         length = len(fre0)
-        fre =  np.append(fre0[int(math.ceil(length/2)):], fre0[:int(math.ceil(length/2))])
+        fre =  np.append(fre0[int(math.ceil(length/2)):], fre0[:int(math.ceil(length/2))])    # this is a roll?
 
         # If two values in fre are the same in magnitude matlab actually looks 
         # at the phase and finds the one with the biggest phase, which we're 
         # not doing here. However, since we are using the first value in the
         # array that matches maxfre, fre_pos = np.nonzero(...), the phase thing 
         # is not and issue - according to Jerry.
         absfre = np.abs(fre)
@@ -344,15 +375,14 @@
         pa = np.polyfit(frot,carea,2)
         y = np.polyval(pa,frot)
 
         # This is the value considering areas
         frotn = -pa[1]/(2.0*pa[0])    
 
         # If p[0] > .001, or p[1]>.001, or niter > 19, iterations failed?
-        # :FIXME: Can frotn be greater than 1.0 ??? ask Jerry.
 
         if frotn < 0:
             error_message = 'Invalid Result: Fraction less than zero'
             raise PulseFuncException(error_message, 1)           
 
         return frotn
```

## vespa/common/twix_parser_multi_raid.py

```diff
@@ -265,14 +265,22 @@
         """
         Returns True if this scan is the last acquisition (which means it
         contains no FID), False otherwise.
         
         """
         return bool(self.test_eval_info_by_label("MDH_ACQEND"))
 
+    @property
+    def is_first_acquisition(self):
+        """
+        Returns True if this scan is the first acquisition (which means it
+        contains FID), False otherwise.
+
+        """
+        return bool(self.test_eval_info_by_label("MDH_FIRSTSCANINSLICE"))
 
     @property
     def clock_time(self):
         """
         Returns the scan's timestamp as a string representing the clock
         time when the scan was taken. The string is in ISO format and 
         includes microseconds -- HH:MM:SS,uSEC
@@ -780,40 +788,45 @@
         infile.seek(measurement_start + self.header_size, os.SEEK_SET)
 
 #        print 'after all evps = '+str(infile.tell())
 
         # Read the scans one by one until we hit the last (which should be flagged)
         # or run off the end of the file.
         scans = []
-        more_scans = True
+        more_scans = True       # if last scan, it has not data so don't save
+        save_scans = False      # don't save until 'MDH_FIRSTSCANINSLICE' flag is seen
         index = 0
         while more_scans:
             scan = TwixScan()
             scan.populate_from_file(infile)
             scan.scan_index = index
 
             if scan.scan_header.is_last_acquisition:
                 more_scans = False
-            else:
+            if scan.scan_header.is_first_acquisition:
+                # begin saving scans
+                save_scans = True
+
+            if save_scans and more_scans:
                 scans.append(scan)
 
                 # PS - I'm not sure if this is necessary. In the samples I have,
                 # the scan.scan_header.is_last_acquisition flag is set appropriately so I 
                 # never run off the end of the file.
                 if (infile.tell() - measurement_start) >= measurement_length:
                     more_scans = False
 
-            index += 1
+                index += 1
 
         self.scans = scans
         self.evps  = evps
         self.free_parameters = self.get_free_parameters()
         self.ice_parameters = self.get_ice_parameters()
 
-        self.indices_list   = self.create_ice_indices()
+        self.indices_list   = self.create_ice_indices()   # bjs TODO still out of sync with data array
         self.indices_unique = self.check_unique_indices()
         self.dims           = self.get_dims()
 
     ######## Sort functionality methods #######################################
     #
     # On successful return from populate_from_file() we automatically create a
     # list of all ICE dimensions for each scan and run a check on these dims to
@@ -863,16 +876,23 @@
 
         return dims
 
     def get_dims(self):
         """ return list of the max value in each dim, plus samples per scan """
 
         # transpose the list of lists and check max val in each dimension
+
+        if self.indices_list == []:   # TODO bjs, this is an empirical hack, check on reality
+            return []
+
         dims = [max(item) + 1 for item in zip(*self.indices_list)]
 
+        if len(self.scans) == 0:
+            return dims
+
         dims.append(self.scans[0].scan_header.used_channels)
         dims.append(self.scans[0].scan_header.samples_in_scan)
 
         return dims
 
     def check_unique_indices(self):
         """ uses set to determine if all ice dims are unique """
```

## vespa/common/wx_gravy/image_panel_toolbar.py

```diff
@@ -8,22 +8,16 @@
 custom icons is attached to the bottom that allow the user to pan, zoom,
 save figures, and undo/home the images in the axes. Note that standard
 settings are for multiple axes to be linked for pan/zoom operations.  
 
 Brian J. Soher, Duke University, April, 2014
 """
 # Python modules
-
 import os
 
-
-# Used to guarantee to use at least Wx2.8
-#import wxversion
-#wxversion.ensureMinimal('2.8')
-
 # third party modules
 import wx
 import numpy as np
 import matplotlib
 import matplotlib.cm as cm
 
 matplotlib.use('WXAgg')
```

## vespa/common/wx_gravy/plot_panel.py

```diff
@@ -550,15 +550,15 @@
 
     def on_middle_select(self, xstr, ystr, xend, yend, indx):
         """ placeholder, overload for user defined event handling """
         self._dprint('ext on_middle_select, X(str,end)='+str(xstr)+','+str(xend)+'  Y(str,end)='+str(ystr)+','+str(yend)+'  Index = '+str(indx))
         
     def on_middle_motion(self, xcur, ycur, xprev, yprev, indx):
         """ placeholder, overload for user defined event handling """
-        self._dprint('on_middle_move, X(cur,prev)='+str(xstr)+','+str(xprev)+'  Y(cur,prev)='+str(ystr)+','+str(yprev)+'  Index = '+str(indx))
+        self._dprint('on_middle_move, X(cur,prev)='+str(xcur)+','+str(xprev)+'  Y(cur,prev)='+str(ycur)+','+str(yprev)+'  Index = '+str(indx))
 
     def on_middle_press(self, xloc, yloc, indx, bounds=None, xdata=None, ydata=None):
         """ placeholder, overload for user defined event handling """
         self._dprint('on_middle_press, Xloc='+str(xloc)+'  Yloc='+str(yloc)+'  Index = '+str(indx))
         
 
 class ZoomSpan:
```

## vespa/common/wx_gravy/plot_panel_spectrum.py

```diff
@@ -815,14 +815,29 @@
         """ Return a copy of one and only one of the data sets. """
         if index < 0 or index >= self.naxes:
             return None
         else:
             return self.data[index][0]['data'].copy()
 
 
+    def set_data_direct(self, data, index):
+        """
+        Convenience function to simplify direct change to data arrays.
+        - data must be same shape and dtype as existing array
+        - index must be existing location
+        """
+        if index < 0 or index >= self.naxes:
+            return
+        if self.data[index][0]['data'].dtype != data.dtype:
+            return
+        if self.data[index][0]['data'].shape != data.shape:
+            return
+        self.data[index][0]['data'] = data
+
+
     def format_axes(self):
         """
         Here the plot_option settings are enforced for display of x-axis
         label, data_type (real/imag/magn) selection, display of zero line
         and position of zero line.
         
         """
```

## vespa/common/wx_gravy/widgets/floatspin/floatspin.py

```diff
@@ -1,34 +1,39 @@
 
 """\
 FloatSpin objects
 
-@copyright: 2016-2021     Brian J. Soher
+@copyright: 2016-2019     Brian J. Soher
 @license: MIT (see LICENSE.txt) - THIS PROGRAM COMES WITH NO WARRANTY
 """
 
 import wx
+
 from edit_windows import ManagedBase, EditStylesMixin
-import time
-import common, compat, misc
+from tree import Node
+import common, config, compat, misc
 import new_properties as np
 from collections import OrderedDict
 
 from wx.lib.agw.floatspin import FloatSpin, EVT_FLOATSPIN, FS_LEFT, FS_RIGHT, FS_CENTRE, FS_READONLY
 
 
 
 class EditFloatSpin(ManagedBase, EditStylesMixin):
-    """  Class to handle FloatSpin objects  """
-    WX_CLASS = 'FloatSpin'
+    """\
+    Class to handle FloatSpin objects
+    
+    """
     _PROPERTIES = ["Widget", "range", "value", "increment", "digits", "extrastyle", "style"]
     PROPERTIES = ManagedBase.PROPERTIES + _PROPERTIES + ManagedBase.EXTRA_PROPERTIES
 
-    def __init__(self, name, parent, index):
-        ManagedBase.__init__(self, name, parent, index)
+    def __init__(self, name, parent, id, sizer, pos):
+        
+        # Initialise parent classes
+        ManagedBase.__init__(self, name, 'FloatSpin', parent, id, sizer, pos)
         EditStylesMixin.__init__(self)
 
         # initialise instance properties
         self.range      = np.FloatRangePropertyA( "0.0, 100.0" )
         self.value      = np.SpinDoublePropertyA(0.0, val_range=(0.0,100.0), immediate=True, default_value=0.0)
         self.increment  = np.SpinDoublePropertyA(1.0, val_range=(0.0,100.0), immediate=True, default_value=1.0)
         self.digits     = np.SpinPropertyA(3, val_range=(0,20), immediate=True, default_value=3)
@@ -37,34 +42,33 @@
 
     def create_widget(self):
         mi,ma  = self.properties["range"].get_tuple()
         value  = self.properties["value"].get()
         incr   = self.properties["increment"].get()
         digits = self.properties["digits"].get()
         
-        self.widget = FloatSpin(self.parent_window.widget, wx.ID_ANY, min_val=mi, max_val=ma,
+        self.widget = FloatSpin(self.parent.widget, self.id, min_val=mi, max_val=ma,
                                 value=value, increment=incr, digits=digits)
     
 
-    def finish_widget_creation(self, level, sel_marker_parent=None):
-        ManagedBase.finish_widget_creation(self, level, sel_marker_parent)
+    def finish_widget_creation(self, sel_marker_parent=None, re_add=True):
+        ManagedBase.finish_widget_creation(self, sel_marker_parent, re_add)
         self.widget.Bind(wx.EVT_CHILD_FOCUS, self._on_set_focus)
         self.widget.Bind(wx.EVT_SET_FOCUS, self._on_set_focus)
         self.widget.Bind(wx.EVT_SPIN, self.on_set_focus)
 
 
     def _on_set_focus(self, event):
-        # within a short time window, we ignore focus events as these seem due losing focus
-        if not misc.focused_widget is self and time.time()-misc.focused_time > 0.05:
-            # don't set focused_widget during event, as this may cause crashes; use delay instead
+        # don't set focused_widget during event, as this may cause crashes
+        if not misc.focused_widget is self:
             misc.set_focused_widget(self, delayed=True)
         event.Skip()
 
 
-    def _properties_changed(self, modified, actions):  # from SpinCtrlDouble
+    def properties_changed(self, modified):  # from SpinCtrlDouble
 
         if not modified or "range" in modified and self.widget:
             mi,ma = self.properties["range"].get_tuple()
             self.widget.SetRange(mi, ma)
             self.properties["value"].set_range(mi,ma)
             self.properties["increment"].set_range(mi,ma)
 
@@ -87,16 +91,16 @@
                     value_p.set(ma)
                     value = ma
                 if self.widget:
                     self.widget.SetValue(value)
 
         # FS style changes do not need any action here
         
-        EditStylesMixin._properties_changed(self, modified, actions)
-        ManagedBase._properties_changed(self, modified, actions)
+        EditStylesMixin.properties_changed(self, modified)
+        ManagedBase.properties_changed(self, modified)
         
 
 # end of class EditFloatSpin
 
 
 class WidgetExtraStyleProperty(np.WidgetStyleProperty):
     # for Extra-Styles widget/settings for FloatSpin; e.g. FS_LEFT, FS_RIGHT, FS_CENTER,FS_READONLY
@@ -176,32 +180,52 @@
 
         self.update_display(True)
         for checkbox in self._choices:
             if checkbox is not None:
                 checkbox.Bind(wx.EVT_CHECKBOX, self.on_checkbox)     
 
 
-def builder(parent, index):
+def builder(parent, sizer, pos, number=[1]):
     """ factory function for EditFloatSpin objects.  """
-    name = parent.toplevel_parent.get_next_contained_name('float_spin_%d')
+    name = 'float_spin_%d' % number[0]
+    while common.app_tree.has_name(name):
+        number[0] += 1
+        name = 'float_spin_%d' % number[0]
+
     with parent.frozen():
-        editor = EditFloatSpin(name, parent, index)
-        editor.properties["style"].set_to_default()
-        editor.check_defaults()
-        if parent.widget: editor.create()
-    return editor
+        spin = EditFloatSpin(name, parent, wx.ID_ANY, sizer, pos)
+        spin.properties["style"].set_to_default()
+        spin.check_defaults()
+        node = Node(spin)
+        spin.node = node
+        if parent.widget: spin.create()
+    common.app_tree.insert(node, sizer.node, pos-1)
 
 
-def xml_builder(parser, base, name, parent, index):
+def xml_builder(attrs, parent, sizer, sizeritem, pos=None):
     """ factory function to build EditFloatSpin objects from a XML file """
-    editor = EditFloatSpin( name, parent, index)
-    editor.properties["value"].set_active(False)
-    return editor
+    from xml_parse import XmlParsingError
+    try:
+        name = attrs['name']
+    except KeyError:
+        raise XmlParsingError(_("'name' attribute missing"))
+    if sizer is None or sizeritem is None:
+        raise XmlParsingError(_("sizer or sizeritem object cannot be None"))
+
+    spin = EditFloatSpin( name, parent, wx.ID_ANY, sizer, pos )
+    spin.properties["value"].set_active(False)
+    node = Node(spin)
+    spin.node = node
+    if pos is None:
+        common.app_tree.add(node, sizer.node)
+    else:
+        common.app_tree.insert(node, sizer.node, pos-1)
+    return spin
 
 
 def initialize():
     """ initialization function for the module: returns a wxBitmapButton to be added to the main palette. """
     import os
-    common.widget_classes['EditFloatSpin'] = EditFloatSpin
     common.widgets['EditFloatSpin'] = builder
     common.widgets_from_xml['EditFloatSpin'] = xml_builder
-    return common.make_object_button('EditFloatSpin', os.path.join(os.path.dirname(__file__), 'floatspin.png'))
+
+    return common.make_object_button('EditFloatSpin', os.path.join(os.path.dirname(__file__), 'floatspin.xpm'))
```

## vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier.py

```diff
@@ -1,38 +1,40 @@
 
 """\
 FloatSpinMultiplier objects
 
-@copyright: 2016-2021     Brian J. Soher
+@copyright: 2016-2019     Brian J. Soher
 @license: MIT (see LICENSE.txt) - THIS PROGRAM COMES WITH NO WARRANTY
 """
 
 import wx
 
 from edit_windows import ManagedBase, EditStylesMixin
-import time
+from tree import Node
 import common, compat, config, misc
 import new_properties as np
 from collections import OrderedDict
 
 from wx.lib.agw.floatspin import FloatSpin, EVT_FLOATSPIN, FS_LEFT, FS_RIGHT, FS_CENTRE, FS_READONLY
-
 from .floatspin_multiplier_base import *
 
 
 
-
 class EditFloatSpinMultiplier(ManagedBase, EditStylesMixin):
-    """  Class to handle FloatSpinMultiplier objects  """
-    WX_CLASS = 'FloatSpinMultiplier'
+    """\
+    Class to handle FloatSpinMultiplier objects
+    
+    """
     _PROPERTIES = ["Widget", "range", "value", "increment", "digits", "extrastyle", "style"]
     PROPERTIES = ManagedBase.PROPERTIES + _PROPERTIES + ManagedBase.EXTRA_PROPERTIES
 
-    def __init__(self, name, parent, index):
-        ManagedBase.__init__(self, name, parent, index)
+    def __init__(self, name, parent, id, sizer, pos):
+
+        # Initialise parent classes
+        ManagedBase.__init__(self, name, 'FloatSpinMultiplier', parent, id, sizer, pos)
         EditStylesMixin.__init__(self)
 
         # initialise instance properties
         self.range      = np.FloatRangePropertyA( "0.0, 100.0" )
         self.value      = np.SpinDoublePropertyA(0.0, val_range=(0.0,100.0), immediate=True, default_value=0.0)
         self.multiplier = np.SpinDoublePropertyA(1.1, val_range=(0.0,100.0), immediate=True, default_value=1.0)
         self.digits     = np.SpinPropertyA(3, val_range=(0,20), immediate=True, default_value=3)
@@ -45,34 +47,33 @@
 
     def create_widget(self):
         mi,ma  = self.properties["range"].get_tuple()
         value  = self.properties["value"].get()
         mult   = self.properties["multiplier"].get()
         digits = self.properties["digits"].get()
         
-        self.widget = FloatSpinMultiplier(self.parent_window.widget, wx.ID_ANY, min_val=mi, max_val=ma,
+        self.widget = FloatSpinMultiplier(self.parent.widget, self.id, min_val=mi, max_val=ma,
                                           value=value, multiplier=mult, digits=digits)
 
 
-    def finish_widget_creation(self, level, sel_marker_parent=None):
-        ManagedBase.finish_widget_creation(self, level, sel_marker_parent)
+    def finish_widget_creation(self, sel_marker_parent=None, re_add=True):
+        ManagedBase.finish_widget_creation(self, sel_marker_parent, re_add)
         self.widget.Bind(wx.EVT_CHILD_FOCUS, self._on_set_focus)
         self.widget.Bind(wx.EVT_SET_FOCUS, self._on_set_focus)
         self.widget.Bind(wx.EVT_SPIN, self.on_set_focus)
 
 
     def _on_set_focus(self, event):
-        # within a short time window, we ignore focus events as these seem due losing focus
-        if not misc.focused_widget is self and time.time()-misc.focused_time > 0.05:
-            # don't set focused_widget during event, as this may cause crashes; use delay instead
+        # don't set focused_widget during event, as this may cause crashes
+        if not misc.focused_widget is self:
             misc.set_focused_widget(self, delayed=True)
         event.Skip()
 
 
-    def _properties_changed(self, modified, actions):  # from SpinCtrlDouble
+    def properties_changed(self, modified):  # from SpinCtrlDouble
 
         if not modified or "range" in modified and self.widget:
             mi,ma = self.properties["range"].get_tuple()
             self.widget.SetRange(mi, ma)
             self.properties["value"].set_range(mi,ma)
             self.properties["multiplier"].set_range(mi,ma)
 
@@ -95,16 +96,16 @@
                     value_p.set(ma)
                     value = ma
                 if self.widget:
                     self.widget.SetValue(value)
 
         # FS style changes do not need any action here
         
-        EditStylesMixin._properties_changed(self, modified, actions)
-        ManagedBase._properties_changed(self, modified, actions)
+        EditStylesMixin.properties_changed(self, modified)
+        ManagedBase.properties_changed(self, modified)
 
 # end of class EditFloatSpinMultiplier
 
 
 
 class WidgetExtraStyleProperty(np.WidgetStyleProperty):
     # for Extra-Styles widget/settings for FloatSpin; e.g. FS_LEFT, FS_RIGHT, FS_CENTER,FS_READONLY
@@ -184,34 +185,59 @@
 
         self.update_display(True)
         for checkbox in self._choices:
             if checkbox is not None:
                 checkbox.Bind(wx.EVT_CHECKBOX, self.on_checkbox)     
 
 
-def builder(parent, index):
-    """  factory function for EditFloatSpin objects.  """
-    name = parent.toplevel_parent.get_next_contained_name('float_spin_multiplier_%d')
+def builder(parent, sizer, pos, number=[1]):
+    """\
+    factory function for EditFloatSpin objects.
+    """
+    name = 'float_spin_multiplier_%d' % number[0]
+    while common.app_tree.has_name(name):
+        number[0] += 1
+        name = 'float_spin_multiplier_%d' % number[0]
+        
     with parent.frozen():
-        editor = EditFloatSpinMultiplier(name, parent, index)
-        editor.properties["style"].set_to_default()
-        editor.check_defaults()
-        if parent.widget: editor.create()
-    return editor
+        spin = EditFloatSpinMultiplier(name, parent, wx.ID_ANY, sizer, pos)
+        spin.properties["style"].set_to_default()
+        spin.check_defaults()
+        node = Node(spin)
+        spin.node = node
+        if parent.widget: spin.create()
+    common.app_tree.insert(node, sizer.node, pos - 1)
 
 
-def xml_builder(parser, base, name, parent, index):
+def xml_builder(attrs, parent, sizer, sizeritem, pos=None):
     """ factory function to build EditFloatSpinMultiplier objects from a XML file """
-    editor = EditFloatSpinMultiplier(name, parent, index)
-    editor.properties["value"].set_active(False)
-    return editor
+    from xml_parse import XmlParsingError
+    try:
+        name = attrs['name']
+    except KeyError:
+        raise XmlParsingError(_("'name' attribute missing"))
+    if sizer is None or sizeritem is None:
+        raise XmlParsingError(_("sizer or sizeritem object cannot be None"))
+
+    spin = EditFloatSpinMultiplier( name, parent, wx.ID_ANY, sizer, pos )
+    spin.properties["value"].set_active(False)
+    node = Node(spin)
+    spin.node = node
+    if pos is None:
+        common.app_tree.add(node, sizer.node)
+    else:
+        common.app_tree.insert(node, sizer.node, pos-1)
+    return spin
 
 
 def initialize():
-    """ initialization function for the module: returns a wxBitmapButton to be added to the main palette. """
+    """\
+    initialization function for the module: returns a wxBitmapButton to be
+    added to the main palette.
+    """
     import os
-    common.widget_classes['EditFloatSpinMultiplier'] = EditFloatSpinMultiplier
     common.widgets['EditFloatSpinMultiplier'] = builder
     common.widgets_from_xml['EditFloatSpinMultiplier'] = xml_builder
-    return common.make_object_button('EditFloatSpinMultiplier', os.path.join(os.path.dirname(__file__), 'floatspinmultiplier.png'))
+
+    return common.make_object_button('EditFloatSpinMultiplier', os.path.join(os.path.dirname(__file__), 'floatspinmultiplier.xpm'))
```

## vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier_base.py

```diff
@@ -1,14 +1,13 @@
 
 """\
 FloatSpinMultiplier objects
 
-@copyright: 2016-2021     Brian J. Soher
+@copyright: 2016-     Brian J. Soher
 @license: MIT (see LICENSE.txt) - THIS PROGRAM COMES WITH NO WARRANTY
-
 """
 
 import wx
 
 from wx.lib.agw.floatspin import FloatSpin, EVT_FLOATSPIN, FS_LEFT, FS_RIGHT, FS_CENTRE, FS_READONLY
```

## vespa/pulse/tab_transform.py

```diff
@@ -269,37 +269,34 @@
         """
         self._inner_notebook.run(self)
 
 
     def on_usage(self, event):
         
         use_type = self.ComboUsageType.GetStringSelection()
-
-# bjs-start - temporary comment out to do a release without Grad_Refocus
-
         use_type = constants.UsageType.get_type_for_value(use_type, 'display')
         
         if use_type == constants.UsageType.EXCITE:
             self.PanelGradRefocus.Show()
         else:
             self.PanelGradRefocus.Hide()
             self.CheckGradRefocus.SetValue(False)
         self.PanelLeftSide.Layout()
         self.PanelLeftSide.Refresh()        
         
         self.plot({'update_profiles':True, 'relim_flag':True})
-# bjs-end - temporary comment out to do a release without Grad_Refocus
 
 
     def on_bloch_range_value(self, event):
         val = self.FloatBlochRangeValue.GetValue()
         self.bloch_range_value = val
         self._inner_notebook.run(self)
         self._last_bloch_range_value = self.bloch_range_value
-    
+
+
     def on_bloch_range_units(self, event):
         unit = self.ComboBlochRangeUnits.GetStringSelection()
         if unit == self.bloch_range_units:
             return
         self.bloch_range_units = unit
 
         gamma = self._pulse_design.gyromagnetic_nuclei      # a string, e.g. '1H'
@@ -327,21 +324,49 @@
     def on_check(self, event):
         self.plot({})
 
 
     def on_check_grad_refocus(self, event):
         result = self.transform.result
         if result:
+            if self.CheckGradRefocus.GetValue():
+                gamma = constants.GAMMA_VALUES[self._pulse_design.gyromagnetic_nuclei]  # float MHz/T
+                grad_value = self.FloatGradRefocus.GetValue()
+                result.gradient_refocusing(grad_value, self.bloch_range_units, gamma)
+                self.profile_grad_refocus = result.refocused_profile
             self.plot({'update_profiles':True})
         
         
     def on_float_grad_refocus(self, event):
         result = self.transform.result
         if result: 
-            self.plot({'update_profiles':True, 'update_refocus':True})
+            if self.CheckGradRefocus.GetValue():
+                gamma = constants.GAMMA_VALUES[self._pulse_design.gyromagnetic_nuclei]  # float MHz/T
+                grad_value = self.FloatGradRefocus.GetValue()
+                result.gradient_refocusing(grad_value, self.bloch_range_units, gamma)
+                self.profile_grad_refocus = result.refocused_profile
+                self.plot({'update_profiles':True})
+
+
+    def on_grad_refocus_auto(self, event):
+        result = self.transform.result
+        if result:
+
+            if self.CheckGradRefocus.GetValue():
+                gamma = constants.GAMMA_VALUES[self._pulse_design.gyromagnetic_nuclei]  # float MHz/T
+                val = result.gradient_refocusing_auto(self.bloch_range_units, gamma)
+                if not np.isfinite(val):
+                    # algol failed - recalc grad_refocus profile for default val
+                    val = 0.5
+                    result.gradient_refocusing(val, self.bloch_range_units, gamma)
+
+                self.FloatGradRefocus.SetValue(val)
+                self.profile_grad_refocus = result.refocused_profile
+
+                self.plot({'update_profiles': True})
 
 
     def on_menu_view_option(self, event):
         event_id = event.GetId()
 
         if self._prefs.handle_event(event_id):
             if event_id == util_menu.ViewIds.ZERO_LINE_SHOW:
@@ -996,26 +1021,28 @@
         if not self.transform.result:
             grad_refocus_fraction = 0.0
         else:
             grad_refocus_fraction = self.transform.result.grad_refocus_fraction
 
         result = self.transform.result
         if result:
-            if grad_refocus_fraction == 0.0:
-                result.gradient_refocusing()
-                grad_refocus_fraction = result.grad_refocus_fraction
+            gamma = constants.GAMMA_VALUES[self._pulse_design.gyromagnetic_nuclei]  # float MHz/T
+            if grad_refocus_fraction != 0.0:
+                result.gradient_refocusing(grad_refocus_fraction, self.bloch_range_units, gamma)
             else:
-                result.gradient_refocusing(grad_refocus_fraction)
+                val = result.gradient_refocusing_auto(self.bloch_range_units, gamma)
+                self.FloatGradRefocus.SetValue(val)
             self.profile_grad_refocus = result.refocused_profile
 
+
         self.FloatGradRefocus.SetMinSize((75, -1))
         self.FloatGradRefocus.SetSize((75, -1))
         self.FloatGradRefocus.SetDigits(5)
         self.FloatGradRefocus.SetIncrement(0.0005)
-        self.FloatGradRefocus.SetRange(0.0, 1.0)
+        self.FloatGradRefocus.SetRange(0.0, 100.0)
         self.FloatGradRefocus.SetValue(grad_refocus_fraction)      
 
         self.PanelGradRefocus.Hide()
 
         # Gradient refocus widgets
 
         use_type = self.ComboUsageType.GetStringSelection()
@@ -1166,14 +1193,16 @@
                 
             outputs['calc_resolution']     = self._pulse_design.calc_resolution
             outputs['gyromagnetic_nuclei'] = self._pulse_design.gyromagnetic_nuclei
             outputs['bloch_range_value']   = self.bloch_range_value
             outputs['bloch_range_units']   = self.bloch_range_units
             outputs['bloch_offset_value']  = self.bloch_offset_value
             outputs['update_profiles']     = True
+            outputs['update_refocus']      = True
+
             result = self.transform.result
             
             if 'plot_method' in list(outputs.keys()) and 'update_method' in list(outputs.keys()):
                 # user kernel defined calls - might be contour or polar plot
                 plot   = getattr(self,   outputs['plot_method'], None)
                 update = getattr(result, outputs['update_method'], None)
                 if plot is not None and update is not None:
@@ -1200,47 +1229,47 @@
         select which ones to display in the figure. If "update_profiles" is
         True then we go through each axes, calculate the profile and extended
         profile based on the usage_type and then plot the real, imag and zero
         line into lines[0], [1] and [2] respectively. We then go through and
         make lines visible or not and xaxis on/off depending on prefs.
         
         '''
+        gamma0 = constants.GAMMA_VALUES[self._pulse_design.gyromagnetic_nuclei] # float MHz/T
+
         update_profiles = outputs["update_profiles"] if "update_profiles" in list(outputs.keys()) else False
         relim_flag      = outputs["relim_flag"]      if "relim_flag"      in list(outputs.keys()) else False
         update_refocus  = outputs["update_refocus"]  if "update_refocus"  in list(outputs.keys()) else False
         
         if not self.transform or not self.transform.result or (self.transform.result.rf_waveform is None):
             # Clear the plot.
             for axes in self.view.all_axes:
                 for line in axes.lines:
                     line.set_visible(False)
                 axes.xaxis.set_visible(False)
     
             self.view.canvas.draw()
             return
-        
+
+        if self.CheckGradRefocus.GetValue() and update_refocus:
+            grad_value = self.FloatGradRefocus.GetValue()
+            self.transform.result.gradient_refocusing(grad_value, self.bloch_range_units, gamma0)
+            self.profile_grad_refocus = self.transform.result.refocused_profile
+
         checks = []
         checks.append(self.CheckProfile.IsChecked())
         checks.append(self.CheckAbsolute.IsChecked()) 
         checks.append(self.CheckProfileExtended.IsChecked())
         checks.append(self.CheckAbsoluteExtended.IsChecked())
         checks.append(self.CheckGradient.IsChecked())
         checks.append(self.CheckWaveform.IsChecked())
         checks.append(self.CheckWaveformMagn.IsChecked())
         checks.append(self.CheckWaveformPhase.IsChecked())
 #        checks.append(self.CheckContour.IsChecked())
         checks.append(self.CheckGradRefocus.IsChecked())
-        # tell the view which plot axes to include in the figure
-        self.view.display_naxes(checks)
-        naxes = len(self.view.figure.axes) 
-        
-        if naxes == 0: return
-        
-        fsize = ['medium','medium','small','small','x-small','x-small','x-small','x-small','x-small']
-        fsize = fsize[naxes-1]
+
         use_type = self.ComboUsageType.GetStringSelection()
         use_type = constants.UsageType.get_type_for_value(use_type, 'display')
 
         if update_profiles != False or self.profile == None or self.profile_ext == None:
             result = self.transform.result
             self.profile     = result.get_profile(use_type, False, False)
             self.profile_ext = result.get_profile(use_type, True, False)
@@ -1249,44 +1278,19 @@
 
         if self.bloch_range_units == 'cm':
             cm2khz = 1.0
         else:
             # Units are in kHz, but remember any gradient other than the
             # default 1g/cm will shove more kHz/cm (or less), so gradient
             # strength has to be part of this calculation.
-            gamma0 = constants.GAMMA_VALUES[self._pulse_design.gyromagnetic_nuclei]           # float MHz/T
             gamma = gamma0 * 0.1                      # for 1H -> 4.2576 kHz/gauss
             g0 = result.first_gradient_value * 0.1    # for gauss/cm
             cm2khz = gamma * g0                       # scaled for gradient
 
-        if self.CheckGradRefocus.GetValue():
-            grad_value = self.FloatGradRefocus.GetValue()
-            if grad_value == 0.0:
-                # request for auto-calculate refocus percentile
-                result.gradient_refocusing()
-                if not np.isfinite(result.grad_refocus_fraction):
-                    # algol failed - recalc grad_refocus profile for default val
-                    val = 0.5
-                    result.gradient_refocusing(val * cm2khz)
-                else:
-                    # algo worked
-                    val = result.grad_refocus_fraction / cm2khz
-                self.FloatGradRefocus.SetValue(val)
-            else:
-                # user provided a value
-                result.gradient_refocusing(grad_value * cm2khz)
-            self.profile_grad_refocus = result.refocused_profile
-        else:
-             self.profile_grad_refocus = self.profile[0] * 0.0
-
-        # :FIXME: For the next 4 plots .. Will these
-        # always be in Frequency or will we allow it 
-        # in spatial coordinates (e.g. millimeters).
-
-        # Frequency Profile  
+        # Frequency Profile
         fy, fx = self.profile
         fx0 = np.array(fx) * cm2khz
         fx1 = np.array(fx) * cm2khz
         fy0 = np.array([i.real for i in fy])            
         fy1 = np.array([i.imag for i in fy])
         axes = self.view.all_axes[0]
         axes.lines[0].set_xdata(fx0)
@@ -1385,23 +1389,37 @@
 #             fy, fx = self.profile
 #             axes = self.view.all_axes[8]
 #             axes.lines[0].set_xdata(np.array(fx))
 #             axes.lines[0].set_ydata(np.array([i.real for i in fy]))
 #             axes.lines[1].set_xdata(np.array(fx))
 #             axes.lines[1].set_ydata(np.array([i.imag for i in fy]))
 
-        # Grad Refocused Profile  
+        # Grad Refocused Profile
         fy = self.profile_grad_refocus
         _, fx = self.profile
         axes = self.view.all_axes[8]
         axes.lines[0].set_xdata(np.array(fx * cm2khz))
         axes.lines[0].set_ydata(np.array([i.real for i in fy]))
         axes.lines[1].set_xdata(np.array(fx * cm2khz))
         axes.lines[1].set_ydata(np.array([i.imag for i in fy]))
 
+        # NB. bjs - moved next 6 lines here as workaround for display bug
+        # where GradRefocus plot first check crashed program. This was after
+        # I changed default units to kHz. Still not sure why, but some sort
+        # of 'broadcast' error in canvas.show() call? fsize move was due to
+        # dependency on naxes.
+
+        # tell the view which plot axes to include in the figure
+        self.view.display_naxes(checks)
+        naxes = len(self.view.figure.axes)
+        if naxes == 0: return
+
+        fsize = ['medium', 'medium', 'small', 'small', 'x-small', 'x-small', 'x-small', 'x-small', 'x-small']
+        fsize = fsize[naxes - 1]
+
         for i in range(9):
             self.format_plot(self.view.all_axes[i], i, use_type,  fsize)
             
         for i, axes in enumerate(self.view.all_axes):
             if self._prefs.data_type_real:
                 axes.lines[0].set_visible(True)
                 axes.lines[1].set_visible(False)
@@ -1411,15 +1429,15 @@
                     axes.lines[1].set_visible(True)
             axes.lines[2].set_visible(self._prefs.zero_line_show)
             axes.xaxis.set_visible(self._prefs.xaxis_show)
 
         for i, axes in enumerate(self.view.figure.axes):
             axes.change_geometry(naxes,1,i+1)
 
-        if relim_flag or update_profiles and not update_refocus:
+        if relim_flag or update_profiles:  # and not update_refocus:
             # here we bump out the viewing window a bit on the
             # overall plot so we can get a zoom box around the
             # all sides of the plotted data
             for axes in self.view.all_axes:
                 # first calculate the tight bounds for data
                 x  = axes.lines[0].get_xdata()
                 y0 = axes.lines[0].get_ydata()
```

## vespa/pulse/auto_gui/panel_tab_transform.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# generated by wxGlade 0.9.3 on Wed Sep 11 13:06:23 2019
+# generated by wxGlade 0.9.3 on Thu May  4 10:39:06 2023
 #
 
 import wx
 from wx.lib.agw.floatspin import FloatSpin, EVT_FLOATSPIN, FS_LEFT, FS_RIGHT, FS_CENTRE, FS_READONLY
 
 # begin wxGlade: dependencies
 # end wxGlade
@@ -34,16 +34,17 @@
         self.CheckProfileExtended = wx.CheckBox(self.PanelControls1D, wx.ID_ANY, "Ext Profile")
         self.CheckAbsoluteExtended = wx.CheckBox(self.PanelControls1D, wx.ID_ANY, "Ext-Abs Profile  ")
         self.CheckWaveformMagn = wx.CheckBox(self.PanelControls1D, wx.ID_ANY, "RF [Magn]")
         self.CheckWaveformPhase = wx.CheckBox(self.PanelControls1D, wx.ID_ANY, "RF [deg]")
         self.CheckWaveform = wx.CheckBox(self.PanelControls1D, wx.ID_ANY, "RF [re/im]")
         self.ComboUsageType = wx.ComboBox(self.PanelControls1D, wx.ID_ANY, choices=["Excite", "Inversion", "Spin-Echo Echo Echo", "Saturation"], style=wx.CB_DROPDOWN | wx.CB_READONLY | wx.CB_SIMPLE)
         self.PanelGradRefocus = wx.Panel(self.PanelControls1D, wx.ID_ANY)
-        self.CheckGradRefocus = wx.CheckBox(self.PanelGradRefocus, wx.ID_ANY, "Grad Refoc Profile    Grad Value:")
+        self.CheckGradRefocus = wx.CheckBox(self.PanelGradRefocus, wx.ID_ANY, "Grad Refoc Profile - Grad Value:")
         self.FloatGradRefocus = FloatSpin(self.PanelGradRefocus, wx.ID_ANY, value=0.5, digits=5, min_val=0.0, max_val=100.0, increment=1.0, agwStyle=FS_LEFT, style=0)
+        self.ButtonGradRefocusAuto = wx.Button(self.PanelGradRefocus, wx.ID_ANY, "Auto", style=wx.BU_EXACTFIT)
         self.window_1_pane_results = wx.Panel(self.window_splitter, wx.ID_ANY)
         self.PanelView2D = wx.Panel(self.window_1_pane_results, wx.ID_ANY)
         self.PanelView1D = wx.Panel(self.window_1_pane_results, wx.ID_ANY)
 
         self.__set_properties()
         self.__do_layout()
 
@@ -58,14 +59,15 @@
         self.Bind(wx.EVT_CHECKBOX, self.on_check, self.CheckAbsoluteExtended)
         self.Bind(wx.EVT_CHECKBOX, self.on_check, self.CheckWaveformMagn)
         self.Bind(wx.EVT_CHECKBOX, self.on_check, self.CheckWaveformPhase)
         self.Bind(wx.EVT_CHECKBOX, self.on_check, self.CheckWaveform)
         self.Bind(wx.EVT_COMBOBOX, self.on_usage, self.ComboUsageType)
         self.Bind(wx.EVT_CHECKBOX, self.on_check_grad_refocus, self.CheckGradRefocus)
         self.Bind( EVT_FLOATSPIN, self.on_float_grad_refocus, self.FloatGradRefocus)
+        self.Bind(wx.EVT_BUTTON, self.on_grad_refocus_auto, self.ButtonGradRefocusAuto)
         # end wxGlade
 
     def __set_properties(self):
         # begin wxGlade: PanelTabTransform.__set_properties
         self.ComboBlochRangeUnits.SetSelection(1)
         self.ComboUsageType.SetMinSize((100, 21))
         self.ComboUsageType.SetSelection(1)
@@ -120,14 +122,15 @@
         label_2 = wx.StaticText(self.PanelControls1D, wx.ID_ANY, "Usage Type: ", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(label_2, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.ALL, 4)
         grid_sizer_1.Add(self.ComboUsageType, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 2)
         grid_sizer_1.Add((20, 20), 0, 0, 0)
         sizer_9.Add(grid_sizer_1, 1, wx.EXPAND, 0)
         sizer_6.Add(self.CheckGradRefocus, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 4)
         sizer_6.Add(self.FloatGradRefocus, 0, wx.EXPAND, 0)
+        sizer_6.Add(self.ButtonGradRefocusAuto, 0, wx.ALIGN_CENTER_VERTICAL | wx.LEFT, 4)
         self.PanelGradRefocus.SetSizer(sizer_6)
         sizer_9.Add(self.PanelGradRefocus, 0, wx.EXPAND, 0)
         sizer_11.Add(sizer_9, 0, wx.ALL | wx.EXPAND, 6)
         self.PanelControls1D.SetSizer(sizer_11)
         sizer_5.Add(self.PanelControls1D, 0, wx.EXPAND, 0)
         self.PanelLeftSide.SetSizer(sizer_5)
         sizer_12.Add(self.PanelView2D, 1, wx.EXPAND, 0)
@@ -168,14 +171,18 @@
         print("Event handler 'on_check_grad_refocus' not implemented!")
         event.Skip()
 
     def on_float_grad_refocus(self, event):  # wxGlade: PanelTabTransform.<event_handler>
         print("Event handler 'on_float_grad_refocus' not implemented!")
         event.Skip()
 
+    def on_grad_refocus_auto(self, event):  # wxGlade: PanelTabTransform.<event_handler>
+        print("Event handler 'on_grad_refocus_auto' not implemented!")
+        event.Skip()
+
 # end of class PanelTabTransform
 
 class MyFrame(wx.Frame):
     def __init__(self, *args, **kwds):
         # begin wxGlade: MyFrame.__init__
         kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_FRAME_STYLE
         wx.Frame.__init__(self, *args, **kwds)
```

## Comparing `Vespa_Suite-1.0.2.dist-info/LICENSE` & `Vespa_Suite-1.1.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Vespa_Suite-1.0.2.dist-info/METADATA` & `Vespa_Suite-1.1.0rc1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Vespa-Suite
-Version: 1.0.2
+Version: 1.1.0rc1
 Summary: Vespa is a suite of inter-connnected applications for magnetic resonance spectroscopy simulation and data analysis.
 Home-page: https://github.com/vespa-mrs/vespa/
 Maintainer: Dr. Brian J. Soher
 Maintainer-email: bsoher@briansoher.com
 License: http://creativecommons.org/licenses/BSD/
 Keywords: mri,mrs,pygamma,spectral simulation,rf pulses,magnetic resonance spectroscopy,fitting,time domain,frequency domain
 Platform: Linux
```

## Comparing `Vespa_Suite-1.0.2.dist-info/RECORD` & `Vespa_Suite-1.1.0rc1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 vespa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/check_dependencies.py,sha256=rfEBOMaZp-Xy_lBFKADBqp1JreIX2qLgNvD6qF1-3-8,8316
 vespa/create_shortcuts.py,sha256=o_h6a0j7jtEopzHrzNbs69yTq5XFupjxgTn0tmdGFSA,6021
 vespa/requirements.txt,sha256=lqAIfxjo2q-Y5CO4403kuO_nRpx_fjpAlQsECK6mOrQ,1853
 vespa/analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/analysis/block.py,sha256=xJ78fdHii-eaaO87ctjrDT5eEwOiKP5tjtgL1DHFaKM,2824
-vespa/analysis/block_fit_giso.py,sha256=XXZZ2IS9cQ3vCOxftFGp4-OVMahK_s5wKFUxyXmTNhY,54813
+vespa/analysis/block_fit_giso.py,sha256=4jx4LJH2jM8ylLcvLWZcgmajFPGkaTPulwvUwWist6I,53457
+vespa/analysis/block_fit_giso_Last.py,sha256=XXZZ2IS9cQ3vCOxftFGp4-OVMahK_s5wKFUxyXmTNhY,54813
 vespa/analysis/block_fit_identity.py,sha256=-BIt_5zz7aqQHEQ-biG9FjCeiJuMBEwiZvz_WqDFWDw,2948
+vespa/analysis/block_fit_voigt - Copy.py,sha256=vn5d5Tdm5OL7VjLHvjENkxMFeJ3k8j5Fgx3N30ZZtAo,40393
 vespa/analysis/block_fit_voigt.py,sha256=vn5d5Tdm5OL7VjLHvjENkxMFeJ3k8j5Fgx3N30ZZtAo,40393
 vespa/analysis/block_prep_edit_fidsum.py,sha256=WCyNrtIsPCcrEoq9duNBjbXKGs7LFdRI6QQwUhrk5AI,1620
 vespa/analysis/block_prep_fidsum.py,sha256=z9wPI_3OCKhqnWaw3xcysYu_LZL6yJqbtH7QfID4isU,28301
 vespa/analysis/block_prep_identity.py,sha256=i7kAOqBtZfuffDAciNJUp3lpGKqiqqensR2qQm5KwwA,2814
 vespa/analysis/block_prep_megalaser.py,sha256=fTEg9Fiup3TS92zcMQJLg6NVR60gZ2BgxKKq0jXTISg,11384
 vespa/analysis/block_prep_timeseries.py,sha256=SY8YUbRLNexECVsWExeQuWP4S2a_mA7L5R3sbISSTQE,14223
 vespa/analysis/block_prep_wbnaa.py,sha256=RV-mZitTKtxlOc-KTUX-gsiRAILx5tcnYATjHmdU7B8,14072
 vespa/analysis/block_quant_identity.py,sha256=COy-A9I6HGIsd0VMYhdrbkjkXQZB_ARaY96t22wqEF4,2800
 vespa/analysis/block_quant_watref.py,sha256=NUe3cW0-D1Ys7KRhb0OtQC_1D_Rva26t5bp4XvcDxsg,16636
 vespa/analysis/block_raw.py,sha256=DeHDZ3cTsSsm2ZmmqFI_eE2239praOiISQGzF8vf_O8,4255
 vespa/analysis/block_raw_cmrr_slaser.py,sha256=1FXl2PPBSAbBdOBgZx94IzyAkCZmfe6hUe5aVn1tV84,9535
-vespa/analysis/block_raw_edit_fidsum.py,sha256=Av7_8xID2EVsg7avuy4tS6ZCPNzmwlFCxpY4pdQjeRI,6801
-vespa/analysis/block_raw_probep.py,sha256=L7gp-9lH0Mo11Othj3o7cfS152xz_Y7HX9ll4wh6x3Q,4246
+vespa/analysis/block_raw_edit.py,sha256=Y9_6vNIA-JLGGRW7Su2yZgPFPWq0ViCRcCYOr457ScA,9115
+vespa/analysis/block_raw_edit_fidsum.py,sha256=zctV0r_WwQ6O1cqobLug8mJGOA3gVyRzygWaXnfmMfE,9265
+vespa/analysis/block_raw_probep.py,sha256=4Ch1H0YyWzr5T_53Rz1pPYYMw2k6jnpqaahPQBo2BGM,4265
 vespa/analysis/block_spectral.py,sha256=GrXvHxIaUxZZhTMBG5G0hYXbXGjsKajcMiHRt38VjZk,39995
 vespa/analysis/block_spectral_identity.py,sha256=yhSxUgC-Gusr3DOCMEdiUoQJ38_s9SkEkLZAvQU7lA4,2844
 vespa/analysis/chain_base.py,sha256=ttJxzO8CntONDRklqDPdnUJVFlNqqn5lpUMFlLB7OJ4,1326
 vespa/analysis/chain_fit_giso.py,sha256=t01nA-7WZ47N1mw6uHF11MVdk7-gBY9oK64gcIQgFSc,20823
 vespa/analysis/chain_fit_identity.py,sha256=oglp-ugiWOFb1jC1Z--kVvfclqgI_SbanjmMqX0B1DM,474
 vespa/analysis/chain_fit_voigt.py,sha256=87CXIoCWtkpi05pp3vlFpxTC6QKtegf0iEZCjgz6H1s,38831
 vespa/analysis/chain_prep_fidsum.py,sha256=b6P8vPnMUZUj7LWWivH53PjdybAaM6SkuYj0Mg9ldHk,7370
@@ -31,65 +34,65 @@
 vespa/analysis/chain_prep_timeseries.py,sha256=l7Me0ESJJKE-mRMpXkmQcMfA4NpORDXZDvJEs7Z_QMU,3169
 vespa/analysis/chain_prep_wbnaa.py,sha256=QJNSMWtb6zWgSu_cAq02HrXb532vdkbUuc3zjB8p-44,3067
 vespa/analysis/chain_quant_identity.py,sha256=qMejG-ZnVZbjftVtJe4zIYwLKxnnUTD7rnj7ZRZx7Qg,476
 vespa/analysis/chain_quant_watref.py,sha256=dW1xD9IdWjyxUApnmRXJ4tp2ppF_ikla8WcGJyOVbLA,5660
 vespa/analysis/chain_raw.py,sha256=X6nyc5kjCEZVd2yJTKYfLNSLx6RXofzsGr2BhG-Mmsg,632
 vespa/analysis/chain_spectral.py,sha256=PIhQlA90eurJMRTQ997pm0erd9-pkPGG8Qvyo57XO7s,5420
 vespa/analysis/chain_spectral_identity.py,sha256=sxxhQ_cMKZH5qsIVk2zImziTP74InF5Gtwy-Xm87XRs,489
-vespa/analysis/constants.py,sha256=xZ-KGYucydu3T77kEkaAQamhMptZAyQR29GQhfgl44o,26640
+vespa/analysis/constants.py,sha256=UbXvKi-BtZmA7aC36N3PuLIUQziZ-e__JbjUY7mL0Nk,26649
 vespa/analysis/deprecated_dynamic_list_user_prior.py,sha256=jO1Pgs5Sp4MxvNTMR30jM3xsbxkrMabOemK2QYUp95s,6119
 vespa/analysis/dialog_dataset_browser.py,sha256=dvH10Val0qHsl6WykuOnQAeUQ4TiarYGxZSwCkQ6VHQ,7091
 vespa/analysis/dialog_experiment_indices.py,sha256=fU7sCF9f3RIhQaE2iAdRZTzO88Z2q-9xmHYwCSc2NL4,10805
 vespa/analysis/dialog_user_defined_metabolite.py,sha256=M8sltgWYhhHP1vg5gWlgBKw_OU0chzpoZWbXEahGfBI,23643
 vespa/analysis/dialog_user_defined_prior.py,sha256=h8fkPhhNiaXANNDB3T9R5RSSBAd4xfvpH2YMujEwZuU,31127
 vespa/analysis/dialog_user_metabolite_info.py,sha256=eXf96rKLy3lPBnkTn2Ezq0eotDQ8wr2Oi55jr_U5IaY,13767
 vespa/analysis/dialog_user_prior.py,sha256=sERk5YMp5v_StZ7dL1xP4MDwFpKUwPVqJDNzqYhH5Gw,19804
 vespa/analysis/dynamic_list_giso_metabolite.py,sha256=hmweyFye5zfR6RrRyP5rpyBwf78xf3Fy1sHsfF7Rd4I,11637
 vespa/analysis/dynamic_list_voigt_metabolite.py,sha256=UvOdumPHvsqyBsGF8a6GA0mbDgV1JRMyi0Xns8zKN38,11659
 vespa/analysis/figure_layouts.py,sha256=JYQfeICInZKCSocBGV2WB5wezhkGr5-2sTlv-9wFelA,107792
 vespa/analysis/liver31p_series_sorter.py,sha256=cZxuEIUDe5tBhxHOeD26pRN5J0K0L_IFY4QQSdE6Ypc,6983
-vespa/analysis/main.py,sha256=myam0OyYAxRv38huU0oKQ2Rgaq2tLTpLuZ8LaTAQguE,32510
-vespa/analysis/mrs_dataset.py,sha256=M2RdpJrehkxHx9TwxN4sBBLkl0GNyPM48LcEfCRJkr8,102829
+vespa/analysis/main.py,sha256=W3XtLunUDHlH8SAReRsAmEbDNi4w5bS8ofSwD6FoBaU,33195
+vespa/analysis/mrs_dataset.py,sha256=X3QP9PWSDOQalAEcimNFoepJ238sFhjejCA5IXAgRy0,103551
 vespa/analysis/mrs_macromolecule.py,sha256=p562nkXM-OwNwswfrfILayNy_-v9A45zHrbV_ast8yA,4256
 vespa/analysis/mrs_metinfo.py,sha256=nA8g97dkBoIZIwSMpwzHqjHhBg7LIHWqe4qCam1aTrw,18240
 vespa/analysis/mrs_user_prior.py,sha256=7ZjUlkguxErN6H-p1DPS9HOSn1un_k-v96nwHuj4GcQ,4516
 vespa/analysis/mrs_user_prior_spectrum.py,sha256=V9z18YrnB613zP-VhfUaEdbb-jDV2rtvlsjhT1PSkgU,5345
-vespa/analysis/notebook_datasets.py,sha256=EUeeqMromAZ21w2n6pLQ-sCQ9_ileoxZ2SPbFArdGMU,28391
+vespa/analysis/notebook_datasets.py,sha256=bh6Tsrfe4IVQA8HzUj36dck_ZYiKuuVRiAscFrufhGM,30137
 vespa/analysis/plot_panel_giso.py,sha256=RYW3J0ZQwDkaeLbzzBKLcYB0z95KAUUYAPcPjjXB5EM,10386
 vespa/analysis/plot_panel_prep_fidsum.py,sha256=dX-tt1tLs28vt2lABmE-txghchxlG8v2yx15Pz0kHqU,14377
 vespa/analysis/plot_panel_prep_megalaser.py,sha256=UKzZeXOb6jF3JJWGxuVTtO_aEdgXz_x5laxktK6WXKw,6691
 vespa/analysis/plot_panel_prep_timeseries.py,sha256=nq5Kuh_BXZR6RlF5eEuZ6JwLSmvpxtWpqRzk_IGvBRw,7084
 vespa/analysis/plot_panel_prep_wbnaa.py,sha256=6GVBvAO5ir86P45R7Su8BI8r8fDzKVUxdW8xoyexSCg,11940
 vespa/analysis/plot_panel_spectral.py,sha256=byGWWs4VV92wPZv_M4oIpG7VrRCPryidywCpCliAFz0,10050
 vespa/analysis/plot_panel_svd_filter.py,sha256=hfDf_o8lOPSy7_e0H10QtQRgRrNudlOZqIQPqjTdeNU,9383
 vespa/analysis/plot_panel_user_defined_metabolite.py,sha256=dRrCCCVIy4LmHpaVYrxscH81ctTxDmnJRmZorLLqa9I,4966
 vespa/analysis/plot_panel_user_prior.py,sha256=6Ni8NgvVzS3I8gWzhq80HI23Frmo_tCOMexSU_Om6IQ,5020
 vespa/analysis/plot_panel_voigt.py,sha256=uA2_FR5j3sAxdZPoEoyRwVa4TGHnTdS1W2GFPrIRw1Q,10463
 vespa/analysis/plot_panel_watref.py,sha256=h4aTHHHguoLE2sFc6qN2vWVBuwC5eDcrrpt7t5XCqdU,9969
 vespa/analysis/prefs.py,sha256=IZUmPt_2cijFSW-Z6a3OsP-wW0PXZ9WyKaeCTsn9Plw,14386
 vespa/analysis/svd_output.py,sha256=ekoUubskfcv5-Rogfc5iuxIXRY9Gadrrlu6HcRV7CVQ,4112
 vespa/analysis/tab_base.py,sha256=OyHeJwGiFqGjhzf1nnZZT6xS6v6wN5_mle6DzJXGbww,4581
-vespa/analysis/tab_dataset.py,sha256=Mo717ZPUBlsGy3LrXl8gTBJZLx_gNr3m8Z6LY8xIRhQ,28549
+vespa/analysis/tab_dataset.py,sha256=yFpfLCpI0R0e-QGd5ttBSLcdzmih-P_0oK3X4t_CASg,28792
 vespa/analysis/tab_giso.py,sha256=nBvkF5P_Q0XWaxdHAnjHv0rNsR0nwdG95mm-jd1rXjE,118580
-vespa/analysis/tab_prep_fidsum.py,sha256=dvPwvPu0f5CE9zKIVvJK1Girv338Ab_4Yi5j-7j1p8I,51561
-vespa/analysis/tab_prep_timeseries.py,sha256=A9AayFqCCRvhU6qT3gCbroaUmqfISJxNNLMXqxwki7c,24000
+vespa/analysis/tab_prep_fidsum.py,sha256=izc13WwNcRFkTYK0wkRz5mXU0zrPIzOJcRIdlQQ0G_s,51841
+vespa/analysis/tab_prep_timeseries.py,sha256=mspyvVmkpCq-gcL76vpPwpOW6azHQxLefHwFiqjaWp8,24081
 vespa/analysis/tab_prep_wbnaa.py,sha256=VzI90ita2gBcQmqa7tu9iCeWEy_3m2arDVAjaz90igI,27449
 vespa/analysis/tab_raw.py,sha256=zAJ2suZpZ5fVfjbrjWo6_ng-TsVxEDBqoKvJYIEVP24,5874
-vespa/analysis/tab_spectral.py,sha256=K5SptBeTPyYISY_edBXtpSM0-pu3evgsBjk0hxvh4UM,94724
+vespa/analysis/tab_spectral.py,sha256=LX3gzuoUthYzDw7yM0MlrfyB0VrWvuwpuh4tJDDhc4g,106352
 vespa/analysis/tab_voigt.py,sha256=MIzyUDcHTnnYeIt4alen-wv438ESFV4pmqY02CMDEkY,152487
 vespa/analysis/tab_watref.py,sha256=abpMd4aaPHx-7qLcoY9vXifzxsDw2RN5YeINA6BuXNg,36691
 vespa/analysis/test_multi_optimize.py,sha256=2JhU6iulksAk_PAxOcw4fvlYCRagNi2JKefhzz0T7ow,25912
 vespa/analysis/test_multi_optimize_pool.py,sha256=hdjeYzywVrovFM0B5ChOTOQmxvl3eVY40Ai9hnqYeWw,30675
 vespa/analysis/util_analysis_config.py,sha256=NCuUzpubA6FrFxSQiOCAdzQuUp0rcyFYyrFxhw5iP1Y,2288
 vespa/analysis/util_db.py,sha256=O8iuAWDJsqORYhEXsFUvabexYm6HRo96R1eNrbsXVgQ,586
-vespa/analysis/util_file_import.py,sha256=QzqJu1T9woENdwwIcFG7C6HPdmf4hZw8G1UretH4TZM,18798
+vespa/analysis/util_file_import.py,sha256=tULDhxkRImj74dvPETU8bOY3S7OtxUrMnDWePvmFjuo,21320
 vespa/analysis/util_import.py,sha256=gWHT5erqRkcaOmg6vDPa5WT0pqFdq3m19v9LAsKTjYQ,2518
 vespa/analysis/util_initial_values.py,sha256=QHPB_pcnCvfELqY1ej1kOZk0uDFG3eJct3493KC8j1M,70015
-vespa/analysis/util_menu.py,sha256=ZuV_1AqzKvcrme3JATp3aA4IvhZ_sqj9R4glDcmTxdo,44104
-vespa/analysis/utils.py,sha256=4pulJWtlNkrK-ohRg1czxbpp3PX6WClJlwPG9qpkL8k,1149
+vespa/analysis/util_menu.py,sha256=1XtsMrn5hnNqywF1OMFaBJYYjTNuGG04hnJjiH6q10A,46427
+vespa/analysis/utils.py,sha256=Ht3vr7GKV33JfQsvBY3jSK1InZyMAtBRzDoNSl3TI0c,5791
 vespa/analysis/algos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/analysis/algos/auto_correlate.py,sha256=fAxi6FxSn6JAHrWUp0uGRTG-oK_p8C-2yq_9sbBs4po,1633
 vespa/analysis/algos/b0_correction.py,sha256=fHRikwOtKIiIg3Q16ItElQ2tOZRRpaYjDrCKl_zVqHs,1683
 vespa/analysis/algos/constrained_levenberg_marquardt.py,sha256=P5yuZW_n9138S2EIUhjwXW7og29mghCfbwNSz4UV_fE,13137
 vespa/analysis/algos/cross_correlate.py,sha256=iAX37bZ6YuukOKjOyUeajBTqkG-a01IvKks7MBN_Vr4,1564
 vespa/analysis/algos/fida_ecc.py,sha256=RQFzwrSwtpObTm0_0JgCPrZcOW8vNgFYbkFVGe6U0sQ,3228
 vespa/analysis/algos/fida_getcoilcombos_specReg.py,sha256=HdSX4bBMc3UUrlhag-JnUw2-1RaMpoToaHOpPPZbRe4,3246
@@ -119,26 +122,28 @@
 vespa/analysis/auto_gui/raw.py,sha256=_nFctE-nV9N-2C6iXuJ7oKZJR1GBlBqNi0ZfT-r2lSQ,3010
 vespa/analysis/auto_gui/spectral.py,sha256=2sPAn8wg3-VfIeqaA2WlOSdKgTypo1aR6y5GuxPqPFQ,35026
 vespa/analysis/auto_gui/timeseries.py,sha256=1I35vOdYWlVxl2T6Nuqu6DSZfitn4DyG6IA82sEretg,17067
 vespa/analysis/auto_gui/voigt.py,sha256=RUuqEPI3_Wuk9C3Ox0YGUIyJ6L1ejyAYOn4cbWmHYOQ,86685
 vespa/analysis/auto_gui/watref.py,sha256=qxxq0SBesHTy-JJ1fKV6yaR60uMoJlzf9pFW2ZZrYio,17137
 vespa/analysis/fileio/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/analysis/fileio/bruker.py,sha256=mKuAU_ihT7Ur0jQ6ei2WgAF_5Av3xQZIvnY3eunFWAc,4656
-vespa/analysis/fileio/dicom_browser_dialog.py,sha256=uhnwP8zkDty4bCyt4PAa-RBKXmNY67FwrhbmU_p_EL0,60309
+vespa/analysis/fileio/dicom_browser_dialog.py,sha256=VfNNCOOP_HcWa-aVucWjLwRDB-k_8OtBnjD6terKX_w,60852
 vespa/analysis/fileio/dicom_philips.py,sha256=LfodE8nJ-D5-p6ZAGRQNhm9OcvrINLJTzgFx3frV_Kg,8306
-vespa/analysis/fileio/dicom_siemens.py,sha256=SbYve7stoTRiprOTyY5AS_lDIGO8oZmTVQ5LTadFZyg,15275
+vespa/analysis/fileio/dicom_siemens.py,sha256=_ZM90vYmRTXZQ7rrq_KwJtGZ0GWKAa5uWvf_d7HGOvQ,15392
+vespa/analysis/fileio/dicom_siemens_cmrr_mpress.py,sha256=ssWVD5yzOkiTRCVGNueCFfiJj4h6HK3_CbSpzrggnrs,19729
+vespa/analysis/fileio/dicom_siemens_eja_svs_mpress.py,sha256=9MNW3nQPpCO8CwxxPOpGutGlsbDLbyrz8Zs736TOQ8Q,19998
 vespa/analysis/fileio/dicom_siemens_timeseries.py,sha256=3KFVZzU-CKZelAdb45JX4G_2keE5bj320LEGuQKHwGs,720
-vespa/analysis/fileio/ge_pfile.py,sha256=SqRwGqsRZbyKZdF1gDqwmphE0OJcSNylfWkthIPP42I,8041
+vespa/analysis/fileio/ge_pfile.py,sha256=LPXMKjjDrYn1gl2zSSmd1rSu7kqSxWxrFtUizlmoeTc,8193
 vespa/analysis/fileio/philips_fidsum.py,sha256=7u1ThE0r4bKOCHTTw8yipSMTdEwUk7Wf6PxTqDKuRIc,1894
 vespa/analysis/fileio/philips_spar.py,sha256=mlb2ylIyAAzr_vC7L5Dss5Esez_-z6ZNlLR7Ke06x6Y,7281
-vespa/analysis/fileio/raw_reader.py,sha256=2AUGH54PMbc-lcIAd1T6tfsrwt0jEkG8OOWGWC1dkMg,9119
+vespa/analysis/fileio/raw_reader.py,sha256=_NF-C_Aov_FUilxq5BKz2FBKraOEr56en0wj-II3few,9690
 vespa/analysis/fileio/siemens_rda.py,sha256=sqqnehm-PL05nbbiUSKeUtjQz7cVb38VeewjBBI-Nw8,4381
-vespa/analysis/fileio/siemens_twix.py,sha256=EeiGeGiu_Q0NrKr-Y_HnDwstM7IhMS0r2pE_H6YA9cs,20784
+vespa/analysis/fileio/siemens_twix.py,sha256=_WgYffw7uSfF61ycZ16kF88_AsmvGEIXDKMfGalcggU,21064
 vespa/analysis/fileio/siemens_twix_slaser_cmrr.py,sha256=3BcrSRHbmW9HGKC386GXpGgCuSq0nZ3LTMMu9Nydbp0,7395
-vespa/analysis/fileio/siemens_twix_svs_edit.py,sha256=ZFqoeBOEXKAn3dAVzgtE2cBYKkzD_MxnmAtLVYc3qic,2993
+vespa/analysis/fileio/siemens_twix_svs_edit.py,sha256=k5uWh2rmdVmvDQCJZxlbmKo8E1KQzv2oqBmQxYkO6c0,3055
 vespa/analysis/fileio/siemens_twix_svs_se.py,sha256=Bu-Y9FOOxJnJzSLYRA9IZ2soPZ32_3dOl4RpD_zti7w,1735
 vespa/analysis/fileio/siemens_twix_wbnaa.py,sha256=aCTBTszTDbeoygeO0O6R5pj20wrDqbIdjTHv6I_0PK0,15803
 vespa/analysis/fileio/template.py,sha256=gUX3R-AViIB5_SITqBYSlnaFxSw0wr6GyAPMDne8S0Y,7146
 vespa/analysis/fileio/util_exceptions.py,sha256=i_KhvHeyqLkJUiguYyktXusJk89-El3v_gwaDLiezj4,2347
 vespa/analysis/fileio/util_parameters.py,sha256=-9emo82e_H4MHOYt06086kE4Y_tXatrF5Rw1Y1HHsk0,6634
 vespa/analysis/fileio/util_philips.py,sha256=aeXHbfIYlm1UCDrTNkMoyUy6s1AoTTjO6L6qlr95XHk,8272
 vespa/analysis/fileio/varian.py,sha256=TK2aWD37zy6BuQwNmSVgisAl8p8J91J9MVGtxKRgZ3Y,4721
@@ -153,71 +158,71 @@
 vespa/analysis/fileio/dicom_browser/auto_gui/dicom_browser.py,sha256=HxOOxzKW1ftdNnsr09OqxAt1GsGyshmTt1JkOEUWw_E,3288
 vespa/analysis/fileio/nmrglue/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/analysis/fileio/nmrglue/bruker_for_vespa.py,sha256=TZ_TrtsLOG-UjOizYMRdOJPm29kO8C84180d8J4Dppc,84694
 vespa/analysis/fileio/nmrglue/fileiobase.py,sha256=Eo8pTT7pNyjVsk_4dMcV8Nnd_tjNiSWm62RjGoI6AaQ,20111
 vespa/analysis/fileio/nmrglue/proc_base.py,sha256=wBTUKY7Tm28HG3HJJNMfJtkrv7oWc27S14AfRhpGSGY,63756
 vespa/analysis/fileio/nmrglue/varian.py,sha256=xU9CGlAzWl-jObh1ax7MSZ_HS0i1MawNHnOxeHetAY0,64749
 vespa/analysis/functors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vespa/analysis/functors/funct_ecc.py,sha256=rU_Ja3ge020wOLhc68ZGevWak-0bIJfnVrYNr7qOotE,22520
+vespa/analysis/functors/funct_ecc.py,sha256=ErSgOYzSz0ZtlWgPXEPRdqy9Gg7_dBPWBQhkUqGIScA,23166
 vespa/analysis/functors/funct_fidsum_all.py,sha256=RyNJ4gjuKqpSZ2ou0k09RGZrdeqD8zpz3AhY6tRZsOQ,9504
 vespa/analysis/functors/funct_fidsum_coil_combine.py,sha256=DgWoij4QXCZ-bgEHijeALTWDJwT5sbJ5iK1mhFmuJjM,19534
-vespa/analysis/functors/funct_fidsum_correction.py,sha256=PstMD296nJSEvy4_RPX1hBE69IXgu1Fv8wautDeSQpU,16331
+vespa/analysis/functors/funct_fidsum_correction.py,sha256=sFVEkiwCMYR-tX2KIa5ZlhRyFbFmcmtLTO25zVI-DhA,16394
 vespa/analysis/functors/funct_fidsum_exclude.py,sha256=YvJLr1iipdWcpItqSdgRRv9QRp5uvSlzm1nZUI4cgnc,2590
 vespa/analysis/functors/funct_fidsum_megalaser.py,sha256=WIu_Ns2LfEi2vVoX2jaGRjR7pOudWQ4UqvnUt1mYEtA,11631
 vespa/analysis/functors/funct_fidsum_wbnaa.py,sha256=XIwn-mpjtVLAUtDkvdMGZb4Zv-lo4IwkjcANqm4tibM,12259
 vespa/analysis/functors/funct_fit_giso.py,sha256=NJhpvo_dY3cVlv5e3ENeQRjZKmKpJG50DM1gTqCBG4k,34838
-vespa/analysis/functors/funct_fit_voigt.py,sha256=NYQIL47JuikCWLLuIuvpgpA_SnYAzVtMTMpMvoiXUFc,45038
+vespa/analysis/functors/funct_fit_voigt.py,sha256=34_472pdU1qkgjSRQcYKmokC3tgB-bi_Ymyk9tCZGrg,45412
 vespa/analysis/functors/funct_quant_watref_all.py,sha256=PjiIyrw2nTt2c0_eC1hlK1lI1f7TKLLhn0U94WPxRmY,363
 vespa/analysis/functors/funct_spectral_all.py,sha256=wAQuVgYuHJBRSNh9PlcvWJTiViehYiFR3vBpj0XDVKY,15521
 vespa/analysis/functors/funct_timeseries_all.py,sha256=gGshZilv5EBdSBNxsMXTo19h2HUgy4f36Jj0XbAJGoM,10751
 vespa/analysis/functors/funct_water_filter.py,sha256=8llg7q58JsTNY9q_ySB95OR266jO6KmbwVtcgmY0M6s,13207
 vespa/analysis/functors/functor.py,sha256=rKnmDjPZ8xu-pyz5jXrC-rbpepb46iDWDIBOH5A4KQs,1055
 vespa/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/common/base_transform.py,sha256=UqLZz8LeGCSbCDVb0e8xyGSlOPfT0yiNnQmQYoh1tkA,8785
 vespa/common/bloch_call.py,sha256=h3Twjx13B7YuG-6RKLZzieZEaK7-ussXvMYc0mGe8es,6970
 vespa/common/configobj.py,sha256=-6g4THBdQMT5EcluePMOrO81FFqMKBC8YMurGaHJRwA,1232
-vespa/common/constants.py,sha256=huwW2Os_YUBm2Yucf_vC52I7VECisGX3BArS-Xh_KCw,30989
+vespa/common/constants.py,sha256=Xb6tm9FrMTwm1v2dSFcJ_y-eVEfgvU5ThV2IGiqvPHc,30990
 vespa/common/create_database.py,sha256=YD1HrsU4UdwD7m9Kxh2v-4Q83rERRz-n_Obk64VvLkY,11886
 vespa/common/default_ini_file_content.py,sha256=MmdyJK7rHnE28Ny3wMu2TedaE_-sp9zYjpwzUbko30M,15836
 vespa/common/dialog_experiment_browser.py,sha256=p7wsVvpVFzFebWCTZGAu80-2-MmRRhVgiqgjNPfVSIc,6615
 vespa/common/dialog_export.py,sha256=fJUGYRKNCRKn5PJdH1k5YHlqpolGwqglVdDK8CsdG9M,5828
 vespa/common/dialog_pulse_design_browser.py,sha256=y7PlfaZ5Ns_wd9rzy8qMQOBwaYaHmgHhxp72-1BHT6E,6528
-vespa/common/exception_handler.py,sha256=PEzNZS-cBXoqMw-XQRgmeNIlIZamdckJssNnZEeHsSY,12150
+vespa/common/exception_handler.py,sha256=AhNdznmXKykN_KMRpymNyXKv9Mr5HUQhTOqCKKnSDXQ,12182
 vespa/common/experiment_preview.py,sha256=SMOi4ABiVX5NbzuuqMkUahVZTq9Fz-LERap7A8Nn7RE,2465
-vespa/common/ge_read_pfile.py,sha256=urDgdvv6doIawS6Qq40Y_tYEPvxhmRC1Y5sFUhnM1nQ,210652
+vespa/common/ge_read_pfile.py,sha256=YnrMH55RprW0QvcBaba-FAMwEs6H2JDmyoNNxGbrdeM,198250
 vespa/common/hlsvdpropy.py,sha256=NUZVXRtwpWPsiavJPdiw69rs0Edh9deL6dY0q9Luzp8,36943
 vespa/common/images.py,sha256=yiWz5rXu-1E2ekZec_H2EVHp4KJCEOFL2urIFgMpAso,10905
 vespa/common/menu.py,sha256=Phi0sIZSbEb2B0dOG7F9mfab_DxYaukEeYs0JQ8mDyA,10917
 vespa/common/minf_parabolic_info.py,sha256=q9Hws47y9EKg0Cov146sMdOxPLmAU9y2JYbn8ng3Q7w,7261
-vespa/common/mrs_data_raw.py,sha256=sDUXMTnAMTHwIO_TjT6EB7phOIxa-PENa23ATbLQBnE,20366
+vespa/common/mrs_data_raw.py,sha256=FOwe8VQRvlHy_OVQwmQfo3FQWCVkANwa6PEudIZ2Z9w,23597
 vespa/common/mrs_data_raw_timeseries.py,sha256=9eAkgIrnKSfPwTQKZPxf6BKvZLkukGpmnFpTlnB46jA,788
 vespa/common/mrs_data_raw_wbnaa.py,sha256=xzVWVbSVqMY36yLYVfnc2KXQDc_0tru374RsrZ44qa0,996
 vespa/common/mrs_experiment.py,sha256=QQ5I90oDFbYCH-aTwvjuIakchmoc-_3QqVWi16HAs3c,17733
 vespa/common/mrs_generic.py,sha256=xEdo5wo5PK7m0uNwavidKxeCBEgP4n1JV3FW4lV8lm4,10811
 vespa/common/mrs_generic_basis.py,sha256=NM8U5o9dRMuOuVZpiaEmhSzy3QN6f8KVhcjNE_4JMv8,13639
 vespa/common/mrs_j_coupling.py,sha256=IZMsmJLHetWOdIO6kSeP6M5AmL9x1ufFSET4dONBhJI,2489
 vespa/common/mrs_metabolite.py,sha256=71pkBu4dRTxvlCkBWdCGQgqAM8rey_-hH40UIW05s-M,8055
 vespa/common/mrs_prior.py,sha256=jLeYcArXDbcz-NIQRDky7sah1yYcUoI0Rzb0iZanGTc,9319
 vespa/common/mrs_prior_metabolite.py,sha256=Cx0R-748IIlF-eu8iDaGUqgIw4oGSx5pZZNCo9uURM0,5083
 vespa/common/mrs_pulse_sequence.py,sha256=ga_yDvE9bTRqEaeh73n_MimmbtUnNHTiSRY3riWci1s,9326
 vespa/common/mrs_simulation.py,sha256=GDV-8HzDai4z0RVXNU9q0r73yUwZvkTkJntkEh5a7yA,11755
 vespa/common/mrs_spin.py,sha256=Dp_dJWM0Xe8Cp3YwYFEDjPUd6Ta6GUUUnvAhzJi5NsY,2177
-vespa/common/prefs.py,sha256=nYZE3cYBsGil3xirY9PVj-LpRzOv2RGoXIT7LAuy12U,8707
+vespa/common/prefs.py,sha256=2v7UNgBtFtlMtfbAq3DNGC3AA0NwHaTDtTde1R8XIw0,8740
 vespa/common/rfp_machine_specs.py,sha256=HNV1rsgXlKVolLnwxdVvMilIghJB50gS92mHiKH9Hcc,9473
 vespa/common/rfp_master_parameters.py,sha256=chcm-QZ6dY74ME4qpFBGRE88xVGV1iDvqZJod6NptB4,2842
-vespa/common/rfp_pulse_design.py,sha256=Zucqe252J_6piAS1APxV-CqaFLd2usVw_5k7kEcUQq4,19774
+vespa/common/rfp_pulse_design.py,sha256=t_ro6gowXZF24FIfBbh5x6Pxdkvg-nGmca3j2B1a1hI,19777
 vespa/common/rfp_pulse_design_preview.py,sha256=-jwCNmAovxI48nTvha_ce5WMvWWEZraVn1rD8KEuCc0,2182
-vespa/common/rfp_rf_result.py,sha256=j1Y0hXYaBhqrieu33cz-_WRATJS4udUhcal-xVPHc88,24203
+vespa/common/rfp_rf_result.py,sha256=r_vNeYHaQBaN9jcIe67yCrgQeF-2Yn_aGajbfJwcCYA,25646
 vespa/common/rfp_transform.py,sha256=uUWBKMGQdb2UAZmqGyDlVio_AEtEATMjb9h3IPM7iq0,11262
 vespa/common/rfp_transform_kernel.py,sha256=l5wRxqX7iWpORBaE6Ii4l0NdaR5rC1Vwhh0VPXUCUHc,19525
 vespa/common/styled_text_control.py,sha256=BgspuvDpX3WD_26t0O3rBZkAiTMJ2-Jyx7OgomPqCHo,15742
 vespa/common/transform_kernel_preview.py,sha256=1ItneTYOs3xhY0H9PbuM1n6pi2WgvdFniCsZHbRZCKE,2264
 vespa/common/transform_run_exception.py,sha256=fGRxf-jd6jxBpTCPzWI-RmkY9om37CIsLPReQjoYDXs,802
 vespa/common/twix_parser.py,sha256=_ydYHshyvjAeTT6gpTCR4xlRX7gCuIkmDlWY0oPXr8g,42333
-vespa/common/twix_parser_multi_raid.py,sha256=1c7t80AvqhYT1unEVMOaw6glw8MUYEuhOgQg4GFrIdA,67633
+vespa/common/twix_parser_multi_raid.py,sha256=x4iNLoqtA6ruAkj_5gKrrmZ27sz2aGVjOzdfBvU6yMU,68433
 vespa/common/wavelet_1d.py,sha256=eyyDIZhkg1aQsu1RzlVCiVieYSqK4kvn3Fpwd9oTI6U,262945
 vespa/common/auto_gui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/common/auto_gui/exception_report.py,sha256=Bt1_SjoRJTUXQkaJWAUAqeULLGXcuVouXZKuO7DOaec,2203
 vespa/common/auto_gui/experiment_browser.py,sha256=dwUfIcJlbT5C4-bq-iJe5U25P_SFmH75a0YJhI_AkqM,3417
 vespa/common/auto_gui/export.py,sha256=vSEiHa8WYSfS9EA2GYiS0BXYe9iF5R0Xe-Kq44sPH2M,3105
 vespa/common/auto_gui/pulse_design_browser.py,sha256=0UVUdL4R5oO0eruI42BAEphKqrt_IMVh8NQv8-cNsqQ,3637
 vespa/common/auto_gui/pulse_project_browser.py,sha256=v3RpCGYABYo_pkKfDek-rdNOCVvgf5GClh_sos-O_cc,2846
@@ -285,32 +290,32 @@
 vespa/common/util/ppm.py,sha256=WNp_VJwPgN2uB4pRO2ws-ek-RE8Z83Z_FmXgjRs2_m4,6326
 vespa/common/util/time_.py,sha256=5lvZi44tXXTope-25VNgGNdVcB3n50r03Kd8k9qGrH8,4873
 vespa/common/util/xml_.py,sha256=L0fMPq51eCgSrtleu31WXMJX7o7nxSutjKDqCdBYSDU,28288
 vespa/common/wx_gravy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/common/wx_gravy/common_dialogs.py,sha256=m9JIsjcNxt0G13658NbMXG39rSGz67fuwHAKgUkcKNk,7027
 vespa/common/wx_gravy/image_panel.py,sha256=_NDFYPbAUpkjYl22Q8cDZVPpotKJ8LHyX1GiF8GjmnA,68903
 vespa/common/wx_gravy/image_panel_roi.py,sha256=925nUrIL54mo0IYh5ENxEHdroNieUYiYbBDmgSYzKm0,98996
-vespa/common/wx_gravy/image_panel_toolbar.py,sha256=P8gyG31ATtWmh3N5Y9EXiRx20ZDCxkcPAeDZELZR_U0,67355
+vespa/common/wx_gravy/image_panel_toolbar.py,sha256=c-CJuBn5SW8PPQYUULLSpRShW6s8A58_yjJAUUJG3B8,67254
 vespa/common/wx_gravy/mask_panel_toolbar.py,sha256=rhc9lRdfaMdR1flQRb42_7RKSYM0FBeiuJFdYvQw0TU,78240
 vespa/common/wx_gravy/notebooks.py,sha256=uUEl6wGwHHqgrIr4c09F5txTr2HQ0FqriHucxa5mFic,6415
-vespa/common/wx_gravy/plot_panel.py,sha256=yw-Tpdh_DZyOHsGKkZip7GKZwk-z5Gousi6i7M1bx74,59997
+vespa/common/wx_gravy/plot_panel.py,sha256=M-qMNva9RJjcuqhXl-eyO0phf-MK4oWMQQGixhbXb4k,59997
 vespa/common/wx_gravy/plot_panel_points.py,sha256=wna0aFUWj1rhuTNncozFoO5KBR_yHUmAE6h1AYiprFU,93072
 vespa/common/wx_gravy/plot_panel_scatter.py,sha256=H2ZiHjvRv_vO6SYEH57ZOsXLWHPHFTvpJXtz99L5OMc,94844
-vespa/common/wx_gravy/plot_panel_spectrum.py,sha256=A3wFwSBW7-oNQo7YQUHgE6eDCAWuQPLfuJIkxCmH7Wk,116167
+vespa/common/wx_gravy/plot_panel_spectrum.py,sha256=EBPBxPoXpCHAZUR9-zQwW-tUA26TgR_davYAWmeqkHE,116692
 vespa/common/wx_gravy/util.py,sha256=ZgQD5Etsxqy2wRKEM5VLrJ4CNoGo2QCivD_krTItgI4,18536
 vespa/common/wx_gravy/zot.py,sha256=TlA3zuvD9_WPUeCvprZFVVZN7rLvpovM8TrYbxFsMyM,2386
 vespa/common/wx_gravy/widgets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/common/wx_gravy/widgets/floatspin/__init__.py,sha256=phTZLmNs5VUaLhhyeUrzCgm5MqziHWLb10vh6IN-LHE,162
 vespa/common/wx_gravy/widgets/floatspin/codegen.py,sha256=P0TpKQpQl5qgjjNI2U7sPUC4Ev1rJ9xA7tFOE3IllFk,1721
-vespa/common/wx_gravy/widgets/floatspin/floatspin.py,sha256=e_6cBk2DCJOBPhSwhuyClhmzuoMITBrrciBOQlPGHjA,8725
+vespa/common/wx_gravy/widgets/floatspin/floatspin.py,sha256=YOCmCaRM8gp4KSVZarmSAPCeiGWNPruVO-LITQMz8_I,9243
 vespa/common/wx_gravy/widgets/floatspin/wconfig.py,sha256=oDXZI5mFPTJcC09ZXuiBpAuDv_hQIOXGzHCRXYB8nsY,3200
 vespa/common/wx_gravy/widgets/floatspin_multiplier/__init__.py,sha256=qjYAh-ieXE9X2q5sQP2xGea42rmVamvODDQ-WWJDBA8,172
 vespa/common/wx_gravy/widgets/floatspin_multiplier/codegen.py,sha256=WNsSVwuwrgFCKeTJtLkvdvJzL4pmEZP5gjA8frAKG2g,2206
-vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier.py,sha256=OZpQRFWwJgzwKbGf3noFJTct9ho36_ukG1KHbjfImbA,9088
-vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier_base.py,sha256=aFEuXFZh7oLx9-yzVDd_dfDCCx6yDbxmNo_mhA61LKg,2514
+vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier.py,sha256=v8EpGjh7DWTWjRhgy_sZ64852Y4N69zZ4yXdiboh6GA,9611
+vespa/common/wx_gravy/widgets/floatspin_multiplier/floatspin_multiplier_base.py,sha256=2c0ISjDV4ewBdCu-vB-LwKWFM8e2L0ITVOYc8WcxnB8,2508
 vespa/common/wx_gravy/widgets/floatspin_multiplier/wconfig.py,sha256=IopymEFnaXiKU69RbR3VrhLDyXArV-ffkcHGo_b6qpM,3236
 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/__init__.py,sha256=qjYAh-ieXE9X2q5sQP2xGea42rmVamvODDQ-WWJDBA8,172
 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/codegen.py,sha256=WNsSVwuwrgFCKeTJtLkvdvJzL4pmEZP5gjA8frAKG2g,2206
 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/floatspin_multiplier.py,sha256=v8EpGjh7DWTWjRhgy_sZ64852Y4N69zZ4yXdiboh6GA,9611
 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/floatspin_multiplier_base.py,sha256=2c0ISjDV4ewBdCu-vB-LwKWFM8e2L0ITVOYc8WcxnB8,2508
 vespa/common/wx_gravy/widgets/floatspin_multiplier_v96/wconfig.py,sha256=IopymEFnaXiKU69RbR3VrhLDyXArV-ffkcHGo_b6qpM,3236
 vespa/common/wx_gravy/widgets/floatspin_v96/__init__.py,sha256=phTZLmNs5VUaLhhyeUrzCgm5MqziHWLb10vh6IN-LHE,162
@@ -340,14 +345,23 @@
 vespa/docs/datasim_user_manual.pdf,sha256=S2XH8ZWM21kaumqrixWhVK8FSXDM5ybZEkvSe3HDD5Q,448020
 vespa/docs/pulse_user_manual.pdf,sha256=W4wAjuDUf_6_IGpEEKqAkUK4xYzlhDEouqSsSDYAwS4,1181178
 vespa/docs/simulation_user_manual.pdf,sha256=qXZFcgXOyxbewopir0yAVJSTe_FKG_6MYNmj-cLse_g,1132329
 vespa/icons/icon1_datasim.ico,sha256=ghk-fPDCxzi1qPUfXQ9SJMQMZt_LDhT1VlpxX3cbNMs,19518
 vespa/icons/icon2_simulation.ico,sha256=UCbbHNlkmkrtg3Vj5broyo-8WRIo8guQkdEs3SWeSyc,19518
 vespa/icons/icon3_pulse.ico,sha256=wBJ3rVMwVo56Z2MnftAVyh-sBSDqgN-G8Gsc8HXQ4tE,19518
 vespa/icons/icon4_analysis.ico,sha256=S7G7VIiwpSG6dURZoJZzbeTP1oiCUZx9pumf05ulSHw,19518
+vespa/interfaces/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vespa/interfaces/inline/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vespa/interfaces/inline/vespa_inline_engine.py,sha256=VfEHhJz3fyWLVKAzK2fD-JYPhvKXey3VrcWfE3ZOfhE,25199
+vespa/interfaces/inline/ge/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vespa/interfaces/inline/ge/inline_vespa_ge.py,sha256=vBwKDUBOkIIycPuNkdIvatA7oSf_NOWLTQIeF6vBIWE,118878
+vespa/interfaces/inline/ge/run_inline_vespa_ge.py,sha256=SFunEiwMgYhyUhG3T9mnDkxuXHUnqrkMLvcKvTYBPHU,17884
+vespa/interfaces/inline/ge/run_inline_vespa_ge_v1.py,sha256=n66U3168_m7KEU9vV1d0Ay3HANBnVcJizH3Byy2yuMQ,4880
+vespa/interfaces/inline/philips/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+vespa/interfaces/inline/philips/run_inline_vespa_philips.py,sha256=ZBI78exuZ7z32o9IEDJIIVRwbEDMl9C8H1aT5ncW_lU,20930
 vespa/public/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/public/annotated_coding_example.py,sha256=20mGlFneiPDeHfLGE9ImDXfuBsGd0EybORBiUa34R-s,3482
 vespa/public/convert_ascii2viff.py,sha256=yiSYulx7bmzjqKwDHNy_6wTfGEI1NWxIrOqxtFDKjc8,7232
 vespa/public/minimalist_pulse.py,sha256=HFe-LSreHJQtdK5WP8FZyThKoY6zuBT2r4iYL6XOFuk,1819
 vespa/public/simulation_description.py,sha256=Fqf7IBhO3TtflrmsweNdclzMm-TMb016R0sSlsCLMT8,5589
 vespa/public/transform_description.py,sha256=mFsCwnaUZA7a-WxBEma9MvAQ4vf_VhhOpIVwK2GW6sY,1513
 vespa/pulse/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
@@ -368,15 +382,15 @@
 vespa/pulse/plot_panel_transform.py,sha256=fj8gSF1KRbH6Odyp13I4JBF1YZCPGd7zSQhIxKbN8RY,2645
 vespa/pulse/plot_panel_transform_contour.py,sha256=NaypKpXcPhRJ2AeYVzsBSOr6AvJL6Iy_RnmOKiRCHto,5166
 vespa/pulse/prefs.py,sha256=1jGPYRQG4zq7qo7dTWeP-G1-KKpn4qeiKPWBWpWa9rI,2363
 vespa/pulse/run_transform_controller.py,sha256=su7YyDdMbGKR714KQl53Ow1zCYsqo1IRosPBl8yXuLg,26064
 vespa/pulse/run_transform_controller_multi.py,sha256=KpFX0pSPobi2P95_c9kM9D3z4PIMgowJdaKqNdzGqQo,27877
 vespa/pulse/tab_basic_info.py,sha256=SKX0EeCJ8HEJ9cMJWJe4pW5-bthIpD5SkVWX7l4AKeg,13461
 vespa/pulse/tab_pulse_design.py,sha256=hNfFtrSPqq9R9zxshdUOtpDYcWmdtMIs4LcJWTTG_Ts,29011
-vespa/pulse/tab_transform.py,sha256=8v0gEPjrFntXmMKmlFDFz5brsaMckJCmX3wFPnf8gUE,71252
+vespa/pulse/tab_transform.py,sha256=RQZHLnqRKSiQNSHs3bVFxxsWOYKTz5b97d2JRpzzSLI,72322
 vespa/pulse/util.py,sha256=NKe1po_AcgzxIUku2684gAqsfgI1gyqgz_XZ3t0gDyo,838
 vespa/pulse/util_db.py,sha256=VyE-N6ebpxx4WJBylMsiXqr3NqEca6_pbKEuvg5kFvM,18518
 vespa/pulse/util_menu.py,sha256=MruUqfc2fGGKIsTrL3NnOATSXSERupQvhm5LhnpInpI,8599
 vespa/pulse/util_pulse_config.py,sha256=mHefX-tULrP14aaiPSv-6i5J2bub9L_v6rHBABJXedQ,745
 vespa/pulse/auto_gui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/pulse/auto_gui/basic_info.py,sha256=8ygmMZGJ8OV1LH_hQVnVXEFajoxKX2jG9ezZMR1gzz4,6787
 vespa/pulse/auto_gui/editor_transform.py,sha256=gY0mdjkqjRIQpC0Y3eJ6uk-10ZJEv26Erf0W-PacicY,13112
@@ -384,15 +398,15 @@
 vespa/pulse/auto_gui/machine_specs.py,sha256=BF0u61QISHXIpKiRgJNSZiHCyMEVcpkY7ZBXU52qHpE,7126
 vespa/pulse/auto_gui/manage_machine_specs.py,sha256=Z11cakRjzxADzjlYJN3EcHL58M3vcCFB5434JS7UAsE,4657
 vespa/pulse/auto_gui/manage_pulse_designs.py,sha256=qDBvO-_t35b9MctjUwJhkfuthJxcb_bEPauW9RLdURI,5272
 vespa/pulse/auto_gui/manage_transform_kernels.py,sha256=2qDZLHb4HJ_8JjwXWdM-1Ra0aEySHwYmYMSXvaia2GI,5720
 vespa/pulse/auto_gui/ocn.py,sha256=K0P28NvczyD9O3IFJB_6H_YrnTeu7C4FNoZdYvQtYhA,14094
 vespa/pulse/auto_gui/optional_message.py,sha256=JzYKLRmkd2Xh9q185mvgipXBU0Hn94ZVLKssY0Uqi9M,1507
 vespa/pulse/auto_gui/panel_kernel_globals.py,sha256=xMM1iFZmworuImxeEUb-BN4oymTZllKQDfje_yhXcPk,4039
-vespa/pulse/auto_gui/panel_tab_transform.py,sha256=WNt2liDoXWXQWlBQVdu5hN1oNvEfFnzY4JNwUPDFfwo,11463
+vespa/pulse/auto_gui/panel_tab_transform.py,sha256=8E9ZrcNQIErul731nit3K6ZIgbgQrYVmK6rjeqw4Oeg,11940
 vespa/pulse/auto_gui/panel_transform_editor.py,sha256=Uz4huokt5HJD_EvJaALsytTwH-88u8VOaum121ubsho,9615
 vespa/pulse/auto_gui/referrers.py,sha256=Qrdc6dRQoSQTZ9_Ax3P1IqG6zE2G10VZZ5MU4kCQo14,1970
 vespa/pulse/auto_gui/third_party_export.py,sha256=oqQBTY6sa8rlBfJKvM849cO68ECQjB6zxBNHFdS10fM,12269
 vespa/pulse/auto_gui/view_pulse_design.py,sha256=1EU-njfm1otEOVapepNz-QEIl-8uGEnKa2AR5UnhGks,1893
 vespa/pulse/auto_gui/view_transform_kernel.py,sha256=5SllikYz0xSmzg484OeVLrfNBl1jCjI43aAdnj2g4gc,1934
 vespa/simulation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vespa/simulation/aui_subclass.py,sha256=Kx70DkHUVI0r__9CfbfyKEc00-sqKOQBoDUqpho2Ds8,630
@@ -434,12 +448,12 @@
 vespa/simulation/auto_gui/mixed_metabolite_designer.py,sha256=T15IMyG83qIXA8BqpizQ--gNEHOuC49aAsY5J7kIO4w,4137
 vespa/simulation/auto_gui/mixed_metabolite_output.py,sha256=3npi7QuhQWZnkrbOXQr4gY9nasdHJNE5QBARQqpFEOw,25640
 vespa/simulation/auto_gui/pulse_sequence_editor.py,sha256=EQ3uvEOuRRtPtDDX6m3-Ry4btoytpr7ULeYMXc-S1Lk,22576
 vespa/simulation/auto_gui/pulse_sequence_info.py,sha256=Wn2lX2q2pPHBden2P4dB80UGD6o89v9UDm-I8gehA54,6996
 vespa/simulation/auto_gui/simulate.py,sha256=eOca4A6jamHH0WmYt-pslXksPEpTllsnSMoitA4FrrY,13199
 vespa/simulation/auto_gui/visualize.py,sha256=e-yIdNJn-zWjuuY8iA3dr2OYuH2IuIG9ZH9qDh5iOdo,16152
 vespa/simulation/auto_gui/visualize_resolution.py,sha256=CCaUG8aUyUKku21BHELwLr5BoBtcF2EkhyBE0lh7cTE,3137
-Vespa_Suite-1.0.2.dist-info/LICENSE,sha256=FwI2vIxc5HkyUOQW1hHLnGfmFbwA--JdwJ_ZRKXqOAE,1704
-Vespa_Suite-1.0.2.dist-info/METADATA,sha256=T50_ENERJ5Vnm75uiCnIvbcfiSRWj77_qZBsRxOD7vM,2093
-Vespa_Suite-1.0.2.dist-info/WHEEL,sha256=I5zY81DUoJ6uVSd-fokuUFvpLqLUGPlQYMOYm0Te7V4,93
-Vespa_Suite-1.0.2.dist-info/top_level.txt,sha256=uzFxUKvF72u8QfzlL-CkmaWw449e27Ch1XVlOgJWgbs,6
-Vespa_Suite-1.0.2.dist-info/RECORD,,
+Vespa_Suite-1.1.0rc1.dist-info/LICENSE,sha256=FwI2vIxc5HkyUOQW1hHLnGfmFbwA--JdwJ_ZRKXqOAE,1704
+Vespa_Suite-1.1.0rc1.dist-info/METADATA,sha256=P4uqInkiR3adIfhHDhIthyXOpOxXDbI0t5V-ACC2vik,2096
+Vespa_Suite-1.1.0rc1.dist-info/WHEEL,sha256=xpWd874vjxk-rlDUiSLccticwhjoUitFv4Zo1xTPV2U,93
+Vespa_Suite-1.1.0rc1.dist-info/top_level.txt,sha256=uzFxUKvF72u8QfzlL-CkmaWw449e27Ch1XVlOgJWgbs,6
+Vespa_Suite-1.1.0rc1.dist-info/RECORD,,
```

