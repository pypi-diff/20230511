# Comparing `tmp/codat-sync-for-commerce-0.12.3.tar.gz` & `tmp/codat-sync-for-commerce-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-commerce-0.12.3.tar", last modified: Thu May 11 20:38:32 2023, max compression
+gzip compressed data, was "codat-sync-for-commerce-0.9.0.tar", last modified: Wed Apr 26 15:03:44 2023, max compression
```

## Comparing `codat-sync-for-commerce-0.12.3.tar` & `codat-sync-for-commerce-0.9.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.253296 codat-sync-for-commerce-0.12.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 20:38:32.253296 codat-sync-for-commerce-0.12.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3065 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:38:32.253296 codat-sync-for-commerce-0.12.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.237296 codat-sync-for-commerce-0.12.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.241296 codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 20:38:32.000000 codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-11 20:38:32.000000 codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:38:32.000000 codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 20:38:32.000000 codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:38:32.000000 codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.241296 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8928 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/company_management.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4973 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3862 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.241296 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.245296 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/create_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      914 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/create_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      621 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      803 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_integration_branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1264 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_sync_flow_url.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      621 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      953 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_visible_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/list_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1744 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/list_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/list_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/request_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/request_sync_for_date_range.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      803 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/set_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/update_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.253296 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/accountoption.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1449 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/branding.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/brandingbutton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/brandingimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/brandinglogo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4153 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/configaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5383 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1182 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/createcompany.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/datatypefeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/daterange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/featurestate_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/featuretype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/fees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/feessupplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      914 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/groupinglevels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/groupingperiod.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/halref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      804 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/imagereference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3204 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/invoicelevelselection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/invoicelinelevelselection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      878 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/invoicestatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/localization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/newpayments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/newtaxrates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      760 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/option.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      859 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2184 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/sales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/sourcetype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/supportedfeature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/syncflowurl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3834 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/syncsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1431 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/synctolatestargs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/taxrateamount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      976 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/taxratemapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/updateconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      611 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/visibleaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4640 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8953 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/sync_flow_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:38:32.253296 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25963 2023-05-11 20:38:14.000000 codat-sync-for-commerce-0.12.3/src/codatsynccommerce/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3066 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.155307 codat-sync-for-commerce-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.155307 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 15:03:44.000000 codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8903 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/company_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3852 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.159307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      580 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      926 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      827 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_integration_branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1278 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_flow_url.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      965 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_visible_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1762 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1634 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/set_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1021 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/accountoption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1455 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/branding.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingbutton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandinglogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5409 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/createcompany.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2694 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/datatypefeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2503 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/daterange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/featurestate_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/featuretype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/fees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1005 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/feessupplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupinglevels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupingperiod.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/halref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/imagereference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3226 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelevelselection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicestatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/localization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1870 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newtaxrates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      764 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/option.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sourcetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/supportedfeature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncflowurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/synctolatestargs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxrateamount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxratemapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/updateconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/visibleaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4630 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8928 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync_flow_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:03:44.163307 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-26 15:03:34.000000 codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/utils.py
```

### Comparing `codat-sync-for-commerce-0.12.3/PKG-INFO` & `codat-sync-for-commerce-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-commerce
-Version: 0.12.3
+Version: 0.9.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -29,16 +29,17 @@
 
 s = codatsynccommerce.CodatSyncCommerce(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
+
 req = shared.CreateCompany(
-    name='Bob's Burgers',
+    name="Bob's Burgers",
 )
 
 res = s.company_management.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
```

### Comparing `codat-sync-for-commerce-0.12.3/README.md` & `codat-sync-for-commerce-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 
 s = codatsynccommerce.CodatSyncCommerce(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
+
 req = shared.CreateCompany(
-    name='Bob's Burgers',
+    name="Bob's Burgers",
 )
 
 res = s.company_management.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
```

### Comparing `codat-sync-for-commerce-0.12.3/setup.py` & `codat-sync-for-commerce-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-commerce",
-    version="0.12.3",
+    version="0.9.0",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/PKG-INFO` & `codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-commerce
-Version: 0.12.3
+Version: 0.9.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -29,16 +29,17 @@
 
 s = codatsynccommerce.CodatSyncCommerce(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
+
 req = shared.CreateCompany(
-    name='Bob's Burgers',
+    name="Bob's Burgers",
 )
 
 res = s.company_management.create_company(req)
 
 if res.company is not None:
     # handle response
 ```
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codat_sync_for_commerce.egg-info/SOURCES.txt` & `codat-sync-for-commerce-0.9.0/src/codat_sync_for_commerce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/company_management.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/company_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def create_company(self, request: shared.CreateCompany, retries: Optional[utils.RetryConfig] = None) -> operations.CreateCompanyResponse:
         r"""Create Sync for Commerce company
         Creates a Codat company with a commerce partner data connection.
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/meta/companies/sync'
@@ -59,15 +58,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Company])
                 res.company = out
 
         return res
 
-    
     def create_connection(self, request: operations.CreateConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateConnectionResponse:
         r"""Create connection
         Create a data connection for company.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateConnectionRequest, base_url, '/meta/companies/{companyId}/connections', request)
@@ -100,15 +98,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
 
         return res
 
-    
     def list_companies(self, request: operations.ListCompaniesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListCompaniesResponse:
         r"""List companies
         Retrieve a list of all companies the client has created.
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/meta/companies'
@@ -138,15 +135,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Companies])
                 res.companies = out
 
         return res
 
-    
     def list_connections(self, request: operations.ListConnectionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListConnectionsResponse:
         r"""List data connections
         Retrieve previously created data connections.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListConnectionsRequest, base_url, '/meta/companies/{companyId}/connections', request)
@@ -176,15 +172,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connections])
                 res.connections = out
 
         return res
 
-    
     def update_connection(self, request: operations.UpdateConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateConnectionResponse:
         r"""Update data connection
         Update a data connection
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateConnectionRequest, base_url, '/meta/companies/{companyId}/connections/{connectionId}', request)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def get_configuration(self, request: operations.GetConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetConfigurationResponse:
         r"""Retrieve config preferences set for a company.
         Retrieve current config preferences.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetConfigurationRequest, base_url, '/config/companies/{companyId}/sync/commerce', request)
@@ -55,15 +54,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Configuration])
                 res.configuration = out
 
         return res
 
-    
     def get_sync_status(self, request: operations.GetSyncStatusRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncStatusResponse:
         r"""Get status for a company's syncs
         Check the sync history and sync status for a company.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncStatusRequest, base_url, '/meta/companies/{companyId}/sync/commerce/status', request)
@@ -88,15 +86,14 @@
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetSyncStatusResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
-    
     def set_configuration(self, request: operations.SetConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.SetConfigurationResponse:
         r"""Create or update configuration.
         Make changes to configuration preferences.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.SetConfigurationRequest, base_url, '/config/companies/{companyId}/sync/commerce', request)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/integrations.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/integrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def get_integration_branding(self, request: operations.GetIntegrationBrandingRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetIntegrationBrandingResponse:
         r"""Get branding for an integration
         Retrieve Integration branding assets.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetIntegrationBrandingRequest, base_url, '/config/integrations/{platformKey}/branding', request)
@@ -55,15 +54,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Branding])
                 res.branding = out
 
         return res
 
-    
     def list_integrations(self, request: operations.ListIntegrationsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListIntegrationsResponse:
         r"""List information on Codat's supported integrations
         Retrieve a list of available integrations support by datatype and state of release.
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/config/integrations'
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/__init__.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/create_company.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import company as shared_company
+from ..shared import localization as shared_localization
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateCompanyResponse:
+class GetConfigTextSyncFlowResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    company: Optional[shared_company.Company] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/create_connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/create_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ..shared import connection as shared_connection
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateConnectionRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    request_body: Optional[str] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[str] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class CreateConnectionResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_config_text_sync_flow.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_config_text_sync_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dataclasses
 import requests as requests_http
 from ..shared import localization as shared_localization
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetConfigTextSyncFlowResponse:
+class UpdateConfigTextSyncFlowResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     localization_info: Optional[dict[str, shared_localization.Localization]] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from ..shared import configuration as shared_configuration
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetConfigurationRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GetConfigurationResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_integration_branding.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_integration_branding.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetIntegrationBrandingRequest:
     
     platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
-    r"""PlatformKey"""
+    r"""PlatformKey"""  
     
 
 @dataclasses.dataclass
 class GetIntegrationBrandingResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     branding: Optional[shared_branding.Branding] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_sync_flow_url.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_companies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import syncflowurl as shared_syncflowurl
+from ..shared import companies as shared_companies
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetSyncFlowURLRequest:
+class ListCompaniesRequest:
     
-    accounting_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountingKey', 'style': 'simple', 'explode': False }})
-    r"""Accounting platform key"""
-    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})
-    r"""Commerce platform key"""
-    merchant_identifier: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'merchantIdentifier', 'style': 'form', 'explode': True }})
-    r"""Identifier for your merchant, can be the merchant name or Codat company id."""
+    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+    order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
+    page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+    query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
 @dataclasses.dataclass
-class GetSyncFlowURLResponse:
+class ListCompaniesResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    sync_flow_url: Optional[shared_syncflowurl.SyncFlowURL] = dataclasses.field(default=None)
-    r"""Success"""
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    companies: Optional[shared_companies.Companies] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_sync_status.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_sync_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetSyncStatusRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GetSyncStatusResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/get_visible_accounts.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/get_visible_accounts.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ..shared import visibleaccounts as shared_visibleaccounts
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetVisibleAccountsRequest:
     
-    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
-    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})
+    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})  
+    platform_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'platformKey', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GetVisibleAccountsResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
-    r"""Success"""
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/list_companies.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_connections.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import companies as shared_companies
+from ..shared import connections as shared_connections
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListCompaniesRequest:
+class ListConnectionsRequest:
     
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
 @dataclasses.dataclass
-class ListCompaniesResponse:
+class ListConnectionsResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    companies: Optional[shared_companies.Companies] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    connections: Optional[shared_connections.Connections] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/list_connections.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/list_integrations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import connections as shared_connections
+from ..shared import integrations as shared_integrations
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListConnectionsRequest:
+class ListIntegrationsRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
 @dataclasses.dataclass
-class ListConnectionsResponse:
+class ListIntegrationsResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    connections: Optional[shared_connections.Connections] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    integrations: Optional[shared_integrations.Integrations] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/request_sync.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from ..shared import synctolatestargs as shared_synctolatestargs
 from typing import Optional
 
 
 @dataclasses.dataclass
 class RequestSyncRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    sync_to_latest_args: Optional[shared_synctolatestargs.SyncToLatestArgs] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    sync_to_latest_args: Optional[shared_synctolatestargs.SyncToLatestArgs] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class RequestSyncResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
-    r"""Success"""
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/request_sync_for_date_range.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/request_sync_for_date_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from ..shared import syncsummary as shared_syncsummary
 from typing import Optional
 
 
 @dataclasses.dataclass
 class RequestSyncForDateRangeRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    date_range: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    date_range: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class RequestSyncForDateRangeResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     sync_summary: Optional[shared_syncsummary.SyncSummary] = dataclasses.field(default=None)
-    r"""Success"""
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/set_configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/set_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from ..shared import configuration as shared_configuration
 from typing import Optional
 
 
 @dataclasses.dataclass
 class SetConfigurationRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class SetConfigurationResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     configuration: Optional[shared_configuration.Configuration] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/update_connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from ..shared import updateconnection as shared_updateconnection
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UpdateConnectionRequest:
     
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    update_connection: Optional[shared_updateconnection.UpdateConnection] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    update_connection: Optional[shared_updateconnection.UpdateConnection] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class UpdateConnectionResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     connection: Optional[shared_connection.Connection] = dataclasses.field(default=None)
-    r"""Success"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/operations/update_visible_accounts_sync_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ..shared import visibleaccounts as shared_visibleaccounts
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UpdateVisibleAccountsSyncFlowRequest:
     
-    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})
-    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    commerce_key: str = dataclasses.field(metadata={'path_param': { 'field_name': 'commerceKey', 'style': 'simple', 'explode': False }})  
+    visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class UpdateVisibleAccountsSyncFlowResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     visible_accounts: Optional[shared_visibleaccounts.VisibleAccounts] = dataclasses.field(default=None)
-    r"""Success"""
+    r"""Success"""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/__init__.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/accountoption.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/accountoption.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AccountOption:
     
     classification: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('classification'), 'exclude': lambda f: f is None }})
-    r"""Classification of the type of G/L account."""
+    r"""Classification of the type of G/L account."""  
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Identifier for the account, unique for the company."""
+    r"""Identifier for the account, unique for the company."""  
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name of the account."""
+    r"""Name of the account."""  
     nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})
-    r"""Reference given to each nominal account for a business. It ensures money is allocated to the correct account. This code isn't a unique identifier in the Codat system."""
+    r"""Reference given to each nominal account for a business. It ensures money is allocated to the correct account. This code isn't a unique identifier in the Codat system."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/branding.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/branding.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Branding:
     r"""Success"""
     
     button: Optional[shared_brandingbutton.BrandingButton] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('button'), 'exclude': lambda f: f is None }})
-    r"""Button branding references."""
+    r"""Button branding references."""  
     logo: Optional[shared_brandinglogo.BrandingLogo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logo'), 'exclude': lambda f: f is None }})
-    r"""Logo branding references."""
+    r"""Logo branding references."""  
     source_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId'), 'exclude': lambda f: f is None }})
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/brandingbutton.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingbutton.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingButton:
     r"""Button branding references."""
     
-    default: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})
-    hover: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hover'), 'exclude': lambda f: f is None }})
+    default: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})  
+    hover: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hover'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/brandingimage.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandingimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingImage:
     
     image: Optional[shared_imagereference.ImageReference] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('image'), 'exclude': lambda f: f is None }})
-    r"""Image reference."""
+    r"""Image reference."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/brandinglogo.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/brandinglogo.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BrandingLogo:
     r"""Logo branding references."""
     
-    full: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('full'), 'exclude': lambda f: f is None }})
-    square: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('square'), 'exclude': lambda f: f is None }})
+    full: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('full'), 'exclude': lambda f: f is None }})  
+    square: Optional[shared_brandingimage.BrandingImage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('square'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/companies.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integrations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import company as shared_company
+from ..shared import integration as shared_integration
 from ..shared import links as shared_links
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Companies:
+class Integrations:
     r"""Success"""
     
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[shared_company.Company]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/company.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Company:
     r"""A company in Codat represent a small or medium sized business, whose data you wish to share"""
     
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique identifier for your SMB in Codat."""
+    r"""Unique identifier for your SMB in Codat."""  
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""The name of the company"""
+    r"""The name of the company"""  
     redirect: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('redirect') }})
-    r"""The `redirect` [Link URL](https://docs.codat.io/auth-flow/authorize-hosted-link) enabling the customer to start their auth flow journey for the company."""
+    r"""The `redirect` [Link URL](https://docs.codat.io/auth-flow/authorize-hosted-link) enabling the customer to start their auth flow journey for the company."""  
     created: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -35,19 +35,19 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    created_by_user_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdByUserName'), 'exclude': lambda f: f is None }})
-    data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})
+    """  
+    created_by_user_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdByUserName'), 'exclude': lambda f: f is None }})  
+    data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})  
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""Additional information about the company. This can be used to store foreign IDs, references, etc."""
+    r"""Additional information about the company. This can be used to store foreign IDs, references, etc."""  
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -60,10 +60,10 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})
+    """  
+    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/configaccount.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configaccount.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConfigAccount:
     r"""G/L account object for configuration."""
     
     account_options: Optional[list[shared_accountoption.AccountOption]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountOptions'), 'exclude': lambda f: f is None }})
-    r"""Object containing account options."""
+    r"""Object containing account options."""  
     description_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptionText'), 'exclude': lambda f: f is None }})
-    r"""Descriprtive text for sales configuration section."""
+    r"""Descriprtive text for sales configuration section."""  
     label_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('labelText'), 'exclude': lambda f: f is None }})
-    r"""Label text for sales configuration section."""
+    r"""Label text for sales configuration section."""  
     required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})
-    r"""Required section to be configured for sync."""
+    r"""Required section to be configured for sync."""  
     selected_account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedAccountId'), 'exclude': lambda f: f is None }})
-    r"""Selected account id from the list of available accounts."""
+    r"""Selected account id from the list of available accounts."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/configuration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Configuration:
     r"""Success"""
     
-    fees: Optional[shared_fees.Fees] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fees'), 'exclude': lambda f: f is None }})
-    new_payments: Optional[shared_newpayments.NewPayments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newPayments'), 'exclude': lambda f: f is None }})
-    payments: Optional[shared_payments.Payments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payments'), 'exclude': lambda f: f is None }})
-    sales: Optional[shared_sales.Sales] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sales'), 'exclude': lambda f: f is None }})
+    fees: Optional[shared_fees.Fees] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fees'), 'exclude': lambda f: f is None }})  
+    new_payments: Optional[shared_newpayments.NewPayments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newPayments'), 'exclude': lambda f: f is None }})  
+    payments: Optional[shared_payments.Payments] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payments'), 'exclude': lambda f: f is None }})  
+    sales: Optional[shared_sales.Sales] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sales'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/connection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,32 +39,32 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """  
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique identifier for a company's data connection."""
+    r"""Unique identifier for a company's data connection."""  
     integration_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
-    r"""A Codat ID representing the integration."""
+    r"""A Codat ID representing the integration."""  
     integration_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationKey') }})
-    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""
-    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})
-    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})
+    r"""A unique four-character ID that identifies the platform of the company's data connection. This ensures continuity if the platform changes its name in the future."""  
+    link_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkUrl') }})  
+    platform_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformName') }})  
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
     source_type: ConnectionSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    r"""The type of platform of the connection."""
+    r"""The type of platform of the connection."""  
     status: shared_dataconnectionstatus_enum.DataConnectionStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    r"""The current authorization status of the data connection."""
-    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})
-    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})
-    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})
+    r"""The current authorization status of the data connection."""  
+    additional_properties: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additionalProperties'), 'exclude': lambda f: f is None }})  
+    connection_info: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionInfo'), 'exclude': lambda f: f is None }})  
+    data_connection_errors: Optional[list[shared_dataconnectionerror.DataConnectionError]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionErrors'), 'exclude': lambda f: f is None }})  
     last_sync: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastSync'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -77,9 +77,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/connections.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/connections.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Connections:
     r"""Success"""
     
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
+    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
+    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
+    results: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/createcompany.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/createcompany.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateCompany:
     
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""Name of the company in Codat with a partner-commerce data connection."""
+    r"""Name of the company in Codat with a partner-commerce data connection."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/customer.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Customer:
     
     customer_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerOptions'), 'exclude': lambda f: f is None }})
-    r"""List of customer options from the list of customer records on the accounting software."""
+    r"""List of customer options from the list of customer records on the accounting software."""  
     selected_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedCustomerId'), 'exclude': lambda f: f is None }})
-    r"""Selected customer id from the list of customer records on the accounting software."""
+    r"""Selected customer id from the list of customer records on the accounting software."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/dataconnectionerror.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/dataconnectionerror.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
+    """  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    status_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})  
+    status_text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusText'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/datatypefeature.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/datatypefeature.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,11 +55,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DataTypeFeature:
     r"""Describes support for a given datatype and associated operations"""
     
-    supported_features: list[shared_supportedfeature.SupportedFeature] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supportedFeatures') }})
+    supported_features: list[shared_supportedfeature.SupportedFeature] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supportedFeatures') }})  
     data_type: Optional[DataTypeFeatureDataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    r"""Available Data types"""
+    r"""Available Data types"""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/daterange.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/daterange.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """  
     start: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -48,9 +48,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/fees.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/fees.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Fees:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-    fees_supplier: Optional[shared_feessupplier.FeesSupplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feesSupplier'), 'exclude': lambda f: f is None }})
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    fees_supplier: Optional[shared_feessupplier.FeesSupplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feesSupplier'), 'exclude': lambda f: f is None }})  
     sync_fees: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncFees'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator to enable syncing fees."""
+    r"""Boolean indicator to enable syncing fees."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/feessupplier.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/feessupplier.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class FeesSupplier:
     
     selected_supplier_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedSupplierId'), 'exclude': lambda f: f is None }})
-    r"""Selected supplier id from the list of supplier records on the accounting software."""
+    r"""Selected supplier id from the list of supplier records on the accounting software."""  
     supplier_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierOptions'), 'exclude': lambda f: f is None }})
-    r"""List of supplier options from the list of supplier records on the accounting software."""
+    r"""List of supplier options from the list of supplier records on the accounting software."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/grouping.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Grouping:
     
-    grouping_levels: Optional[shared_groupinglevels.GroupingLevels] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingLevels'), 'exclude': lambda f: f is None }})
-    grouping_period: Optional[shared_groupingperiod.GroupingPeriod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriod'), 'exclude': lambda f: f is None }})
+    grouping_levels: Optional[shared_groupinglevels.GroupingLevels] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingLevels'), 'exclude': lambda f: f is None }})  
+    grouping_period: Optional[shared_groupingperiod.GroupingPeriod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriod'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/groupinglevels.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupinglevels.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GroupingLevels:
     
-    invoice_level: Optional[shared_invoicelevelselection.InvoiceLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLevel'), 'exclude': lambda f: f is None }})
-    invoice_line_level: Optional[shared_invoicelinelevelselection.InvoiceLineLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLineLevel'), 'exclude': lambda f: f is None }})
+    invoice_level: Optional[shared_invoicelevelselection.InvoiceLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLevel'), 'exclude': lambda f: f is None }})  
+    invoice_line_level: Optional[shared_invoicelinelevelselection.InvoiceLineLevelSelection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceLineLevel'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/groupingperiod.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/groupingperiod.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GroupingPeriod:
     
     grouping_period_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupingPeriodOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of grouping period options."""
+    r"""Array of grouping period options."""  
     selected_grouping_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupingPeriod'), 'exclude': lambda f: f is None }})
-    r"""Grouping period i.e. Daily sales."""
+    r"""Grouping period i.e. Daily sales."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/halref.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/halref.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class HalRef:
     
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
+    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/imagereference.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/imagereference.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ImageReference:
     r"""Image reference."""
     
     alt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alt'), 'exclude': lambda f: f is None }})
-    r"""Alternative text when image is not available."""
+    r"""Alternative text when image is not available."""  
     src: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('src'), 'exclude': lambda f: f is None }})
-    r"""Source URL for image."""
+    r"""Source URL for image."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/integration.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Integration:
     r"""An integration that Codat supports"""
     
     enabled: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('enabled') }})
-    r"""Whether this integration is enabled for your customers to use"""
+    r"""Whether this integration is enabled for your customers to use"""  
     key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-    r"""A unique 4-letter key to represent a platform in each integration. View [accounting](https://docs.codat.io/integrations/accounting/accounting-platform-keys), [banking](https://docs.codat.io/integrations/banking/banking-platform-keys), and [commerce](https://docs.codat.io/integrations/commerce/commerce-platform-keys) platform keys."""
-    logo_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logoUrl') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    data_provided_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataProvidedBy'), 'exclude': lambda f: f is None }})
-    datatype_features: Optional[list[shared_datatypefeature.DataTypeFeature]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datatypeFeatures'), 'exclude': lambda f: f is None }})
+    r"""A unique 4-letter key to represent a platform in each integration. View [accounting](https://docs.codat.io/integrations/accounting/accounting-platform-keys), [banking](https://docs.codat.io/integrations/banking/banking-platform-keys), and [commerce](https://docs.codat.io/integrations/commerce/commerce-platform-keys) platform keys."""  
+    logo_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logoUrl') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    data_provided_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataProvidedBy'), 'exclude': lambda f: f is None }})  
+    datatype_features: Optional[list[shared_datatypefeature.DataTypeFeature]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datatypeFeatures'), 'exclude': lambda f: f is None }})  
     integration_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
-    r"""A Codat ID representing the integration."""
-    is_beta: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBeta'), 'exclude': lambda f: f is None }})
-    is_offline_connector: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isOfflineConnector'), 'exclude': lambda f: f is None }})
+    r"""A Codat ID representing the integration."""  
+    is_beta: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBeta'), 'exclude': lambda f: f is None }})  
+    is_offline_connector: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isOfflineConnector'), 'exclude': lambda f: f is None }})  
     source_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId'), 'exclude': lambda f: f is None }})
-    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""
+    r"""A source-specific ID used to distinguish between different sources originating from the same data connection. In general, a data connection is a single data source. However, for TrueLayer, `sourceId` is associated with a specific bank and has a many-to-one relationship with the `integrationId`."""  
     source_type: Optional[shared_sourcetype_enum.SourceTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType'), 'exclude': lambda f: f is None }})
-    r"""The type of platform of the connection."""
+    r"""The type of platform of the connection."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/integrations.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/links.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import integration as shared_integration
-from ..shared import links as shared_links
+from ..shared import halref as shared_halref
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Integrations:
-    r"""Success"""
+class Links:
     
-    links: shared_links.Links = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+    current: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})  
+    self_: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})  
+    next: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})  
+    previous: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/invoicelevelselection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelevelselection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InvoiceLevelSelection:
     
     group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Options for grouping sales."""
+    r"""Options for grouping sales."""  
     selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Selected array of grouping options."""
+    r"""Selected array of grouping options."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/invoicelinelevelselection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/option.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceLineLevelSelection:
+class Option:
     
-    group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Options for grouping on invoice lines."""
-    selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
-    r"""Invoice line level selection."""
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for the option."""  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Name value of the option."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/invoicestatus.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicestatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InvoiceStatus:
     
     invoice_status_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatusOptions'), 'exclude': lambda f: f is None }})
-    r"""Options for invoice statuses."""
+    r"""Options for invoice statuses."""  
     selected_invoice_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedInvoiceStatus'), 'exclude': lambda f: f is None }})
-    r"""Selected option for invoice status for invoice to be synced."""
+    r"""Selected option for invoice status for invoice to be synced."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/links.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/localization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import halref as shared_halref
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Links:
+class Localization:
     
-    current: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
-    self_: shared_halref.HalRef = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
-    next: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[shared_halref.HalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+    required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})  
+    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
+    r"""Value of the property."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/localization.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxrateamount.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import option as shared_option
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Localization:
+class TaxRateAmount:
     
-    required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required'), 'exclude': lambda f: f is None }})
-    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
-    r"""Value of the property."""
+    selected_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedTaxRateId'), 'exclude': lambda f: f is None }})
+    r"""Selected tax rate id from the list of tax rates on the accounting software."""  
+    tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateOptions'), 'exclude': lambda f: f is None }})
+    r"""Array of tax rate options object."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/newpayments.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/payments.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class NewPayments:
+class Payments:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
     sync_payments: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncPayments'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator for syncing payments."""
+    r"""Boolean indicator for syncing sales."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/newtaxrates.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newtaxrates.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class NewTaxRates:
     
     accounting_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountingTaxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of accounting tax rate options."""
+    r"""Array of accounting tax rate options."""  
     commerce_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commerceTaxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of tax component options."""
+    r"""Array of tax component options."""  
     default_zero_tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultZeroTaxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Default zero tax rate selected for sync."""
+    r"""Default zero tax rate selected for sync."""  
     selected_default_zero_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedDefaultZeroTaxRateId'), 'exclude': lambda f: f is None }})
-    r"""Default tax rate selected for sync."""
+    r"""Default tax rate selected for sync."""  
     tax_rate_mappings: Optional[list[shared_taxratemapping.TaxRateMapping]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateMappings'), 'exclude': lambda f: f is None }})
-    r"""Array of tax component to rate mapppings."""
+    r"""Array of tax component to rate mapppings."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/option.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/updateconnection.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,12 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Option:
+class UpdateConnection:
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the option."""
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name value of the option."""
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    r"""The current authorization status of the data connection."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/payments.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/newpayments.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Payments:
+class NewPayments:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
     sync_payments: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncPayments'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator for syncing sales."""
+    r"""Boolean indicator for syncing payments."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/sales.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/sales.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Sales:
     
-    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
-    grouping: Optional[shared_grouping.Grouping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping'), 'exclude': lambda f: f is None }})
-    invoice_status: Optional[shared_invoicestatus.InvoiceStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatus'), 'exclude': lambda f: f is None }})
-    new_tax_rates: Optional[shared_newtaxrates.NewTaxRates] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newTaxRates'), 'exclude': lambda f: f is None }})
-    sales_customer: Optional[shared_customer.Customer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesCustomer'), 'exclude': lambda f: f is None }})
+    accounts: Optional[dict[str, shared_configaccount.ConfigAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})  
+    grouping: Optional[shared_grouping.Grouping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping'), 'exclude': lambda f: f is None }})  
+    invoice_status: Optional[shared_invoicestatus.InvoiceStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoiceStatus'), 'exclude': lambda f: f is None }})  
+    new_tax_rates: Optional[shared_newtaxrates.NewTaxRates] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newTaxRates'), 'exclude': lambda f: f is None }})  
+    sales_customer: Optional[shared_customer.Customer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesCustomer'), 'exclude': lambda f: f is None }})  
     sync_sales: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncSales'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator for syncing sales."""
-    tax_rates: Optional[dict[str, shared_taxrateamount.TaxRateAmount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
+    r"""Boolean indicator for syncing sales."""  
+    tax_rates: Optional[dict[str, shared_taxrateamount.TaxRateAmount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRates'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/supportedfeature.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/supportedfeature.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SupportedFeature:
     
-    feature_state: shared_featurestate_enum.FeatureStateEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureState') }})
-    feature_type: shared_featuretype_enum.FeatureTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureType') }})
+    feature_state: shared_featurestate_enum.FeatureStateEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureState') }})  
+    feature_type: shared_featuretype_enum.FeatureTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('featureType') }})
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/syncflowurl.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncflowurl.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SyncFlowURL:
     r"""Success"""
     
     url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
-    r"""Sync flow URL."""
+    r"""Sync flow URL."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/syncsummary.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/syncsummary.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SyncSummary:
     r"""Success"""
     
     commerce_sync_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commerceSyncId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for the sync in Codat."""
+    r"""Unique identifier for the sync in Codat."""  
     company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-    r"""Unique identifier for your SMB in Codat."""
+    r"""Unique identifier for your SMB in Codat."""  
     data_connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnections'), 'exclude': lambda f: f is None }})
-    r"""Array of containing objects data connection information for the company."""
+    r"""Array of containing objects data connection information for the company."""  
     data_pushed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataPushed'), 'exclude': lambda f: f is None }})
-    r"""Boolean indicator for data being pushed during a sync operation."""
+    r"""Boolean indicator for data being pushed during a sync operation."""  
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    r"""Friendly error message for the sync operation."""
-    sync_date_range_utc: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncDateRangeUtc'), 'exclude': lambda f: f is None }})
+    r"""Friendly error message for the sync operation."""  
+    sync_date_range_utc: Optional[shared_daterange.DateRange] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncDateRangeUtc'), 'exclude': lambda f: f is None }})  
     sync_exception_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncExceptionMessage'), 'exclude': lambda f: f is None }})
-    r"""Exception message for the sync operation."""
+    r"""Exception message for the sync operation."""  
     sync_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatus'), 'exclude': lambda f: f is None }})
-    r"""Status of the sync of the company data. This is linked to status code."""
+    r"""Status of the sync of the company data. This is linked to status code."""  
     sync_status_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncStatusCode'), 'exclude': lambda f: f is None }})
-    r"""Numerical status code sync of the company data."""
+    r"""Numerical status code sync of the company data."""  
     sync_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncUtc'), 'exclude': lambda f: f is None }})
     r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
     ```
     2020-10-08T22:40:50Z
     2021-01-01T00:00:00
     ```
@@ -47,9 +47,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/synctolatestargs.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/synctolatestargs.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,9 @@
     - Unqualified local time: `2021-11-15T01:00:00`
     - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
     > Time zones
     > 
     > Not all dates from Codat will contain information about time zones.  
     > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
-    """
+    """
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/taxrateamount.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/invoicelinelevelselection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import option as shared_option
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TaxRateAmount:
+class InvoiceLineLevelSelection:
     
-    selected_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedTaxRateId'), 'exclude': lambda f: f is None }})
-    r"""Selected tax rate id from the list of tax rates on the accounting software."""
-    tax_rate_options: Optional[list[shared_option.Option]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateOptions'), 'exclude': lambda f: f is None }})
-    r"""Array of tax rate options object."""
+    group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groupByOptions'), 'exclude': lambda f: f is None }})
+    r"""Options for grouping on invoice lines."""  
+    selected_group_by_options: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedGroupByOptions'), 'exclude': lambda f: f is None }})
+    r"""Invoice line level selection."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/taxratemapping.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/taxratemapping.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TaxRateMapping:
     
     selected_accounting_tax_rate_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedAccountingTaxRateId'), 'exclude': lambda f: f is None }})
-    r"""Selected tax rate id from the list of tax rates on the accounting software."""
+    r"""Selected tax rate id from the list of tax rates on the accounting software."""  
     selected_commerce_tax_rate_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('selectedCommerceTaxRateIds'), 'exclude': lambda f: f is None }})
-    r"""Selected tax component id from the list of tax components on the commerce software."""
+    r"""Selected tax component id from the list of tax components on the commerce software."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/models/shared/updateconnection.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/models/shared/visibleaccounts.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,12 +5,13 @@
 from codatsynccommerce import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UpdateConnection:
+class VisibleAccounts:
+    r"""Success"""
     
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""The current authorization status of the data connection."""
+    visible_accounts: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('visibleAccounts'), 'exclude': lambda f: f is None }})
+    r"""Visible accounts on sync flow."""
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/sdk.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     sync_flow_preferences: SyncFlowPreferences
     r"""Configure preferences for any given Sync for Commerce company using sync flow."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.12.3"
-    _gen_version: str = "2.26.3"
+    _sdk_version: str = "0.9.0"
+    _gen_version: str = "2.22.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/sync.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def request_sync(self, request: operations.RequestSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.RequestSyncResponse:
         r"""Run a Commerce sync from the last successful sync
         Run a Commerce sync from the last successful sync up to the date provided (optional), otherwise UtcNow is used.
         If there was no previously successful sync, the start date in the config is used.
         """
         base_url = self._server_url
         
@@ -60,15 +59,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.SyncSummary])
                 res.sync_summary = out
 
         return res
 
-    
     def request_sync_for_date_range(self, request: operations.RequestSyncForDateRangeRequest, retries: Optional[utils.RetryConfig] = None) -> operations.RequestSyncForDateRangeResponse:
         r"""Run a Commerce sync from a given date range
         Run a Commerce sync from the specified start date to the specified finish date in the request payload.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.RequestSyncForDateRangeRequest, base_url, '/meta/companies/{companyId}/sync/commerce/historic', request)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/sync_flow_preferences.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/sync_flow_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def get_config_text_sync_flow(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetConfigTextSyncFlowResponse:
         r"""Retrieve preferences for text fields on Sync Flow
         To enable retrieval of preferences set for the text fields on Sync Flow.
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/sync/commerce/config/ui/text'
@@ -55,15 +54,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[dict[str, shared.Localization]])
                 res.localization_info = out
 
         return res
 
-    
     def get_sync_flow_url(self, request: operations.GetSyncFlowURLRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncFlowURLResponse:
         r"""Retrieve sync flow url
         Get a URL for Sync Flow including a one time passcode.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncFlowURLRequest, base_url, '/config/sync/commerce/{commerceKey}/{accountingKey}/start', request)
@@ -93,15 +91,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.SyncFlowURL])
                 res.sync_flow_url = out
 
         return res
 
-    
     def get_visible_accounts(self, request: operations.GetVisibleAccountsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetVisibleAccountsResponse:
         r"""List visible accounts
         Enable retrieval for accounts which are visible on sync flow.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetVisibleAccountsRequest, base_url, '/clients/{clientId}/config/ui/accounts/platform/{platformKey}', request)
@@ -130,15 +127,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.VisibleAccounts])
                 res.visible_accounts = out
 
         return res
 
-    
     def update_config_text_sync_flow(self, request: dict[str, shared.Localization], retries: Optional[utils.RetryConfig] = None) -> operations.UpdateConfigTextSyncFlowResponse:
         r"""Update preferences for text fields on sync flow
         To enable update of preferences set for the text fields on sync flow.
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/sync/commerce/config/ui/text'
@@ -171,15 +167,14 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[dict[str, shared.Localization]])
                 res.localization_info = out
 
         return res
 
-    
     def update_visible_accounts_sync_flow(self, request: operations.UpdateVisibleAccountsSyncFlowRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UpdateVisibleAccountsSyncFlowResponse:
         r"""Update the visible accounts on Sync Flow
         To enable update of accounts visible preferences set on Sync Flow.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateVisibleAccountsSyncFlowRequest, base_url, '/sync/commerce/config/ui/accounts/platform/{commerceKey}', request)
```

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/utils/retries.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-commerce-0.12.3/src/codatsynccommerce/utils/utils.py` & `codat-sync-for-commerce-0.9.0/src/codatsynccommerce/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,15 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
-                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
+def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
     path_param_fields: Tuple[Field, ...] = fields(clazz)
     for field in path_param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
@@ -230,16 +229,15 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
-    str, list[str]]:
+def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     param_fields: Tuple[Field, ...] = fields(clazz)
     for field in param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
@@ -265,19 +263,16 @@
                     params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, ",")
-            elif style == 'pipeDelimited':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, "|")
+                params = params | _get_form_query_params(
+                    metadata, f_name, value)
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -328,23 +323,20 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -372,52 +364,48 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, array_delimiter: str) -> dict[
-    str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, array_delimiter)
+def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
+    'json':      'application/json',
+    'form':      'application/x-www-form-urlencoded',
     'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    'raw':       'application/octet-stream',
+    'string':    'text/plain',
 }
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
-    str, any, any]:
+def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[str, any, any]:
     if request is None:
         return None, None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request)
+        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method], request)
 
     request_val = getattr(request, request_field_name)
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
             request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is None:
         raise Exception('invalid request type')
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'), request_val)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -482,15 +470,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-    str, list[str]]:
+        str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -522,15 +510,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
+                        field_name, metadata.get('explode', True), val, _get_form_field_name)
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -544,16 +532,15 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, array_delimiter: str) -> \
-        dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -600,15 +587,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [array_delimiter.join([str(item) for item in items])]
+            params[field_name] = [','.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
@@ -740,15 +727,15 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return str(val.value)
+        return val.value
 
     return str(val)
 
 
 def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
     if value is None and gbls is not None:
         if 'parameters' in gbls:
```

