# Comparing `tmp/starkinfra-0.7.0.tar.gz` & `tmp/starkinfra-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starkinfra-0.7.0.tar", last modified: Thu Apr 27 20:26:45 2023, max compression
+gzip compressed data, was "starkinfra-0.8.0.tar", last modified: Thu May 11 17:41:38 2023, max compression
```

## Comparing `starkinfra-0.7.0.tar` & `starkinfra-0.8.0.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.038408 starkinfra-0.7.0/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-01 13:39:31.000000 starkinfra-0.7.0/LICENSE.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-01 13:39:31.000000 starkinfra-0.7.0/MANIFEST.in
--rw-r--r--   0 caiodottori   (501) staff       (20)    71265 2023-04-27 20:26:45.038200 starkinfra-0.7.0/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)    70847 2023-04-27 20:24:01.000000 starkinfra-0.7.0/README.md
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2023-04-27 20:26:45.038472 starkinfra-0.7.0/setup.cfg
--rw-r--r--   0 caiodottori   (501) staff       (20)      828 2023-04-27 20:25:01.000000 starkinfra-0.7.0/setup.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.843866 starkinfra-0.7.0/starkinfra/
--rw-r--r--   0 caiodottori   (501) staff       (20)     3392 2023-04-27 20:25:35.000000 starkinfra-0.7.0/starkinfra/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.849030 starkinfra-0.7.0/starkinfra/brcodepreview/
--rw-r--r--   0 caiodottori   (501) staff       (20)     5010 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/brcodepreview/__brcodepreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/brcodepreview/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.851991 starkinfra-0.7.0/starkinfra/cardmethod/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1297 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/cardmethod/__cardmethod.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       32 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/cardmethod/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.854830 starkinfra-0.7.0/starkinfra/creditholmes/
--rw-r--r--   0 caiodottori   (501) staff       (20)     6542 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditholmes/__creditholmes.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       98 2022-12-21 18:15:18.000000 starkinfra-0.7.0/starkinfra/creditholmes/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.859603 starkinfra-0.7.0/starkinfra/creditholmes/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-12-21 18:15:18.000000 starkinfra-0.7.0/starkinfra/creditholmes/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5157 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditholmes/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.864526 starkinfra-0.7.0/starkinfra/creditnote/
--rw-r--r--   0 caiodottori   (501) staff       (20)    12152 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditnote/__creditnote.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      325 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/creditnote/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     3535 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/__transfer.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.867993 starkinfra-0.7.0/starkinfra/creditnote/invoice/
--rw-r--r--   0 caiodottori   (501) staff       (20)      534 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__description.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      507 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__discount.py
--rw-r--r--   0 caiodottori   (501) staff       (20)        0 2022-06-03 20:41:22.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5403 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditnote/invoice/__invoice.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.871217 starkinfra-0.7.0/starkinfra/creditnote/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/creditnote/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5163 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditnote/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.875616 starkinfra-0.7.0/starkinfra/creditpreview/
--rw-r--r--   0 caiodottori   (501) staff       (20)     3364 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/creditpreview/__creditnotepreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1995 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/creditpreview/__creditpreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/creditpreview/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.878677 starkinfra-0.7.0/starkinfra/creditsigner/
--rw-r--r--   0 caiodottori   (501) staff       (20)      756 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/creditsigner/__creditsigner.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       55 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/creditsigner/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.882003 starkinfra-0.7.0/starkinfra/dynamicbrcode/
--rw-r--r--   0 caiodottori   (501) staff       (20)    15774 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/dynamicbrcode/__dynamicbrcode.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       94 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/dynamicbrcode/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.884835 starkinfra-0.7.0/starkinfra/event/
--rw-r--r--   0 caiodottori   (501) staff       (20)     8846 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/event/__event.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      122 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/event/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.887791 starkinfra-0.7.0/starkinfra/event/attempt/
--rw-r--r--   0 caiodottori   (501) staff       (20)     4981 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/event/attempt/__attempt.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       40 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/event/attempt/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.890840 starkinfra-0.7.0/starkinfra/individualdocument/
--rw-r--r--   0 caiodottori   (501) staff       (20)     7065 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualdocument/__individualdocument.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualdocument/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.892232 starkinfra-0.7.0/starkinfra/individualdocument/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualdocument/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5257 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualdocument/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.895715 starkinfra-0.7.0/starkinfra/individualidentity/
--rw-r--r--   0 caiodottori   (501) staff       (20)     7874 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualidentity/__individualidentity.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualidentity/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.896889 starkinfra-0.7.0/starkinfra/individualidentity/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.7.0/starkinfra/individualidentity/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5249 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/individualidentity/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.902204 starkinfra-0.7.0/starkinfra/issuingbalance/
--rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingbalance/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1603 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/issuingbalance/__issuingbalance.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.904526 starkinfra-0.7.0/starkinfra/issuingcard/
--rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/issuingcard/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    11393 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingcard/__issuingcard.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.907710 starkinfra-0.7.0/starkinfra/issuingcard/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingcard/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5260 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingcard/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.910615 starkinfra-0.7.0/starkinfra/issuingdesign/
--rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingdesign/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4754 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingdesign/__issuingdesign.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.911343 starkinfra-0.7.0/starkinfra/issuingembossingkit/
--rw-r--r--   0 caiodottori   (501) staff       (20)       52 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingkit/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5269 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingkit/__issuingembossingkit.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.914503 starkinfra-0.7.0/starkinfra/issuingembossingrequest/
--rw-r--r--   0 caiodottori   (501) staff       (20)      109 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     8738 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.917301 starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6001 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.920475 starkinfra-0.7.0/starkinfra/issuingholder/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/issuingholder/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     8239 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingholder/__issuingholder.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.923956 starkinfra-0.7.0/starkinfra/issuingholder/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingholder/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5225 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingholder/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.927588 starkinfra-0.7.0/starkinfra/issuinginvoice/
--rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6663 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/__issuinginvoice.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.930260 starkinfra-0.7.0/starkinfra/issuinginvoice/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4939 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuinginvoice/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.935080 starkinfra-0.7.0/starkinfra/issuingproduct/
--rw-r--r--   0 caiodottori   (501) staff       (20)       42 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/issuingproduct/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2825 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/issuingproduct/__issuingproduct.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.936380 starkinfra-0.7.0/starkinfra/issuingpurchase/
--rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    13027 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/__issuingpurchase.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.939320 starkinfra-0.7.0/starkinfra/issuingpurchase/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5986 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingpurchase/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.943562 starkinfra-0.7.0/starkinfra/issuingrestock/
--rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingrestock/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6412 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingrestock/__issuingrestock.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.945689 starkinfra-0.7.0/starkinfra/issuingrestock/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingrestock/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5242 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingrestock/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.948749 starkinfra-0.7.0/starkinfra/issuingrule/
--rw-r--r--   0 caiodottori   (501) staff       (20)       78 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/issuingrule/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     3925 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingrule/__issuingrule.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.951424 starkinfra-0.7.0/starkinfra/issuingstock/
--rw-r--r--   0 caiodottori   (501) staff       (20)       90 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingstock/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5619 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingstock/__issuingstock.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.954105 starkinfra-0.7.0/starkinfra/issuingstock/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.7.0/starkinfra/issuingstock/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5270 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingstock/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.957213 starkinfra-0.7.0/starkinfra/issuingtransaction/
--rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingtransaction/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5402 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingtransaction/__issuingtransaction.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.960296 starkinfra-0.7.0/starkinfra/issuingwithdrawal/
--rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/issuingwithdrawal/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6033 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.966311 starkinfra-0.7.0/starkinfra/merchantcategory/
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/merchantcategory/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1757 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/merchantcategory/__merchantcategory.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.969455 starkinfra-0.7.0/starkinfra/merchantcountry/
--rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/merchantcountry/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1403 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/merchantcountry/__merchantcountry.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.970503 starkinfra-0.7.0/starkinfra/pixbalance/
--rw-r--r--   0 caiodottori   (501) staff       (20)       30 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixbalance/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1635 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixbalance/__pixbalance.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.974118 starkinfra-0.7.0/starkinfra/pixchargeback/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixchargeback/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10153 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixchargeback/__pixchargeback.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.977151 starkinfra-0.7.0/starkinfra/pixchargeback/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixchargeback/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5370 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixchargeback/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.980720 starkinfra-0.7.0/starkinfra/pixclaim/
--rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/pixclaim/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10003 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixclaim/__pixclaim.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.983140 starkinfra-0.7.0/starkinfra/pixclaim/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/pixclaim/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5518 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixclaim/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.987767 starkinfra-0.7.0/starkinfra/pixdirector/
--rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixdirector/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2165 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixdirector/__pixdirector.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.992582 starkinfra-0.7.0/starkinfra/pixdomain/
--rw-r--r--   0 caiodottori   (501) staff       (20)      457 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixdomain/__certificate.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       70 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixdomain/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1382 2022-08-26 19:22:07.000000 starkinfra-0.7.0/starkinfra/pixdomain/__pixdomain.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.993730 starkinfra-0.7.0/starkinfra/pixinfraction/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixinfraction/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     9589 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixinfraction/__pixinfraction.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.996248 starkinfra-0.7.0/starkinfra/pixinfraction/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixinfraction/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5368 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixinfraction/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.999068 starkinfra-0.7.0/starkinfra/pixkey/
--rw-r--r--   0 caiodottori   (501) staff       (20)      108 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/pixkey/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10238 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixkey/__pixkey.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.002188 starkinfra-0.7.0/starkinfra/pixkey/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/pixkey/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5107 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixkey/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.005134 starkinfra-0.7.0/starkinfra/pixrequest/
--rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/pixrequest/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    13971 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixrequest/__pixrequest.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.008265 starkinfra-0.7.0/starkinfra/pixrequest/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixrequest/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5534 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixrequest/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.012456 starkinfra-0.7.0/starkinfra/pixreversal/
--rw-r--r--   0 caiodottori   (501) staff       (20)      114 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/pixreversal/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10438 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixreversal/__pixreversal.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.015397 starkinfra-0.7.0/starkinfra/pixreversal/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixreversal/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5138 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixreversal/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.018096 starkinfra-0.7.0/starkinfra/pixstatement/
--rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/pixstatement/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5856 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/pixstatement/__pixstatement.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.021134 starkinfra-0.7.0/starkinfra/staticbrcode/
--rw-r--r--   0 caiodottori   (501) staff       (20)       53 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/staticbrcode/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6859 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/staticbrcode/__staticbrcode.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.035839 starkinfra-0.7.0/starkinfra/utils/
--rw-r--r--   0 caiodottori   (501) staff       (20)       88 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      451 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/bacenid.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      360 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/endtoendid.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      151 2022-07-08 00:58:09.000000 starkinfra-0.7.0/starkinfra/utils/parse.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      579 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/utils/relay.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      510 2022-05-01 13:39:31.000000 starkinfra-0.7.0/starkinfra/utils/rest.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      354 2022-05-01 20:57:34.000000 starkinfra-0.7.0/starkinfra/utils/returnid.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:45.037825 starkinfra-0.7.0/starkinfra/webhook/
--rw-r--r--   0 caiodottori   (501) staff       (20)       56 2022-05-24 01:07:12.000000 starkinfra-0.7.0/starkinfra/webhook/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4765 2023-04-27 20:24:01.000000 starkinfra-0.7.0/starkinfra/webhook/__webhook.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-04-27 20:26:44.845649 starkinfra-0.7.0/starkinfra.egg-info/
--rw-r--r--   0 caiodottori   (501) staff       (20)    71265 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)     5195 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)        1 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-04-27 20:26:44.000000 starkinfra-0.7.0/starkinfra.egg-info/top_level.txt
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.736128 starkinfra-0.8.0/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-01 13:39:31.000000 starkinfra-0.8.0/LICENSE.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-01 13:39:31.000000 starkinfra-0.8.0/MANIFEST.in
+-rw-r--r--   0 caiodottori   (501) staff       (20)    71335 2023-05-11 17:41:38.735823 starkinfra-0.8.0/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)    70917 2023-05-11 17:39:45.000000 starkinfra-0.8.0/README.md
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2023-05-11 17:41:38.736191 starkinfra-0.8.0/setup.cfg
+-rw-r--r--   0 caiodottori   (501) staff       (20)      828 2023-04-27 20:25:01.000000 starkinfra-0.8.0/setup.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.561650 starkinfra-0.8.0/starkinfra/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3392 2023-05-11 17:40:28.000000 starkinfra-0.8.0/starkinfra/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.566926 starkinfra-0.8.0/starkinfra/brcodepreview/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5446 2023-05-11 17:39:45.000000 starkinfra-0.8.0/starkinfra/brcodepreview/__brcodepreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/brcodepreview/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.569365 starkinfra-0.8.0/starkinfra/cardmethod/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1297 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/cardmethod/__cardmethod.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       32 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/cardmethod/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.572285 starkinfra-0.8.0/starkinfra/creditholmes/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6542 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditholmes/__creditholmes.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       98 2022-12-21 18:15:18.000000 starkinfra-0.8.0/starkinfra/creditholmes/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.575012 starkinfra-0.8.0/starkinfra/creditholmes/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-12-21 18:15:18.000000 starkinfra-0.8.0/starkinfra/creditholmes/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5157 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditholmes/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.580477 starkinfra-0.8.0/starkinfra/creditnote/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    12304 2023-05-11 17:39:45.000000 starkinfra-0.8.0/starkinfra/creditnote/__creditnote.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      325 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/creditnote/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3535 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/__transfer.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.586553 starkinfra-0.8.0/starkinfra/creditnote/invoice/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      534 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__description.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      507 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__discount.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)        0 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5403 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__invoice.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.589079 starkinfra-0.8.0/starkinfra/creditnote/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/creditnote/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5163 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditnote/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.593145 starkinfra-0.8.0/starkinfra/creditpreview/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3364 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditpreview/__creditnotepreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1995 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/creditpreview/__creditpreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/creditpreview/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.595710 starkinfra-0.8.0/starkinfra/creditsigner/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      756 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/creditsigner/__creditsigner.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       55 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/creditsigner/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.599671 starkinfra-0.8.0/starkinfra/dynamicbrcode/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    15774 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/dynamicbrcode/__dynamicbrcode.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       94 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/dynamicbrcode/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.602628 starkinfra-0.8.0/starkinfra/event/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8846 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/event/__event.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      122 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/event/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.605533 starkinfra-0.8.0/starkinfra/event/attempt/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4981 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/event/attempt/__attempt.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       40 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/event/attempt/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.609033 starkinfra-0.8.0/starkinfra/individualdocument/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7065 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualdocument/__individualdocument.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualdocument/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.612021 starkinfra-0.8.0/starkinfra/individualdocument/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualdocument/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5257 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualdocument/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.614783 starkinfra-0.8.0/starkinfra/individualidentity/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7874 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualidentity/__individualidentity.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualidentity/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.617362 starkinfra-0.8.0/starkinfra/individualidentity/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualidentity/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5249 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualidentity/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.619987 starkinfra-0.8.0/starkinfra/issuingbalance/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingbalance/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1603 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/issuingbalance/__issuingbalance.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.623561 starkinfra-0.8.0/starkinfra/issuingcard/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/issuingcard/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    11393 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingcard/__issuingcard.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.626208 starkinfra-0.8.0/starkinfra/issuingcard/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingcard/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5260 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingcard/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.628989 starkinfra-0.8.0/starkinfra/issuingdesign/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingdesign/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4754 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingdesign/__issuingdesign.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.631352 starkinfra-0.8.0/starkinfra/issuingembossingkit/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       52 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingkit/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5269 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingkit/__issuingembossingkit.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.634248 starkinfra-0.8.0/starkinfra/issuingembossingrequest/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      109 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8738 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.636706 starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6001 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.639099 starkinfra-0.8.0/starkinfra/issuingholder/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/issuingholder/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8239 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingholder/__issuingholder.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.641607 starkinfra-0.8.0/starkinfra/issuingholder/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingholder/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5225 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingholder/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.646557 starkinfra-0.8.0/starkinfra/issuinginvoice/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6663 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/__issuinginvoice.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.649211 starkinfra-0.8.0/starkinfra/issuinginvoice/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4939 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.651631 starkinfra-0.8.0/starkinfra/issuingproduct/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       42 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/issuingproduct/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2825 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/issuingproduct/__issuingproduct.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.654489 starkinfra-0.8.0/starkinfra/issuingpurchase/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    13027 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/__issuingpurchase.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.656742 starkinfra-0.8.0/starkinfra/issuingpurchase/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5986 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.658870 starkinfra-0.8.0/starkinfra/issuingrestock/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingrestock/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6412 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingrestock/__issuingrestock.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.660875 starkinfra-0.8.0/starkinfra/issuingrestock/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingrestock/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5242 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingrestock/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.663334 starkinfra-0.8.0/starkinfra/issuingrule/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       78 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/issuingrule/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3925 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingrule/__issuingrule.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.665518 starkinfra-0.8.0/starkinfra/issuingstock/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       90 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingstock/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5619 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingstock/__issuingstock.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.668239 starkinfra-0.8.0/starkinfra/issuingstock/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingstock/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5270 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingstock/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.670992 starkinfra-0.8.0/starkinfra/issuingtransaction/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingtransaction/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5402 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingtransaction/__issuingtransaction.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.675453 starkinfra-0.8.0/starkinfra/issuingwithdrawal/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingwithdrawal/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6033 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.678139 starkinfra-0.8.0/starkinfra/merchantcategory/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/merchantcategory/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1757 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/merchantcategory/__merchantcategory.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.680294 starkinfra-0.8.0/starkinfra/merchantcountry/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/merchantcountry/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1403 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/merchantcountry/__merchantcountry.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.682236 starkinfra-0.8.0/starkinfra/pixbalance/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       30 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixbalance/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1635 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixbalance/__pixbalance.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.684771 starkinfra-0.8.0/starkinfra/pixchargeback/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixchargeback/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10153 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixchargeback/__pixchargeback.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.686969 starkinfra-0.8.0/starkinfra/pixchargeback/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixchargeback/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5370 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixchargeback/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.690072 starkinfra-0.8.0/starkinfra/pixclaim/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/pixclaim/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10003 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixclaim/__pixclaim.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.692452 starkinfra-0.8.0/starkinfra/pixclaim/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/pixclaim/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5518 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixclaim/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.695340 starkinfra-0.8.0/starkinfra/pixdirector/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixdirector/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2165 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixdirector/__pixdirector.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.698640 starkinfra-0.8.0/starkinfra/pixdomain/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      457 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixdomain/__certificate.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       70 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixdomain/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1382 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/pixdomain/__pixdomain.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.701091 starkinfra-0.8.0/starkinfra/pixinfraction/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixinfraction/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     9589 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixinfraction/__pixinfraction.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.703182 starkinfra-0.8.0/starkinfra/pixinfraction/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixinfraction/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5368 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixinfraction/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.705492 starkinfra-0.8.0/starkinfra/pixkey/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      108 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixkey/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10238 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixkey/__pixkey.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.707380 starkinfra-0.8.0/starkinfra/pixkey/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/pixkey/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5107 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixkey/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.709868 starkinfra-0.8.0/starkinfra/pixrequest/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/pixrequest/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    13971 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixrequest/__pixrequest.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.711969 starkinfra-0.8.0/starkinfra/pixrequest/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixrequest/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5534 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixrequest/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.714771 starkinfra-0.8.0/starkinfra/pixreversal/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      114 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/pixreversal/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10438 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixreversal/__pixreversal.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.717594 starkinfra-0.8.0/starkinfra/pixreversal/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixreversal/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5138 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixreversal/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.720527 starkinfra-0.8.0/starkinfra/pixstatement/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixstatement/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5856 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixstatement/__pixstatement.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.721539 starkinfra-0.8.0/starkinfra/staticbrcode/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       53 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/staticbrcode/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7081 2023-05-11 17:39:45.000000 starkinfra-0.8.0/starkinfra/staticbrcode/__staticbrcode.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.733214 starkinfra-0.8.0/starkinfra/utils/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       88 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      451 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/bacenid.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      360 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/endtoendid.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      151 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/utils/parse.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      579 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/utils/relay.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      510 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/utils/rest.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      354 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/returnid.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.735498 starkinfra-0.8.0/starkinfra/webhook/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       56 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/webhook/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4765 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/webhook/__webhook.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.562970 starkinfra-0.8.0/starkinfra.egg-info/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    71335 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5195 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)        1 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/top_level.txt
```

### Comparing `starkinfra-0.7.0/LICENSE.txt` & `starkinfra-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/PKG-INFO` & `starkinfra-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkinfra
-Version: 0.7.0
+Version: 0.8.0
 Summary: SDK to facilitate Python integrations with Stark Infra
 Home-page: https://github.com/starkinfra/sdk-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Keywords: stark infra,starkinfra,sdk,open banking,openbanking,banking,open,stark
 Platform: UNKNOWN
@@ -2188,18 +2188,20 @@
 You can create BrcodePreviews to preview BR Codes before paying them.
 
 ```python
 import starkinfra
 
 previews = starkinfra.brcodepreview.create([
     starkinfra.BrcodePreview(
-        id="00020126420014br.gov.bcb.pix0120nedstark@hotmail.com52040000530398654075000.005802BR5909Ned Stark6014Rio de Janeiro621605126674869738606304FF71"
+        id="00020126420014br.gov.bcb.pix0120nedstark@hotmail.com52040000530398654075000.005802BR5909Ned Stark6014Rio de Janeiro621605126674869738606304FF71",
+        payer_id="012.345.678-90"
     ),
     starkinfra.BrcodePreview(
-        id="00020126430014br.gov.bcb.pix0121aryastark@hotmail.com5204000053039865406100.005802BR5910Arya Stark6014Rio de Janeiro6216051262678188104863042BA4"
+        id="00020126430014br.gov.bcb.pix0121aryastark@hotmail.com5204000053039865406100.005802BR5910Arya Stark6014Rio de Janeiro6216051262678188104863042BA4",
+        payer_id="012.345.678-90"
     ),
 ])
 
 for preview in previews:
     print(preview)
 ```
```

### Comparing `starkinfra-0.7.0/README.md` & `starkinfra-0.8.0/starkinfra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: starkinfra
+Version: 0.8.0
+Summary: SDK to facilitate Python integrations with Stark Infra
+Home-page: https://github.com/starkinfra/sdk-python
+Author: Stark Infra
+Author-email: developers@starkbank.com
+License: MIT License
+Keywords: stark infra,starkinfra,sdk,open banking,openbanking,banking,open,stark
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Stark Infra Python SDK - Beta
 
 Welcome to the Stark Infra Python SDK! This tool is made for Python 
 developers who want to easily integrate with our API.
 This SDK version is compatible with the Stark Infra API v2.
 
 # Introduction
@@ -2175,18 +2188,20 @@
 You can create BrcodePreviews to preview BR Codes before paying them.
 
 ```python
 import starkinfra
 
 previews = starkinfra.brcodepreview.create([
     starkinfra.BrcodePreview(
-        id="00020126420014br.gov.bcb.pix0120nedstark@hotmail.com52040000530398654075000.005802BR5909Ned Stark6014Rio de Janeiro621605126674869738606304FF71"
+        id="00020126420014br.gov.bcb.pix0120nedstark@hotmail.com52040000530398654075000.005802BR5909Ned Stark6014Rio de Janeiro621605126674869738606304FF71",
+        payer_id="012.345.678-90"
     ),
     starkinfra.BrcodePreview(
-        id="00020126430014br.gov.bcb.pix0121aryastark@hotmail.com5204000053039865406100.005802BR5910Arya Stark6014Rio de Janeiro6216051262678188104863042BA4"
+        id="00020126430014br.gov.bcb.pix0121aryastark@hotmail.com5204000053039865406100.005802BR5910Arya Stark6014Rio de Janeiro6216051262678188104863042BA4",
+        payer_id="012.345.678-90"
     ),
 ])
 
 for preview in previews:
     print(preview)
 ```
 
@@ -2948,7 +2963,9 @@
 # Help and Feedback
 
 If you have any questions about our SDK, just send us an email.
 We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
 We also love feedback, so don't be shy about sharing your thoughts with us.
 
 Email: help@starkbank.com
+
+
```

### Comparing `starkinfra-0.7.0/setup.py` & `starkinfra-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/__init__.py` & `starkinfra-0.8.0/starkinfra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = "0.7.0"
+version = "0.8.0"
 language = "en-US"
 timeout = 15
 user = None
 
 from starkcore import Project, Organization, key, error
 
 from . import event
```

### Comparing `starkinfra-0.7.0/starkinfra/brcodepreview/__brcodepreview.py` & `starkinfra-0.8.0/starkinfra/brcodepreview/__brcodepreview.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     """# BrcodePreview object
     The BrcodePreview object is used to preview information from a BR Code before paying it.
     When you initialize a BrcodePreview, the entity will not be automatically
     created in the Stark Infra API. The 'create' function sends the objects
     to the Stark Infra API and returns the created object.
     ## Parameters (required):
     - id [string]: BR Code from a Pix payment. This is also de information directly encoded in a QR Code. ex: "00020126580014br.gov.bcb.pix0136a629532e-7693-4846-852d-1bbff817b5a8520400005303986540510.005802BR5908T'Challa6009Sao Paulo62090505123456304B14A"
+    - payer_id [string]: tax id (CPF/CNPJ) of the individual or business requesting the PixKey information. This id is used by the Central Bank to limit request rates. ex: "20.018.183/0001-80"
+    ## Parameters (optional):
+    - end_to_end_id [string]: central bank's unique transaction ID. ex: "E79457883202101262140HHX553UPqeq"
     ## Attributes (return-only):
     - account_number [string]: Payment receiver account number. ex: "1234567"
     - account_type [string]: Payment receiver account type. ex: "checking"
     - amount [integer]: Value in cents that this payment is expecting to receive. If 0, any value is accepted. ex: 123 (= R$1,23)
     - amount_type [string]: amount type of the Brcode. If the amount type is "custom" the Brcode's amount can be changed by the sender at the moment of payment. Options: "fixed" or "custom"
     - bank_code [string]: Payment receiver bank code. ex: "20018183"
     - branch_code [string]: Payment receiver branch code. ex: "0001"
@@ -30,20 +33,22 @@
     - reconciliation_id [string]: Reconciliation ID linked to this payment. If the brcode is dynamic, the reconciliation_id will have from 26 to 35 alphanumeric characters, ex: "cd65c78aeb6543eaaa0170f68bd741ee". If the brcode is static, the reconciliation_id will have up to 25 alphanumeric characters "ah27s53agj6493hjds6836v49"
     - reduction_amount [integer]: Reduction value to discount from nominal_amount. ex: 1000
     - scheduled [datetime.datetime]: date of payment execution. ex: datetime(2020, 3, 10)
     - status [string]: Payment status. ex: "active", "paid", "canceled" or "unknown"
     - tax_id [string]: Payment receiver tax ID. ex: "012.345.678-90"
     """
 
-    def __init__(self, id, account_number=None, account_type=None, amount=None, amount_type=None, bank_code=None,
+    def __init__(self, id, payer_id, account_number=None, account_type=None, amount=None, amount_type=None, bank_code=None,
                  branch_code=None, cash_amount=None, cashier_bank_code=None, cashier_type=None, discount_amount=None,
-                 fine_amount=None, interest_amount=None, key_id=None, name=None, nominal_amount=None,
+                 fine_amount=None, interest_amount=None, key_id=None, name=None, nominal_amount=None, end_to_end_id=None,
                  reconciliation_id=None, reduction_amount=None, scheduled=None, status=None, tax_id=None):
         Resource.__init__(self, id=id)
         
+        self.payer_id = payer_id
+        self.end_to_end_id = end_to_end_id
         self.account_number = account_number
         self.account_type = account_type
         self.amount = amount
         self.amount_type = amount_type
         self.bank_code = bank_code
         self.branch_code = branch_code
         self.cash_amount = cash_amount
```

### Comparing `starkinfra-0.7.0/starkinfra/cardmethod/__cardmethod.py` & `starkinfra-0.8.0/starkinfra/cardmethod/__cardmethod.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditholmes/__creditholmes.py` & `starkinfra-0.8.0/starkinfra/creditholmes/__creditholmes.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditholmes/log/__log.py` & `starkinfra-0.8.0/starkinfra/creditholmes/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditnote/__creditnote.py` & `starkinfra-0.8.0/starkinfra/creditnote/__creditnote.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,70 +16,71 @@
     When you initialize a CreditNote, the entity will not be automatically
     created in the Stark Infra API. The 'create' function sends the objects
     to the Stark Infra API and returns the list of created objects.
     ## Parameters (required):
     - template_id [string]: ID of the contract template on which the CreditNote will be based. ex: "0123456789101112"
     - name [string]: credit receiver's full name. ex: "Edward Stark"
     - tax_id [string]: credit receiver's tax ID (CPF or CNPJ). ex: "20.018.183/0001-80"
-    - nominal_amount [integer]: amount in cents transferred to the credit receiver, before deductions. ex: 11234 (= R$ 112.34)
     - scheduled [datetime.date, datetime.datetime or string]: date of transfer execution. ex: datetime(2020, 3, 10)
     - invoices [list of Invoice objects]: list of Invoice objects to be created and sent to the credit receiver. ex: [Invoice(), Invoice()]
     - payment [creditnote.Transfer]: payment entity to be created and sent to the credit receiver. ex: creditnote.Transfer()
     - signers [list of CreditSigner objects]: signer's name, contact and delivery method for the signature request. ex: [CreditSigner(), CreditSigner()]
     - external_id [string]: a string that must be unique among all your CreditNotes, used to avoid resource duplication. ex: "my-internal-id-123456"
     - street_line_1 [string]: credit receiver main address. ex: "Av. Paulista, 200"
     - street_line_2 [string]: credit receiver address complement. ex: "Apto. 123"
     - district [string]: credit receiver address district / neighbourhood. ex: "Bela Vista"
     - city [string]: credit receiver address city. ex: "Rio de Janeiro"
     - state_code [string]: credit receiver address state. ex: "GO"
     - zip_code [string]: credit receiver address zip code. ex: "01311-200"
     ## Parameters (conditionally required):
     - payment_type [string]: payment type, inferred from the payment parameter if it is not a dictionary. ex: "transfer"
+    - nominal_amount [integer]: CreditNote value in cents. The nominal_amount parameter is required when amount is not sent. ex: 1234 (= R$ 12.34)
+    - amount [integer]: amount in cents transferred to the credit receiver, before deductions. The amount parameter is required when nominal_amount is not sent. ex: 1234 (= R$ 12.34)
     ## Parameters (optional):
     - rebate_amount [integer, default 0]: credit analysis fee deducted from lent amount. ex: 11234 (= R$ 112.34)
     - tags [list of strings, default []]: list of strings for reference when searching for CreditNotes. ex: ["employees", "monthly"]
     - expiration [integer or datetime.timedelta, default 604800 (7 days)]: time interval in seconds between scheduled date and expiration date. ex 123456789
     ## Attributes (return-only):
     - id [string]: unique id returned when the CreditNote is created. ex: "5656565656565656"
-    - amount [integer]: CreditNote value in cents. ex: 1234 (= R$ 12.34)
     - document_id [string]: ID of the signed document to execute this CreditNote. ex: "4545454545454545"
     - status [string]: current status of the CreditNote. ex: "canceled", "created", "expired", "failed", "processing", "signed", "success"
     - transaction_ids [list of strings]: ledger transaction ids linked to this CreditNote. ex: ["19827356981273"]
     - workspace_id [string]: ID of the Workspace that generated this CreditNote. ex: "4545454545454545"
     - tax_amount [integer]: tax amount included in the CreditNote. ex: 100
     - nominal_interest [float]: yearly nominal interest rate of the CreditNote, in percentage. ex: 11.5
     - interest [float]: yearly effective interest rate of the CreditNote, in percentage. ex: 12.5
     - created [datetime.datetime]: creation datetime for the CreditNote. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - updated [datetime.datetime]: latest update datetime for the CreditNote. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
-    def __init__(self, template_id, name, tax_id, nominal_amount, scheduled, invoices, payment, signers, external_id,
+    def __init__(self, template_id, name, tax_id, scheduled, invoices, payment, signers, external_id,
                  street_line_1, street_line_2, district, city, state_code, zip_code, payment_type=None,
-                 rebate_amount=None, tags=None, expiration=None, id=None, amount=None, document_id=None, status=None,
-                 transaction_ids=None, workspace_id=None, tax_amount=None, nominal_interest=None, interest=None, created=None, updated=None):
+                 nominal_amount=None, amount=None, rebate_amount=None, tags=None, expiration=None, id=None,
+                 document_id=None, status=None, transaction_ids=None, workspace_id=None, tax_amount=None,
+                 nominal_interest=None, interest=None, created=None, updated=None):
         Resource.__init__(self, id=id)
 
         self.template_id = template_id
         self.name = name
         self.tax_id = tax_id
-        self.nominal_amount = nominal_amount
         self.scheduled = scheduled
         self.invoices = _parse_invoices(invoices)
         self.signers = _parse_signers(signers)
         self.external_id = external_id
         self.street_line_1 = street_line_1
         self.street_line_2 = street_line_2
         self.district = district
         self.city = city
         self.state_code = state_code
         self.zip_code = zip_code
+        self.nominal_amount = nominal_amount
+        self.amount = amount
         self.rebate_amount = rebate_amount
         self.tags = tags
         self.expiration = expiration
-        self.amount = amount
         self.document_id = document_id
         self.status = status
         self.transaction_ids = transaction_ids
         self.workspace_id = workspace_id
         self.tax_amount = tax_amount
         self.nominal_interest = nominal_interest
         self.interest = interest
```

### Comparing `starkinfra-0.7.0/starkinfra/creditnote/__transfer.py` & `starkinfra-0.8.0/starkinfra/creditnote/__transfer.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditnote/invoice/__description.py` & `starkinfra-0.8.0/starkinfra/creditnote/invoice/__description.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditnote/invoice/__invoice.py` & `starkinfra-0.8.0/starkinfra/creditnote/invoice/__invoice.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditnote/log/__log.py` & `starkinfra-0.8.0/starkinfra/creditnote/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditpreview/__creditnotepreview.py` & `starkinfra-0.8.0/starkinfra/creditpreview/__creditnotepreview.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditpreview/__creditpreview.py` & `starkinfra-0.8.0/starkinfra/creditpreview/__creditpreview.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/creditsigner/__creditsigner.py` & `starkinfra-0.8.0/starkinfra/creditsigner/__creditsigner.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/dynamicbrcode/__dynamicbrcode.py` & `starkinfra-0.8.0/starkinfra/dynamicbrcode/__dynamicbrcode.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/event/__event.py` & `starkinfra-0.8.0/starkinfra/event/__event.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/event/attempt/__attempt.py` & `starkinfra-0.8.0/starkinfra/event/attempt/__attempt.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/individualdocument/__individualdocument.py` & `starkinfra-0.8.0/starkinfra/individualdocument/__individualdocument.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/individualdocument/log/__log.py` & `starkinfra-0.8.0/starkinfra/individualdocument/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/individualidentity/__individualidentity.py` & `starkinfra-0.8.0/starkinfra/individualidentity/__individualidentity.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/individualidentity/log/__log.py` & `starkinfra-0.8.0/starkinfra/individualidentity/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingbalance/__issuingbalance.py` & `starkinfra-0.8.0/starkinfra/issuingbalance/__issuingbalance.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingcard/__issuingcard.py` & `starkinfra-0.8.0/starkinfra/issuingcard/__issuingcard.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingcard/log/__log.py` & `starkinfra-0.8.0/starkinfra/issuingcard/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingdesign/__issuingdesign.py` & `starkinfra-0.8.0/starkinfra/issuingdesign/__issuingdesign.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingembossingkit/__issuingembossingkit.py` & `starkinfra-0.8.0/starkinfra/issuingembossingkit/__issuingembossingkit.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py` & `starkinfra-0.8.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingembossingrequest/log/__log.py` & `starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingholder/__issuingholder.py` & `starkinfra-0.8.0/starkinfra/issuingholder/__issuingholder.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingholder/log/__log.py` & `starkinfra-0.8.0/starkinfra/issuingholder/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuinginvoice/__issuinginvoice.py` & `starkinfra-0.8.0/starkinfra/issuinginvoice/__issuinginvoice.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuinginvoice/log/__log.py` & `starkinfra-0.8.0/starkinfra/issuinginvoice/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingproduct/__issuingproduct.py` & `starkinfra-0.8.0/starkinfra/issuingproduct/__issuingproduct.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingpurchase/__issuingpurchase.py` & `starkinfra-0.8.0/starkinfra/issuingpurchase/__issuingpurchase.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingpurchase/log/__log.py` & `starkinfra-0.8.0/starkinfra/issuingpurchase/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingrestock/__issuingrestock.py` & `starkinfra-0.8.0/starkinfra/issuingrestock/__issuingrestock.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingrestock/log/__log.py` & `starkinfra-0.8.0/starkinfra/issuingrestock/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingrule/__issuingrule.py` & `starkinfra-0.8.0/starkinfra/issuingrule/__issuingrule.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingstock/__issuingstock.py` & `starkinfra-0.8.0/starkinfra/issuingstock/__issuingstock.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingstock/log/__log.py` & `starkinfra-0.8.0/starkinfra/issuingstock/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingtransaction/__issuingtransaction.py` & `starkinfra-0.8.0/starkinfra/issuingtransaction/__issuingtransaction.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py` & `starkinfra-0.8.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/merchantcategory/__merchantcategory.py` & `starkinfra-0.8.0/starkinfra/merchantcategory/__merchantcategory.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/merchantcountry/__merchantcountry.py` & `starkinfra-0.8.0/starkinfra/merchantcountry/__merchantcountry.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixbalance/__pixbalance.py` & `starkinfra-0.8.0/starkinfra/pixbalance/__pixbalance.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixchargeback/__pixchargeback.py` & `starkinfra-0.8.0/starkinfra/pixchargeback/__pixchargeback.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixchargeback/log/__log.py` & `starkinfra-0.8.0/starkinfra/pixchargeback/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixclaim/__pixclaim.py` & `starkinfra-0.8.0/starkinfra/pixclaim/__pixclaim.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixclaim/log/__log.py` & `starkinfra-0.8.0/starkinfra/pixclaim/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixdirector/__pixdirector.py` & `starkinfra-0.8.0/starkinfra/pixdirector/__pixdirector.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixdomain/__pixdomain.py` & `starkinfra-0.8.0/starkinfra/pixdomain/__pixdomain.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixinfraction/__pixinfraction.py` & `starkinfra-0.8.0/starkinfra/pixinfraction/__pixinfraction.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixinfraction/log/__log.py` & `starkinfra-0.8.0/starkinfra/pixinfraction/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixkey/__pixkey.py` & `starkinfra-0.8.0/starkinfra/pixkey/__pixkey.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixkey/log/__log.py` & `starkinfra-0.8.0/starkinfra/pixkey/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixrequest/__pixrequest.py` & `starkinfra-0.8.0/starkinfra/pixrequest/__pixrequest.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixrequest/log/__log.py` & `starkinfra-0.8.0/starkinfra/pixrequest/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixreversal/__pixreversal.py` & `starkinfra-0.8.0/starkinfra/pixreversal/__pixreversal.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixreversal/log/__log.py` & `starkinfra-0.8.0/starkinfra/pixreversal/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/pixstatement/__pixstatement.py` & `starkinfra-0.8.0/starkinfra/pixstatement/__pixstatement.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/staticbrcode/__staticbrcode.py` & `starkinfra-0.8.0/starkinfra/staticbrcode/__staticbrcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,35 +11,37 @@
     created in the Stark Infra API. The 'create' function sends the objects
     ## Parameters (required):
     - name [string]: receiver's name. ex: "Tony Stark"
     - key_id [string]: receiver's Pixkey id. ex: "+5541999999999"
     - city [string]: receiver's city name. ex: "Rio de Janeiro"
     ## Parameters (optional):
     - amount [integer, default 0]: positive integer that represents the amount in cents of the resulting Pix transaction. ex: 1234 (= R$ 12.34)
-    - cashier_bank_code [string, default ""] Cashier's bank code. ex: "20018183".
+    - cashier_bank_code [string, default None]: Cashier's bank code. ex: "20018183".
     - reconciliation_id [string, default None]: id to be used for conciliation of the resulting Pix transaction. This id must have up to 25 alphanumeric characters ex: "ah27s53agj6493hjds6836v49"
+    - description [string, default None]: optional description to override default description to be shown in the bank statement. ex: "Payment for service #1234"
     - tags [list of strings, default []]: list of strings for tagging. ex: ["travel", "food"]
     ## Attributes (return-only):
     - id [string]: id returned on creation, this is the BR code. ex: "00020126360014br.gov.bcb.pix0114+552840092118152040000530398654040.095802BR5915Jamie Lannister6009Sao Paulo620705038566304FC6C"
     - uuid [string]: unique uuid returned when a StaticBrcode is created. ex: "97756273400d42ce9086404fe10ea0d6"
     - url [string]: url link to the BR code image. ex: "https://brcode-h.development.starkinfra.com/static-qrcode/97756273400d42ce9086404fe10ea0d6.png"
     - updated [datetime.datetime]: latest update datetime for the StaticBrcode. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - created [datetime.datetime]: creation datetime for the StaticBrcode. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
     def __init__(self, name, key_id, city, amount=None, cashier_bank_code=None, reconciliation_id=None, tags=None,
-                 id=None, uuid=None, url=None, updated=None, created=None):
+                 id=None, description=None, uuid=None, url=None, updated=None, created=None):
         Resource.__init__(self, id=id)
 
         self.name = name
         self.key_id = key_id
         self.city = city
         self.amount = amount
         self.cashier_bank_code = cashier_bank_code
         self.reconciliation_id = reconciliation_id
+        self.description = description
         self.tags = tags
         self.uuid = uuid
         self.url = url
         self.updated = check_datetime(updated)
         self.created = check_datetime(created)
```

### Comparing `starkinfra-0.7.0/starkinfra/utils/relay.py` & `starkinfra-0.8.0/starkinfra/utils/relay.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra/webhook/__webhook.py` & `starkinfra-0.8.0/starkinfra/webhook/__webhook.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.7.0/starkinfra.egg-info/PKG-INFO` & `starkinfra-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: starkinfra
-Version: 0.7.0
-Summary: SDK to facilitate Python integrations with Stark Infra
-Home-page: https://github.com/starkinfra/sdk-python
-Author: Stark Infra
-Author-email: developers@starkbank.com
-License: MIT License
-Keywords: stark infra,starkinfra,sdk,open banking,openbanking,banking,open,stark
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Stark Infra Python SDK - Beta
 
 Welcome to the Stark Infra Python SDK! This tool is made for Python 
 developers who want to easily integrate with our API.
 This SDK version is compatible with the Stark Infra API v2.
 
 # Introduction
@@ -2188,18 +2175,20 @@
 You can create BrcodePreviews to preview BR Codes before paying them.
 
 ```python
 import starkinfra
 
 previews = starkinfra.brcodepreview.create([
     starkinfra.BrcodePreview(
-        id="00020126420014br.gov.bcb.pix0120nedstark@hotmail.com52040000530398654075000.005802BR5909Ned Stark6014Rio de Janeiro621605126674869738606304FF71"
+        id="00020126420014br.gov.bcb.pix0120nedstark@hotmail.com52040000530398654075000.005802BR5909Ned Stark6014Rio de Janeiro621605126674869738606304FF71",
+        payer_id="012.345.678-90"
     ),
     starkinfra.BrcodePreview(
-        id="00020126430014br.gov.bcb.pix0121aryastark@hotmail.com5204000053039865406100.005802BR5910Arya Stark6014Rio de Janeiro6216051262678188104863042BA4"
+        id="00020126430014br.gov.bcb.pix0121aryastark@hotmail.com5204000053039865406100.005802BR5910Arya Stark6014Rio de Janeiro6216051262678188104863042BA4",
+        payer_id="012.345.678-90"
     ),
 ])
 
 for preview in previews:
     print(preview)
 ```
 
@@ -2961,9 +2950,7 @@
 # Help and Feedback
 
 If you have any questions about our SDK, just send us an email.
 We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
 We also love feedback, so don't be shy about sharing your thoughts with us.
 
 Email: help@starkbank.com
-
-
```

### Comparing `starkinfra-0.7.0/starkinfra.egg-info/SOURCES.txt` & `starkinfra-0.8.0/starkinfra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

