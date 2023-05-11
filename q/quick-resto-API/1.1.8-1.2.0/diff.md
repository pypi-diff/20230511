# Comparing `tmp/quick_resto_API-1.1.8.tar.gz` & `tmp/quick_resto_API-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_resto_API-1.1.8.tar", last modified: Tue May  2 14:36:18 2023, max compression
+gzip compressed data, was "quick_resto_API-1.2.0.tar", last modified: Wed May 10 14:39:59 2023, max compression
```

## Comparing `quick_resto_API-1.1.8.tar` & `quick_resto_API-1.2.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      219 2023-05-02 14:35:20.000000 quick_resto_API-1.1.8/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.591298 quick_resto_API-1.1.8/quick_resto_API/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5150 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.593298 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.601298 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4403 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/account_type_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4600 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4464 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4431 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4296 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/business_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cancellation_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4393 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/company_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4512 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4455 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4388 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4716 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4512 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5626 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/dish_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4297 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/employee_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4356 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/encashment_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4464 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4168 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/hall_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4612 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5869 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4225 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/markup_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4411 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5832 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/modifier_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4658 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4328 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4411 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4412 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/payment_type_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5869 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7934 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/providers_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4605 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4353 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/sale_place_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4600 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5933 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/semi_product_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4188 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/shift_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6047 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/single_product_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4453 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4194 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4202 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4403 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4294 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4444 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4320 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/operations_with_objects.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       25 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/system_object.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2947 2022-08-29 08:42:46.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4045 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_interface.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.601298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.590298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.602298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1432 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1139 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.603298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2082 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/business.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2043 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/company_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2335 2022-08-08 09:56:10.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1084 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1523 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4413 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment_types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      554 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.605298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      922 2023-04-03 12:13:12.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1050 2023-04-03 12:13:17.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_type.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3641 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1109 2023-04-03 12:13:08.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3911 2023-04-03 12:35:57.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2023-04-03 12:13:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1974 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1091 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4490 2022-08-29 09:39:40.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/markup.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3599 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.608298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3912 2022-08-29 07:33:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/cancellation.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      944 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/device_command.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/encashment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1150 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/hall.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1837 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8027 2023-04-28 14:05:39.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4908 2023-02-09 11:42:24.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_item.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3107 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2661 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2285 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7697 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/shift.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2502 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2060 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3783 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4101 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1851 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3121 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.608298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1478 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/employee.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/user.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.614297 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1267 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2128 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2146 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2792 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1492 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4215 2022-10-23 12:12:25.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2810 2022-09-07 13:17:38.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1069 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      678 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2008 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2708 2022-12-15 17:43:37.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2223 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4389 2023-02-09 11:48:16.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2565 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1271 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1264 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2137 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      802 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4986 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3366 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1819 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3241 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1097 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1815 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      393 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/right.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      557 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/right_link.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1447 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/role.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2090 2022-09-01 15:28:18.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/quick_resto_object.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      735 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/styler.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.592298 quick_resto_API-1.1.8/quick_resto_API.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8520 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       16 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      950 2023-05-02 14:36:05.000000 quick_resto_API-1.1.8/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.161838 quick_resto_API-1.2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-10 14:39:59.160838 quick_resto_API-1.2.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      219 2023-05-02 14:35:20.000000 quick_resto_API-1.2.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.133839 quick_resto_API-1.2.0/quick_resto_API/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5150 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.135839 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.148838 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4595 2023-05-10 14:17:46.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/account_type_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4792 2023-05-10 14:18:31.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4656 2023-05-10 14:19:00.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4623 2023-05-10 14:19:53.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4488 2023-05-10 14:20:24.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/business_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4621 2023-05-10 14:21:05.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/cancellation_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4585 2023-05-10 14:20:45.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/company_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4704 2023-05-10 14:21:48.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4647 2023-05-10 14:22:04.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4580 2023-05-10 14:22:23.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4882 2023-05-10 14:22:55.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4704 2023-05-10 14:23:08.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5817 2023-05-02 15:36:47.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/dish_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4488 2023-05-10 14:23:32.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/employee_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4548 2023-05-10 14:27:48.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/encashment_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-10 14:27:54.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4656 2023-05-10 14:27:59.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4360 2023-05-10 14:28:03.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/hall_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-10 14:28:07.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4804 2023-05-10 14:28:26.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6061 2023-05-10 14:28:30.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4417 2023-05-10 14:28:34.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/markup_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4603 2023-05-10 14:28:41.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6024 2023-05-10 14:28:45.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/modifier_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4850 2023-05-10 14:28:37.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4520 2023-05-10 14:27:44.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/order_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-10 14:28:48.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4603 2023-05-10 14:33:00.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4604 2023-05-10 14:33:06.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/payment_type_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6061 2023-05-10 14:33:12.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4622 2023-05-10 14:34:14.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4806 2023-05-10 14:34:09.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8126 2023-05-10 14:34:05.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/providers_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4797 2023-05-10 14:34:00.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4545 2023-05-10 14:33:57.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/sale_place_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4792 2023-05-10 14:33:54.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6125 2023-05-10 14:33:50.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/semi_product_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4380 2023-05-10 14:33:46.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/shift_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6239 2023-05-10 14:33:42.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/single_product_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4645 2023-05-10 14:33:39.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4386 2023-05-10 14:33:35.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/store_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4394 2023-05-10 14:33:32.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/table_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4595 2023-05-10 14:33:29.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4486 2023-05-10 14:33:24.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4636 2023-05-10 14:33:19.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4581 2023-05-10 13:25:58.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/operations_with_objects.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       25 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/system_object.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2947 2023-05-10 13:24:23.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4045 2022-07-25 09:16:26.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_interface.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.149838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.133839 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.149838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/alcohol/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1432 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1139 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.150838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2082 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/business.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2043 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/company_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2335 2022-08-08 09:56:10.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1084 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1523 2022-07-25 09:16:26.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/payment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4413 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/payment_types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      554 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.151838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      922 2023-04-03 12:13:12.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1050 2023-04-03 12:13:17.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/account_type.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3641 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1109 2023-04-03 12:13:08.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3911 2023-04-03 12:35:57.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/customer.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2023-04-03 12:13:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1974 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1091 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4490 2022-08-29 09:39:40.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/markup.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3599 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.154838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3912 2022-08-29 07:33:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/cancellation.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      944 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/device_command.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/encashment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1150 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/hall.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1837 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8027 2023-04-28 14:05:39.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/order_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4908 2023-02-09 11:42:24.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/order_item.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3107 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2661 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2285 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7697 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/shift.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2502 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2060 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3783 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4101 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1851 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3121 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.154838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/personnel/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1478 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/personnel/employee.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/personnel/user.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.159838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1267 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2128 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2146 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2792 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1492 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4215 2023-05-10 13:10:59.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2810 2023-05-10 13:46:52.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1069 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      678 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2008 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2708 2022-12-15 17:43:37.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2223 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4389 2023-02-09 11:48:16.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2565 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1271 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1264 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2137 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      802 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4986 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3366 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1819 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3241 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1097 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/store.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1815 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.160838 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/platform/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      393 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/platform/right.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      557 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/platform/right_link.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1447 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/platform/role.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2191 2023-05-10 13:31:30.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/quick_resto_object.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      735 2022-07-15 09:27:22.000000 quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/styler.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-10 14:39:59.134839 quick_resto_API-1.2.0/quick_resto_API.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-10 14:39:59.000000 quick_resto_API-1.2.0/quick_resto_API.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8520 2023-05-10 14:39:59.000000 quick_resto_API-1.2.0/quick_resto_API.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-10 14:39:59.000000 quick_resto_API-1.2.0/quick_resto_API.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       16 2023-05-10 14:39:59.000000 quick_resto_API-1.2.0/quick_resto_API.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-05-10 14:39:59.161838 quick_resto_API-1.2.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      950 2023-05-10 14:38:38.000000 quick_resto_API-1.2.0/setup.py
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/__init__.py` & `quick_resto_API-1.2.0/quick_resto_API/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/account_type_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/account_type_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.crm.account_type import AccountType
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class AccountTypeOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "crm.accounting.account.type"
 
     def get_list_of_account_type(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[AccountType]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[AccountType]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[AccountType] = []
 
         for object in json_response:
             result.append(AccountType(**object))
 
         return result
 
     def get_tree_of_account_type(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[AccountType]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[AccountType]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[AccountType] = list()
 
         for object in json_response:
             result.append(AccountType(**object))
 
         return result
 
     def get_account_type(self, objectId: int, objectRid: int = None) -> AccountType:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return AccountType(**json_response)
 
     def get_account_type_with_subobjects(self, objectId: int, objectRid: int = None) -> AccountType:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return AccountType(**json_response)
 
     def create_account_type(self, object: AccountType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AccountType:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AccountType(**json_response)
 
     def update_account_type(self, object: AccountType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AccountType:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AccountType(**json_response)
 
     def remove_account_type(self, object: AccountType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AccountType:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AccountType(**json_response)
 
     def recover_account_type(self, object: AccountType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AccountType:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AccountType(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.alcohol.alcohol_dictionary import AlcoholDictionary
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class AlcoholDictionaryOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "alcohol.dictionary"
 
     def get_list_of_alcohol_dictionary(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[AlcoholDictionary]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[AlcoholDictionary]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[AlcoholDictionary] = list()
 
         for object in json_response:
             result.append(AlcoholDictionary(**object))
 
         return result
 
     def get_tree_of_alcohol_dictionary(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[AlcoholDictionary]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[AlcoholDictionary]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[AlcoholDictionary] = list()
 
         for object in json_response:
             result.append(AlcoholDictionary(**object))
 
         return result
 
     def get_alcohol_dictionary(self, objectId: int, objectRid: int = None) -> AlcoholDictionary:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return AlcoholDictionary(**json_response)
 
     def get_alcohol_dictionary_with_subobjects(self, objectId: int, objectRid: int = None) -> AlcoholDictionary:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return AlcoholDictionary(**json_response)
 
     def create_alcohol_dictionary(self, object: AlcoholDictionary,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholDictionary:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholDictionary(**json_response)
 
     def update_alcohol_dictionary(self, object: AlcoholDictionary,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholDictionary:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholDictionary(**json_response)
 
     def remove_alcohol_dictionary(self, object: AlcoholDictionary,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholDictionary:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholDictionary(**json_response)
 
     def recover_alcohol_dictionary(self, object: AlcoholDictionary,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholDictionary:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholDictionary(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.alcohol.alcohol_report import AlcoholReport
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class AlcoholReportOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "alcohol.report"
 
     def get_list_of_alcohol_report(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[AlcoholReport]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[AlcoholReport]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[AlcoholReport] = list()
 
         for object in json_response:
             result.append(AlcoholReport(**object))
 
         return result
 
     def get_tree_of_alcohol_report(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[AlcoholReport]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[AlcoholReport]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[AlcoholReport] = list()
 
         for object in json_response:
             result.append(AlcoholReport(**object))
 
         return result
 
     def get_alcohol_report(self, objectId: int, objectRid: int = None) -> AlcoholReport:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return AlcoholReport(**json_response)
 
     def get_alcohol_report_with_subobjects(self, objectId: int, objectRid: int = None) -> AlcoholReport:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return AlcoholReport(**json_response)
 
     def create_alcohol_report(self, object: AlcoholReport,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholReport:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholReport(**json_response)
 
     def update_alcohol_report(self, object: AlcoholReport,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholReport:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholReport(**json_response)
 
     def remove_alcohol_report(self, object: AlcoholReport,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholReport:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholReport(**json_response)
 
     def recover_alcohol_report(self, object: AlcoholReport,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> AlcoholReport:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return AlcoholReport(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.crm.bonus_program import BonusProgram
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class BonusProgramOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "crm.settings.bonus"
 
     def get_list_of_bonus_program(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[BonusProgram]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[BonusProgram]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[BonusProgram] = list()
 
         for object in json_response:
             result.append(BonusProgram(**object))
 
         return result
 
     def get_tree_of_bonus_program(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[BonusProgram]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[BonusProgram]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[BonusProgram] = list()
 
         for object in json_response:
             result.append(BonusProgram(**object))
 
         return result
 
     def get_bonus_program(self, objectId: int, objectRid: int = None) -> BonusProgram:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return BonusProgram(**json_response)
 
     def get_bonus_program_with_subobjects(self, objectId: int, objectRid: int = None) -> BonusProgram:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return BonusProgram(**json_response)
 
     def create_bonus_program(self, object: BonusProgram,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> BonusProgram:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return BonusProgram(**json_response)
 
     def update_bonus_program(self, object: BonusProgram,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> BonusProgram:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return BonusProgram(**json_response)
 
     def remove_bonus_program(self, object: BonusProgram,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> BonusProgram:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return BonusProgram(**json_response)
 
     def recover_bonus_program(self, object: BonusProgram,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> BonusProgram:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return BonusProgram(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/business_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/business_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.core.business import Business
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class BusinessOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "core.company.businesses"
 
     def get_list_of_business(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Business]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Business]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Business] = list()
 
         for object in json_response:
             result.append(Business(**object))
 
         return result
 
     def get_tree_of_business(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Business]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Business]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Business] = list()
 
         for object in json_response:
             result.append(Business(**object))
 
         return result
 
     def get_business(self, objectId: int, objectRid: int = None) -> Business:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return Business(**json_response)
 
     def get_business_with_subobjects(self, objectId: int, objectRid: int = None) -> Business:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return Business(**json_response)
 
     def create_business(self, object: Business,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Business:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Business(**json_response)
 
     def update_business(self, object: Business,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Business:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Business(**json_response)
 
     def remove_business(self, object: Business,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Business:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Business(**json_response)
 
     def recover_business(self, object: Business,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Business:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Business(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cancellation_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/cancellation_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.cancellation import Cancellation
-
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class CancellationOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.cancellations"
 
     def get_list_of_cancellations(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Cancellation]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Cancellation]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Cancellation] = list()
 
         for object in json_response:
             result.append(Cancellation(**object))
 
         return result
 
     def get_tree_of_cancellations(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Cancellation]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Cancellation]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Cancellation] = list()
 
         for object in json_response:
             result.append(Cancellation(**object))
 
         return result
 
     def get_cancellations(self, objectId: int, objectRid: int = None) -> Cancellation:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return Cancellation(**json_response)
 
     def get_cancellations_with_subobjects(self, objectId: int, objectRid: int = None) -> Cancellation:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return Cancellation(**json_response)
 
     def create_cancellation(self, object: Cancellation,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Cancellation:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Cancellation(**json_response)
 
     def update_cancellation(self, object: Cancellation,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Cancellation:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Cancellation(**json_response)
 
     def remove_cancellation(self, object: Cancellation,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Cancellation:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Cancellation(**json_response)
 
     def recover_cancellation(self, object: Cancellation,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Cancellation:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Cancellation(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/company_info_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/company_info_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.core.company_info import CompanyInfo
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class CompanyInfoOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "core.company"
 
     def get_list_of_company_info(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CompanyInfo]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CompanyInfo]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CompanyInfo] = list()
 
         for object in json_response:
             result.append(CompanyInfo(**object))
 
         return result
 
     def get_tree_of_company_info(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CompanyInfo]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CompanyInfo]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CompanyInfo] = list()
 
         for object in json_response:
             result.append(CompanyInfo(**object))
 
         return result
 
     def get_company_info(self, objectId: int, objectRid: int = None) -> CompanyInfo:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return CompanyInfo(**json_response)
 
     def get_company_info_with_subobjects(self, objectId: int, objectRid: int = None) -> CompanyInfo:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return CompanyInfo(**json_response)
 
     def create_company_info(self, object: CompanyInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CompanyInfo:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CompanyInfo(**json_response)
 
     def update_company_info(self, object: CompanyInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CompanyInfo:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CompanyInfo(**json_response)
 
     def remove_company_info(self, object: CompanyInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CompanyInfo:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CompanyInfo(**json_response)
 
     def recover_company_info(self, object: CompanyInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CompanyInfo:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CompanyInfo(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.cooking_invoice import CookingInvoice
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class CookingInvoiceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.documents.cooking"
 
     def get_list_of_cooking_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CookingInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CookingInvoice]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CookingInvoice] = list()
 
         for object in json_response:
             result.append(CookingInvoice(**object))
 
         return result
 
     def get_tree_of_cooking_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CookingInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CookingInvoice]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CookingInvoice] = list()
 
         for object in json_response:
             result.append(CookingInvoice(**object))
 
         return result
 
     def get_cooking_invoice(self, objectId: int, objectRid: int = None) -> CookingInvoice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return CookingInvoice(**json_response)
 
     def get_cooking_invoice_with_subobjects(self, objectId: int, objectRid: int = None) -> CookingInvoice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return CookingInvoice(**json_response)
 
     def create_cooking_invoice(self, object: CookingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingInvoice:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingInvoice(**json_response)
 
     def update_cooking_invoice(self, object: CookingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingInvoice:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingInvoice(**json_response)
 
     def remove_cooking_invoice(self, object: CookingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingInvoice:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingInvoice(**json_response)
 
     def recover_cooking_invoice(self, object: CookingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingInvoice:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingInvoice(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.cooking_place import CookingPlace
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class CookingPlaceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.nomenclature.cooking_place"
 
     def get_list_of_cooking_place(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CookingPlace]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CookingPlace]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CookingPlace] = list()
 
         for object in json_response:
             result.append(CookingPlace(**object))
 
         return result
 
     def get_tree_of_cooking_place(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CookingPlace]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CookingPlace]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CookingPlace] = list()
 
         for object in json_response:
             result.append(CookingPlace(**object))
 
         return result
 
     def get_cooking_place(self, objectId: int, objectRid: int = None) -> CookingPlace:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return CookingPlace(**json_response)
 
     def get_cooking_place_with_subobjects(self, objectId: int, objectRid: int = None) -> CookingPlace:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return CookingPlace(**json_response)
 
     def create_cooking_place(self, object: CookingPlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingPlace:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingPlace(**json_response)
 
     def update_cooking_place(self, object: CookingPlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingPlace:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingPlace(**json_response)
 
     def remove_cooking_place(self, object: CookingPlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingPlace:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingPlace(**json_response)
 
     def recover_cooking_place(self, object: CookingPlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CookingPlace:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CookingPlace(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.crm.customer import CrmCustomer
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class CrmCustomerOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "crm.customer"
 
     def get_list_of_crm_customer(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CrmCustomer]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CrmCustomer]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CrmCustomer] = list()
 
         for object in json_response:
             result.append(CrmCustomer(**object))
 
         return result
 
     def get_tree_of_crm_customer(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[CrmCustomer]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[CrmCustomer]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[CrmCustomer] = list()
 
         for object in json_response:
             result.append(CrmCustomer(**object))
 
         return result
 
     def get_crm_customer(self, objectId: int, objectRid: int = None) -> CrmCustomer:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return CrmCustomer(**json_response)
 
     def get_crm_customer_with_subobjects(self, objectId: int, objectRid: int = None) -> CrmCustomer:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return CrmCustomer(**json_response)
 
     def create_crm_customer(self, object: CrmCustomer,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CrmCustomer:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CrmCustomer(**json_response)
 
     def update_crm_customer(self, object: CrmCustomer,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CrmCustomer:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CrmCustomer(**json_response)
 
     def remove_crm_customer(self, object: CrmCustomer,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CrmCustomer:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CrmCustomer(**json_response)
 
     def recover_crm_customer(self, object: CrmCustomer,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> CrmCustomer:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return CrmCustomer(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.decomposition_invoice import DecompositionInvoice
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class DecompositionInvoiceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.documents.decomposition"
 
     def get_list_of_decomposition_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[DecompositionInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[DecompositionInvoice]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
+        json_response = self._operations_with_objects.get_list(self._module_name,
                                                               ownerContextId, ownerContextClassName, showDeleted).json()
 
         result:list[DecompositionInvoice] = list()
 
         for object in json_response:
             result.append(DecompositionInvoice(**object))
 
         return result
 
     def get_tree_of_decomposition_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[DecompositionInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[DecompositionInvoice]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
+        json_response = self._operations_with_objects.get_tree(self._module_name,
                                                               ownerContextId, ownerContextClassName, showDeleted).json()
 
         result:list[DecompositionInvoice] = list()
 
         for object in json_response:
             result.append(DecompositionInvoice(**object))
 
         return result
 
     def get_decomposition_invoice(self, objectId: int, objectRid: int = None) -> DecompositionInvoice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return DecompositionInvoice(**json_response)
 
     def get_decomposition_invoice_with_subobjects(self, objectId: int, objectRid: int = None) -> DecompositionInvoice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return DecompositionInvoice(**json_response)
 
     def create_decomposition_invoice(self, object: DecompositionInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DecompositionInvoice:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DecompositionInvoice(**json_response)
 
     def update_decomposition_invoice(self, object: DecompositionInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DecompositionInvoice:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DecompositionInvoice(**json_response)
 
     def remove_decomposition_invoice(self, object: DecompositionInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DecompositionInvoice:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DecompositionInvoice(**json_response)
 
     def recover_decomposition_invoice(self, object: DecompositionInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DecompositionInvoice:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DecompositionInvoice(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.discard_invoice import DiscardInvoice
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class DiscardInvoiceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.documents.discard"
 
     def get_list_of_discard_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[DiscardInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[DiscardInvoice]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[DiscardInvoice] = list()
 
         for object in json_response:
             result.append(DiscardInvoice(**object))
 
         return result
 
     def get_tree_of_discard_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[DiscardInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[DiscardInvoice]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[DiscardInvoice] = list()
 
         for object in json_response:
             result.append(DiscardInvoice(**object))
 
         return result
 
     def get_discard_invoice(self, objectId: int, objectRid: int = None) -> DiscardInvoice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return DiscardInvoice(**json_response)
 
     def get_discard_invoice_with_subobjects(self, objectId: int, objectRid: int = None) -> DiscardInvoice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return DiscardInvoice(**json_response)
 
     def create_discard_invoice(self, object: DiscardInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DiscardInvoice:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DiscardInvoice(**json_response)
 
     def update_discard_invoice(self, object: DiscardInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DiscardInvoice:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DiscardInvoice(**json_response)
 
     def remove_discard_invoice(self, object: DiscardInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DiscardInvoice:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DiscardInvoice(**json_response)
 
     def recover_discard_invoice(self, object: DiscardInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> DiscardInvoice:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return DiscardInvoice(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/dish_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/dish_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.dish import Dish
 from quick_resto_API.quick_resto_objects.modules.warehouse.dish_category import DishCategory
-
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class DishOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.nomenclature.dish"
 
     def get_list_of_dishes(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Dish|DishCategory]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Dish|DishCategory]:
 
-        json_response = self._operations_with_objects.getList(self._module_name, ownerContextId, 
-                                                                    ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name, ownerContextId, 
+                                                                    ownerContextClassName, showDeleted, listRequest).json()
 
         dishes:list[Dish|DishCategory] = list()
 
         for dish in json_response:
             if 'DishCategory' in dish['className']:
                 dishes.append(DishCategory(**dish))
             elif 'Dish' in dish['className']:
                 dishes.append(Dish(**dish))
 
         return dishes
 
     def get_tree_of_dishes(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Dish|DishCategory]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Dish|DishCategory]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         dishes:list[Dish|DishCategory] = list()
 
         for dish in json_response:
             if 'DishCategory' in dish['className']:
                 dishes.append(DishCategory(**dish))
             elif 'Dish' in dish['className']:
                 dishes.append(Dish(**dish))
 
         return dishes
 
     def get_dish_or_dish_category(self, objectId: int, objectRid: int = None) -> Dish | DishCategory:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         if 'DishCategory' in json_response['className']:
             return DishCategory(**json_response)
         else:
             return Dish(**json_response)
 
     def get_dish_or_dish_category_with_subobjects(self, objectId: int, objectRid: int = None) -> Dish | DishCategory:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         if 'DishCategory' in json_response['className']:
             return DishCategory(**json_response)
         else:
             return Dish(**json_response)
 
     def create_dish_or_dish_category(self, object: Dish | DishCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Dish | DishCategory:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'DishCategory' in json_response['className']:
             return DishCategory(**json_response)
         else:
             return Dish(**json_response)
 
     def update_dish_or_dish_category(self, object: Dish | DishCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Dish | DishCategory:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'DishCategory' in json_response['className']:
             return DishCategory(**json_response)
         else:
             return Dish(**json_response)
 
     def remove_dish_or_dish_category(self, object: Dish | DishCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Dish | DishCategory:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'DishCategory' in json_response['className']:
             return DishCategory(**json_response)
         else:
             return Dish(**json_response)
 
     def recover_dish_or_dish_category(self, object: Dish | DishCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Dish | DishCategory:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'DishCategory' in json_response['className']:
             return DishCategory(**json_response)
         else:
             return Dish(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/employee_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/employee_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.personnel.employee import Employee
-
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class EmployeeOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "personnel.employee"
 
     def get_list_of_employee(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Employee]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Employee]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Employee] = list()
 
         for object in json_response:
             result.append(Employee(**object))
 
         return result
 
     def get_tree_of_employee(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Employee]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Employee]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Employee] = list()
 
         for object in json_response:
             result.append(Employee(**object))
 
         return result
 
     def get_employee(self, objectId: int, objectRid: int = None) -> Employee:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return Employee(**json_response)
 
     def get_employee_with_subobjects(self, objectId: int, objectRid: int = None) -> Employee:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return Employee(**json_response)
 
     def create_employee(self, object: Employee,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Employee:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Employee(**json_response)
 
     def update_employee(self, object: Employee,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Employee:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Employee(**json_response)
 
     def remove_employee(self, object: Employee,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Employee:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Employee(**json_response)
 
     def recover_employee(self, object: Employee,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Employee:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Employee(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/encashment_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/encashment_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.encashment import Encashment
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class EncashmentOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.encashment"
 
     def get_list_of_encashment(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Encashment]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Encashment]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Encashment] = list()
 
         for object in json_response:
             result.append(Encashment(**object))
 
         return result
 
     def get_tree_of_encashment(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Encashment]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Encashment]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Encashment] = list()
 
         for object in json_response:
             result.append(Encashment(**object))
 
         return result
 
     def get_encashment(self, objectId: int, objectRid: int = None) -> Encashment:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return Encashment(**json_response)
 
     def get_encashment_with_subobjects(self, objectId: int, objectRid: int = None) -> Encashment:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return Encashment(**json_response)
 
     def create_encashment(self, object: Encashment,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Encashment:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Encashment(**json_response)
 
     def update_encashment(self, object: Encashment,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Encashment:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Encashment(**json_response)
 
     def remove_encashment(self, object: Encashment,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Encashment:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Encashment(**json_response)
 
     def recover_encashment(self, object: Encashment,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Encashment:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Encashment(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.exchange_invoice import ExchangeInvoice
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class ExchangeInvoiceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.documents.exchange"
 
     def get_list_of_exchange_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[ExchangeInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[ExchangeInvoice]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[ExchangeInvoice] = list()
 
         for object in json_response:
             result.append(ExchangeInvoice(**object))
 
         return result
 
     def get_tree_of_exchange_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[ExchangeInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[ExchangeInvoice]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[ExchangeInvoice] = list()
 
         for object in json_response:
             result.append(ExchangeInvoice(**object))
 
         return result
 
     def get_exchange_invoice(self, objectId: int, objectRid: int = None) -> ExchangeInvoice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return ExchangeInvoice(**json_response)
 
     def get_exchange_invoice_with_subobjects(self, objectId: int, objectRid: int = None) -> ExchangeInvoice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return ExchangeInvoice(**json_response)
 
     def create_exchange_invoice(self, object: ExchangeInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ExchangeInvoice:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ExchangeInvoice(**json_response)
 
     def update_exchange_invoice(self, object: ExchangeInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ExchangeInvoice:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ExchangeInvoice(**json_response)
 
     def remove_exchange_invoice(self, object: ExchangeInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ExchangeInvoice:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ExchangeInvoice(**json_response)
 
     def recover_exchange_invoice(self, object: ExchangeInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ExchangeInvoice:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ExchangeInvoice(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.crm.fixed_discount import FixedDiscount
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class FixedDiscountOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "crm.settings.fixed"
 
     def get_list_of_fixed_discount(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[FixedDiscount]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[FixedDiscount]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[FixedDiscount] = list()
 
         for object in json_response:
             result.append(FixedDiscount(**object))
 
         return result
 
     def get_tree_of_fixed_discount(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[FixedDiscount]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[FixedDiscount]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[FixedDiscount] = list()
 
         for object in json_response:
             result.append(FixedDiscount(**object))
 
         return result
 
     def get_fixed_discount(self, objectId: int, objectRid: int = None) -> FixedDiscount:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return FixedDiscount(**json_response)
 
     def get_fixed_discount_with_subobjects(self, objectId: int, objectRid: int = None) -> FixedDiscount:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return FixedDiscount(**json_response)
 
     def create_fixed_discount(self, object: FixedDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> FixedDiscount:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return FixedDiscount(**json_response)
 
     def update_fixed_discount(self, object: FixedDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> FixedDiscount:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return FixedDiscount(**json_response)
 
     def remove_fixed_discount(self, object: FixedDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> FixedDiscount:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return FixedDiscount(**json_response)
 
     def recover_fixed_discount(self, object: FixedDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> FixedDiscount:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return FixedDiscount(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/hall_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
-from quick_resto_API.quick_resto_objects.modules.front.hall import Hall
+from quick_resto_API.quick_resto_objects.modules.core.packing_unit import PackingUnit
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
-class HallOperations(SystemObject):
+class PackingUnitOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
-        self._module_name:str = "front.tablemanagement.hall"
+        self._module_name:str = "core.dictionaries.packingunits"
 
-    def get_list_of_hall(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Hall]:
+    def get_list_of_packing_unit(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PackingUnit]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[Hall] = list()
+        result:list[PackingUnit] = list()
 
         for object in json_response:
-            result.append(Hall(**object))
+            result.append(PackingUnit(**object))
 
         return result
 
-    def get_tree_of_hall(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Hall]:
+    def get_tree_of_packing_unit(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PackingUnit]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[Hall] = list()
+        result:list[PackingUnit] = list()
 
         for object in json_response:
-            result.append(Hall(**object))
+            result.append(PackingUnit(**object))
 
         return result
 
-    def get_hall(self, objectId: int, objectRid: int = None) -> Hall:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+    def get_packing_unit(self, objectId: int, objectRid: int = None) -> PackingUnit:
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
-        return Hall(**json_response)
+        return PackingUnit(**json_response)
 
-    def get_hall_with_subobjects(self, objectId: int, objectRid: int = None) -> Hall:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+    def get_packing_unit_with_subobjects(self, objectId: int, objectRid: int = None) -> PackingUnit:
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
-        return Hall(**json_response)
+        return PackingUnit(**json_response)
 
-    def create_hall(self, object: Hall,ownerContextId: int = None,
+    def create_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Hall:
+                                                parentContextClassName: str = None) -> PackingUnit:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Hall(**json_response)
+        return PackingUnit(**json_response)
 
-    def update_hall(self, object: Hall,ownerContextId: int = None,
+    def update_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Hall:
+                                                parentContextClassName: str = None) -> PackingUnit:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Hall(**json_response)
+        return PackingUnit(**json_response)
 
-    def remove_hall(self, object: Hall,ownerContextId: int = None,
+    def remove_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Hall:
+                                                parentContextClassName: str = None) -> PackingUnit:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Hall(**json_response)
+        return PackingUnit(**json_response)
 
-    def recover_hall(self, object: Hall,ownerContextId: int = None,
+    def recover_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Hall:
+                                                parentContextClassName: str = None) -> PackingUnit:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Hall(**json_response)
+        return PackingUnit(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.incoming_invoice import IncomingInvoice
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class IncomingInvoiceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.documents.incoming"
 
     def get_list_of_incoming_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[IncomingInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[IncomingInvoice]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[IncomingInvoice] = list()
 
         for object in json_response:
             result.append(IncomingInvoice(**object))
 
         return result
 
     def get_tree_of_incoming_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[IncomingInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[IncomingInvoice]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[IncomingInvoice] = list()
 
         for object in json_response:
             result.append(IncomingInvoice(**object))
 
         return result
 
     def get_incoming_invoice(self, objectId: int, objectRid: int = None) -> IncomingInvoice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return IncomingInvoice(**json_response)
 
     def get_incoming_invoice_with_subobjects(self, objectId: int, objectRid: int = None) -> IncomingInvoice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return IncomingInvoice(**json_response)
 
     def create_incoming_invoice(self, object: IncomingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> IncomingInvoice:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return IncomingInvoice(**json_response)
 
     def update_incoming_invoice(self, object: IncomingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> IncomingInvoice:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return IncomingInvoice(**json_response)
 
     def remove_incoming_invoice(self, object: IncomingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> IncomingInvoice:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return IncomingInvoice(**json_response)
 
     def recover_incoming_invoice(self, object: IncomingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> IncomingInvoice:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return IncomingInvoice(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/store_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
-from quick_resto_API.quick_resto_objects.modules.warehouse.inventory_document import InventoryDocument
+from quick_resto_API.quick_resto_objects.modules.warehouse.store import Store
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
-class InventoryDocumentOperations(SystemObject):
+class StoreOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
-        self._module_name:str = "warehouse.inventory.document"
+        self._module_name:str = "warehouse.store"
 
-    def get_list_of_inventory_document(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[InventoryDocument]:
+    def get_list_of_store(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Store]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[InventoryDocument] = list()
+        result:list[Store] = list()
 
         for object in json_response:
-            result.append(InventoryDocument(**object))
+            result.append(Store(**object))
 
         return result
 
-    def get_tree_of_inventory_document(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[InventoryDocument]:
+    def get_tree_of_store(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Store]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[InventoryDocument] = list()
+        result:list[Store] = list()
 
         for object in json_response:
-            result.append(InventoryDocument(**object))
+            result.append(Store(**object))
 
         return result
 
-    def get_inventory_document(self, objectId: int, objectRid: int = None) -> InventoryDocument:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+    def get_store(self, objectId: int, objectRid: int = None) -> Store:
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
-        return InventoryDocument(**json_response)
+        return Store(**json_response)
 
-    def get_inventory_document_with_subobjects(self, objectId: int, objectRid: int = None) -> InventoryDocument:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+    def get_store_with_subobjects(self, objectId: int, objectRid: int = None) -> Store:
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
-        return InventoryDocument(**json_response)
+        return Store(**json_response)
 
-    def create_inventory_document(self, object: InventoryDocument,ownerContextId: int = None,
+    def create_store(self, object: Store,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> InventoryDocument:
+                                                parentContextClassName: str = None) -> Store:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return InventoryDocument(**json_response)
+        return Store(**json_response)
 
-    def update_inventory_document(self, object: InventoryDocument,ownerContextId: int = None,
+    def update_store(self, object: Store,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> InventoryDocument:
+                                                parentContextClassName: str = None) -> Store:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return InventoryDocument(**json_response)
+        return Store(**json_response)
 
-    def remove_inventory_document(self, object: InventoryDocument,ownerContextId: int = None,
+    def remove_store(self, object: Store,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> InventoryDocument:
+                                                parentContextClassName: str = None) -> Store:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return InventoryDocument(**json_response)
+        return Store(**json_response)
 
-    def recover_inventory_document(self, object: InventoryDocument,ownerContextId: int = None,
+    def recover_store(self, object: Store,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> InventoryDocument:
+                                                parentContextClassName: str = None) -> Store:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return InventoryDocument(**json_response)
+        return Store(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.kkm_terminal import KkmTerminal
 from quick_resto_API.quick_resto_objects.modules.front.virtual_kkm_terminal import VirtualKkmTerminal
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class KkmTerminalOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.terminals.kkm"
 
     def get_list_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[KkmTerminal|VirtualKkmTerminal]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[KkmTerminal|VirtualKkmTerminal]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[KkmTerminal|VirtualKkmTerminal] = list()
 
         for object in json_response:
             if 'KkmTerminal' in object['className']:
                 result.append(KkmTerminal(**object))
             elif 'VirtualKkmTerminal' in object['className']:
                 result.append(VirtualKkmTerminal(**object))
 
         return result
 
     def get_tree_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[KkmTerminal|VirtualKkmTerminal]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[KkmTerminal|VirtualKkmTerminal]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[KkmTerminal|VirtualKkmTerminal] = list()
 
         for object in json_response:
             if 'KkmTerminal' in object['className']:
                 result.append(KkmTerminal(**object))
             elif 'VirtualKkmTerminal' in object['className']:
                 result.append(VirtualKkmTerminal(**object))
 
         return result
 
     def get_terminal(self, objectId: int, objectRid: int = None) -> KkmTerminal|VirtualKkmTerminal:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         if 'KkmTerminal' in json_response['className']:
             return KkmTerminal(**json_response)
         else:
             return VirtualKkmTerminal(**json_response)
 
     def get_terminal_with_subobjects(self, objectId: int, objectRid: int = None) -> KkmTerminal|VirtualKkmTerminal:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         if 'KkmTerminal' in json_response['className']:
             return KkmTerminal(**json_response)
         else:
             return VirtualKkmTerminal(**json_response)
 
     def create_terminal(self, object: KkmTerminal|VirtualKkmTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> KkmTerminal|VirtualKkmTerminal:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'KkmTerminal' in json_response['className']:
             return KkmTerminal(**json_response)
         else:
             return VirtualKkmTerminal(**json_response)
 
     def update_terminal(self, object: KkmTerminal|VirtualKkmTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> KkmTerminal|VirtualKkmTerminal:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'KkmTerminal' in json_response['className']:
             return KkmTerminal(**json_response)
         else:
             return VirtualKkmTerminal(**json_response)
 
     def remove_terminal(self, object: KkmTerminal|VirtualKkmTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> KkmTerminal|VirtualKkmTerminal:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'KkmTerminal' in json_response['className']:
             return KkmTerminal(**json_response)
         else:
             return VirtualKkmTerminal(**json_response)
 
     def recover_terminal(self, object: KkmTerminal|VirtualKkmTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> KkmTerminal|VirtualKkmTerminal:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'KkmTerminal' in json_response['className']:
             return KkmTerminal(**json_response)
         else:
             return VirtualKkmTerminal(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/markup_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/markup_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.crm.markup import Markup
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class MarkupOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "crm.settings.markup"
 
     def get_list_of_markup(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Markup]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Markup]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Markup] = list()
 
         for object in json_response:
             result.append(Markup(**object))
 
         return result
 
     def get_tree_of_markup(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Markup]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Markup]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Markup] = list()
 
         for object in json_response:
             result.append(Markup(**object))
 
         return result
 
     def get_markup(self, objectId: int, objectRid: int = None) -> Markup:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return Markup(**json_response)
 
     def get_markup_with_subobjects(self, objectId: int, objectRid: int = None) -> Markup:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return Markup(**json_response)
 
     def create_markup(self, object: Markup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Markup:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Markup(**json_response)
 
     def update_markup(self, object: Markup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Markup:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Markup(**json_response)
 
     def remove_markup(self, object: Markup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Markup:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Markup(**json_response)
 
     def recover_markup(self, object: Markup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Markup:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Markup(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.core.measure_unit import MeasureUnit
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class MeasureUnitOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "core.dictionaries.measureunits"
 
     def get_list_of_measure_unit(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[MeasureUnit]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[MeasureUnit]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[MeasureUnit] = list()
 
         for object in json_response:
             result.append(MeasureUnit(**object))
 
         return result
 
     def get_tree_of_measure_unit(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[MeasureUnit]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[MeasureUnit]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[MeasureUnit] = list()
 
         for object in json_response:
             result.append(MeasureUnit(**object))
 
         return result
 
     def get_measure_unit(self, objectId: int, objectRid: int = None) -> MeasureUnit:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return MeasureUnit(**json_response)
 
     def get_measure_unit_with_subobjects(self, objectId: int, objectRid: int = None) -> MeasureUnit:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return MeasureUnit(**json_response)
 
     def create_measure_unit(self, object: MeasureUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> MeasureUnit:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return MeasureUnit(**json_response)
 
     def update_measure_unit(self, object: MeasureUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> MeasureUnit:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return MeasureUnit(**json_response)
 
     def remove_measure_unit(self, object: MeasureUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> MeasureUnit:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return MeasureUnit(**json_response)
 
     def recover_measure_unit(self, object: MeasureUnit,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> MeasureUnit:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return MeasureUnit(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/modifier_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/modifier_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,108 +1,109 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_objects.modules.warehouse.modifier import Modifier
 from quick_resto_API.quick_resto_objects.modules.warehouse.modifier_group import ModifierGroup
 from quick_resto_API.quick_resto_api import QuickRestoApi
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class ModifierOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.nomenclature.mods"
 
     def get_list_of_modifiers(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Modifier|ModifierGroup]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Modifier|ModifierGroup]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Modifier|ModifierGroup] = list()
 
         for object in json_response:
             if 'ModifierGroup' in object['className']:
                 result.append(ModifierGroup(**object))
             elif 'Modifier' in object['className']:
                 result.append(Modifier(**object))
 
         return result
 
     def get_tree_of_modifiers(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Modifier|ModifierGroup]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Modifier|ModifierGroup]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Modifier|ModifierGroup] = list()
 
         for object in json_response:
             if 'ModifierGroup' in object['className']:
                 result.append(ModifierGroup(**object))
             elif 'Modifier' in object['className']:
                 result.append(Modifier(**object))
 
         return result
 
     def get_modifiers_or_modifier_groups(self, objectId: int, objectRid: int = None) -> Modifier | ModifierGroup:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         if 'ModifierGroup' in json_response['className']:
             return ModifierGroup(**json_response)
         else:
             return Modifier(**json_response)
 
     def get_modifiers_or_modifier_groups_with_subobjects(self, objectId: int, objectRid: int = None) -> Modifier | ModifierGroup:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         if 'ModifierGroup' in json_response['className']:
             return ModifierGroup(**json_response)
         else:
             return Modifier(**json_response)
 
     def create_modifiers_or_modifier_groups(self, object: Modifier | ModifierGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Modifier | ModifierGroup:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'ModifierGroup' in json_response['className']:
             return ModifierGroup(**json_response)
         else:
             return Modifier(**json_response)
 
     def update_modifiers_or_modifier_groups(self, object: Modifier | ModifierGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Modifier | ModifierGroup:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'ModifierGroup' in json_response['className']:
             return ModifierGroup(**json_response)
         else:
             return Modifier(**json_response)
 
     def remove_modifiers_or_modifier_groups(self, object: Modifier | ModifierGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Modifier | ModifierGroup:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'ModifierGroup' in json_response['className']:
             return ModifierGroup(**json_response)
         else:
             return Modifier(**json_response)
 
     def recover_modifiers_or_modifier_groups(self, object: Modifier | ModifierGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Modifier | ModifierGroup:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'ModifierGroup' in json_response['className']:
             return ModifierGroup(**json_response)
         else:
             return Modifier(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.core.order_discard_reason import OrderDiscardReason
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class OrderDiscardReasonOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "core.dictionaries.orderdiscardreasons"
 
     def get_list_of_order_discard_reason(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[OrderDiscardReason]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[OrderDiscardReason]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[OrderDiscardReason] = list()
 
         for object in json_response:
             result.append(OrderDiscardReason(**object))
 
         return result
 
     def get_tree_of_order_discard_reason(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[OrderDiscardReason]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[OrderDiscardReason]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[OrderDiscardReason] = list()
 
         for object in json_response:
             result.append(OrderDiscardReason(**object))
 
         return result
 
     def get_order_discard_reason(self, objectId: int, objectRid: int = None) -> OrderDiscardReason:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return OrderDiscardReason(**json_response)
 
     def get_order_discard_reason_with_subobjects(self, objectId: int, objectRid: int = None) -> OrderDiscardReason:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return OrderDiscardReason(**json_response)
 
     def create_order_discard_reason(self, object: OrderDiscardReason,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderDiscardReason:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderDiscardReason(**json_response)
 
     def update_order_discard_reason(self, object: OrderDiscardReason,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderDiscardReason:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderDiscardReason(**json_response)
 
     def remove_order_discard_reason(self, object: OrderDiscardReason,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderDiscardReason:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderDiscardReason(**json_response)
 
     def recover_order_discard_reason(self, object: OrderDiscardReason,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderDiscardReason:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderDiscardReason(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_info_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/order_info_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.order_info import OrderInfo
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class OrderInfoOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.orders"
 
     def get_list_of_order_info(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[OrderInfo]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[OrderInfo]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[OrderInfo] = list()
 
         for object in json_response:
             result.append(OrderInfo(**object))
 
         return result
 
     def get_tree_of_order_info(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[OrderInfo]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[OrderInfo]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[OrderInfo] = list()
 
         for object in json_response:
             result.append(OrderInfo(**object))
 
         return result
 
     def get_order_info(self, objectId: int, objectRid: int = None) -> OrderInfo:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return OrderInfo(**json_response)
 
     def get_order_info_with_subobjects(self, objectId: int, objectRid: int = None) -> OrderInfo:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return OrderInfo(**json_response)
 
     def create_order_info(self, object: OrderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderInfo:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderInfo(**json_response)
 
     def update_order_info(self, object: OrderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderInfo:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderInfo(**json_response)
 
     def remove_order_info(self, object: OrderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderInfo:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderInfo(**json_response)
 
     def recover_order_info(self, object: OrderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OrderInfo:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OrderInfo(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.outgoing_invoice import OutgoingInvoice
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class OutgoingInvoiceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.documents.outgoing"
 
     def get_list_of_outgoing_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[OutgoingInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[OutgoingInvoice]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[OutgoingInvoice] = list()
 
         for object in json_response:
             result.append(OutgoingInvoice(**object))
 
         return result
 
     def get_tree_of_outgoing_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[OutgoingInvoice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[OutgoingInvoice]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[OutgoingInvoice] = list()
 
         for object in json_response:
             result.append(OutgoingInvoice(**object))
 
         return result
 
     def get_outgoing_invoice(self, objectId: int, objectRid: int = None) -> OutgoingInvoice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return OutgoingInvoice(**json_response)
 
     def get_outgoing_invoice_with_subobjects(self, objectId: int, objectRid: int = None) -> OutgoingInvoice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return OutgoingInvoice(**json_response)
 
     def create_outgoing_invoice(self, object: OutgoingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OutgoingInvoice:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OutgoingInvoice(**json_response)
 
     def update_outgoing_invoice(self, object: OutgoingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OutgoingInvoice:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OutgoingInvoice(**json_response)
 
     def remove_outgoing_invoice(self, object: OutgoingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OutgoingInvoice:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OutgoingInvoice(**json_response)
 
     def recover_outgoing_invoice(self, object: OutgoingInvoice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> OutgoingInvoice:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return OutgoingInvoice(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
-from quick_resto_API.quick_resto_objects.modules.core.packing_unit import PackingUnit
+from quick_resto_API.quick_resto_objects.modules.front.preorder_info import PreorderInfo
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
-class PackingUnitOperations(SystemObject):
+class PreorderInfoOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
-        self._module_name:str = "core.dictionaries.packingunits"
+        self._module_name:str = "front.preorders"
 
-    def get_list_of_packing_unit(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[PackingUnit]:
+    def get_list_of_preorder_info(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PreorderInfo]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[PackingUnit] = list()
+        result:list[PreorderInfo] = list()
 
         for object in json_response:
-            result.append(PackingUnit(**object))
+            result.append(PreorderInfo(**object))
 
         return result
 
-    def get_tree_of_packing_unit(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[PackingUnit]:
+    def get_tree_of_preorder_info(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PreorderInfo]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[PackingUnit] = list()
+        result:list[PreorderInfo] = list()
 
         for object in json_response:
-            result.append(PackingUnit(**object))
+            result.append(PreorderInfo(**object))
 
         return result
 
-    def get_packing_unit(self, objectId: int, objectRid: int = None) -> PackingUnit:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+    def get_preorder_info(self, objectId: int, objectRid: int = None) -> PreorderInfo:
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
-        return PackingUnit(**json_response)
+        return PreorderInfo(**json_response)
 
-    def get_packing_unit_with_subobjects(self, objectId: int, objectRid: int = None) -> PackingUnit:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+    def get_preorder_info_with_subobjects(self, objectId: int, objectRid: int = None) -> PreorderInfo:
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
-        return PackingUnit(**json_response)
+        return PreorderInfo(**json_response)
 
-    def create_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
+    def create_preorder_info(self, object: PreorderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> PackingUnit:
+                                                parentContextClassName: str = None) -> PreorderInfo:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return PackingUnit(**json_response)
+        return PreorderInfo(**json_response)
 
-    def update_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
+    def update_preorder_info(self, object: PreorderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> PackingUnit:
+                                                parentContextClassName: str = None) -> PreorderInfo:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return PackingUnit(**json_response)
+        return PreorderInfo(**json_response)
 
-    def remove_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
+    def remove_preorder_info(self, object: PreorderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> PackingUnit:
+                                                parentContextClassName: str = None) -> PreorderInfo:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return PackingUnit(**json_response)
+        return PreorderInfo(**json_response)
 
-    def recover_packing_unit(self, object: PackingUnit,ownerContextId: int = None,
+    def recover_preorder_info(self, object: PreorderInfo,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> PackingUnit:
+                                                parentContextClassName: str = None) -> PreorderInfo:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return PackingUnit(**json_response)
+        return PreorderInfo(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/payment_type_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/payment_type_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.core.payment_types import PaymentType
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class PaymentTypeOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "core.dictionaries.paymenttypes"
 
     def get_list_of_payment_type(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[PaymentType]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PaymentType]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[PaymentType] = list()
 
         for object in json_response:
             result.append(PaymentType(**object))
 
         return result
 
     def get_tree_of_payment_type(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[PaymentType]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PaymentType]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[PaymentType] = list()
 
         for object in json_response:
             result.append(PaymentType(**object))
 
         return result
 
     def get_payment_type(self, objectId: int, objectRid: int = None) -> PaymentType:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return PaymentType(**json_response)
 
     def get_payment_type_with_subobjects(self, objectId: int, objectRid: int = None) -> PaymentType:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return PaymentType(**json_response)
 
     def create_payment_type(self, object: PaymentType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PaymentType:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return PaymentType(**json_response)
 
     def update_payment_type(self, object: PaymentType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PaymentType:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return PaymentType(**json_response)
 
     def remove_payment_type(self, object: PaymentType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PaymentType:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return PaymentType(**json_response)
 
     def recover_payment_type(self, object: PaymentType,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PaymentType:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return PaymentType(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.pos_terminal import PosTerminal
 from quick_resto_API.quick_resto_objects.modules.front.virtual_pos_terminal import VirtualPosTerminal
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class PosTerminalOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.terminals.pos"
 
     def get_list_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[PosTerminal|VirtualPosTerminal]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PosTerminal|VirtualPosTerminal]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[PosTerminal|VirtualPosTerminal] = list()
 
         for object in json_response:
             if 'PosTerminal' in object['className']:
                 result.append(PosTerminal(**object))
             elif 'VirtualPosTerminal' in object['className']:
                 result.append(VirtualPosTerminal(**object))
 
         return result
 
     def get_tree_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[PosTerminal|VirtualPosTerminal]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[PosTerminal|VirtualPosTerminal]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[PosTerminal|VirtualPosTerminal] = list()
 
         for object in json_response:
             if 'PosTerminal' in object['className']:
                 result.append(PosTerminal(**object))
             elif 'VirtualPosTerminal' in object['className']:
                 result.append(VirtualPosTerminal(**object))
 
         return result
 
     def get_terminal(self, objectId: int, objectRid: int = None) -> PosTerminal|VirtualPosTerminal:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         if 'PosTerminal' in json_response['className']:
             return PosTerminal(**json_response)
         else:
             return VirtualPosTerminal(**json_response)
 
     def get_terminal_with_subobjects(self, objectId: int, objectRid: int = None) -> PosTerminal|VirtualPosTerminal:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         if 'PosTerminal' in json_response['className']:
             return PosTerminal(**json_response)
         else:
             return VirtualPosTerminal(**json_response)
 
     def create_terminal(self, object: PosTerminal|VirtualPosTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PosTerminal|VirtualPosTerminal:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'PosTerminal' in json_response['className']:
             return PosTerminal(**json_response)
         else:
             return VirtualPosTerminal(**json_response)
 
     def update_terminal(self, object: PosTerminal|VirtualPosTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PosTerminal|VirtualPosTerminal:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'PosTerminal' in json_response['className']:
             return PosTerminal(**json_response)
         else:
             return VirtualPosTerminal(**json_response)
 
     def remove_terminal(self, object: PosTerminal|VirtualPosTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PosTerminal|VirtualPosTerminal:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'PosTerminal' in json_response['className']:
             return PosTerminal(**json_response)
         else:
             return VirtualPosTerminal(**json_response)
 
     def recover_terminal(self, object: PosTerminal|VirtualPosTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> PosTerminal|VirtualPosTerminal:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'PosTerminal' in json_response['className']:
             return PosTerminal(**json_response)
         else:
             return VirtualPosTerminal(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/terminal_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
-from quick_resto_API.quick_resto_objects.modules.warehouse.processing_invoice import ProcessingInvoice
+from quick_resto_API.quick_resto_objects.modules.front.terminal import Terminal
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
-class ProcessingInvoiceOperations(SystemObject):
+class TerminalOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
-        self._module_name:str = "warehouse.documents.processing"
+        self._module_name:str = "front.terminals.ipad"
 
-    def get_list_of_processing_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[ProcessingInvoice]:
+    def get_list_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Terminal]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[ProcessingInvoice] = list()
+        result:list[Terminal] = list()
 
         for object in json_response:
-            result.append(ProcessingInvoice(**object))
+            result.append(Terminal(**object))
 
         return result
 
-    def get_tree_of_processing_invoice(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[ProcessingInvoice]:
+    def get_tree_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Terminal]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[ProcessingInvoice] = list()
+        result:list[Terminal] = list()
 
         for object in json_response:
-            result.append(ProcessingInvoice(**object))
+            result.append(Terminal(**object))
 
         return result
 
-    def get_processing_invoice(self, objectId: int, objectRid: int = None) -> ProcessingInvoice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+    def get_terminal(self, objectId: int, objectRid: int = None) -> Terminal:
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
-        return ProcessingInvoice(**json_response)
+        return Terminal(**json_response)
 
-    def get_processing_invoice_with_subobjects(self, objectId: int, objectRid: int = None) -> ProcessingInvoice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+    def get_terminal_with_subobjects(self, objectId: int, objectRid: int = None) -> Terminal:
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
-        return ProcessingInvoice(**json_response)
+        return Terminal(**json_response)
 
-    def create_processing_invoice(self, object: ProcessingInvoice,ownerContextId: int = None,
+    def create_terminal(self, object: Terminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> ProcessingInvoice:
+                                                parentContextClassName: str = None) -> Terminal:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return ProcessingInvoice(**json_response)
+        return Terminal(**json_response)
 
-    def update_processing_invoice(self, object: ProcessingInvoice,ownerContextId: int = None,
+    def update_terminal(self, object: Terminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> ProcessingInvoice:
+                                                parentContextClassName: str = None) -> Terminal:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return ProcessingInvoice(**json_response)
+        return Terminal(**json_response)
 
-    def remove_processing_invoice(self, object: ProcessingInvoice,ownerContextId: int = None,
+    def remove_terminal(self, object: Terminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> ProcessingInvoice:
+                                                parentContextClassName: str = None) -> Terminal:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return ProcessingInvoice(**json_response)
+        return Terminal(**json_response)
 
-    def recover_processing_invoice(self, object: ProcessingInvoice,ownerContextId: int = None,
+    def recover_terminal(self, object: Terminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> ProcessingInvoice:
+                                                parentContextClassName: str = None) -> Terminal:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return ProcessingInvoice(**json_response)
+        return Terminal(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/providers_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/providers_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.businessman import Businessman
 from quick_resto_API.quick_resto_objects.modules.warehouse.natural_person import NaturalPerson
 from quick_resto_API.quick_resto_objects.modules.warehouse.organization import Organization
 from quick_resto_API.quick_resto_objects.modules.warehouse.provider_group import ProviderGroup
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class ProvidersOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.providers"
 
     def get_list_of_provider(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Businessman|NaturalPerson|Organization|ProviderGroup]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Businessman|NaturalPerson|Organization|ProviderGroup]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Businessman|NaturalPerson|Organization|ProviderGroup] = list()
 
         for object in json_response:
             if 'Businessman' in object['className']:
                 result.append(Businessman(**object))
             elif 'NaturalPerson' in object['className']:
@@ -29,18 +30,18 @@
                 result.append(Organization(**object))
             elif 'ProviderGroup' in object['className']:
                 result.append(ProviderGroup(**object))
 
         return result
 
     def get_tree_of_provider(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Businessman|NaturalPerson|Organization|ProviderGroup]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Businessman|NaturalPerson|Organization|ProviderGroup]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Businessman|NaturalPerson|Organization|ProviderGroup] = list()
 
         for object in json_response:
             if 'Businessman' in object['className']:
                 result.append(Businessman(**object))
             elif 'NaturalPerson' in object['className']:
@@ -49,42 +50,42 @@
                 result.append(Organization(**object))
             elif 'ProviderGroup' in object['className']:
                 result.append(ProviderGroup(**object))
 
         return result
 
     def get_provider(self, objectId: int, objectRid: int = None) -> Businessman|NaturalPerson|Organization|ProviderGroup:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         if 'Businessman' in object['className']:
             return Businessman(**json_response)
         elif 'NaturalPerson' in object['className']:
             return NaturalPerson(**json_response)
         elif 'Organization' in object['className']:
             return Organization(**json_response)
         else:
             return ProviderGroup(**json_response)
 
     def get_provider_with_subobjects(self, objectId: int, objectRid: int = None) -> Businessman|NaturalPerson|Organization|ProviderGroup:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         if 'Businessman' in object['className']:
             return Businessman(**json_response)
         elif 'NaturalPerson' in object['className']:
             return NaturalPerson(**json_response)
         elif 'Organization' in object['className']:
             return Organization(**json_response)
         else:
             return ProviderGroup(**json_response)
 
     def create_provider(self, object: Businessman|NaturalPerson|Organization|ProviderGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Businessman|NaturalPerson|Organization|ProviderGroup:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'Businessman' in object['className']:
             return Businessman(**json_response)
         elif 'NaturalPerson' in object['className']:
             return NaturalPerson(**json_response)
         elif 'Organization' in object['className']:
@@ -92,15 +93,15 @@
         else:
             return ProviderGroup(**json_response)
 
     def update_provider(self, object: Businessman|NaturalPerson|Organization|ProviderGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Businessman|NaturalPerson|Organization|ProviderGroup:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'Businessman' in object['className']:
             return Businessman(**json_response)
         elif 'NaturalPerson' in object['className']:
             return NaturalPerson(**json_response)
         elif 'Organization' in object['className']:
@@ -108,15 +109,15 @@
         else:
             return ProviderGroup(**json_response)
 
     def remove_provider(self, object: Businessman|NaturalPerson|Organization|ProviderGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Businessman|NaturalPerson|Organization|ProviderGroup:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'Businessman' in object['className']:
             return Businessman(**json_response)
         elif 'NaturalPerson' in object['className']:
             return NaturalPerson(**json_response)
         elif 'Organization' in object['className']:
@@ -124,15 +125,15 @@
         else:
             return ProviderGroup(**json_response)
 
     def recover_provider(self, object: Businessman|NaturalPerson|Organization|ProviderGroup,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Businessman|NaturalPerson|Organization|ProviderGroup:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'Businessman' in object['className']:
             return Businessman(**json_response)
         elif 'NaturalPerson' in object['className']:
             return NaturalPerson(**json_response)
         elif 'Organization' in object['className']:
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.raspberry_terminal import RaspberryTerminal
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class RaspberryTerminalOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.terminals.raspberry"
 
     def get_list_of_raspberry_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[RaspberryTerminal]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[RaspberryTerminal]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[RaspberryTerminal] = list()
 
         for object in json_response:
             result.append(RaspberryTerminal(**object))
 
         return result
 
     def get_tree_of_raspberry_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[RaspberryTerminal]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[RaspberryTerminal]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[RaspberryTerminal] = list()
 
         for object in json_response:
             result.append(RaspberryTerminal(**object))
 
         return result
 
     def get_raspberry_terminal(self, objectId: int, objectRid: int = None) -> RaspberryTerminal:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return RaspberryTerminal(**json_response)
 
     def get_raspberry_terminal_with_subobjects(self, objectId: int, objectRid: int = None) -> RaspberryTerminal:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return RaspberryTerminal(**json_response)
 
     def create_raspberry_terminal(self, object: RaspberryTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> RaspberryTerminal:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return RaspberryTerminal(**json_response)
 
     def update_raspberry_terminal(self, object: RaspberryTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> RaspberryTerminal:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return RaspberryTerminal(**json_response)
 
     def remove_raspberry_terminal(self, object: RaspberryTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> RaspberryTerminal:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return RaspberryTerminal(**json_response)
 
     def recover_raspberry_terminal(self, object: RaspberryTerminal,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> RaspberryTerminal:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return RaspberryTerminal(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/sale_place_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/sale_place_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.sale_place import SalePlace
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class SalePlaceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.nomenclature.sale_place"
 
     def get_list_of_sale_place(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[SalePlace]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[SalePlace]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[SalePlace] = list()
 
         for object in json_response:
             result.append(SalePlace(**object))
 
         return result
 
     def get_tree_of_sale_place(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[SalePlace]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[SalePlace]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[SalePlace] = list()
 
         for object in json_response:
             result.append(SalePlace(**object))
 
         return result
 
     def get_sale_place(self, objectId: int, objectRid: int = None) -> SalePlace:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return SalePlace(**json_response)
 
     def get_sale_place_with_subobjects(self, objectId: int, objectRid: int = None) -> SalePlace:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return SalePlace(**json_response)
 
     def create_sale_place(self, object: SalePlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SalePlace:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return SalePlace(**json_response)
 
     def update_sale_place(self, object: SalePlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SalePlace:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return SalePlace(**json_response)
 
     def remove_sale_place(self, object: SalePlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SalePlace:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return SalePlace(**json_response)
 
     def recover_sale_place(self, object: SalePlace,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SalePlace:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return SalePlace(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.crm.scheduled_discount import ScheduledDiscount
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class ScheduledDiscountOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "crm.settings.scheduled"
 
     def get_list_of_scheduled_discount(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[ScheduledDiscount]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[ScheduledDiscount]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[ScheduledDiscount] = list()
 
         for object in json_response:
             result.append(ScheduledDiscount(**object))
 
         return result
 
     def get_tree_of_scheduled_discount(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[ScheduledDiscount]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[ScheduledDiscount]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[ScheduledDiscount] = list()
 
         for object in json_response:
             result.append(ScheduledDiscount(**object))
 
         return result
 
     def get_scheduled_discount(self, objectId: int, objectRid: int = None) -> ScheduledDiscount:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return ScheduledDiscount(**json_response)
 
     def get_scheduled_discount_with_subobjects(self, objectId: int, objectRid: int = None) -> ScheduledDiscount:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return ScheduledDiscount(**json_response)
 
     def create_scheduled_discount(self, object: ScheduledDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ScheduledDiscount:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ScheduledDiscount(**json_response)
 
     def update_scheduled_discount(self, object: ScheduledDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ScheduledDiscount:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ScheduledDiscount(**json_response)
 
     def remove_scheduled_discount(self, object: ScheduledDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ScheduledDiscount:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ScheduledDiscount(**json_response)
 
     def recover_scheduled_discount(self, object: ScheduledDiscount,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> ScheduledDiscount:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return ScheduledDiscount(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/semi_product_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/semi_product_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.semi_product import SemiProduct
 from quick_resto_API.quick_resto_objects.modules.warehouse.store_category import StoreCategory
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class SemiProductOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.nomenclature.semiproduct"
 
     def get_list_of_semi_product(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[SemiProduct|StoreCategory]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[SemiProduct|StoreCategory]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[SemiProduct|StoreCategory] = list()
 
         for object in json_response:
             if 'StoreCategory' in object['className']:
                 result.append(StoreCategory(**object))
             elif 'SemiProduct' in object['className']:
                 result.append(SemiProduct(**object))
 
         return result
 
     def get_tree_of_semi_product(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[SemiProduct|StoreCategory]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[SemiProduct|StoreCategory]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[SemiProduct|StoreCategory] = list()
 
         for object in json_response:
             if 'StoreCategory' in object['className']:
                 result.append(StoreCategory(**object))
             elif 'SemiProduct' in object['className']:
                 result.append(SemiProduct(**object))
 
         return result
 
     def get_semi_product_or_store_category(self, objectId: int, objectRid: int = None) -> SemiProduct | StoreCategory:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         if 'StoreCategory' in json_response['className']:
             return StoreCategory(**json_response)
         else:
             return SemiProduct(**json_response)
 
     def get_semi_product_or_store_category_with_subobjects(self, objectId: int, objectRid: int = None) -> SemiProduct | StoreCategory:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         if 'StoreCategory' in json_response['className']:
             return StoreCategory(**json_response)
         else:
             return SemiProduct(**json_response)
 
     def create_semi_product_or_store_category(self, object: SemiProduct | StoreCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SemiProduct | StoreCategory:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'StoreCategory' in json_response['className']:
             return StoreCategory(**json_response)
         else:
             return SemiProduct(**json_response)
 
     def update_semi_product_or_store_category(self, object: SemiProduct | StoreCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SemiProduct | StoreCategory:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'StoreCategory' in json_response['className']:
             return StoreCategory(**json_response)
         else:
             return SemiProduct(**json_response)
 
     def remove_semi_product_or_store_category(self, object: SemiProduct | StoreCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SemiProduct | StoreCategory:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'StoreCategory' in json_response['className']:
             return StoreCategory(**json_response)
         else:
             return SemiProduct(**json_response)
 
     def recover_semi_product_or_store_category(self, object: SemiProduct | StoreCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SemiProduct | StoreCategory:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'StoreCategory' in json_response['className']:
             return StoreCategory(**json_response)
         else:
             return SemiProduct(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/shift_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/shift_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.shift import Shift
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class ShiftOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.zreport"
 
     def get_list_of_shift(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Shift]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Shift]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Shift] = list()
 
         for object in json_response:
             result.append(Shift(**object))
 
         return result
 
     def get_tree_of_shift(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Shift]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Shift]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Shift] = list()
 
         for object in json_response:
             result.append(Shift(**object))
 
         return result
 
     def get_shift(self, objectId: int, objectRid: int = None) -> Shift:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return Shift(**json_response)
 
     def get_shift_with_subobjects(self, objectId: int, objectRid: int = None) -> Shift:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return Shift(**json_response)
 
     def create_shift(self, object: Shift,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Shift:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Shift(**json_response)
 
     def update_shift(self, object: Shift,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Shift:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Shift(**json_response)
 
     def remove_shift(self, object: Shift,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Shift:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Shift(**json_response)
 
     def recover_shift(self, object: Shift,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Shift:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Shift(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/single_product_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/single_product_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.warehouse.single_category import SingleCategory
 from quick_resto_API.quick_resto_objects.modules.warehouse.single_product import SingleProduct
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class SingleProductOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "warehouse.nomenclature.singleproduct"
     
     def get_list_of_single_product(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[SingleCategory|SingleProduct]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[SingleCategory|SingleProduct]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[SingleCategory|SingleProduct] = list()
 
         for object in json_response:
             if 'SingleCategory' in object['className']:
                 result.append(SingleCategory(**object))
             elif 'SingleProduct' in object['className']:
                 result.append(SingleProduct(**object))
 
         return result
 
     def get_tree_of_single_product(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[SingleCategory|SingleProduct]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[SingleCategory|SingleProduct]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[SingleCategory|SingleProduct] = list()
 
         for object in json_response:
             if 'SingleCategory' in object['className']:
                 result.append(SingleCategory(**object))
             elif 'SingleProduct' in object['className']:
                 result.append(SingleProduct(**object))
 
         return result
 
     def get_single_product_or_single_category(self, objectId: int, objectRid: int = None) -> SingleProduct | SingleCategory:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         if 'SingleCategory' in json_response['className']:
             return SingleCategory(**json_response)
         else:
             return SingleProduct(**json_response)
 
     def get_single_product_or_single_category_with_subobjects(self, objectId: int, objectRid: int = None) -> SingleProduct | SingleCategory:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         if 'SingleCategory' in json_response['className']:
             return SingleCategory(**json_response)
         else:
             return SingleProduct(**json_response)
 
     def create_single_product_or_single_category(self, object: SingleProduct | SingleCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SingleProduct | SingleCategory:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'SingleCategory' in json_response['className']:
             return SingleCategory(**json_response)
         else:
             return SingleProduct(**json_response)
 
     def update_single_product_or_single_category(self, object: SingleProduct | SingleCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SingleProduct | SingleCategory:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'SingleCategory' in json_response['className']:
             return SingleCategory(**json_response)
         else:
             return SingleProduct(**json_response)
 
     def remove_single_product_or_single_category(self, object: SingleProduct | SingleCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SingleProduct | SingleCategory:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'SingleCategory' in json_response['className']:
             return SingleCategory(**json_response)
         else:
             return SingleProduct(**json_response)
 
     def recover_single_product_or_single_category(self, object: SingleProduct | SingleCategory,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> SingleProduct | SingleCategory:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         if 'SingleCategory' in json_response['className']:
             return SingleCategory(**json_response)
         else:
             return SingleProduct(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.core.store_item_tag import StoreItemTag
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class StoreItemTagOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "core.dictionaries.storeitemtag"
 
     def get_list_of_store_item_tag(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[StoreItemTag]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[StoreItemTag]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[StoreItemTag] = list()
 
         for object in json_response:
             result.append(StoreItemTag(**object))
 
         return result
 
     def get_tree_of_store_item_tag(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[StoreItemTag]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[StoreItemTag]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[StoreItemTag] = list()
 
         for object in json_response:
             result.append(StoreItemTag(**object))
 
         return result
 
     def get_store_item_tag(self, objectId: int, objectRid: int = None) -> StoreItemTag:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return StoreItemTag(**json_response)
 
     def get_store_item_tag_with_subobjects(self, objectId: int, objectRid: int = None) -> StoreItemTag:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return StoreItemTag(**json_response)
 
     def create_store_item_tag(self, object: StoreItemTag,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> StoreItemTag:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return StoreItemTag(**json_response)
 
     def update_store_item_tag(self, object: StoreItemTag,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> StoreItemTag:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return StoreItemTag(**json_response)
 
     def remove_store_item_tag(self, object: StoreItemTag,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> StoreItemTag:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return StoreItemTag(**json_response)
 
     def recover_store_item_tag(self, object: StoreItemTag,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> StoreItemTag:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return StoreItemTag(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/operations_with_objects.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,109 @@
-from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
-from quick_resto_API.operations_with_objects.system_object import SystemObject
-from quick_resto_API.quick_resto_api import QuickRestoApi
-from quick_resto_API.quick_resto_objects.modules.warehouse.store import Store
-
-class StoreOperations(SystemObject):
-    def __init__(self, api: QuickRestoApi):
-        self._operations_with_objects = OperationsWithObjects(api)
-
-        self._module_name:str = "warehouse.store"
-
-    def get_list_of_store(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Store]:
-
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
-
-        result:list[Store] = list()
-
-        for object in json_response:
-            result.append(Store(**object))
-
-        return result
-
-    def get_tree_of_store(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Store]:
-
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
-
-        result:list[Store] = list()
-
-        for object in json_response:
-            result.append(Store(**object))
-
-        return result
+import json
 
-    def get_store(self, objectId: int, objectRid: int = None) -> Store:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
-
-        return Store(**json_response)
-
-    def get_store_with_subobjects(self, objectId: int, objectRid: int = None) -> Store:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
-
-        return Store(**json_response)
-
-    def create_store(self, object: Store,ownerContextId: int = None,
-                                                ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Store:
-
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
-                                                ownerContextClassName, parentContextId, parentContextClassName).json()
-
-        return Store(**json_response)
-
-    def update_store(self, object: Store,ownerContextId: int = None,
-                                                ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Store:
-
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
-                                                ownerContextClassName, parentContextId, parentContextClassName).json()
-
-        return Store(**json_response)
-
-    def remove_store(self, object: Store,ownerContextId: int = None,
-                                                ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Store:
-
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
-                                                ownerContextClassName, parentContextId, parentContextClassName).json()
-
-        return Store(**json_response)
+from quick_resto_API.quick_resto_api import QuickRestoApi
+from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
-    def recover_store(self, object: Store,ownerContextId: int = None,
-                                                ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Store:
+class OperationsWithObjects:
+    def __init__(self, quick_resto_api: QuickRestoApi):
+        self._api: QuickRestoApi = quick_resto_api
+
+    def get_list(self, moduleName: str, ownerContextId: int = None,
+                ownerContextClassName: str = None, showDeleted: bool = False, listRequest: ListRequest = None):
+        params = {
+            "moduleName": moduleName,
+            "ownerContextId": ownerContextId,
+            "ownerContextClassName": ownerContextClassName,
+            "showDeleted": showDeleted
+        }
+
+        return self._api.get("/api/list", parameters=params, json_data=listRequest.get_json_object())
+
+    def get_tree(self, moduleName: str, ownerContextId: int = None,
+                ownerContextClassName: str = None, showDeleted: bool = False, listRequest: ListRequest = None):
+        params = {
+            "moduleName": moduleName,
+            "ownerContextId": ownerContextId,
+            "ownerContextClassName": ownerContextClassName,
+            "showDeleted": showDeleted
+        }
+
+        return self._api.get("/api/tree", parameters=params, json_data=listRequest.get_json_object())
+
+    def get_object(self, moduleName: str, objectId: int, objectRid: int = None):
+        params = {
+            "moduleName": moduleName,
+            "objectId": objectId,
+            "objectRid": objectRid
+        }
+
+        return self._api.get("/api/get", parameters=params)
+
+    def get_object_with_subobjects(self, moduleName: str, objectId: int, objectRid: int = None):
+        params = {
+            "moduleName": moduleName,
+            "objectId": objectId,
+            "objectRid": objectRid
+        }
+
+        return self._api.get("/api/read", parameters=params)
+
+    def create_object(self, object: QuickRestoObject, moduleName: str, ownerContextId: int = None,
+                     ownerContextClassName: str = None, parentContextId: int = None,
+                     parentContextClassName: str = None):
+        params = {
+            "moduleName": moduleName,
+            "ownerContextId": ownerContextId,
+            "ownerContextClassName": ownerContextClassName,
+            "parentContextId": parentContextId,
+            "parentContextClassName": parentContextClassName
+        }
+
+        json_data = object.get_json_object()
+
+        return self._api.post("/api/create", parameters=params, json_data=json_data)
+
+    def update_object(self, object: QuickRestoObject, moduleName: str, ownerContextId: int = None,
+                     ownerContextClassName: str = None, parentContextId: int = None,
+                     parentContextClassName: str = None):
+        params = {
+            "moduleName": moduleName,
+            "ownerContextId": ownerContextId,
+            "ownerContextClassName": ownerContextClassName,
+            "parentContextId": parentContextId,
+            "parentContextClassName": parentContextClassName
+        }
+
+        json_data = object.get_json_object()
+
+        return self._api.post("/api/update", parameters=params, json_data=json_data)
+
+    def remove_object(self, object: QuickRestoObject, moduleName: str, ownerContextId: int = None,
+                     ownerContextClassName: str = None, parentContextId: int = None,
+                     parentContextClassName: str = None):
+        params = {
+            "moduleName": moduleName,
+            "ownerContextId": ownerContextId,
+            "ownerContextClassName": ownerContextClassName,
+            "parentContextId": parentContextId,
+            "parentContextClassName": parentContextClassName
+        }
+
+        json_data = object.get_json_object()
+
+        return self._api.post("/api/remove", parameters=params, json_data=json_data)
+
+    def recover_object(self, object: QuickRestoObject, moduleName: str, ownerContextId: int = None,
+                      ownerContextClassName: str = None, parentContextId: int = None,
+                      parentContextClassName: str = None):
+        params = {
+            "moduleName": moduleName,
+            "ownerContextId": ownerContextId,
+            "ownerContextClassName": ownerContextClassName,
+            "parentContextId": parentContextId,
+            "parentContextClassName": parentContextClassName
+        }
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
-                                                ownerContextClassName, parentContextId, parentContextClassName).json()
+        json_data = object.get_json_object()
 
-        return Store(**json_response)
+        return self._api.post("/api/recover", parameters=params, json_data=json_data)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/table_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.table import Table
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class TableOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.tablemanagement.table"
 
     def get_list_of_table(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Table]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Table]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Table] = list()
 
         for object in json_response:
             result.append(Table(**object))
 
         return result
 
     def get_tree_of_table(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Table]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Table]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[Table] = list()
 
         for object in json_response:
             result.append(Table(**object))
 
         return result
 
     def get_table(self, objectId: int, objectRid: int = None) -> Table:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return Table(**json_response)
 
     def get_table_with_subobjects(self, objectId: int, objectRid: int = None) -> Table:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return Table(**json_response)
 
     def create_table(self, object: Table,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Table:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Table(**json_response)
 
     def update_table(self, object: Table,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Table:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Table(**json_response)
 
     def remove_table(self, object: Table,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Table:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Table(**json_response)
 
     def recover_table(self, object: Table,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> Table:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return Table(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.table_scheme import TableScheme
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class TableSchemeOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.tablemanagement"
 
     def get_list_of_table_scheme(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[TableScheme]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[TableScheme]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[TableScheme] = list()
 
         for object in json_response:
             result.append(TableScheme(**object))
 
         return result
 
     def get_tree_of_table_scheme(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[TableScheme]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[TableScheme]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[TableScheme] = list()
 
         for object in json_response:
             result.append(TableScheme(**object))
 
         return result
 
     def get_table_scheme(self, objectId: int, objectRid: int = None) -> TableScheme:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return TableScheme(**json_response)
 
     def get_table_scheme_with_subobjects(self, objectId: int, objectRid: int = None) -> TableScheme:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return TableScheme(**json_response)
 
     def create_table_scheme(self, object: TableScheme,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TableScheme:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TableScheme(**json_response)
 
     def update_table_scheme(self, object: TableScheme,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TableScheme:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TableScheme(**json_response)
 
     def remove_table_scheme(self, object: TableScheme,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TableScheme:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TableScheme(**json_response)
 
     def recover_table_scheme(self, object: TableScheme,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TableScheme:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TableScheme(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/terminal_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/hall_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
-from quick_resto_API.quick_resto_objects.modules.front.terminal import Terminal
+from quick_resto_API.quick_resto_objects.modules.front.hall import Hall
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
-class TerminalOperations(SystemObject):
+class HallOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
-        self._module_name:str = "front.terminals.ipad"
+        self._module_name:str = "front.tablemanagement.hall"
 
-    def get_list_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Terminal]:
+    def get_list_of_hall(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Hall]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[Terminal] = list()
+        result:list[Hall] = list()
 
         for object in json_response:
-            result.append(Terminal(**object))
+            result.append(Hall(**object))
 
         return result
 
-    def get_tree_of_terminal(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[Terminal]:
+    def get_tree_of_hall(self, ownerContextId: int = None, ownerContextClassName: str = None,
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[Hall]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
-        result:list[Terminal] = list()
+        result:list[Hall] = list()
 
         for object in json_response:
-            result.append(Terminal(**object))
+            result.append(Hall(**object))
 
         return result
 
-    def get_terminal(self, objectId: int, objectRid: int = None) -> Terminal:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+    def get_hall(self, objectId: int, objectRid: int = None) -> Hall:
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
-        return Terminal(**json_response)
+        return Hall(**json_response)
 
-    def get_terminal_with_subobjects(self, objectId: int, objectRid: int = None) -> Terminal:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+    def get_hall_with_subobjects(self, objectId: int, objectRid: int = None) -> Hall:
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
-        return Terminal(**json_response)
+        return Hall(**json_response)
 
-    def create_terminal(self, object: Terminal,ownerContextId: int = None,
+    def create_hall(self, object: Hall,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Terminal:
+                                                parentContextClassName: str = None) -> Hall:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Terminal(**json_response)
+        return Hall(**json_response)
 
-    def update_terminal(self, object: Terminal,ownerContextId: int = None,
+    def update_hall(self, object: Hall,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Terminal:
+                                                parentContextClassName: str = None) -> Hall:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Terminal(**json_response)
+        return Hall(**json_response)
 
-    def remove_terminal(self, object: Terminal,ownerContextId: int = None,
+    def remove_hall(self, object: Hall,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Terminal:
+                                                parentContextClassName: str = None) -> Hall:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Terminal(**json_response)
+        return Hall(**json_response)
 
-    def recover_terminal(self, object: Terminal,ownerContextId: int = None,
+    def recover_hall(self, object: Hall,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
-                                                parentContextClassName: str = None) -> Terminal:
+                                                parentContextClassName: str = None) -> Hall:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
-        return Terminal(**json_response)
+        return Hall(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py` & `quick_resto_API-1.2.0/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from quick_resto_API.operations_with_objects.operations_with_objects import OperationsWithObjects
 from quick_resto_API.operations_with_objects.system_object import SystemObject
 from quick_resto_API.quick_resto_api import QuickRestoApi
 from quick_resto_API.quick_resto_objects.modules.front.ticket_device import TicketDevice
+from quick_resto_API.operations_with_objects.list_request.list_request import ListRequest
 
 class TicketDeviceOperations(SystemObject):
     def __init__(self, api: QuickRestoApi):
         self._operations_with_objects = OperationsWithObjects(api)
 
         self._module_name:str = "front.terminals.ticketdevices"
 
     def get_list_of_ticket_device(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[TicketDevice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[TicketDevice]:
 
-        json_response = self._operations_with_objects.getList(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_list(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[TicketDevice] = list()
 
         for object in json_response:
             result.append(TicketDevice(**object))
 
         return result
 
     def get_tree_of_ticket_device(self, ownerContextId: int = None, ownerContextClassName: str = None,
-                           showDeleted: bool = False) -> list[TicketDevice]:
+                           showDeleted: bool = False, listRequest: ListRequest = None) -> list[TicketDevice]:
 
-        json_response = self._operations_with_objects.getTree(self._module_name,
-                                                              ownerContextId, ownerContextClassName, showDeleted).json()
+        json_response = self._operations_with_objects.get_tree(self._module_name,
+                                                              ownerContextId, ownerContextClassName, showDeleted, listRequest).json()
 
         result:list[TicketDevice] = list()
 
         for object in json_response:
             result.append(TicketDevice(**object))
 
         return result
 
     def get_ticket_device(self, objectId: int, objectRid: int = None) -> TicketDevice:
-        json_response = self._operations_with_objects.getObject(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object(self._module_name, objectId, objectRid).json()
 
         return TicketDevice(**json_response)
 
     def get_ticket_device_with_subobjects(self, objectId: int, objectRid: int = None) -> TicketDevice:
-        json_response = self._operations_with_objects.getObjectWithSubobjects(self._module_name, objectId, objectRid).json()
+        json_response = self._operations_with_objects.get_object_with_subobjects(self._module_name, objectId, objectRid).json()
 
         return TicketDevice(**json_response)
 
     def create_ticket_device(self, object: TicketDevice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TicketDevice:
 
-        json_response = self._operations_with_objects.createObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.create_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TicketDevice(**json_response)
 
     def update_ticket_device(self, object: TicketDevice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TicketDevice:
 
-        json_response = self._operations_with_objects.updateObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.update_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TicketDevice(**json_response)
 
     def remove_ticket_device(self, object: TicketDevice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TicketDevice:
 
-        json_response = self._operations_with_objects.removeObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.remove_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TicketDevice(**json_response)
 
     def recover_ticket_device(self, object: TicketDevice,ownerContextId: int = None,
                                                 ownerContextClassName: str = None, parentContextId: int = None,
                                                 parentContextClassName: str = None) -> TicketDevice:
 
-        json_response = self._operations_with_objects.recoverObject(object, self._module_name, ownerContextId, 
+        json_response = self._operations_with_objects.recover_object(object, self._module_name, ownerContextId, 
                                                 ownerContextClassName, parentContextId, parentContextClassName).json()
 
         return TicketDevice(**json_response)
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_api.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_api.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_interface.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_interface.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/business.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/business.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/company_info.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/company_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/payment.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment_types.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/payment_types.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_type.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/account_type.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/customer.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/group.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/group.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/markup.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/markup.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/cancellation.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/cancellation.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/device_command.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/device_command.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/encashment.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/encashment.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/hall.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/hall.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_info.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/order_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_item.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/order_item.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/shift.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/shift.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/table.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/terminal.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/employee.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/personnel/employee.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/user.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/personnel/user.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/store.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/right_link.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/platform/right_link.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/role.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/platform/role.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/quick_resto_object.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/quick_resto_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         result = dict()
 
         for key, value in as_dict.items():
             parameter_name = styler.to_camel_case(key)
 
             if issubclass(type(value), QuickRestoObject):
                 result[parameter_name] = value.get_json_object()
+            elif issubclass(type(value), Enum):
+                result[parameter_name] = value.value
             elif issubclass(type(value), list):
                 list_of_subobjects = []
 
                 for obj in value:
                     if issubclass(type(obj), QuickRestoObject):
                         list_of_subobjects.append(obj.get_json_object())
```

### Comparing `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/styler.py` & `quick_resto_API-1.2.0/quick_resto_API/quick_resto_objects/styler.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/quick_resto_API.egg-info/SOURCES.txt` & `quick_resto_API-1.2.0/quick_resto_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.8/setup.py` & `quick_resto_API-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from pathlib import Path
 
 setup(
     name="quick_resto_API",
-    version="1.1.8",
+    version="1.2.0",
     description='Quick Resto API',
     packages=['quick_resto_API', 'quick_resto_API.operations_with_objects.modules', 'quick_resto_API.operations_with_objects', 
                 'quick_resto_API.quick_resto_objects.modules.alcohol', 'quick_resto_API.quick_resto_objects.modules.core',
                 'quick_resto_API.quick_resto_objects.modules.crm','quick_resto_API.quick_resto_objects.modules.front',
                 'quick_resto_API.quick_resto_objects.modules.personnel','quick_resto_API.quick_resto_objects.modules.warehouse',
                 'quick_resto_API.quick_resto_objects.platform','quick_resto_API.quick_resto_objects'],
```

