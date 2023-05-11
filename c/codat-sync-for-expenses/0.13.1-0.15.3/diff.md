# Comparing `tmp/codat-sync-for-expenses-0.13.1.tar.gz` & `tmp/codat-sync-for-expenses-0.15.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.13.1.tar", last modified: Thu Apr 27 15:54:16 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.15.3.tar", last modified: Thu May 11 20:35:54 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.13.1.tar` & `codat-sync-for-expenses-0.15.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.912276 codat-sync-for-expenses-0.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 15:54:16.912276 codat-sync-for-expenses-0.13.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:54:16.912276 codat-sync-for-expenses-0.13.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.904276 codat-sync-for-expenses-0.13.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.904276 codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 15:54:16.000000 codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-27 15:54:16.000000 codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:54:16.000000 codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 15:54:16.000000 codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 15:54:16.000000 codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.904276 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4374 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4441 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.904276 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.908276 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      816 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1614 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.912276 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5711 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5408 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4851 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1329 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/integrationtype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      569 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2148 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2418 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1611 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2027 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3968 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:54:16.912276 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-27 15:53:56.000000 codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.909308 codat-sync-for-expenses-0.15.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.913308 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.917308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4384 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2400 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4451 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2329 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.917308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.921308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/integrationtype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6597 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3978 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25963 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.13.1/PKG-INFO` & `codat-sync-for-expenses-0.15.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.13.1
+Version: 0.15.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -29,17 +29,16 @@
 
 s = codatsyncexpenses.CodatSyncExpenses(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
-
 req = operations.GetCompanyConfigurationRequest(
-    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    company_id='8a210b68-6988-11ed-a1eb-0242ac120002',
 )
 
 res = s.configuration.get_company_configuration(req)
 
 if res.company_configuration is not None:
     # handle response
 ```
```

### Comparing `codat-sync-for-expenses-0.13.1/README.md` & `codat-sync-for-expenses-0.15.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 
 s = codatsyncexpenses.CodatSyncExpenses(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
-
 req = operations.GetCompanyConfigurationRequest(
-    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    company_id='8a210b68-6988-11ed-a1eb-0242ac120002',
 )
 
 res = s.configuration.get_company_configuration(req)
 
 if res.company_configuration is not None:
     # handle response
 ```
```

### Comparing `codat-sync-for-expenses-0.13.1/setup.py` & `codat-sync-for-expenses-0.15.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.13.1",
+    version="0.15.3",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.13.1
+Version: 0.15.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -29,17 +29,16 @@
 
 s = codatsyncexpenses.CodatSyncExpenses(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
-
 req = operations.GetCompanyConfigurationRequest(
-    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    company_id='8a210b68-6988-11ed-a1eb-0242ac120002',
 )
 
 res = s.configuration.get_company_configuration(req)
 
 if res.company_configuration is not None:
     # handle response
 ```
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def get_company_configuration(self, request: operations.GetCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyConfigurationResponse:
         r"""Get company configuration
         Gets a companies expense sync configuration
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
@@ -54,14 +55,15 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanyConfiguration])
                 res.company_configuration = out
 
         return res
 
+    
     def save_company_configuration(self, request: operations.SaveCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.SaveCompanyConfigurationResponse:
         r"""Set company configuration
         Sets a companies expense sync configuration
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.SaveCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def create_partner_expense_connection(self, request: operations.CreatePartnerExpenseConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreatePartnerExpenseConnectionResponse:
         r"""Create Partner Expense connection
         Creates a Partner Expense data connection
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreatePartnerExpenseConnectionRequest, base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/expenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def create_expense_dataset(self, request: operations.CreateExpenseDatasetRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateExpenseDatasetResponse:
         r"""Create expense-transactions
         Create an expense transaction
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateExpenseDatasetRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
@@ -58,14 +59,15 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateExpenseResponse])
                 res.create_expense_response = out
 
         return res
 
+    
     def upload_attachment(self, request: operations.UploadAttachmentRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UploadAttachmentResponse:
         r"""Upload attachment
         Creates an attachment in the accounting software against the given transactionId
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.UploadAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/mapping_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def get_mapping_options(self, request: operations.GetMappingOptionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetMappingOptionsResponse:
         r"""Mapping options
         Gets the expense mapping options for a companies accounting software
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,19 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateExpenseDatasetRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     create_expense_request: Optional[shared_createexpenserequest.CreateExpenseRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
     
 
 @dataclasses.dataclass
 class CreateExpenseDatasetResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     create_expense_response: Optional[shared_createexpenseresponse.CreateExpenseResponse] = dataclasses.field(default=None)
-
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreatePartnerExpenseConnectionRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class CreatePartnerExpenseConnectionResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     data_connection: Optional[shared_dataconnection.DataConnection] = dataclasses.field(default=None)
-
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetCompanyConfigurationRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class GetCompanyConfigurationResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
-
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetLastSuccessfulSyncRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class GetLastSuccessfulSyncResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
-
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetLatestSyncRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class GetLatestSyncResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
-
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import mappingoptions as shared_mappingoptions
+from ..shared import companysyncstatus as shared_companysyncstatus
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetMappingOptionsRequest:
+class GetSyncByIDRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
+    sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a sync."""
     
 
 @dataclasses.dataclass
-class GetMappingOptionsResponse:
+class GetSyncByIDResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
-    mapping_options: Optional[shared_mappingoptions.MappingOptions] = dataclasses.field(default=None)
-
+    company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,22 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetSyncTransactionRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
-
     r"""Unique identifier for a sync."""
     transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transactionId', 'style': 'simple', 'explode': False }})
-
     r"""The unique identifier for your SMB's transaction."""
     
 
 @dataclasses.dataclass
 class GetSyncTransactionResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     transaction_metadata: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None)
-
     r"""Success"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,21 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class IntiateSyncRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     post_sync: Optional[shared_postsync.PostSync] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
     
 
 @dataclasses.dataclass
 class IntiateSyncResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     codat_error_message: Optional[shared_codaterrormessage.CodatErrorMessage] = dataclasses.field(default=None)
-
     r"""If model is incorrect"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     sync_initiated: Optional[shared_syncinitiated.SyncInitiated] = dataclasses.field(default=None)
-
     r"""Returns the newly created SyncId"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,32 +7,24 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListSyncTransactionsRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-
     r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
-
     r"""Unique identifier for a sync."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-
     r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
     
 
 @dataclasses.dataclass
 class ListSyncTransactionsResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     transaction_metadata_list: Optional[shared_transactionmetadatalist.TransactionMetadataList] = dataclasses.field(default=None)
-
     r"""Success"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListSyncsRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class ListSyncsResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     company_sync_statuses: Optional[list[shared_companysyncstatus.CompanySyncStatus]] = dataclasses.field(default=None)
-
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,28 +8,21 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class SaveCompanyConfigurationRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-
     
 
 @dataclasses.dataclass
 class SaveCompanyConfigurationResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     codat_error_message: Optional[shared_codaterrormessage.CodatErrorMessage] = dataclasses.field(default=None)
-
     r"""Bad Request"""
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
-
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,40 +7,30 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UploadAttachmentRequestBody:
     
     content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})
-
     request_body: str = dataclasses.field(metadata={'multipart_form': { 'field_name': 'requestBody' }})
-
     
 
 @dataclasses.dataclass
 class UploadAttachmentRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-
     sync_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'syncId', 'style': 'simple', 'explode': False }})
-
     r"""Unique identifier for a sync."""
     transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transactionId', 'style': 'simple', 'explode': False }})
-
     r"""The unique identifier for your SMB's transaction."""
     request_body: Optional[UploadAttachmentRequestBody] = dataclasses.field(default=None, metadata={'multipart_form': { 'file': True }, 'request': { 'media_type': 'multipart/form-data' }})
-
     
 
 @dataclasses.dataclass
 class UploadAttachmentResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     attachment: Optional[shared_attachment.Attachment] = dataclasses.field(default=None)
-
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,17 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AccountMappingInfo:
     
     account_type: Optional[AccountMappingInfoAccountTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
-
     r"""Type of the account."""
     currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-
     r"""Currency of the account."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""Unique identifier of account."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-
     r"""Name of the account as it appears in the companies accounting software."""
     valid_transaction_types: Optional[list[AccountMappingInfoValidTransactionTypesEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
-
     r"""Supported transaction types for the account."""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,13 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Attachment:
     r"""OK"""
     
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-
     r"""Unique ID of company in Codat"""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""Unique identifier of attachment"""
     transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
-
     r"""Unique identifier of transaction"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,10 +8,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BankAccount:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""The id of the account from which purchases are made"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,84 +8,58 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidationErrors:
     
     item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
-
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
-
     validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidationInternals:
     
     item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
-
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
-
     validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidationWarnings:
     
     item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
-
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-
     rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
-
     validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessageValidation:
     
     errors: Optional[list[CodatErrorMessageValidationErrors]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
-
     has_errors: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasErrors'), 'exclude': lambda f: f is None }})
-
     has_internals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasInternals'), 'exclude': lambda f: f is None }})
-
     has_warnings: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasWarnings'), 'exclude': lambda f: f is None }})
-
     internals: Optional[list[CodatErrorMessageValidationInternals]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('internals'), 'exclude': lambda f: f is None }})
-
     warnings: Optional[list[CodatErrorMessageValidationWarnings]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warnings'), 'exclude': lambda f: f is None }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessage:
     r"""Bad Request"""
     
     can_be_retried: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('canBeRetried'), 'exclude': lambda f: f is None }})
-
     correlation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('correlationId'), 'exclude': lambda f: f is None }})
-
     detailed_error_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailedErrorCode'), 'exclude': lambda f: f is None }})
-
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-
     inner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inner'), 'exclude': lambda f: f is None }})
-
     service: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service'), 'exclude': lambda f: f is None }})
-
     status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-
     validation: Optional[CodatErrorMessageValidation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,13 +11,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompanyConfiguration:
     r"""Success"""
     
     bank_account: shared_bankaccount.BankAccount = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccount') }})
-
     customer: shared_customer.Customer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})
-
     supplier: shared_supplier.Supplier = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplier') }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,36 +9,28 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CompanySyncStatus:
     r"""Success"""
     
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-
     r"""Unique identifier for your SMB in Codat."""
     data_pushed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataPushed'), 'exclude': lambda f: f is None }})
-
     r"""Boolean of whether the sync resulted in data being pushed."""
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-
     r"""Error message of the sync."""
     sync_exception_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncExceptionMessage'), 'exclude': lambda f: f is None }})
-
     r"""Exception message of the sync."""
     sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncId'), 'exclude': lambda f: f is None }})
-
     r"""Unique identifier of the sync."""
     sync_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatus'), 'exclude': lambda f: f is None }})
-
     r"""Text status of the sync."""
     sync_status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatusCode'), 'exclude': lambda f: f is None }})
-
     r"""Status code of the sync."""
     sync_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncUtc'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateExpenseRequest:
     
     items: Optional[list[shared_expensetransaction.ExpenseTransaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,10 +9,9 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateExpenseResponse:
     r"""OK"""
     
     dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetId'), 'exclude': lambda f: f is None }})
-
     r"""Unique id of dataset created"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,10 +8,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Customer:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""id of the customer for all income related activities to be associated to."""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataConnection:
     r"""A connection represents the link between a `company` and a source of data."""
     
     created: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created') }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -42,43 +41,31 @@
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-
     r"""Unique identifier for a company's data connection."""
     integration_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
-
     r"""A Codat ID representing the integration."""
     integration_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationKey') }})
-
     r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""
     link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})
-
     platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})
-
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-
     r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
     source_type: DataConnectionSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     r"""The type of platform of the connection."""
     status: shared_dataconnectionstatus_enum.DataConnectionStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-
     r"""The current authorization status of the data connection."""
     additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})
-
     connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})
-
     data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})
-
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataConnectionError:
     
     errored_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('erroredOnUtc'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -30,13 +29,10 @@
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-
     status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-
     status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,21 +21,18 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpenseTransaction:
     
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
-
     r"""Currency the transaction was recorded in."""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-
     r"""Your unique identifier for the transaction."""
     issue_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issueDate') }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -49,18 +46,16 @@
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
     type: ExpenseTransactionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-
     r"""The type of transaction."""
     currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
-
     r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
     
     Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
     
     Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
     
     For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
@@ -78,16 +73,13 @@
     | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (USD) |
     | :--------------- | :------------- | :------------ | :------------------------- |
     | **GBP**          | £20            | 1.277         | $25.54                     |
     | **EUR**          | €20            | 1.134         | $22.68                     |
     | **RUB**          | ₽20            | 0.015         | $0.30                      |
     """
     lines: Optional[list[shared_expensetransactionline.ExpenseTransactionLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
-
     r"""Array of transaction lines."""
     merchant_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('merchantName'), 'exclude': lambda f: f is None }})
-
     r"""Name of the merchant where the purchase took place"""
     notes: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
-
     r"""Any private, company notes about the transaction."""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ExpenseTransactionLine:
     
     account_ref: shared_recordref.RecordRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef') }})
-
     net_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('netAmount') }})
-
     r"""Amount of the line, exclusive of tax."""
     tax_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount') }})
-
     r"""Amount of tax for the line."""
     tax_rate_ref: Optional[shared_recordref.RecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})
-
     tracking_refs: Optional[list[shared_recordref.RecordRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingRefs'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/hallink.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class HalLink:
     
     href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,15 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class MappingOptions:
     r"""Success"""
     
     accounts: Optional[list[shared_accountmappinginfo.AccountMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-
     r"""Array of available accounts for mapping."""
     expense_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expenseProvider'), 'exclude': lambda f: f is None }})
-
     r"""Name of the expense integration."""
     tax_rates: Optional[list[shared_taxratemappinginfo.TaxRateMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
-
     r"""Array of available tax rates for mapping."""
     tracking_categories: Optional[list[shared_trackingcategorymappinginfo.TrackingCategoryMappingInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingCategories'), 'exclude': lambda f: f is None }})
-
     r"""Array of available tracking categories for mapping."""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostSync:
     
     dataset_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetIds'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,10 +8,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class RecordRef:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""identifier of linked reference from mapping options."""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,10 +8,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Supplier:
     
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""id of the supplier for all purchases to be associated to"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SyncInitiated:
     r"""Returns the newly created SyncId"""
     
     sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncId'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,19 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TaxRateMappingInfo:
     
     code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
-
     r"""Code for the tax rate from the accounting platform."""
     effective_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('effectiveTaxRate'), 'exclude': lambda f: f is None }})
-
     r"""Effective tax rate."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""Unique identifier of tax rate."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-
     r"""Name of the tax rate in the accounting platform."""
     total_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalTaxRate'), 'exclude': lambda f: f is None }})
-
     r"""Total (not compounded) sum of the components of a tax rate."""
     valid_transaction_types: Optional[list[TaxRateMappingInfoValidTransactionTypesEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validTransactionTypes'), 'exclude': lambda f: f is None }})
-
     r"""Supported transaction types for the account."""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,18 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackingCategoryMappingInfo:
     
     has_children: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasChildren'), 'exclude': lambda f: f is None }})
-
     r"""Boolean of whether the tracking category has child categories."""
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""Unique identifier of the tracking category."""
     modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
-
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
     
@@ -36,13 +33,11 @@
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
     """
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-
     r"""Name of the tracking category as it appears in the accounting software."""
     parent_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentId'), 'exclude': lambda f: f is None }})
-
     r"""ID of the parent tracking category"""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionMetadata:
     
     integration_type: Optional[shared_integrationtype_enum.IntegrationTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationType'), 'exclude': lambda f: f is None }})
-
     r"""Type of transaction that has been processed e.g. Expense or Bank Feed."""
     message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-
     r"""Metadata such as validation errors or the resulting record created in the accounting software."""
     status: Optional[shared_transactionstatus_enum.TransactionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-
     r"""Status of the transaction."""
     transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
-
     r"""Your unique idenfier of the transaction."""
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,32 +10,23 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionMetadataListLinks:
     
     current: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
-
     self_: shared_hallink.HalLink = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
-
     next: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-
     previous: Optional[shared_hallink.HalLink] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionMetadataList:
     r"""Success"""
     
     links: TransactionMetadataListLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-
     page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-
     total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-
     results: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
-
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     transaction_status: TransactionStatus
     r"""Retrieve the status of transactions within a sync."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.13.1"
-    _gen_version: str = "2.23.1"
+    _sdk_version: str = "0.15.3"
+    _gen_version: str = "2.26.3"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def intiate_sync(self, request: operations.IntiateSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.IntiateSyncResponse:
         r"""Initiate sync
         Initiate sync of pending transactions.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.IntiateSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs', request)
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def get_last_successful_sync(self, request: operations.GetLastSuccessfulSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLastSuccessfulSyncResponse:
         r"""Last successful sync
         Gets the status of the last successfull sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLastSuccessfulSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/lastSuccessful/status', request)
@@ -54,14 +55,15 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
                 res.company_sync_status = out
 
         return res
 
+    
     def get_latest_sync(self, request: operations.GetLatestSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLatestSyncResponse:
         r"""Latest sync status
         Gets the latest sync status
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLatestSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/latest/status', request)
@@ -90,14 +92,15 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
                 res.company_sync_status = out
 
         return res
 
+    
     def get_sync_by_id(self, request: operations.GetSyncByIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncByIDResponse:
         r"""Get Sync status
         Get the sync status for a specified sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncByIDRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/status', request)
@@ -126,14 +129,15 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
                 res.company_sync_status = out
 
         return res
 
+    
     def list_syncs(self, request: operations.ListSyncsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncsResponse:
         r"""List sync statuses
         Gets a list of sync statuses
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/list/status', request)
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/transaction_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def get_sync_transaction(self, request: operations.GetSyncTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncTransactionResponse:
         r"""Get Sync Transaction
         Gets the status of a transaction for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
@@ -54,14 +55,15 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[list[shared.TransactionMetadata]])
                 res.transaction_metadata = out
 
         return res
 
+    
     def list_sync_transactions(self, request: operations.ListSyncTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncTransactionsResponse:
         r"""Get Sync transactions
         Get's the transactions and status for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
```

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.13.1/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,16 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
+def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
+                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
     path_param_fields: Tuple[Field, ...] = fields(clazz)
     for field in path_param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
@@ -229,15 +230,16 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[str, list[str]]:
+def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
+    str, list[str]]:
     params: dict[str, list[str]] = {}
 
     param_fields: Tuple[Field, ...] = fields(clazz)
     for field in param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
@@ -263,16 +265,19 @@
                     params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
-                params = params | _get_form_query_params(
-                    metadata, f_name, value)
+                params = params | _get_delimited_query_params(
+                    metadata, f_name, value, ",")
+            elif style == 'pipeDelimited':
+                params = params | _get_delimited_query_params(
+                    metadata, f_name, value, "|")
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -323,20 +328,23 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
+                        _val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -364,48 +372,52 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
+def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, array_delimiter: str) -> dict[
+    str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, array_delimiter)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json':      'application/json',
-    'form':      'application/x-www-form-urlencoded',
+    'json': 'application/json',
+    'form': 'application/x-www-form-urlencoded',
     'multipart': 'multipart/form-data',
-    'raw':       'application/octet-stream',
-    'string':    'text/plain',
+    'raw': 'application/octet-stream',
+    'string': 'text/plain',
 }
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[str, any, any]:
+def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
+    str, any, any]:
     if request is None:
         return None, None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method], request)
+        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+                                      request)
 
     request_val = getattr(request, request_field_name)
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
             request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is None:
         raise Exception('invalid request type')
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'), request_val)
+    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
+                                  request_val)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -470,15 +482,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-        str, list[str]]:
+    str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,15 +522,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name)
+                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -532,15 +544,16 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, array_delimiter: str) -> \
+        dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -587,15 +600,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [','.join([str(item) for item in items])]
+            params[field_name] = [array_delimiter.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
@@ -727,15 +740,15 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return val.value
+        return str(val.value)
 
     return str(val)
 
 
 def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
     if value is None and gbls is not None:
         if 'parameters' in gbls:
```

