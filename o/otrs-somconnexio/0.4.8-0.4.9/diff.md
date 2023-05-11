# Comparing `tmp/otrs_somconnexio-0.4.8.tar.gz` & `tmp/otrs_somconnexio-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/otrs_somconnexio-0.4.8.tar", last modified: Tue Feb  9 17:11:12 2021, max compression
+gzip compressed data, was "dist/otrs_somconnexio-0.4.9.tar", last modified: Mon Mar 22 08:37:26 2021, max compression
```

## Comparing `otrs_somconnexio-0.4.8.tar` & `otrs_somconnexio-0.4.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/
--rw-rw-rw-   0 root         (0) root         (0)     2487 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/README.md
--rw-r--r--   0 root         (0) root         (0)     3719 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/
--rw-rw-rw-   0 root         (0) root         (0)     5747 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/client.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/user_management_client/
--rw-rw-rw-   0 root         (0) root         (0)     2522 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/user_management_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/user_management_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/user_management_client/user_management_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/process_ticket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/process_ticket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2474 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/process_ticket/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/process_ticket/internet.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/customer_user.py
--rw-rw-rw-   0 root         (0) root         (0)      885 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage_article.py
--rw-rw-rw-   0 root         (0) root         (0)     1190 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/ticket_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/customer_data.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/fiber_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     3984 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/internet_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1904 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/mobile_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/adsl_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/abstract_article.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/provision_article.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage/mm_fibre.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage/adsl.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage/vdf_fibre.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/telecom_company.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/mobile_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/adsl_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/provision_ticket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/configurations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/configurations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/configurations/fiber_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/configurations/mobile_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/configurations/adsl_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/fiber_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2137 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/provision_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1390 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1825 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/adsl_data.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/fiber_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/providers.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/mobile_data.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/vf_provisioning_article.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/responses/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/responses/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/responses/ticket_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/services/update_process_ticket_with_coverage_tickets_info_service.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/services/mapping_services.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/services/mapping_mobile_minutes.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/services/update_process_ticket_with_VF_provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/otrs_somconnexio/services/update_ticket_with_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     3719 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4577 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/data/otrs_raw_responses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/user_management_client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/user_management_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/user_management_client/test_user_management_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4562 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/user_management_client/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/otrs_models/
--rw-rw-rw-   0 root         (0) root         (0)     3771 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_fiber_ticket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/otrs_models/process_ticket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/process_ticket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4143 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/process_ticket/test_mobile_process_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     8413 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/process_ticket/test_internet_process_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)    16122 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_adsl_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5104 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_vf_provisioning_article.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_mobile_data.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_abstract_article.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/otrs_models/configuration/
--rw-rw-rw-   0 root         (0) root         (0)     1296 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/configuration/test_fiber_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/configuration/test_adsl_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/configuration/test_mobile_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_ticket_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_coverage_article.py
--rw-rw-rw-   0 root         (0) root         (0)     3785 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_adsl_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)    16049 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_fiber_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_telecom_company.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_adsl_data.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_coverage_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     3868 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_mobile_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)    10928 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_mobile_dynamic_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_customer_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/otrs_models/test_fiber_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/responses/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/responses/test_ticket_creation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/responses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/integration/test_change_customer_language.py
--rw-rw-rw-   0 root         (0) root         (0)     4970 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/integration/test_ticket_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/integration/test_update_ticket_with_coverage_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/tests/services/
--rw-rw-rw-   0 root         (0) root         (0)      844 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/services/test_mappint_services.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/services/test_update_process_ticket_with_coverage_tickets_info_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/services/test_update_process_ticket_with_VF_provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/services/test_update_ticket_with_provider_info.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/tests/services/test_mapping_mobile_minutes.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-09 17:11:12.000000 otrs_somconnexio-0.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2021-02-09 17:11:03.000000 otrs_somconnexio-0.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     3719 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/
+-rw-rw-rw-   0 root         (0) root         (0)     5747 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/client.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/user_management_client/
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/user_management_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/user_management_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/user_management_client/user_management_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/process_ticket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/process_ticket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/process_ticket/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/process_ticket/internet.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/customer_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      885 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage_article.py
+-rw-rw-rw-   0 root         (0) root         (0)     1190 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/ticket_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/customer_data.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/fiber_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     3984 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/internet_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/mobile_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/adsl_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/abstract_article.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/provision_article.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage/mm_fibre.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage/adsl.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage/vdf_fibre.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/telecom_company.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/mobile_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/adsl_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/provision_ticket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/configurations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/configurations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/configurations/fiber_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/configurations/mobile_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/configurations/adsl_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/fiber_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/provision_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/adsl_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/fiber_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)      716 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/mobile_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/vf_provisioning_article.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/responses/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/responses/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/responses/ticket_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      851 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/services/update_process_ticket_with_coverage_tickets_info_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/services/mapping_services.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/services/mapping_mobile_minutes.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/services/update_process_ticket_with_VF_provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/otrs_somconnexio/services/update_ticket_with_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     3719 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4577 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/data/otrs_raw_responses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/user_management_client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/user_management_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/user_management_client/test_user_management_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4562 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/user_management_client/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/otrs_models/
+-rw-rw-rw-   0 root         (0) root         (0)     4126 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_fiber_ticket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/otrs_models/process_ticket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/process_ticket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4143 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/process_ticket/test_mobile_process_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     8413 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/process_ticket/test_internet_process_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)    16121 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_adsl_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5104 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_vf_provisioning_article.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_mobile_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_abstract_article.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/otrs_models/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/configuration/test_fiber_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/configuration/test_adsl_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/configuration/test_mobile_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_ticket_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_coverage_article.py
+-rw-rw-rw-   0 root         (0) root         (0)     3841 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_adsl_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)    16048 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_fiber_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_telecom_company.py
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_adsl_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_coverage_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     3781 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_mobile_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)    10926 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_mobile_dynamic_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_customer_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/otrs_models/test_fiber_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/responses/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/responses/test_ticket_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/responses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/integration/test_change_customer_language.py
+-rw-rw-rw-   0 root         (0) root         (0)     4994 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/integration/test_ticket_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/integration/test_update_ticket_with_coverage_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/tests/services/
+-rw-rw-rw-   0 root         (0) root         (0)      844 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/services/test_mappint_services.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/services/test_update_process_ticket_with_coverage_tickets_info_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/services/test_update_process_ticket_with_VF_provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/services/test_update_ticket_with_provider_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/tests/services/test_mapping_mobile_minutes.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-03-22 08:37:26.000000 otrs_somconnexio-0.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2021-03-22 08:37:19.000000 otrs_somconnexio-0.4.9/setup.py
```

### Comparing `otrs_somconnexio-0.4.8/README.md` & `otrs_somconnexio-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/PKG-INFO` & `otrs_somconnexio-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otrs_somconnexio
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python package for Somconnexio data syncing in OTRS
 Home-page: https://gitlab.com/coopdevs/otrs_somconnexio
 Author: Coopdevs
 Author-email: info@coopdevs.org
 License: UNKNOWN
 Description: # Python 2.7/3.8 module to manage the SomConnexio's ERP integration with OTRS
```

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/client.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/client.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/user_management_client/client.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/user_management_client/client.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/user_management_client/user_management_response.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/user_management_client/user_management_response.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/process_ticket/mobile.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/process_ticket/mobile.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/process_ticket/internet.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/process_ticket/internet.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/customer_user.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/customer_user.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage_article.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage_article.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/ticket_factory.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/ticket_factory.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/fiber_ticket.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/fiber_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/internet_dynamic_fields.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/internet_dynamic_fields.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/mobile_dynamic_fields.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/mobile_dynamic_fields.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/adsl_dynamic_fields.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/adsl_dynamic_fields.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/coverage_ticket.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/coverage_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/telecom_company.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/telecom_company.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/mobile_ticket.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/mobile_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/adsl_ticket.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/adsl_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/provision_ticket.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/provision_ticket.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,17 @@
                 self.service_data.order_id
             ),
             "Type": self._ticket_type(),
             "Queue": self._ticket_queue(),
             "State": self._ticket_state(),
             "Priority": self._ticket_priority(),
             "CustomerUser": self._customer_id(),
-            "CustomerID": self._customer_id()
+            "CustomerID": self._customer_id(),
+            "Service": self._ticket_service(),
+            "SLA": self._ticket_SLA(),
         })
 
     def _build_article(self):
         provision_article = ProvisionArticle(
             self.service_type(),
             self.service_data.order_id
         )
@@ -55,9 +57,21 @@
 
     def _ticket_activity_id(self):
         return self.otrs_configuration.activity_id
 
     def _ticket_process_id(self):
         return self.otrs_configuration.process_id
 
+    def _ticket_service(self):
+        if hasattr(self.otrs_configuration, "service"):
+            return self.otrs_configuration.service
+        else:
+            return False
+
+    def _ticket_SLA(self):
+        if hasattr(self.otrs_configuration, "SLA"):
+            return self.otrs_configuration.SLA
+        else:
+            return False
+
     def _customer_id(self):
         return self.customer_data.id
```

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/configurations/mobile_ticket.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/configurations/mobile_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/configurations/adsl_ticket.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/configurations/adsl_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/fiber_data.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/fiber_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 class FiberData:
     type = 'fiber'
 
     def __init__(
-        self, order_id, phone_number, iban, service_address, service_city,
+        self, order_id, phone_number, iban, email, service_address, service_city,
         service_zip, service_subdivision, service_subdivision_code, shipment_address, shipment_city, shipment_zip,
         shipment_subdivision, previous_service, previous_provider, previous_internal_provider,
         previous_owner_vat, previous_owner_name, previous_owner_surname, notes,
             adsl_coverage, mm_fiber_coverage, vdf_fiber_coverage, change_address, product):
         # Common all the Tickets
         self.order_id = order_id
         self.phone_number = phone_number
         self.iban = iban
+        self.email = email
         self.previous_internal_provider = previous_internal_provider
         self.previous_provider = previous_provider
         self.previous_owner_vat = previous_owner_vat
         self.previous_owner_name = previous_owner_name
         self.previous_owner_surname = previous_owner_surname
 
         # Common Internet the Tickets
```

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/provision_dynamic_fields.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/provision_dynamic_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def _name(self):
         return DynamicField("cognom1", self.customer_data.name)
 
     def _vat_number(self):
         return DynamicField(name="NIFNIESoci", value=self.customer_data.vat_number)
 
     def _mail(self):
-        return DynamicField(name="correuElectronic", value=self.customer_data.email)
+        return DynamicField(name="correuElectronic", value=self.service_data.email)
 
     def _phone(self):
         return DynamicField(name="telefonContacte", value=self.customer_data.phone)
 
     def _iban(self):
         return DynamicField("IBAN", self.service_data.iban)
```

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/service.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/service.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/adsl_data.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/adsl_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 class ADSLData:
     type = 'adsl'
 
     def __init__(
-        self, order_id, phone_number, iban,
+        self, order_id, phone_number, iban, email,
         landline_phone_number, service_address, service_city, service_zip,
         service_subdivision, service_subdivision_code, shipment_address, shipment_city, shipment_zip,
         shipment_subdivision, previous_service, previous_provider, previous_internal_provider,
         previous_owner_vat, previous_owner_name, previous_owner_surname, notes,
             adsl_coverage, mm_fiber_coverage, vdf_fiber_coverage, change_address, product):
         # Common all the Tickets
         self.order_id = order_id
         self.phone_number = phone_number
         self.iban = iban
+        self.email = email
         self.previous_provider = previous_provider
         self.previous_internal_provider = previous_internal_provider
         self.previous_owner_vat = previous_owner_vat
         self.previous_owner_name = previous_owner_name
         self.previous_owner_surname = previous_owner_surname
 
         # Common Internet the Tickets
```

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/mobile_data.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/mobile_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 class MobileData:
     type = 'mobile'
 
     def __init__(
-        self, order_id, phone_number, iban, sc_icc, icc,
+        self, order_id, phone_number, iban, email, sc_icc, icc,
         portability, previous_owner_vat,
             previous_owner_name, previous_owner_surname, previous_provider, product):
         self.order_id = order_id
         self.phone_number = phone_number
         self.iban = iban
+        self.email = email
         self.sc_icc = sc_icc
         self.icc = icc
         self.portability = portability
         self.previous_provider = previous_provider
         self.previous_owner_vat = previous_owner_vat
         self.previous_owner_name = previous_owner_name
         self.previous_owner_surname = previous_owner_surname
```

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/otrs_models/vf_provisioning_article.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/otrs_models/vf_provisioning_article.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/responses/ticket_creation.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/responses/ticket_creation.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/exceptions.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/exceptions.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/services/update_process_ticket_with_coverage_tickets_info_service.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/services/update_process_ticket_with_coverage_tickets_info_service.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/services/update_process_ticket_with_VF_provisioning.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/services/update_process_ticket_with_VF_provisioning.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio/services/update_ticket_with_provider_info.py` & `otrs_somconnexio-0.4.9/otrs_somconnexio/services/update_ticket_with_provider_info.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/PKG-INFO` & `otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otrs-somconnexio
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python package for Somconnexio data syncing in OTRS
 Home-page: https://gitlab.com/coopdevs/otrs_somconnexio
 Author: Coopdevs
 Author-email: info@coopdevs.org
 License: UNKNOWN
 Description: # Python 2.7/3.8 module to manage the SomConnexio's ERP integration with OTRS
```

### Comparing `otrs_somconnexio-0.4.8/otrs_somconnexio.egg-info/SOURCES.txt` & `otrs_somconnexio-0.4.9/otrs_somconnexio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/data/otrs_raw_responses.py` & `otrs_somconnexio-0.4.9/tests/data/otrs_raw_responses.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/user_management_client/test_user_management_response.py` & `otrs_somconnexio-0.4.9/tests/user_management_client/test_user_management_response.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/user_management_client/test_client.py` & `otrs_somconnexio-0.4.9/tests/user_management_client/test_client.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_fiber_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_fiber_ticket.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,19 @@
         service_data = Mock(spec=['order_id'])
 
         expected_ticket_arguments = {
             "Title": "Sol·licitud fiber {}".format(service_data.order_id),
             "Type": FiberTicketConfiguration.type,
             "Queue": FiberTicketConfiguration.queue,
             "State": FiberTicketConfiguration.state,
+            "SLA": FiberTicketConfiguration.SLA,
+            "Service": FiberTicketConfiguration.service,
             "Priority": FiberTicketConfiguration.priority,
             "CustomerUser": customer_data.id,
-            "CustomerID": customer_data.id
+            "CustomerID": customer_data.id,
         }
 
         FiberTicket(service_data, customer_data)._build_ticket()
         MockTicket.assert_called_with(expected_ticket_arguments)
 
     @patch('otrs_somconnexio.otrs_models.provision_ticket.ProvisionArticle')
     def test_build_article(self, MockInternetArticle):
@@ -55,23 +57,23 @@
         )
         mock_fiber_dynamic_fields.all.assert_called_once()
 
     @patch('otrs_somconnexio.otrs_models.provision_ticket.OTRSClient')
     def test_create(self, MockOTRSClient):
         customer_data = Mock(spec=[
             'id',
-            'email',
             'phone',
             'first_name',
             'name',
             'vat_number',
         ])
         service_data = Mock(spec=[
             'order_id',
             'iban',
+            'email',
             'previous_service',
             'phone_number',
             'previous_provider',
             'previous_owner_vat',
             'previous_owner_name',
             'previous_owner_surname',
             'service_address',
@@ -100,7 +102,10 @@
         ticket = FiberTicket(service_data, customer_data)
         ticket.create()
 
         mock_otrs_client.create_otrs_process_ticket.assert_called_once()
 
         self.assertEqual(ticket.id, 123)
         self.assertEqual(ticket.number, '#123')
+        self.assertEqual(ticket.otrs_configuration.type, "Petición")
+        self.assertEqual(ticket.otrs_configuration.SLA, "No pendent resposta")
+        self.assertEqual(ticket.otrs_configuration.service, "Banda Ancha::Fibra::Provisió Fibra")
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/process_ticket/test_mobile_process_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/process_ticket/test_mobile_process_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/process_ticket/test_internet_process_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/process_ticket/test_internet_process_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_adsl_dynamic_fields.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_adsl_dynamic_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 class ADSLDynamicFieldsTestCase(unittest.TestCase):
     def setUp(self):
         self.customer_data = Mock(spec=[
             'first_name',
             'name',
             'vat_number',
             'phone',
-            'email',
         ])
         self.service_data = Mock(spec=[
             'order_id',
             'iban',
+            'email',
             'phone_number',
             'landline_phone_number',
             'service_address',
             'service_city',
             'service_zip',
             'service_subdivision',
             'service_subdivision_code',
@@ -151,15 +151,15 @@
             self.adsl_otrs_activity_id
         ).all()
 
         dynamic_fields_dct = dynamic_fields_to_dct(dynamic_fields)
         self.assertEqual(dynamic_fields_dct["telefonContacte"], "666666666")
 
     def test_contact_email_field(self):
-        self.customer_data.email = "test@email.org"
+        self.service_data.email = "test@email.org"
 
         dynamic_fields = ADSLDynamicFields(
             self.service_data,
             self.customer_data,
             self.adsl_otrs_process_id,
             self.adsl_otrs_activity_id
         ).all()
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_service.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_service.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_vf_provisioning_article.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_vf_provisioning_article.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_mobile_data.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_mobile_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class MobileDataTestCase(unittest.TestCase):
 
     def test_init(self):
         mobile_data = MobileData(
             order_id=123,
             phone_number="666666666",
             iban="ES6621000418401234567891",
+            email="test@test.com",
             previous_provider="SC",
             previous_owner_vat="740227654G",
             previous_owner_name="name",
             previous_owner_surname="surname",
             portability=False,
             sc_icc="123456789",
             icc=None,
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_abstract_article.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_abstract_article.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/configuration/test_fiber_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/configuration/test_fiber_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/configuration/test_adsl_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/configuration/test_adsl_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/configuration/test_mobile_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/configuration/test_mobile_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_ticket_factory.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_ticket_factory.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_coverage_article.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_coverage_article.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_adsl_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_adsl_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         service_data = Mock(spec=['order_id'])
 
         expected_ticket_arguments = {
             "Title": "Sol·licitud adsl {}".format(service_data.order_id),
             "Type": ADSLTicketConfiguration.type,
             "Queue": ADSLTicketConfiguration.queue,
             "State": ADSLTicketConfiguration.state,
+            "SLA": False,
+            "Service": False,
             "Priority": ADSLTicketConfiguration.priority,
             "CustomerUser": customer_data.id,
             "CustomerID": customer_data.id
         }
 
         ADSLTicket(service_data, customer_data)._build_ticket()
         MockTicket.assert_called_with(expected_ticket_arguments)
@@ -55,23 +57,23 @@
         )
         mock_adsl_dynamic_fields.all.assert_called_once()
 
     @patch('otrs_somconnexio.otrs_models.provision_ticket.OTRSClient')
     def test_create(self, MockOTRSClient):
         customer_data = Mock(spec=[
             'id',
-            'email',
             'phone',
             'first_name',
             'name',
             'vat_number',
         ])
         service_data = Mock(spec=[
             'order_id',
             'iban',
+            'email',
             'previous_service',
             'phone_number',
             'previous_provider',
             'previous_owner_vat',
             'previous_owner_name',
             'previous_owner_surname',
             'service_address',
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_fiber_dynamic_fields.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_fiber_dynamic_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 class FiberDynamicFieldsTestCase(unittest.TestCase):
     def setUp(self):
         self.customer_data = Mock(spec=[
             'first_name',
             'name',
             'vat_number',
             'phone',
-            'email',
         ])
         self.service_data = Mock(spec=[
             'order_id',
             'iban',
+            'email',
             'phone_number',
             'service_address',
             'service_city',
             'service_zip',
             'service_subdivision',
             'service_subdivision_code',
             'shipment_address',
@@ -151,15 +151,15 @@
             self.adsl_otrs_activity_id
         ).all()
 
         dynamic_fields_dct = dynamic_fields_to_dct(dynamic_fields)
         self.assertEqual(dynamic_fields_dct["telefonContacte"], "666666666")
 
     def test_contact_email_field(self):
-        self.customer_data.email = "test@email.org"
+        self.service_data.email = "test@email.org"
 
         dynamic_fields = FiberDynamicFields(
             self.service_data,
             self.customer_data,
             self.adsl_otrs_process_id,
             self.adsl_otrs_activity_id
         ).all()
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_telecom_company.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_telecom_company.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_adsl_data.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_adsl_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class ADSLDataTestCase(unittest.TestCase):
 
     def test_init(self):
         adsl_data = ADSLData(
             order_id=123,
             phone_number="666666666",
             iban="ES6621000418401234567891",
+            email="test@test.com",
             previous_provider="SC",
             previous_internal_provider=None,
             previous_owner_vat="740227654G",
             previous_owner_name="name",
             previous_owner_surname="surname",
             service_address="address",
             service_city="city",
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_coverage_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_coverage_ticket.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_mobile_ticket.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_mobile_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,23 @@
     @patch('otrs_somconnexio.otrs_models.provision_ticket.Ticket')
     def test_build_ticket(self, MockTicket):
         mobile_data = Mock(spec=[
             'order_id'
         ])
         mobile_data.order_id = 123
 
-        customer_data = Mock(spec=[
-            'id',
-            'email',
-        ])
-        customer_data.email = 'contact@mail.com'
+        customer_data = Mock(spec=['id'])
 
         expected_ticket_arguments = {
             "Title": "Sol·licitud mobile {}".format(mobile_data.order_id),
             "Type": MobileTicketConfiguration.type,
             "Queue": MobileTicketConfiguration.queue,
             "State": MobileTicketConfiguration.state,
+            "SLA": False,
+            "Service": False,
             "Priority": MobileTicketConfiguration.priority,
             "CustomerUser": customer_data.id,
             "CustomerID": customer_data.id,
         }
 
         MobileTicket(mobile_data, customer_data)._build_ticket()
 
@@ -67,14 +65,15 @@
         mock_mobile_dynamic_fields.all.assert_called_once()
 
     @patch('otrs_somconnexio.otrs_models.provision_ticket.OTRSClient')
     def test_create(self, MockOTRSClient):
         mobile_data = Mock(spec=[
             'order_id',
             'iban',
+            'email',
             'phone_number',
             'sc_icc',
             'icc',
             'portability',
             'previous_provider',
             'previous_owner_vat',
             'previous_owner_name',
@@ -82,26 +81,24 @@
             'product',
         ])
         mobile_data.order_id = 4321
         mobile_data.portability = False
 
         customer_data = Mock(spec=[
             'id',
-            'email',
             'phone',
             'first_name',
             'name',
             'vat_number',
             'street',
             'city',
             'zip',
             'subdivision',
         ])
         customer_data.id = 1234
-        customer_data.email = 'contact@mail.coop'
 
         mock_otrs_client = Mock(spec=['create_otrs_process_ticket'])
         mock_otrs_client.create_otrs_process_ticket.return_value = Mock(MobileTicket, autospec=True)
         mock_otrs_client.create_otrs_process_ticket.return_value.id = 123
         mock_otrs_client.create_otrs_process_ticket.return_value.number = '#123'
         MockOTRSClient.return_value = mock_otrs_client
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_mobile_dynamic_fields.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_mobile_dynamic_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 
 
 class MobileDynamicFieldsTestCase(unittest.TestCase):
     def setUp(self):
         self.customer_data = Mock(spec=[
             'id',
             'vat_number',
-            'email',
             'phone',
             'name',
             'first_name',
             'street',
             'zip',
             'city',
             'subdivision',
         ])
         self.mobile_data = Mock(spec=[
             'order_id',
             'phone_number',
             'iban',
+            'email',
             'sc_icc',
             'icc',
             'service_internet_unlimited',
             'portability',
             'previous_owner_vat',
             'previous_owner_name',
             'previous_owner_surname',
@@ -185,15 +185,15 @@
             self.mobile_otrs_activity_id
         ).all()
 
         dynamic_fields_dct = dynamic_fields_to_dct(dynamic_fields)
         self.assertEqual(dynamic_fields_dct["IBAN"], "ES6621000418401234567891")
 
     def test_contact_email_field(self):
-        self.customer_data.email = "test@email.org"
+        self.mobile_data.email = "test@email.org"
 
         dynamic_fields = MobileDynamicFields(
             self.mobile_data,
             self.customer_data,
             self.mobile_otrs_process_id,
             self.mobile_otrs_activity_id
         ).all()
```

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_customer_user.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_customer_user.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/otrs_models/test_fiber_data.py` & `otrs_somconnexio-0.4.9/tests/otrs_models/test_fiber_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class FiberDataTestCase(unittest.TestCase):
 
     def test_init(self):
         fiber_data = FiberData(
             order_id=123,
             phone_number="666666666",
             iban="ES6621000418401234567891",
+            email="test@test.com",
             previous_provider="SC",
             previous_internal_provider=None,
             previous_owner_vat="740227654G",
             previous_owner_name="name",
             previous_owner_surname="surname",
             service_address="address",
             service_city="city",
```

### Comparing `otrs_somconnexio-0.4.8/tests/responses/test_ticket_creation.py` & `otrs_somconnexio-0.4.9/tests/responses/test_ticket_creation.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/integration/test_change_customer_language.py` & `otrs_somconnexio-0.4.9/tests/integration/test_change_customer_language.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/integration/test_ticket_factory.py` & `otrs_somconnexio-0.4.9/tests/integration/test_ticket_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     @patch('otrs_somconnexio.otrs_models.provision_ticket.OTRSClient')
     def test_create_mobile_ticket_factory(self, MockOTRSClient):
         mobile_data = Mock(spec=[
             'order_id',
             'type',
             'iban',
+            'email',
             'phone_number',
             'sc_icc',
             'icc',
             'portability',
             'previous_provider',
             'previous_owner_name',
             'previous_owner_surname',
@@ -26,15 +27,14 @@
             'product',
         ])
         customer_data = Mock(spec=[
             'id',
             'first_name',
             'name',
             'vat_number',
-            'email',
             'phone',
             'street',
             'city',
             'zip',
             'subdivision'])
 
         mobile_data.type = 'mobile'
@@ -57,14 +57,15 @@
 
     @patch('otrs_somconnexio.otrs_models.provision_ticket.OTRSClient')
     def test_create_adsl_ticket_factory(self, MockOTRSClient):
         service_data = Mock(spec=[
             'order_id',
             'type',
             'iban',
+            'email',
             'phone_number',
             'previous_provider',
             'previous_owner_name',
             'previous_owner_surname',
             'previous_owner_vat',
             'previous_service',
             'service_address',
@@ -81,15 +82,15 @@
             'mm_fiber_coverage',
             'vdf_fiber_coverage',
             'change_address',
             'landline_phone_number',
             'product',
             'previous_internal_provider',
         ])
-        customer_data = Mock(spec=['id', 'first_name', 'name', 'vat_number', 'email', 'phone'])
+        customer_data = Mock(spec=['id', 'first_name', 'name', 'vat_number', 'phone'])
 
         service_data.type = 'adsl'
 
         otrs_process_ticket = Mock(spec=['id'])
         otrs_process_ticket.id = 234
 
         mock_otrs_client = Mock(spec=['create_otrs_process_ticket'])
@@ -108,14 +109,15 @@
 
     @patch('otrs_somconnexio.otrs_models.provision_ticket.OTRSClient')
     def test_create_fiber_ticket_factory(self, MockOTRSClient):
         service_data = Mock(spec=[
             'order_id',
             'type',
             'iban',
+            'email',
             'phone_number',
             'previous_provider',
             'previous_owner_name',
             'previous_owner_surname',
             'previous_owner_vat',
             'previous_service',
             'service_address',
@@ -131,15 +133,15 @@
             'adsl_coverage',
             'mm_fiber_coverage',
             'vdf_fiber_coverage',
             'change_address',
             'product',
             'previous_internal_provider',
         ])
-        customer_data = Mock(spec=['id', 'first_name', 'name', 'vat_number', 'email', 'phone'])
+        customer_data = Mock(spec=['id', 'first_name', 'name', 'vat_number', 'phone'])
 
         service_data.type = 'fiber'
 
         otrs_process_ticket = Mock(spec=['id'])
         otrs_process_ticket.id = 234
 
         mock_otrs_client = Mock(spec=['create_otrs_process_ticket'])
```

### Comparing `otrs_somconnexio-0.4.8/tests/integration/test_update_ticket_with_coverage_data.py` & `otrs_somconnexio-0.4.9/tests/integration/test_update_ticket_with_coverage_data.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/services/test_mappint_services.py` & `otrs_somconnexio-0.4.9/tests/services/test_mappint_services.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/services/test_update_process_ticket_with_coverage_tickets_info_service.py` & `otrs_somconnexio-0.4.9/tests/services/test_update_process_ticket_with_coverage_tickets_info_service.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/services/test_update_process_ticket_with_VF_provisioning.py` & `otrs_somconnexio-0.4.9/tests/services/test_update_process_ticket_with_VF_provisioning.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/services/test_update_ticket_with_provider_info.py` & `otrs_somconnexio-0.4.9/tests/services/test_update_ticket_with_provider_info.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/tests/services/test_mapping_mobile_minutes.py` & `otrs_somconnexio-0.4.9/tests/services/test_mapping_mobile_minutes.py`

 * *Files identical despite different names*

### Comparing `otrs_somconnexio-0.4.8/setup.py` & `otrs_somconnexio-0.4.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     README = f.read()
 
 
-VERSION = '0.4.8'
+VERSION = '0.4.9'
 
 setup(
     name='otrs_somconnexio',
     version=VERSION,
     author='Coopdevs',
     author_email='info@coopdevs.org',
     url='https://gitlab.com/coopdevs/otrs_somconnexio',
```

