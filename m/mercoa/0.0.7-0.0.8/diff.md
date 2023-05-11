# Comparing `tmp/mercoa-0.0.7.tar.gz` & `tmp/mercoa-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.0.7.tar", max compression
+gzip compressed data, was "mercoa-0.0.8.tar", max compression
```

## Comparing `mercoa-0.0.7.tar` & `mercoa-0.0.8.tar`

### file list

```diff
@@ -1,137 +1,144 @@
--rw-r--r--   0        0        0      410 2023-05-05 17:43:49.129647 mercoa-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4757 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/__init__.py
--rw-r--r--   0        0        0     4619 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      326 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/py.typed
--rw-r--r--   0        0        0     4879 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     2582 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      359 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      148 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      216 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      407 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      855 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      141 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4542 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/client.py
--rw-r--r--   0        0        0      157 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0      753 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    18085 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     1104 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0     1535 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0       80 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_id.py
--rw-r--r--   0        0        0     1262 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1497 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     1302 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0     1372 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0      974 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      761 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      207 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/__init__.py
--rw-r--r--   0        0        0     9662 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/client.py
--rw-r--r--   0        0        0      281 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/__init__.py
--rw-r--r--   0        0        0       84 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_response.py
--rw-r--r--   0        0        0      695 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    19563 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0     1012 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0       81 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_id.py
--rw-r--r--   0        0        0      750 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_request.py
--rw-r--r--   0        0        0      937 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_response.py
--rw-r--r--   0        0        0     1048 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/create_vendor_request.py
--rw-r--r--   0        0        0      955 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/document_response.py
--rw-r--r--   0        0        0       81 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_id.py
--rw-r--r--   0        0        0     1253 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1180 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     3388 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     3075 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1332 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0     1060 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_response.py
--rw-r--r--   0        0        0     1261 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_status.py
--rw-r--r--   0        0        0      213 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4443 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      298 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/attachments.py
--rw-r--r--   0        0        0     1969 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/email_ocr_request.py
--rw-r--r--   0        0        0      891 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_mailbox.py
--rw-r--r--   0        0        0     1234 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      983 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0     7449 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-05-05 17:43:49.129647 mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      656 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1009 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      797 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0      943 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    12242 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/client.py
--rw-r--r--   0        0        0     1411 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0       85 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_id.py
--rw-r--r--   0        0        0     1297 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1318 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0       78 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_id.py
--rw-r--r--   0        0        0     1120 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1217 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0       79 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_id.py
--rw-r--r--   0        0        0     1152 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1327 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0       80 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_id.py
--rw-r--r--   0        0        0     1568 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1922 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0       87 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_id.py
--rw-r--r--   0        0        0     1296 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1508 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      425 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0     6115 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      589 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1160 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1249 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1468 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      269 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/__init__.py
--rw-r--r--   0        0        0     8182 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-05-05 17:43:49.133648 mercoa-0.0.7/src/mercoa/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-05-11 04:26:07.369902 mercoa-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4995 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     5019 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/py.typed
+-rw-r--r--   0        0        0     5125 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     2582 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      359 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      407 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      855 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      199 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4513 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/client.py
+-rw-r--r--   0        0        0      256 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/types/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/types/counterparty_response.py
+-rw-r--r--   0        0        0     1446 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/types/find_counterparties_response.py
+-rw-r--r--   0        0        0      811 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    21970 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     1195 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/account_type.py
+-rw-r--r--   0        0        0     1535 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/business_type.py
+-rw-r--r--   0        0        0      741 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/ein.py
+-rw-r--r--   0        0        0       80 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_id.py
+-rw-r--r--   0        0        0     1546 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_request.py
+-rw-r--r--   0        0        0     1590 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_status.py
+-rw-r--r--   0        0        0     1586 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_update_request.py
+-rw-r--r--   0        0        0     1372 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_response.py
+-rw-r--r--   0        0        0     1059 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0      974 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/profile_response.py
+-rw-r--r--   0        0        0      761 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/tax_id.py
+-rw-r--r--   0        0        0      207 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/__init__.py
+-rw-r--r--   0        0        0     9662 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/client.py
+-rw-r--r--   0        0        0      281 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_response.py
+-rw-r--r--   0        0        0      633 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    19563 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      916 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_id.py
+-rw-r--r--   0        0        0      750 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_request.py
+-rw-r--r--   0        0        0      937 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_response.py
+-rw-r--r--   0        0        0     1048 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/create_vendor_request.py
+-rw-r--r--   0        0        0    22179 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/currency_code.py
+-rw-r--r--   0        0        0      955 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/document_response.py
+-rw-r--r--   0        0        0       81 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_id.py
+-rw-r--r--   0        0        0     1302 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1229 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     3437 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_request.py
+-rw-r--r--   0        0        0     3144 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_response.py
+-rw-r--r--   0        0        0     1332 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_status.py
+-rw-r--r--   0        0        0      213 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4443 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      298 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/attachments.py
+-rw-r--r--   0        0        0     1969 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/email_ocr_request.py
+-rw-r--r--   0        0        0      891 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_mailbox.py
+-rw-r--r--   0        0        0     1234 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      983 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0     7449 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      656 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1145 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      797 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0      943 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    12242 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/client.py
+-rw-r--r--   0        0        0     1411 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_id.py
+-rw-r--r--   0        0        0     1297 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_request.py
+-rw-r--r--   0        0        0     1318 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_brand.py
+-rw-r--r--   0        0        0       78 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_id.py
+-rw-r--r--   0        0        0     1120 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_request.py
+-rw-r--r--   0        0        0     1217 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_type.py
+-rw-r--r--   0        0        0       79 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_id.py
+-rw-r--r--   0        0        0     1152 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_request.py
+-rw-r--r--   0        0        0     1327 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_response.py
+-rw-r--r--   0        0        0       80 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_id.py
+-rw-r--r--   0        0        0     1568 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1922 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0       87 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_id.py
+-rw-r--r--   0        0        0     1296 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_request.py
+-rw-r--r--   0        0        0     1508 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_response.py
+-rw-r--r--   0        0        0     1229 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_type.py
+-rw-r--r--   0        0        0      425 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0     7794 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0      589 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/__init__.py
+-rw-r--r--   0        0        0     1984 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1249 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1468 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0      269 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/__init__.py
+-rw-r--r--   0        0        0     8182 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/client.py
+-rw-r--r--   0        0        0      381 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/responsibilities.py
+-rw-r--r--   0        0        0      211 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     4206 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      284 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1125 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1261 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.8/PKG-INFO
```

### Comparing `mercoa-0.0.7/src/mercoa/__init__.py` & `mercoa-0.0.8/src/mercoa/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     ColorSchemeRequest,
     ColorSchemeResponse,
     CommentId,
     CommentRequest,
     CommentResponse,
     CounterpartyResponse,
     CreateVendorRequest,
+    CurrencyCode,
     CustomId,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
     DocumentResponse,
     Ein,
     EmailLogResponse,
     EmailOcrRequest,
@@ -49,21 +50,23 @@
     EntityRequest,
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     EntityUserId,
     EntityUserRequest,
     EntityUserResponse,
+    FindCounterpartiesResponse,
     FullName,
     IndividualGovernmentID,
     IndividualProfileRequest,
     IndividualProfileResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
+    InvoiceMetricsResponse,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     OcrMailbox,
     OCRResponse,
     OrganizationId,
     OrganizationRequest,
@@ -87,28 +90,30 @@
     ProfileRequest,
     ProfileResponse,
     RepresentativeId,
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
     TaxID,
+    TransactionId,
     TransactionResponse,
     TransactionStatus,
     UnauthorizedError,
     bank_lookup,
     commons,
     counterparty,
     entity,
     entity_users,
     invoice,
     ocr,
     organization,
     payment_method,
     payment_method_schema,
     representative,
+    transaction,
 )
 
 __all__ = [
     "AccountType",
     "Address",
     "Attachments",
     "BankAccountId",
@@ -133,14 +138,15 @@
     "ColorSchemeRequest",
     "ColorSchemeResponse",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "CounterpartyResponse",
     "CreateVendorRequest",
+    "CurrencyCode",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "DocumentResponse",
     "Ein",
     "EmailLogResponse",
     "EmailOcrRequest",
@@ -153,22 +159,24 @@
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
+    "FindCounterpartiesResponse",
     "FullName",
     "ITIN",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
+    "InvoiceMetricsResponse",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "MercoaEnvironment",
     "OCRResponse",
     "OcrMailbox",
     "OrganizationId",
@@ -194,22 +202,24 @@
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "SSN",
     "TaxID",
+    "TransactionId",
     "TransactionResponse",
     "TransactionStatus",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
     "entity_users",
     "invoice",
     "ocr",
     "organization",
     "payment_method",
     "payment_method_schema",
     "representative",
+    "transaction",
 ]
```

### Comparing `mercoa-0.0.7/src/mercoa/client.py` & `mercoa-0.0.8/src/mercoa/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .resources.entity_users.client import AsyncEntityUsersClient, EntityUsersClient
 from .resources.invoice.client import AsyncInvoiceClient, InvoiceClient
 from .resources.ocr.client import AsyncOcrClient, OcrClient
 from .resources.organization.client import AsyncOrganizationClient, OrganizationClient
 from .resources.payment_method.client import AsyncPaymentMethodClient, PaymentMethodClient
 from .resources.payment_method_schema.client import AsyncPaymentMethodSchemaClient, PaymentMethodSchemaClient
 from .resources.representative.client import AsyncRepresentativeClient, RepresentativeClient
+from .resources.transaction.client import AsyncTransactionClient, TransactionClient
 
 
 class Mercoa:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -60,14 +61,18 @@
     def payment_method(self) -> PaymentMethodClient:
         return PaymentMethodClient(environment=self._environment, token=self._token)
 
     @cached_property
     def representative(self) -> RepresentativeClient:
         return RepresentativeClient(environment=self._environment, token=self._token)
 
+    @cached_property
+    def transaction(self) -> TransactionClient:
+        return TransactionClient(environment=self._environment, token=self._token)
+
 
 class AsyncMercoa:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
@@ -107,7 +112,11 @@
     @cached_property
     def payment_method(self) -> AsyncPaymentMethodClient:
         return AsyncPaymentMethodClient(environment=self._environment, token=self._token)
 
     @cached_property
     def representative(self) -> AsyncRepresentativeClient:
         return AsyncRepresentativeClient(environment=self._environment, token=self._token)
+
+    @cached_property
+    def transaction(self) -> AsyncTransactionClient:
+        return AsyncTransactionClient(environment=self._environment, token=self._token)
```

### Comparing `mercoa-0.0.7/src/mercoa/core/datetime_utils.py` & `mercoa-0.0.8/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.0.8/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,50 +8,51 @@
     entity_users,
     invoice,
     ocr,
     organization,
     payment_method,
     payment_method_schema,
     representative,
+    transaction,
 )
 from .bank_lookup import BankAddress, BankLookupResponse
 from .commons import ITIN, SSN, Address, BirthDate, FullName, IndividualGovernmentID, PhoneNumber, UnauthorizedError
-from .counterparty import CounterpartyResponse
+from .counterparty import CounterpartyResponse, FindCounterpartiesResponse
 from .entity import (
     AccountType,
     BusinessProfileRequest,
     BusinessProfileResponse,
     BusinessType,
     Ein,
     EntityId,
     EntityRequest,
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     IndividualProfileRequest,
     IndividualProfileResponse,
+    InvoiceMetricsResponse,
     ProfileRequest,
     ProfileResponse,
     TaxID,
 )
 from .entity_users import EntityUserId, EntityUserRequest, EntityUserResponse
 from .invoice import (
     CommentId,
     CommentRequest,
     CommentResponse,
     CreateVendorRequest,
+    CurrencyCode,
     DocumentResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
-    TransactionResponse,
-    TransactionStatus,
 )
 from .ocr import Attachments, EmailOcrRequest, OcrMailbox, OCRResponse
 from .organization import (
     ColorSchemeRequest,
     ColorSchemeResponse,
     EmailLogResponse,
     EmailProviderRequest,
@@ -95,14 +96,15 @@
     PaymentMethodSchemaField,
     PaymentMethodSchemaFieldType,
     PaymentMethodSchemaId,
     PaymentMethodSchemaRequest,
     PaymentMethodSchemaResponse,
 )
 from .representative import RepresentativeId, RepresentativeRequest, RepresentativeResponse, Responsibilities
+from .transaction import TransactionId, TransactionResponse, TransactionStatus
 
 __all__ = [
     "AccountType",
     "Address",
     "Attachments",
     "BankAccountId",
     "BankAccountRequest",
@@ -126,14 +128,15 @@
     "ColorSchemeRequest",
     "ColorSchemeResponse",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "CounterpartyResponse",
     "CreateVendorRequest",
+    "CurrencyCode",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "DocumentResponse",
     "Ein",
     "EmailLogResponse",
     "EmailOcrRequest",
@@ -146,22 +149,24 @@
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
+    "FindCounterpartiesResponse",
     "FullName",
     "ITIN",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
+    "InvoiceMetricsResponse",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "OCRResponse",
     "OcrMailbox",
     "OrganizationId",
     "OrganizationRequest",
@@ -186,22 +191,24 @@
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "SSN",
     "TaxID",
+    "TransactionId",
     "TransactionResponse",
     "TransactionStatus",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
     "entity_users",
     "invoice",
     "ocr",
     "organization",
     "payment_method",
     "payment_method_schema",
     "representative",
+    "transaction",
 ]
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.0.8/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/commons/types/address.py` & `mercoa-0.0.8/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.0.8/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.0.8/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.0.8/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.0.8/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.0.8/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.0.8/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/counterparty/client.py` & `mercoa-0.0.8/src/mercoa/resources/counterparty/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..entity.types.entity_id import EntityId
 from ..entity.types.entity_response import EntityResponse
-from .types.counterparty_response import CounterpartyResponse
+from .types.find_counterparties_response import FindCounterpartiesResponse
 
 
 class CounterpartyClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -34,31 +34,29 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def find(
-        self, entity_id: EntityId, *, payment_methods: typing.Optional[bool] = None
-    ) -> typing.List[CounterpartyResponse]:
+    def find(self, entity_id: EntityId, *, payment_methods: typing.Optional[bool] = None) -> FindCounterpartiesResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/counterparties"),
             params={"paymentMethods": payment_methods},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[CounterpartyResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindCounterpartiesResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncCounterpartyClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
@@ -80,24 +78,24 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def find(
         self, entity_id: EntityId, *, payment_methods: typing.Optional[bool] = None
-    ) -> typing.List[CounterpartyResponse]:
+    ) -> FindCounterpartiesResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/counterparties"),
                 params={"paymentMethods": payment_methods},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[CounterpartyResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindCounterpartiesResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/counterparty/types/counterparty_response.py` & `mercoa-0.0.8/src/mercoa/resources/counterparty/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/entity/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     EntityId,
     EntityRequest,
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     IndividualProfileRequest,
     IndividualProfileResponse,
+    InvoiceMetricsResponse,
     ProfileRequest,
     ProfileResponse,
     TaxID,
 )
 
 __all__ = [
     "AccountType",
@@ -27,11 +28,12 @@
     "EntityId",
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
+    "InvoiceMetricsResponse",
     "ProfileRequest",
     "ProfileResponse",
     "TaxID",
 ]
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/client.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,376 +7,403 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from ..invoice.types.invoice_response import InvoiceResponse
-from ..invoice.types.invoice_status import InvoiceStatus
-from .types.entity_id import EntityId
-from .types.entity_request import EntityRequest
-from .types.entity_response import EntityResponse
-from .types.entity_status import EntityStatus
-from .types.entity_update_request import EntityUpdateRequest
+from .types.comment_id import CommentId
+from .types.comment_request import CommentRequest
+from .types.comment_response import CommentResponse
+from .types.document_response import DocumentResponse
+from .types.invoice_id import InvoiceId
+from .types.invoice_request import InvoiceRequest
+from .types.invoice_response import InvoiceResponse
 
 
-class EntityClient:
+class InvoiceClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def get_all(self) -> typing.List[EntityResponse]:
+    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def find(
-        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
-    ) -> typing.List[EntityResponse]:
+    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
-            params={"foreignId": foreign_id, "status": status},
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, *, request: EntityRequest) -> EntityResponse:
+    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, entity_id: EntityId) -> EntityResponse:
+    def delete(self, invoice_id: InvoiceId) -> None:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
+    def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
         _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
-            json=jsonable_encoder(request),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, entity_id: EntityId) -> None:
+    def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_invoices(
-        self, entity_id: EntityId, *, status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]]
-    ) -> typing.List[InvoiceResponse]:
+    def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
-            params={"status": status},
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def accept_terms_of_service(self, entity_id: EntityId) -> str:
+    def edit_comment(self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest) -> CommentResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_token(self, entity_id: EntityId) -> str:
+    def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def plaid_link_token(self, entity_id: EntityId) -> str:
+    def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
 
-class AsyncEntityClient:
+
+class AsyncInvoiceClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def get_all(self) -> typing.List[EntityResponse]:
+    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def find(
-        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
-    ) -> typing.List[EntityResponse]:
+    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
-                params={"foreignId": foreign_id, "status": status},
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, *, request: EntityRequest) -> EntityResponse:
+    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, entity_id: EntityId) -> EntityResponse:
+    async def delete(self, invoice_id: InvoiceId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
+    async def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
-                json=jsonable_encoder(request),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, entity_id: EntityId) -> None:
+    async def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_invoices(
-        self, entity_id: EntityId, *, status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]]
-    ) -> typing.List[InvoiceResponse]:
+    async def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
-                params={"status": status},
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def accept_terms_of_service(self, entity_id: EntityId) -> str:
+    async def edit_comment(
+        self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest
+    ) -> CommentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_token(self, entity_id: EntityId) -> str:
+    async def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def plaid_link_token(self, entity_id: EntityId) -> str:
+    async def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+            )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .entity_id import EntityId
 from .entity_request import EntityRequest
 from .entity_response import EntityResponse
 from .entity_status import EntityStatus
 from .entity_update_request import EntityUpdateRequest
 from .individual_profile_request import IndividualProfileRequest
 from .individual_profile_response import IndividualProfileResponse
+from .invoice_metrics_response import InvoiceMetricsResponse
 from .profile_request import ProfileRequest
 from .profile_response import ProfileResponse
 from .tax_id import TaxID
 
 __all__ = [
     "AccountType",
     "BusinessProfileRequest",
@@ -25,11 +26,12 @@
     "EntityId",
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
+    "InvoiceMetricsResponse",
     "ProfileRequest",
     "ProfileResponse",
     "TaxID",
 ]
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 
 class EntityRequest(pydantic.BaseModel):
     foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
     email_to: typing.Optional[str] = pydantic.Field(
         alias="emailTo", description=("Email inbox address. Do not inclue the @domain.com\n")
     )
+    email_to_alias: typing.Optional[typing.List[str]] = pydantic.Field(
+        alias="emailToAlias",
+        description=(
+            "Email inbox alias addresses. Used when forwarding emails to the emailTo address from an alias. Include the full email address.\n"
+        ),
+    )
     owned_by_org: typing.Optional[bool] = pydantic.Field(alias="ownedByOrg")
     account_type: AccountType = pydantic.Field(alias="accountType")
     profile: ProfileRequest
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .profile_response import ProfileResponse
 
 
 class EntityResponse(pydantic.BaseModel):
     id: EntityId
     foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
     email_to: typing.Optional[str] = pydantic.Field(alias="emailTo")
+    email_to_alias: typing.Optional[typing.List[str]] = pydantic.Field(alias="emailToAlias")
     owned_by_org: bool = pydantic.Field(alias="ownedByOrg")
     account_type: AccountType = pydantic.Field(alias="accountType")
     name: str
     email: str
     profile: ProfileResponse
     status: EntityStatus
     accepted_tos: bool = pydantic.Field(alias="acceptedTos")
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .account_type import AccountType
-from .profile_request import ProfileRequest
+from .bank_account_id import BankAccountId
+from .bank_type import BankType
 
 
-class EntityUpdateRequest(pydantic.BaseModel):
-    foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
-    email_to: typing.Optional[str] = pydantic.Field(
-        alias="emailTo", description=("Email inbox address. Do not inclue the @domain.com\n")
+class BankAccountRequest(pydantic.BaseModel):
+    id: typing.Optional[BankAccountId]
+    bank_name: str = pydantic.Field(alias="bankName")
+    routing_number: str = pydantic.Field(alias="routingNumber")
+    account_number: str = pydantic.Field(alias="accountNumber")
+    plaid_public_token: typing.Optional[str] = pydantic.Field(
+        alias="plaidPublicToken", description=("Public token from Plaid Link\n")
     )
-    owned_by_org: typing.Optional[bool] = pydantic.Field(alias="ownedByOrg")
-    account_type: typing.Optional[AccountType] = pydantic.Field(alias="accountType")
-    profile: typing.Optional[ProfileRequest]
+    account_type: BankType = pydantic.Field(alias="accountType")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity_users/client.py` & `mercoa-0.0.8/src/mercoa/resources/entity_users/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_request.py` & `mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/entity_users/types/entity_user_response.py` & `mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     CommentId,
     CommentRequest,
     CommentResponse,
     CreateVendorRequest,
+    CurrencyCode,
     DocumentResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
-    TransactionResponse,
-    TransactionStatus,
 )
 
 __all__ = [
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "CreateVendorRequest",
+    "CurrencyCode",
     "DocumentResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
-    "TransactionResponse",
-    "TransactionStatus",
 ]
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/client.py` & `mercoa-0.0.8/src/mercoa/resources/entity/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,409 +1,457 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import datetime as dt
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
+from ...core.datetime_utils import serialize_datetime
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from .types.comment_id import CommentId
-from .types.comment_request import CommentRequest
-from .types.comment_response import CommentResponse
-from .types.document_response import DocumentResponse
-from .types.invoice_id import InvoiceId
-from .types.invoice_request import InvoiceRequest
-from .types.invoice_response import InvoiceResponse
+from ..invoice.types.currency_code import CurrencyCode
+from ..invoice.types.invoice_response import InvoiceResponse
+from ..invoice.types.invoice_status import InvoiceStatus
+from .types.entity_id import EntityId
+from .types.entity_request import EntityRequest
+from .types.entity_response import EntityResponse
+from .types.entity_status import EntityStatus
+from .types.entity_update_request import EntityUpdateRequest
+from .types.invoice_metrics_response import InvoiceMetricsResponse
 
 
-class InvoiceClient:
+class EntityClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
+    def get_all(self) -> typing.List[EntityResponse]:
         _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
-            json=jsonable_encoder(request),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+    def find(
+        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
+    ) -> typing.List[EntityResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
+            params={"foreignId": foreign_id, "status": status},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    def create(self, *, request: EntityRequest) -> EntityResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, invoice_id: InvoiceId) -> None:
+    def get(self, entity_id: EntityId) -> EntityResponse:
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
+    def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
+    def delete(self, entity_id: EntityId) -> None:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
+    def get_invoices(
+        self, entity_id: EntityId, *, status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]]
+    ) -> typing.List[InvoiceResponse]:
         _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
-            json=jsonable_encoder(request),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
+            params={"status": status},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def edit_comment(self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest) -> CommentResponse:
+    def get_invoice_metrics(
+        self,
+        entity_id: EntityId,
+        *,
+        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
+        due_date_start: typing.Optional[dt.datetime] = None,
+        due_date_end: typing.Optional[dt.datetime] = None,
+        created_date_start: typing.Optional[dt.datetime] = None,
+        created_date_end: typing.Optional[dt.datetime] = None,
+        currency: CurrencyCode,
+    ) -> InvoiceMetricsResponse:
         _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
-            json=jsonable_encoder(request),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
+            params={
+                "status": status,
+                "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
+                "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
+                "createdDateStart": serialize_datetime(created_date_start) if created_date_start is not None else None,
+                "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
+                "currency": currency,
+            },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceMetricsResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
+    def accept_terms_of_service(self, entity_id: EntityId) -> str:
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_vendor_link(self, invoice_id: InvoiceId) -> str:
+    def get_token(self, entity_id: EntityId) -> str:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+    def plaid_link_token(self, entity_id: EntityId) -> str:
         _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncInvoiceClient:
+class AsyncEntityClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
+    async def get_all(self) -> typing.List[EntityResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
-                json=jsonable_encoder(request),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
+    async def find(
+        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
+    ) -> typing.List[EntityResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
+                params={"foreignId": foreign_id, "status": status},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
+    async def create(self, *, request: EntityRequest) -> EntityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, invoice_id: InvoiceId) -> None:
+    async def get(self, entity_id: EntityId) -> EntityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
+    async def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
+    async def delete(self, entity_id: EntityId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
+    async def get_invoices(
+        self, entity_id: EntityId, *, status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]]
+    ) -> typing.List[InvoiceResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
-                json=jsonable_encoder(request),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
+                params={"status": status},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def edit_comment(
-        self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest
-    ) -> CommentResponse:
+    async def get_invoice_metrics(
+        self,
+        entity_id: EntityId,
+        *,
+        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
+        due_date_start: typing.Optional[dt.datetime] = None,
+        due_date_end: typing.Optional[dt.datetime] = None,
+        created_date_start: typing.Optional[dt.datetime] = None,
+        created_date_end: typing.Optional[dt.datetime] = None,
+        currency: CurrencyCode,
+    ) -> InvoiceMetricsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
-                json=jsonable_encoder(request),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
+                params={
+                    "status": status,
+                    "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
+                    "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
+                    "createdDateStart": serialize_datetime(created_date_start)
+                    if created_date_start is not None
+                    else None,
+                    "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
+                    "currency": currency,
+                },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceMetricsResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
+    async def accept_terms_of_service(self, entity_id: EntityId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_vendor_link(self, invoice_id: InvoiceId) -> str:
+    async def get_token(self, entity_id: EntityId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+    async def plaid_link_token(self, entity_id: EntityId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .comment_id import CommentId
 from .comment_request import CommentRequest
 from .comment_response import CommentResponse
 from .create_vendor_request import CreateVendorRequest
+from .currency_code import CurrencyCode
 from .document_response import DocumentResponse
 from .invoice_id import InvoiceId
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_request import InvoiceRequest
 from .invoice_response import InvoiceResponse
 from .invoice_status import InvoiceStatus
-from .transaction_response import TransactionResponse
-from .transaction_status import TransactionStatus
 
 __all__ = [
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "CreateVendorRequest",
+    "CurrencyCode",
     "DocumentResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
-    "TransactionResponse",
-    "TransactionStatus",
 ]
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_request.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/comment_response.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/create_vendor_request.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/create_vendor_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/document_response.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_request.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .currency_code import CurrencyCode
 
 
 class InvoiceLineItemRequest(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(
         description=(
             "If provided, will overwrite line item on the invoice with this ID. If not provided, will create a new line item.\n"
         )
     )
     amount: typing.Optional[float]
-    currency: typing.Optional[str]
+    currency: typing.Optional[CurrencyCode]
     description: typing.Optional[str]
     name: typing.Optional[str]
     quantity: typing.Optional[int]
     unit_price: typing.Optional[float] = pydantic.Field(alias="unitPrice")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_line_item_response.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .currency_code import CurrencyCode
 
 
 class InvoiceLineItemResponse(pydantic.BaseModel):
     id: str
     amount: typing.Optional[float]
-    currency: typing.Optional[str]
+    currency: typing.Optional[CurrencyCode]
     description: typing.Optional[str]
     name: typing.Optional[str]
     quantity: typing.Optional[int]
     unit_price: typing.Optional[float] = pydantic.Field(alias="unitPrice")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_id import EntityId
 from ...payment_method.types.payment_method_id import PaymentMethodId
 from .create_vendor_request import CreateVendorRequest
+from .currency_code import CurrencyCode
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceRequest(pydantic.BaseModel):
     status: typing.Optional[InvoiceStatus]
     amount: typing.Optional[float]
-    currency: typing.Optional[str]
+    currency: typing.Optional[CurrencyCode]
     deduction_date: typing.Optional[dt.datetime] = pydantic.Field(
         alias="deductionDate", description=("Date when funds will be deducted from payer's account.\n")
     )
     funded_date: typing.Optional[dt.datetime] = pydantic.Field(
         alias="fundedDate", description=("Date of funds settlement.\n")
     )
     due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate", description=("Due date of invoice.\n"))
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_id import EntityId
 from ...entity.types.entity_response import EntityResponse
 from ...payment_method.types.payment_method_id import PaymentMethodId
 from ...payment_method.types.payment_method_response import PaymentMethodResponse
+from ...transaction.types.transaction_response import TransactionResponse
+from .currency_code import CurrencyCode
 from .invoice_id import InvoiceId
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_status import InvoiceStatus
-from .transaction_response import TransactionResponse
 
 
 class InvoiceResponse(pydantic.BaseModel):
     id: InvoiceId
     status: InvoiceStatus
     amount: typing.Optional[float]
-    currency: typing.Optional[str]
+    currency: typing.Optional[CurrencyCode]
     deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
     funded_date: typing.Optional[dt.datetime] = pydantic.Field(alias="fundedDate")
     due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
     service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
     service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_response.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .transaction_status import TransactionStatus
+from .email_sender_provider import EmailSenderProvider
 
 
-class TransactionResponse(pydantic.BaseModel):
-    id: str
-    status: TransactionStatus
-    amount: float
-    currency: typing.Optional[str]
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+class EmailSenderResponse(pydantic.BaseModel):
+    provider: EmailSenderProvider
+    from_email: str = pydantic.Field(alias="fromEmail")
+    from_name: str = pydantic.Field(alias="fromName")
+    has_api_key: bool = pydantic.Field(alias="hasApiKey")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/invoice/types/transaction_status.py` & `mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/ocr/client.py` & `mercoa-0.0.8/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/ocr/types/attachments.py` & `mercoa-0.0.8/src/mercoa/resources/ocr/types/attachments.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/ocr/types/email_ocr_request.py` & `mercoa-0.0.8/src/mercoa/resources/ocr/types/email_ocr_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_mailbox.py` & `mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_mailbox.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/client.py` & `mercoa-0.0.8/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_provider import EmailSenderProvider
+from .card_brand import CardBrand
+from .card_id import CardId
+from .card_type import CardType
 
 
-class EmailSenderResponse(pydantic.BaseModel):
-    provider: EmailSenderProvider
-    from_email: str = pydantic.Field(alias="fromEmail")
-    from_name: str = pydantic.Field(alias="fromName")
-    has_api_key: bool = pydantic.Field(alias="hasApiKey")
+class CardRequest(pydantic.BaseModel):
+    id: typing.Optional[CardId]
+    type: CardType
+    brand: CardBrand
+    last_four: str = pydantic.Field(alias="lastFour")
+    exp_month: str = pydantic.Field(alias="expMonth")
+    exp_year: str = pydantic.Field(alias="expYear")
+    token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method.types.payment_method_type import PaymentMethodType
-from .payment_rail_markup import PaymentRailMarkup
+from .payment_method_schema_field import PaymentMethodSchemaField
 
 
-class PaymentRailRequest(pydantic.BaseModel):
-    type: PaymentMethodType
+class PaymentMethodSchemaRequest(pydantic.BaseModel):
     name: str
-    markup: typing.Optional[PaymentRailMarkup]
-    description: typing.Optional[str]
-    active: bool
+    is_source: bool = pydantic.Field(
+        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
+    )
+    is_destination: bool = pydantic.Field(
+        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
+    )
+    fields: typing.List[PaymentMethodSchemaField]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/client.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.0.8/src/mercoa/resources/representative/types/representative_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .bank_account_id import BankAccountId
-from .bank_type import BankType
-
-
-class BankAccountRequest(pydantic.BaseModel):
-    id: typing.Optional[BankAccountId]
-    bank_name: str = pydantic.Field(alias="bankName")
-    routing_number: str = pydantic.Field(alias="routingNumber")
-    account_number: str = pydantic.Field(alias="accountNumber")
-    plaid_public_token: typing.Optional[str] = pydantic.Field(
-        alias="plaidPublicToken", description=("Public token from Plaid Link\n")
-    )
-    account_type: BankType = pydantic.Field(alias="accountType")
+from ...commons.types.address import Address
+from ...commons.types.full_name import FullName
+from ...commons.types.phone_number import PhoneNumber
+from .representative_id import RepresentativeId
+from .responsibilities import Responsibilities
+
+
+class RepresentativeResponse(pydantic.BaseModel):
+    id: RepresentativeId
+    name: FullName
+    phone: PhoneNumber
+    email: str
+    address: Address
+    birth_date_provided: bool = pydantic.Field(alias="birthDateProvided")
+    government_id_provided: bool = pydantic.Field(alias="governmentIDProvided")
+    responsibilities: Responsibilities
+    created_on: dt.datetime = pydantic.Field(alias="createdOn")
+    updated_on: dt.datetime = pydantic.Field(alias="updatedOn")
+    disabled_on: typing.Optional[dt.datetime] = pydantic.Field(alias="disabledOn")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 from ....core.datetime_utils import serialize_datetime
 from .card_brand import CardBrand
 from .card_id import CardId
 from .card_type import CardType
 
 
-class CardRequest(pydantic.BaseModel):
-    id: typing.Optional[CardId]
+class CardResponse(pydantic.BaseModel):
+    id: CardId
     type: CardType
     brand: CardBrand
     last_four: str = pydantic.Field(alias="lastFour")
     exp_month: str = pydantic.Field(alias="expMonth")
     exp_year: str = pydantic.Field(alias="expYear")
-    token: str
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.0.8/src/mercoa/resources/representative/types/responsibilities.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,28 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .card_brand import CardBrand
-from .card_id import CardId
-from .card_type import CardType
 
 
-class CardResponse(pydantic.BaseModel):
-    id: CardId
-    type: CardType
-    brand: CardBrand
-    last_four: str = pydantic.Field(alias="lastFour")
-    exp_month: str = pydantic.Field(alias="expMonth")
-    exp_year: str = pydantic.Field(alias="expYear")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+class Responsibilities(pydantic.BaseModel):
+    job_title: typing.Optional[str] = pydantic.Field(alias="jobTitle")
+    is_controller: typing.Optional[bool] = pydantic.Field(alias="isController")
+    is_owner: typing.Optional[bool] = pydantic.Field(alias="isOwner")
+    ownership_percentage: typing.Optional[float] = pydantic.Field(alias="ownershipPercentage")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,30 @@
 class PaymentMethodSchemaClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
+    def get_all(self) -> typing.List[PaymentMethodSchemaResponse]:
+        _response = httpx.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.List[PaymentMethodSchemaResponse], _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def create(self, *, request: PaymentMethodSchemaRequest) -> PaymentMethodSchemaResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
@@ -76,14 +92,31 @@
 class AsyncPaymentMethodSchemaClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
+    async def get_all(self) -> typing.List[PaymentMethodSchemaResponse]:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.List[PaymentMethodSchemaResponse], _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def create(self, *, request: PaymentMethodSchemaRequest) -> PaymentMethodSchemaResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "paymentMethod/schema"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/__init__.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_method_schema_field_type import PaymentMethodSchemaFieldType
+from .payment_method_schema_field import PaymentMethodSchemaField
+from .payment_method_schema_id import PaymentMethodSchemaId
 
 
-class PaymentMethodSchemaField(pydantic.BaseModel):
+class PaymentMethodSchemaResponse(pydantic.BaseModel):
+    id: PaymentMethodSchemaId
     name: str
-    display_name: typing.Optional[str] = pydantic.Field(alias="displayName")
-    type: PaymentMethodSchemaFieldType
-    optional: bool
-    options: typing.Optional[str] = pydantic.Field(
-        description=("When type is 'select', provide options that can be selected\n")
+    is_source: bool = pydantic.Field(
+        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
     )
+    is_destination: bool = pydantic.Field(
+        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
+    )
+    fields: typing.List[PaymentMethodSchemaField]
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_method_schema_field import PaymentMethodSchemaField
+from ...invoice.types.currency_code import CurrencyCode
+from .transaction_status import TransactionStatus
 
 
-class PaymentMethodSchemaRequest(pydantic.BaseModel):
-    name: str
-    is_source: bool = pydantic.Field(
-        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
-    )
-    is_destination: bool = pydantic.Field(
-        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
-    )
-    fields: typing.List[PaymentMethodSchemaField]
+class TransactionResponse(pydantic.BaseModel):
+    id: str
+    status: TransactionStatus
+    amount: float
+    currency: typing.Optional[CurrencyCode]
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py` & `mercoa-0.0.8/src/mercoa/resources/representative/types/representative_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_method_schema_field import PaymentMethodSchemaField
-from .payment_method_schema_id import PaymentMethodSchemaId
-
-
-class PaymentMethodSchemaResponse(pydantic.BaseModel):
-    id: PaymentMethodSchemaId
-    name: str
-    is_source: bool = pydantic.Field(
-        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
-    )
-    is_destination: bool = pydantic.Field(
-        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
-    )
-    fields: typing.List[PaymentMethodSchemaField]
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+from ...commons.types.address import Address
+from ...commons.types.birth_date import BirthDate
+from ...commons.types.full_name import FullName
+from ...commons.types.individual_government_id import IndividualGovernmentID
+from ...commons.types.phone_number import PhoneNumber
+from .responsibilities import Responsibilities
+
+
+class RepresentativeRequest(pydantic.BaseModel):
+    name: FullName
+    phone: PhoneNumber
+    email: str
+    address: Address
+    birth_date: BirthDate = pydantic.Field(alias="birthDate")
+    government_id: IndividualGovernmentID = pydantic.Field(alias="governmentID")
+    responsibilities: Responsibilities
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/representative/client.py` & `mercoa-0.0.8/src/mercoa/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.7/src/mercoa/resources/representative/types/representative_request.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_update_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.address import Address
-from ...commons.types.birth_date import BirthDate
-from ...commons.types.full_name import FullName
-from ...commons.types.individual_government_id import IndividualGovernmentID
-from ...commons.types.phone_number import PhoneNumber
-from .responsibilities import Responsibilities
-
-
-class RepresentativeRequest(pydantic.BaseModel):
-    name: FullName
-    phone: PhoneNumber
-    email: str
-    address: Address
-    birth_date: BirthDate = pydantic.Field(alias="birthDate")
-    government_id: IndividualGovernmentID = pydantic.Field(alias="governmentID")
-    responsibilities: Responsibilities
+from .account_type import AccountType
+from .profile_request import ProfileRequest
+
+
+class EntityUpdateRequest(pydantic.BaseModel):
+    foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
+    email_to: typing.Optional[str] = pydantic.Field(
+        alias="emailTo", description=("Email inbox address. Do not inclue the @domain.com\n")
+    )
+    email_to_alias: typing.Optional[typing.List[str]] = pydantic.Field(
+        alias="emailToAlias",
+        description=(
+            "Email inbox alias addresses. Used when forwarding emails to the emailTo address from an alias. Include the full email address.\n"
+        ),
+    )
+    owned_by_org: typing.Optional[bool] = pydantic.Field(alias="ownedByOrg")
+    account_type: typing.Optional[AccountType] = pydantic.Field(alias="accountType")
+    profile: typing.Optional[ProfileRequest]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/src/mercoa/resources/representative/types/representative_response.py` & `mercoa-0.0.8/src/mercoa/resources/entity/types/invoice_metrics_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,33 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.address import Address
-from ...commons.types.full_name import FullName
-from ...commons.types.phone_number import PhoneNumber
-from .representative_id import RepresentativeId
-from .responsibilities import Responsibilities
-
-
-class RepresentativeResponse(pydantic.BaseModel):
-    id: RepresentativeId
-    name: FullName
-    phone: PhoneNumber
-    email: str
-    address: Address
-    birth_date_provided: bool = pydantic.Field(alias="birthDateProvided")
-    government_id_provided: bool = pydantic.Field(alias="governmentIDProvided")
-    responsibilities: Responsibilities
-    created_on: dt.datetime = pydantic.Field(alias="createdOn")
-    updated_on: dt.datetime = pydantic.Field(alias="updatedOn")
-    disabled_on: typing.Optional[dt.datetime] = pydantic.Field(alias="disabledOn")
+from ...invoice.types.currency_code import CurrencyCode
+
+
+class InvoiceMetricsResponse(pydantic.BaseModel):
+    total_amount: float = pydantic.Field(alias="totalAmount")
+    total_count: int = pydantic.Field(alias="totalCount")
+    average_amount: float = pydantic.Field(alias="averageAmount")
+    currency: CurrencyCode
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.7/PKG-INFO` & `mercoa-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

