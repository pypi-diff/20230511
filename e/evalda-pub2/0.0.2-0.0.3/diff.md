# Comparing `tmp/evalda_pub2-0.0.2.tar.gz` & `tmp/evalda_pub2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalda_pub2-0.0.2.tar", max compression
+gzip compressed data, was "evalda_pub2-0.0.3.tar", max compression
```

## Comparing `evalda_pub2-0.0.2.tar` & `evalda_pub2-0.0.3.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     1065 2023-03-23 10:21:49.117225 evalda_pub2-0.0.2/LICENSE
--rw-r--r--   0        0        0       49 2023-05-11 11:10:05.028504 evalda_pub2-0.0.2/evalda_pub2/__init__.py
--rw-r--r--   0        0        0     6463 2023-04-19 16:13:42.482308 evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc
--rw-r--r--   0        0        0     7757 2023-05-11 11:06:07.920873 evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-39.pyc
--rw-r--r--   0        0        0      483 2023-04-19 16:13:46.716225 evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/load_model.cpython-38.pyc
--rw-r--r--   0        0        0      483 2023-05-11 11:06:12.255364 evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/load_model.cpython-39.pyc
--rw-r--r--   0        0        0     3805 2023-04-19 16:13:50.367481 evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-38.pyc
--rw-r--r--   0        0        0     5771 2023-05-11 11:06:15.805110 evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-39.pyc
--rw-r--r--   0        0        0     9729 2023-05-03 17:07:47.956149 evalda_pub2-0.0.2/evalda_pub2/base_tasks/abc_lm_utilities.py
--rw-r--r--   0        0        0    41806 2023-05-03 17:07:47.956965 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask-danish-bert-boxto.png
--rw-r--r--   0        0        0    41198 2023-05-03 17:07:47.962956 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask-xlm-roberta-base.png
--rw-r--r--   0        0        0    39889 2023-05-03 17:07:47.964069 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert-base.png
--rw-r--r--   0        0        0      167 2023-05-03 17:07:47.964705 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert.csv
--rw-r--r--   0        0        0      167 2023-05-03 17:07:47.965139 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask_xlm.csv
--rw-r--r--   0        0        0   172315 2023-05-03 17:07:47.968269 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo.png
--rw-r--r--   0        0        0      351 2023-05-03 17:07:47.969075 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo_detailed.csv
--rw-r--r--   0        0        0      153 2023-05-03 17:07:47.969716 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo_simple.csv
--rw-r--r--   0        0        0      321 2023-05-03 17:07:47.970113 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_nb-bert-base_detailed.csv
--rw-r--r--   0        0        0      142 2023-05-03 17:07:47.970677 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_nb-bert-base_simple.csv
--rw-r--r--   0        0        0   162904 2023-05-03 17:07:47.973083 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base.png
--rw-r--r--   0        0        0      306 2023-05-03 17:07:47.974612 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base_detailed.csv
--rw-r--r--   0        0        0      138 2023-05-03 17:07:47.974908 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base_simple.csv
--rw-r--r--   0        0        0   136458 2023-05-03 17:07:47.976400 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large.png
--rw-r--r--   0        0        0      308 2023-05-03 17:07:47.976765 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large_detailed.csv
--rw-r--r--   0        0        0      138 2023-05-03 17:07:47.976940 evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large_simple.csv
--rw-r--r--   0        0        0      256 2023-04-13 13:14:23.045077 evalda_pub2-0.0.2/evalda_pub2/base_tasks/load_model.py
--rw-r--r--   0        0        0      208 2023-05-03 17:07:47.978516 evalda_pub2-0.0.2/evalda_pub2/base_tasks/requirements.txt
--rw-r--r--   0        0        0     6576 2023-05-11 08:11:25.536312 evalda_pub2-0.0.2/evalda_pub2/base_tasks/wino_fillmask_utilities.py
--rw-r--r--   0        0        0    47715 2023-05-03 17:07:47.981385 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_output/coref_abc.png
--rw-r--r--   0        0        0   155593 2023-05-03 17:07:47.983658 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_output/coref_winobias.png
--rw-r--r--   0        0        0      363 2023-05-03 17:07:47.984394 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_output/detailed_output_abc_coref.csv
--rw-r--r--   0        0        0      168 2023-05-03 17:07:47.984949 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_output/detailed_output_coref_wino_xlm.csv
--rw-r--r--   0        0        0    20070 2023-05-03 17:07:47.985819 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_utils.py
--rw-r--r--   0        0        0      178 2023-04-25 09:41:14.573026 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/requirements.txt
--rw-r--r--   0        0        0      171 2023-04-13 13:14:23.052881 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/setup.sh
--rw-r--r--   0        0        0    31060 2023-04-25 09:41:14.573856 evalda_pub2-0.0.2/evalda_pub2/coref_tasks/testing-coref.ipynb
--rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 evalda_pub2-0.0.2/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt
--rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 evalda_pub2-0.0.2/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt
--rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498742 evalda_pub2-0.0.2/evalda_pub2/data/abc_fem_sents.txt
--rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 evalda_pub2-0.0.2/evalda_pub2/data/abc_male_sents.txt
--rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv
--rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv
--rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv
--rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132606 evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv
--rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/unisex_names.csv
--rw-r--r--   0        0        0    13233 2023-05-11 11:08:09.654740 evalda_pub2-0.0.2/evalda_pub2/evalda_pub2.py
--rw-r--r--   0        0        0      427 2023-03-21 15:07:17.952937 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/__pycache__/evaluate.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-02-16 13:19:59.521115 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__init__.py
--rw-r--r--   0        0        0      198 2023-03-22 09:10:40.650810 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      434 2023-03-17 08:48:06.958238 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/apply_fn_scandi.cpython-39.pyc
--rw-r--r--   0        0        0      932 2023-03-22 14:48:24.602691 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/augmentation.cpython-39.pyc
--rw-r--r--   0        0        0      628 2023-03-23 13:05:20.448682 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/load_model.cpython-39.pyc
--rw-r--r--   0        0        0      726 2023-03-22 14:51:32.726951 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/overlap_fns.cpython-39.pyc
--rw-r--r--   0        0        0     2112 2023-03-23 07:54:42.282095 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/performance.cpython-39.pyc
--rw-r--r--   0        0        0     1557 2023-03-22 14:51:32.724071 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/process_names.cpython-39.pyc
--rw-r--r--   0        0        0     1097 2023-04-26 12:51:01.528045 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/augmentation.py
--rw-r--r--   0        0        0     1219 2023-05-03 17:07:48.135657 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/load_model.py
--rw-r--r--   0        0        0      409 2023-03-16 08:22:24.188834 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/overlap_fns.py
--rw-r--r--   0        0        0     3807 2023-05-03 17:07:48.136458 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/performance.py
--rw-r--r--   0        0        0     2695 2023-05-03 17:07:48.137155 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/process_names.py
--rw-r--r--   0        0        0      266 2023-05-03 17:07:48.137928 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/danish-bert_ner.csv
--rw-r--r--   0        0        0   155753 2023-05-03 17:07:48.139804 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png
--rw-r--r--   0        0        0      265 2023-05-03 17:07:48.140395 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_detailed.csv
--rw-r--r--   0        0        0      116 2023-05-03 17:07:48.140749 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_simple.csv
--rw-r--r--   0        0        0   172944 2023-05-03 17:07:48.143343 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png
--rw-r--r--   0        0        0      265 2023-05-03 17:07:48.143877 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_detailed.csv
--rw-r--r--   0        0        0      115 2023-05-03 17:07:48.144202 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_simple.csv
--rw-r--r--   0        0        0   137074 2023-05-03 17:07:48.146073 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png
--rw-r--r--   0        0        0      266 2023-05-03 17:07:48.146697 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_detailed.csv
--rw-r--r--   0        0        0      116 2023-05-03 17:07:48.147077 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_simple.csv
--rw-r--r--   0        0        0     1002 2023-05-03 17:07:48.147499 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/requirements-dacy-ner.txt
--rw-r--r--   0        0        0       82 2023-05-03 17:07:48.147901 evalda_pub2-0.0.2/evalda_pub2/ner_tasks/requirements-ner-minimum.txt
--rw-r--r--   0        0        0      625 2023-05-11 11:09:58.364013 evalda_pub2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 evalda_pub2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-23 10:21:49.117225 evalda_pub2-0.0.3/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-11 07:49:48.584000 evalda_pub2-0.0.3/README.md
+-rw-r--r--   0        0        0       49 2023-05-11 11:13:56.173871 evalda_pub2-0.0.3/evalda_pub2/__init__.py
+-rw-r--r--   0        0        0     6463 2023-04-19 16:13:42.482308 evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc
+-rw-r--r--   0        0        0     7757 2023-05-11 11:06:07.920873 evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-39.pyc
+-rw-r--r--   0        0        0      483 2023-04-19 16:13:46.716225 evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/load_model.cpython-38.pyc
+-rw-r--r--   0        0        0      483 2023-05-11 11:06:12.255364 evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/load_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3805 2023-04-19 16:13:50.367481 evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-38.pyc
+-rw-r--r--   0        0        0     5771 2023-05-11 11:06:15.805110 evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-39.pyc
+-rw-r--r--   0        0        0     9729 2023-05-03 17:07:47.956149 evalda_pub2-0.0.3/evalda_pub2/base_tasks/abc_lm_utilities.py
+-rw-r--r--   0        0        0    41806 2023-05-03 17:07:47.956965 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask-danish-bert-boxto.png
+-rw-r--r--   0        0        0    41198 2023-05-03 17:07:47.962956 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask-xlm-roberta-base.png
+-rw-r--r--   0        0        0    39889 2023-05-03 17:07:47.964069 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert-base.png
+-rw-r--r--   0        0        0      167 2023-05-03 17:07:47.964705 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert.csv
+-rw-r--r--   0        0        0      167 2023-05-03 17:07:47.965139 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask_xlm.csv
+-rw-r--r--   0        0        0   172315 2023-05-03 17:07:47.968269 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo.png
+-rw-r--r--   0        0        0      351 2023-05-03 17:07:47.969075 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo_detailed.csv
+-rw-r--r--   0        0        0      153 2023-05-03 17:07:47.969716 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo_simple.csv
+-rw-r--r--   0        0        0      321 2023-05-03 17:07:47.970113 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_nb-bert-base_detailed.csv
+-rw-r--r--   0        0        0      142 2023-05-03 17:07:47.970677 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_nb-bert-base_simple.csv
+-rw-r--r--   0        0        0   162904 2023-05-03 17:07:47.973083 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base.png
+-rw-r--r--   0        0        0      306 2023-05-03 17:07:47.974612 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base_detailed.csv
+-rw-r--r--   0        0        0      138 2023-05-03 17:07:47.974908 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base_simple.csv
+-rw-r--r--   0        0        0   136458 2023-05-03 17:07:47.976400 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large.png
+-rw-r--r--   0        0        0      308 2023-05-03 17:07:47.976765 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large_detailed.csv
+-rw-r--r--   0        0        0      138 2023-05-03 17:07:47.976940 evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large_simple.csv
+-rw-r--r--   0        0        0      256 2023-04-13 13:14:23.045077 evalda_pub2-0.0.3/evalda_pub2/base_tasks/load_model.py
+-rw-r--r--   0        0        0      208 2023-05-03 17:07:47.978516 evalda_pub2-0.0.3/evalda_pub2/base_tasks/requirements.txt
+-rw-r--r--   0        0        0     6576 2023-05-11 08:11:25.536312 evalda_pub2-0.0.3/evalda_pub2/base_tasks/wino_fillmask_utilities.py
+-rw-r--r--   0        0        0    47715 2023-05-03 17:07:47.981385 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_output/coref_abc.png
+-rw-r--r--   0        0        0   155593 2023-05-03 17:07:47.983658 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_output/coref_winobias.png
+-rw-r--r--   0        0        0      363 2023-05-03 17:07:47.984394 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_output/detailed_output_abc_coref.csv
+-rw-r--r--   0        0        0      168 2023-05-03 17:07:47.984949 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_output/detailed_output_coref_wino_xlm.csv
+-rw-r--r--   0        0        0    20070 2023-05-03 17:07:47.985819 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_utils.py
+-rw-r--r--   0        0        0      178 2023-04-25 09:41:14.573026 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/requirements.txt
+-rw-r--r--   0        0        0      171 2023-04-13 13:14:23.052881 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/setup.sh
+-rw-r--r--   0        0        0    31060 2023-04-25 09:41:14.573856 evalda_pub2-0.0.3/evalda_pub2/coref_tasks/testing-coref.ipynb
+-rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 evalda_pub2-0.0.3/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt
+-rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 evalda_pub2-0.0.3/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt
+-rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498742 evalda_pub2-0.0.3/evalda_pub2/data/abc_fem_sents.txt
+-rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 evalda_pub2-0.0.3/evalda_pub2/data/abc_male_sents.txt
+-rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv
+-rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv
+-rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv
+-rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132606 evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv
+-rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/unisex_names.csv
+-rw-r--r--   0        0        0    13233 2023-05-11 11:08:09.654740 evalda_pub2-0.0.3/evalda_pub2/evalda_pub2.py
+-rw-r--r--   0        0        0      427 2023-03-21 15:07:17.952937 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/__pycache__/evaluate.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-02-16 13:19:59.521115 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__init__.py
+-rw-r--r--   0        0        0      198 2023-03-22 09:10:40.650810 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      434 2023-03-17 08:48:06.958238 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/apply_fn_scandi.cpython-39.pyc
+-rw-r--r--   0        0        0      932 2023-03-22 14:48:24.602691 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/augmentation.cpython-39.pyc
+-rw-r--r--   0        0        0      628 2023-03-23 13:05:20.448682 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/load_model.cpython-39.pyc
+-rw-r--r--   0        0        0      726 2023-03-22 14:51:32.726951 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/overlap_fns.cpython-39.pyc
+-rw-r--r--   0        0        0     2112 2023-03-23 07:54:42.282095 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/performance.cpython-39.pyc
+-rw-r--r--   0        0        0     1557 2023-03-22 14:51:32.724071 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/process_names.cpython-39.pyc
+-rw-r--r--   0        0        0     1097 2023-04-26 12:51:01.528045 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/augmentation.py
+-rw-r--r--   0        0        0     1219 2023-05-03 17:07:48.135657 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/load_model.py
+-rw-r--r--   0        0        0      409 2023-03-16 08:22:24.188834 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/overlap_fns.py
+-rw-r--r--   0        0        0     3807 2023-05-03 17:07:48.136458 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/performance.py
+-rw-r--r--   0        0        0     2695 2023-05-03 17:07:48.137155 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/process_names.py
+-rw-r--r--   0        0        0      266 2023-05-03 17:07:48.137928 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/danish-bert_ner.csv
+-rw-r--r--   0        0        0   155753 2023-05-03 17:07:48.139804 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png
+-rw-r--r--   0        0        0      265 2023-05-03 17:07:48.140395 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_detailed.csv
+-rw-r--r--   0        0        0      116 2023-05-03 17:07:48.140749 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_simple.csv
+-rw-r--r--   0        0        0   172944 2023-05-03 17:07:48.143343 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png
+-rw-r--r--   0        0        0      265 2023-05-03 17:07:48.143877 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_detailed.csv
+-rw-r--r--   0        0        0      115 2023-05-03 17:07:48.144202 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_simple.csv
+-rw-r--r--   0        0        0   137074 2023-05-03 17:07:48.146073 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png
+-rw-r--r--   0        0        0      266 2023-05-03 17:07:48.146697 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_detailed.csv
+-rw-r--r--   0        0        0      116 2023-05-03 17:07:48.147077 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_simple.csv
+-rw-r--r--   0        0        0     1002 2023-05-03 17:07:48.147499 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/requirements-dacy-ner.txt
+-rw-r--r--   0        0        0       82 2023-05-03 17:07:48.147901 evalda_pub2-0.0.3/evalda_pub2/ner_tasks/requirements-ner-minimum.txt
+-rw-r--r--   0        0        0      646 2023-05-11 11:13:45.940938 evalda_pub2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 evalda_pub2-0.0.3/PKG-INFO
```

### Comparing `evalda_pub2-0.0.2/LICENSE` & `evalda_pub2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-39.pyc` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-38.pyc` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-39.pyc` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/abc_lm_utilities.py` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/abc_lm_utilities.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask-danish-bert-boxto.png` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask-danish-bert-boxto.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask-xlm-roberta-base.png` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask-xlm-roberta-base.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert-base.png` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert-base.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo.png` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base.png` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large.png` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/base_tasks/wino_fillmask_utilities.py` & `evalda_pub2-0.0.3/evalda_pub2/base_tasks/wino_fillmask_utilities.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_output/coref_abc.png` & `evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_output/coref_abc.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_output/coref_winobias.png` & `evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_output/coref_winobias.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/coref_tasks/coref_utils.py` & `evalda_pub2-0.0.3/evalda_pub2/coref_tasks/coref_utils.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/coref_tasks/testing-coref.ipynb` & `evalda_pub2-0.0.3/evalda_pub2/coref_tasks/testing-coref.ipynb`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt` & `evalda_pub2-0.0.3/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt` & `evalda_pub2-0.0.3/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/abc_fem_sents.txt` & `evalda_pub2-0.0.3/evalda_pub2/data/abc_fem_sents.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/abc_male_sents.txt` & `evalda_pub2-0.0.3/evalda_pub2/data/abc_male_sents.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv` & `evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv` & `evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv` & `evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv` & `evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/data/name_aug_csv_files/unisex_names.csv` & `evalda_pub2-0.0.3/evalda_pub2/data/name_aug_csv_files/unisex_names.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/evalda_pub2.py` & `evalda_pub2-0.0.3/evalda_pub2/evalda_pub2.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/augmentation.cpython-39.pyc` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/augmentation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/load_model.cpython-39.pyc` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/load_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/overlap_fns.cpython-39.pyc` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/overlap_fns.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/performance.cpython-39.pyc` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/performance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/__pycache__/process_names.cpython-39.pyc` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/__pycache__/process_names.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/augmentation.py` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/augmentation.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/load_model.py` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/load_model.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/performance.py` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/performance.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/helper_fns/process_names.py` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/helper_fns/process_names.py`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/evalda_pub2/ner_tasks/requirements-dacy-ner.txt` & `evalda_pub2-0.0.3/evalda_pub2/ner_tasks/requirements-dacy-ner.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.2/pyproject.toml` & `evalda_pub2-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "evalda-pub2"
-version = "0.0.2"
+version = "0.0.3"
 description = "A package for quantifying bias in Danish language models."
 authors = ["Astrid Rybner <astrid.rybner@hotmail.com>", 
         "Thea Rolskov <thearollesloth@hotmail.com>"]
 packages = [{include = "evalda_pub2"}]
 license = "MIT"
 repository = "https://github.com/DaDebias/evalda-pub2"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 spacy = "3.4.4"
 dacy = "2.3.1"
 augmenty = "1.3.1"
 protobuf = "3.20.3"
```

