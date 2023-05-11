# Comparing `tmp/g2p-1.0.20230417.tar.gz` & `tmp/g2p-1.1.20230511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-1.0.20230417.tar", last modified: Mon Apr 17 18:58:21 2023, max compression
+gzip compressed data, was "g2p-1.1.20230511.tar", last modified: Thu May 11 18:01:34 2023, max compression
```

## Comparing `g2p-1.0.20230417.tar` & `g2p-1.1.20230511.tar`

### file list

```diff
@@ -1,430 +1,431 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-17 18:58:05.000000 g2p-1.0.20230417/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-17 18:58:05.000000 g2p-1.0.20230417/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-17 18:58:21.870860 g2p-1.0.20230417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-04-17 18:58:05.000000 g2p-1.0.20230417/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.814860 g2p-1.0.20230417/g2p/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    28100 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.814860 g2p-1.0.20230417/g2p/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/create_fallback_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/create_ipa_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/alq/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/alq/alq_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/alq/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/atj/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/atj_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/atj/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/ckt/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ckt/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/clc/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/clc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/clc/doulos.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.822860 g2p-1.0.20230417/g2p/mappings/langs/crg/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/crg-dv-to-crg-ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crg/crg-tmd-to-crg-ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crj/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/crj_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crj/crj_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crk/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crk/crk_to_crk-no-symbols.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crl/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/crl_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crl/crl_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crm/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/crm_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crm/crm_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/crx/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crx/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/csw/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/csw_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/csw/csw_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.826860 g2p-1.0.20230417/g2p/mappings/langs/ctp/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ctp/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.830860 g2p-1.0.20230417/g2p/mappings/langs/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/dan_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/dan_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/dan/dan_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/eng/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  4215929 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/dummy_to_arpabet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/eng_inventory.json
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/make_alignments.sh
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/make_ipa_cmudict.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/eng/reverse_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/fin/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fin/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fin/fin_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/fn_unicode.csv
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/hei_doulos.csv
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/hei_times.csv
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/font-encodings/nav_times.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.834860 g2p-1.0.20230417/g2p/mappings/langs/fra/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/fra_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/fra/fra_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.838860 g2p-1.0.20230417/g2p/mappings/langs/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/alq-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/lml-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/see-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-17 18:58:05.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/git/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/APA.csv
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/Ortho_variables.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/Orthography.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/Orthography_Deterministic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/RAPA.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/RAPA_Deterministic.csv
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/git/git_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/gla/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gla/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gla/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gla/gla_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/gwi/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gwi/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gwi/gwi_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/gwi/gwi_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/haa/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/haa_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/haa_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/haa/haa_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/ikt/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ikt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ikt/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ikt/ikt_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/iku/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/iku_equiv_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/iku_sro_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/iku/iku_to_iku_equiv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.842860 g2p-1.0.20230417/g2p/mappings/langs/kkz/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kkz/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/kwk/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_napa_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_ubc.csv
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_uvic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/kwk/umista_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)  7050749 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/langs.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/lml/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/lml/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/lml/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/lml/lml_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/mic/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/mic/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/mic/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/mic/mic_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/moe_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moe/moe_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/moh/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/moh_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/moh_to_festival.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/moh/moh_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/network.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.846860 g2p-1.0.20230417/g2p/mappings/langs/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/norm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/norm/panphon_preprocessor.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/norm/tone-map.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/oji/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oji/oji_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/oka/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oka/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oka/oka_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/oka/oka_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/see/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/see/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/see/see_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/srs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/srs/config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/srs/srs_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/str/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/str_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/str/str_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tau/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tau/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tau/tau_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tau/tau_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tce/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/tce_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tce/tce_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tgx/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tgx/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/tli/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/tli_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/tli/tli_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.850860 g2p-1.0.20230417/g2p/mappings/langs/ttm/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/ttm_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/ttm/ttm_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.854860 g2p-1.0.20230417/g2p/mappings/langs/und/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/und/und_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.854860 g2p-1.0.20230417/g2p/mappings/langs/win/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/hoocak_alphabet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/langs/win/win_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/mappings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.854860 g2p-1.0.20230417/g2p/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/blockly_main.js
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/blocks.js
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    23193 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/echart_custom.js
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/languages-network.json
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/normalize.css
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/skeleton.css
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/static/swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.858860 g2p-1.0.20230417/g2p/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/templates/docs.html
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.862860 g2p-1.0.20230417/g2p/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.862860 g2p-1.0.20230417/g2p/tests/public/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.866860 g2p-1.0.20230417/g2p/tests/public/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crg.psv
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crj.psv
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crk.psv
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crl.psv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/crm.psv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/csw.psv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/ctp.csv
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/eng.csv
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fin.psv
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fn_unicode.psv
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra.psv
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams_NFD.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/fra_simple.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/git.psv
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/gwi.psv
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/haa.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/ikt.psv
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/iku-sro.psv
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/iku.psv
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/kwk.psv
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/lml.psv
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/mic.psv
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/moe.psv
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/moh.psv
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/oji-syl.psv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/oji.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/oka.csv
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/srs.psv
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/str.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/str_un_human_rights.txt
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/tau.psv
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/tce.csv
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/tli.csv
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/ttm.csv
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/data/win.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/git_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviation_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviation_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.psv
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.substring.csv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/abbreviations.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.810860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/lang1/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/lang1/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs/lang1/minimal.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.810860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/lang1/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/lang1/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_langs2/lang1/minimal.csv
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/bad_lexicon_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/cf-in-lc-to-cf-out-uc.csv
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/compose1-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/compose2-3.csv
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion.csv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion.json
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion_config_csv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/deletion_config_json.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/g2p_studio.csv
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/g2p_studio2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-1.csv
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map-3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gen-map_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gm1-ipa_to_gm2-ipa.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gm2-ipa_to_gm3-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/gm3-ipa_to_gm2-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/hello.aligned.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/lexicon_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/malformed_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.csv
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.psv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/minimal_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/no_escape.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/null.csv
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/null_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/rule-ordering.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/test_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/tokenize_punct.csv
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/mappings/tokenize_punct_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/public/sample_response.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4682 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_api_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_check_ipa_arpabet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16189 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6249 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_create_mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_doctor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_doctor_expensive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_fallback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23149 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_indices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_lexicon_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13478 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_mappings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10273 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_studio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5937 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_tokenize_and_map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5723 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_tokenizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11446 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_unidecode_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10830 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9835 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/test_z_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/tests/time_panphon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.870860 g2p-1.0.20230417/g2p/transducer/
--rw-r--r--   0 runner    (1001) docker     (123)    49089 2023-04-17 18:58:06.000000 g2p-1.0.20230417/g2p/transducer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:58:21.814860 g2p-1.0.20230417/g2p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 18:58:21.000000 g2p-1.0.20230417/g2p.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-17 18:58:21.874860 g2p-1.0.20230417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-17 18:58:06.000000 g2p-1.0.20230417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.611293 g2p-1.1.20230511/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-11 18:01:16.000000 g2p-1.1.20230511/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-11 18:01:16.000000 g2p-1.1.20230511/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-05-11 18:01:34.611293 g2p-1.1.20230511/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-11 18:01:16.000000 g2p-1.1.20230511/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.559293 g2p-1.1.20230511/g2p/
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28350 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.563294 g2p-1.1.20230511/g2p/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/create_fallback_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/create_ipa_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.567294 g2p-1.1.20230511/g2p/mappings/langs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/alq/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/alq/alq_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/alq/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/atj/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/atj/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/atj/atj_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/atj/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/ckt/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ckt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ckt/ckt_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ckt/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/clc/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/clc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/clc/doulos.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/crg/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crg/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crg/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crg/crg-dv-to-crg-ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crg/crg-tmd-to-crg-ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/crj/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crj/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crj/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crj/crj_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crj/crj_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/crk/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crk/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crk/crk_to_crk-no-symbols.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.571293 g2p-1.1.20230511/g2p/mappings/langs/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crl/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crl/crl_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crl/crl_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.575293 g2p-1.1.20230511/g2p/mappings/langs/crm/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crm/crm_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crm/crm_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.575293 g2p-1.1.20230511/g2p/mappings/langs/crx/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crx/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.575293 g2p-1.1.20230511/g2p/mappings/langs/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/csw/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/csw/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/csw/csw_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/csw/csw_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.575293 g2p-1.1.20230511/g2p/mappings/langs/ctp/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ctp/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ctp/ctp_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.575293 g2p-1.1.20230511/g2p/mappings/langs/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/dan/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/dan/dan_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/dan/dan_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/dan/dan_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.579293 g2p-1.1.20230511/g2p/mappings/langs/eng/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  4215929 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/dummy_to_arpabet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/eng_inventory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/make_alignments.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/make_ipa_cmudict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/eng/reverse_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.579293 g2p-1.1.20230511/g2p/mappings/langs/fin/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/fin/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/fin/fin_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.579293 g2p-1.1.20230511/g2p/mappings/langs/font-encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/font-encodings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/font-encodings/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/font-encodings/fn_unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/font-encodings/hei_doulos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/font-encodings/hei_times.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/font-encodings/nav_times.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.583293 g2p-1.1.20230511/g2p/mappings/langs/fra/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/fra/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/fra/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/fra/fra_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/fra/fra_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.587293 g2p-1.1.20230511/g2p/mappings/langs/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/alq-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/lml-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/moh-equiv_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/see-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/str-equiv_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/und-ascii_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.587293 g2p-1.1.20230511/g2p/mappings/langs/git/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/APA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/Ortho_variables.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/Orthography.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/Orthography_Deterministic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/RAPA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/RAPA_Deterministic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/git/git_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.587293 g2p-1.1.20230511/g2p/mappings/langs/gla/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/gla/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/gla/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/gla/gla_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.587293 g2p-1.1.20230511/g2p/mappings/langs/gwi/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/gwi/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/gwi/gwi_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/gwi/gwi_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.587293 g2p-1.1.20230511/g2p/mappings/langs/haa/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/haa/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/haa/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/haa/haa_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/haa/haa_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/haa/haa_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.587293 g2p-1.1.20230511/g2p/mappings/langs/ikt/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ikt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ikt/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ikt/ikt_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/iku/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/iku/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/iku/iku_equiv_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/iku/iku_sro_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/iku/iku_to_iku_equiv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/kkz/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kkz/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kkz/kkz_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/kwk/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_napa_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/napa_equiv_ubc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/napa_equiv_uvic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/kwk/umista_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  7050749 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/langs.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/lml/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/lml/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/lml/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/lml/lml_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/mic/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/mic/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/mic/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/mic/mic_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moe/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moe/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moe/moe_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moe/moe_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/moh/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moh/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moh/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moh/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moh/moh_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moh/moh_to_festival.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/moh/moh_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/network.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.591293 g2p-1.1.20230511/g2p/mappings/langs/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/norm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/norm/panphon_preprocessor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/norm/tone-map.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/oji/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/oji/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/oji/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/oji/oji_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/oka/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/oka/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/oka/oka_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/oka/oka_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/see/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/see/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/see/see_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/srs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/srs/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/srs/srs_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/str/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/str/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/str/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/str/str_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/str/str_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/tau/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tau/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tau/tau_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tau/tau_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/tce/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tce/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tce/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tce/tce_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tce/tce_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/tgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tgx/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tgx/tgx_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/tli/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tli/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tli/tli_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/tli/tli_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/ttm/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ttm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ttm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ttm/ttm_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/ttm/ttm_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.595293 g2p-1.1.20230511/g2p/mappings/langs/und/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/und/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/und/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/und/und_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.599293 g2p-1.1.20230511/g2p/mappings/langs/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/win/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/win/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/win/hoocak_alphabet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/langs/win/win_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/mappings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.599293 g2p-1.1.20230511/g2p/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/blockly_main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/blocks.js
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23193 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/echart_custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/languages-network.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/skeleton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/static/swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.599293 g2p-1.1.20230511/g2p/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/templates/docs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.603293 g2p-1.1.20230511/g2p/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.603293 g2p-1.1.20230511/g2p/tests/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.607293 g2p-1.1.20230511/g2p/tests/public/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/crg.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/crj.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/crk.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/crl.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/crm.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/csw.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/ctp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/eng.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/fin.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/fn_unicode.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/fra.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/fra_panagrams.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/fra_panagrams_NFD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/fra_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/git.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/gwi.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/haa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/ikt.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/iku-sro.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/iku.psv
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/kwk.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/lml.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/mic.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/moe.psv
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/moh.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/oji-syl.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/oji.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/oka.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/srs.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/str.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/str_un_human_rights.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/tau.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/tce.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/tli.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/ttm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/data/win.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/git_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.611293 g2p-1.1.20230511/g2p/tests/public/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/abbreviation_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/abbreviation_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/abbreviations.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/abbreviations.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/abbreviations.substring.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/abbreviations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.559293 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.611293 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs/lang1/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs/lang1/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs/lang1/minimal.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.559293 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.611293 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs2/lang1/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs2/lang1/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/bad_langs2/lang1/minimal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/bad_lexicon_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.611293 g2p-1.1.20230511/g2p/tests/public/mappings/case-feed/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/case-feed/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/case-feed/cf-in-lc-to-cf-out-uc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/case-feed/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/case-feed/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/compose1-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/compose2-3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/deletion.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/deletion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/deletion_config_csv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/deletion_config_json.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/g2p_studio.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/g2p_studio2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gen-map-1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gen-map-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gen-map-3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gen-map-3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gen-map_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gm1-ipa_to_gm2-ipa.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gm2-ipa_to_gm3-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/gm3-ipa_to_gm2-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/hello.aligned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/lexicon_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/malformed_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/minimal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/minimal.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/minimal.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/minimal.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/minimal_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/minimal_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/no_escape.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/null.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/null_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/rule-ordering.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/test_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/tokenize_punct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/mappings/tokenize_punct_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/public/sample_response.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4682 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6103 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_api_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5157 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_check_ipa_arpabet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18637 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6249 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_create_mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_doctor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_doctor_expensive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_fallback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23149 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_indices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_lexicon_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14061 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_mappings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11204 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_studio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7906 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_tokenize_and_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5723 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_tokenizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11446 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2565 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_unidecode_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10830 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10145 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/test_z_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/tests/time_panphon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.611293 g2p-1.1.20230511/g2p/transducer/
+-rw-r--r--   0 runner    (1001) docker     (123)    49068 2023-05-11 18:01:16.000000 g2p-1.1.20230511/g2p/transducer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:01:34.563294 g2p-1.1.20230511/g2p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-05-11 18:01:34.000000 g2p-1.1.20230511/g2p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-05-11 18:01:34.000000 g2p-1.1.20230511/g2p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:01:34.000000 g2p-1.1.20230511/g2p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 18:01:34.000000 g2p-1.1.20230511/g2p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:01:34.000000 g2p-1.1.20230511/g2p.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-11 18:01:34.000000 g2p-1.1.20230511/g2p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-11 18:01:34.000000 g2p-1.1.20230511/g2p.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-11 18:01:34.611293 g2p-1.1.20230511/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 18:01:16.000000 g2p-1.1.20230511/setup.py
```

### Comparing `g2p-1.0.20230417/LICENSE` & `g2p-1.1.20230511/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/PKG-INFO` & `g2p-1.1.20230511/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p
-Version: 1.0.20230417
+Version: 1.1.20230511
 Summary: Module for creating context-aware, rule-based G2P mappings that preserve indices
 Home-page: https://github.com/roedoejet/g2p
 Author: Aidan Pine
 Author-email: hello@aidanpine.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `g2p-1.0.20230417/README.md` & `g2p-1.1.20230511/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/__init__.py` & `g2p-1.1.20230511/g2p/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,109 @@
 """
 
 Basic init file for g2p module
 
 The main entry points for the g2p module are:
  - make_g2p() to create a mapper from and lang to another
- - make_tokenizer() to create a tokenizeer for a given language
+ - make_tokenizer() to create a tokenizer for a given language
  - get_arpabet_langs() to get the list of languages with a path to eng-arpabet
 
 Basic Usage:
     from g2p import make_g2p
-    converter = make_g2p(in_lang, out_lang, tok_lang)
+    converter = make_g2p(in_lang, out_lang)
     transduction_graph = converter(input_text_in_in_alang)
     converted_text_in_out_lang = transduction_graph.output_string
 
     from g2p import make_tokenizer
     tokenizer = make_tokenizer(lang)
     list_of_tokens = tokenizer.tokenize_text(input_text)
 
     from g2p import get_arpabet_langs
     LANGS, LANG_NAMES = get_arpabet_langs()
 """
-import sys
 from typing import Dict, Optional, Tuple, Union
 
 from networkx import has_path, shortest_path
 from networkx.exception import NetworkXNoPath
 
+import g2p.deprecation
 from g2p.exceptions import InvalidLanguageCode, NoPath
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.langs import LANGS, LANGS_NETWORK
-from g2p.mappings.tokenizer import make_tokenizer
+from g2p.mappings.tokenizer import Tokenizer, make_tokenizer
 from g2p.transducer import CompositeTransducer, TokenizingTransducer, Transducer
 
-if sys.version_info < (3, 6):
-    sys.exit(
-        f"Python 3.6 or more recent is required. You are using {sys.version}.\n"
-        "Please use a newer version of Python."
-    )
-
 
 _g2p_cache: Dict[
-    Tuple[str, str, Optional[str]],
+    Tuple[str, str, Optional[str], bool, int],
     Union[Transducer, CompositeTransducer, TokenizingTransducer],
 ] = {}
 
 
-def make_g2p(in_lang: str, out_lang: str, tok_lang: Optional[str] = None):
+def make_g2p(  # noqa: C901
+    in_lang: str,
+    out_lang: str,
+    tok_lang: Optional[str] = None,  # DEPRECATED
+    *,
+    tokenize: bool = True,
+    custom_tokenizer: Optional[Tokenizer] = None,
+):
     """Make a g2p Transducer for mapping text from in_lang to out_lang via the
     shortest path between them.
 
-    In general you should also add `tok_lang` to specify the language
-    for tokenization (probably the same as `in_lang`), because
-    transducers are not guaranteed to deal with whitespace,
+    By default, the input is tokenized using the path of mappings from in_lang
+    to out_lang, because transducers are not guaranteed to deal with whitespace,
     punctuation, etc, properly.
 
     Args:
         in_lang (str): input language code
         out_lang (str): output language code
-        tok_lang (Optional[str]): language for tokenization
+        tok_lang (Optional[str]): DEPRECATED language for tokenization
+        tokenize (bool): whether tokenization should happen (default: True)
+        custom_tokenizer (Tokenizer): the tokenizer to use (default: a tokenizer
+                                      built on the path from in_lang and out_lang)
 
     Returns:
         Transducer from in_lang to out_lang, optionally with a tokenizer.
 
     Raises:
         InvalidLanguageCode: if in_lang or out_lang don't exist
         NoPath: if there is path between in_lang and out_lang
-
     """
-    if (in_lang, out_lang, tok_lang) in _g2p_cache:
-        return _g2p_cache[(in_lang, out_lang, tok_lang)]
+
+    if (in_lang, out_lang, tok_lang, tokenize, id(custom_tokenizer)) in _g2p_cache:
+        return _g2p_cache[(in_lang, out_lang, tok_lang, tokenize, id(custom_tokenizer))]
+
+    g2p.deprecation.handle_tok_lang_deprecation(tok_lang)
 
     # Check in_lang is a node in network
     if in_lang not in LANGS_NETWORK.nodes:
         LOGGER.error(f"No lang called '{in_lang}'. Please try again.")
         raise InvalidLanguageCode(in_lang)
 
     # Check out_lang is a node in network
     if out_lang not in LANGS_NETWORK.nodes:
         LOGGER.error(f"No lang called '{out_lang}'. Please try again.")
         raise InvalidLanguageCode(out_lang)
 
     if in_lang == out_lang:
         LOGGER.error(
-            "Sorry, you can't transduce between the same language. Please select a different output language code."
+            "Sorry, you can't transduce between the same language. "
+            "Please select a different output language code."
         )
         raise NoPath(in_lang, out_lang)
 
     # Try to find the shortest path between the nodes
     try:
         path = shortest_path(LANGS_NETWORK, in_lang, out_lang)
     except NetworkXNoPath as e:
         LOGGER.error(
-            f"Sorry, we couldn't find a way to convert {in_lang} to {out_lang}. Please update your langs by running `g2p update` and try again."
+            f"Sorry, we couldn't find a way to convert {in_lang} to {out_lang}. "
+            "Please update your langs by running `g2p update` and try again."
         )
         raise NoPath(in_lang, out_lang) from e
 
     # Find all mappings needed
     mappings_needed = []
     for lang1, lang2 in zip(path[:-1], path[1:]):
         mapping = Mapping(in_lang=lang1, out_lang=lang2)
@@ -109,22 +116,26 @@
     transducer: Union[Transducer, CompositeTransducer, TokenizingTransducer]
     if len(mappings_needed) == 1:
         transducer = Transducer(mappings_needed[0])
     else:
         transducer = CompositeTransducer([Transducer(x) for x in mappings_needed])
 
     # If tokenization was requested, return a TokenizingTransducer
-    if tok_lang:
-        if tok_lang == "path":
+    if custom_tokenizer:
+        transducer = TokenizingTransducer(transducer, custom_tokenizer)
+    elif tokenize or tok_lang:
+        if (tok_lang == "path") or (tokenize and not tok_lang):
             tokenizer = make_tokenizer(in_lang=in_lang, tok_path=path)
         else:
             tokenizer = make_tokenizer(in_lang=tok_lang)
         transducer = TokenizingTransducer(transducer, tokenizer)
 
-    _g2p_cache[(in_lang, out_lang, tok_lang)] = transducer
+    _g2p_cache[
+        (in_lang, out_lang, tok_lang, tokenize, id(custom_tokenizer))
+    ] = transducer
     return transducer
 
 
 def tokenize_and_map(tokenizer, transducer, input: str):
     result = ""
     for token in tokenizer.tokenize_text(input):
         if token["is_word"]:
```

### Comparing `g2p-1.0.20230417/g2p/api.py` & `g2p-1.1.20230511/g2p/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,24 +106,34 @@
             dest="debugger",
             type=inputs.boolean,
             location="args",
             default=False,
             required=False,
             help="Debugging information about the transduction process",
         )
+        self.parser.add_argument(
+            "tokenize",
+            dest="tokenize",
+            type=inputs.boolean,
+            location="args",
+            default=False,
+            required=False,
+            help="Tokenize before transducing",
+        )
 
     def get(self):
         args = self.parser.parse_args()
         in_lang = args["in-lang"]
         out_lang = args["out-lang"]
         text = args["text"]
         index = args["index"]
         debugger = args["debugger"]
+        tokenize = args["tokenize"]
         try:
-            transducer = make_g2p(in_lang, out_lang)
+            transducer = make_g2p(in_lang, out_lang, tokenize=tokenize)
             tg = transducer(text)
             text = tg.output_string
             input_text = tg.input_string
             debugger = tg.debugger if debugger else debugger
             index = tg.edges if index else index
             return {
                 "input-text": input_text,
```

### Comparing `g2p-1.0.20230417/g2p/app.py` & `g2p-1.1.20230511/g2p/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,15 +161,17 @@
         output_string = transducer(message["data"]["input_string"]).output_string
         emit("conversion response", {"output_string": output_string})
 
 
 @SOCKETIO.on("table event", namespace="/table")
 def change_table(message):
     """Change the lookup table"""
-    if message["in_lang"] == "custom" or message["out_lang"] == "custom":
+    if "in_lang" not in message or "out_lang" not in message:
+        emit("table response", [])
+    elif message["in_lang"] == "custom" or message["out_lang"] == "custom":
         # These are only used to generate JSON to send to the client,
         # so it's safe to create a list of references to the same thing.
         mappings = [
             {"in": "", "out": "", "context_before": "", "context_after": ""}
         ] * DEFAULT_N
         abbs = [[""] * 6] * DEFAULT_N
         kwargs = {
@@ -194,25 +196,19 @@
                     "mappings": mappings,
                     "abbs": abbs,
                     "kwargs": kwargs,
                 }
             ],
         )
     else:
-        # Do not create a composite transducer just to decompose it,
-        # because it is the individual ones which are cached by g2p
         path = shortest_path(LANGS_NETWORK, message["in_lang"], message["out_lang"])
-        if len(path) == 1:
-            transducer = make_g2p(message["in_lang"], message["out_lang"])
-            mappings = [transducer.mapping]
-        else:
-            mappings = []
-            for lang1, lang2 in zip(path[:-1], path[1:]):
-                transducer = make_g2p(lang1, lang2)
-                mappings.append(transducer.mapping)
+        mappings = []
+        for lang1, lang2 in zip(path[:-1], path[1:]):
+            transducer = make_g2p(lang1, lang2, tokenize=False)
+            mappings.append(transducer.mapping)
         emit(
             "table response",
             [
                 {
                     "mappings": x.plain_mapping(),
                     "abbs": expand_abbreviations_format(x.abbreviations),
                     "kwargs": x.kwargs,
```

### Comparing `g2p-1.0.20230417/g2p/cli.py` & `g2p-1.1.20230511/g2p/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 
 import click
 import yaml
 from flask.cli import FlaskGroup
 from networkx import has_path
 
-from g2p import make_g2p
+from g2p import make_g2p, make_tokenizer
 from g2p._version import VERSION
 from g2p.api import update_docs
 from g2p.app import APP
 from g2p.exceptions import InvalidLanguageCode, MappingMissing, NoPath
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.create_fallback_mapping import (
@@ -31,14 +31,15 @@
 )
 from g2p.mappings.langs import (
     LANGS_DIR,
     LANGS_NETWORK,
     LANGS_PKL_NAME,
     MAPPINGS_AVAILABLE,
     NETWORK_PKL_NAME,
+    reload_db,
 )
 from g2p.mappings.langs.utils import (
     cache_langs,
     check_ipa_known_segs,
     network_to_echart,
 )
 from g2p.mappings.utils import is_ipa, is_xsampa, load_mapping_from_path, normalize
@@ -469,20 +470,15 @@
     help="Override the tokenizing language. Implies --tok.",
 )
 @click.option(
     "--tok/--no-tok",
     "-t",
     default=None,  # three-way var: None=not set, True/False=set to True/False
     is_flag=True,
-    help="Tokenize INPUT_TEXT before converting.",
-)
-@click.option(
-    "--path",
-    type=click.Path(exists=True, file_okay=True, dir_okay=False),
-    help="Read text to convert from FILE.",
+    help="Tokenize INPUT_TEXT before converting. Default is --tok, specify --no-tok to turn off.",
 )
 @click.option(
     "--config",
     type=click.Path(exists=True, file_okay=True, dir_okay=False),
     help="A path to a mapping configuration file to use",
 )
 @click.argument("out_lang")
@@ -492,15 +488,14 @@
     context_settings=CONTEXT_SETTINGS,
     short_help="Convert text through a g2p mapping path.",
 )
 def convert(  # noqa: C901
     in_lang,
     out_lang,
     input_text,
-    path,
     tok,
     check,
     debugger,
     pretty_edges,
     tok_lang,
     config,
     substring_alignments,
@@ -556,21 +551,22 @@
         )
     if os.path.exists(input_text) and input_text.endswith("txt"):
         with open(input_text, encoding="utf8") as f:
             input_text = f.read()
     # Determine which tokenizer to use, if any
     if tok is not None and not tok and tok_lang is not None:
         raise click.UsageError("Specified conflicting --no-tok and --tok-lang options.")
-    if tok and tok_lang is None:
-        tok_lang = "path"
+    if tok is None:
+        tok = True  # Tokenize by default
+    custom_tokenizer = make_tokenizer(tok_lang) if tok_lang else None
     # Transduce!!!
-    if in_lang and out_lang:
-        transducer = make_g2p(in_lang, out_lang, tok_lang=tok_lang)
-    elif path:
-        transducer = Transducer(Mapping(path))
+    assert in_lang and out_lang
+    transducer = make_g2p(
+        in_lang, out_lang, tokenize=tok, custom_tokenizer=custom_tokenizer
+    )
     tg = transducer(input_text)
     if check:
         transducer.check(tg, display_warnings=True)
     outputs = [tg.output_string]
     if substring_alignments:
         outputs += [tg.substring_alignments()]
     if pretty_edges:
@@ -665,18 +661,22 @@
     if out_dir is None:
         langs_path = os.path.join(in_dir, LANGS_PKL_NAME)
         network_path = os.path.join(in_dir, NETWORK_PKL_NAME)
     else:
         langs_path = os.path.join(out_dir, LANGS_PKL_NAME)
         network_path = os.path.join(out_dir, NETWORK_PKL_NAME)
     cache_langs(dir_path=in_dir, langs_path=langs_path, network_path=network_path)
-    update_docs()
-    network_to_echart(
-        outfile=os.path.join(os.path.dirname(static_file), "languages-network.json")
-    )
+
+    if in_dir == LANGS_DIR and out_dir is None:
+        # We only update the documentation when updating using the default directories
+        reload_db()
+        update_docs()  # updates g2p/static/swagger.json
+        network_to_echart(
+            outfile=os.path.join(os.path.dirname(static_file), "languages-network.json")
+        )  # updates g2p/status/languages-network.json
 
 
 @click.argument("path", type=click.Path(exists=True, file_okay=True, dir_okay=False))
 @click.argument("lang")
 @cli.command(
     context_settings=CONTEXT_SETTINGS,
     short_help="Scan a document for unknown characters.",
@@ -738,15 +738,15 @@
     Mappings on the path from LANG1 to LANG2 are displayed.
     If only LANG1 is used, all mappings to or from LANG1 are displayed.
     With no LANG, all cached mappings are included.
     """
 
     if lang1 is not None and lang2 is not None:
         try:
-            transducer = make_g2p(lang1, lang2)
+            transducer = make_g2p(lang1, lang2, tokenize=False)
         except (NoPath, InvalidLanguageCode) as e:
             raise click.UsageError(
                 f'Cannot find mapping from "{lang1}" to "{lang2}": {e}'
             ) from e
 
         if isinstance(transducer, Transducer):
             mappings = [transducer.mapping]
```

### Comparing `g2p-1.0.20230417/g2p/exceptions.py` & `g2p-1.1.20230511/g2p/exceptions.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/__init__.py` & `g2p-1.1.20230511/g2p/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/create_fallback_mapping.py` & `g2p-1.1.20230511/g2p/mappings/create_fallback_mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     config = {"in_lang": mapping.kwargs[f"{io}_lang"], "out_lang": "dummy"}
     default_char = "t"
     if is_ipa(mapping.kwargs[f"{io}_lang"]):
         mapping = align_inventories(
             mapping.inventory(io), DUMMY_INVENTORY, distance=distance, quiet=quiet
         )
     else:
-        und_g2p = make_g2p("und", "und-ipa")
+        und_g2p = make_g2p("und", "und-ipa", tokenize=False)
         mapping = [
             {
                 "in": unicode_escape(x),
                 "out": und_g2p(unidecode(x).lower()).output_string,
             }
             for x in mapping.inventory(io)
         ]
```

### Comparing `g2p-1.0.20230417/g2p/mappings/create_ipa_mapping.py` & `g2p-1.1.20230511/g2p/mappings/create_ipa_mapping.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/__init__.py` & `g2p-1.1.20230511/g2p/mappings/langs/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,45 +20,67 @@
         with open(path, "rb") as f:
             return pickle.load(f)
     except Exception as e:
         LOGGER.warning(f"Failed to read language cache from {path}: {e}")
         return {}
 
 
-LANGS = load_langs()
-
-
 def load_network(path: str = LANGS_NWORK_PATH):
     try:
         return read_gpickle(path)
     except Exception as e:
         LOGGER.warning(f"Failed to read language network from {path}: {e}")
         return DiGraph()
 
 
-def get_available_languages(langs: dict = LANGS) -> list:
+def get_available_languages(langs: dict) -> list:
     language_names = set()
     for k, v in langs.items():
         if k in ["generated", "font-encodings"]:
             continue
         if "mappings" in v:
             for vv in v["mappings"]:
                 if "language_name" in vv:
                     language_names.add(vv["language_name"])
         elif "language_name" in v:
             language_names.add(v["language_name"])
     return sorted(language_names)
 
 
-def get_available_mappings(langs: dict = LANGS) -> list:
+def get_available_mappings(langs: dict) -> list:
     mappings_available = []
-    for k, v in LANGS.items():
+    for k, v in langs.items():
         if "mappings" in v:
             mappings_available.extend(v["mappings"])
         else:
             mappings_available.append(v)
     return mappings_available
 
 
+LANGS = load_langs()
 LANGS_NETWORK = load_network()
-LANGS_AVAILABLE = get_available_languages()
-MAPPINGS_AVAILABLE = get_available_mappings()
+LANGS_AVAILABLE = get_available_languages(LANGS)
+MAPPINGS_AVAILABLE = get_available_mappings(LANGS)
+
+
+def reload_db():
+    """Reload the langs and network data, necessary after a g2p update."""
+
+    # We update all structures in place, so that another module having done from
+    # g2p.mappings.langs import VAR will see the udpates without any code changes.
+
+    global LANGS
+    LANGS.clear()
+    LANGS.update(load_langs())
+
+    global LANGS_NETWORK
+    LANGS_NETWORK.clear()
+    new_langs_network = load_network()
+    LANGS_NETWORK.update(new_langs_network.edges, new_langs_network.nodes)
+
+    global LANGS_AVAILABLE
+    LANGS_AVAILABLE.clear()
+    LANGS_AVAILABLE.extend(get_available_languages(LANGS))
+
+    global MAPPINGS_AVAILABLE
+    MAPPINGS_AVAILABLE.clear()
+    MAPPINGS_AVAILABLE.extend(get_available_mappings(LANGS))
```

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/atj/atj_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/atj/atj_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/ckt/ckt_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/ckt/ckt_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crg/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/crg/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crj/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/crj/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crj/crj_equiv.json` & `g2p-1.1.20230511/g2p/mappings/langs/crj/crj_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crj/crj_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/crj/crj_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crk/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/crk/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crl/README.md` & `g2p-1.1.20230511/g2p/mappings/langs/crl/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crl/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/crl/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crl/crl_equiv.json` & `g2p-1.1.20230511/g2p/mappings/langs/crl/crl_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crl/crl_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/crl/crl_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crm/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/crm/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crm/crm_equiv.json` & `g2p-1.1.20230511/g2p/mappings/langs/crm/crm_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crm/crm_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/crm/crm_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv` & `g2p-1.1.20230511/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv` & `g2p-1.1.20230511/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/csw/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/csw/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/csw/csw_equiv.json` & `g2p-1.1.20230511/g2p/mappings/langs/csw/csw_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/csw/csw_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/csw/csw_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/ctp/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/ctp/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/ctp/ctp_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/ctp/ctp_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/dan/dan_to_dummy.json` & `g2p-1.1.20230511/g2p/mappings/langs/dan/dan_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/eng/README.md` & `g2p-1.1.20230511/g2p/mappings/langs/eng/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt` & `g2p-1.1.20230511/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/eng/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/eng/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json` & `g2p-1.1.20230511/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/eng/make_alignments.sh` & `g2p-1.1.20230511/g2p/mappings/langs/eng/make_alignments.sh`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/eng/make_ipa_cmudict.py` & `g2p-1.1.20230511/g2p/mappings/langs/eng/make_ipa_cmudict.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/font-encodings/README.md` & `g2p-1.1.20230511/g2p/mappings/langs/font-encodings/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/font-encodings/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/font-encodings/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/font-encodings/fn_unicode.csv` & `g2p-1.1.20230511/g2p/mappings/langs/font-encodings/fn_unicode.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/fra/README.txt` & `g2p-1.1.20230511/g2p/mappings/langs/fra/README.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/fra/fra_to_ipa.csv` & `g2p-1.1.20230511/g2p/mappings/langs/fra/fra_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/generated/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_dummy.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/moh-equiv_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_dummy.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/str-equiv_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_dummy.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/und-ascii_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/APA.csv` & `g2p-1.1.20230511/g2p/mappings/langs/git/APA.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/Orthography.csv` & `g2p-1.1.20230511/g2p/mappings/langs/git/Orthography.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/Orthography_Deterministic.csv` & `g2p-1.1.20230511/g2p/mappings/langs/git/Orthography_Deterministic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/RAPA.csv` & `g2p-1.1.20230511/g2p/mappings/langs/git/RAPA.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/RAPA_Deterministic.csv` & `g2p-1.1.20230511/g2p/mappings/langs/git/RAPA_Deterministic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/git/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/git/git_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/git/git_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/gla/gla_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/gla/gla_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/gwi/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/gwi/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/gwi/gwi_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/gwi/gwi_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/haa/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/haa/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/haa/haa_abbs.csv` & `g2p-1.1.20230511/g2p/mappings/langs/haa/haa_abbs.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/haa/haa_to_ipa.csv` & `g2p-1.1.20230511/g2p/mappings/langs/haa/haa_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/ikt/ikt_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/ikt/ikt_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/iku/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/iku/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/iku/iku_equiv_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/iku/iku_equiv_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/iku/iku_sro_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/iku/iku_sro_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/iku/iku_to_iku_equiv.json` & `g2p-1.1.20230511/g2p/mappings/langs/iku/iku_to_iku_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kkz/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/kkz/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kkz/kkz_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/kkz/kkz_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_ubc.csv` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/napa_equiv_ubc.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/napa_equiv_uvic.csv` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/napa_equiv_uvic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/kwk/umista_equiv.csv` & `g2p-1.1.20230511/g2p/mappings/langs/kwk/umista_equiv.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/langs.pkl` & `g2p-1.1.20230511/g2p/mappings/langs/langs.pkl`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/mic/mic_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/mic/mic_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/moe/moe_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/moe/moe_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/moh/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/moh/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/moh/moh_equiv.json` & `g2p-1.1.20230511/g2p/mappings/langs/moh/moh_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/moh/moh_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/moh/moh_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/network.pkl` & `g2p-1.1.20230511/g2p/mappings/langs/network.pkl`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/norm/tone-map.txt` & `g2p-1.1.20230511/g2p/mappings/langs/norm/tone-map.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/oji/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/oji/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv` & `g2p-1.1.20230511/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/srs/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/srs/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/srs/srs_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/srs/srs_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/str/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/str/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/str/str_equiv.json` & `g2p-1.1.20230511/g2p/mappings/langs/str/str_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/str/str_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/str/str_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tau/config.yml` & `g2p-1.1.20230511/g2p/mappings/langs/tau/config.yml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tau/tau_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/tau/tau_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tce/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/tce/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tce/tce_to_ipa.csv` & `g2p-1.1.20230511/g2p/mappings/langs/tce/tce_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tgx/config.yml` & `g2p-1.1.20230511/g2p/mappings/langs/tgx/config.yml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tgx/tgx_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/tgx/tgx_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tli/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/tli/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/tli/tli_to_ipa.csv` & `g2p-1.1.20230511/g2p/mappings/langs/tli/tli_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/ttm/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/ttm/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/und/config.yaml` & `g2p-1.1.20230511/g2p/mappings/langs/und/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/und/und_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/und/und_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/utils.py` & `g2p-1.1.20230511/g2p/mappings/langs/utils.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/langs/win/win_to_ipa.json` & `g2p-1.1.20230511/g2p/mappings/langs/win/win_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/mappings/tokenizer.py` & `g2p-1.1.20230511/g2p/mappings/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 from g2p.exceptions import MappingMissing
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.langs import LANGS_NETWORK
 from g2p.mappings.utils import get_unicode_category, is_ipa, merge_if_same_label
 
 
-class DefaultTokenizer:
+class Tokenizer:
+    """Base class for all g2p tokenizers; implements the default tokenizing behaviour.
+
+    By default, a token is defined as a sequence of letters, numbers and
+    diacritics, as defined in the Unicode Standard.
+    """
+
     def __init__(self):
         self.inventory = []
         self.delim = ""
         self.case_sensitive = False
         # Hack for Tlingit where . is a letter when not word final:
         self.dot_is_letter = False
 
@@ -50,15 +56,15 @@
                     and units[i + 1]["is_word"]
                 ):
                     unit["is_word"] = True
         units = merge_if_same_label(units, "text", "is_word")
         return units
 
 
-class Tokenizer(DefaultTokenizer):
+class SpecializedTokenizer(Tokenizer):
     def __init__(self, mapping: Mapping):
         self.inventory = mapping.inventory("in")
         self.lang = mapping.kwargs.get("language_name", "")
         self.delim = mapping.kwargs.get("in_delimiter", "")
         self.case_sensitive = mapping.kwargs.get("case_sensitive", True)
         self.dot_is_letter = False
         # create regex
@@ -87,15 +93,15 @@
             flags |= re.I
         self.regex = re.compile(pattern, flags)
 
     def tokenize_aux(self, text):
         return self.regex.findall(text)
 
 
-class MultiHopTokenizer(Tokenizer):
+class MultiHopTokenizer(SpecializedTokenizer):
     def __init__(self, mappings: list):
         assert mappings
         self.inventory = sum([m.inventory("in") for m in mappings], [])
         self.lang = mappings[0].kwargs.get("language_name", "")
         self.delim = mappings[0].kwargs.get("in_delimiter", "")
         self.case_sensitive = mappings[0].kwargs.get("case_sensitive", True)
         self.dot_is_letter = False
@@ -107,26 +113,28 @@
     """
     The TokenizerLibrary holds the collection of tokenizers that have been
     initialized so far. We don't initialize them all since that takes costly
     loading time; instead, we initialize each only as requested.
     """
 
     def __init__(self):
-        self.tokenizers = {None: DefaultTokenizer()}
+        self.tokenizers = {None: Tokenizer()}
 
     def make_tokenizer_key(self, in_lang, out_lang=None, tok_path=None):
         if not in_lang:
             return None
         if tok_path:
             return in_lang + "+tok_path=" + "-to-".join(tok_path)
         if not out_lang:
             out_lang = in_lang + "-ipa"
         return in_lang + "-to-" + out_lang
 
-    def make_tokenizer(self, in_lang, out_lang=None, tok_path=None):  # noqa C901
+    def make_tokenizer(  # noqa C901
+        self, in_lang, out_lang=None, tok_path=None
+    ) -> Tokenizer:
         tokenizer_key = self.make_tokenizer_key(in_lang, out_lang, tok_path)
         if not self.tokenizers.get(tokenizer_key):
             # This tokenizer was not created yet, initialize it now.
             if tok_path:
                 # LOGGER.warning(f"in_lang={in_lang} tok_path={tok_path}")
                 if tok_path[0] != in_lang:
                     raise ValueError(
@@ -185,15 +193,15 @@
                     LOGGER.warning(
                         f"missing mapping yet we looked for mappings in graph for {in_lang}-{out_lang}."
                     )
             else:
                 # Build a one-hop tokenizer
                 try:
                     mapping = Mapping(in_lang=in_lang, out_lang=out_lang)
-                    self.tokenizers[tokenizer_key] = Tokenizer(mapping)
+                    self.tokenizers[tokenizer_key] = SpecializedTokenizer(mapping)
                 except MappingMissing:
                     self.tokenizers[tokenizer_key] = self.tokenizers[None]
                     LOGGER.warning(
                         f"Cannot find mapping from '{in_lang}' to '{out_lang}'. Using default tokenizer instead"
                     )
 
             # Hack for Tlingit using dot as a letter when non word-final
@@ -202,15 +210,15 @@
 
         return self.tokenizers.get(tokenizer_key)
 
 
 _the_tokenizer_library = TokenizerLibrary()
 
 
-def make_tokenizer(in_lang=None, out_lang=None, tok_path=None):
+def make_tokenizer(in_lang=None, out_lang=None, tok_path=None) -> Tokenizer:
     """Make the tokenizer for input in language in_lang
 
     Logic used when only in_lang is provided:
     - if in_lang -> in_lang-ipa, or in_lang -> X-ipa exists, tokenize using the input
       inventory of that mapping.
     - elif in_lang -> X -> Y-ipa exists, e.g., tce -> tce-equiv -> tce-ipa, tokenize
       using the input inventory of those two hops.
```

### Comparing `g2p-1.0.20230417/g2p/mappings/utils.py` & `g2p-1.1.20230511/g2p/mappings/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,25 +425,24 @@
         # TODO: proper exception handling
         raise exceptions.MalformedMapping(
             "Formatting error in mapping in {}.".format(path)
         ) from e
 
 
 def escape_special_characters(to_escape: Dict[str, str]) -> Dict[str, str]:
-    for k, v in to_escape.items():
-        if isinstance(v, str):
-            escaped = re.escape(v)
-        else:
-            escaped = v
-        if escaped != v:
+    for key in ['in', 'context_before', 'context_after']:
+        if key not in to_escape or not isinstance(to_escape[key], str):
+            continue
+        escaped = re.escape(to_escape[key])
+        if to_escape[key] != escaped:
             LOGGER.debug(
-                f"Escaped special characters in '{v}' with '{escaped}''. Set 'escape_special' "
+                f"Escaped special characters in '{to_escape[key]}' with '{escaped}'. Set 'escape_special' "
                 "to False in your Mapping configuration to disable this."
             )
-        to_escape[k] = escaped
+        to_escape[key] = escaped
     return to_escape
 
 
 def load_abbreviations_from_file(path):
     """Helper method to load abbreviations from file."""
     if path.endswith("csv"):
         abbs = []
```

### Comparing `g2p-1.0.20230417/g2p/static/blockly_main.js` & `g2p-1.1.20230511/g2p/static/blockly_main.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/blocks.js` & `g2p-1.1.20230511/g2p/static/blocks.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/custom.css` & `g2p-1.1.20230511/g2p/static/custom.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/custom.js` & `g2p-1.1.20230511/g2p/static/custom.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/echart_custom.js` & `g2p-1.1.20230511/g2p/static/echart_custom.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/languages-network.json` & `g2p-1.1.20230511/g2p/static/languages-network.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/normalize.css` & `g2p-1.1.20230511/g2p/static/normalize.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/skeleton.css` & `g2p-1.1.20230511/g2p/static/skeleton.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/static/swagger.json` & `g2p-1.1.20230511/g2p/static/swagger.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999276620370371%*

 * *Differences: {"'paths'": "{'/g2p': {'get': {'parameters': {insert: [(5, OrderedDict([('name', 'tokenize'), "*

 * *            "('in', 'query'), ('description', 'tokenize before transducing'), ('required', False), "*

 * *            "('style', 'form'), ('explode', True), ('schema', OrderedDict([('type', "*

 * *            "'boolean')]))]))]}}}}"}*

```diff
@@ -284,14 +284,25 @@
                         "in": "query",
                         "name": "debugger",
                         "required": false,
                         "schema": {
                             "type": "boolean"
                         },
                         "style": "form"
+                    },
+                    {
+                        "description": "tokenize before transducing",
+                        "explode": true,
+                        "in": "query",
+                        "name": "tokenize",
+                        "required": false,
+                        "schema": {
+                            "type": "boolean"
+                        },
+                        "style": "form"
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
```

### Comparing `g2p-1.0.20230417/g2p/templates/docs.html` & `g2p-1.1.20230511/g2p/templates/docs.html`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/templates/index.html` & `g2p-1.1.20230511/g2p/templates/index.html`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/__init__.py` & `g2p-1.1.20230511/g2p/tests/public/data/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/crl.psv` & `g2p-1.1.20230511/g2p/tests/public/data/crl.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/fin.psv` & `g2p-1.1.20230511/g2p/tests/public/data/fin.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/fra.psv` & `g2p-1.1.20230511/g2p/tests/public/data/fra.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams.txt` & `g2p-1.1.20230511/g2p/tests/public/data/fra_panagrams.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/fra_panagrams_NFD.txt` & `g2p-1.1.20230511/g2p/tests/public/data/fra_panagrams_NFD.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/gwi.psv` & `g2p-1.1.20230511/g2p/tests/public/data/gwi.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/haa.csv` & `g2p-1.1.20230511/g2p/tests/public/data/haa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/ikt.psv` & `g2p-1.1.20230511/g2p/tests/public/data/ikt.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/iku-sro.psv` & `g2p-1.1.20230511/g2p/tests/public/data/iku-sro.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/kwk.psv` & `g2p-1.1.20230511/g2p/tests/public/data/kwk.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/mic.psv` & `g2p-1.1.20230511/g2p/tests/public/data/mic.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/moh.psv` & `g2p-1.1.20230511/g2p/tests/public/data/moh.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/oji-syl.psv` & `g2p-1.1.20230511/g2p/tests/public/data/oji-syl.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/oka.csv` & `g2p-1.1.20230511/g2p/tests/public/data/oka.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/tau.psv` & `g2p-1.1.20230511/g2p/tests/public/data/tau.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/data/tli.csv` & `g2p-1.1.20230511/g2p/tests/public/data/tli.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/git_to_ipa.json` & `g2p-1.1.20230511/g2p/tests/public/git_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/README.md` & `g2p-1.1.20230511/g2p/tests/public/mappings/case-feed/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/mappings/case-feed/config.yaml` & `g2p-1.1.20230511/g2p/tests/public/mappings/case-feed/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/mappings/gen-map_config.yaml` & `g2p-1.1.20230511/g2p/tests/public/mappings/gen-map_config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/mappings/minimal.xlsx` & `g2p-1.1.20230511/g2p/tests/public/mappings/minimal.xlsx`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/mappings/minimal_configs.yaml` & `g2p-1.1.20230511/g2p/tests/public/mappings/minimal_configs.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/public/sample_response.json` & `g2p-1.1.20230511/g2p/tests/public/sample_response.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/run.py` & `g2p-1.1.20230511/g2p/tests/run.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_api_resources.py` & `g2p-1.1.20230511/g2p/tests/test_api_resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -139,10 +139,42 @@
         self.assertEqual(same_response.status_code, 400)
         with self.assertLogs(LOGGER, level="ERROR"):
             missing_response = self.client().get(
                 self.conversion_route, query_string=missing_params
             )
         self.assertEqual(missing_response.status_code, 404)
 
+    def test_g2p_conversion_with_tok(self):
+        params_with_tok = {
+            "in-lang": "fra",
+            "out-lang": "eng-arpabet",
+            "text": "ceci, celà",
+            "debugger": True,
+            "index": True,
+            "tokenize": True,
+        }
+        response = self.client().get(
+            self.conversion_route, query_string=params_with_tok
+        )
+        self.assertEqual(response.status_code, 200)
+        res_json_tok = response.get_json()
+        self.assertEqual(res_json_tok["debugger"][0][0][0]["input"], "ceci")
+
+        params_no_tok = {
+            "in-lang": "fra",
+            "out-lang": "eng-arpabet",
+            "text": "ceci, celà",
+            "debugger": True,
+            "index": True,
+            "tokenize": False,
+        }
+        response = self.client().get(self.conversion_route, query_string=params_no_tok)
+        self.assertEqual(response.status_code, 200)
+        res_json_no_tok = response.get_json()
+        self.assertNotEqual(res_json_tok, res_json_no_tok)
+        self.assertEqual(res_json_no_tok["debugger"][0][0][0]["input"], "ceci, celà")
+
+        self.assertNotEqual(res_json_tok["debugger"], res_json_no_tok["debugger"])
+
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_check_ipa_arpabet.py` & `g2p-1.1.20230511/g2p/tests/test_check_ipa_arpabet.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         transducer = make_g2p("eng-ipa", "eng-arpabet")
         self.assertTrue(transducer.check(transducer("jŋeːi")))
         self.assertFalse(transducer.check(transducer("gaŋi")))
         self.assertTrue(transducer.check(transducer("ɡɑŋi")))
         self.assertFalse(transducer.check(transducer("ñ")))
 
     def test_check_ipa(self):
-        transducer = make_g2p("fra", "fra-ipa")
+        transducer = make_g2p("fra", "fra-ipa", tokenize=False)
         self.assertTrue(transducer.check(transducer("ceci")))
         self.assertFalse(transducer.check(transducer("ñ")))
         with self.assertLogs(LOGGER, level="WARNING"):
             self.assertFalse(transducer.check(transducer("ñ"), display_warnings=True))
         self.assertTrue(transducer.check(transducer("ceci est un test été à")))
 
         transducer = make_g2p("fra-ipa", "eng-ipa")
@@ -45,31 +45,31 @@
 
     def test_is_ipa_with_panphon_preprocessor(self):
         # panphon doesn't like these directly, but our panphon proprocessor "patches" them
         # because they are valid IPA phonetic constructs that panphon is a bit too picky about.
         self.assertTrue(utils.is_panphon("ɻ̊j̊ oⁿk oᵐp"))
 
     def test_check_composite_transducer(self):
-        transducer = make_g2p("fra", "eng-arpabet")
+        transducer = make_g2p("fra", "eng-arpabet", tokenize=False)
         self.assertTrue(transducer.check(transducer("ceci est un test été à")))
         self.assertFalse(transducer.check(transducer("ñ")))
 
     def test_check_tokenizing_transducer(self):
-        transducer = make_g2p("fra", "fra-ipa", tok_lang="fra")
+        transducer = make_g2p("fra", "fra-ipa")
         self.assertTrue(transducer.check(transducer("ceci est un test été à")))
         self.assertFalse(transducer.check(transducer("ñ oǹ")))
         self.assertTrue(
             transducer.check(transducer("ceci, cela; c'est tokenizé: alors c'est bon!"))
         )
         self.assertFalse(
             transducer.check(transducer("mais... c'est ñoñ, si du texte ne passe pas!"))
         )
 
     def test_check_tokenizing_composite_transducer(self):
-        transducer = make_g2p("fra", "eng-arpabet", tok_lang="fra")
+        transducer = make_g2p("fra", "eng-arpabet")
         self.assertTrue(transducer.check(transducer("ceci est un test été à")))
         self.assertFalse(transducer.check(transducer("ñ oǹ")))
         self.assertTrue(
             transducer.check(transducer("ceci, cela; c'est tokenizé: alors c'est bon!"))
         )
         self.assertFalse(
             transducer.check(transducer("mais... c'est ñoñ, si du texte ne passe pas!"))
@@ -79,33 +79,33 @@
                 transducer.check(
                     transducer("mais... c'est ñoñ, si du texte ne passe pas!"),
                     display_warnings=True,
                 )
             )
 
     def test_shallow_check(self):
-        transducer = make_g2p("win", "eng-arpabet", tok_lang="win")
+        transducer = make_g2p("win", "eng-arpabet")
         # This is False, but should be True! It's False because the mapping outputs :
         # instead of ː
         # EJJ 2022-06-16 With #100 fixed, this check is no longer failing.
         # self.assertFalse(transducer.check(transducer("uu")))
         self.assertTrue(transducer.check(transducer("uu")))
         self.assertTrue(transducer.check(transducer("uu"), shallow=True))
 
     def test_check_with_equiv(self):
-        transducer = make_g2p("tau", "eng-arpabet", tok_lang="tau")
-        tau_ipa = make_g2p("tau", "tau-ipa", tok_lang="tau")(
+        transducer = make_g2p("tau", "eng-arpabet")
+        tau_ipa = make_g2p("tau", "tau-ipa")(
             "sh'oo Jign maasee' do'eent'aa shyyyh"
         ).output_string
         self.assertTrue(utils.is_panphon(tau_ipa))
-        eng_ipa = make_g2p("tau", "eng-ipa", tok_lang="tau")(
+        eng_ipa = make_g2p("tau", "eng-ipa")(
             "sh'oo Jign maasee' do'eent'aa shyyyh"
         ).output_string
         self.assertTrue(utils.is_panphon(eng_ipa))
-        eng_arpabet = make_g2p("tau", "eng-arpabet", tok_lang="tau")(
+        eng_arpabet = make_g2p("tau", "eng-arpabet")(
             "sh'oo Jign maasee' do'eent'aa shyyyh"
         ).output_string
         self.assertTrue(utils.is_arpabet(eng_arpabet))
         # LOGGER.warning(
         #     f"tau-ipa {tau_ipa}\neng-ipa {eng_ipa}\n eng-arpabet {eng_arpabet}"
         # )
         self.assertTrue(
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_cli.py` & `g2p-1.1.20230511/g2p/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,21 @@
             self.assertIn(low, returned_set)
         mapped_upper = "ABCDEHIJKLMNOPQSTUVWXYZ"
         for u in mapped_upper:
             self.assertNotIn(u, returned_set)
         mapped_lower = "s"
         self.assertNotIn(mapped_lower, returned_set)
 
+    def test_scan_err(self):
+        results = self.runner.invoke(
+            scan, ["bad_lang", os.path.join(DATA_DIR, "fra_simple.txt")]
+        )
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn("is not a valid value for 'LANG'", results.output)
+
     def test_convert_option_a(self):
         result = self.runner.invoke(convert, "-a hello eng eng-arpabet")
         self.assertIn(
             "[('h', 'HH '), ('e', 'AH '), ('ll', 'L '), ('o', 'OW ')]", result.stdout
         )
 
     def test_convert_option_e(self):
@@ -262,14 +269,18 @@
         self.assertNotEqual(results.exit_code, 0)
         self.assertIn("Cannot find IPA mapping", results.output)
 
         results = self.runner.invoke(generate_mapping, "--list-dummy")
         self.assertEqual(results.exit_code, 0)  # this one not an error
         self.assertIn("Dummy phone inventory", results.output)
 
+        results = self.runner.invoke(generate_mapping, "--list-dummy fra")
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn("IN_LANG is not allowed with --list-dummy", results.output)
+
         results = self.runner.invoke(generate_mapping, "--ipa --dummy fra")
         self.assertNotEqual(results.exit_code, 0)
         self.assertIn("Error: Multiple modes selected", results.output)
 
         results = self.runner.invoke(
             generate_mapping, "--out-dir does-not-exist --ipa fra"
         )
@@ -300,14 +311,30 @@
         self.assertNotEqual(results.exit_code, 0)
         self.assertIn("is allowed in square brackets", results.output)
 
         results = self.runner.invoke(generate_mapping, "--from fra_to_eng --to eng")
         self.assertNotEqual(results.exit_code, 0)
         self.assertIn("Cannot find mapping", results.output)
 
+        results = self.runner.invoke(generate_mapping, "--merge --from fra --to eng")
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn(
+            "--merge is only compatible with --ipa and --dummy", results.output
+        )
+
+        results = self.runner.invoke(generate_mapping, "--merge --ipa fra")
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn("OUT_LANG is required with --merge", results.output)
+
+        results = self.runner.invoke(
+            generate_mapping, "--ipa --out-dir foo_bar_baz fra"
+        )
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn("Invalid value for '--out-dir': Directory", results.output)
+
     def test_show_mappings(self):
         # One arg = all mappings to or from that language
         results = self.runner.invoke(show_mappings, ["fra-ipa", "--verbose"])
         self.assertEqual(results.exit_code, 0)
         self.assertIn("French to IPA", results.output)
         self.assertIn("French IPA to English IPA", results.output)
         self.assertEqual(len(re.findall(r"display_name", results.output)), 2)
@@ -361,10 +388,40 @@
         results = self.runner.invoke(show_mappings, ["fra", "not-a-lang"])
         self.assertNotEqual(results.exit_code, 0)
 
         # No path
         results = self.runner.invoke(show_mappings, ["fra", "moe"])
         self.assertNotEqual(results.exit_code, 0)
 
+    def test_convert_from_file(self):
+        results = self.runner.invoke(
+            convert, [os.path.join(DATA_DIR, "fra_simple.txt"), "fra", "fra-ipa"]
+        )
+        self.assertEqual(results.exit_code, 0)
+        self.assertIn("fʁɑ̃sɛ", results.output)
+
+    def test_convert_errors(self):
+        """Exercise code handling error situations in g2p convert"""
+        results = self.runner.invoke(convert, "asdf bad_in_lang eng-ipa")
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn("not a valid value for 'IN_LANG'", results.output)
+
+        results = self.runner.invoke(convert, "asdf fra bad_out_lang")
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn("not a valid value for 'OUT_LANG'", results.output)
+
+        results = self.runner.invoke(convert, "asdf fra dan")
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn("Path between", results.output)
+        self.assertIn("does not exist", results.output)
+
+        results = self.runner.invoke(
+            convert, "--no-tok --tok-lang fra asdf fra fra-ipa"
+        )
+        self.assertNotEqual(results.exit_code, 0)
+        self.assertIn(
+            "Specified conflicting --no-tok and --tok-lang options", results.output
+        )
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_create_mapping.py` & `g2p-1.1.20230511/g2p/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_doctor.py` & `g2p-1.1.20230511/g2p/tests/test_doctor.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_doctor_expensive.py` & `g2p-1.1.20230511/g2p/tests/test_doctor_expensive.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_fallback.py` & `g2p-1.1.20230511/g2p/tests/test_fallback.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_indices.py` & `g2p-1.1.20230511/g2p/tests/test_indices.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_langs.py` & `g2p-1.1.20230511/g2p/tests/test_langs.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_lexicon_transducer.py` & `g2p-1.1.20230511/g2p/tests/test_lexicon_transducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,10 +199,15 @@
     def test_eng_transducer(self):
         """Test the cached eng to eng-ipa lexicon from make_g2p
         ."""
         transducer = make_g2p("eng", "eng-arpabet")
         tg = transducer("hello")
         self.assertEqual(tg.output_string, "HH AH L OW ")
 
+        # since we tokenize by default now, this works:
+        self.assertEqual(
+            transducer("hello my friend").output_string, "HH AH L OW  M AY  F R EH N D "
+        )
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_mappings.py` & `g2p-1.1.20230511/g2p/tests/test_mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,20 +162,27 @@
         self.assertEqual(transducer("a").output_string, "b")
         self.assertEqual(transducer_case_sensitive("a").output_string, "a")
         self.assertEqual(transducer("A").output_string, "b")
 
     def test_escape_special(self):
         mapping = Mapping([{"in": r"\d", "out": "digit"}])
         mapping_escaped = Mapping([{"in": r"\d", "out": "b"}], escape_special=True)
+        mapping_input_and_output_special_escaped = Mapping([{"in": "&", "out": "&"}], escape_special=True)
+        mapping_specific_from_fpcc = Mapping([{"in": r"^", "out": "A"}, {"in": "o", "out": r"."}], rule_ordering="apply-longest-first", escape_special=True)
         transducer = Transducer(mapping)
         transducer_escaped = Transducer(mapping_escaped)
+        transducer_escaped_input_output = Transducer(mapping_input_and_output_special_escaped)
+        transducer_fpcc = Transducer(mapping_specific_from_fpcc)
         self.assertEqual(transducer("1").output_string, "digit")
         self.assertEqual(transducer(r"\d").output_string, r"\d")
         self.assertEqual(transducer_escaped("1").output_string, "1")
         self.assertEqual(transducer_escaped(r"\d").output_string, "b")
+        self.assertEqual(transducer_escaped_input_output('&').output_string, "&")
+        self.assertEqual(transducer_fpcc("^o").output_string, "A.")
+        
 
     def test_norm_form(self):
         mapping_nfc = Mapping([{"in": "a\u0301", "out": "a"}])  # Defaults to NFC
         mapping_nfd = Mapping([{"in": "a\u0301", "out": "a"}], norm_form="NFD")
         mapping_none = Mapping([{"in": "a\u0301", "out": "a"}], norm_form=False)
 
         transducer_nfc = Transducer(mapping_nfc)
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_network.py` & `g2p-1.1.20230511/g2p/tests/test_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
                 make_g2p("git", "bar")
 
     def test_no_path(self):
         with self.assertRaises(NoPath), self.assertLogs(LOGGER, level="ERROR"):
             make_g2p("hei", "git")
 
     def test_valid_composite(self):
-        transducer = make_g2p("atj", "eng-ipa")
+        transducer = make_g2p("atj", "eng-ipa", tokenize=False)
         self.assertTrue(isinstance(transducer, CompositeTransducer))
         self.assertEqual("niɡiɡw", transducer("nikikw").output_string)
 
     def test_valid_transducer(self):
-        transducer = make_g2p("atj", "atj-ipa")
+        transducer = make_g2p("atj", "atj-ipa", tokenize=False)
         self.assertTrue(isinstance(transducer, Transducer))
         self.assertEqual("niɡiɡw", transducer("nikikw").output_string)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_studio.py` & `g2p-1.1.20230511/g2p/tests/test_studio.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 minimal dev mode:
     python run_studio.py
 or robust server mode (*nix only, gunicorn does not work on Windows):
     gunicorn --worker-class eventlet  -w 1 g2p.app:APP --no-sendfile --bind 0.0.0.0:5000 --daemon
 """
 
 from datetime import datetime
+from random import sample
 
 # flake8: noqa: C901
 from unittest import IsolatedAsyncioTestCase, main
 
 from playwright.async_api import async_playwright
 
 from g2p.app import APP, SOCKETIO
@@ -25,14 +26,15 @@
 
 
 class StudioTest(IsolatedAsyncioTestCase):
     def __init__(self, *args):
         super().__init__(*args)
         self.port = 5000
         self.debug = True
+        self.timeout_delay = 500
 
     def setUp(self):
         self.flask_test_client = APP.test_client()
         self.socketio_test_client = SOCKETIO.test_client(
             APP, flask_test_client=self.flask_test_client
         )
 
@@ -40,55 +42,69 @@
         self.assertTrue(self.socketio_test_client.is_connected())
 
     async def test_sanity(self):
         async with async_playwright() as p:
             browser = await p.chromium.launch(channel="chrome", headless=True)
             page = await browser.new_page()
             await page.goto(f"http://localhost:{self.port}/docs")
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
             await page.goto(f"http://localhost:{self.port}")
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
             input_el = page.locator("#input")
             output_el = page.locator("#output")
             await page.type("#input", "hello world")
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
             input_text = await input_el.input_value()
             output_text = await output_el.input_value()
             self.assertEqual(input_text, output_text)
             self.assertEqual(input_text, "hello world")
             await input_el.fill("")
             await output_el.fill("")
             await page.type("#input", "hello world")
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
             radio_el = page.locator("#animated-radio")
             await radio_el.click()
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
 
     async def test_switch_langs(self):
         async with async_playwright() as p:
             browser = await p.chromium.launch(channel="chrome", headless=True)
             page = await browser.new_page()
             await page.goto(f"http://localhost:{self.port}")
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
             in_lang_selector = page.locator("#input-langselect")
             # Switch to a language
             await in_lang_selector.select_option(value="alq")
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
             settings_title = await page.text_content("#link-0")
             self.assertEqual(settings_title, "Algonquin to IPA")
             # Switch back to custom
             await in_lang_selector.select_option(value="Custom")
-            await page.wait_for_timeout(1000)
+            await page.wait_for_timeout(self.timeout_delay)
             settings_title = await page.text_content("#link-0")
             self.assertEqual(settings_title, "Custom")
             # FIXME: Test that the table works somewhere, somehow
+            # Switch to in_lang = eng-arpabet, which means there is no possible outlang
+            await in_lang_selector.select_option(value="eng-arpabet")
+            await page.wait_for_timeout(self.timeout_delay)
+            self.assertEqual(await page.locator("#link-0").count(), 0)
 
     async def test_langs(self):
 
         langs_to_test = load_public_test_data()
+        # Doing the whole test set takes a long time, so let's use a 10% random sample,
+        # knowing that all cases always get exercised in test_cli.py and test_langs.py.
+        # 10% is enough to catch a sudden drift where the studio might stop being campatible.
+        langs_to_test = [
+            langs_to_test[i]
+            for i in sorted(
+                sample(range(len(langs_to_test)), k=len(langs_to_test) // 10)
+            )
+        ]
+
         error_count = 0
 
         # The current g2p-studio app leaks memory, so that if we try to run all the test
         # cases in one single browser instance, a case (not always the same) eventually
         # breaks. While that should get patched, for now, let's make unit testing
         # reliable by running tests by blocks we know the app can handle.
         block_size = 50
@@ -119,15 +135,15 @@
                     LOGGER.info(
                         f"{i+block*block_size} {datetime.now()} "
                         f"{test[0]}->{test[1]} {test[2]} -> {test[3]}"
                     )
                     for attempt in range(1, 4):
                         if attempt > 1:
                             LOGGER.info(f"Attempt #{attempt}")
-                            await page.wait_for_timeout(1000)
+                            await page.wait_for_timeout(self.timeout_delay)
                         # Clear input and output
                         await input_el.fill("")
                         await output_el.fill("")
                         output_text = ""
 
                         # Select the input language
                         await in_lang_selector.select_option(value=test[0])
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_tokenizer.py` & `g2p-1.1.20230511/g2p/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_transducer.py` & `g2p-1.1.20230511/g2p/tests/test_transducer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_unidecode_transducer.py` & `g2p-1.1.20230511/g2p/tests/test_unidecode_transducer.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,32 @@
         self.assertEqual(m.mapping, [])
         self.assertEqual(m.kwargs["type"], "unidecode")
         t = Transducer(m)
         tg = t("été Nunavut ᓄᓇᕗᑦ")
         self.assertEqual(tg.output_string, "ete Nunavut nonafot")
 
     def test_unidecode_g2p(self):
-        transducer = make_g2p("und", "und-ascii")
+        transducer = make_g2p("und", "und-ascii", tokenize=False)
         tg = transducer(normalize("éçà", "NFD"))
         self.assertEqual(tg.output_string, "eca")
         self.assertEqual(tg.edges, [(0, 0), (1, 0), (2, 1), (3, 1), (4, 2), (5, 2)])
 
         tg = transducer(normalize("éçà", "NFC"))
         self.assertEqual(tg.output_string, "eca")
         self.assertEqual(tg.edges, [(0, 0), (1, 1), (2, 2)])
 
     def test_unidecode_empty_output(self):
-        transducer = make_g2p("und", "und-ascii")
+        transducer = make_g2p("und", "und-ascii", tokenize=False)
         # \u0361 on its own gets deleted completely by unidecode
         tg = transducer("\u0361")
         self.assertEqual(tg.output_string, "")
         self.assertEqual(tg.edges, [])
 
     def test_unidecode_to_arpabet(self):
-        transducer = make_g2p("und", "eng-arpabet")
+        transducer = make_g2p("und", "eng-arpabet", tokenize=False)
         tg = transducer("été Nunavut ᓄᓇᕗᑦ")
         self.assertEqual(
             tg.output_string, "EY T EY  N UW N AA V UW T  N OW N AA F OW T "
         )
 
     def test_unidecode_arabic_to_arpabet(self):
         transducer = make_g2p("und", "eng-arpabet")
@@ -53,15 +53,15 @@
 
     def test_unidecode_kanji_to_arpabet(self):
         transducer = make_g2p("und", "eng-arpabet")
         tg = transducer("日本語")
         self.assertEqual(tg.output_string, "D IY B EY N Y UW ")
 
     def test_unidecode_hanzi_to_arpabet(self):
-        transducer = make_g2p("und", "eng-arpabet")
+        transducer = make_g2p("und", "eng-arpabet", tokenize=False)
         tg = transducer("你们好!你们说汉语马?")
         self.assertEqual(
             tg.output_string,
             "N IY M EY N HH AA OW N IY M EY N S HH UW OW Y IY Y UW M AA HH ",
         )
```

### Comparing `g2p-1.0.20230417/g2p/tests/test_utils.py` & `g2p-1.1.20230511/g2p/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/tests/test_z_local_config.py` & `g2p-1.1.20230511/g2p/tests/test_z_local_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -211,25 +211,43 @@
                 output = json.load(f)
             self.assertEqual(output, ref)
 
     def test_compose_NFC_NFD(self):
         config_path = self.mappings_dir / "compose.yaml"
         result = self.runner.invoke(
             convert,
-            [normalize("é", "NFD"), "c1", "c3", "--config", config_path, "-d", "-e"],
+            [
+                normalize("é", "NFD"),
+                "c1",
+                "c3",
+                "--no-tok",
+                "--config",
+                config_path,
+                "-d",
+                "-e",
+            ],
         )
         self.assertEqual(result.exit_code, 0)
         self.assertIn("[[(0, 0), (1, 0)], [(0, 0), (0, 1)]]", result.output)
         self.assertIn(
             "[[('e', 'ò'), ('́', 'ò')], [('ò', 'u'), ('ò', '̀')]]", result.output
         )
 
         result = self.runner.invoke(
             convert,
-            [normalize("é", "NFC"), "c1", "c3", "--config", config_path, "-d", "-e"],
+            [
+                normalize("é", "NFC"),
+                "c1",
+                "c3",
+                "--no-tok",
+                "--config",
+                config_path,
+                "-d",
+                "-e",
+            ],
         )
         self.assertEqual(result.exit_code, 0)
         self.assertIn("[[(0, 0)], [(0, 0), (0, 1)]]", result.output)
         self.assertIn("[[('é', 'ò')], [('ò', 'u'), ('ò', '̀')]]", result.output)
 
 
 if __name__ == "__main__":
```

### Comparing `g2p-1.0.20230417/g2p/tests/time_panphon.py` & `g2p-1.1.20230511/g2p/tests/time_panphon.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230417/g2p/transducer/__init__.py` & `g2p-1.1.20230511/g2p/transducer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Dict, List, Optional, Set, Tuple, Union
 
 import text_unidecode
 
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.langs.utils import is_arpabet, is_panphon
-from g2p.mappings.tokenizer import DefaultTokenizer
+from g2p.mappings.tokenizer import Tokenizer
 from g2p.mappings.utils import (
     compose_indices,
     is_ipa,
     normalize,
     normalize_with_indices,
     unicode_escape,
 )
@@ -1176,21 +1176,21 @@
     """This class combines tokenization and transduction.
 
     This is particularly useful for lexicon mappings, which cannot
     handle more than a single word at a time.
 
     Attributes:
         transducer (Transducer): A Transducer object for the mapping part
-        tokenizer (DefaultTokenizer): A Tokenizer object to split the string before mapping
+        tokenizer (Tokenizer): A Tokenizer object to split the string before mapping
     """
 
     def __init__(
         self,
         transducer: Union[Transducer, CompositeTransducer],
-        tokenizer: DefaultTokenizer,
+        tokenizer: Tokenizer,
     ):
         self._transducer = transducer
         self._tokenizer = tokenizer
 
     def __call__(self, to_convert: str):
         # perform normalization before tokenizing, since it can change tokenization
         if self._transducer.norm_form:
```

### Comparing `g2p-1.0.20230417/g2p.egg-info/PKG-INFO` & `g2p-1.1.20230511/g2p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p
-Version: 1.0.20230417
+Version: 1.1.20230511
 Summary: Module for creating context-aware, rule-based G2P mappings that preserve indices
 Home-page: https://github.com/roedoejet/g2p
 Author: Aidan Pine
 Author-email: hello@aidanpine.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `g2p-1.0.20230417/g2p.egg-info/SOURCES.txt` & `g2p-1.1.20230511/g2p.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 g2p/__init__.py
 g2p/_version.py
 g2p/api.py
 g2p/app.py
 g2p/cli.py
+g2p/deprecation.py
 g2p/exceptions.py
 g2p/log.py
 g2p.egg-info/PKG-INFO
 g2p.egg-info/SOURCES.txt
 g2p.egg-info/dependency_links.txt
 g2p.egg-info/entry_points.txt
 g2p.egg-info/not-zip-safe
```

### Comparing `g2p-1.0.20230417/setup.py` & `g2p-1.1.20230511/setup.py`

 * *Files identical despite different names*

