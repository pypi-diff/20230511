# Comparing `tmp/mindee-3.8.0.tar.gz` & `tmp/mindee-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-3.8.0.tar", last modified: Wed May 10 13:39:45 2023, max compression
+gzip compressed data, was "mindee-3.8.1.tar", last modified: Thu May 11 14:53:19 2023, max compression
```

## Comparing `mindee-3.8.0.tar` & `mindee-3.8.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 13:39:26.000000 mindee-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-10 13:39:45.412331 mindee-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-10 13:39:26.000000 mindee-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/documents/cropper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/cropper/cropper_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/documents/custom/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/custom/custom_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/eu/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/eu/license_plate/license_plate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/financial/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/financial/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/financial/financial_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_grise/carte_grise_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/id_card/id_card_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/line_item_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/invoice_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice_splitter/invoice_splitter_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/passport/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/passport/passport_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/proof_of_address/proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/receipt/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/line_item_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/receipt_v5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/documents/shipping_container/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/shipping_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/shipping_container/shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/documents/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/api_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/response.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/version
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:39:30.000000 mindee-3.8.0/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-10 13:39:26.000000 mindee-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-10 13:39:45.412331 mindee-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-10 13:39:26.000000 mindee-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_financial_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_invoice_splitter_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/us/test_bank_check_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_pkg_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 14:52:52.000000 mindee-3.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-11 14:53:19.870598 mindee-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-11 14:52:52.000000 mindee-3.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.854597 mindee-3.8.1/mindee/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/cropper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/cropper/cropper_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/custom/custom_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/eu/license_plate/license_plate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/financial/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/financial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/financial/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/financial/financial_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_grise/carte_grise_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/id_card/id_card_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/line_item_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice_splitter/invoice_splitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/passport/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/passport/passport_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/proof_of_address/proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/receipt/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/line_item_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/receipt_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/shipping_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/shipping_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/shipping_container/shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.866598 mindee-3.8.1/mindee/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/api_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.866598 mindee-3.8.1/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.854597 mindee-3.8.1/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:53:01.000000 mindee-3.8.1/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-11 14:52:52.000000 mindee-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-11 14:53:19.870598 mindee-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 14:52:52.000000 mindee-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.866598 mindee-3.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_financial_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/us/test_bank_check_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_pkg_versions.py
```

### Comparing `mindee-3.8.0/LICENSE` & `mindee-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/PKG-INFO` & `mindee-3.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.8.0
+Version: 3.8.1
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.8.0/README.md` & `mindee-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/cli.py` & `mindee-3.8.1/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/client.py` & `mindee-3.8.1/mindee/client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/__init__.py` & `mindee-3.8.1/mindee/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/base.py` & `mindee-3.8.1/mindee/documents/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/config.py` & `mindee-3.8.1/mindee/documents/config.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/cropper/cropper_v1.py` & `mindee-3.8.1/mindee/documents/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/custom/custom_v1.py` & `mindee-3.8.1/mindee/documents/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/eu/license_plate/license_plate_v1.py` & `mindee-3.8.1/mindee/documents/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/financial/financial_document_v1.py` & `mindee-3.8.1/mindee/documents/financial/financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/financial/financial_v1.py` & `mindee-3.8.1/mindee/documents/financial/financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py` & `mindee-3.8.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/fr/carte_grise/carte_grise_v1.py` & `mindee-3.8.1/mindee/documents/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py` & `mindee-3.8.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/fr/id_card/id_card_v1.py` & `mindee-3.8.1/mindee/documents/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/invoice/checks.py` & `mindee-3.8.1/mindee/documents/invoice/checks.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/invoice/invoice_v3.py` & `mindee-3.8.1/mindee/documents/invoice/invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/invoice/invoice_v4.py` & `mindee-3.8.1/mindee/documents/invoice/invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/invoice/line_item_v4.py` & `mindee-3.8.1/mindee/documents/invoice/line_item_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/invoice/reconstruct.py` & `mindee-3.8.1/mindee/documents/invoice/reconstruct.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/invoice_splitter/invoice_splitter_v1.py` & `mindee-3.8.1/mindee/documents/invoice_splitter/invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/passport/passport_v1.py` & `mindee-3.8.1/mindee/documents/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/proof_of_address/proof_of_address_v1.py` & `mindee-3.8.1/mindee/documents/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/receipt/line_item_v5.py` & `mindee-3.8.1/mindee/documents/receipt/line_item_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/receipt/receipt_v3.py` & `mindee-3.8.1/mindee/documents/receipt/receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/receipt/receipt_v4.py` & `mindee-3.8.1/mindee/documents/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/receipt/receipt_v5.py` & `mindee-3.8.1/mindee/documents/receipt/receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/shipping_container/shipping_container_v1.py` & `mindee-3.8.1/mindee/documents/shipping_container/shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/documents/us/bank_check/bank_check_v1.py` & `mindee-3.8.1/mindee/documents/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/endpoints.py` & `mindee-3.8.1/mindee/endpoints.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/amount.py` & `mindee-3.8.1/mindee/fields/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/api_builder.py` & `mindee-3.8.1/mindee/fields/api_builder.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/base.py` & `mindee-3.8.1/mindee/fields/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/company_registration.py` & `mindee-3.8.1/mindee/fields/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/date.py` & `mindee-3.8.1/mindee/fields/date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/locale.py` & `mindee-3.8.1/mindee/fields/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/orientation.py` & `mindee-3.8.1/mindee/fields/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/payment_details.py` & `mindee-3.8.1/mindee/fields/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/position.py` & `mindee-3.8.1/mindee/fields/position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/tax.py` & `mindee-3.8.1/mindee/fields/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/fields/text.py` & `mindee-3.8.1/mindee/fields/text.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/geometry.py` & `mindee-3.8.1/mindee/geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/input/page_options.py` & `mindee-3.8.1/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/input/sources.py` & `mindee-3.8.1/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee/response.py` & `mindee-3.8.1/mindee/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class Job:
     """
     Job class for asynchronous requests.
 
     Will hold information on the queue a document has been submitted to.
     """
 
-    job_id: Optional[str] = None
+    id: Optional[str] = None
     """ID of the job sent by the API in response to an enqueue request."""
     issued_at: datetime
     """Timestamp of the request reception by the API."""
     available_at: Optional[datetime] = None
     """Timestamp of the request after it has been completed."""
     status: Optional[str] = None
     """Status of the request, as seen by the API."""
@@ -53,15 +53,15 @@
         Wrapper for the HTTP response sent from the API when a document is enqueued.
 
         :param json_response: JSON response sent by the server
         """
         self.issued_at = datetime.fromisoformat(json_response["issued_at"])
         if json_response.get("available_at"):
             self.available_at = datetime.fromisoformat(json_response["available_at"])
-        self.job_id = json_response.get("id")
+        self.id = json_response.get("id")
         self.status = json_response.get("status")
         if self.available_at:
             self.millisecs_taken = int(
                 (self.available_at - self.issued_at).total_seconds() * 1000
             )
 
     def __str__(self) -> str:
```

### Comparing `mindee-3.8.0/mindee/versions.py` & `mindee-3.8.1/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/mindee.egg-info/PKG-INFO` & `mindee-3.8.1/mindee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.8.0
+Version: 3.8.1
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.8.0/mindee.egg-info/SOURCES.txt` & `mindee-3.8.1/mindee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/pyproject.toml` & `mindee-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/setup.cfg` & `mindee-3.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/fr/test_bank_account_details_v1.py` & `mindee-3.8.1/tests/documents/fr/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/fr/test_carte_grise_v1.py` & `mindee-3.8.1/tests/documents/fr/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/fr/test_carte_vitale_v1.py` & `mindee-3.8.1/tests/documents/fr/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/fr/test_id_card_v1.py` & `mindee-3.8.1/tests/documents/fr/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_cropper_v1.py` & `mindee-3.8.1/tests/documents/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_custom_v1.py` & `mindee-3.8.1/tests/documents/test_custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_financial_document_v1.py` & `mindee-3.8.1/tests/documents/test_financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_financial_v1.py` & `mindee-3.8.1/tests/documents/test_financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_invoice_splitter_v1.py` & `mindee-3.8.1/tests/documents/test_invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_invoice_v3.py` & `mindee-3.8.1/tests/documents/test_invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_invoice_v4.py` & `mindee-3.8.1/tests/documents/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_passport_v1.py` & `mindee-3.8.1/tests/documents/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_proof_of_address_v1.py` & `mindee-3.8.1/tests/documents/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_receipt_v3.py` & `mindee-3.8.1/tests/documents/test_receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_receipt_v4.py` & `mindee-3.8.1/tests/documents/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_receipt_v5.py` & `mindee-3.8.1/tests/documents/test_receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/test_shipping_container_v1.py` & `mindee-3.8.1/tests/documents/test_shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/documents/us/test_bank_check_v1.py` & `mindee-3.8.1/tests/documents/us/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_amount.py` & `mindee-3.8.1/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_date.py` & `mindee-3.8.1/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_field.py` & `mindee-3.8.1/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_locale.py` & `mindee-3.8.1/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_orientation.py` & `mindee-3.8.1/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_payment_details.py` & `mindee-3.8.1/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_position.py` & `mindee-3.8.1/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/fields/test_tax.py` & `mindee-3.8.1/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/test_cli.py` & `mindee-3.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/test_client.py` & `mindee-3.8.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/test_geometry.py` & `mindee-3.8.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/test_inputs.py` & `mindee-3.8.1/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.0/tests/test_pkg_versions.py` & `mindee-3.8.1/tests/test_pkg_versions.py`

 * *Files identical despite different names*

